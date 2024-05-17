# Comparing `tmp/python_asynctools-0.0.2.1.tar.gz` & `tmp/python_asynctools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_asynctools-0.0.2.1.tar", max compression
+gzip compressed data, was "python_asynctools-0.0.3.tar", max compression
```

## Comparing `python_asynctools-0.0.2.1.tar` & `python_asynctools-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_asynctools-0.0.2.1/LICENSE
--rwxr-xr-x   0        0        0     5679 2024-05-17 10:03:55.460056 python_asynctools-0.0.2.1/asynctools/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_asynctools-0.0.2.1/asynctools/py.typed
--rw-r--r--   0        0        0     1214 2024-05-17 10:06:27.176309 python_asynctools-0.0.2.1/pyproject.toml
--rw-r--r--   0        0        0      212 2024-05-17 05:56:46.790546 python_asynctools-0.0.2.1/readme.md
--rw-r--r--   0        0        0     1423 1970-01-01 00:00:00.000000 python_asynctools-0.0.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_asynctools-0.0.3/LICENSE
+-rwxr-xr-x   0        0        0     6145 2024-05-17 14:51:11.875839 python_asynctools-0.0.3/asynctools/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_asynctools-0.0.3/asynctools/py.typed
+-rw-r--r--   0        0        0     1212 2024-05-17 14:52:02.093995 python_asynctools-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      212 2024-05-17 05:56:46.790546 python_asynctools-0.0.3/readme.md
+-rw-r--r--   0        0        0     1421 1970-01-01 00:00:00.000000 python_asynctools-0.0.3/PKG-INFO
```

### Comparing `python_asynctools-0.0.2.1/LICENSE` & `python_asynctools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_asynctools-0.0.2.1/asynctools/__init__.py` & `python_asynctools-0.0.3/asynctools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 2)
+__version__ = (0, 0, 3)
 __all__ = [
     "as_thread", "ensure_async", "ensure_await", "ensure_coroutine", "ensure_aiter", 
-    "async_map", "async_filter", "async_reduce", "async_zip", "call_as_aiter", "to_list", 
+    "async_map", "async_filter", "async_reduce", "async_zip", "async_chain", 
+    "call_as_aiter", "to_list", 
 ]
 
 from asyncio import to_thread
 from collections.abc import Awaitable, AsyncIterable, AsyncIterator, Callable, Coroutine, Iterable
 from inspect import isawaitable, iscoroutinefunction, isgenerator
 from typing import cast, Any, ParamSpec, TypeVar
 
@@ -160,14 +161,28 @@
         except StopAsyncIteration:
             pass
     else:
         async for e in iterable:
             yield e
 
 
+async def async_chain(*iterables, threaded: bool = True):
+    for it in iterables:
+        async for e in ensure_aiter(it, threaded=threaded):
+            yield e
+
+
+async def async_chain_from_iterable(iterable, /, threaded: bool = True):
+    async for it in ensure_aiter(iterable, threaded=False):
+        async for e in ensure_aiter(it, threaded=threaded):
+            yield e
+
+setattr(async_chain, "from_iterable", async_chain_from_iterable)
+
+
 async def call_as_aiter(
     func: Callable[[], T] | Callable[[], Awaitable[T]], 
     /, 
     sentinel = undefined, 
     threaded: bool = True, 
 ) -> AsyncIterator[T]:
     func = ensure_async(func, threaded=threaded)
```

### Comparing `python_asynctools-0.0.2.1/pyproject.toml` & `python_asynctools-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-asynctools"
-version = "0.0.2.1"
+version = "0.0.3"
 description = "Python asynchronous tools."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-asynctools"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-asynctools"
 keywords = ["asynchronous", "tools"]
```

### Comparing `python_asynctools-0.0.2.1/PKG-INFO` & `python_asynctools-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-asynctools
-Version: 0.0.2.1
+Version: 0.0.3
 Summary: Python asynchronous tools.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-asynctools
 License: MIT
 Keywords: asynchronous,tools
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

