# Comparing `tmp/llama_index_vector_stores_azureaisearch-0.1.5.tar.gz` & `tmp/llama_index_vector_stores_azureaisearch-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_azureaisearch-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_azureaisearch-0.1.6.tar", max compression
```

## Comparing `llama_index_vector_stores_azureaisearch-0.1.5.tar` & `llama_index_vector_stores_azureaisearch-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       56 2024-05-03 00:43:18.177806 llama_index_vector_stores_azureaisearch-0.1.5/README.md
--rw-r--r--   0        0        0      306 2024-05-03 00:43:18.177806 llama_index_vector_stores_azureaisearch-0.1.5/llama_index/vector_stores/azureaisearch/__init__.py
--rw-r--r--   0        0        0    32218 2024-05-03 00:43:18.177806 llama_index_vector_stores_azureaisearch-0.1.5/llama_index/vector_stores/azureaisearch/base.py
--rw-r--r--   0        0        0     1565 2024-05-03 00:43:18.177806 llama_index_vector_stores_azureaisearch-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 llama_index_vector_stores_azureaisearch-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       56 2024-03-14 20:48:35.041242 llama_index_vector_stores_azureaisearch-0.1.6/README.md
+-rw-r--r--   0        0        0      306 2024-03-14 20:48:35.041818 llama_index_vector_stores_azureaisearch-0.1.6/llama_index/vector_stores/azureaisearch/__init__.py
+-rw-r--r--   0        0        0    32219 2024-05-15 01:33:55.537626 llama_index_vector_stores_azureaisearch-0.1.6/llama_index/vector_stores/azureaisearch/base.py
+-rw-r--r--   0        0        0     1565 2024-05-16 00:15:26.095059 llama_index_vector_stores_azureaisearch-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 llama_index_vector_stores_azureaisearch-0.1.6/PKG-INFO
```

### Comparing `llama_index_vector_stores_azureaisearch-0.1.5/llama_index/vector_stores/azureaisearch/base.py` & `llama_index_vector_stores_azureaisearch-0.1.6/llama_index/vector_stores/azureaisearch/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -593,15 +593,15 @@
                     "provide entry in 'filterable_metadata_field_keys' for this "
                     "vector store"
                 )
 
             index_field = metadata_mapping[0]
 
             if len(odata_filter) > 0:
-                odata_filter.append(" {metadata_filters.condition.value} ")
+                odata_filter.append(f" {metadata_filters.condition.value} ")
             if isinstance(f.value, str):
                 escaped_value = "".join([("''" if s == "'" else s) for s in f.value])
                 odata_filter.append(f"{index_field} eq '{escaped_value}'")
             else:
                 odata_filter.append(f"{index_field} eq {f.value}")
 
         odata_expr = "".join(odata_filter)
```

### Comparing `llama_index_vector_stores_azureaisearch-0.1.5/pyproject.toml` & `llama_index_vector_stores_azureaisearch-0.1.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores azureaisearch integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-azureaisearch"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 azure-search-documents = "^11.4.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_vector_stores_azureaisearch-0.1.5/PKG-INFO` & `llama_index_vector_stores_azureaisearch-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-azureaisearch
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index vector_stores azureaisearch integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

