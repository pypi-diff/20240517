# Comparing `tmp/modelmerge-0.4.4.tar.gz` & `tmp/modelmerge-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.4.4.tar", last modified: Fri May 17 03:47:17 2024, max compression
+gzip compressed data, was "modelmerge-0.4.5.tar", last modified: Fri May 17 04:20:51 2024, max compression
```

## Comparing `modelmerge-0.4.4.tar` & `modelmerge-0.4.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.988625 modelmerge-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-17 03:47:05.000000 modelmerge-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-17 03:47:17.988625 modelmerge-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-17 03:47:05.000000 modelmerge-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:47:17.988625 modelmerge-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-17 03:47:05.000000 modelmerge-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.980625 modelmerge-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.980625 modelmerge-0.4.4/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.980625 modelmerge-0.4.4/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29573 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.984625 modelmerge-0.4.4/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.984625 modelmerge-0.4.4/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.984625 modelmerge-0.4.4/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.988625 modelmerge-0.4.4/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-17 03:47:17.000000 modelmerge-0.4.4/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-17 03:47:17.000000 modelmerge-0.4.4/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:47:17.000000 modelmerge-0.4.4/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-17 03:47:17.000000 modelmerge-0.4.4/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 03:47:17.000000 modelmerge-0.4.4/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.988625 modelmerge-0.4.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_API.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_Web_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_claude_zh_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_langchain_search_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_tikitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:51.547686 modelmerge-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-17 04:20:42.000000 modelmerge-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-17 04:20:51.547686 modelmerge-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-17 04:20:42.000000 modelmerge-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 04:20:51.547686 modelmerge-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-17 04:20:42.000000 modelmerge-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:51.543686 modelmerge-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:51.543686 modelmerge-0.4.5/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:51.543686 modelmerge-0.4.5/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29573 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:51.543686 modelmerge-0.4.5/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:51.543686 modelmerge-0.4.5/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:51.543686 modelmerge-0.4.5/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-17 04:20:42.000000 modelmerge-0.4.5/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:51.547686 modelmerge-0.4.5/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-17 04:20:51.000000 modelmerge-0.4.5/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-17 04:20:51.000000 modelmerge-0.4.5/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 04:20:51.000000 modelmerge-0.4.5/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-17 04:20:51.000000 modelmerge-0.4.5/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 04:20:51.000000 modelmerge-0.4.5/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:51.547686 modelmerge-0.4.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 04:20:42.000000 modelmerge-0.4.5/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-17 04:20:42.000000 modelmerge-0.4.5/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-17 04:20:42.000000 modelmerge-0.4.5/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-17 04:20:42.000000 modelmerge-0.4.5/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-17 04:20:42.000000 modelmerge-0.4.5/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-17 04:20:42.000000 modelmerge-0.4.5/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-17 04:20:42.000000 modelmerge-0.4.5/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-17 04:20:42.000000 modelmerge-0.4.5/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-17 04:20:42.000000 modelmerge-0.4.5/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-17 04:20:42.000000 modelmerge-0.4.5/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-17 04:20:42.000000 modelmerge-0.4.5/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-17 04:20:42.000000 modelmerge-0.4.5/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-17 04:20:42.000000 modelmerge-0.4.5/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-17 04:20:42.000000 modelmerge-0.4.5/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-17 04:20:42.000000 modelmerge-0.4.5/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 04:20:42.000000 modelmerge-0.4.5/test/test_whisper.py
```

### Comparing `modelmerge-0.4.4/LICENSE` & `modelmerge-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/PKG-INFO` & `modelmerge-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.4.4
+Version: 0.4.5
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.4.4/README.md` & `modelmerge-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.4.5/src/ModelMerge/models/chatgpt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/src/ModelMerge/models/claude.py` & `modelmerge-0.4.5/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/src/ModelMerge/models/config.py` & `modelmerge-0.4.5/src/ModelMerge/models/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 
 from ..utils import prompt
 
 PLUGINS = {
     "SEARCH": (os.environ.get('SEARCH', "True") == "False") == False,
     "URL": True,
-    "IMAGE": (os.environ.get('IMAGE', "True") == "False") == False,
+    "IMAGE": (os.environ.get('IMAGE', "False") == "False") == False,
     "DATE": False,
     "VERSION": False,
     "TARVEL": (os.environ.get('TARVEL', "False") == "False") == False,
 }
 
 LANGUAGE = os.environ.get('LANGUAGE', 'Simplified Chinese')
```

### Comparing `modelmerge-0.4.4/src/ModelMerge/models/genimi.py` & `modelmerge-0.4.5/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/src/ModelMerge/models/groq.py` & `modelmerge-0.4.5/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/src/ModelMerge/plugins/image.py` & `modelmerge-0.4.5/src/ModelMerge/plugins/image.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.4.5/src/ModelMerge/plugins/tarvel.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.4.5/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/src/ModelMerge/tools/function_call.py` & `modelmerge-0.4.5/src/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/src/ModelMerge/utils/prompt.py` & `modelmerge-0.4.5/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/src/ModelMerge/utils/scripts.py` & `modelmerge-0.4.5/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.4.5/src/modelmerge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.4.4
+Version: 0.4.5
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.4.4/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.4.5/src/modelmerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/test/test_Web_crawler.py` & `modelmerge-0.4.5/test/test_Web_crawler.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/test/test_claude_zh_char.py` & `modelmerge-0.4.5/test/test_claude_zh_char.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/test/test_ddg_search.py` & `modelmerge-0.4.5/test/test_ddg_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/test/test_download_pdf.py` & `modelmerge-0.4.5/test/test_download_pdf.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/test/test_google_search.py` & `modelmerge-0.4.5/test/test_google_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/test/test_jieba.py` & `modelmerge-0.4.5/test/test_jieba.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/test/test_json.py` & `modelmerge-0.4.5/test/test_json.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/test/test_langchain_search_old.py` & `modelmerge-0.4.5/test/test_langchain_search_old.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/test/test_logging.py` & `modelmerge-0.4.5/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/test/test_ollama.py` & `modelmerge-0.4.5/test/test_ollama.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/test/test_tikitoken.py` & `modelmerge-0.4.5/test/test_tikitoken.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/test/test_token.py` & `modelmerge-0.4.5/test/test_token.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.4/test/test_url.py` & `modelmerge-0.4.5/test/test_url.py`

 * *Files identical despite different names*

