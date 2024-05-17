# Comparing `tmp/python_decotools-0.0.1.tar.gz` & `tmp/python_decotools-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_decotools-0.0.1.tar", max compression
+gzip compressed data, was "python_decotools-0.0.1.1.tar", max compression
```

## Comparing `python_decotools-0.0.1.tar` & `python_decotools-0.0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_decotools-0.0.1/LICENSE
--rwxr-xr-x   0        0        0     8913 2024-05-15 06:39:24.329773 python_decotools-0.0.1/decotools/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_decotools-0.0.1/decotools/py.typed
--rwxr-xr-x   0        0        0     4346 2024-05-01 15:56:13.284910 python_decotools-0.0.1/decotools/util.py
--rw-r--r--   0        0        0     1196 2024-05-15 06:38:02.844357 python_decotools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      206 2024-05-15 06:39:06.954400 python_decotools-0.0.1/readme.md
--rw-r--r--   0        0        0     1415 1970-01-01 00:00:00.000000 python_decotools-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_decotools-0.0.1.1/LICENSE
+-rwxr-xr-x   0        0        0     8976 2024-05-17 07:58:07.481242 python_decotools-0.0.1.1/decotools/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_decotools-0.0.1.1/decotools/py.typed
+-rwxr-xr-x   0        0        0     4460 2024-05-16 03:49:39.865839 python_decotools-0.0.1.1/decotools/util.py
+-rw-r--r--   0        0        0     1198 2024-05-17 08:00:13.138146 python_decotools-0.0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      194 2024-05-15 12:46:46.959377 python_decotools-0.0.1.1/readme.md
+-rw-r--r--   0        0        0     1405 1970-01-01 00:00:00.000000 python_decotools-0.0.1.1/PKG-INFO
```

### Comparing `python_decotools-0.0.1/LICENSE` & `python_decotools-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_decotools-0.0.1/decotools/__init__.py` & `python_decotools-0.0.1.1/decotools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,27 +17,28 @@
 from partial import ppartial
 from undefined import undefined
 
 
 Args = ParamSpec("Args")
 Args0 = ParamSpec("Args0")
 R = TypeVar("R")
+T = TypeVar("T")
 
 
 def update_wrapper(f, g, /, *args, **kwds):
     if f is g:
         return f
     else:
         return _update_wrapper(f, g, *args, **kwds)
 
 
 def decorated(
-    f: Callable[Concatenate[Callable[Args, R], Args], R], 
+    f: Callable[Concatenate[Callable[Args, R], Args], T], 
     /, 
-) -> Callable[[Callable[Args, R]], Callable[Args, R]]:
+) -> Callable[[Callable[Args, R]], Callable[Args, T]]:
     """Transform the 2-layers decorator into 1-layer.
 
     @decorated
     def decorator(func, /, *args, **kwds):
         ...
         return func(*args, **kwds)
 
@@ -51,17 +52,18 @@
             return func(*args, **kwds)
         return functools.update_wrapper(wrapper, func)
     """
     return update_wrapper(lambda g, /: update_wrapper(lambda *a, **k: f(g, *a, **k), g), f)
 
 
 def optional(
-    f: Callable[Concatenate[Callable[Args, R], Args0], Callable[Args, R]], 
+    f: Callable[Concatenate[Callable[Args, R], Args0], Callable[Args, T]], 
     /, 
-) -> Callable[Concatenate[None, Args0], ppartial] | Callable[Concatenate[Callable[Args, R], Args0], Callable[Args, R]]:
+) -> Callable[Concatenate[None, Args0], Callable[[Callable[Args, R]], Callable[Args, T]]] \
+    | Callable[Concatenate[Callable[Args, R], Args0], Callable[Args, T]]:
     """This function decorates another decorator that with optional parameters.
     NOTE: Make sure that these optional parameters have default values.
 
     @optional
     def decorator(func=None, /, *args, **kwds):
         ...
         def wrapper(*args1, **kwds1):
@@ -156,17 +158,17 @@
             return update_wrapper(f(func, *args, **kwds), func)
         else:
             return ppartial(wrapped, undefined, func, *args, **kwds)
     return update_wrapper(wrapped, f)
 
 
 def optional_args(
-    f: Callable[Args0, Callable[Concatenate[Callable[Args, R], Args], R]], 
+    f: Callable[Args0, Callable[Concatenate[Callable[Args, R], Args], T]], 
     /,
-) -> Callable[Args0, Callable[[Callable[Args, R]], Callable[Args, R]]] | Callable[Concatenate[Callable[Args, R], Args0], Callable[Args, R]]:
+) -> Callable[Args0, Callable[[Callable[Args, R]], Callable[Args, T]]] | Callable[Concatenate[Callable[Args, R], Args0], Callable[Args, T]]:
     """This function decorates another decorator that with optional parameters.
     NOTE: Make sure that these optional parameters have default values.
 
     @optional
     def decorator(func=None, /, *args, **kwds):
         ...
         def wrapper(*args1, **kwds1):
```

### Comparing `python_decotools-0.0.1/decotools/util.py` & `python_decotools-0.0.1.1/decotools/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 __author__  = "ChenyangGao <https://chenyanggao.github.io>"
-__all__ = ["callback", "suppressed", "threaded", "timethis", "with_cm", "with_lock"]
+__all__ = ["callback", "suppressed", "threaded", "asynced", "timethis", "with_cm", "with_lock"]
 
 from _thread import start_new_thread
-from asyncio import Lock as AsyncLock
+from asyncio import Lock as AsyncLock, to_thread
 from concurrent.futures import Future
 from inspect import isawaitable, iscoroutinefunction
 from threading import Lock
 from time import perf_counter
 from typing import ContextManager, AsyncContextManager
 
 from undefined import undefined
@@ -88,14 +88,19 @@
         except BaseException as e:
             fu.set_exception(e)
     fu: Future = Future()
     start_new_thread(start_future, ())
     return fu
 
 
+@decorated
+def asynced(func, /, *args, **kwds):
+    return to_thread(func, *args, **kwds)
+
+
 @optional
 def timethis(func, /, output=lambda t: print(f"cost time: {t} s")):
     if iscoroutinefunction(func):
         async def wrapper(*args, **kwds):
             start = perf_counter()
             result = await func(*args, **kwds)
             callasync(output, perf_counter() - start)
```

### Comparing `python_decotools-0.0.1/pyproject.toml` & `python_decotools-0.0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-decotools"
-version = "0.0.1"
+version = "0.0.1.1"
 description = "Python decorator tools."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decotools"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decotools"
 keywords = ["decorator"]
```

### Comparing `python_decotools-0.0.1/PKG-INFO` & `python_decotools-0.0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-decotools
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Python decorator tools.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decotools
 License: MIT
 Keywords: decorator
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -22,23 +22,23 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: python-partial (>=0.0.4,<0.0.5)
 Requires-Dist: python-undefined
 Project-URL: Repository, https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decotools
 Description-Content-Type: text/markdown
 
-# Python decorator tools.
+# Python chunked iterator..
 
 ## Installation
 
-You can install from [pypi](https://pypi.org/project/python-decotools/)
+You can install from [pypi](https://pypi.org/project/chunkiter/)
 
 ```console
-pip install -U python-decotools
+pip install -U chunkiter
 ```
 
 ## Usage
 
 ```python
-import decotools
+import chunkiter
 ```
```

