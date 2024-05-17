# Comparing `tmp/python_asynctools-0.0.2.tar.gz` & `tmp/python_asynctools-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_asynctools-0.0.2.tar", max compression
+gzip compressed data, was "python_asynctools-0.0.2.1.tar", max compression
```

## Comparing `python_asynctools-0.0.2.tar` & `python_asynctools-0.0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_asynctools-0.0.2/LICENSE
--rwxr-xr-x   0        0        0     5236 2024-05-17 09:42:12.938654 python_asynctools-0.0.2/asynctools/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_asynctools-0.0.2/asynctools/py.typed
--rw-r--r--   0        0        0     1212 2024-05-17 09:41:43.838161 python_asynctools-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      212 2024-05-17 05:56:46.790546 python_asynctools-0.0.2/readme.md
--rw-r--r--   0        0        0     1421 1970-01-01 00:00:00.000000 python_asynctools-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_asynctools-0.0.2.1/LICENSE
+-rwxr-xr-x   0        0        0     5679 2024-05-17 10:03:55.460056 python_asynctools-0.0.2.1/asynctools/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_asynctools-0.0.2.1/asynctools/py.typed
+-rw-r--r--   0        0        0     1214 2024-05-17 10:06:27.176309 python_asynctools-0.0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      212 2024-05-17 05:56:46.790546 python_asynctools-0.0.2.1/readme.md
+-rw-r--r--   0        0        0     1423 1970-01-01 00:00:00.000000 python_asynctools-0.0.2.1/PKG-INFO
```

### Comparing `python_asynctools-0.0.2/LICENSE` & `python_asynctools-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_asynctools-0.0.2/asynctools/__init__.py` & `python_asynctools-0.0.2.1/asynctools/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -81,30 +81,45 @@
     it: Iterable[T] | AsyncIterable[T], 
     /, 
     threaded: bool = True, 
 ) -> AsyncIterator[T]:
     if isinstance(it, AsyncIterable):
         return aiter(it)
     if isgenerator(it):
-        send = ensure_async(it.send, threaded=threaded)
-        async def wrapper():
-            e: Any = None
-            try:
-                while True:
-                    e = yield await send(e)
-            except StopAsyncIteration:
-                pass
+        if threaded:
+            send = as_thread(it.send)
+            async def wrapper():
+                e: Any = None
+                try:
+                    while True:
+                        e = yield await send(e)
+                except StopAsyncIteration:
+                    pass
+        else:
+            send = it.send
+            async def wrapper():
+                e: Any = None
+                try:
+                    while True:
+                        e = yield send(e)
+                except StopIteration:
+                    pass
     else:
-        get = ensure_async(iter(it).__next__, threaded=threaded)
-        async def wrapper():
-            try:
-                while True:
-                    yield await get()
-            except:
-                pass
+        if threaded:
+            get = as_thread(iter(it).__next__)
+            async def wrapper():
+                try:
+                    while True:
+                        yield await get()
+                except StopAsyncIteration:
+                    pass
+        else:
+            async def wrapper():
+                for e in it:
+                    yield e
     return wrapper()
 
 
 async def async_map(func, iterable, /, *iterables, threaded: bool = True):
     func = ensure_async(func, threaded=threaded)
     if iterables:
         async for args in async_zip(iterable, *iterables, threaded=threaded):
```

### Comparing `python_asynctools-0.0.2/pyproject.toml` & `python_asynctools-0.0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-asynctools"
-version = "0.0.2"
+version = "0.0.2.1"
 description = "Python asynchronous tools."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-asynctools"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-asynctools"
 keywords = ["asynchronous", "tools"]
```

### Comparing `python_asynctools-0.0.2/PKG-INFO` & `python_asynctools-0.0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-asynctools
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: Python asynchronous tools.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-asynctools
 License: MIT
 Keywords: asynchronous,tools
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

