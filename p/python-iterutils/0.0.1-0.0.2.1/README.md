# Comparing `tmp/python_iterutils-0.0.1.tar.gz` & `tmp/python_iterutils-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_iterutils-0.0.1.tar", max compression
+gzip compressed data, was "python_iterutils-0.0.2.1.tar", max compression
```

## Comparing `python_iterutils-0.0.1.tar` & `python_iterutils-0.0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_iterutils-0.0.1/LICENSE
--rwxr-xr-x   0        0        0     3123 2024-05-15 14:00:44.241026 python_iterutils-0.0.1/iterutils/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_iterutils-0.0.1/iterutils/py.typed
--rw-r--r--   0        0        0     1161 2024-05-15 14:06:28.358464 python_iterutils-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      208 2024-05-15 13:48:16.668636 python_iterutils-0.0.1/readme.md
--rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 python_iterutils-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_iterutils-0.0.2.1/LICENSE
+-rwxr-xr-x   0        0        0     3182 2024-05-17 09:56:38.276885 python_iterutils-0.0.2.1/iterutils/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_iterutils-0.0.2.1/iterutils/py.typed
+-rw-r--r--   0        0        0     1163 2024-05-17 10:05:02.519712 python_iterutils-0.0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      208 2024-05-15 13:48:16.668636 python_iterutils-0.0.2.1/readme.md
+-rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 python_iterutils-0.0.2.1/PKG-INFO
```

### Comparing `python_iterutils-0.0.1/LICENSE` & `python_iterutils-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_iterutils-0.0.1/iterutils/__init__.py` & `python_iterutils-0.0.2.1/iterutils/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 1)
-__all__ = ["iterable", "async_iterable", "acc_step", "cut_iter", "asyncify_iter"]
+__version__ = (0, 0, 2)
+__all__ = [
+    "iterable", "async_iterable", "foreach", "async_foreach", "through", "async_through", 
+    "wrap_iter", "wrap_aiter", "acc_step", "cut_iter", 
+]
 
-from asyncio import to_thread
-from collections.abc import AsyncGenerator, AsyncIterable, Generator, Iterable, Iterator
-from typing import overload, Any, Optional, TypeVar
+from collections.abc import AsyncIterable, AsyncIterator, Callable, Iterable, Iterator
+from typing import Any, TypeVar
 
+from asynctools import async_zip, ensure_async, ensure_aiter
 
-TI = TypeVar("TI")
-TO = TypeVar("TO")
+
+T = TypeVar("T")
 
 
 def iterable(it, /) -> bool:
     try:
         return isinstance(iter(it), Iterable)
     except TypeError:
         return False
@@ -24,86 +27,106 @@
 def async_iterable(it, /) -> bool:
     try:
         return isinstance(iter(it), AsyncIterable)
     except TypeError:
         return False
 
 
+def foreach(func: Callable, iterable, /, *iterables):
+    if iterables:
+        for args in zip(iterable, *iterables):
+            func(*args)
+    else:
+        for arg in iterable:
+            func(arg)
+
+
+async def async_foreach(func: Callable, iterable, /, *iterables, threaded: bool = True):
+    func = ensure_async(func, threaded=threaded)
+    if iterables:
+        async for args in async_zip(iterable, *iterables, threaded=threaded):
+            await func(*args)
+    else:
+        async for arg in ensure_aiter(iterable, threaded=threaded):
+            await func(arg)
+
+
+def through(it: Iterable, /):
+    for _ in it:
+        pass
+
+
+async def async_through(
+    it: Iterable | AsyncIterable, 
+    /, 
+    threaded: bool = True, 
+):
+    async for _ in ensure_aiter(it, threaded=threaded):
+        pass
+
+
+def wrap_iter(
+    it: Iterable[T], 
+    /, 
+    callprev: None | Callable[[T], Any] = None, 
+    callnext: None | Callable[[T], Any] = None,  
+) -> Iterator[T]:
+    if not callable(callprev):
+        callprev = None
+    if not callable(callnext):
+        callnext = None
+    for e in it:
+        if callprev:
+            callprev(e)
+        yield e
+        if callnext:
+            callnext(e)
+
+
+async def wrap_aiter(
+    it: Iterable[T] | AsyncIterable[T], 
+    /, 
+    callprev: None | Callable[[T], Any] = None, 
+    callnext: None | Callable[[T], Any] = None,  
+    threaded: bool = True, 
+) -> AsyncIterator[T]:
+    callprev = ensure_async(callprev) if callable(callprev) else None
+    callnext = ensure_async(callnext) if callable(callnext) else None
+    async for e in ensure_aiter(it, threaded=threaded):
+        if callprev:
+            await callprev(e)
+        yield e
+        if callnext:
+            await callnext(e)
+
+
 def acc_step(
     start: int, 
-    stop: Optional[int] = None, 
+    stop: None | int = None, 
     step: int = 1, 
 ) -> Iterator[tuple[int, int, int]]:
     if stop is None:
         start, stop = 0, start
     for i in range(start + step, stop, step):
         yield start, (start := i), step
     if start != stop:
         yield start, stop, stop - start
 
 
 def cut_iter(
     start: int, 
-    stop: Optional[int] = None, 
+    stop: None | int = None, 
     step: int = 1, 
 ) -> Iterator[tuple[int, int]]:
     if stop is None:
         start, stop = 0, start
     for start in range(start + step, stop, step):
         yield start, step
     if start != stop:
         yield stop, stop - start
 
 
-@overload
-async def _asyncify_iter(it: Generator[TI, TO, Any], /, wait_for_thread: bool) -> AsyncGenerator[TI, TO]: ...
-@overload
-async def _asyncify_iter(it: Iterable[TO], /, wait_for_thread: bool) -> AsyncGenerator[Any, TO]: ...
-async def _asyncify_iter(it, /, wait_for_thread: bool = False):
-    if wait_for_thread:
-        if isinstance(it, Generator):
-            send = it.send
-            def nextval(val):
-                try:
-                    return send(val), None
-                except BaseException as e:
-                    return None, e
-        else:
-            getnext = iter(it).__next__
-            def nextval(val):
-                try:
-                    return getnext(), None
-                except BaseException as e:
-                    return None, e
-        val = None
-        while True:
-            yield_val, exc = await to_thread(nextval, val)
-            if exc is None:
-                yield yield_val
-            elif isinstance(exc, StopIteration):
-                break
-            else:
-                raise exc
-    elif isinstance(it, Generator):
-        send = it.send
-        val = None
-        try:
-            while True:
-                val = yield send(val)
-        except StopIteration:
-            pass
-    else:
-        for val in it:
-            yield val
-
+async def iter_to_aiter():
+    for i in it:
+        yield i
 
-@overload
-def asyncify_iter(it: AsyncIterable[TO], /, wait_for_thread: bool) -> AsyncIterable[TO]: ...
-@overload
-def asyncify_iter(it: Generator[TI, TO, Any], /, wait_for_thread: bool) -> AsyncGenerator[TI, TO]: ...
-@overload
-def asyncify_iter(it: Iterable[TO], /, wait_for_thread: bool) -> AsyncGenerator[Any, TO]: ...
-def asyncify_iter(it, /, wait_for_thread: bool = False):
-    if isinstance(it, AsyncIterable):
-        return it
-    return _asyncify_iter(it, wait_for_thread=wait_for_thread)
```

### Comparing `python_iterutils-0.0.1/pyproject.toml` & `python_iterutils-0.0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-iterutils"
-version = "0.0.1"
+version = "0.0.2.1"
 description = "Python another itertools."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-iterutils"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-iterutils"
 keywords = ["iterable", "iterutils"]
```

### Comparing `python_iterutils-0.0.1/PKG-INFO` & `python_iterutils-0.0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iterutils
-Version: 0.0.1
+Version: 0.0.2.1
 Summary: Python another itertools.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-iterutils
 License: MIT
 Keywords: iterable,iterutils
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

