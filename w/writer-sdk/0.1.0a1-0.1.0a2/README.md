# Comparing `tmp/writer_sdk-0.1.0a1.tar.gz` & `tmp/writer_sdk-0.1.0a2.tar.gz`

## Comparing `writer_sdk-0.1.0a1.tar` & `writer_sdk-0.1.0a2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/__init__.py
--rw-r--r--   0        0        0    64416 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_base_client.py
--rw-r--r--   0        0        0    16163 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_constants.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_qs.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_resource.py
--rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_response.py
--rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_streaming.py
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_types.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_utils/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/lib/.keep
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/resources/__init__.py
--rw-r--r--   0        0        0    13414 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/resources/chat.py
--rw-r--r--   0        0        0    14107 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/resources/completions.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/resources/models.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/types/__init__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/types/chat.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/types/chat_chat_params.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/types/chat_streaming_data.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/types/completion.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/types/completion_create_params.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/types/model_list_response.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer/types/streaming_data.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writer_ai/lib/.keep
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/src/writerai/lib/.keep
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/.gitignore
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/LICENSE
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0    13295 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writer/lib/.keep
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writer_ai/lib/.keep
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/__init__.py
+-rw-r--r--   0        0        0    64416 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_base_client.py
+-rw-r--r--   0        0        0    16163 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_constants.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_qs.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_resource.py
+-rw-r--r--   0        0        0    28383 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_response.py
+-rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_streaming.py
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_types.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_utils/__init__.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/lib/.keep
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/resources/__init__.py
+-rw-r--r--   0        0        0    13414 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/resources/chat.py
+-rw-r--r--   0        0        0    14107 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/resources/completions.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/resources/models.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/types/__init__.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/types/chat.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/types/chat_chat_params.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/types/chat_streaming_data.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/types/completion.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/types/completion_create_params.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/types/model_list_response.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/types/streaming_data.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/.gitignore
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/PKG-INFO
```

### Comparing `writer_sdk-0.1.0a1/src/writer/__init__.py` & `writer_sdk-0.1.0a2/src/writerai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,16 @@
 ]
 
 _setup_logging()
 
 # Update the __module__ attribute for exported symbols so that
 # error messages point to this module instead of the module
 # it was originally defined in, e.g.
-# writer._exceptions.NotFoundError -> writer.NotFoundError
+# writerai._exceptions.NotFoundError -> writerai.NotFoundError
 __locals = locals()
 for __name in __all__:
     if not __name.startswith("__"):
         try:
-            __locals[__name].__module__ = "writer"
+            __locals[__name].__module__ = "writerai"
         except (TypeError, AttributeError):
             # Some of our exported symbols are builtins which we can't set attributes for.
             pass
```

### Comparing `writer_sdk-0.1.0a1/src/writer/_base_client.py` & `writer_sdk-0.1.0a2/src/writerai/_base_client.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/_client.py` & `writer_sdk-0.1.0a2/src/writerai/_client.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/_compat.py` & `writer_sdk-0.1.0a2/src/writerai/_compat.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/_exceptions.py` & `writer_sdk-0.1.0a2/src/writerai/_exceptions.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/_files.py` & `writer_sdk-0.1.0a2/src/writerai/_files.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/_models.py` & `writer_sdk-0.1.0a2/src/writerai/_models.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/_qs.py` & `writer_sdk-0.1.0a2/src/writerai/_qs.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/_resource.py` & `writer_sdk-0.1.0a2/src/writerai/_resource.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/_response.py` & `writer_sdk-0.1.0a2/src/writerai/_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             # the response class ourselves but that is something that should be supported directly in httpx
             # as it would be easy to incorrectly construct the Response object due to the multitude of arguments.
             if cast_to != httpx.Response:
                 raise ValueError(f"Subclasses of httpx.Response cannot be passed to `cast_to`")
             return cast(R, response)
 
         if inspect.isclass(origin) and not issubclass(origin, BaseModel) and issubclass(origin, pydantic.BaseModel):
-            raise TypeError("Pydantic models must subclass our base model type, e.g. `from writer import BaseModel`")
+            raise TypeError("Pydantic models must subclass our base model type, e.g. `from writerai import BaseModel`")
 
         if (
             cast_to is not object
             and not origin is list
             and not origin is dict
             and not origin is Union
             and not issubclass(origin, BaseModel)
@@ -267,15 +267,15 @@
 
         For lower-level control, see `.read()`, `.json()`, `.iter_bytes()`.
 
         You can customise the type that the response is parsed into through
         the `to` argument, e.g.
 
         ```py
-        from writer import BaseModel
+        from writerai import BaseModel
 
 
         class MyModel(BaseModel):
             foo: str
 
 
         obj = response.parse(to=MyModel)
@@ -371,15 +371,15 @@
 
         For lower-level control, see `.read()`, `.json()`, `.iter_bytes()`.
 
         You can customise the type that the response is parsed into through
         the `to` argument, e.g.
 
         ```py
-        from writer import BaseModel
+        from writerai import BaseModel
 
 
         class MyModel(BaseModel):
             foo: str
 
 
         obj = response.parse(to=MyModel)
@@ -542,15 +542,15 @@
             async for data in self.iter_bytes(chunk_size):
                 await f.write(data)
 
 
 class MissingStreamClassError(TypeError):
     def __init__(self) -> None:
         super().__init__(
-            "The `stream` argument was set to `True` but the `stream_cls` argument was not given. See `writer._streaming` for reference",
+            "The `stream` argument was set to `True` but the `stream_cls` argument was not given. See `writerai._streaming` for reference",
         )
 
 
 class StreamAlreadyConsumed(WriterError):
     """
     Attempted to read or stream content, but the content has already
     been streamed.
```

### Comparing `writer_sdk-0.1.0a1/src/writer/_streaming.py` & `writer_sdk-0.1.0a2/src/writerai/_streaming.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/_types.py` & `writer_sdk-0.1.0a2/src/writerai/_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 # method that uses `ResponseT` which would lead to an unacceptable
 # amount of code duplication and make it unreadable. See _base_client.py
 # for example usage.
 #
 # This unfortunately means that you will either have
 # to import this type and pass it explicitly:
 #
-# from writer import NoneType
+# from writerai import NoneType
 # client.get('/foo', cast_to=NoneType)
 #
 # or build it yourself:
 #
 # client.get('/foo', cast_to=type(None))
 if TYPE_CHECKING:
     NoneType: Type[None]
```

### Comparing `writer_sdk-0.1.0a1/src/writer/_utils/__init__.py` & `writer_sdk-0.1.0a2/src/writerai/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/_utils/_logs.py` & `writer_sdk-0.1.0a2/src/writerai/_utils/_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import logging
 
-logger: logging.Logger = logging.getLogger("writer")
+logger: logging.Logger = logging.getLogger("writerai")
 httpx_logger: logging.Logger = logging.getLogger("httpx")
 
 
 def _basic_config() -> None:
-    # e.g. [2023-10-05 14:12:26 - writer._base_client:818 - DEBUG] HTTP Request: POST http://127.0.0.1:4010/foo/bar "200 OK"
+    # e.g. [2023-10-05 14:12:26 - writerai._base_client:818 - DEBUG] HTTP Request: POST http://127.0.0.1:4010/foo/bar "200 OK"
     logging.basicConfig(
         format="[%(asctime)s - %(name)s:%(lineno)d - %(levelname)s] %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
 
 def setup_logging() -> None:
```

### Comparing `writer_sdk-0.1.0a1/src/writer/_utils/_proxy.py` & `writer_sdk-0.1.0a2/src/writerai/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/_utils/_sync.py` & `writer_sdk-0.1.0a2/src/writerai/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/_utils/_transform.py` & `writer_sdk-0.1.0a2/src/writerai/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/_utils/_typing.py` & `writer_sdk-0.1.0a2/src/writerai/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/_utils/_utils.py` & `writer_sdk-0.1.0a2/src/writerai/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/resources/__init__.py` & `writer_sdk-0.1.0a2/src/writerai/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/resources/chat.py` & `writer_sdk-0.1.0a2/src/writerai/resources/chat.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/resources/completions.py` & `writer_sdk-0.1.0a2/src/writerai/resources/completions.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/resources/models.py` & `writer_sdk-0.1.0a2/src/writerai/resources/models.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/types/__init__.py` & `writer_sdk-0.1.0a2/src/writerai/types/__init__.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/types/chat.py` & `writer_sdk-0.1.0a2/src/writerai/types/chat.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/types/chat_chat_params.py` & `writer_sdk-0.1.0a2/src/writerai/types/chat_chat_params.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/types/completion.py` & `writer_sdk-0.1.0a2/src/writerai/types/completion.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/src/writer/types/completion_create_params.py` & `writer_sdk-0.1.0a2/src/writerai/types/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/LICENSE` & `writer_sdk-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a1/pyproject.toml` & `writer_sdk-0.1.0a2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "writer-sdk"
-version = "0.1.0-alpha.1"
+version = "0.1.0-alpha.2"
 description = "The official Python library for the writer API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Writer", email = "dev-feedback@writer.com" },
 ]
 dependencies = [
@@ -80,28 +80,28 @@
 "fix:ruff" = "ruff --fix ."
 
 typecheck = { chain = [
   "typecheck:pyright",
   "typecheck:mypy"
 ]}
 "typecheck:pyright" = "pyright"
-"typecheck:verify-types" = "pyright --verifytypes writer --ignoreexternal"
+"typecheck:verify-types" = "pyright --verifytypes writerai --ignoreexternal"
 "typecheck:mypy" = "mypy ."
 
 [build-system]
 requires = ["hatchling", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 include = [
   "src/*"
 ]
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/writer"]
+packages = ["src/writerai"]
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
 
@@ -183,14 +183,14 @@
 "functools.lru_cache".msg = "This function does not retain type information for the wrapped function's arguments; The `lru_cache` function from `_utils` should be used instead"
 
 [tool.ruff.lint.isort]
 length-sort = true
 length-sort-straight = true
 combine-as-imports = true
 extra-standard-library = ["typing_extensions"]
-known-first-party = ["writer", "tests"]
+known-first-party = ["writerai", "tests"]
 
 [tool.ruff.per-file-ignores]
 "bin/**.py" = ["T201", "T203"]
 "scripts/**.py" = ["T201", "T203"]
 "tests/**.py" = ["T201", "T203"]
 "examples/**.py" = ["T201", "T203"]
```

### Comparing `writer_sdk-0.1.0a1/PKG-INFO` & `writer_sdk-0.1.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: writer-sdk
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: The official Python library for the writer API
 Project-URL: Homepage, https://github.com/WriterColab/sdk.python
 Project-URL: Repository, https://github.com/WriterColab/sdk.python
 Author-email: Writer <dev-feedback@writer.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -55,15 +55,15 @@
 
 ## Usage
 
 The full API of this library can be found in [api.md](https://github.com/WriterColab/sdk.python/tree/main/api.md).
 
 ```python
 import os
-from writer import Writer
+from writerai import Writer
 
 client = Writer(
     # This is the default and can be omitted
     api_key=os.environ.get("WRITER_API_KEY"),
 )
 
 chat = client.chat.chat(
@@ -86,15 +86,15 @@
 ## Async usage
 
 Simply import `AsyncWriter` instead of `Writer` and use `await` with each API call:
 
 ```python
 import os
 import asyncio
-from writer import AsyncWriter
+from writerai import AsyncWriter
 
 client = AsyncWriter(
     # This is the default and can be omitted
     api_key=os.environ.get("WRITER_API_KEY"),
 )
 
 
@@ -117,15 +117,15 @@
 Functionality between the synchronous and asynchronous clients is otherwise identical.
 
 ## Streaming responses
 
 We provide support for streaming responses using Server Side Events (SSE).
 
 ```python
-from writer import Writer
+from writerai import Writer
 
 client = Writer()
 
 stream = client.completions.create(
     model="palmyra-x-v2",
     prompt="Hi, my name is",
     stream=True,
@@ -133,15 +133,15 @@
 for completion in stream:
     print(completion.choices)
 ```
 
 The async client uses the exact same interface.
 
 ```python
-from writer import AsyncWriter
+from writerai import AsyncWriter
 
 client = AsyncWriter()
 
 stream = await client.completions.create(
     model="palmyra-x-v2",
     prompt="Hi, my name is",
     stream=True,
@@ -157,43 +157,43 @@
 - Serializing back into JSON, `model.to_json()`
 - Converting to a dictionary, `model.to_dict()`
 
 Typed requests and responses provide autocomplete and documentation within your editor. If you would like to see type errors in VS Code to help catch bugs earlier, set `python.analysis.typeCheckingMode` to `basic`.
 
 ## Handling errors
 
-When the library is unable to connect to the API (for example, due to network connection problems or a timeout), a subclass of `writer.APIConnectionError` is raised.
+When the library is unable to connect to the API (for example, due to network connection problems or a timeout), a subclass of `writerai.APIConnectionError` is raised.
 
 When the API returns a non-success status code (that is, 4xx or 5xx
-response), a subclass of `writer.APIStatusError` is raised, containing `status_code` and `response` properties.
+response), a subclass of `writerai.APIStatusError` is raised, containing `status_code` and `response` properties.
 
-All errors inherit from `writer.APIError`.
+All errors inherit from `writerai.APIError`.
 
 ```python
-import writer
-from writer import Writer
+import writerai
+from writerai import Writer
 
 client = Writer()
 
 try:
     client.chat.chat(
         messages=[
             {
                 "content": "Hello!",
                 "role": "user",
             }
         ],
         model="palmyra-x-chat-v2-32k",
     )
-except writer.APIConnectionError as e:
+except writerai.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
-except writer.RateLimitError as e:
+except writerai.RateLimitError as e:
     print("A 429 status code was received; we should back off a bit.")
-except writer.APIStatusError as e:
+except writerai.APIStatusError as e:
     print("Another non-200-range status code was received")
     print(e.status_code)
     print(e.response)
 ```
 
 Error codes are as followed:
 
@@ -213,15 +213,15 @@
 Certain errors are automatically retried 2 times by default, with a short exponential backoff.
 Connection errors (for example, due to a network connectivity problem), 408 Request Timeout, 409 Conflict,
 429 Rate Limit, and >=500 Internal errors are all retried by default.
 
 You can use the `max_retries` option to configure or disable retry settings:
 
 ```python
-from writer import Writer
+from writerai import Writer
 
 # Configure the default for all requests:
 client = Writer(
     # default is 2
     max_retries=0,
 )
 
@@ -239,15 +239,15 @@
 
 ### Timeouts
 
 By default requests time out after 1 minute. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration) object:
 
 ```python
-from writer import Writer
+from writerai import Writer
 
 # Configure the default for all requests:
 client = Writer(
     # 20 seconds (default is 1 minute)
     timeout=20.0,
 )
 
@@ -297,15 +297,15 @@
 ```
 
 ### Accessing raw response data (e.g. headers)
 
 The "raw" Response object can be accessed by prefixing `.with_raw_response.` to any HTTP method call, e.g.,
 
 ```py
-from writer import Writer
+from writerai import Writer
 
 client = Writer()
 response = client.chat.with_raw_response.chat(
     messages=[{
         "content": "Hello!",
         "role": "user",
     }],
@@ -313,17 +313,17 @@
 )
 print(response.headers.get('X-My-Header'))
 
 chat = response.parse()  # get the object that `chat.chat()` would have returned
 print(chat.id)
 ```
 
-These methods return an [`APIResponse`](https://github.com/WriterColab/sdk.python/tree/main/src/writer/_response.py) object.
+These methods return an [`APIResponse`](https://github.com/WriterColab/sdk.python/tree/main/src/writerai/_response.py) object.
 
-The async client returns an [`AsyncAPIResponse`](https://github.com/WriterColab/sdk.python/tree/main/src/writer/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
+The async client returns an [`AsyncAPIResponse`](https://github.com/WriterColab/sdk.python/tree/main/src/writerai/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
 
 #### `.with_streaming_response`
 
 The above interface eagerly reads the full response body when you make the request, which may not always be what you want.
 
 To stream the response body, use `.with_streaming_response` instead, which requires a context manager and only reads the response body once you call `.read()`, `.text()`, `.json()`, `.iter_bytes()`, `.iter_text()`, `.iter_lines()` or `.parse()`. In the async client, these are async methods.
 
@@ -385,15 +385,15 @@
 You can directly override the [httpx client](https://www.python-httpx.org/api/#client) to customize it for your use case, including:
 
 - Support for proxies
 - Custom transports
 - Additional [advanced](https://www.python-httpx.org/advanced/#client-instances) functionality
 
 ```python
-from writer import Writer, DefaultHttpxClient
+from writerai import Writer, DefaultHttpxClient
 
 client = Writer(
     # Or use the `WRITER_BASE_URL` env var
     base_url="http://my.test.server.example.com:8083",
     http_client=DefaultHttpxClient(
         proxies="http://my.test.proxy.example.com",
         transport=httpx.HTTPTransport(local_address="0.0.0.0"),
```

