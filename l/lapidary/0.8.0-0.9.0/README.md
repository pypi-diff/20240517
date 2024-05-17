# Comparing `tmp/lapidary-0.8.0.tar.gz` & `tmp/lapidary-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapidary-0.8.0.tar", max compression
+gzip compressed data, was "lapidary-0.9.0.tar", max compression
```

## Comparing `lapidary-0.8.0.tar` & `lapidary-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,23 @@
--rw-r--r--   0        0        0      106 2022-12-15 10:14:24.170845 lapidary-0.8.0/Readme.md
--rw-r--r--   0        0        0      815 2023-01-02 14:36:51.900087 lapidary-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      143 2022-12-15 10:14:24.172769 lapidary-0.8.0/src/lapidary/runtime/__init__.py
--rw-r--r--   0        0        0     2728 2022-12-29 15:20:56.045557 lapidary-0.8.0/src/lapidary/runtime/_params.py
--rw-r--r--   0        0        0      482 2022-12-15 10:14:24.173508 lapidary-0.8.0/src/lapidary/runtime/absent.py
--rw-r--r--   0        0        0       86 2022-12-15 10:14:24.174119 lapidary-0.8.0/src/lapidary/runtime/auth/__init__.py
--rw-r--r--   0        0        0     1097 2022-12-15 10:14:24.174566 lapidary-0.8.0/src/lapidary/runtime/auth/api_key.py
--rw-r--r--   0        0        0      216 2022-12-15 10:14:24.174883 lapidary-0.8.0/src/lapidary/runtime/auth/common.py
--rw-r--r--   0        0        0      738 2023-01-01 21:58:09.881391 lapidary-0.8.0/src/lapidary/runtime/auth/http.py
--rw-r--r--   0        0        0     3009 2023-01-01 21:53:36.179933 lapidary-0.8.0/src/lapidary/runtime/client_base.py
--rw-r--r--   0        0        0       79 2022-12-15 10:14:24.176322 lapidary-0.8.0/src/lapidary/runtime/http_consts.py
--rw-r--r--   0        0        0     1561 2022-12-29 15:20:56.049782 lapidary-0.8.0/src/lapidary/runtime/load.py
--rw-r--r--   0        0        0      373 2022-12-15 10:14:24.177122 lapidary-0.8.0/src/lapidary/runtime/mime.py
--rw-r--r--   0        0        0      373 2022-12-29 15:20:56.051281 lapidary-0.8.0/src/lapidary/runtime/model/__init__.py
--rw-r--r--   0        0        0     1305 2023-01-01 21:47:18.802610 lapidary-0.8.0/src/lapidary/runtime/model/auth.py
--rw-r--r--   0        0        0      756 2022-12-29 15:20:56.053064 lapidary-0.8.0/src/lapidary/runtime/model/client.py
--rw-r--r--   0        0        0     2112 2022-12-29 15:20:56.053984 lapidary-0.8.0/src/lapidary/runtime/model/client_init.py
--rw-r--r--   0        0        0     1701 2022-12-30 13:15:20.319127 lapidary-0.8.0/src/lapidary/runtime/model/op.py
--rw-r--r--   0        0        0      318 2022-12-15 10:14:24.180327 lapidary-0.8.0/src/lapidary/runtime/model/params.py
--rw-r--r--   0        0        0      451 2022-12-29 15:20:56.055226 lapidary-0.8.0/src/lapidary/runtime/model/plugins.py
--rw-r--r--   0        0        0     2484 2022-12-29 15:20:56.055858 lapidary-0.8.0/src/lapidary/runtime/model/refs.py
--rw-r--r--   0        0        0     2841 2022-12-30 13:15:30.380537 lapidary-0.8.0/src/lapidary/runtime/model/response_map.py
--rw-r--r--   0        0        0     8405 2022-12-29 15:20:56.057355 lapidary-0.8.0/src/lapidary/runtime/model/type_hint.py
--rw-r--r--   0        0        0     1404 2022-12-15 10:14:24.182315 lapidary-0.8.0/src/lapidary/runtime/module_path.py
--rw-r--r--   0        0        0     2528 2022-12-29 15:20:56.058092 lapidary-0.8.0/src/lapidary/runtime/names.py
--rw-r--r--   0        0        0       40 2022-12-29 15:20:56.058749 lapidary-0.8.0/src/lapidary/runtime/openapi/__init__.py
--rw-r--r--   0        0        0     3414 2023-01-01 21:45:48.735162 lapidary-0.8.0/src/lapidary/runtime/openapi/base.py
--rw-r--r--   0        0        0      810 2022-12-29 15:20:56.059444 lapidary-0.8.0/src/lapidary/runtime/openapi/ext.py
--rw-r--r--   0        0        0    16968 2023-01-01 22:10:14.147998 lapidary-0.8.0/src/lapidary/runtime/openapi/model.py
--rw-r--r--   0        0        0      492 2022-12-15 10:14:24.184357 lapidary-0.8.0/src/lapidary/runtime/openapi/utils.py
--rw-r--r--   0        0        0        0 2022-12-15 10:14:24.184486 lapidary-0.8.0/src/lapidary/runtime/py.typed
--rw-r--r--   0        0        0      278 2022-12-15 10:14:24.184784 lapidary-0.8.0/src/lapidary/runtime/pydantic_utils.py
--rw-r--r--   0        0        0     2340 2022-12-29 15:20:56.060675 lapidary-0.8.0/src/lapidary/runtime/request.py
--rw-r--r--   0        0        0     3779 2022-12-29 15:20:56.061213 lapidary-0.8.0/src/lapidary/runtime/response.py
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 lapidary-0.8.0/setup.py
--rw-r--r--   0        0        0     1009 1970-01-01 00:00:00.000000 lapidary-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1830 2024-05-17 06:45:47.938634 lapidary-0.9.0/Readme.md
+-rw-r--r--   0        0        0     1757 2024-05-17 06:45:47.938634 lapidary-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      641 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/__init__.py
+-rw-r--r--   0        0        0      419 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/_httpx.py
+-rw-r--r--   0        0        0      164 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/auth.py
+-rw-r--r--   0        0        0     5134 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/client_base.py
+-rw-r--r--   0        0        0       79 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/http_consts.py
+-rw-r--r--   0        0        0      397 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/mime.py
+-rw-r--r--   0        0        0      155 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/model/__init__.py
+-rw-r--r--   0        0        0      811 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/model/api_key.py
+-rw-r--r--   0        0        0     4803 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/model/encode_param.py
+-rw-r--r--   0        0        0     1938 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/model/op.py
+-rw-r--r--   0        0        0     4078 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/model/params.py
+-rw-r--r--   0        0        0     2194 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/model/request.py
+-rw-r--r--   0        0        0      274 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/model/response_map.py
+-rw-r--r--   0        0        0     1286 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/operation.py
+-rw-r--r--   0        0        0     1937 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/param.py
+-rw-r--r--   0        0        0        0 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/py.typed
+-rw-r--r--   0        0        0      238 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/pycompat.py
+-rw-r--r--   0        0        0     1039 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/request.py
+-rw-r--r--   0        0        0     1524 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/response.py
+-rw-r--r--   0        0        0      307 2024-05-17 06:45:47.938634 lapidary-0.9.0/src/lapidary/runtime/types_.py
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 lapidary-0.9.0/PKG-INFO
```

### Comparing `lapidary-0.8.0/src/lapidary/runtime/request.py` & `lapidary-0.9.0/src/lapidary/runtime/model/op.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,73 @@
-import enum
-import typing
-from typing import Optional, Any, Union
+import dataclasses as dc
+import inspect
 
 import httpx
-import pydantic
+import typing_extensions as typing
 
-from ._params import process_params
-from .http_consts import MIME_JSON, CONTENT_TYPE, ACCEPT
-from .mime import find_mime
-from .model import ResponseMap, ParamLocation
-from .pydantic_utils import to_model
-
-
-def get_accept_header(response_map: Optional[ResponseMap], global_response_map: Optional[ResponseMap]) -> Optional[str]:
-    all_mime_types = {
-        mime
-        for rmap in [response_map, global_response_map]
-        if rmap
-        for mime_map in rmap.values()
-        for mime in mime_map.keys()
-    }
-    return find_mime(all_mime_types, MIME_JSON)
-
-
-class RequestParts(typing.TypedDict):
-    content: Union[str, bytes, None]
-    params: Optional[httpx.QueryParams]
-    headers: Optional[httpx.Headers]
-    cookies: Optional[httpx.Cookies]
-
-
-def build_request(
-        param_model: Optional[pydantic.BaseModel],
-        request_body: Any,
-        response_map: Optional[ResponseMap],
-        global_response_map: Optional[ResponseMap],
-) -> RequestParts:
-    if param_model:
-        params, headers, cookies = process_params(param_model)
-    else:
-        params = cookies = None
-        headers = httpx.Headers()
-
-    if request_body is not None:
-        headers[CONTENT_TYPE] = MIME_JSON
-
-    if (accept := get_accept_header(response_map, global_response_map)) is not None:
-        headers[ACCEPT] = accept
-
-    if not isinstance(request_body, pydantic.BaseModel) and request_body is not None:
-        request_body = to_model(request_body)
-
-    content = (
-        request_body.json(by_alias=True, exclude_unset=True, exclude_defaults=True)
-        if request_body is not None
-        else None
+from ..response import find_type, parse_model
+from .params import ParameterAnnotation, RequestPartHandler, find_annotations, process_params
+from .response_map import ResponseMap, Responses
+
+if typing.TYPE_CHECKING:
+    from .request import RequestBuilder
+
+
+@dc.dataclass
+class OperationModel:
+    method: str
+    path: str
+    params: typing.Mapping[str, ParameterAnnotation]
+    response_map: ResponseMap
+
+    def process_params(
+        self,
+        actual_params: typing.Mapping[str, typing.Any],
+        request: 'RequestBuilder',
+    ) -> None:
+        for param_name, value in actual_params.items():
+            param_handler = self.params[param_name]
+            if isinstance(param_handler, RequestPartHandler):
+                param_handler.apply(request, actual_params[param_name])
+            else:
+                raise TypeError(param_name, type(value))
+
+    def handle_response(self, response: httpx.Response) -> typing.Any:
+        """
+        Possible special cases:
+        Exception
+        Auth
+        """
+
+        typ = find_type(response, self.response_map)
+
+        if typ is None:
+            return None
+
+        obj: typing.Any = parse_model(response, typ)
+
+        if isinstance(obj, Exception):
+            raise obj
+        else:
+            return obj
+
+
+def get_response_map(return_anno: type) -> ResponseMap:
+    annos = find_annotations(return_anno, Responses)
+    if len(annos) != 1:
+        raise TypeError('Operation function must have exactly one Responses annotation')
+
+    return annos[0].responses
+
+
+def get_operation_model(
+    method: str,
+    path: str,
+    fn: typing.Callable,
+) -> OperationModel:
+    sig = inspect.signature(fn)
+    return OperationModel(
+        method=method,
+        path=path,
+        params=process_params(sig),
+        response_map=get_response_map(sig.return_annotation),
     )
-
-    return dict(
-        content=content,
-        params=params,
-        headers=headers,
-        cookies=cookies
-    )
-
-
-def get_path(path_format: str, param_model: pydantic.BaseModel) -> str:
-    path_params = {
-        param_name: param_to_str(param_model.__dict__[param_name])
-        for param_name in param_model.__fields_set__
-        if param_model.__fields__[param_name].field_info.extra['in_'] is ParamLocation.path
-    } if param_model else {}
-    return path_format.format(**path_params)
-
-
-def param_to_str(value: Any) -> str:
-    if isinstance(value, enum.Enum):
-        return value.value
-    return str(value)
```

