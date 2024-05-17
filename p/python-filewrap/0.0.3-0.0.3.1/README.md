# Comparing `tmp/python_filewrap-0.0.3.tar.gz` & `tmp/python_filewrap-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_filewrap-0.0.3.tar", max compression
+gzip compressed data, was "python_filewrap-0.0.3.1.tar", max compression
```

## Comparing `python_filewrap-0.0.3.tar` & `python_filewrap-0.0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.3/LICENSE
--rwxr-xr-x   0        0        0     9765 2024-05-16 15:59:19.428444 python_filewrap-0.0.3/filewrap/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.3/filewrap/py.typed
--rw-r--r--   0        0        0     1147 2024-05-16 15:59:32.162427 python_filewrap-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.3/readme.md
--rw-r--r--   0        0        0     1329 1970-01-01 00:00:00.000000 python_filewrap-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.3.1/LICENSE
+-rwxr-xr-x   0        0        0     9893 2024-05-16 16:17:24.244899 python_filewrap-0.0.3.1/filewrap/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.3.1/filewrap/py.typed
+-rw-r--r--   0        0        0     1149 2024-05-16 16:17:52.890490 python_filewrap-0.0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.3.1/readme.md
+-rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 python_filewrap-0.0.3.1/PKG-INFO
```

### Comparing `python_filewrap-0.0.3/LICENSE` & `python_filewrap-0.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_filewrap-0.0.3/filewrap/__init__.py` & `python_filewrap-0.0.3.1/filewrap/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -262,52 +262,56 @@
 ):
     async for _ in bio_skip_async_iter(bio, size, chunksize, callback=callback):
         pass
 
 
 def bytes_iter_to_reader(it: Iterable[bytes | bytearray], /) -> SupportsRead[bytes]:
     get_next = iter(it).__next__
-    unconsumed = bytearray(b"")
+    at_eof = False
+    unconsumed: bytearray = bytearray(b"")
     def read(n=-1):
-        nonlocal unconsumed
-        if n == 0:
+        nonlocal at_eof, unconsumed
+        if at_eof or n == 0:
             return b""
         try:
             if n < 0:
                 while True:
-                    unconsumed.extend(get_next())
+                    unconsumed += get_next()
             else:
                 while n > len(unconsumed):
-                    unconsumed.extend(get_next())
+                    unconsumed += get_next()
                 b, unconsumed = unconsumed[:n], unconsumed[n:]
                 return bytes(b)
         except StopIteration:
+            at_eof = True
             return bytes(unconsumed)
     reprs = f"<reader for {it!r}>"
     return type("reader", (), {"read": staticmethod(read), "__repr__": staticmethod(lambda: reprs)})()
 
 
 def bytes_iter_to_reader_async(it: Iterable[bytes | bytearray] | AsyncIterable[bytes | bytearray], /) -> SupportsRead[bytes]:
-    unconsumed = bytearray(b"")
     if isinstance(it, AsyncIterable):
         get_next = aiter(it).__anext__
     else:
         sync_next = iter(it).__next__
         get_next = lambda: to_thread(sync_next)
+    at_eof = False
+    unconsumed: bytearray = bytearray(b"")
     async def read(n=-1):
-        nonlocal unconsumed
-        if n == 0:
+        nonlocal at_eof, unconsumed
+        if at_eof or n == 0:
             return b""
         try:
             if n < 0:
                 while True:
-                    unconsumed.extend(await get_next())
+                    unconsumed += await get_next()
             else:
                 while n > len(unconsumed):
-                    unconsumed.extend(await get_next())
+                    unconsumed += await get_next()
                 b, unconsumed = unconsumed[:n], unconsumed[n:]
                 return bytes(b)
         except StopIteration:
+            at_eof = True
             return bytes(unconsumed)
     reprs = f"<reader for {it!r}>"
     return type("reader", (), {"read": staticmethod(read), "__repr__": staticmethod(lambda: reprs)})()
```

### Comparing `python_filewrap-0.0.3/pyproject.toml` & `python_filewrap-0.0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-filewrap"
-version = "0.0.3"
+version = "0.0.3.1"
 description = "Python file wrappers."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 keywords = ["file", "wrapper"]
```

### Comparing `python_filewrap-0.0.3/PKG-INFO` & `python_filewrap-0.0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-filewrap
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: Python file wrappers.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap
 License: MIT
 Keywords: file,wrapper
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

