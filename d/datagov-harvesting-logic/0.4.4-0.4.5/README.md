# Comparing `tmp/datagov_harvesting_logic-0.4.4.tar.gz` & `tmp/datagov_harvesting_logic-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagov_harvesting_logic-0.4.4.tar", max compression
+gzip compressed data, was "datagov_harvesting_logic-0.4.5.tar", max compression
```

## Comparing `datagov_harvesting_logic-0.4.4.tar` & `datagov_harvesting_logic-0.4.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1878 2024-05-17 14:55:55.722791 datagov_harvesting_logic-0.4.4/LICENSE.md
--rw-r--r--   0        0        0     5935 2024-05-17 14:55:55.722791 datagov_harvesting_logic-0.4.4/README.md
--rw-r--r--   0        0        0      164 2024-05-17 14:55:55.726791 datagov_harvesting_logic-0.4.4/harvester/__init__.py
--rw-r--r--   0        0        0     8369 2024-05-17 14:55:55.726791 datagov_harvesting_logic-0.4.4/harvester/ckan_utils.py
--rw-r--r--   0        0        0     2158 2024-05-17 14:55:55.726791 datagov_harvesting_logic-0.4.4/harvester/exceptions.py
--rw-r--r--   0        0        0    14138 2024-05-17 14:55:55.726791 datagov_harvesting_logic-0.4.4/harvester/harvest.py
--rw-r--r--   0        0        0      589 2024-05-17 14:55:55.726791 datagov_harvesting_logic-0.4.4/harvester/logger_config.py
--rw-r--r--   0        0        0     4058 2024-05-17 14:55:55.726791 datagov_harvesting_logic-0.4.4/harvester/utils.py
--rw-r--r--   0        0        0     2297 2024-05-17 14:55:55.730791 datagov_harvesting_logic-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     7180 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1878 2024-05-17 17:49:47.969693 datagov_harvesting_logic-0.4.5/LICENSE.md
+-rw-r--r--   0        0        0     5935 2024-05-17 17:49:47.969693 datagov_harvesting_logic-0.4.5/README.md
+-rw-r--r--   0        0        0      164 2024-05-17 17:49:47.977693 datagov_harvesting_logic-0.4.5/harvester/__init__.py
+-rw-r--r--   0        0        0     8369 2024-05-17 17:49:47.977693 datagov_harvesting_logic-0.4.5/harvester/ckan_utils.py
+-rw-r--r--   0        0        0     2158 2024-05-17 17:49:47.977693 datagov_harvesting_logic-0.4.5/harvester/exceptions.py
+-rw-r--r--   0        0        0    14138 2024-05-17 17:49:47.977693 datagov_harvesting_logic-0.4.5/harvester/harvest.py
+-rw-r--r--   0        0        0      589 2024-05-17 17:49:47.977693 datagov_harvesting_logic-0.4.5/harvester/logger_config.py
+-rw-r--r--   0        0        0     4058 2024-05-17 17:49:47.977693 datagov_harvesting_logic-0.4.5/harvester/utils.py
+-rw-r--r--   0        0        0     2297 2024-05-17 17:49:47.977693 datagov_harvesting_logic-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     7180 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.4.5/PKG-INFO
```

### Comparing `datagov_harvesting_logic-0.4.4/LICENSE.md` & `datagov_harvesting_logic-0.4.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.4/README.md` & `datagov_harvesting_logic-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.4/harvester/ckan_utils.py` & `datagov_harvesting_logic-0.4.5/harvester/ckan_utils.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.4/harvester/exceptions.py` & `datagov_harvesting_logic-0.4.5/harvester/exceptions.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.4/harvester/harvest.py` & `datagov_harvesting_logic-0.4.5/harvester/harvest.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.4/harvester/logger_config.py` & `datagov_harvesting_logic-0.4.5/harvester/logger_config.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.4/harvester/utils.py` & `datagov_harvesting_logic-0.4.5/harvester/utils.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.4/pyproject.toml` & `datagov_harvesting_logic-0.4.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datagov-harvesting-logic"
-version = "0.4.4"
+version = "0.4.5"
 description = ""
 # authors = [
 #     {name = "Jin Sun", email = "jin.sun@gsa.gov"},
 #     {name = "Tyler Burton", email = "tyler.burton@gsa.gov"},
 # ]
 authors = [
     "Datagov Team <datagov@gsa.gov>",
```

### Comparing `datagov_harvesting_logic-0.4.4/PKG-INFO` & `datagov_harvesting_logic-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagov-harvesting-logic
-Version: 0.4.4
+Version: 0.4.5
 Summary: 
 Home-page: https://github.com/GSA/datagov-harvesting-logic
 License: LICENSE.md
 Author: Datagov Team
 Author-email: datagov@gsa.gov
 Maintainer: Datagov Team
 Maintainer-email: datagov@gsa.gov
```

