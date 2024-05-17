# Comparing `tmp/arcee_py-1.0.7.tar.gz` & `tmp/arcee_py-1.0.8.tar.gz`

## Comparing `arcee_py-1.0.7.tar` & `arcee_py-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 arcee_py-1.0.7/.python-version
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 arcee_py-1.0.7/tasks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 arcee_py-1.0.7/.github/CODEOWNERS
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 arcee_py-1.0.7/.github/iced/test.yml
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 arcee_py-1.0.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/__init__.py
--rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/api.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/api_handler.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/cli.py
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/cli_handler.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/config.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/dalm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/schemas/__init__.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/schemas/doc.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/schemas/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.7/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.7/tests/conftest.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 arcee_py-1.0.7/tests/test_api_handler.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 arcee_py-1.0.7/.gitignore
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 arcee_py-1.0.7/README.md
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 arcee_py-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 arcee_py-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 arcee_py-1.0.8/.python-version
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 arcee_py-1.0.8/tasks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 arcee_py-1.0.8/.github/CODEOWNERS
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 arcee_py-1.0.8/.github/iced/test.yml
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 arcee_py-1.0.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/__init__.py
+-rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/api.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/api_handler.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/cli.py
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/cli_handler.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/config.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/dalm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/schemas/__init__.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/schemas/doc.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 arcee_py-1.0.8/arcee/schemas/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.8/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.8/tests/conftest.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 arcee_py-1.0.8/tests/test_api_handler.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 arcee_py-1.0.8/.gitignore
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 arcee_py-1.0.8/README.md
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 arcee_py-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 arcee_py-1.0.8/PKG-INFO
```

### Comparing `arcee_py-1.0.7/tasks.py` & `arcee_py-1.0.8/tasks.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.7/.github/iced/test.yml` & `arcee_py-1.0.8/.github/iced/test.yml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.7/.github/workflows/publish.yml` & `arcee_py-1.0.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.7/arcee/__init__.py` & `arcee_py-1.0.8/arcee/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 
 import os
 
 from arcee import config
 from arcee.api import upload_docs, upload_corpus_folder, upload_qa_pairs, start_alignment, start_pretraining, start_retriever_training, get_retriever_status, start_deployment, stop_deployment, generate, retrieve, delete_corpus, upload_alignment, start_merging
 from arcee.dalm import DALM, DALMFilter
```

### Comparing `arcee_py-1.0.7/arcee/api.py` & `arcee_py-1.0.8/arcee/api.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.7/arcee/api_handler.py` & `arcee_py-1.0.8/arcee/api_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     params: Optional[Dict[str, Any]] = None,
     headers: Optional[Dict[str, Any]] = None,
 ) -> Dict[str, str]:
     """Makes the request"""
     headers = headers or {}
     internal_headers = {"X-Token": f"{config.ARCEE_API_KEY}", "Content-Type": "application/json"}
     headers.update(**internal_headers)
-    url = f"{config.ARCEE_API_URL}/{config.ARCEE_API_VERSION}/{route}"
+    arcee_api_url = config.ARCEE_API_URL.rstrip("/")
+    url = f"{arcee_api_url}/{config.ARCEE_API_VERSION}/{route}"
 
     req_type = getattr(requests, request)
     response = req_type(url, json=body, params=params, headers=headers)
     if response.status_code not in (200, 201, 202):
         raise Exception(f"Failed to make request. Response: {response.text}")
     return response.json()
```

### Comparing `arcee_py-1.0.7/arcee/cli.py` & `arcee_py-1.0.8/arcee/cli.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.7/arcee/cli_handler.py` & `arcee_py-1.0.8/arcee/cli_handler.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.7/arcee/config.py` & `arcee_py-1.0.8/arcee/config.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.7/arcee/dalm.py` & `arcee_py-1.0.8/arcee/dalm.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.7/tests/test_api_handler.py` & `arcee_py-1.0.8/tests/test_api_handler.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.7/.gitignore` & `arcee_py-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.7/README.md` & `arcee_py-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.7/pyproject.toml` & `arcee_py-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.7/PKG-INFO` & `arcee_py-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcee-py
-Version: 1.0.7
+Version: 1.0.8
 Project-URL: Home, https://arcee.ai
 Author-email: Jacob Solowetz <jacob@arcee.ai>, Ben Epstein <ben@arcee.ai>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: pydantic<3.0,>=2.4.2
 Requires-Dist: requests
 Requires-Dist: rich
```

