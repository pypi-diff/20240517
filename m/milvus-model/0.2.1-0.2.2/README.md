# Comparing `tmp/milvus_model-0.2.1.tar.gz` & `tmp/milvus_model-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milvus_model-0.2.1.tar", last modified: Sat May 11 12:10:10 2024, max compression
+gzip compressed data, was "milvus_model-0.2.2.tar", last modified: Fri May 17 12:35:16 2024, max compression
```

## Comparing `milvus_model-0.2.1.tar` & `milvus_model-0.2.2.tar`

### file list

```diff
@@ -1,45 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.480344 milvus_model-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.472344 milvus_model-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.472344 milvus_model-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-11 12:10:04.000000 milvus_model-0.2.1/.github/workflows/publish_dev_package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-11 12:10:04.000000 milvus_model-0.2.1/.github/workflows/publish_on_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-11 12:10:04.000000 milvus_model-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-11 12:10:04.000000 milvus_model-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-11 12:10:10.480344 milvus_model-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-11 12:10:04.000000 milvus_model-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-11 12:10:04.000000 milvus_model-0.2.1/_version_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.472344 milvus_model-0.2.1/milvus_model/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.476344 milvus_model-0.2.1/milvus_model/dense/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/dense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/dense/jinaai.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/dense/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/dense/sentence_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/dense/voyageai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.476344 milvus_model-0.2.1/milvus_model/hybrid/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/hybrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/hybrid/bge_m3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.476344 milvus_model-0.2.1/milvus_model/reranker/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/reranker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/reranker/bgereranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/reranker/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/reranker/cross_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/reranker/jinaai.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/reranker/voyageai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.476344 milvus_model-0.2.1/milvus_model/sparse/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/sparse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.476344 milvus_model-0.2.1/milvus_model/sparse/bm25/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/sparse/bm25/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/sparse/bm25/bm25.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/sparse/bm25/lang.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/sparse/bm25/tokenizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/sparse/splade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.480344 milvus_model-0.2.1/milvus_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-11 12:10:10.000000 milvus_model-0.2.1/milvus_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-11 12:10:10.000000 milvus_model-0.2.1/milvus_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:10:10.000000 milvus_model-0.2.1/milvus_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-11 12:10:10.000000 milvus_model-0.2.1/milvus_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 12:10:10.000000 milvus_model-0.2.1/milvus_model.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-11 12:10:04.000000 milvus_model-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:10:10.480344 milvus_model-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.246464 milvus_model-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.238464 milvus_model-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.238464 milvus_model-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 12:35:09.000000 milvus_model-0.2.2/.github/workflows/publish_dev_package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-17 12:35:09.000000 milvus_model-0.2.2/.github/workflows/publish_on_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-17 12:35:09.000000 milvus_model-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 12:35:09.000000 milvus_model-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-17 12:35:16.246464 milvus_model-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-17 12:35:09.000000 milvus_model-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-17 12:35:09.000000 milvus_model-0.2.2/_version_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.238464 milvus_model-0.2.2/milvus_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.242464 milvus_model-0.2.2/milvus_model/dense/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/dense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/dense/jinaai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/dense/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/dense/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/dense/sentence_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/dense/voyageai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.242464 milvus_model-0.2.2/milvus_model/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/hybrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/hybrid/bge_m3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.242464 milvus_model-0.2.2/milvus_model/reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/reranker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/reranker/bgereranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/reranker/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/reranker/cross_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/reranker/jinaai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/reranker/voyageai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.242464 milvus_model-0.2.2/milvus_model/sparse/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/sparse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.242464 milvus_model-0.2.2/milvus_model/sparse/bm25/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/sparse/bm25/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/sparse/bm25/bm25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/sparse/bm25/lang.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/sparse/bm25/tokenizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/sparse/splade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.242464 milvus_model-0.2.2/milvus_model/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/utils/dependency_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-17 12:35:09.000000 milvus_model-0.2.2/milvus_model/utils/lazy_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:35:16.242464 milvus_model-0.2.2/milvus_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-17 12:35:16.000000 milvus_model-0.2.2/milvus_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-17 12:35:16.000000 milvus_model-0.2.2/milvus_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:35:16.000000 milvus_model-0.2.2/milvus_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-17 12:35:16.000000 milvus_model-0.2.2/milvus_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 12:35:16.000000 milvus_model-0.2.2/milvus_model.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-17 12:35:09.000000 milvus_model-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 12:35:16.246464 milvus_model-0.2.2/setup.cfg
```

### Comparing `milvus_model-0.2.1/.github/workflows/publish_dev_package.yml` & `milvus_model-0.2.2/.github/workflows/publish_dev_package.yml`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.1/.github/workflows/publish_on_release.yml` & `milvus_model-0.2.2/.github/workflows/publish_on_release.yml`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.1/LICENSE` & `milvus_model-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.1/PKG-INFO` & `milvus_model-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 Metadata-Version: 2.1
 Name: milvus-model
-Version: 0.2.1
+Version: 0.2.2
 Summary: Model components for PyMilvus, the Python SDK for Milvus
 Author-email: Milvus Team <milvus-team@zilliz.com>
 Project-URL: repository, https://github.com/milvus-io/milvus-model
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai>=1.12.0
-Requires-Dist: sentence-transformers
-Requires-Dist: FlagEmbedding>=1.2.2
-Requires-Dist: nltk
 Requires-Dist: transformers>=4.36.0
-Requires-Dist: jieba
-Requires-Dist: konlpy
-Requires-Dist: mecab-python3
+Requires-Dist: onnxruntime
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: protobuf==3.20.2
-Requires-Dist: unidic-lite
-Requires-Dist: cohere
-Requires-Dist: voyageai>=0.2.0
+Requires-Dist: numpy
 
 # Milvus Model Lib
 
 The milvus-model library provides model components for PyMilvus, the official Python SDK for Milvus, an open-source vector database built for AI applications.
 
 ## Installation
```

### Comparing `milvus_model-0.2.1/README.md` & `milvus_model-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.1/_version_helper.py` & `milvus_model-0.2.2/_version_helper.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.1/milvus_model/base.py` & `milvus_model-0.2.2/milvus_model/base.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.1/milvus_model/dense/jinaai.py` & `milvus_model-0.2.2/milvus_model/dense/jinaai.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.1/milvus_model/dense/openai.py` & `milvus_model-0.2.2/milvus_model/dense/openai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 from collections import defaultdict
 from typing import List, Optional
 
 import numpy as np
 
 from milvus_model.base import BaseEmbeddingFunction
+from milvus_model.utils import import_openai
 
+import_openai()
+from openai import OpenAI
 
 class OpenAIEmbeddingFunction(BaseEmbeddingFunction):
     def __init__(
         self,
         model_name: str = "text-embedding-ada-002",
         api_key: Optional[str] = None,
         base_url: Optional[str] = None,
         dimensions: Optional[int] = None,
         **kwargs,
     ):
-        try:
-            from openai import OpenAI
-        except ImportError as err:
-            error_message = "openai is not installed."
-            raise ImportError(error_message) from err
-
         self._openai_model_meta_info = defaultdict(dict)
         self._openai_model_meta_info["text-embedding-3-small"]["dim"] = 1536
         self._openai_model_meta_info["text-embedding-3-large"]["dim"] = 3072
         self._openai_model_meta_info["text-embedding-ada-002"]["dim"] = 1536
 
         self._model_config = dict({"api_key": api_key, "base_url": base_url}, **kwargs)
         additional_encode_config = {}
```

### Comparing `milvus_model-0.2.1/milvus_model/dense/sentence_transformer.py` & `milvus_model-0.2.2/milvus_model/dense/sentence_transformer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from typing import List
 
 import numpy as np
 
 from milvus_model.base import BaseEmbeddingFunction
+from milvus_model.utils import import_sentence_transformers
 
+import_sentence_transformers()
+from sentence_transformers import SentenceTransformer
 
 class SentenceTransformerEmbeddingFunction(BaseEmbeddingFunction):
     def __init__(
         self,
         model_name: str = "all-MiniLM-L6-v2",
         batch_size: int = 32,
         query_instruction: str = "",
         doc_instruction: str = "",
         device: str = "cpu",
         normalize_embeddings: bool = True,
         **kwargs,
     ):
-        try:
-            from sentence_transformers import SentenceTransformer
-        except ImportError as err:
-            error_message = "sentence-transformers is not installed."
-            raise ImportError(error_message) from err
         self.model_name = model_name
         self.query_instruction = query_instruction
         self.doc_instruction = doc_instruction
         self.batch_size = batch_size
         self.normalize_embeddings = normalize_embeddings
 
         _model_config = dict({"model_name_or_path": model_name, "device": device}, **kwargs)
```

### Comparing `milvus_model-0.2.1/milvus_model/dense/voyageai.py` & `milvus_model-0.2.2/milvus_model/dense/voyageai.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from collections import defaultdict
 from typing import List, Optional
 
 import numpy as np
 
 from milvus_model.base import BaseEmbeddingFunction
+from milvus_model.utils import import_voyageai
 
+import_voyageai()
+import voyageai
 
 class VoyageEmbeddingFunction(BaseEmbeddingFunction):
     def __init__(self, model_name: str = "voyage-2", api_key: Optional[str] = None, **kwargs):
-        try:
-            import voyageai
-        except ImportError as err:
-            error_message = "voyageai is not installed."
-            raise ImportError(error_message) from err
         self.model_name = model_name
         self._voyageai_model_meta_info = defaultdict(dict)
         self._voyageai_model_meta_info["voyage-large-2"]["dim"] = 1536
         self._voyageai_model_meta_info["voyage-code-2"]["dim"] = 1536
         self._voyageai_model_meta_info["voyage-2"]["dim"] = 1024
         self._voyageai_model_meta_info["voyage-lite-02-instruct"]["dim"] = 1024
         self.client = voyageai.Client(api_key, **kwargs)
```

### Comparing `milvus_model-0.2.1/milvus_model/hybrid/bge_m3.py` & `milvus_model-0.2.2/milvus_model/hybrid/bge_m3.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import logging
 from typing import Dict, List
 
 from scipy.sparse import csr_array, vstack
 
 from milvus_model.base import BaseEmbeddingFunction
+from milvus_model.utils import import_FlagEmbedding
+
+import_FlagEmbedding()
+from FlagEmbedding import BGEM3FlagModel
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 class BGEM3EmbeddingFunction(BaseEmbeddingFunction):
     def __init__(
@@ -18,19 +22,14 @@
         normalize_embeddings: bool = True,
         use_fp16: bool = False,
         return_dense: bool = True,
         return_sparse: bool = True,
         return_colbert_vecs: bool = False,
         **kwargs,
     ):
-        try:
-            from FlagEmbedding import BGEM3FlagModel
-        except ImportError as err:
-            error_message = "FlagEmbedding is not installed."
-            raise ImportError(error_message) from err
         self.model_name = model_name
         self.batch_size = batch_size
         self.normalize_embeddings = normalize_embeddings
         self.device = device
         self.use_fp16 = use_fp16
 
         if device == "cpu" and use_fp16 is True:
```

### Comparing `milvus_model-0.2.1/milvus_model/reranker/bgereranker.py` & `milvus_model-0.2.2/milvus_model/reranker/bgereranker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,32 @@
 from typing import List, Optional, Union
 
 import torch
 
 from milvus_model.base import BaseRerankFunction, RerankResult
+from milvus_model.utils import import_FlagEmbedding, import_transformers
 
-try:
-    from FlagEmbedding import FlagReranker
-    from transformers import (
-        AutoModelForSequenceClassification,
-        AutoTokenizer,
-        is_torch_npu_available,
-    )
-
-    _DEPENDENCIES_AVAILABLE = True
-except ImportError as e:
-    _DEPENDENCY_ERROR_MESSAGE = str(e)
-    _DEPENDENCIES_AVAILABLE = False
-
-    class FlagReranker:
-        def __init__(self, *args, **kwargs):
-            error_message = str(_DEPENDENCY_ERROR_MESSAGE)
-            raise NotImplementedError(error_message)
-
+import_FlagEmbedding()
+import_transformers()
+from FlagEmbedding import FlagReranker
+from transformers import (
+    AutoModelForSequenceClassification,
+    AutoTokenizer,
+    is_torch_npu_available,
+)
 
 class BGERerankFunction(BaseRerankFunction):
     def __init__(
         self,
         model_name: str = "BAAI/bge-reranker-v2-m3",
         use_fp16: bool = True,
         batch_size: int = 32,
         normalize: bool = True,
         device: Optional[str] = None,
     ):
-        if _DEPENDENCIES_AVAILABLE is False:
-            raise ImportError(_DEPENDENCY_ERROR_MESSAGE)
 
         self.model_name = model_name
         self.batch_size = batch_size
         self.normalize = normalize
         self.device = device
         self.reranker = _FlagReranker(model_name, use_fp16=use_fp16, device=device)
```

### Comparing `milvus_model-0.2.1/milvus_model/reranker/cohere.py` & `milvus_model-0.2.2/milvus_model/reranker/voyageai.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 from typing import List, Optional
 
 from milvus_model.base import BaseRerankFunction, RerankResult
+from milvus_model.utils import import_voyageai
 
-try:
-    import cohere
-except ImportError:
-    cohere = None
+import_voyageai()
+import voyageai
 
-
-class CohereRerankFunction(BaseRerankFunction):
-    def __init__(self, model_name: str = "rerank-english-v2.0", api_key: Optional[str] = None):
-        if cohere is None:
-            error_message = "cohere is not installed."
-            raise ImportError(error_message)
+class VoyageRerankFunction(BaseRerankFunction):
+    def __init__(self, model_name: str = "rerank-lite-1", api_key: Optional[str] = None):
         self.model_name = model_name
-        self.client = cohere.Client(api_key)
+        self.client = voyageai.Client(api_key=api_key)
 
     def __call__(self, query: str, documents: List[str], top_k: int = 5) -> List[RerankResult]:
-        co_results = self.client.rerank(
-            query=query, documents=documents, top_n=top_k, model="rerank-english-v2.0"
-        )
+        vo_results = self.client.rerank(query, documents, model=self.model_name, top_k=top_k)
         results = []
-        for co_result in co_results.results:
+        for vo_result in vo_results.results:
             results.append(
                 RerankResult(
-                    text=co_result.document["text"],
-                    score=co_result.relevance_score,
-                    index=co_result.index,
+                    text=vo_result.document, score=vo_result.relevance_score, index=vo_result.index
                 )
             )
         return results
```

### Comparing `milvus_model-0.2.1/milvus_model/reranker/cross_encoder.py` & `milvus_model-0.2.2/milvus_model/reranker/cross_encoder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from typing import Any, List
 
 from milvus_model.base import BaseRerankFunction, RerankResult
+from milvus_model.utils import import_sentence_transformers
 
-try:
-    import sentence_transformers
-except ImportError:
-    sentence_transformers = None
-
+import_sentence_transformers()
+import sentence_transformers
 
 class CrossEncoderRerankFunction(BaseRerankFunction):
     def __init__(
         self,
         model_name: str = "",
         device: str = "",
         batch_size: int = 32,
```

### Comparing `milvus_model-0.2.1/milvus_model/reranker/jinaai.py` & `milvus_model-0.2.2/milvus_model/reranker/jinaai.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.1/milvus_model/reranker/voyageai.py` & `milvus_model-0.2.2/milvus_model/reranker/cohere.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from typing import List, Optional
 
 from milvus_model.base import BaseRerankFunction, RerankResult
+from milvus_model.utils import import_cohere
 
-try:
-    import voyageai
-except ImportError:
-    voyageai = None
+import_cohere()
+import cohere
 
-
-class VoyageRerankFunction(BaseRerankFunction):
-    def __init__(self, model_name: str = "rerank-lite-1", api_key: Optional[str] = None):
-        if voyageai is None:
-            error_message = "voyageai is not installed."
-            raise ImportError(error_message)
+class CohereRerankFunction(BaseRerankFunction):
+    def __init__(self, model_name: str = "rerank-english-v2.0", api_key: Optional[str] = None):
         self.model_name = model_name
-        self.client = voyageai.Client(api_key=api_key)
+        self.client = cohere.Client(api_key)
 
     def __call__(self, query: str, documents: List[str], top_k: int = 5) -> List[RerankResult]:
-        vo_results = self.client.rerank(query, documents, model=self.model_name, top_k=top_k)
+        co_results = self.client.rerank(
+            query=query, documents=documents, top_n=top_k, model="rerank-english-v2.0"
+        )
         results = []
-        for vo_result in vo_results.results:
+        for co_result in co_results.results:
             results.append(
                 RerankResult(
-                    text=vo_result.document, score=vo_result.relevance_score, index=vo_result.index
+                    text=co_result.document["text"],
+                    score=co_result.relevance_score,
+                    index=co_result.index,
                 )
             )
         return results
```

### Comparing `milvus_model-0.2.1/milvus_model/sparse/bm25/bm25.py` & `milvus_model-0.2.2/milvus_model/sparse/bm25/bm25.py`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.1/milvus_model/sparse/bm25/lang.yaml` & `milvus_model-0.2.2/milvus_model/sparse/bm25/lang.yaml`

 * *Files identical despite different names*

### Comparing `milvus_model-0.2.1/milvus_model/sparse/bm25/tokenizers.py` & `milvus_model-0.2.2/milvus_model/sparse/bm25/tokenizers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 import re
 import string
 from importlib.util import find_spec
 from pathlib import Path
 from typing import Any, Dict, List, Match, Optional, Type
+from milvus_model.utils import import_nltk, import_jieba, import_mecab, import_konlpy, import_unidic_lite
 
+import_nltk()
 import nltk
 import yaml
 from nltk import word_tokenize
 from nltk.corpus import stopwords
 from nltk.stem.snowball import SnowballStemmer
 
 logger = logging.getLogger(__name__)
@@ -110,28 +112,31 @@
         error_message = "Each tokenizer must implement its 'tokenize' method."
         raise NotImplementedError(error_message)
 
 
 @register_class("JiebaTokenizer")
 class JiebaTokenizer(Tokenizer):
     def __init__(self):
+        import_jieba()
         if find_spec("jieba") is None:
             error_message = "jieba is required for JiebaTokenizer but is not installed. Please install it using 'pip install jieba'."
             logger.error(error_message)
             raise ImportError(error_message)
 
     def tokenize(self, text: str):
         import jieba
 
         return jieba.lcut(text)
 
 
 @register_class("MecabTokenizer")
 class MecabTokenizer(Tokenizer):
     def __init__(self):
+        import_unidic_lite()
+        import_mecab()
         if find_spec("MeCab") is None:
             error_message = "MeCab is required for MecabTokenizer but is not installed. Please install it using 'pip install mecab-python3'."
             logger.error(error_message)
             raise ImportError(error_message)
 
     def tokenize(self, text: str):
         import MeCab
@@ -139,14 +144,15 @@
         wakati = MeCab.Tagger("-Owakati")
         return wakati.parse(text).split()
 
 
 @register_class("KonlpyTokenizer")
 class KonlpyTokenizer(Tokenizer):
     def __init__(self):
+        import_konlpy()
         if find_spec("konlpy") is None:
             error_message = "konlpy is required for KonlpyTokenizer but is not installed. Please install it using 'pip install konlpy'."
             logger.error(error_message)
             raise ImportError(error_message)
 
     def tokenize(self, text: str):
         from konlpy.tag import Kkma
@@ -174,18 +180,18 @@
         for _filter in self.filters:
             tokens = _filter.apply(tokens)
         return tokens
 
 
 def build_default_analyzer(language: str = "en"):
     default_config_path = Path(__file__).parent / "lang.yaml"
-    return build_analyer_from_yaml(default_config_path, language)
+    return build_analyzer_from_yaml(default_config_path, language)
 
 
-def build_analyer_from_yaml(filepath: str, name: str):
+def build_analyzer_from_yaml(filepath: str, name: str):
     with Path(filepath).open(encoding="utf-8") as file:
         config = yaml.safe_load(file)
 
     lang_config = config.get(name)
     if not lang_config:
         error_message = f"No configuration found {name}"
         raise ValueError(error_message)
```

### Comparing `milvus_model-0.2.1/milvus_model/sparse/splade.py` & `milvus_model-0.2.2/milvus_model/sparse/splade.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,20 @@
 import logging
 from typing import Dict, List, Optional
 
 import torch
 from scipy.sparse import csr_array, vstack
 
 from milvus_model.base import BaseEmbeddingFunction
+from milvus_model.utils import import_transformers, import_scipy, import_torch
+
+import_torch()
+import_scipy()
+import_transformers()
+from transformers import AutoModelForMaskedLM, AutoTokenizer
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 class SpladeEmbeddingFunction(BaseEmbeddingFunction):
     model_name: str
@@ -99,19 +105,14 @@
     def __init__(
         self,
         model_name_or_path: Optional[str] = None,
         device: Optional[str] = None,
         batch_size: int = 32,
         **kwargs,
     ):
-        try:
-            from transformers import AutoModelForMaskedLM, AutoTokenizer
-        except ImportError as _:
-            logger.error("transformers is not installed.")
-
         self.device = device
         self.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path)
         self.model = AutoModelForMaskedLM.from_pretrained(model_name_or_path, **kwargs)
         self.model.to(self.device)
         self.batch_size = batch_size
 
         self.relu = torch.nn.ReLU()
```

### Comparing `milvus_model-0.2.1/milvus_model.egg-info/PKG-INFO` & `milvus_model-0.2.2/milvus_model.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 Metadata-Version: 2.1
 Name: milvus-model
-Version: 0.2.1
+Version: 0.2.2
 Summary: Model components for PyMilvus, the Python SDK for Milvus
 Author-email: Milvus Team <milvus-team@zilliz.com>
 Project-URL: repository, https://github.com/milvus-io/milvus-model
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai>=1.12.0
-Requires-Dist: sentence-transformers
-Requires-Dist: FlagEmbedding>=1.2.2
-Requires-Dist: nltk
 Requires-Dist: transformers>=4.36.0
-Requires-Dist: jieba
-Requires-Dist: konlpy
-Requires-Dist: mecab-python3
+Requires-Dist: onnxruntime
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: protobuf==3.20.2
-Requires-Dist: unidic-lite
-Requires-Dist: cohere
-Requires-Dist: voyageai>=0.2.0
+Requires-Dist: numpy
 
 # Milvus Model Lib
 
 The milvus-model library provides model components for PyMilvus, the official Python SDK for Milvus, an open-source vector database built for AI applications.
 
 ## Installation
```

### Comparing `milvus_model-0.2.1/milvus_model.egg-info/SOURCES.txt` & `milvus_model-0.2.2/milvus_model.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 milvus_model.egg-info/PKG-INFO
 milvus_model.egg-info/SOURCES.txt
 milvus_model.egg-info/dependency_links.txt
 milvus_model.egg-info/requires.txt
 milvus_model.egg-info/top_level.txt
 milvus_model/dense/__init__.py
 milvus_model/dense/jinaai.py
+milvus_model/dense/onnx.py
 milvus_model/dense/openai.py
 milvus_model/dense/sentence_transformer.py
 milvus_model/dense/voyageai.py
 milvus_model/hybrid/__init__.py
 milvus_model/hybrid/bge_m3.py
 milvus_model/reranker/__init__.py
 milvus_model/reranker/bgereranker.py
@@ -26,8 +27,11 @@
 milvus_model/reranker/jinaai.py
 milvus_model/reranker/voyageai.py
 milvus_model/sparse/__init__.py
 milvus_model/sparse/splade.py
 milvus_model/sparse/bm25/__init__.py
 milvus_model/sparse/bm25/bm25.py
 milvus_model/sparse/bm25/lang.yaml
-milvus_model/sparse/bm25/tokenizers.py
+milvus_model/sparse/bm25/tokenizers.py
+milvus_model/utils/__init__.py
+milvus_model/utils/dependency_control.py
+milvus_model/utils/lazy_import.py
```

### Comparing `milvus_model-0.2.1/pyproject.toml` & `milvus_model-0.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -12,27 +12,19 @@
 authors = [
   {name = "Milvus Team", email = "milvus-team@zilliz.com"},
 ]
 requires-python = ">=3.8"
 description = "Model components for PyMilvus, the Python SDK for Milvus"
 readme = "README.md"
 dependencies = [
-    "openai >= 1.12.0",
-    "sentence-transformers",
-    "FlagEmbedding >= 1.2.2",
-    "nltk",
     "transformers >= 4.36.0",
-    "jieba",
-    "konlpy",
-    "mecab-python3",
+    "onnxruntime",
     "scipy >= 1.10.0",
     "protobuf==3.20.2",
-    "unidic-lite",
-    "cohere",
-    "voyageai >= 0.2.0",
+    "numpy"
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
```

