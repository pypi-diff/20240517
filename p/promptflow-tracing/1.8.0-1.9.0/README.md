# Comparing `tmp/promptflow_tracing-1.8.0-py3-none-any.whl.zip` & `tmp/promptflow_tracing-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 21795 bytes, number of entries: 18
+Zip file size: 22988 bytes, number of entries: 18
 -rw-r--r--  2.0 unx      412 b- defN 80-Jan-01 00:00 promptflow/tracing/__init__.py
--rw-r--r--  2.0 unx      400 b- defN 80-Jan-01 00:00 promptflow/tracing/_constants.py
+-rw-r--r--  2.0 unx      451 b- defN 80-Jan-01 00:00 promptflow/tracing/_constants.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 promptflow/tracing/_integrations/__init__.py
 -rw-r--r--  2.0 unx     8399 b- defN 80-Jan-01 00:00 promptflow/tracing/_integrations/_openai_injector.py
 -rw-r--r--  2.0 unx    10353 b- defN 80-Jan-01 00:00 promptflow/tracing/_openai_utils.py
 -rw-r--r--  2.0 unx     7470 b- defN 80-Jan-01 00:00 promptflow/tracing/_operation_context.py
--rw-r--r--  2.0 unx     3500 b- defN 80-Jan-01 00:00 promptflow/tracing/_start_trace.py
+-rw-r--r--  2.0 unx     7658 b- defN 80-Jan-01 00:00 promptflow/tracing/_start_trace.py
 -rw-r--r--  2.0 unx     1138 b- defN 80-Jan-01 00:00 promptflow/tracing/_thread_local_singleton.py
--rw-r--r--  2.0 unx    18907 b- defN 80-Jan-01 00:00 promptflow/tracing/_trace.py
--rw-r--r--  2.0 unx     7297 b- defN 80-Jan-01 00:00 promptflow/tracing/_tracer.py
+-rw-r--r--  2.0 unx    18929 b- defN 80-Jan-01 00:00 promptflow/tracing/_trace.py
+-rw-r--r--  2.0 unx     7460 b- defN 80-Jan-01 00:00 promptflow/tracing/_tracer.py
 -rw-r--r--  2.0 unx     3372 b- defN 80-Jan-01 00:00 promptflow/tracing/_utils.py
 -rw-r--r--  2.0 unx      299 b- defN 80-Jan-01 00:00 promptflow/tracing/_version.py
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 promptflow/tracing/contracts/__init__.py
 -rw-r--r--  2.0 unx      696 b- defN 80-Jan-01 00:00 promptflow/tracing/contracts/generator_proxy.py
 -rw-r--r--  2.0 unx     2091 b- defN 80-Jan-01 00:00 promptflow/tracing/contracts/trace.py
--rw-r--r--  2.0 unx     2227 b- defN 80-Jan-01 00:00 promptflow_tracing-1.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 promptflow_tracing-1.8.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1639 b- defN 16-Jan-01 00:00 promptflow_tracing-1.8.0.dist-info/RECORD
-18 files, 68550 bytes uncompressed, 19055 bytes compressed:  72.2%
+-rw-r--r--  2.0 unx     2227 b- defN 80-Jan-01 00:00 promptflow_tracing-1.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 promptflow_tracing-1.9.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1639 b- defN 16-Jan-01 00:00 promptflow_tracing-1.9.0.dist-info/RECORD
+18 files, 72944 bytes uncompressed, 20248 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -39,17 +39,17 @@
 
 Filename: promptflow/tracing/contracts/generator_proxy.py
 Comment: 
 
 Filename: promptflow/tracing/contracts/trace.py
 Comment: 
 
-Filename: promptflow_tracing-1.8.0.dist-info/METADATA
+Filename: promptflow_tracing-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: promptflow_tracing-1.8.0.dist-info/WHEEL
+Filename: promptflow_tracing-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: promptflow_tracing-1.8.0.dist-info/RECORD
+Filename: promptflow_tracing-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## promptflow/tracing/_constants.py

```diff
@@ -5,9 +5,10 @@
 
 class ResourceAttributesFieldName:
     SERVICE_NAME = "service.name"
     COLLECTION = "collection"
 
 
 RESOURCE_ATTRIBUTES_SERVICE_NAME = "promptflow"
+RESOURCE_ATTRIBUTES_COLLECTION_DEFAULT = "default"
 
 PF_TRACING_SKIP_LOCAL_SETUP_ENVIRON = "PF_TRACING_SKIP_LOCAL_SETUP"
```

## promptflow/tracing/_start_trace.py

```diff
@@ -1,109 +1,179 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
+import importlib.metadata
+import inspect
+import logging
 import os
 import typing
 
 from opentelemetry import trace
 from opentelemetry.sdk.environment_variables import OTEL_EXPORTER_OTLP_ENDPOINT
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 
 from ._constants import (
     PF_TRACING_SKIP_LOCAL_SETUP_ENVIRON,
+    RESOURCE_ATTRIBUTES_COLLECTION_DEFAULT,
     RESOURCE_ATTRIBUTES_SERVICE_NAME,
     ResourceAttributesFieldName,
 )
 from ._integrations._openai_injector import inject_openai_api
 
+TRACER_PROVIDER_PROTECTED_COLLECTION_ATTR = "_protected_collection"
+
 
 def start_trace(
     *,
     resource_attributes: typing.Optional[dict] = None,
     collection: typing.Optional[str] = None,
     **kwargs,
 ):
     """Promptflow instrumentation.
 
-    Instrument `openai`, and set tracer provider for current process.
-
     :param resource_attributes: Specify the resource attributes for current process.
     :type resource_attributes: typing.Optional[dict]
     :param collection: Specify the collection for current tracing.
     :type collection: typing.Optional[str]
     """
 
     # When PF_TRACING_SKIP_LOCAL_SETUP_ENVIRON is set to true, the start_trace should be skipped.
     # An example is that user call start_trace at cloud mode. Nothing should happen.
     if _skip_tracing_local_setup():
+        logging.info("skip tracing local setup as the environment variable is set.")
         return
 
     # prepare resource.attributes and set tracer provider
     res_attrs = {ResourceAttributesFieldName.SERVICE_NAME: RESOURCE_ATTRIBUTES_SERVICE_NAME}
-    if collection is not None:
-        res_attrs[ResourceAttributesFieldName.COLLECTION] = collection
     if isinstance(resource_attributes, dict):
+        logging.debug("specified resource attributes: %s", resource_attributes)
         for attr_key, attr_value in resource_attributes.items():
             res_attrs[attr_key] = attr_value
-    _set_tracer_provider(res_attrs)
+
+    # determine collection
+    collection_user_specified = collection is not None
+    if not collection_user_specified:
+        logging.debug("collection is not user specified")
+        if is_collection_writeable():
+            # internal parameter for devkit call
+            _collection = kwargs.get("_collection", None)
+            if _collection is not None:
+                logging.debug("received internal parameter _collection: %s, will use this", _collection)
+                collection = _collection
+            else:
+                logging.debug("trying to get from current working directory...")
+                collection = _get_collection_from_cwd()
+        else:
+            logging.debug("collection is protected, will directly use that...")
+            tracer_provider: TracerProvider = trace.get_tracer_provider()
+            collection = tracer_provider.resource.attributes[ResourceAttributesFieldName.COLLECTION]
+    logging.info("collection: %s", collection)
+    res_attrs[ResourceAttributesFieldName.COLLECTION] = collection
+    logging.info("resource attributes: %s", res_attrs)
+
+    # if user specifies collection, we will add a flag on tracer provider to avoid override
+    _set_tracer_provider(res_attrs, protected_collection=collection_user_specified)
 
     if _is_devkit_installed():
         from promptflow._sdk._tracing import start_trace_with_devkit
 
-        start_trace_with_devkit(
-            collection=collection,
-            attrs=kwargs.get("attributes", None),
-            run=kwargs.get("run", None),
-        )
+        logging.debug("promptflow-devkit is installed.")
 
+        # in promptflow-devkit<=1.8.0, `start_trace_with_devkit` cannot accept `**kwargs`
+        # so we need to handle this with function signature check, and warn user on this
+        if _kwargs_in_func(start_trace_with_devkit):
+            logging.debug("compatible promptflow-devkit version, will pass `collection` and `kwargs`...")
+            logging.debug("collection: %s", collection)
+            logging.debug("kwargs: %s", kwargs)
+            start_trace_with_devkit(collection=collection, **kwargs)
+        else:
+            warning_msg = (
+                "incompatible `promptflow-devkit` version installed, which may lead to unexpected behavior; "
+                "it is recommended to use 'promptflow-devkit>=1.9.0' for better trace experience."
+            )
+            logging.warning(warning_msg)
+            print(warning_msg)
+            logging.debug("will pass `collection`, `attributes`, and `run`...")
+            _attributes = kwargs.get("attributes", None)
+            _run = kwargs.get("run", None)
+            logging.debug("collection: %s", collection)
+            logging.debug("attributes: %s", _attributes)
+            logging.debug("run: %s", _run)
+            start_trace_with_devkit(collection=collection, attributes=_attributes, run=_run)
 
-def setup_exporter_from_environ() -> None:
 
+def setup_exporter_from_environ() -> None:
     # openai instrumentation
+    logging.debug("injecting OpenAI API...")
     inject_openai_api()
+    logging.debug("OpenAI API injected.")
 
     # Ignore all the setup if the endpoint is not set
     endpoint = os.getenv(OTEL_EXPORTER_OTLP_ENDPOINT)
+    logging.debug("environ OTEL_EXPORTER_OTLP_ENDPOINT: %s", endpoint)
     if not endpoint:
+        logging.info("environ OTEL_EXPORTER_OTLP_ENDPOINT is not set, will skip the following setup.")
         return
 
     if _is_devkit_installed():
         from promptflow._sdk._tracing import setup_exporter_to_pfs
 
+        logging.debug("promptflow-devkit is installed, will continue local setup...")
         setup_exporter_to_pfs()
 
 
 def _skip_tracing_local_setup() -> bool:
     return str(os.getenv(PF_TRACING_SKIP_LOCAL_SETUP_ENVIRON, "false")).lower() == "true"
 
 
-def _is_tracer_provider_set() -> bool:
-    return isinstance(trace.get_tracer_provider(), TracerProvider)
-
-
-def _force_set_tracer_provider(tracer_provider: TracerProvider) -> None:
-    from opentelemetry.trace import _TRACER_PROVIDER_SET_ONCE
-
-    with _TRACER_PROVIDER_SET_ONCE._lock:
-        _TRACER_PROVIDER_SET_ONCE._done = False
-
-    trace.set_tracer_provider(tracer_provider)
+def _get_collection_from_cwd() -> str:
+    """Try to use cwd folder name as collection name; will fall back to default value if run into exception."""
+    cur_folder_name = ""
+    try:
+        cwd = os.getcwd()
+        cur_folder_name = os.path.basename(cwd)
+    except Exception:  # pylint: disable=broad-except
+        # possible exception: PermissionError, FileNotFoundError, OSError, etc.
+        pass
+    collection = cur_folder_name if cur_folder_name != "" else RESOURCE_ATTRIBUTES_COLLECTION_DEFAULT
+    return collection
 
 
-def _set_tracer_provider(res_attrs: typing.Dict[str, str]) -> None:
+def _set_tracer_provider(res_attrs: typing.Dict[str, str], protected_collection: bool) -> None:
     res = Resource(attributes=res_attrs)
     tracer_provider = TracerProvider(resource=res)
-    if _is_tracer_provider_set():
-        _force_set_tracer_provider(tracer_provider)
+
+    cur_tracer_provider = trace.get_tracer_provider()
+    if isinstance(cur_tracer_provider, TracerProvider):
+        logging.info("tracer provider is already set, will merge the resource attributes...")
+        cur_res = cur_tracer_provider.resource
+        logging.debug("current resource: %s", cur_res.attributes)
+        new_res = cur_res.merge(res)
+        cur_tracer_provider._resource = new_res
+        logging.info("tracer provider is updated with resource attributes: %s", new_res.attributes)
     else:
         trace.set_tracer_provider(tracer_provider)
+        logging.info("tracer provider is set with resource attributes: %s", res.attributes)
+
+    if protected_collection:
+        logging.info("user specifies collection, will add a flag on tracer provider to avoid override...")
+        setattr(trace.get_tracer_provider(), TRACER_PROVIDER_PROTECTED_COLLECTION_ATTR, True)
+
+
+def is_collection_writeable() -> bool:
+    return not getattr(trace.get_tracer_provider(), TRACER_PROVIDER_PROTECTED_COLLECTION_ATTR, False)
 
 
 def _is_devkit_installed() -> bool:
     try:
-        from promptflow._sdk._tracing import setup_exporter_to_pfs, start_trace_with_devkit  # noqa: F401
-
+        importlib.metadata.version("promptflow-devkit")
         return True
-    except ImportError:
+    except importlib.metadata.PackageNotFoundError:
         return False
+
+
+def _kwargs_in_func(func: typing.Callable) -> bool:
+    signature = inspect.signature(func)
+    params = signature.parameters.values()
+    return any(param.kind == param.VAR_KEYWORD for param in params)
```

## promptflow/tracing/_trace.py

```diff
@@ -278,30 +278,30 @@
             return json.dumps(serialized_value, indent=2)
     except Exception as e:
         logging.warning(f"Failed to serialize attribute: {e}")
         return None
 
 
 def _traced(
-    func: Callable = None, *, args_to_ignore: Optional[List[str]] = None, trace_type=TraceType.FUNCTION
+    func: Callable = None, *, args_to_ignore: Optional[List[str]] = None, trace_type=TraceType.FUNCTION, name=None
 ) -> Callable:
     """
     Decorator that adds tracing to a function.
 
     Args:
         func (Callable): The function to be traced.
         args_to_ignore (Optional[List[str]], optional): A list of argument names to be ignored in the trace.
                                                         Defaults to None.
         trace_type (TraceType, optional): The type of the trace. Defaults to TraceType.FUNCTION.
 
     Returns:
         Callable: The traced function.
     """
     wrapped_method = _traced_async if inspect.iscoroutinefunction(func) else _traced_sync
-    return wrapped_method(func, args_to_ignore=args_to_ignore, trace_type=trace_type)
+    return wrapped_method(func, args_to_ignore=args_to_ignore, trace_type=trace_type, name=name)
 
 
 def _traced_async(
     func: Callable = None,
     *,
     args_to_ignore: Optional[List[str]] = None,
     trace_type=TraceType.FUNCTION,
```

## promptflow/tracing/_tracer.py

```diff
@@ -133,15 +133,21 @@
         return {
             "message": str(error),
             "type": type(error).__qualname__,
         }
 
 
 def _create_trace_from_function_call(
-    f, *, args=None, kwargs=None, args_to_ignore: Optional[List[str]] = None, trace_type=TraceType.FUNCTION, name=None,
+    f,
+    *,
+    args=None,
+    kwargs=None,
+    args_to_ignore: Optional[List[str]] = None,
+    trace_type=TraceType.FUNCTION,
+    name=None,
 ):
     """
     Creates a trace object from a function call.
 
     Args:
         f (Callable): The function to be traced.
         args (list, optional): The positional arguments to the function. Defaults to None.
@@ -173,15 +179,19 @@
         pass
 
     # TODO: put parameters in self to inputs for builtin tools
     all_kwargs.pop("self", None)
     for key in args_to_ignore:
         all_kwargs.pop(key, None)
 
-    function = f.__qualname__
+    if hasattr(f, "__qualname__"):
+        function = f.__qualname__
+    else:
+        # Get __qualname__ from callable class
+        function = f.__call__.__qualname__
     if trace_type in [TraceType.LLM, TraceType.EMBEDDING] and f.__module__:
         function = f"{f.__module__}.{function}"
 
     return Trace(
         name=name or function,  # Use the function name as the trace name if not provided
         type=trace_type,
         start_time=datetime.utcnow().timestamp(),
```

## Comparing `promptflow_tracing-1.8.0.dist-info/METADATA` & `promptflow_tracing-1.9.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptflow-tracing
-Version: 1.8.0
+Version: 1.9.0
 Summary: Prompt flow tracing
 Home-page: https://microsoft.github.io/promptflow/
 License: MIT
 Keywords: telemetry
 Author: Microsoft Corporation
 Author-email: aml-pt-eng@microsoft.com
 Requires-Python: >=3.8,<4.0
```

## Comparing `promptflow_tracing-1.8.0.dist-info/RECORD` & `promptflow_tracing-1.9.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 promptflow/tracing/__init__.py,sha256=2RELQpoR4iNv5RbG3ThHKY_a6snK9m0amicO4iT2K4g,412
-promptflow/tracing/_constants.py,sha256=N3eGPmPv84Opjvg-FEm9KFR-a0WPugD1qHA_onWw5GQ,400
+promptflow/tracing/_constants.py,sha256=ZQz-khncuHJgi51dLNvnJKbJtR3pGHSBVlVf1DJXKRk,451
 promptflow/tracing/_integrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 promptflow/tracing/_integrations/_openai_injector.py,sha256=Ivtl_WKqIqA2_GbR_VSqty-5FhVrwYf9IzpW07kk4fQ,8399
 promptflow/tracing/_openai_utils.py,sha256=-2L9tCJ3Hvhr75akFuhL264qFeWpynRrx2nX9FOQa68,10353
 promptflow/tracing/_operation_context.py,sha256=bYqAoamY3kiz2JHR23uxhVAP1pS1F_3ULwfRFuQav3g,7470
-promptflow/tracing/_start_trace.py,sha256=r8rWLt3kjilAkqaAJ1wfVlfoRhOjlsfsVM2CmcTwl4g,3500
+promptflow/tracing/_start_trace.py,sha256=G2iesX8PA4S2A7nezSO4BklVO7KyghTJWlNzdcu-cDk,7658
 promptflow/tracing/_thread_local_singleton.py,sha256=JPTGjbpG1LpMEUh-fqgXDz3-It5zlI3R1db4bHrIH4Y,1138
-promptflow/tracing/_trace.py,sha256=r7vNqAtqg5y7-Fic6J_-PjN62upt0_2TO_H6UjN0-_g,18907
-promptflow/tracing/_tracer.py,sha256=wy_W-X4ikkst2nMANKSGwojK9ywvd82OMEZ-GNC9QDA,7297
+promptflow/tracing/_trace.py,sha256=WXDpe8gT8i70ZDdzaacdw1l50h1EWgrmmDQYgysh7HY,18929
+promptflow/tracing/_tracer.py,sha256=rba5KIW5FEDI1BgJgWjfr9ktPGsDjZAioKWpE8XDqfk,7460
 promptflow/tracing/_utils.py,sha256=sZrYjG-3YgxSMVZGRWF0KHz-vRMSBKIrk9REfmTGnFo,3372
 promptflow/tracing/_version.py,sha256=v7XN-ZZdY9fb-B9aAIoxmqWjMrrkdEPiOIDdEx3nOEc,299
 promptflow/tracing/contracts/__init__.py,sha256=vV8bhHRJHrJVbMOhR8jvnWF0_ZwCRQiSsUwf0X04gtg,262
 promptflow/tracing/contracts/generator_proxy.py,sha256=0vrOocScGwAwuEAimqMNbATCH_F6Iz-iMN6KhJnMosA,696
 promptflow/tracing/contracts/trace.py,sha256=ZBcMYUbfmOdeXufvTH5x-phAa4BziGLjBxNrjzLYUTo,2091
-promptflow_tracing-1.8.0.dist-info/METADATA,sha256=ittFCEp7zYBYsXa-iWybqoXS7gI46xnVGhdF7H7mH2g,2227
-promptflow_tracing-1.8.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-promptflow_tracing-1.8.0.dist-info/RECORD,,
+promptflow_tracing-1.9.0.dist-info/METADATA,sha256=O-Ny0qdxZR08BSh-jUumwFeo92xP-TNtVbFnfyqCNVI,2227
+promptflow_tracing-1.9.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+promptflow_tracing-1.9.0.dist-info/RECORD,,
```

