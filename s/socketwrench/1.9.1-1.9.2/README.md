# Comparing `tmp/socketwrench-1.9.1.tar.gz` & `tmp/socketwrench-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketwrench-1.9.1.tar", last modified: Thu May 16 23:39:05 2024, max compression
+gzip compressed data, was "socketwrench-1.9.2.tar", last modified: Fri May 17 03:26:26 2024, max compression
```

## Comparing `socketwrench-1.9.1.tar` & `socketwrench-1.9.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:39:05.416073 socketwrench-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-16 23:39:01.000000 socketwrench-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 23:39:01.000000 socketwrench-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 23:39:05.416073 socketwrench-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-16 23:39:01.000000 socketwrench-1.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-16 23:39:01.000000 socketwrench-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 23:39:05.416073 socketwrench-1.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:39:05.412073 socketwrench-1.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:39:05.416073 socketwrench-1.9.1/src/socketwrench/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 23:39:01.000000 socketwrench-1.9.1/src/socketwrench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 23:39:01.000000 socketwrench-1.9.1/src/socketwrench/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-16 23:39:01.000000 socketwrench-1.9.1/src/socketwrench/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    26920 2024-05-16 23:39:01.000000 socketwrench-1.9.1/src/socketwrench/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-16 23:39:01.000000 socketwrench-1.9.1/src/socketwrench/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:39:05.416073 socketwrench-1.9.1/src/socketwrench/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-16 23:39:01.000000 socketwrench-1.9.1/src/socketwrench/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:39:05.416073 socketwrench-1.9.1/src/socketwrench/resources/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-16 23:39:01.000000 socketwrench-1.9.1/src/socketwrench/resources/playground/panels.js
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 23:39:01.000000 socketwrench-1.9.1/src/socketwrench/resources/playground/playground.html
--rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-16 23:39:01.000000 socketwrench-1.9.1/src/socketwrench/resources/playground/playground.js
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-16 23:39:01.000000 socketwrench-1.9.1/src/socketwrench/resources/swagger.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:39:05.416073 socketwrench-1.9.1/src/socketwrench/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 23:39:01.000000 socketwrench-1.9.1/src/socketwrench/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-16 23:39:01.000000 socketwrench-1.9.1/src/socketwrench/samples/file_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-16 23:39:01.000000 socketwrench-1.9.1/src/socketwrench/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-16 23:39:01.000000 socketwrench-1.9.1/src/socketwrench/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 23:39:01.000000 socketwrench-1.9.1/src/socketwrench/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    30708 2024-05-16 23:39:01.000000 socketwrench-1.9.1/src/socketwrench/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:39:05.416073 socketwrench-1.9.1/src/socketwrench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 23:39:05.000000 socketwrench-1.9.1/src/socketwrench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 23:39:05.000000 socketwrench-1.9.1/src/socketwrench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 23:39:05.000000 socketwrench-1.9.1/src/socketwrench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 23:39:05.000000 socketwrench-1.9.1/src/socketwrench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:26:26.321150 socketwrench-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-17 03:26:22.000000 socketwrench-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 03:26:22.000000 socketwrench-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-17 03:26:26.321150 socketwrench-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-17 03:26:22.000000 socketwrench-1.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-17 03:26:22.000000 socketwrench-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:26:26.321150 socketwrench-1.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:26:26.317150 socketwrench-1.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:26:26.317150 socketwrench-1.9.2/src/socketwrench/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-17 03:26:22.000000 socketwrench-1.9.2/src/socketwrench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-17 03:26:22.000000 socketwrench-1.9.2/src/socketwrench/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-17 03:26:22.000000 socketwrench-1.9.2/src/socketwrench/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30750 2024-05-17 03:26:22.000000 socketwrench-1.9.2/src/socketwrench/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-17 03:26:22.000000 socketwrench-1.9.2/src/socketwrench/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:26:26.317150 socketwrench-1.9.2/src/socketwrench/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-17 03:26:22.000000 socketwrench-1.9.2/src/socketwrench/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:26:26.321150 socketwrench-1.9.2/src/socketwrench/resources/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-17 03:26:22.000000 socketwrench-1.9.2/src/socketwrench/resources/playground/panels.js
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-17 03:26:22.000000 socketwrench-1.9.2/src/socketwrench/resources/playground/playground.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-17 03:26:22.000000 socketwrench-1.9.2/src/socketwrench/resources/playground/playground.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-17 03:26:22.000000 socketwrench-1.9.2/src/socketwrench/resources/swagger.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:26:26.321150 socketwrench-1.9.2/src/socketwrench/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:26:22.000000 socketwrench-1.9.2/src/socketwrench/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-17 03:26:22.000000 socketwrench-1.9.2/src/socketwrench/samples/file_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-17 03:26:22.000000 socketwrench-1.9.2/src/socketwrench/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-17 03:26:22.000000 socketwrench-1.9.2/src/socketwrench/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-17 03:26:22.000000 socketwrench-1.9.2/src/socketwrench/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30709 2024-05-17 03:26:22.000000 socketwrench-1.9.2/src/socketwrench/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:26:26.321150 socketwrench-1.9.2/src/socketwrench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-17 03:26:26.000000 socketwrench-1.9.2/src/socketwrench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-17 03:26:26.000000 socketwrench-1.9.2/src/socketwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:26:26.000000 socketwrench-1.9.2/src/socketwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 03:26:26.000000 socketwrench-1.9.2/src/socketwrench.egg-info/top_level.txt
```

### Comparing `socketwrench-1.9.1/LICENSE` & `socketwrench-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.1/PKG-INFO` & `socketwrench-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.9.1
+Version: 1.9.2
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.9.1/README.md` & `socketwrench-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.1/pyproject.toml` & `socketwrench-1.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketwrench"
-version = "1.9.1"
+version = "1.9.2"
 description = "A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger."
 readme = "README.md"
 authors = [{ name = "Torin Halsted", email = "modularizer@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
```

### Comparing `socketwrench-1.9.1/src/socketwrench/__init__.py` & `socketwrench-1.9.2/src/socketwrench/__init__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.1/src/socketwrench/__main__.py` & `socketwrench-1.9.2/src/socketwrench/__main__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.1/src/socketwrench/connection.py` & `socketwrench-1.9.2/src/socketwrench/connection.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.1/src/socketwrench/handlers.py` & `socketwrench-1.9.2/src/socketwrench/handlers.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from contextlib import suppress
 from functools import wraps
 from pathlib import Path
 import socket
 
 from socketwrench.tags import tag, get, gettag
 from socketwrench.types import Request, Response, Query, Body, Route, FullPath, Method, File, ClientAddr, \
-    HTTPStatusCode, ErrorResponse, Headers, ErrorModes, FileResponse, HTMLResponse, url_decode
+    HTTPStatusCode, ErrorResponse, Headers, ErrorModes, FileResponse, HTMLResponse, url_decode, StandardHTMLResponse
 
 logger = logging.getLogger("socketwrench")
 
 
 class Autofill:
     def request(self, request: Request) -> Request:
         return request
@@ -369,14 +369,18 @@
         r = FileResponse(p, version=request.version)
         print("content type", r.headers.get("Content-Type"))
         return r
 
 
 def matches_variadic_route(route: str, variadic_route: str) -> dict:
     try:
+        if route.endswith("/") and not variadic_route.endswith("/"):
+            route = route[:-1]
+        elif variadic_route.endswith("/") and not route.endswith("/"):
+            variadic_route = variadic_route[:-1]
         route_parts = route.split("/")
         variadic_parts = variadic_route.split("/")
         n = len(route_parts)
         if n != len(variadic_parts):
             return False
 
         found_matches = {}
@@ -475,39 +479,82 @@
                   total_nonvariadic_chars,
                   total_variadic_pattern_count,
                   len(pattern),
                   pattern))
     sorted_patterns = [_v[-1] for _v in reversed(sorted(q))]
     return sorted_patterns
 
+
+def is_object_instance(obj):
+    # Check if obj is an instance of a custom class
+    if not hasattr(obj, '__class__'):
+        return False
+    # Get all members of the object's class
+    members = inspect.getmembers(obj.__class__, predicate=inspect.isfunction)
+
+    # Check if there are any user-defined methods (excluding special methods)
+    user_defined_methods = [name for name, f in members if not name.startswith('_')]
+
+    return bool(user_defined_methods)
+
+
 class RouteHandler:
     resources_folder = Path(__file__).parent / "resources"
     playground_folder = resources_folder / "playground"
     default_favicon = resources_folder / "favicon.ico"
 
     def __init__(self,
                  routes: dict | None = None,
                  fallback_handler=None,
                  base_path: str = "/",
                  require_tag: bool = False,
                  error_mode: str = ErrorModes.HIDE,
-                 favicon: str | None = default_favicon
+                 favicon: str | None = default_favicon,
+                 nav_path = "/",
+                 nav_recursion = True,
                  ):
+        base_path = base_path.replace("//", "/")
+        if not base_path.endswith("/"):
+            base_path += "/"
         self.base_path = base_path
         self.require_tag = require_tag
         self.error_mode = error_mode
         self.favicon_path = favicon
 
         self.routes = {}
         self.matchable_routes = {}
         self.variadic_routes = {}
+        self.sub_route_handlers = {}
+        self.nav_path = nav_path
+        self.nav_recursion = nav_recursion
         if routes:
+            if isinstance(routes, type):
+                routes = routes()
+
+            kw = {
+                "error_mode": error_mode,
+                "require_tag": require_tag,
+                "nav_path": nav_path,
+                "nav_recursion": nav_recursion,
+            }
             if isinstance(routes, dict):
                 for k, v in routes.items():
-                    self[k] = v
+                    sub = self.base_path + (k[1:] if k.startswith("/") else k) + ("/" if not k.endswith("/") else "")
+                    sub = sub.replace("//", "/")
+
+                    if isinstance(v, type):
+                        self.sub_route_handlers[sub] = RouteHandler(v(), base_path=sub, **kw)
+                    elif isinstance(v, RouteHandler):
+                        self.sub_route_handlers[sub] = v
+                    elif isinstance(v, dict):
+                        self.sub_route_handlers[sub] = RouteHandler(v, base_path=sub, **kw)
+                    elif is_object_instance(v):
+                        self.sub_route_handlers[sub] = RouteHandler(v, base_path=sub, **kw)
+                    else:
+                        self[k] = v
             else:
                 self.parse_routes_from_object(routes)
         self.fallback_handler = wrap_handler(fallback_handler) if fallback_handler else None
 
         op = wrap_handler(self.openapi, error_mode=error_mode)
         sw = wrap_handler(self.swagger, error_mode=error_mode)
 
@@ -520,21 +567,27 @@
             "/api": wrap_handler(self.playground, error_mode=error_mode),
             "/api/playground.js": wrap_handler(self.playground_js, error_mode=error_mode),
             "/api/panels.js": wrap_handler(self.playground_panels_js, error_mode=error_mode),
         }
         if self.favicon_path:
             self.default_routes["/favicon.ico"] = wrap_handler(self.favicon, error_mode=error_mode)
 
-    @get
-    def openapi(self) -> str:
-        from socketwrench.openapi import openapi_schema
+    def _all_routes(self, recursive=True):
         d = {
             **self.routes,
             **self.variadic_routes
         }
+        if recursive:
+            for k, v in self.sub_route_handlers.items():
+                d.update(v._all_routes(recursive))
+        return d
+    @get
+    def openapi(self) -> str:
+        from socketwrench.openapi import openapi_schema
+        d = self._all_routes()
         o = openapi_schema(d)
         return o
 
     @get
     def favicon(self, request: Request) -> Response:
         try:
             r = FileResponse(self.favicon_path, version=request.version)
@@ -567,18 +620,53 @@
                         continue
                     if getattr(v, "do_not_serve", False):
                         continue
                     routes = getattr(v, "routes", [k])
                     for route in routes:
                         with suppress(Exception):
                             self[route] = v
+        if callable(obj):
+            self[""] = obj
+
+    def get_nav(self):
+        routes = self._all_routes(self.nav_recursion)
+        links = []
+        for route in routes:
+            if route.startswith(self.base_path):
+                r = route[len(self.base_path):]
+                if not r.endswith("/"):
+                    r += "/"
+                n = r.count("/")
+                links.append(self.base_path + r)
+        links = sorted(links)
+        nav = "<ul>\n" + "\n\t".join([f'<li><a href="{l}">{l}</a></li>' if '{' not in l else f'<li>{l}</li>'  for l in links]) + "\n</ul>"
+        return StandardHTMLResponse(nav, title=self.base_path)
 
     def __call__(self, request: Request) -> Response:
         route = request.path.route()
+
+        route_diff = route[len(self.base_path):]
+        if not route_diff.startswith("/"):
+            route_diff = "/" + route_diff
+        if self.nav_path and (route_diff == self.nav_path or route_diff == self.nav_path + "/"):
+            return self.get_nav()
+
+        if not route.startswith(self.base_path):
+            return Response(b'Not Found',
+                            status_code=404,
+                            headers={"Content-Type": "text/plain"},
+                            version=request.version)
+        # search from longest to shortest subroute by length or string
+        subroute_keys = sorted(self.sub_route_handlers.keys(), key=lambda x: (len(x), x), reverse=True)
+        for k in subroute_keys:
+            if route.startswith(k):
+                return self.sub_route_handlers[k](request)
+
         handler = self.routes.get(route, None)
+
         route_params = {}
         if handler is None:
             for k, v in self.matchable_routes.items():
                 if v.match(route):
                     handler = v
                     break
             else:
@@ -619,14 +707,15 @@
         if route_params:
             r = handler(request, route_params)
         else:
             r = handler(request)
         return r
 
     def route(self, handler, route: str | None = None, allowed_methods: tuple[str] | None = None):
+        route = route.replace("//", "/")
         if isinstance(handler, Path):
             handler = StaticFileHandler(Path, route)
 
         if isinstance(handler, str):
             return lambda handler: self.route(handler, route, allowed_methods)
 
         if route is None:
@@ -634,20 +723,23 @@
         if allowed_methods is None:
             allowed_methods = getattr(handler, "allowed_methods", ("GET",))
         em = getattr(handler, "error_mode", self.error_mode)
         h = wrap_handler(handler, error_mode=em)
         h.__dict__["allowed_methods"] = allowed_methods
         if self.base_path == "/" and route.startswith("/"):
             route = route[1:]
+
+        sub = self.base_path + route + ("/" if not route.endswith("/") else "")
+        sub = sub.replace("//", "/")
         if "{" in route and "}" in route:
-            self.variadic_routes[self.base_path + route] = h
+            self.variadic_routes[sub] = h
         elif hasattr(h, "match") and callable(h.match):
-            self.matchable_routes[self.base_path + route] = h
+            self.matchable_routes[sub] = h
         else:
-            self.routes[self.base_path + route] = h
+            self.routes[sub] = h
 
     def get(self, handler=None, route: str | None = None):
         return self.route(handler, route, allowed_methods=("GET",))
 
     def post(self, handler=None, route: str | None = None):
         return self.route(handler, route, allowed_methods=("POST",))
```

### Comparing `socketwrench-1.9.1/src/socketwrench/openapi.py` & `socketwrench-1.9.2/src/socketwrench/openapi.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.1/src/socketwrench/resources/favicon.ico` & `socketwrench-1.9.2/src/socketwrench/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.1/src/socketwrench/resources/playground/panels.js` & `socketwrench-1.9.2/src/socketwrench/resources/playground/panels.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.1/src/socketwrench/resources/playground/playground.html` & `socketwrench-1.9.2/src/socketwrench/resources/playground/playground.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.1/src/socketwrench/resources/playground/playground.js` & `socketwrench-1.9.2/src/socketwrench/resources/playground/playground.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.1/src/socketwrench/resources/swagger.html` & `socketwrench-1.9.2/src/socketwrench/resources/swagger.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.1/src/socketwrench/samples/file_sample.py` & `socketwrench-1.9.2/src/socketwrench/samples/file_sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.1/src/socketwrench/samples/sample.py` & `socketwrench-1.9.2/src/socketwrench/samples/sample.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from pathlib import Path
 
 import cv2
 import numpy as np
 
 from socketwrench.handlers import StaticFileHandler
-from socketwrench.tags import private, post, put, patch, delete, route, methods
+from socketwrench.tags import private, post, put, patch, delete, route, methods, get
 from socketwrench.types import TBDBResponse, FileTypeResponse
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 class Sample:
     src = StaticFileHandler(Path(__file__).parent.parent.parent)
@@ -163,15 +163,46 @@
 
     def random_img(self) -> FileTypeResponse("image/png", lambda x: cv2.imencode(".png", x.astype(np.uint8))[1].tobytes()):
         x = np.random.rand(100, 100, 3) * 255
         x = x.astype(np.uint8)
         return x
 
 
+
+
+class Other:
+    def hello(self):
+        return "world"
+
+    def goodbye(self):
+        return "cruel world"
+
+
+class Another:
+    @get("/add/{x}/{y}")
+    def add(self, x, y):
+        return x + y
+
+    @get("/sub/{x}/{y}")
+    def sub(self, x, y):
+        return x - y
+
+    def hello(self):
+        return "world"
+
+
+
 if __name__ == '__main__':
     from socketwrench import serve
     s = Sample()
-    serve(s)
+    serve({
+        "sample": s,
+        "a": Another(),
+        "nest": {
+            "a": Another,
+            "o": Other
+        }
+    }, nav_path="/nav")
     # OR
     # serve(Sample)
     # OR
     # serve("socketwrench.samples.sample.Sample")
```

### Comparing `socketwrench-1.9.1/src/socketwrench/server.py` & `socketwrench-1.9.2/src/socketwrench/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """A simple HTTP server built directly on top of socket.socket."""
 import socket
 import logging
 import time
 from pathlib import Path
 
 from socketwrench.connection import Connection
-from socketwrench.handlers import RouteHandler, wrap_handler
+from socketwrench.handlers import RouteHandler, wrap_handler, is_object_instance
 
 logger = logging.getLogger("socketwrench")
 
 
 class Server(socket.socket):
     """A simple HTTP server built directly on top of socket.socket."""
     default_port = 8080
     default_host = ''
     default_backlog = 1
     default_chunk_size = Connection.default_chunk_size
     default_num_connection_threads = 1
     default_socket_options = {
         socket.SOL_SOCKET: {
-            socket.SO_REUSEADDR: 1,
-            socket.SO_REUSEPORT: 1
+            socket.SO_REUSEADDR: 1
         }
     }
     default_pause_sleep = 0.1
     default_accept_sleep = 0
     default_favicon = RouteHandler.default_favicon
 
     def __init__(self,
@@ -35,15 +34,16 @@
                  chunk_size: int = default_chunk_size,
                  num_connection_threads: int = default_num_connection_threads,
                  socket_options: dict[int, dict[int, int]] | None = default_socket_options,
                  pause_sleep: float = default_pause_sleep,
                  accept_sleep: float = default_accept_sleep,
                  fallback_handler=None,
                  serve: bool = True,
-                 favicon: str | Path = default_favicon
+                 favicon: str | Path = default_favicon,
+                 **kwargs
                  ):
         """A simple HTTP server built directly on top of socket.socket.
 
         Args:
             routes (dict[str, RequestHandler] | None, optional): A dictionary of routes to handlers.
             port (int, optional): The port to listen on. Defaults to 8080.
             host (str, optional): The host to listen on. Defaults to ''.
@@ -56,33 +56,32 @@
             pause_sleep (float, optional): The number of seconds to sleep between checking the threading.Event
                 when the server is paused. Could affect CPU and latency. Defaults to 0.1.
             accept_sleep (float, optional): The number of seconds to sleep between checking for new connections.
                 Could affect latency. Defaults to 0.1.
             fallback_handler (RequestHandler, optional): The function to use to handle requests that don't match any routes.
             serve (bool, optional): Whether to start serving immediately. Defaults to True.
         """
-        if isinstance(routes, type):
-            routes = routes()
 
         s = str(routes)
         s2 = s.split("\n")[0][:50]
         s = s2 + ("..." if len(s) > len(s2) else "")
         logger.info(f"Creating server with {s}")
 
-        if callable(routes):
+        if callable(routes) and not is_object_instance(routes):
             if isinstance(routes, RouteHandler):
                 self.handler = routes
             else:
                 self.handler = wrap_handler(routes)
         else:
             self.handler = RouteHandler(
                 fallback_handler=fallback_handler,
                 routes=routes,
                 base_path="/",
-                favicon=favicon
+                favicon=favicon,
+                **kwargs
             )
 
         self.host = host
         self.port = port
         self.backlog = backlog
         self.chunk_size = chunk_size
         self.num_connection_threads = num_connection_threads
@@ -122,22 +121,22 @@
             return
 
         # set socket options
         for level, options in socket_options.items():
             for option, value in options.items():
                 self.setsockopt(level, option, value)
 
-    def serve(self, thread: bool = False, cleanup_event = None, pause_event = None, **kwargs) -> None | tuple:
+    def serve(self, thread: bool = False, cleanup_event = None, pause_event = None, nav_path="/", **kwargs) -> None | tuple:
         if not isinstance(self, Server):
             if isinstance(self, str) or "<module" in str(type(self)):
-                return Server.serve_module(self, thread=thread, cleanup_event=cleanup_event, pause_event=pause_event, **kwargs)
+                return Server.serve_module(self, thread=thread, cleanup_event=cleanup_event, pause_event=pause_event, nav_path=nav_path, **kwargs)
             elif isinstance(self, type):
-                return Server.serve_class(self, thread=thread, cleanup_event=cleanup_event, pause_event=pause_event, **kwargs)
+                return Server.serve_class(self, thread=thread, cleanup_event=cleanup_event, pause_event=pause_event, nav_path=nav_path,**kwargs)
             # allows classmethod-like usage of Server.serve(my_server_instance)
-            return Server(self).serve(thread=thread, cleanup_event=cleanup_event, pause_event=pause_event)
+            return Server(self, nav_path=nav_path, **kwargs).serve(thread=thread, cleanup_event=cleanup_event, pause_event=pause_event)
         if thread:
             import threading
 
             self.cleanup_event = threading.Event()
             self.pause_event = threading.Event()
 
             t = threading.Thread(target=self.serve, args=(False, self.cleanup_event, self.pause_event), daemon=True)
```

### Comparing `socketwrench-1.9.1/src/socketwrench/tags.py` & `socketwrench-1.9.2/src/socketwrench/tags.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.1/src/socketwrench/types.py` & `socketwrench-1.9.2/src/socketwrench/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1006,7 +1006,8 @@
     DEFAULT = HIDE
 
 
 def set_default_error_mode(mode: str):
     if mode not in [ErrorModes.HIDE, ErrorModes.TYPE, ErrorModes.SHORT, ErrorModes.TRACEBACK]:
         raise ValueError(f"Invalid error mode: {mode}. Options are 'hide', 'type', 'short', 'traceback'.")
     ErrorModes.DEFAULT = mode
+
```

### Comparing `socketwrench-1.9.1/src/socketwrench.egg-info/PKG-INFO` & `socketwrench-1.9.2/src/socketwrench.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.9.1
+Version: 1.9.2
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.9.1/src/socketwrench.egg-info/SOURCES.txt` & `socketwrench-1.9.2/src/socketwrench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

