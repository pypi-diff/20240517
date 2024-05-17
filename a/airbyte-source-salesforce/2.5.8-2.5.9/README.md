# Comparing `tmp/airbyte_source_salesforce-2.5.8.tar.gz` & `tmp/airbyte_source_salesforce-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_salesforce-2.5.8.tar", max compression
+gzip compressed data, was "airbyte_source_salesforce-2.5.9.tar", max compression
```

## Comparing `airbyte_source_salesforce-2.5.8.tar` & `airbyte_source_salesforce-2.5.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4568 2024-04-30 22:49:06.000000 airbyte_source_salesforce-2.5.8/README.md
--rw-r--r--   0        0        0      830 2024-05-01 00:02:14.834032 airbyte_source_salesforce-2.5.8/pyproject.toml
--rw-r--r--   0        0        0      131 2024-04-30 22:49:06.000000 airbyte_source_salesforce-2.5.8/source_salesforce/__init__.py
--rw-r--r--   0        0        0    17451 2024-04-30 22:49:06.000000 airbyte_source_salesforce-2.5.8/source_salesforce/api.py
--rw-r--r--   0        0        0     1621 2024-04-30 22:49:06.000000 airbyte_source_salesforce-2.5.8/source_salesforce/availability_strategy.py
--rw-r--r--   0        0        0      808 2024-04-30 22:49:06.000000 airbyte_source_salesforce-2.5.8/source_salesforce/exceptions.py
--rw-r--r--   0        0        0     3946 2024-04-30 22:49:06.000000 airbyte_source_salesforce-2.5.8/source_salesforce/rate_limiting.py
--rw-r--r--   0        0        0     1619 2024-04-30 22:49:06.000000 airbyte_source_salesforce-2.5.8/source_salesforce/run.py
--rw-r--r--   0        0        0    17796 2024-04-30 22:49:06.000000 airbyte_source_salesforce-2.5.8/source_salesforce/schemas/Describe.json
--rw-r--r--   0        0        0    15502 2024-04-30 22:49:06.000000 airbyte_source_salesforce-2.5.8/source_salesforce/source.py
--rw-r--r--   0        0        0     4769 2024-04-30 22:49:06.000000 airbyte_source_salesforce-2.5.8/source_salesforce/spec.yaml
--rw-r--r--   0        0        0    41928 2024-04-30 22:49:06.000000 airbyte_source_salesforce-2.5.8/source_salesforce/streams.py
--rw-r--r--   0        0        0     1024 2024-04-30 22:49:06.000000 airbyte_source_salesforce-2.5.8/source_salesforce/utils.py
--rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 airbyte_source_salesforce-2.5.8/PKG-INFO
+-rw-r--r--   0        0        0     4568 2024-05-06 12:33:43.000000 airbyte_source_salesforce-2.5.9/README.md
+-rw-r--r--   0        0        0      830 2024-05-06 14:31:55.963605 airbyte_source_salesforce-2.5.9/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-05-06 12:33:43.000000 airbyte_source_salesforce-2.5.9/source_salesforce/__init__.py
+-rw-r--r--   0        0        0    17451 2024-05-06 12:33:43.000000 airbyte_source_salesforce-2.5.9/source_salesforce/api.py
+-rw-r--r--   0        0        0     1621 2024-05-06 12:33:43.000000 airbyte_source_salesforce-2.5.9/source_salesforce/availability_strategy.py
+-rw-r--r--   0        0        0      808 2024-05-06 12:33:43.000000 airbyte_source_salesforce-2.5.9/source_salesforce/exceptions.py
+-rw-r--r--   0        0        0     3946 2024-05-06 12:33:43.000000 airbyte_source_salesforce-2.5.9/source_salesforce/rate_limiting.py
+-rw-r--r--   0        0        0     1619 2024-05-06 12:33:43.000000 airbyte_source_salesforce-2.5.9/source_salesforce/run.py
+-rw-r--r--   0        0        0    17796 2024-05-06 12:33:43.000000 airbyte_source_salesforce-2.5.9/source_salesforce/schemas/Describe.json
+-rw-r--r--   0        0        0    15502 2024-05-06 12:33:43.000000 airbyte_source_salesforce-2.5.9/source_salesforce/source.py
+-rw-r--r--   0        0        0     4769 2024-05-06 12:33:43.000000 airbyte_source_salesforce-2.5.9/source_salesforce/spec.yaml
+-rw-r--r--   0        0        0    41928 2024-05-06 12:33:43.000000 airbyte_source_salesforce-2.5.9/source_salesforce/streams.py
+-rw-r--r--   0        0        0     1024 2024-05-06 12:33:43.000000 airbyte_source_salesforce-2.5.9/source_salesforce/utils.py
+-rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 airbyte_source_salesforce-2.5.9/PKG-INFO
```

### Comparing `airbyte_source_salesforce-2.5.8/README.md` & `airbyte_source_salesforce-2.5.9/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.8/pyproject.toml` & `airbyte_source_salesforce-2.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.5.8"
+version = "2.5.9"
 name = "airbyte-source-salesforce"
 description = "Source implementation for Salesforce."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_salesforce-2.5.8/source_salesforce/api.py` & `airbyte_source_salesforce-2.5.9/source_salesforce/api.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.8/source_salesforce/availability_strategy.py` & `airbyte_source_salesforce-2.5.9/source_salesforce/availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.8/source_salesforce/exceptions.py` & `airbyte_source_salesforce-2.5.9/source_salesforce/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.8/source_salesforce/rate_limiting.py` & `airbyte_source_salesforce-2.5.9/source_salesforce/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.8/source_salesforce/run.py` & `airbyte_source_salesforce-2.5.9/source_salesforce/run.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.8/source_salesforce/schemas/Describe.json` & `airbyte_source_salesforce-2.5.9/source_salesforce/schemas/Describe.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.8/source_salesforce/source.py` & `airbyte_source_salesforce-2.5.9/source_salesforce/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.8/source_salesforce/spec.yaml` & `airbyte_source_salesforce-2.5.9/source_salesforce/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.8/source_salesforce/streams.py` & `airbyte_source_salesforce-2.5.9/source_salesforce/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.8/source_salesforce/utils.py` & `airbyte_source_salesforce-2.5.9/source_salesforce/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.8/PKG-INFO` & `airbyte_source_salesforce-2.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-salesforce
-Version: 2.5.8
+Version: 2.5.9
 Summary: Source implementation for Salesforce.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

