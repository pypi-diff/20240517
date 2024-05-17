# Comparing `tmp/dartmouth_langchain-0.0.5.tar.gz` & `tmp/dartmouth_langchain-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dartmouth_langchain-0.0.5.tar", last modified: Wed May 15 15:52:20 2024, max compression
+gzip compressed data, was "dartmouth_langchain-0.0.6.tar", last modified: Fri May 17 12:49:40 2024, max compression
```

## Comparing `dartmouth_langchain-0.0.5.tar` & `dartmouth_langchain-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 15:52:20.636065 dartmouth_langchain-0.0.5/
--rw-r--r--   0 f006pfk    (502) staff       (20)     1068 2024-03-12 21:00:11.000000 dartmouth_langchain-0.0.5/LICENSE
--rw-r--r--   0 f006pfk    (502) staff       (20)     1816 2024-05-15 15:52:20.635806 dartmouth_langchain-0.0.5/PKG-INFO
--rw-r--r--   0 f006pfk    (502) staff       (20)     1070 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.5/README.md
--rw-r--r--   0 f006pfk    (502) staff       (20)      713 2024-05-15 15:52:00.000000 dartmouth_langchain-0.0.5/pyproject.toml
--rw-r--r--   0 f006pfk    (502) staff       (20)       38 2024-05-15 15:52:20.636114 dartmouth_langchain-0.0.5/setup.cfg
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 15:52:20.630692 dartmouth_langchain-0.0.5/src/
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 15:52:20.632617 dartmouth_langchain-0.0.5/src/dartmouth_langchain/
--rw-r--r--   0 f006pfk    (502) staff       (20)        0 2024-03-12 20:49:51.000000 dartmouth_langchain-0.0.5/src/dartmouth_langchain/__init__.py
--rw-r--r--   0 f006pfk    (502) staff       (20)      805 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.5/src/dartmouth_langchain/base.py
--rw-r--r--   0 f006pfk    (502) staff       (20)      836 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.5/src/dartmouth_langchain/cross_encoders.py
--rw-r--r--   0 f006pfk    (502) staff       (20)      163 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.5/src/dartmouth_langchain/definitions.py
--rw-r--r--   0 f006pfk    (502) staff       (20)     1776 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.5/src/dartmouth_langchain/embeddings.py
--rw-r--r--   0 f006pfk    (502) staff       (20)     2817 2024-05-15 14:23:04.000000 dartmouth_langchain-0.0.5/src/dartmouth_langchain/llms.py
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 15:52:20.634615 dartmouth_langchain-0.0.5/src/dartmouth_langchain/retrievers/
--rw-r--r--   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.5/src/dartmouth_langchain/retrievers/__init__.py
--rw-r--r--   0 f006pfk    (502) staff       (20)     3421 2024-05-15 15:51:49.000000 dartmouth_langchain-0.0.5/src/dartmouth_langchain/retrievers/document_compressors.py
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 15:52:20.635437 dartmouth_langchain-0.0.5/src/dartmouth_langchain.egg-info/
--rw-r--r--   0 f006pfk    (502) staff       (20)     1816 2024-05-15 15:52:20.000000 dartmouth_langchain-0.0.5/src/dartmouth_langchain.egg-info/PKG-INFO
--rw-r--r--   0 f006pfk    (502) staff       (20)      606 2024-05-15 15:52:20.000000 dartmouth_langchain-0.0.5/src/dartmouth_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 f006pfk    (502) staff       (20)        1 2024-05-15 15:52:20.000000 dartmouth_langchain-0.0.5/src/dartmouth_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 f006pfk    (502) staff       (20)       61 2024-05-15 15:52:20.000000 dartmouth_langchain-0.0.5/src/dartmouth_langchain.egg-info/requires.txt
--rw-r--r--   0 f006pfk    (502) staff       (20)       20 2024-05-15 15:52:20.000000 dartmouth_langchain-0.0.5/src/dartmouth_langchain.egg-info/top_level.txt
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 15:52:20.634791 dartmouth_langchain-0.0.5/tests/
--rw-r--r--   0 f006pfk    (502) staff       (20)     2654 2024-05-15 15:51:49.000000 dartmouth_langchain-0.0.5/tests/tests.py
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-17 12:49:40.285373 dartmouth_langchain-0.0.6/
+-rw-r--r--   0 f006pfk    (502) staff       (20)     1068 2024-03-12 21:00:11.000000 dartmouth_langchain-0.0.6/LICENSE
+-rw-r--r--   0 f006pfk    (502) staff       (20)     1816 2024-05-17 12:49:40.285099 dartmouth_langchain-0.0.6/PKG-INFO
+-rw-r--r--   0 f006pfk    (502) staff       (20)     1070 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.6/README.md
+-rw-r--r--   0 f006pfk    (502) staff       (20)      713 2024-05-17 12:49:10.000000 dartmouth_langchain-0.0.6/pyproject.toml
+-rw-r--r--   0 f006pfk    (502) staff       (20)       38 2024-05-17 12:49:40.285430 dartmouth_langchain-0.0.6/setup.cfg
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-17 12:49:40.280308 dartmouth_langchain-0.0.6/src/
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-17 12:49:40.282306 dartmouth_langchain-0.0.6/src/dartmouth_langchain/
+-rw-r--r--   0 f006pfk    (502) staff       (20)        0 2024-03-12 20:49:51.000000 dartmouth_langchain-0.0.6/src/dartmouth_langchain/__init__.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)      805 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.6/src/dartmouth_langchain/base.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)      836 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.6/src/dartmouth_langchain/cross_encoders.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)      163 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.6/src/dartmouth_langchain/definitions.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)     1776 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.6/src/dartmouth_langchain/embeddings.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)     2817 2024-05-15 14:23:04.000000 dartmouth_langchain-0.0.6/src/dartmouth_langchain/llms.py
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-17 12:49:40.284122 dartmouth_langchain-0.0.6/src/dartmouth_langchain/retrievers/
+-rw-r--r--   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.6/src/dartmouth_langchain/retrievers/__init__.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)     3422 2024-05-16 19:36:27.000000 dartmouth_langchain-0.0.6/src/dartmouth_langchain/retrievers/document_compressors.py
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-17 12:49:40.284690 dartmouth_langchain-0.0.6/src/dartmouth_langchain.egg-info/
+-rw-r--r--   0 f006pfk    (502) staff       (20)     1816 2024-05-17 12:49:40.000000 dartmouth_langchain-0.0.6/src/dartmouth_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 f006pfk    (502) staff       (20)      606 2024-05-17 12:49:40.000000 dartmouth_langchain-0.0.6/src/dartmouth_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 f006pfk    (502) staff       (20)        1 2024-05-17 12:49:40.000000 dartmouth_langchain-0.0.6/src/dartmouth_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 f006pfk    (502) staff       (20)       61 2024-05-17 12:49:40.000000 dartmouth_langchain-0.0.6/src/dartmouth_langchain.egg-info/requires.txt
+-rw-r--r--   0 f006pfk    (502) staff       (20)       20 2024-05-17 12:49:40.000000 dartmouth_langchain-0.0.6/src/dartmouth_langchain.egg-info/top_level.txt
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-17 12:49:40.284300 dartmouth_langchain-0.0.6/tests/
+-rw-r--r--   0 f006pfk    (502) staff       (20)     2651 2024-05-17 12:49:02.000000 dartmouth_langchain-0.0.6/tests/tests.py
```

### Comparing `dartmouth_langchain-0.0.5/LICENSE` & `dartmouth_langchain-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dartmouth_langchain-0.0.5/PKG-INFO` & `dartmouth_langchain-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartmouth_langchain
-Version: 0.0.5
+Version: 0.0.6
 Summary: LangChain components for Dartmouth-hosted models.
 Author-email: Simon Stone <simon.stone@dartmouth.edu>
 Project-URL: Homepage, https://git.dartmouth.edu/lib-digital-strategies/RDS/projects/dartmouth-langchain
 Project-URL: Issues, https://git.dartmouth.edu/lib-digital-strategies/RDS/projects/dartmouth-langchain/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dartmouth_langchain-0.0.5/README.md` & `dartmouth_langchain-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dartmouth_langchain-0.0.5/pyproject.toml` & `dartmouth_langchain-0.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dartmouth_langchain"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Simon Stone", email="simon.stone@dartmouth.edu" },
 ]
 description = "LangChain components for Dartmouth-hosted models."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dartmouth_langchain-0.0.5/src/dartmouth_langchain/base.py` & `dartmouth_langchain-0.0.6/src/dartmouth_langchain/base.py`

 * *Files identical despite different names*

### Comparing `dartmouth_langchain-0.0.5/src/dartmouth_langchain/cross_encoders.py` & `dartmouth_langchain-0.0.6/src/dartmouth_langchain/cross_encoders.py`

 * *Files identical despite different names*

### Comparing `dartmouth_langchain-0.0.5/src/dartmouth_langchain/embeddings.py` & `dartmouth_langchain-0.0.6/src/dartmouth_langchain/embeddings.py`

 * *Files identical despite different names*

### Comparing `dartmouth_langchain-0.0.5/src/dartmouth_langchain/llms.py` & `dartmouth_langchain-0.0.6/src/dartmouth_langchain/llms.py`

 * *Files identical despite different names*

### Comparing `dartmouth_langchain-0.0.5/src/dartmouth_langchain/retrievers/document_compressors.py` & `dartmouth_langchain-0.0.6/src/dartmouth_langchain/retrievers/document_compressors.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,26 +58,26 @@
     jwt_url: str = None
     """URL of the Dartmouth API endpoint returning a JSON Web Token (JWT)"""
 
     def __init__(
         self,
         *args,
         dartmouth_api_key: str = None,
-        model_name: str = "bge-reranker-large",
+        model_name: str = "bge-reranker-v2-m3",
         authenticator: Callable = None,
         jwt_url: str = None,
         **kwargs,
     ):
         """
         Initializes the object
 
         Args:
             dartmouth_api_key (str, optional): A valid Dartmouth API key (see https://developer.dartmouth.edu/keys).
                 If not specified, it is attempted to be inferred from an environment variable DARTMOUTH_API_KEY.
-            model_name (str, optional): Name of the model to use. Defaults to "bge-large-en-v1-5".
+            model_name (str, optional): Name of the model to use. Defaults to "bge-reranker-v2-m3".
             authenticator (Callable, optional): A Callable that returns a valid JWT to use for authentication.
                 If specified, `dartmouth_api_key` is ignored.
         """
         endpoint = f"{RERANK_BASE_URL}{model_name}/"
         if "client" not in kwargs:
             kwargs["client"] = TextEmbeddingInferenceClient(
                 inference_server_url=endpoint
```

### Comparing `dartmouth_langchain-0.0.5/src/dartmouth_langchain.egg-info/PKG-INFO` & `dartmouth_langchain-0.0.6/src/dartmouth_langchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartmouth_langchain
-Version: 0.0.5
+Version: 0.0.6
 Summary: LangChain components for Dartmouth-hosted models.
 Author-email: Simon Stone <simon.stone@dartmouth.edu>
 Project-URL: Homepage, https://git.dartmouth.edu/lib-digital-strategies/RDS/projects/dartmouth-langchain
 Project-URL: Issues, https://git.dartmouth.edu/lib-digital-strategies/RDS/projects/dartmouth-langchain/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dartmouth_langchain-0.0.5/src/dartmouth_langchain.egg-info/SOURCES.txt` & `dartmouth_langchain-0.0.6/src/dartmouth_langchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dartmouth_langchain-0.0.5/tests/tests.py` & `dartmouth_langchain-0.0.6/tests/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,16 +67,17 @@
     query = "What is Deep Learning?"
     texts = [
         "Deep Learning is not...",
         "Deep learning is...",
     ]
     tei_client = TextEmbeddingInferenceClient()
     scores = tei_client.rerank(query=query, texts=texts)
+
     assert scores
 
 
 if __name__ == "__main__":
     test_dartmouth_chat()
     test_dartmouth_embeddings()
-    # test_tei_client()
-    # test_tei_reranker()
+    test_tei_client()
+    test_tei_reranker()
     test_dartmouth_reranker()
```

