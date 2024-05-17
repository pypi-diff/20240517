# Comparing `tmp/msqlite-0.2.3.tar.gz` & `tmp/msqlite-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msqlite-0.2.3.tar", last modified: Fri Mar 29 19:06:24 2024, max compression
+gzip compressed data, was "msqlite-0.3.0.tar", last modified: Fri Mar 29 20:31:32 2024, max compression
```

## Comparing `msqlite-0.2.3.tar` & `msqlite-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 19:06:24.907656 msqlite-0.2.3/
--rw-rw-rw-   0        0        0     1088 2024-03-10 05:30:02.000000 msqlite-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     3242 2024-03-29 19:06:24.905582 msqlite-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1457 2024-03-12 22:40:35.000000 msqlite-0.2.3/README.md
--rw-rw-rw-   0        0        0      699 2024-03-29 19:04:54.000000 msqlite-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-29 19:06:24.907656 msqlite-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-29 19:06:24.870579 msqlite-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-29 19:06:24.880003 msqlite-0.2.3/src/msqlite/
--rw-rw-rw-   0        0        0       54 2024-03-14 21:04:48.000000 msqlite-0.2.3/src/msqlite/__init__.py
--rw-rw-rw-   0        0        0     5070 2024-03-29 19:03:42.000000 msqlite-0.2.3/src/msqlite/msqlite.py
--rw-rw-rw-   0        0        0        0 2024-03-26 01:08:19.000000 msqlite-0.2.3/src/msqlite/py.typed
-drwxrwxrwx   0        0        0        0 2024-03-29 19:06:24.904538 msqlite-0.2.3/src/msqlite.egg-info/
--rw-rw-rw-   0        0        0     3242 2024-03-29 19:06:24.000000 msqlite-0.2.3/src/msqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-03-29 19:06:24.000000 msqlite-0.2.3/src/msqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 19:06:24.000000 msqlite-0.2.3/src/msqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-29 19:06:24.000000 msqlite-0.2.3/src/msqlite.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-29 20:31:32.044885 msqlite-0.3.0/
+-rw-rw-rw-   0        0        0     1088 2024-03-10 05:30:02.000000 msqlite-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     3242 2024-03-29 20:31:32.043750 msqlite-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1457 2024-03-12 22:40:35.000000 msqlite-0.3.0/README.md
+-rw-rw-rw-   0        0        0      699 2024-03-29 20:14:25.000000 msqlite-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-29 20:31:32.044885 msqlite-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-29 20:31:32.006038 msqlite-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-03-29 20:31:32.015652 msqlite-0.3.0/src/msqlite/
+-rw-rw-rw-   0        0        0       75 2024-03-29 20:28:29.000000 msqlite-0.3.0/src/msqlite/__init__.py
+-rw-rw-rw-   0        0        0     5437 2024-03-29 20:30:12.000000 msqlite-0.3.0/src/msqlite/msqlite.py
+-rw-rw-rw-   0        0        0        0 2024-03-26 01:08:19.000000 msqlite-0.3.0/src/msqlite/py.typed
+drwxrwxrwx   0        0        0        0 2024-03-29 20:31:32.041635 msqlite-0.3.0/src/msqlite.egg-info/
+-rw-rw-rw-   0        0        0     3242 2024-03-29 20:31:31.000000 msqlite-0.3.0/src/msqlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-03-29 20:31:31.000000 msqlite-0.3.0/src/msqlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-29 20:31:31.000000 msqlite-0.3.0/src/msqlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-03-29 20:31:31.000000 msqlite-0.3.0/src/msqlite.egg-info/top_level.txt
```

### Comparing `msqlite-0.2.3/LICENSE` & `msqlite-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `msqlite-0.2.3/PKG-INFO` & `msqlite-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msqlite
-Version: 0.2.3
+Version: 0.3.0
 Summary: Execute simple SQLite statements that are multithreaded/multiprocess safe
 Author-email: James Abel <j@abel.co>
 License: MIT License
         
         Copyright (c) 2024 James Abel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `msqlite-0.2.3/README.md` & `msqlite-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `msqlite-0.2.3/pyproject.toml` & `msqlite-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msqlite"
-version = "0.2.3"
+version = "0.3.0"
 description = "Execute simple SQLite statements that are multithreaded/multiprocess safe"
 readme = "README.md"
 authors = [{ name = "James Abel", email = "j@abel.co" }]
 license = { file="LICENSE" }
 keywords = ["sqlite", "multithread", "multiprocess"]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `msqlite-0.2.3/src/msqlite/msqlite.py` & `msqlite-0.3.0/src/msqlite/msqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 import sqlite3
 from logging import getLogger
 import time
 import random
 from pathlib import Path
 from typing import Type
+import json
 
 log = getLogger()
 
 
 class MSQLiteMaxRetriesError(sqlite3.OperationalError):
     pass
 
 
 type_to_sqlite_type = {
     int: "INTEGER",
+    "int": "INTEGER",
     float: "REAL",
+    "float": "REAL",
     str: "TEXT",
+    "str": "TEXT",
     bytes: "BLOB",
+    "bytes": "BLOB",
     bool: "INTEGER",
+    "bool": "INTEGER",
+    json: "JSON",
+    "JSON": "JSON",
     type(None): "NULL",
+    "None": "NULL",
 }
 
 
 def _convert_column_dict_to_sqlite(column_spec: str, column_type: Type) -> str:
     """
     Convert a column specification to a SQLite column specification.
     :param column_spec: column name and optional constraints. Example: "id PRIMARY KEY"
     :param column_type: column type (Python types such as int, float, str, etc.). Example: int
     :return: column specification string for SQLite
     """
     column_spec_parts = column_spec.split()
     assert len(column_spec_parts) > 0  # at least the column name
     column_name = column_spec_parts[0]
-    column_type_string = type_to_sqlite_type[column_type]
+    if (column_type_string := type_to_sqlite_type.get(column_type)) is None:
+        raise ValueError(f"{column_type} (type={type(column_type)}) is not a supported SQLite column type (see msqlite.type_to_sqlite_type for supported types)")
     if len(column_spec_parts) > 1:
         constraints = column_spec_parts[1:]
     else:
         constraints = []
     spec_components = [column_name, column_type_string]
     spec_components.extend(constraints)
     spec = " ".join(spec_components)
```

### Comparing `msqlite-0.2.3/src/msqlite.egg-info/PKG-INFO` & `msqlite-0.3.0/src/msqlite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msqlite
-Version: 0.2.3
+Version: 0.3.0
 Summary: Execute simple SQLite statements that are multithreaded/multiprocess safe
 Author-email: James Abel <j@abel.co>
 License: MIT License
         
         Copyright (c) 2024 James Abel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

