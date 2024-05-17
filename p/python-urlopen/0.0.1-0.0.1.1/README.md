# Comparing `tmp/python_urlopen-0.0.1.tar.gz` & `tmp/python_urlopen-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_urlopen-0.0.1.tar", max compression
+gzip compressed data, was "python_urlopen-0.0.1.1.tar", max compression
```

## Comparing `python_urlopen-0.0.1.tar` & `python_urlopen-0.0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_urlopen-0.0.1/LICENSE
--rw-r--r--   0        0        0     1179 2024-05-14 12:34:40.672688 python_urlopen-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      213 2024-05-02 13:37:47.661441 python_urlopen-0.0.1/readme.md
--rwxr-xr-x   0        0        0     7231 2024-05-14 12:13:17.352415 python_urlopen-0.0.1/urlopen/__init__.py
--rwxr-xr-x   0        0        0     2768 2024-05-14 12:33:59.520772 python_urlopen-0.0.1/urlopen/__main__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_urlopen-0.0.1/urlopen/py.typed
--rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 python_urlopen-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_urlopen-0.0.1.1/LICENSE
+-rw-r--r--   0        0        0     1204 2024-05-17 11:37:50.503432 python_urlopen-0.0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      839 2024-05-14 12:36:18.615669 python_urlopen-0.0.1.1/readme.md
+-rwxr-xr-x   0        0        0     7268 2024-05-17 11:37:04.011875 python_urlopen-0.0.1.1/urlopen/__init__.py
+-rwxr-xr-x   0        0        0     2768 2024-05-14 12:33:59.520772 python_urlopen-0.0.1.1/urlopen/__main__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_urlopen-0.0.1.1/urlopen/py.typed
+-rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 python_urlopen-0.0.1.1/PKG-INFO
```

### Comparing `python_urlopen-0.0.1/LICENSE` & `python_urlopen-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_urlopen-0.0.1/pyproject.toml` & `python_urlopen-0.0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-urlopen"
-version = "0.0.1"
+version = "0.0.1.1"
 description = "Python urlopen wrapper."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-urlopen"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-urlopen"
 keywords = ["urlopen"]
@@ -25,14 +25,15 @@
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 http_response = "*"
 python-filewrap = "*"
+python-iterutils = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.packages]]
 include = "urlopen"
```

### Comparing `python_urlopen-0.0.1/urlopen/__init__.py` & `python_urlopen-0.0.1.1/urlopen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 from os.path import abspath, dirname, isdir, join as joinpath
 from shutil import COPY_BUFSIZE # type: ignore
 from ssl import SSLContext, _create_unverified_context
 from typing import cast, Any, Optional
 from urllib.parse import urlencode, urlsplit
 from urllib.request import build_opener, HTTPSHandler, OpenerDirector, Request
 
-from filewrap import bio_skip_bytes, SupportsRead, SupportsWrite
+from filewrap import bio_skip_iter, SupportsRead, SupportsWrite
 from http_response import get_filename, get_length, is_chunked, is_range_request
+from iterutils import foreach
 
 
 if "__del__" not in HTTPResponse.__dict__:
     setattr(HTTPResponse, "__del__", HTTPResponse.close)
 
 
 def urlopen(
@@ -191,15 +192,15 @@
                 resp.close()
                 resp = urlopen(url, headers={**headers, "Range": "bytes=%d-" % filesize}, **urlopen_kwargs)
                 if not is_range_request(resp):
                     raise OSError(errno.EIO, f"range request failed: {url!r}")
                 if reporthook:
                     reporthook(filesize)
             elif resume:
-                bio_skip_bytes(resp, filesize, callback=reporthook)
+                foreach(bio_skip_iter(resp, filesize, callback=reporthook))
 
         fsrc_read = resp.read 
         fdst_write = fdst.write
         while (chunk := fsrc_read(chunksize)):
             fdst_write(chunk)
             if reporthook:
                 reporthook(len(chunk))
```

### Comparing `python_urlopen-0.0.1/urlopen/__main__.py` & `python_urlopen-0.0.1.1/urlopen/__main__.py`

 * *Files identical despite different names*

