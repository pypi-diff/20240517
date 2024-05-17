# Comparing `tmp/datagov_harvesting_logic-0.4.2.tar.gz` & `tmp/datagov_harvesting_logic-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagov_harvesting_logic-0.4.2.tar", max compression
+gzip compressed data, was "datagov_harvesting_logic-0.4.4.tar", max compression
```

## Comparing `datagov_harvesting_logic-0.4.2.tar` & `datagov_harvesting_logic-0.4.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1878 2024-05-10 20:27:44.878631 datagov_harvesting_logic-0.4.2/LICENSE.md
--rw-r--r--   0        0        0     5935 2024-05-10 20:27:44.878631 datagov_harvesting_logic-0.4.2/README.md
--rw-r--r--   0        0        0      164 2024-05-10 20:27:44.882631 datagov_harvesting_logic-0.4.2/harvester/__init__.py
--rw-r--r--   0        0        0     8369 2024-05-10 20:27:44.882631 datagov_harvesting_logic-0.4.2/harvester/ckan_utils.py
--rw-r--r--   0        0        0     2158 2024-05-10 20:27:44.882631 datagov_harvesting_logic-0.4.2/harvester/exceptions.py
--rw-r--r--   0        0        0    14138 2024-05-10 20:27:44.882631 datagov_harvesting_logic-0.4.2/harvester/harvest.py
--rw-r--r--   0        0        0      589 2024-05-10 20:27:44.882631 datagov_harvesting_logic-0.4.2/harvester/logger_config.py
--rw-r--r--   0        0        0     4058 2024-05-10 20:27:44.882631 datagov_harvesting_logic-0.4.2/harvester/utils.py
--rw-r--r--   0        0        0     2275 2024-05-10 20:27:44.886631 datagov_harvesting_logic-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     7180 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1878 2024-05-17 14:55:55.722791 datagov_harvesting_logic-0.4.4/LICENSE.md
+-rw-r--r--   0        0        0     5935 2024-05-17 14:55:55.722791 datagov_harvesting_logic-0.4.4/README.md
+-rw-r--r--   0        0        0      164 2024-05-17 14:55:55.726791 datagov_harvesting_logic-0.4.4/harvester/__init__.py
+-rw-r--r--   0        0        0     8369 2024-05-17 14:55:55.726791 datagov_harvesting_logic-0.4.4/harvester/ckan_utils.py
+-rw-r--r--   0        0        0     2158 2024-05-17 14:55:55.726791 datagov_harvesting_logic-0.4.4/harvester/exceptions.py
+-rw-r--r--   0        0        0    14138 2024-05-17 14:55:55.726791 datagov_harvesting_logic-0.4.4/harvester/harvest.py
+-rw-r--r--   0        0        0      589 2024-05-17 14:55:55.726791 datagov_harvesting_logic-0.4.4/harvester/logger_config.py
+-rw-r--r--   0        0        0     4058 2024-05-17 14:55:55.726791 datagov_harvesting_logic-0.4.4/harvester/utils.py
+-rw-r--r--   0        0        0     2297 2024-05-17 14:55:55.730791 datagov_harvesting_logic-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     7180 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.4.4/PKG-INFO
```

### Comparing `datagov_harvesting_logic-0.4.2/LICENSE.md` & `datagov_harvesting_logic-0.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.2/README.md` & `datagov_harvesting_logic-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.2/harvester/ckan_utils.py` & `datagov_harvesting_logic-0.4.4/harvester/ckan_utils.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.2/harvester/exceptions.py` & `datagov_harvesting_logic-0.4.4/harvester/exceptions.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.2/harvester/harvest.py` & `datagov_harvesting_logic-0.4.4/harvester/harvest.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.2/harvester/logger_config.py` & `datagov_harvesting_logic-0.4.4/harvester/logger_config.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.2/harvester/utils.py` & `datagov_harvesting_logic-0.4.4/harvester/utils.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.2/pyproject.toml` & `datagov_harvesting_logic-0.4.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datagov-harvesting-logic"
-version = "0.4.2"
+version = "0.4.4"
 description = ""
 # authors = [
 #     {name = "Jin Sun", email = "jin.sun@gsa.gov"},
 #     {name = "Tyler Burton", email = "tyler.burton@gsa.gov"},
 # ]
 authors = [
     "Datagov Team <datagov@gsa.gov>",
@@ -37,14 +37,15 @@
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.3.2"
 ruff = "^0.0.291"
 pytest-cov = "^4.0.0"
 debugpy = "^1.8.1"
 isort = "^5.13.2"
 black = "^24.4.2"
+pre-commit = "^3.7.1"
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
 select = ["E", "F"]
 ignore = []
 ignore-init-module-imports = true
```

### Comparing `datagov_harvesting_logic-0.4.2/PKG-INFO` & `datagov_harvesting_logic-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagov-harvesting-logic
-Version: 0.4.2
+Version: 0.4.4
 Summary: 
 Home-page: https://github.com/GSA/datagov-harvesting-logic
 License: LICENSE.md
 Author: Datagov Team
 Author-email: datagov@gsa.gov
 Maintainer: Datagov Team
 Maintainer-email: datagov@gsa.gov
```

