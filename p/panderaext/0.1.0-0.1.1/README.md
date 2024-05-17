# Comparing `tmp/panderaext-0.1.0.tar.gz` & `tmp/panderaext-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panderaext-0.1.0.tar", max compression
+gzip compressed data, was "panderaext-0.1.1.tar", max compression
```

## Comparing `panderaext-0.1.0.tar` & `panderaext-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2024-05-17 14:29:09.748475 panderaext-0.1.0/LICENSE
--rw-r--r--   0        0        0      170 2024-05-17 14:38:42.827017 panderaext-0.1.0/README.md
--rw-r--r--   0        0        0      542 2024-05-17 14:33:28.413515 panderaext-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 14:30:20.755787 panderaext-0.1.0/src/panderaext/__init__.py
--rw-r--r--   0        0        0      302 2023-02-22 09:30:19.137573 panderaext-0.1.0/src/panderaext/checks.py
--rw-r--r--   0        0        0     2211 2024-03-17 16:13:13.533942 panderaext-0.1.0/src/panderaext/schema_helper.py
--rw-r--r--   0        0        0     1270 2024-04-18 09:39:56.222200 panderaext-0.1.0/src/panderaext/serializable_check_types.py
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 panderaext-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-17 14:29:09.748475 panderaext-0.1.1/LICENSE
+-rw-r--r--   0        0        0      265 2024-05-17 14:42:49.606578 panderaext-0.1.1/README.md
+-rw-r--r--   0        0        0      542 2024-05-17 14:42:49.610812 panderaext-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 14:30:20.755787 panderaext-0.1.1/src/panderaext/__init__.py
+-rw-r--r--   0        0        0      302 2023-02-22 09:30:19.137573 panderaext-0.1.1/src/panderaext/checks.py
+-rw-r--r--   0        0        0     2211 2024-03-17 16:13:13.533942 panderaext-0.1.1/src/panderaext/schema_helper.py
+-rw-r--r--   0        0        0     1270 2024-04-18 09:39:56.222200 panderaext-0.1.1/src/panderaext/serializable_check_types.py
+-rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 panderaext-0.1.1/PKG-INFO
```

### Comparing `panderaext-0.1.0/LICENSE` & `panderaext-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panderaext-0.1.0/src/panderaext/schema_helper.py` & `panderaext-0.1.1/src/panderaext/schema_helper.py`

 * *Files identical despite different names*

### Comparing `panderaext-0.1.0/src/panderaext/serializable_check_types.py` & `panderaext-0.1.1/src/panderaext/serializable_check_types.py`

 * *Files identical despite different names*

### Comparing `panderaext-0.1.0/PKG-INFO` & `panderaext-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panderaext
-Version: 0.1.0
+Version: 0.1.1
 Summary: Extension of pandera type checking
 Home-page: https://github.com/artoby/panderaext
 License: MIT
 Keywords: pandera,schema,pandas
 Author: Artyom Vorobyov
 Author-email: artyom.vorobyov@gmail.com
 Requires-Python: >=3.10,<3.11
@@ -29,10 +29,14 @@
 ```
 
 # Usage
 
 ```python
 import pandas as pd
 import pandera as pa
+
+from panderaext.schema_helper import get_schema_columns
+
+cols = get_schema_columns(MyDataset)
 ...
 ```
```

