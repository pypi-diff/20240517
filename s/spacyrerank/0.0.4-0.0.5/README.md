# Comparing `tmp/spacyrerank-0.0.4.tar.gz` & `tmp/spacyrerank-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacyrerank-0.0.4.tar", last modified: Fri May 17 06:10:47 2024, max compression
+gzip compressed data, was "spacyrerank-0.0.5.tar", last modified: Fri May 17 06:16:00 2024, max compression
```

## Comparing `spacyrerank-0.0.4.tar` & `spacyrerank-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:10:47.062645 spacyrerank-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-17 06:10:34.000000 spacyrerank-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-17 06:10:47.062645 spacyrerank-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-17 06:10:34.000000 spacyrerank-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-17 06:10:47.062645 spacyrerank-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-17 06:10:34.000000 spacyrerank-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:10:47.062645 spacyrerank-0.0.4/spacyrerank/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:10:34.000000 spacyrerank-0.0.4/spacyrerank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-17 06:10:34.000000 spacyrerank-0.0.4/spacyrerank/rerank.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-17 06:10:34.000000 spacyrerank-0.0.4/spacyrerank/spacy_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:10:47.062645 spacyrerank-0.0.4/spacyrerank.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-17 06:10:47.000000 spacyrerank-0.0.4/spacyrerank.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-17 06:10:47.000000 spacyrerank-0.0.4/spacyrerank.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:10:47.000000 spacyrerank-0.0.4/spacyrerank.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:10:46.000000 spacyrerank-0.0.4/spacyrerank.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 06:10:47.000000 spacyrerank-0.0.4/spacyrerank.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 06:10:47.000000 spacyrerank-0.0.4/spacyrerank.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:16:00.112599 spacyrerank-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-17 06:15:43.000000 spacyrerank-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-17 06:16:00.112599 spacyrerank-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-17 06:15:43.000000 spacyrerank-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-17 06:16:00.112599 spacyrerank-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-17 06:15:43.000000 spacyrerank-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:16:00.108600 spacyrerank-0.0.5/spacyrerank/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:15:43.000000 spacyrerank-0.0.5/spacyrerank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-17 06:15:43.000000 spacyrerank-0.0.5/spacyrerank/rerank.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-17 06:15:43.000000 spacyrerank-0.0.5/spacyrerank/spacy_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:16:00.112599 spacyrerank-0.0.5/spacyrerank.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-17 06:16:00.000000 spacyrerank-0.0.5/spacyrerank.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-17 06:16:00.000000 spacyrerank-0.0.5/spacyrerank.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:16:00.000000 spacyrerank-0.0.5/spacyrerank.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:15:59.000000 spacyrerank-0.0.5/spacyrerank.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 06:16:00.000000 spacyrerank-0.0.5/spacyrerank.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 06:16:00.000000 spacyrerank-0.0.5/spacyrerank.egg-info/top_level.txt
```

### Comparing `spacyrerank-0.0.4/LICENSE` & `spacyrerank-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spacyrerank-0.0.4/PKG-INFO` & `spacyrerank-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacyrerank
-Version: 0.0.4
+Version: 0.0.5
 Summary: Rank phrases and text based on query by leveraging hugging-face models.
 Home-page: https://github.com/Vishnunkumar/spacyrerank
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: reranker,spacy,transformers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spacyrerank-0.0.4/README.md` & `spacyrerank-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `spacyrerank-0.0.4/setup.py` & `spacyrerank-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   'torch',
   'spacy'
 ]
 
 
 setuptools.setup(
     name="spacyrerank",
-    version="0.0.4",
+    version="0.0.5",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Rank phrases and text based on query by leveraging hugging-face models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/spacyrerank',
     packages=[
```

### Comparing `spacyrerank-0.0.4/spacyrerank/rerank.py` & `spacyrerank-0.0.5/spacyrerank/rerank.py`

 * *Files identical despite different names*

### Comparing `spacyrerank-0.0.4/spacyrerank/spacy_pipeline.py` & `spacyrerank-0.0.5/spacyrerank/spacy_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import spacy
 from transformers import AutoTokenizer, AutoModel
 from functools import lru_cache
 
 
 @lru_cache(maxsize=128)
 def load_model():
-    model_path = "spacyrerank/models/tiny/"
+    model_path = "models/tiny/"
     tokenizer = AutoTokenizer.from_pretrained(model_path)
     model = AutoModel.from_pretrained(model_path)
     return model, tokenizer
 
 
 @lru_cache(maxsize=128)
 def get_embeddings(text):
```

### Comparing `spacyrerank-0.0.4/spacyrerank.egg-info/PKG-INFO` & `spacyrerank-0.0.5/spacyrerank.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacyrerank
-Version: 0.0.4
+Version: 0.0.5
 Summary: Rank phrases and text based on query by leveraging hugging-face models.
 Home-page: https://github.com/Vishnunkumar/spacyrerank
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: reranker,spacy,transformers
 Classifier: Development Status :: 3 - Alpha
```

