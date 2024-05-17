# Comparing `tmp/memvectordb_python-0.0.1.tar.gz` & `tmp/memvectordb_python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memvectordb_python-0.0.1.tar", max compression
+gzip compressed data, was "memvectordb_python-0.0.2.tar", max compression
```

## Comparing `memvectordb_python-0.0.1.tar` & `memvectordb_python-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2160 2024-05-15 14:01:24.743457 memvectordb_python-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-15 14:01:24.743457 memvectordb_python-0.0.1/memvectordb/__init__.py
--rw-r--r--   0        0        0     6575 2024-05-15 14:01:24.743457 memvectordb_python-0.0.1/memvectordb/collection.py
--rw-r--r--   0        0        0      444 2024-05-15 14:01:24.743457 memvectordb_python-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3194 1970-01-01 00:00:00.000000 memvectordb_python-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2164 2024-05-17 13:49:55.624854 memvectordb_python-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 13:49:55.624854 memvectordb_python-0.0.2/memvectordb/__init__.py
+-rw-r--r--   0        0        0     7325 2024-05-17 13:49:55.624854 memvectordb_python-0.0.2/memvectordb/collection.py
+-rw-r--r--   0        0        0      445 2024-05-17 13:49:55.624854 memvectordb_python-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3198 1970-01-01 00:00:00.000000 memvectordb_python-0.0.2/PKG-INFO
```

### Comparing `memvectordb_python-0.0.1/PKG-INFO` & `memvectordb_python-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: memvectordb-python
-Version: 0.0.1
-Summary: memvectordb python client.
-Home-page: https://github.com/KevKibe/memvectordb-python-client
-License: MIT
-Author: Kevin Kibe
-Author-email: keviinkibe@gmail.com
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: requests (==2.31.0)
-Project-URL: Repository, https://github.com/KevKibe/memvectordb-python-client
-Description-Content-Type: text/markdown
-
 # memvectorDB-python client
 
 ## Getting Started
 
 ```bash
 pip install memvectordb-python
 ```
@@ -63,59 +38,67 @@
 collection_name = "collection_name"
 collection = client.delete_collection(collection_name)
 ```
 ### To Insert Vectors(streaming)
 ```python
 
 collection_name = "collection_name"
-embedding = "embedding"
-
-# example of embedding : {
-#                          "id" : "1",
-#                          "vector" :[0.14, 0.316, 0.433], 
-#                          "metadata": {
-#                             "key1": "value1",
-#                             "key2": "value2"
-#                         }
-#                     }
-client.insert_embeddings(collection_name, embedding)
+embedding = {
+    "id": "1",
+    "vector": [0.14, 0.316, 0.433],
+    "metadata": {
+        "key1": "value1",
+        "key2": "value2"
+    }
+}
+
+client.insert_embeddings(
+    collection_name=collection_name, 
+    vector_id=embedding["id"], 
+    vector=embedding["vector"], 
+    metadata=embedding["metadata"]
+)
 ```
 
 ### To Insert Vectors(batch)
 
 ```python
 
 collection_name = "collection_name"
-embeddings = "embeddings"
-
-# example of embeddings : [
-#         {
-#             "id": "1",
-#             "vector": [0.14, 0.316, 0.433],
-#             "metadata": {
-#                 "key1": "value1",
-#                 "key2": "value2"
-#             }
-#         },
-#         {
-#             "id": "2",
-#             "vector": [0.27, 0.531, 0.621],
-#             "metadata": {
-#                 "key1": "value3",
-#                 "key2": "value4"
-#             }
-#         }
-#     ]
-client.update_embeddings(collection_name, embeddings)
+embeddings = [
+    {
+        "id": "1",
+        "vector": [0.14, 0.316, 0.433],
+        "metadata": {
+            "key1": "value1",
+            "key2": "value2"
+        }
+    },
+    {
+        "id": "2",
+        "vector": [0.27, 0.531, 0.621],
+        "metadata": {
+            "key1": "value3",
+            "key2": "value4"
+        }
+    }
+]
+
+for embedding in embeddings:
+    client.batch_insert_embeddings(
+        collection_name=collection_name, 
+        vector_id=embedding["id"], 
+        vector=embedding["vector"], 
+        metadata=embedding["metadata"]
+    )
 ```
 ## To Query Vectors.
 
 ```python
 k = "number-of-items-to query"
 collection_name = "collection_name"
 query_vector = "query_vector"
 
 # example of query_vector: [0.32654, 0.24423, 0.7655] 
-
-client.get_similarity(k, collection_name, query_vector)
+# ensure the dimensions match the collection's dimensions
+client.get_similarity(collection_name, k, query_vector)
 ```
-
```

