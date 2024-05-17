# Comparing `tmp/python_httpfile-0.0.1.tar.gz` & `tmp/python_httpfile-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_httpfile-0.0.1.tar", max compression
+gzip compressed data, was "python_httpfile-0.0.1.1.tar", max compression
```

## Comparing `python_httpfile-0.0.1.tar` & `python_httpfile-0.0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_httpfile-0.0.1/LICENSE
--rwxr-xr-x   0        0        0    12280 2024-05-15 06:47:36.835871 python_httpfile-0.0.1/httpfile/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_httpfile-0.0.1/httpfile/py.typed
--rw-r--r--   0        0        0     1272 2024-05-15 06:47:53.837467 python_httpfile-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      204 2024-05-14 12:38:16.912358 python_httpfile-0.0.1/readme.md
--rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 python_httpfile-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_httpfile-0.0.1.1/LICENSE
+-rwxr-xr-x   0        0        0    12317 2024-05-17 11:30:47.203278 python_httpfile-0.0.1.1/httpfile/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_httpfile-0.0.1.1/httpfile/py.typed
+-rw-r--r--   0        0        0     1297 2024-05-17 11:32:30.904487 python_httpfile-0.0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      204 2024-05-14 12:38:16.912358 python_httpfile-0.0.1.1/readme.md
+-rw-r--r--   0        0        0     1542 1970-01-01 00:00:00.000000 python_httpfile-0.0.1.1/PKG-INFO
```

### Comparing `python_httpfile-0.0.1/LICENSE` & `python_httpfile-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_httpfile-0.0.1/httpfile/__init__.py` & `python_httpfile-0.0.1.1/httpfile/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 from os import fstat, stat, PathLike
 from shutil import COPY_BUFSIZE # type: ignore
 from typing import Any, BinaryIO, IO, Optional, Protocol, Self, TypeVar
 from types import MappingProxyType
 from warnings import warn
 
 from aiohttp import ClientSession
-from filewrap import bio_skip_bytes
+from filewrap import bio_skip_iter
 from http_response import get_filename, get_length, get_range, get_total_length, is_chunked, is_range_request
+from iterutils import foreach
 from property import funcproperty
 from requests import Session
 from urlopen import urlopen
 
 
 def get_filesize(file, /, dont_read: bool = True) -> int:
     if isinstance(file, (bytes, str, PathLike)):
@@ -289,15 +290,15 @@
         if whence == 0:
             if pos < 0:
                 raise OSError(errno.EINVAL, f"negative seek start: {pos!r}")
             old_pos = self.tell()
             if old_pos == pos:
                 return pos
             if pos > old_pos and pos - old_pos <= self.seek_threshold:
-                bio_skip_bytes(self, pos - old_pos)
+                foreach(bio_skip_iter(self, pos - old_pos))
             else:
                 self.reconnect(pos)
             return pos
         elif whence == 1:
             if pos == 0:
                 return self.tell()
             return self.seek(self.tell() + pos)
```

### Comparing `python_httpfile-0.0.1/pyproject.toml` & `python_httpfile-0.0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-httpfile"
-version = "0.0.1"
+version = "0.0.1.1"
 description = "Python httpfile classes."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-httpfile"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-httpfile"
 keywords = ["http", "file", "wrapper"]
@@ -26,14 +26,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "*"
 http_response = "*"
 python-filewrap = "*"
+python-iterutils = "*"
 python-property = "*"
 python-urlopen = "*"
 requests = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `python_httpfile-0.0.1/PKG-INFO` & `python_httpfile-0.0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-httpfile
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Python httpfile classes.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-httpfile
 License: MIT
 Keywords: http,file,wrapper
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp
 Requires-Dist: http_response
 Requires-Dist: python-filewrap
+Requires-Dist: python-iterutils
 Requires-Dist: python-property
 Requires-Dist: python-urlopen
 Requires-Dist: requests
 Project-URL: Repository, https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-httpfile
 Description-Content-Type: text/markdown
 
 # Python httpfile classes.
```

