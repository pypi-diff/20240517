# Comparing `tmp/python_filewrap-0.0.3.1.tar.gz` & `tmp/python_filewrap-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_filewrap-0.0.3.1.tar", max compression
+gzip compressed data, was "python_filewrap-0.0.4.tar", max compression
```

## Comparing `python_filewrap-0.0.3.1.tar` & `python_filewrap-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.3.1/LICENSE
--rwxr-xr-x   0        0        0     9893 2024-05-16 16:17:24.244899 python_filewrap-0.0.3.1/filewrap/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.3.1/filewrap/py.typed
--rw-r--r--   0        0        0     1149 2024-05-16 16:17:52.890490 python_filewrap-0.0.3.1/pyproject.toml
--rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.3.1/readme.md
--rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 python_filewrap-0.0.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.4/LICENSE
+-rwxr-xr-x   0        0        0    13273 2024-05-17 09:07:48.937126 python_filewrap-0.0.4/filewrap/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.4/filewrap/py.typed
+-rw-r--r--   0        0        0     1171 2024-05-17 09:03:48.005534 python_filewrap-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.4/readme.md
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 python_filewrap-0.0.4/PKG-INFO
```

### Comparing `python_filewrap-0.0.3.1/LICENSE` & `python_filewrap-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_filewrap-0.0.3.1/pyproject.toml` & `python_filewrap-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-filewrap"
-version = "0.0.3.1"
+version = "0.0.4"
 description = "Python file wrappers."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 keywords = ["file", "wrapper"]
@@ -23,14 +23,15 @@
 ]
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
+python-asynctools = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.packages]]
 include = "filewrap"
```

### Comparing `python_filewrap-0.0.3.1/PKG-INFO` & `python_filewrap-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-filewrap
-Version: 0.0.3.1
+Version: 0.0.4
 Summary: Python file wrappers.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap
 License: MIT
 Keywords: file,wrapper
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: python-asynctools
 Project-URL: Repository, https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap
 Description-Content-Type: text/markdown
 
 # Python file wrappers.
 
 ## Installation
```

