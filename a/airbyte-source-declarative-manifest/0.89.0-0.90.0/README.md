# Comparing `tmp/airbyte_source_declarative_manifest-0.89.0.tar.gz` & `tmp/airbyte_source_declarative_manifest-0.90.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_declarative_manifest-0.89.0.tar", max compression
+gzip compressed data, was "airbyte_source_declarative_manifest-0.90.0.tar", max compression
```

## Comparing `airbyte_source_declarative_manifest-0.89.0.tar` & `airbyte_source_declarative_manifest-0.90.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     4003 2024-05-15 01:09:38.483284 airbyte_source_declarative_manifest-0.89.0/README.md
--rw-r--r--   0        0        0      817 2024-05-15 01:13:35.618736 airbyte_source_declarative_manifest-0.89.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-15 01:09:38.483284 airbyte_source_declarative_manifest-0.89.0/source_declarative_manifest/__init__.py
--rw-r--r--   0        0        0     2180 2024-05-15 01:09:38.483284 airbyte_source_declarative_manifest-0.89.0/source_declarative_manifest/run.py
--rw-r--r--   0        0        0      554 2024-05-15 01:09:38.483284 airbyte_source_declarative_manifest-0.89.0/source_declarative_manifest/spec.json
--rw-r--r--   0        0        0     4739 1970-01-01 00:00:00.000000 airbyte_source_declarative_manifest-0.89.0/PKG-INFO
+-rw-r--r--   0        0        0     4003 2024-05-17 05:34:07.138979 airbyte_source_declarative_manifest-0.90.0/README.md
+-rw-r--r--   0        0        0      817 2024-05-17 05:38:33.492709 airbyte_source_declarative_manifest-0.90.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 05:34:07.138979 airbyte_source_declarative_manifest-0.90.0/source_declarative_manifest/__init__.py
+-rw-r--r--   0        0        0     2180 2024-05-17 05:34:07.138979 airbyte_source_declarative_manifest-0.90.0/source_declarative_manifest/run.py
+-rw-r--r--   0        0        0      554 2024-05-17 05:34:07.138979 airbyte_source_declarative_manifest-0.90.0/source_declarative_manifest/spec.json
+-rw-r--r--   0        0        0     4739 1970-01-01 00:00:00.000000 airbyte_source_declarative_manifest-0.90.0/PKG-INFO
```

### Comparing `airbyte_source_declarative_manifest-0.89.0/README.md` & `airbyte_source_declarative_manifest-0.90.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_declarative_manifest-0.89.0/pyproject.toml` & `airbyte_source_declarative_manifest-0.90.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.89.0"
+version = "0.90.0"
 name = "airbyte-source-declarative-manifest"
 description = "Base source implementation for low-code sources."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_declarative_manifest" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "0.89.0"
+airbyte-cdk = "0.90.0"
 
 [tool.poetry.scripts]
 source-declarative-manifest = "source_declarative_manifest.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest-mock = "^3.6.1"
 pytest = "^6.2"
```

### Comparing `airbyte_source_declarative_manifest-0.89.0/source_declarative_manifest/run.py` & `airbyte_source_declarative_manifest-0.90.0/source_declarative_manifest/run.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_declarative_manifest-0.89.0/source_declarative_manifest/spec.json` & `airbyte_source_declarative_manifest-0.90.0/source_declarative_manifest/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_declarative_manifest-0.89.0/PKG-INFO` & `airbyte_source_declarative_manifest-0.90.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-declarative-manifest
-Version: 0.89.0
+Version: 0.90.0
 Summary: Base source implementation for low-code sources.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (==0.89.0)
+Requires-Dist: airbyte-cdk (==0.90.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/low-code
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Declarative-Manifest source connector
 
 This is the repository for the Declarative-Manifest source connector, written in Python.
```

