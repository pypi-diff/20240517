# Comparing `tmp/modelmerge-0.4.2.tar.gz` & `tmp/modelmerge-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.4.2.tar", last modified: Fri May 17 01:52:23 2024, max compression
+gzip compressed data, was "modelmerge-0.4.3.tar", last modified: Fri May 17 03:25:43 2024, max compression
```

## Comparing `modelmerge-0.4.2.tar` & `modelmerge-0.4.3.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:52:23.388895 modelmerge-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-17 01:52:14.000000 modelmerge-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-17 01:52:23.384895 modelmerge-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-17 01:52:14.000000 modelmerge-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 01:52:23.388895 modelmerge-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-17 01:52:14.000000 modelmerge-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:52:23.376895 modelmerge-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:52:23.380895 modelmerge-0.4.2/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:52:23.380895 modelmerge-0.4.2/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30876 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:52:23.380895 modelmerge-0.4.2/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:52:23.380895 modelmerge-0.4.2/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:52:23.380895 modelmerge-0.4.2/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-17 01:52:14.000000 modelmerge-0.4.2/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:52:23.384895 modelmerge-0.4.2/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-17 01:52:23.000000 modelmerge-0.4.2/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-17 01:52:23.000000 modelmerge-0.4.2/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 01:52:23.000000 modelmerge-0.4.2/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-17 01:52:23.000000 modelmerge-0.4.2/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 01:52:23.000000 modelmerge-0.4.2/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:52:23.384895 modelmerge-0.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 01:52:14.000000 modelmerge-0.4.2/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-17 01:52:14.000000 modelmerge-0.4.2/test/test_API.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-17 01:52:14.000000 modelmerge-0.4.2/test/test_Web_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-17 01:52:14.000000 modelmerge-0.4.2/test/test_claude_zh_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-17 01:52:14.000000 modelmerge-0.4.2/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-17 01:52:14.000000 modelmerge-0.4.2/test/test_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-17 01:52:14.000000 modelmerge-0.4.2/test/test_google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-17 01:52:14.000000 modelmerge-0.4.2/test/test_jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-17 01:52:14.000000 modelmerge-0.4.2/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-17 01:52:14.000000 modelmerge-0.4.2/test/test_langchain_search_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-17 01:52:14.000000 modelmerge-0.4.2/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-17 01:52:14.000000 modelmerge-0.4.2/test/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-17 01:52:14.000000 modelmerge-0.4.2/test/test_tikitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-17 01:52:14.000000 modelmerge-0.4.2/test/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-17 01:52:14.000000 modelmerge-0.4.2/test/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 01:52:14.000000 modelmerge-0.4.2/test/test_whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.579851 modelmerge-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-17 03:25:31.000000 modelmerge-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-17 03:25:43.579851 modelmerge-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-17 03:25:31.000000 modelmerge-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:25:43.579851 modelmerge-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-17 03:25:31.000000 modelmerge-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.571852 modelmerge-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.571852 modelmerge-0.4.3/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.571852 modelmerge-0.4.3/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31202 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.571852 modelmerge-0.4.3/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.571852 modelmerge-0.4.3/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.575852 modelmerge-0.4.3/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.579851 modelmerge-0.4.3/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-17 03:25:43.000000 modelmerge-0.4.3/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-17 03:25:43.000000 modelmerge-0.4.3/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:25:43.000000 modelmerge-0.4.3/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-17 03:25:43.000000 modelmerge-0.4.3/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 03:25:43.000000 modelmerge-0.4.3/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.575852 modelmerge-0.4.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_whisper.py
```

### Comparing `modelmerge-0.4.2/LICENSE` & `modelmerge-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/PKG-INFO` & `modelmerge-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.4.2
+Version: 0.4.3
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.4.2/README.md` & `modelmerge-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.4.3/src/ModelMerge/models/chatgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -442,14 +442,18 @@
                     function_response = (
                         f"You need to response the following question: {city}. Tarvel infomation is provided inside <infomation></infomation> XML tags. Your task is to think about the question step by step and then answer the above question in {LANGUAGE} based on the tarvel infomation provided. Please response in {LANGUAGE} and adopt a style that is logical, in-depth, and detailed. Note: In order to make the answer appear highly professional, you should be an expert in textual analysis, aiming to make the answer precise and comprehensive."
                         "Here is the tarvel infomation, inside <infomation></infomation> XML tags:"
                         "<infomation>"
                         "{}"
                         "</infomation>"
                     ).format(function_response)
+                if function_call_name == "generate_image":
+                    prompt = json.loads(function_full_response)["prompt"]
+                    function_response = eval(function_call_name)(prompt)
+                    function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                 if function_call_name == "get_date_time_weekday":
                     function_response = eval(function_call_name)()
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                 if function_call_name == "get_version_info":
                     function_response = eval(function_call_name)()
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
             else:
```

### Comparing `modelmerge-0.4.2/src/ModelMerge/models/claude.py` & `modelmerge-0.4.3/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/src/ModelMerge/models/config.py` & `modelmerge-0.4.3/src/ModelMerge/models/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 
 from ..utils import prompt
 
 PLUGINS = {
     "SEARCH": (os.environ.get('SEARCH', "True") == "False") == False,
     "URL": True,
+    "IMAGE": (os.environ.get('IMAGE', "True") == "False") == False,
     "DATE": False,
     "VERSION": False,
     "TARVEL": (os.environ.get('TARVEL', "False") == "False") == False,
 }
 
 LANGUAGE = os.environ.get('LANGUAGE', 'Simplified Chinese')
```

### Comparing `modelmerge-0.4.2/src/ModelMerge/models/genimi.py` & `modelmerge-0.4.3/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/src/ModelMerge/models/groq.py` & `modelmerge-0.4.3/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.4.3/src/ModelMerge/plugins/tarvel.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.4.3/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/src/ModelMerge/tools/function_call.py` & `modelmerge-0.4.3/src/ModelMerge/tools/function_call.py`

 * *Files 21% similar despite different names*

```diff
@@ -87,14 +87,30 @@
                 }
             },
             "required": [
                 "city"
             ]
         }
     },
+    "IMAGE": {
+        "name": "generate_image",
+        "description": "Generate images based on user descriptions.",
+        "parameters": {
+            "type": "object",
+            "properties": {
+                "prompt": {
+                    "type": "string",
+                    "description": "the prompt to generate image"
+                }
+            },
+            "required": [
+                "prompt"
+            ]
+        }
+    },
 }
 def gpt2claude_tools_json(json_dict):
     import copy
     json_dict = copy.deepcopy(json_dict)
     keys_to_change = {
         "parameters": "input_schema",
         "functions": "tools",
```

### Comparing `modelmerge-0.4.2/src/ModelMerge/utils/prompt.py` & `modelmerge-0.4.3/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/src/ModelMerge/utils/scripts.py` & `modelmerge-0.4.3/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.4.3/src/modelmerge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.4.2
+Version: 0.4.3
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.4.2/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.4.3/src/modelmerge.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/ModelMerge/models/__init__.py
 src/ModelMerge/models/chatgpt.py
 src/ModelMerge/models/claude.py
 src/ModelMerge/models/config.py
 src/ModelMerge/models/genimi.py
 src/ModelMerge/models/groq.py
 src/ModelMerge/plugins/__init__.py
+src/ModelMerge/plugins/image.py
 src/ModelMerge/plugins/tarvel.py
 src/ModelMerge/plugins/today.py
 src/ModelMerge/plugins/version.py
 src/ModelMerge/plugins/websearch.py
 src/ModelMerge/tools/__init__.py
 src/ModelMerge/tools/function_call.py
 src/ModelMerge/utils/__init__.py
```

### Comparing `modelmerge-0.4.2/test/test_Web_crawler.py` & `modelmerge-0.4.3/test/test_Web_crawler.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/test/test_claude_zh_char.py` & `modelmerge-0.4.3/test/test_claude_zh_char.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/test/test_ddg_search.py` & `modelmerge-0.4.3/test/test_ddg_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/test/test_download_pdf.py` & `modelmerge-0.4.3/test/test_download_pdf.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/test/test_google_search.py` & `modelmerge-0.4.3/test/test_google_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/test/test_jieba.py` & `modelmerge-0.4.3/test/test_jieba.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/test/test_json.py` & `modelmerge-0.4.3/test/test_json.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/test/test_langchain_search_old.py` & `modelmerge-0.4.3/test/test_langchain_search_old.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/test/test_logging.py` & `modelmerge-0.4.3/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/test/test_ollama.py` & `modelmerge-0.4.3/test/test_ollama.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/test/test_tikitoken.py` & `modelmerge-0.4.3/test/test_tikitoken.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/test/test_token.py` & `modelmerge-0.4.3/test/test_token.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.2/test/test_url.py` & `modelmerge-0.4.3/test/test_url.py`

 * *Files identical despite different names*

