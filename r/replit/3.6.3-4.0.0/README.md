# Comparing `tmp/replit-3.6.3.tar.gz` & `tmp/replit-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit-3.6.3.tar", max compression
+gzip compressed data, was "replit-4.0.0.tar", max compression
```

## Comparing `replit-3.6.3.tar` & `replit-4.0.0.tar`

### file list

```diff
@@ -1,31 +1,27 @@
--rw-r--r--   0        0        0      720 2024-05-03 16:45:51.578735 replit-3.6.3/LICENSE
--rw-r--r--   0        0        0     1491 2024-05-03 16:45:51.578735 replit-3.6.3/README.md
--rw-r--r--   0        0        0     1487 2024-05-03 16:46:00.706749 replit-3.6.3/pyproject.toml
--rw-r--r--   0        0        0      798 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/__init__.py
--rw-r--r--   0        0        0     3029 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/__main__.py
--rw-r--r--   0        0        0      171 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/audio/Makefile
--rw-r--r--   0        0        0    13225 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/audio/__init__.py
--rw-r--r--   0        0        0     1848 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/audio/test.py
--rw-r--r--   0        0        0     3687 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/audio/types.py
--rw-r--r--   0        0        0      862 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/database/__init__.py
--rw-r--r--   0        0        0    24466 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/database/database.py
--rw-r--r--   0        0        0     1521 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/database/default_db.py
--rw-r--r--   0        0        0     2642 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/database/server.py
--rw-r--r--   0        0        0       33 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/goval/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/goval/api/__init__.py
--rw-r--r--   0        0        0     5800 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/goval/api/client_pb2.py
--rw-r--r--   0        0        0        0 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/goval/api/features/__init__.py
--rw-r--r--   0        0        0     1606 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/goval/api/features/features_pb2.py
--rw-r--r--   0        0        0        0 2024-05-03 16:45:51.582735 replit-3.6.3/src/replit/goval/api/repl/__init__.py
--rw-r--r--   0        0        0     4642 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/goval/api/repl/repl_pb2.py
--rw-r--r--   0        0        0     4963 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/goval/api/signing_pb2.py
--rw-r--r--   0        0        0      174 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/identity/__init__.py
--rw-r--r--   0        0        0      159 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/identity/exceptions.py
--rw-r--r--   0        0        0     2110 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/identity/sign.py
--rw-r--r--   0        0        0    13408 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/identity/verify.py
--rw-r--r--   0        0        0     2735 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/info.py
--rw-r--r--   0        0        0      733 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/web/__init__.py
--rw-r--r--   0        0        0     2640 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/web/app.py
--rw-r--r--   0        0        0     3667 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/web/user.py
--rw-r--r--   0        0        0     8607 2024-05-03 16:45:51.586735 replit-3.6.3/src/replit/web/utils.py
--rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 replit-3.6.3/PKG-INFO
+-rw-r--r--   0        0        0      720 2024-05-17 19:24:52.351583 replit-4.0.0/LICENSE
+-rw-r--r--   0        0        0     1429 2024-05-17 19:24:52.351583 replit-4.0.0/README.md
+-rw-r--r--   0        0        0     1487 2024-05-17 19:25:01.939611 replit-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0      755 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/__init__.py
+-rw-r--r--   0        0        0     3029 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/__main__.py
+-rw-r--r--   0        0        0      862 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/database/__init__.py
+-rw-r--r--   0        0        0    24466 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/database/database.py
+-rw-r--r--   0        0        0     1521 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/database/default_db.py
+-rw-r--r--   0        0        0     2642 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/database/server.py
+-rw-r--r--   0        0        0       33 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/goval/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/goval/api/__init__.py
+-rw-r--r--   0        0        0     5800 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/goval/api/client_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/goval/api/features/__init__.py
+-rw-r--r--   0        0        0     1606 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/goval/api/features/features_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/goval/api/repl/__init__.py
+-rw-r--r--   0        0        0     4642 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/goval/api/repl/repl_pb2.py
+-rw-r--r--   0        0        0     4963 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/goval/api/signing_pb2.py
+-rw-r--r--   0        0        0      174 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/identity/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/identity/exceptions.py
+-rw-r--r--   0        0        0     2110 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/identity/sign.py
+-rw-r--r--   0        0        0    13408 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/identity/verify.py
+-rw-r--r--   0        0        0     2735 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/info.py
+-rw-r--r--   0        0        0      733 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/web/__init__.py
+-rw-r--r--   0        0        0     2640 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/web/app.py
+-rw-r--r--   0        0        0     3667 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/web/user.py
+-rw-r--r--   0        0        0     8607 2024-05-17 19:24:52.359583 replit-4.0.0/src/replit/web/utils.py
+-rw-r--r--   0        0        0     2471 1970-01-01 00:00:00.000000 replit-4.0.0/PKG-INFO
```

### Comparing `replit-3.6.3/LICENSE` & `replit-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/README.md` & `replit-4.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 [![Run on Repl.it](https://img.shields.io/badge/run-on_Replit-f26208?logo=replit)](https://repl.it/github/replit/replit-py) [![pypi: replit](https://img.shields.io/pypi/v/replit)](https://pypi.org/project/replit/) [![Read the Docs](https://img.shields.io/readthedocs/replit-py/latest?logo=readthedocs&label=ReadTheDocs)](https://replit-py.readthedocs.io/)
 
 This repository is the home for the `replit` Python package, which provides:
 
 - A fully-featured database client for [Replit DB](https://docs.replit.com/category/databases).
 - Tools and utilities for Flask Web Development, including an interface to Replit's User Authetication service
 - Replit user profile metadata retrieval (more coming here!).
-- A simple audio library that can play tones and audio files!
 
 ### Open Source License
 
 This library is licensed under the [ISC License](https://en.wikipedia.org/wiki/ISC_license) and is free for you to use, change, or even profit from!
 
 ### Setup
```

### Comparing `replit-3.6.3/pyproject.toml` & `replit-4.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "replit"
-version = "3.6.3"  # Set by GitHub Actions
+version = "4.0.0"  # Set by GitHub Actions
 description = "A library for interacting with features of Replit"
 authors = ["Replit <contact@replit.com>", "mat <pypi@matdoes.dev>", "kennethreitz <me@kennethreitz.org>", "Scoder12 <pypi@scoder12.ml>", "AllAwesome497", ]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/replit/replit-py"
 homepage = "https://github.com/replit/replit-py"
 documentation = "https://replit-py.readthedocs.org/"
```

### Comparing `replit-3.6.3/src/replit/__init__.py` & `replit-4.0.0/src/replit/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # flake8: noqa
 
 """The Replit Python module."""
 
 from typing import Any
 
 from . import database, web
-from .audio import Audio
 from .database import (
     Database,
     AsyncDatabase,
     make_database_proxy_blueprint,
     start_database_proxy,
 )
 from .info import ReplInfo
@@ -19,17 +18,14 @@
 
 # Backwards compatibility.
 def clear() -> None:
     """Clear the terminal."""
     print("\033[H\033[2J", end="", flush=True)
 
 
-audio = Audio()
-
-
 # Previous versions of this library would just have side-effects and always set
 # up a database unconditionally. That is very undesirable, so instead of doing
 # that, we are using this egregious hack to get the database / database URL
 # lazily.
 def __getattr__(name: str) -> Any:
     if name == "db":
         return database.db
```

### Comparing `replit-3.6.3/src/replit/__main__.py` & `replit-4.0.0/src/replit/__main__.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/src/replit/database/__init__.py` & `replit-4.0.0/src/replit/database/__init__.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/src/replit/database/database.py` & `replit-4.0.0/src/replit/database/database.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/src/replit/database/default_db.py` & `replit-4.0.0/src/replit/database/default_db.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/src/replit/database/server.py` & `replit-4.0.0/src/replit/database/server.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/src/replit/goval/api/client_pb2.py` & `replit-4.0.0/src/replit/goval/api/client_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/src/replit/goval/api/features/features_pb2.py` & `replit-4.0.0/src/replit/goval/api/features/features_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/src/replit/goval/api/repl/repl_pb2.py` & `replit-4.0.0/src/replit/goval/api/repl/repl_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/src/replit/goval/api/signing_pb2.py` & `replit-4.0.0/src/replit/goval/api/signing_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/src/replit/identity/sign.py` & `replit-4.0.0/src/replit/identity/sign.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/src/replit/identity/verify.py` & `replit-4.0.0/src/replit/identity/verify.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/src/replit/info.py` & `replit-4.0.0/src/replit/info.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/src/replit/web/__init__.py` & `replit-4.0.0/src/replit/web/__init__.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/src/replit/web/app.py` & `replit-4.0.0/src/replit/web/app.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/src/replit/web/user.py` & `replit-4.0.0/src/replit/web/user.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/src/replit/web/utils.py` & `replit-4.0.0/src/replit/web/utils.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.3/PKG-INFO` & `replit-4.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit
-Version: 3.6.3
+Version: 4.0.0
 Summary: A library for interacting with features of Replit
 Home-page: https://github.com/replit/replit-py
 License: ISC
 Author: Replit
 Author-email: contact@replit.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
@@ -31,15 +31,14 @@
 [![Run on Repl.it](https://img.shields.io/badge/run-on_Replit-f26208?logo=replit)](https://repl.it/github/replit/replit-py) [![pypi: replit](https://img.shields.io/pypi/v/replit)](https://pypi.org/project/replit/) [![Read the Docs](https://img.shields.io/readthedocs/replit-py/latest?logo=readthedocs&label=ReadTheDocs)](https://replit-py.readthedocs.io/)
 
 This repository is the home for the `replit` Python package, which provides:
 
 - A fully-featured database client for [Replit DB](https://docs.replit.com/category/databases).
 - Tools and utilities for Flask Web Development, including an interface to Replit's User Authetication service
 - Replit user profile metadata retrieval (more coming here!).
-- A simple audio library that can play tones and audio files!
 
 ### Open Source License
 
 This library is licensed under the [ISC License](https://en.wikipedia.org/wiki/ISC_license) and is free for you to use, change, or even profit from!
 
 ### Setup
```

