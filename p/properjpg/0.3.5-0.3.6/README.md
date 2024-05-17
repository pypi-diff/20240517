# Comparing `tmp/properjpg-0.3.5.tar.gz` & `tmp/properjpg-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "properjpg-0.3.5.tar", max compression
+gzip compressed data, was "properjpg-0.3.6.tar", max compression
```

## Comparing `properjpg-0.3.5.tar` & `properjpg-0.3.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2022-08-12 01:21:26.103821 properjpg-0.3.5/LICENSE
--rw-r--r--   0        0        0     5203 2022-08-23 02:35:03.717431 properjpg-0.3.5/README.rst
--rw-r--r--   0        0        0       22 2022-08-12 01:21:26.106920 properjpg-0.3.5/properjpg/__init__.py
--rw-r--r--   0        0        0     5659 2022-08-12 01:21:26.107078 properjpg-0.3.5/properjpg/cli.py
--rw-r--r--   0        0        0     1399 2022-08-12 01:21:26.107257 properjpg-0.3.5/properjpg/filesmanager.py
--rw-r--r--   0        0        0     4282 2022-08-12 01:21:26.107410 properjpg-0.3.5/properjpg/processing.py
--rw-r--r--   0        0        0     1175 2024-02-03 00:41:48.676304 properjpg-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     6254 1970-01-01 00:00:00.000000 properjpg-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-08-12 01:21:26.103821 properjpg-0.3.6/LICENSE
+-rw-r--r--   0        0        0     5203 2024-05-16 23:54:41.276575 properjpg-0.3.6/README.rst
+-rw-r--r--   0        0        0       22 2022-08-12 01:21:26.106920 properjpg-0.3.6/properjpg/__init__.py
+-rw-r--r--   0        0        0     5659 2022-08-12 01:21:26.107078 properjpg-0.3.6/properjpg/cli.py
+-rw-r--r--   0        0        0     1399 2022-08-12 01:21:26.107257 properjpg-0.3.6/properjpg/filesmanager.py
+-rw-r--r--   0        0        0     4282 2022-08-12 01:21:26.107410 properjpg-0.3.6/properjpg/processing.py
+-rw-r--r--   0        0        0     1175 2024-05-16 23:56:19.191222 properjpg-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     6254 1970-01-01 00:00:00.000000 properjpg-0.3.6/PKG-INFO
```

### Comparing `properjpg-0.3.5/LICENSE` & `properjpg-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `properjpg-0.3.5/README.rst` & `properjpg-0.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `properjpg-0.3.5/properjpg/cli.py` & `properjpg-0.3.6/properjpg/cli.py`

 * *Files identical despite different names*

### Comparing `properjpg-0.3.5/properjpg/filesmanager.py` & `properjpg-0.3.6/properjpg/filesmanager.py`

 * *Files identical despite different names*

### Comparing `properjpg-0.3.5/properjpg/processing.py` & `properjpg-0.3.6/properjpg/processing.py`

 * *Files identical despite different names*

### Comparing `properjpg-0.3.5/pyproject.toml` & `properjpg-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "properjpg"
-version = "0.3.5"
+version = "0.3.6"
 description = "CLI tool to convert almost any image to optimized JPEGs.Fast."
 authors = ["Vitor Loureiro <miseravel.cruller-0o@icloud.com>"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: End Users/Desktop",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.10",
```

### Comparing `properjpg-0.3.5/PKG-INFO` & `properjpg-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: properjpg
-Version: 0.3.5
+Version: 0.3.6
 Summary: CLI tool to convert almost any image to optimized JPEGs.Fast.
 Home-page: https://github.com/vitorrloureiro/properjpg
 License: MIT
 Keywords: image,optimize,jpg,conversor,web,cli
 Author: Vitor Loureiro
 Author-email: miseravel.cruller-0o@icloud.com
 Requires-Python: >=3.10,<4.0
```

