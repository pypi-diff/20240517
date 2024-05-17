# Comparing `tmp/rtorrent_rpc-0.6.2.tar.gz` & `tmp/rtorrent_rpc-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.6.2.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.6.4.tar", max compression
```

## Comparing `rtorrent_rpc-0.6.2.tar` & `rtorrent_rpc-0.6.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2024-05-11 00:46:47.770881 rtorrent_rpc-0.6.2/LICENSE
--rw-r--r--   0        0        0     2515 2024-05-11 00:46:47.770881 rtorrent_rpc-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     1669 2024-05-11 00:46:47.770881 rtorrent_rpc-0.6.2/readme.md
--rw-r--r--   0        0        0    29769 2024-05-11 00:46:47.774881 rtorrent_rpc-0.6.2/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2458 2024-05-11 00:46:47.774881 rtorrent_rpc-0.6.2/rtorrent_rpc/_jsonrpc/__init__.py
--rw-r--r--   0        0        0     3050 2024-05-11 00:46:47.774881 rtorrent_rpc-0.6.2/rtorrent_rpc/_jsonrpc/transport.py
--rw-r--r--   0        0        0     1235 2024-05-11 00:46:47.774881 rtorrent_rpc-0.6.2/rtorrent_rpc/_scgi.py
--rw-r--r--   0        0        0      803 2024-05-11 00:46:47.774881 rtorrent_rpc-0.6.2/rtorrent_rpc/_transport.py
--rw-r--r--   0        0        0     3920 2024-05-11 00:46:47.774881 rtorrent_rpc-0.6.2/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2024-05-11 00:46:47.774881 rtorrent_rpc-0.6.2/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 rtorrent_rpc-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-05-11 00:52:37.142597 rtorrent_rpc-0.6.4/LICENSE
+-rw-r--r--   0        0        0     2550 2024-05-11 00:52:37.142597 rtorrent_rpc-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     1669 2024-05-11 00:52:37.142597 rtorrent_rpc-0.6.4/readme.md
+-rw-r--r--   0        0        0    29769 2024-05-11 00:52:37.142597 rtorrent_rpc-0.6.4/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2458 2024-05-11 00:52:37.142597 rtorrent_rpc-0.6.4/rtorrent_rpc/_jsonrpc/__init__.py
+-rw-r--r--   0        0        0     3050 2024-05-11 00:52:37.142597 rtorrent_rpc-0.6.4/rtorrent_rpc/_jsonrpc/transport.py
+-rw-r--r--   0        0        0     1235 2024-05-11 00:52:37.142597 rtorrent_rpc-0.6.4/rtorrent_rpc/_scgi.py
+-rw-r--r--   0        0        0      803 2024-05-11 00:52:37.142597 rtorrent_rpc-0.6.4/rtorrent_rpc/_transport.py
+-rw-r--r--   0        0        0     3920 2024-05-11 00:52:37.142597 rtorrent_rpc-0.6.4/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2024-05-11 00:52:37.142597 rtorrent_rpc-0.6.4/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     2713 1970-01-01 00:00:00.000000 rtorrent_rpc-0.6.4/PKG-INFO
```

### Comparing `rtorrent_rpc-0.6.2/LICENSE` & `rtorrent_rpc-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.2/pyproject.toml` & `rtorrent_rpc-0.6.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.6.2"
+version = "0.6.4"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
@@ -21,17 +21,18 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 # dependencies
 typing-extensions = ">=4.7.1"
 bencode2 = ">=0.0.6,<1"
 urllib3 = "^2.2.1"
+orjson = { version = '>3.0.0,<4', optional = true }
 
-[tool.poetry.group.orjson.dependencies]
-orjson = ">3.9.0"
+[tool.poetry.extras]
+orjson = ['orjson']
 
 [tool.poetry.group.docs.dependencies]
 sphinx = { version = "^7.0.0", python = "^3.9" }
 furo = { version = "^2024.0.0", python = "^3.9" }
 
 [tool.poetry.group.dev.dependencies]
 # tests
```

### Comparing `rtorrent_rpc-0.6.2/readme.md` & `rtorrent_rpc-0.6.4/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.2/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.6.4/rtorrent_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.2/rtorrent_rpc/_jsonrpc/__init__.py` & `rtorrent_rpc-0.6.4/rtorrent_rpc/_jsonrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.2/rtorrent_rpc/_jsonrpc/transport.py` & `rtorrent_rpc-0.6.4/rtorrent_rpc/_jsonrpc/transport.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.2/rtorrent_rpc/_scgi.py` & `rtorrent_rpc-0.6.4/rtorrent_rpc/_scgi.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.2/rtorrent_rpc/_transport.py` & `rtorrent_rpc-0.6.4/rtorrent_rpc/_transport.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.2/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.6.4/rtorrent_rpc/helper.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.2/PKG-INFO` & `rtorrent_rpc-0.6.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.6.2
+Version: 0.6.4
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
@@ -14,15 +14,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
+Provides-Extra: orjson
 Requires-Dist: bencode2 (>=0.0.6,<1)
+Requires-Dist: orjson (>3.0.0,<4) ; extra == "orjson"
 Requires-Dist: typing-extensions (>=4.7.1)
 Requires-Dist: urllib3 (>=2.2.1,<3.0.0)
 Project-URL: Repository, https://github.com/trim21/rtorrent-rpc
 Description-Content-Type: text/markdown
 
 # Typed rtorrent rpc client
```

