# Comparing `tmp/python_filewrap-0.0.4.tar.gz` & `tmp/python_filewrap-0.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_filewrap-0.0.4.tar", max compression
+gzip compressed data, was "python_filewrap-0.0.4.1.tar", max compression
```

## Comparing `python_filewrap-0.0.4.tar` & `python_filewrap-0.0.4.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.4/LICENSE
--rwxr-xr-x   0        0        0    13273 2024-05-17 09:07:48.937126 python_filewrap-0.0.4/filewrap/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.4/filewrap/py.typed
--rw-r--r--   0        0        0     1171 2024-05-17 09:03:48.005534 python_filewrap-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.4/readme.md
--rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 python_filewrap-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.4.1/LICENSE
+-rwxr-xr-x   0        0        0    13237 2024-05-17 11:20:06.097879 python_filewrap-0.0.4.1/filewrap/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.4.1/filewrap/py.typed
+-rw-r--r--   0        0        0     1173 2024-05-17 11:21:04.523756 python_filewrap-0.0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.4.1/readme.md
+-rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 python_filewrap-0.0.4.1/PKG-INFO
```

### Comparing `python_filewrap-0.0.4/LICENSE` & `python_filewrap-0.0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_filewrap-0.0.4/filewrap/__init__.py` & `python_filewrap-0.0.4.1/filewrap/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -234,36 +234,36 @@
             await callback(length)
         yield length
 
 
 def bytes_iter_to_reader(
     it: Iterable[bytes | bytearray], 
     /, 
-) -> SupportsRead[bytes]:
+) -> SupportsRead[bytearray]:
     getnext = iter(it).__next__
     at_end = False
-    unconsumed: bytearray = bytearray(b"")
+    unconsumed: bytearray = bytearray()
     lock = Lock()
-    def read(n=-1, /) -> bytes:
+    def read(n=-1, /) -> bytearray:
         nonlocal at_end, unconsumed
         if at_end or n == 0:
-            return b""
+            return bytearray()
         with lock:
             try:
                 if n is None or n < 0:
                     while True:
                         unconsumed += getnext()
                 else:
                     while n > len(unconsumed):
                         unconsumed += getnext()
-                    b, unconsumed = bytes(unconsumed[:n]), unconsumed[n:]
+                    b, unconsumed = unconsumed[:n], unconsumed[n:]
                     return b
             except StopIteration:
                 at_end = True
-                return bytes(unconsumed)
+                return unconsumed
     def readinto(buf, /) -> int:
         nonlocal at_end, unconsumed
         if at_end or not (bufsize := len(buf)):
             return 0
         with lock:
             if bufsize <= len(unconsumed):
                 buf[:], unconsumed = unconsumed[:bufsize], unconsumed[bufsize:]
@@ -283,39 +283,39 @@
                         return bufsize
                     else:
                         buf[n:m] = b
                         n = m
             except StopIteration:
                 at_end = True
                 return n
-    def __next__() -> bytes:
+    def __next__() -> bytearray:
         nonlocal unconsumed, at_end
         if at_end:
             raise StopIteration
         if unconsumed:
             # search for b"\n"
             if (idx := unconsumed.find(49)) > -1:
                 idx += 1
-                b, unconsumed = bytes(unconsumed[:idx]), unconsumed[idx:]
+                b, unconsumed = unconsumed[:idx], unconsumed[idx:]
                 return b
         try:
             while True:
-                b = getnext()
-                if not b:
+                r = getnext()
+                if not r:
                     continue
-                if (idx := b.find(49)) > -1:
+                if (idx := r.find(49)) > -1:
                     idx += 1
-                    unconsumed += b[:idx]
-                    b, unconsumed = bytes(unconsumed), bytearray(b[idx:])
+                    unconsumed += r[:idx]
+                    b, unconsumed = unconsumed, bytearray(r[idx:])
                     return b
-                unconsumed += b
+                unconsumed += r
         except StopIteration:
             at_end = True
             if unconsumed:
-                return bytes(unconsumed)
+                return unconsumed
             raise
     reprs = f"<reader for {it!r}>"
     return type("reader", (), {
         "read": staticmethod(read), 
         "readinto": staticmethod(readinto), 
         "__iter__": lambda self, /: self, 
         "__next__": staticmethod(__next__), 
@@ -323,39 +323,39 @@
     })()
 
 
 def bytes_iter_to_async_reader(
     it: Iterable[bytes | bytearray] | AsyncIterable[bytes | bytearray], 
     /, 
     threaded: bool = True, 
-) -> SupportsRead[bytes]:
+) -> SupportsRead[bytearray]:
     if isinstance(it, AsyncIterable):
         getnext = aiter(it).__anext__
     else:
         getnext = ensure_async(iter(it).__next__, threaded=threaded)
     at_end = False
-    unconsumed: bytearray = bytearray(b"")
+    unconsumed: bytearray = bytearray()
     lock = AsyncLock()
-    async def read(n=-1, /) -> bytes:
+    async def read(n=-1, /) -> bytearray:
         nonlocal at_end, unconsumed
         if at_end or n == 0:
-            return b""
+            return bytearray()
         async with lock:
             try:
                 if n is None or n < 0:
                     while True:
                         unconsumed += await getnext()
                 else:
                     while n > len(unconsumed):
                         unconsumed += await getnext()
-                    b, unconsumed = bytes(unconsumed[:n]), unconsumed[n:]
+                    b, unconsumed = unconsumed[:n], unconsumed[n:]
                     return b
             except StopAsyncIteration:
                 at_end = True
-                return bytes(unconsumed)
+                return unconsumed
     async def readinto(buf, /) -> int:
         nonlocal at_end, unconsumed
         if at_end or not (bufsize := len(buf)):
             return 0
         async with lock:
             if bufsize <= len(unconsumed):
                 buf[:], unconsumed = unconsumed[:bufsize], unconsumed[bufsize:]
@@ -375,39 +375,39 @@
                         return bufsize
                     else:
                         buf[n:m] = b
                         n = m
             except StopAsyncIteration:
                 at_end = True
                 return n
-    async def __next__() -> bytes:
+    async def __next__() -> bytearray:
         nonlocal unconsumed, at_end
         if at_end:
             raise StopIteration
         if unconsumed:
             # search for b"\n"
             if (idx := unconsumed.find(49)) > -1:
                 idx += 1
-                b, unconsumed = bytes(unconsumed[:idx]), unconsumed[idx:]
+                b, unconsumed = unconsumed[:idx], unconsumed[idx:]
                 return b
         try:
             while True:
-                b = await getnext()
-                if not b:
+                r = await getnext()
+                if not r:
                     continue
-                if (idx := b.find(49)) > -1:
+                if (idx := r.find(49)) > -1:
                     idx += 1
-                    unconsumed += b[:idx]
-                    b, unconsumed = bytes(unconsumed), bytearray(b[idx:])
+                    unconsumed += r[:idx]
+                    b, unconsumed = unconsumed, bytearray(r[idx:])
                     return b
-                unconsumed += b
+                unconsumed += r
         except StopIteration:
             at_end = True
             if unconsumed:
-                return bytes(unconsumed)
+                return unconsumed
             raise
     reprs = f"<reader for {it!r}>"
     return type("reader", (), {
         "read": staticmethod(read), 
         "readinto": staticmethod(readinto), 
         "__iter__": lambda self, /: self, 
         "__next__": staticmethod(__next__),
```

### Comparing `python_filewrap-0.0.4/pyproject.toml` & `python_filewrap-0.0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-filewrap"
-version = "0.0.4"
+version = "0.0.4.1"
 description = "Python file wrappers."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 keywords = ["file", "wrapper"]
```

### Comparing `python_filewrap-0.0.4/PKG-INFO` & `python_filewrap-0.0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-filewrap
-Version: 0.0.4
+Version: 0.0.4.1
 Summary: Python file wrappers.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap
 License: MIT
 Keywords: file,wrapper
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

