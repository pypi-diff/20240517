# Comparing `tmp/pyview_web-0.0.8a0.tar.gz` & `tmp/pyview_web-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyview_web-0.0.8a0.tar", max compression
+gzip compressed data, was "pyview_web-0.0.9a0.tar", max compression
```

## Comparing `pyview_web-0.0.8a0.tar` & `pyview_web-0.0.9a0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1071 2023-05-02 00:38:29.733278 pyview_web-0.0.8a0/LICENSE
--rw-r--r--   0        0        0     2032 2024-05-15 00:40:24.073292 pyview_web-0.0.8a0/pyproject.toml
--rw-r--r--   0        0        0      223 2023-06-02 16:20:26.327598 pyview_web-0.0.8a0/pyview/__init__.py
--rw-r--r--   0        0        0     2508 2023-05-02 00:38:29.742232 pyview_web-0.0.8a0/pyview/assets/js/app.js
--rw-r--r--   0        0        0     2425 2023-05-02 00:38:29.742415 pyview_web-0.0.8a0/pyview/assets/package-lock.json
--rw-r--r--   0        0        0      151 2023-05-02 00:38:29.742554 pyview_web-0.0.8a0/pyview/assets/package.json
--rw-r--r--   0        0        0      109 2023-06-14 00:18:12.775162 pyview_web-0.0.8a0/pyview/auth/__init__.py
--rw-r--r--   0        0        0      935 2023-06-14 00:18:12.775807 pyview_web-0.0.8a0/pyview/auth/provider.py
--rw-r--r--   0        0        0     1223 2023-06-14 00:18:12.776363 pyview_web-0.0.8a0/pyview/auth/required.py
--rw-r--r--   0        0        0       46 2023-05-02 00:38:29.742781 pyview_web-0.0.8a0/pyview/changesets/__init__.py
--rw-r--r--   0        0        0     1747 2023-05-02 00:38:29.743020 pyview_web-0.0.8a0/pyview/changesets/changesets.py
--rw-r--r--   0        0        0      789 2023-06-13 01:17:27.976763 pyview_web-0.0.8a0/pyview/csrf.py
--rw-r--r--   0        0        0      125 2023-06-02 16:20:26.327913 pyview_web-0.0.8a0/pyview/events.py
--rw-r--r--   0        0        0      751 2023-05-02 00:38:29.743473 pyview_web-0.0.8a0/pyview/js.py
--rw-r--r--   0        0        0      498 2023-05-02 00:38:29.743607 pyview_web-0.0.8a0/pyview/live_routes.py
--rw-r--r--   0        0        0     3314 2023-06-30 19:20:12.827751 pyview_web-0.0.8a0/pyview/live_socket.py
--rw-r--r--   0        0        0     1255 2023-06-13 20:41:53.657377 pyview_web-0.0.8a0/pyview/live_view.py
--rw-r--r--   0        0        0     2302 2024-05-15 00:18:19.445788 pyview_web-0.0.8a0/pyview/pyview.py
--rw-r--r--   0        0        0      363 2023-06-13 01:17:27.979329 pyview_web-0.0.8a0/pyview/secret.py
--rw-r--r--   0        0        0      432 2023-06-13 01:17:27.980035 pyview_web-0.0.8a0/pyview/session.py
--rw-r--r--   0        0        0   199984 2023-05-02 00:38:29.745551 pyview_web-0.0.8a0/pyview/static/assets/app.js
--rw-r--r--   0        0        0      206 2024-05-15 00:06:35.328321 pyview_web-0.0.8a0/pyview/template/__init__.py
--rw-r--r--   0        0        0     1864 2023-06-21 01:27:08.244253 pyview_web-0.0.8a0/pyview/template/live_template.py
--rw-r--r--   0        0        0     1876 2024-05-15 00:33:27.966402 pyview_web-0.0.8a0/pyview/template/root_template.py
--rw-r--r--   0        0        0      826 2023-05-02 00:38:29.746088 pyview_web-0.0.8a0/pyview/template/serializer.py
--rw-r--r--   0        0        0      684 2023-05-02 00:38:29.746210 pyview_web-0.0.8a0/pyview/test_csrf.py
--rw-r--r--   0        0        0        0 2023-05-02 00:38:29.746312 pyview_web-0.0.8a0/pyview/vendor/__init__.py
--rw-r--r--   0        0        0       39 2023-05-02 00:38:29.746495 pyview_web-0.0.8a0/pyview/vendor/flet/pubsub/__init__.py
--rw-r--r--   0        0        0    10184 2023-05-02 00:38:29.746630 pyview_web-0.0.8a0/pyview/vendor/flet/pubsub/pub_sub.py
--rw-r--r--   0        0        0      455 2023-05-02 00:38:29.746775 pyview_web-0.0.8a0/pyview/vendor/ibis/__init__.py
--rw-r--r--   0        0        0     7220 2023-05-02 00:38:29.746901 pyview_web-0.0.8a0/pyview/vendor/ibis/compiler.py
--rw-r--r--   0        0        0     3613 2023-05-02 00:38:29.747013 pyview_web-0.0.8a0/pyview/vendor/ibis/context.py
--rw-r--r--   0        0        0     1531 2023-05-02 00:38:29.747126 pyview_web-0.0.8a0/pyview/vendor/ibis/errors.py
--rw-r--r--   0        0        0     7042 2023-05-02 00:38:29.747263 pyview_web-0.0.8a0/pyview/vendor/ibis/filters.py
--rw-r--r--   0        0        0     3457 2023-05-02 00:38:29.747371 pyview_web-0.0.8a0/pyview/vendor/ibis/loaders.py
--rw-r--r--   0        0        0    25128 2023-05-02 00:38:29.747569 pyview_web-0.0.8a0/pyview/vendor/ibis/nodes.py
--rw-r--r--   0        0        0     2314 2023-06-30 19:20:12.828275 pyview_web-0.0.8a0/pyview/vendor/ibis/template.py
--rw-r--r--   0        0        0     2293 2023-05-02 00:38:29.747817 pyview_web-0.0.8a0/pyview/vendor/ibis/tree.py
--rw-r--r--   0        0        0     2768 2023-05-02 00:38:29.747930 pyview_web-0.0.8a0/pyview/vendor/ibis/utils.py
--rw-r--r--   0        0        0     4738 2023-06-15 02:43:05.038205 pyview_web-0.0.8a0/pyview/ws_handler.py
--rw-r--r--   0        0        0     3154 2023-06-13 01:17:27.982729 pyview_web-0.0.8a0/readme.md
--rw-r--r--   0        0        0     4970 1970-01-01 00:00:00.000000 pyview_web-0.0.8a0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-02 00:38:29.733278 pyview_web-0.0.9a0/LICENSE
+-rw-r--r--   0        0        0     2054 2024-05-17 03:14:24.228411 pyview_web-0.0.9a0/pyproject.toml
+-rw-r--r--   0        0        0      223 2023-06-02 16:20:26.327598 pyview_web-0.0.9a0/pyview/__init__.py
+-rw-r--r--   0        0        0     2508 2023-05-02 00:38:29.742232 pyview_web-0.0.9a0/pyview/assets/js/app.js
+-rw-r--r--   0        0        0     2425 2023-05-02 00:38:29.742415 pyview_web-0.0.9a0/pyview/assets/package-lock.json
+-rw-r--r--   0        0        0      151 2023-05-02 00:38:29.742554 pyview_web-0.0.9a0/pyview/assets/package.json
+-rw-r--r--   0        0        0      109 2023-06-14 00:18:12.775162 pyview_web-0.0.9a0/pyview/auth/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-14 00:18:12.775807 pyview_web-0.0.9a0/pyview/auth/provider.py
+-rw-r--r--   0        0        0     1418 2024-05-17 03:01:41.401570 pyview_web-0.0.9a0/pyview/auth/required.py
+-rw-r--r--   0        0        0       46 2023-05-02 00:38:29.742781 pyview_web-0.0.9a0/pyview/changesets/__init__.py
+-rw-r--r--   0        0        0     1747 2023-05-02 00:38:29.743020 pyview_web-0.0.9a0/pyview/changesets/changesets.py
+-rw-r--r--   0        0        0      789 2023-06-13 01:17:27.976763 pyview_web-0.0.9a0/pyview/csrf.py
+-rw-r--r--   0        0        0      125 2023-06-02 16:20:26.327913 pyview_web-0.0.9a0/pyview/events.py
+-rw-r--r--   0        0        0      751 2023-05-02 00:38:29.743473 pyview_web-0.0.9a0/pyview/js.py
+-rw-r--r--   0        0        0      498 2023-05-02 00:38:29.743607 pyview_web-0.0.9a0/pyview/live_routes.py
+-rw-r--r--   0        0        0     3314 2023-06-30 19:20:12.827751 pyview_web-0.0.9a0/pyview/live_socket.py
+-rw-r--r--   0        0        0     1255 2023-06-13 20:41:53.657377 pyview_web-0.0.9a0/pyview/live_view.py
+-rw-r--r--   0        0        0     2302 2024-05-15 01:27:44.803236 pyview_web-0.0.9a0/pyview/pyview.py
+-rw-r--r--   0        0        0      363 2023-06-13 01:17:27.979329 pyview_web-0.0.9a0/pyview/secret.py
+-rw-r--r--   0        0        0      432 2023-06-13 01:17:27.980035 pyview_web-0.0.9a0/pyview/session.py
+-rw-r--r--   0        0        0   199984 2023-05-02 00:38:29.745551 pyview_web-0.0.9a0/pyview/static/assets/app.js
+-rw-r--r--   0        0        0      206 2024-05-15 01:27:44.803531 pyview_web-0.0.9a0/pyview/template/__init__.py
+-rw-r--r--   0        0        0     1864 2023-06-21 01:27:08.244253 pyview_web-0.0.9a0/pyview/template/live_template.py
+-rw-r--r--   0        0        0     1876 2024-05-15 01:27:44.803791 pyview_web-0.0.9a0/pyview/template/root_template.py
+-rw-r--r--   0        0        0      826 2023-05-02 00:38:29.746088 pyview_web-0.0.9a0/pyview/template/serializer.py
+-rw-r--r--   0        0        0      684 2023-05-02 00:38:29.746210 pyview_web-0.0.9a0/pyview/test_csrf.py
+-rw-r--r--   0        0        0        0 2023-05-02 00:38:29.746312 pyview_web-0.0.9a0/pyview/vendor/__init__.py
+-rw-r--r--   0        0        0       39 2023-05-02 00:38:29.746495 pyview_web-0.0.9a0/pyview/vendor/flet/pubsub/__init__.py
+-rw-r--r--   0        0        0    10184 2023-05-02 00:38:29.746630 pyview_web-0.0.9a0/pyview/vendor/flet/pubsub/pub_sub.py
+-rw-r--r--   0        0        0      455 2023-05-02 00:38:29.746775 pyview_web-0.0.9a0/pyview/vendor/ibis/__init__.py
+-rw-r--r--   0        0        0     7220 2023-05-02 00:38:29.746901 pyview_web-0.0.9a0/pyview/vendor/ibis/compiler.py
+-rw-r--r--   0        0        0     3613 2023-05-02 00:38:29.747013 pyview_web-0.0.9a0/pyview/vendor/ibis/context.py
+-rw-r--r--   0        0        0     1531 2023-05-02 00:38:29.747126 pyview_web-0.0.9a0/pyview/vendor/ibis/errors.py
+-rw-r--r--   0        0        0     7042 2023-05-02 00:38:29.747263 pyview_web-0.0.9a0/pyview/vendor/ibis/filters.py
+-rw-r--r--   0        0        0     3457 2023-05-02 00:38:29.747371 pyview_web-0.0.9a0/pyview/vendor/ibis/loaders.py
+-rw-r--r--   0        0        0    25128 2023-05-02 00:38:29.747569 pyview_web-0.0.9a0/pyview/vendor/ibis/nodes.py
+-rw-r--r--   0        0        0     2314 2023-06-30 19:20:12.828275 pyview_web-0.0.9a0/pyview/vendor/ibis/template.py
+-rw-r--r--   0        0        0     2293 2023-05-02 00:38:29.747817 pyview_web-0.0.9a0/pyview/vendor/ibis/tree.py
+-rw-r--r--   0        0        0     2768 2023-05-02 00:38:29.747930 pyview_web-0.0.9a0/pyview/vendor/ibis/utils.py
+-rw-r--r--   0        0        0     4738 2023-06-15 02:43:05.038205 pyview_web-0.0.9a0/pyview/ws_handler.py
+-rw-r--r--   0        0        0     3403 2024-05-15 01:27:44.804554 pyview_web-0.0.9a0/readme.md
+-rw-r--r--   0        0        0     5220 1970-01-01 00:00:00.000000 pyview_web-0.0.9a0/PKG-INFO
```

### Comparing `pyview_web-0.0.8a0/LICENSE` & `pyview_web-0.0.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyproject.toml` & `pyview_web-0.0.9a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "pyview-web"
 
 packages = [
   { include = "pyview" },
 ]
 
-version = "0.0.8a"
+version = "0.0.9a"
 description = "LiveView in Python"
 authors = ["Larry Ogrodnek <ogrodnek@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://pyview.rocks"
 repository = "https://github.com/ogrodnek/pyview"
 keywords = ["web", "api", "LiveView"]
@@ -39,25 +39,25 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9.16"
-fastapi = "0.89.1"
+fastapi = "0.111.0"
 uvicorn = "0.20.0"
 wsproto = "1.2.0"
 APScheduler = "3.9.1.post1"
 psutil = "^5.9.4"
 markupsafe = "^2.1.2"
 itsdangerous = "^2.1.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.0.0"
-black = "22.12.0"
+black = "24.3.0"
 pyright = "1.1.292"
 aiohttp = "^3.8.4"
 
 [tool.poetry.group.profiling.dependencies]
 scalene = "^1.5.19"
 memray = "^1.6.0"
 
@@ -68,11 +68,12 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 exclude = [
     ".venv",
+    "examples/.venv",
     "**/vendor",
     "**/node_modules",
     "**/__pycache__",
 ]
```

### Comparing `pyview_web-0.0.8a0/pyview/assets/js/app.js` & `pyview_web-0.0.9a0/pyview/assets/js/app.js`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/assets/package-lock.json` & `pyview_web-0.0.9a0/pyview/assets/package-lock.json`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/auth/provider.py` & `pyview_web-0.0.9a0/pyview/auth/provider.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/auth/required.py` & `pyview_web-0.0.9a0/pyview/auth/required.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 import typing
 from dataclasses import dataclass
 from starlette.websockets import WebSocket
 from starlette.authentication import requires as starlette_requires, has_required_scope
 from .provider import AuthProvider, AuthProviderFactory
 from pyview import LiveView
+import sys
 
-_CallableType = typing.TypeVar("_CallableType", bound=typing.Callable)
+if sys.version_info >= (3, 10):  # pragma: no cover
+    from typing import ParamSpec
+else:  # pragma: no cover
+    from typing_extensions import ParamSpec
+
+_P = ParamSpec("_P")
 
 
 @dataclass
 class RequiredScopeAuthProvider(AuthProvider):
     scopes: typing.Sequence[str]
     status_code: int = 403
     redirect: typing.Optional[str] = None
 
-    def wrap(self, func: _CallableType) -> _CallableType:
+    def wrap(
+        self, func: typing.Callable[_P, typing.Any]
+    ) -> typing.Callable[_P, typing.Any]:
         return starlette_requires(self.scopes, self.status_code, self.redirect)(func)
 
-    def has_required_auth(self, websocket: WebSocket) -> bool:
+    async def has_required_auth(self, websocket: WebSocket) -> bool:
         return has_required_scope(websocket, self.scopes)
 
 
 def requires(
     scopes: typing.Union[str, typing.Sequence[str]],
     status_code: int = 403,
     redirect: typing.Optional[str] = None,
 ) -> typing.Callable[[type[LiveView]], type[LiveView]]:
     def decorator(cls: type[LiveView]) -> type[LiveView]:
         scopes_list = [scopes] if isinstance(scopes, str) else list(scopes)
-        return AuthProviderFactory.set(cls, RequiredScopeAuthProvider(scopes_list, status_code, redirect))
+        return AuthProviderFactory.set(
+            cls, RequiredScopeAuthProvider(scopes_list, status_code, redirect)
+        )
 
     return decorator
```

### Comparing `pyview_web-0.0.8a0/pyview/changesets/changesets.py` & `pyview_web-0.0.9a0/pyview/changesets/changesets.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/csrf.py` & `pyview_web-0.0.9a0/pyview/csrf.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/js.py` & `pyview_web-0.0.9a0/pyview/js.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/live_socket.py` & `pyview_web-0.0.9a0/pyview/live_socket.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/live_view.py` & `pyview_web-0.0.9a0/pyview/live_view.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/pyview.py` & `pyview_web-0.0.9a0/pyview/pyview.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/static/assets/app.js` & `pyview_web-0.0.9a0/pyview/static/assets/app.js`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/template/live_template.py` & `pyview_web-0.0.9a0/pyview/template/live_template.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/template/root_template.py` & `pyview_web-0.0.9a0/pyview/template/root_template.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/template/serializer.py` & `pyview_web-0.0.9a0/pyview/template/serializer.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/test_csrf.py` & `pyview_web-0.0.9a0/pyview/test_csrf.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/vendor/flet/pubsub/pub_sub.py` & `pyview_web-0.0.9a0/pyview/vendor/flet/pubsub/pub_sub.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/vendor/ibis/compiler.py` & `pyview_web-0.0.9a0/pyview/vendor/ibis/compiler.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/vendor/ibis/context.py` & `pyview_web-0.0.9a0/pyview/vendor/ibis/context.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/vendor/ibis/errors.py` & `pyview_web-0.0.9a0/pyview/vendor/ibis/errors.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/vendor/ibis/filters.py` & `pyview_web-0.0.9a0/pyview/vendor/ibis/filters.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/vendor/ibis/loaders.py` & `pyview_web-0.0.9a0/pyview/vendor/ibis/loaders.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/vendor/ibis/nodes.py` & `pyview_web-0.0.9a0/pyview/vendor/ibis/nodes.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/vendor/ibis/template.py` & `pyview_web-0.0.9a0/pyview/vendor/ibis/template.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/vendor/ibis/tree.py` & `pyview_web-0.0.9a0/pyview/vendor/ibis/tree.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/vendor/ibis/utils.py` & `pyview_web-0.0.9a0/pyview/vendor/ibis/utils.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/pyview/ws_handler.py` & `pyview_web-0.0.9a0/pyview/ws_handler.py`

 * *Files identical despite different names*

### Comparing `pyview_web-0.0.8a0/readme.md` & `pyview_web-0.0.9a0/readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,30 @@
 
 **Source Code**: <a href="https://github.com/ogrodnek/pyview" target="_blank">https://github.com/ogrodnek/pyview</a>
 
 # Installation
 
 `pip install pyview-web`
 
+## Quickstart
+
+There's a [cookiecutter](https://github.com/cookiecutter/cookiecutter) template available
+
+```
+cookiecutter gh:ogrodnek/pyview-cookiecutter
+```
+
 # Live Examples
 
 [https://examples.pyview.rocks/](https://examples.pyview.rocks/)
 
+## Other Examples
+
+- [pyview AI chat](https://github.com/pyview/pyview-example-ai-chat)
+
 ## Simple Counter
 
 [See it live!](https://examples.pyview.rocks/count)
 
 count.py:
 
 ```python
```

### Comparing `pyview_web-0.0.8a0/PKG-INFO` & `pyview_web-0.0.9a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyview-web
-Version: 0.0.8a0
+Version: 0.0.9a0
 Summary: LiveView in Python
 Home-page: https://pyview.rocks
 License: MIT
 Keywords: web,api,LiveView
 Author: Larry Ogrodnek
 Author-email: ogrodnek@gmail.com
 Requires-Python: >=3.9.16,<4.0.0
@@ -30,15 +30,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: APScheduler (==3.9.1.post1)
-Requires-Dist: fastapi (==0.89.1)
+Requires-Dist: fastapi (==0.111.0)
 Requires-Dist: itsdangerous (>=2.1.2,<3.0.0)
 Requires-Dist: markupsafe (>=2.1.2,<3.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: uvicorn (==0.20.0)
 Requires-Dist: wsproto (==1.2.0)
 Project-URL: Repository, https://github.com/ogrodnek/pyview
 Description-Content-Type: text/markdown
@@ -53,18 +53,30 @@
 
 **Source Code**: <a href="https://github.com/ogrodnek/pyview" target="_blank">https://github.com/ogrodnek/pyview</a>
 
 # Installation
 
 `pip install pyview-web`
 
+## Quickstart
+
+There's a [cookiecutter](https://github.com/cookiecutter/cookiecutter) template available
+
+```
+cookiecutter gh:ogrodnek/pyview-cookiecutter
+```
+
 # Live Examples
 
 [https://examples.pyview.rocks/](https://examples.pyview.rocks/)
 
+## Other Examples
+
+- [pyview AI chat](https://github.com/pyview/pyview-example-ai-chat)
+
 ## Simple Counter
 
 [See it live!](https://examples.pyview.rocks/count)
 
 count.py:
 
 ```python
```

