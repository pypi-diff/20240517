# Comparing `tmp/rag_assistant-0.1.2.tar.gz` & `tmp/rag_assistant-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_assistant-0.1.2.tar", last modified: Wed May 15 22:17:37 2024, max compression
+gzip compressed data, was "rag_assistant-0.1.3.tar", last modified: Fri May 17 01:55:14 2024, max compression
```

## Comparing `rag_assistant-0.1.2.tar` & `rag_assistant-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:17:37.981813 rag_assistant-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-15 22:17:37.981813 rag_assistant-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-15 22:17:29.000000 rag_assistant-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:17:37.981813 rag_assistant-0.1.2/rag_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)    18763 2024-05-15 22:17:29.000000 rag_assistant-0.1.2/rag_assistant/RagAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-15 22:17:29.000000 rag_assistant-0.1.2/rag_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:17:37.981813 rag_assistant-0.1.2/rag_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-15 22:17:37.000000 rag_assistant-0.1.2/rag_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-15 22:17:37.000000 rag_assistant-0.1.2/rag_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 22:17:37.000000 rag_assistant-0.1.2/rag_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 22:17:37.000000 rag_assistant-0.1.2/rag_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 22:17:37.000000 rag_assistant-0.1.2/rag_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 22:17:37.000000 rag_assistant-0.1.2/rag_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 22:17:37.981813 rag_assistant-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-15 22:17:29.000000 rag_assistant-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:55:14.759526 rag_assistant-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-17 01:55:14.759526 rag_assistant-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-17 01:55:01.000000 rag_assistant-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:55:14.755526 rag_assistant-0.1.3/rag_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)    18763 2024-05-17 01:55:01.000000 rag_assistant-0.1.3/rag_assistant/RagAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-17 01:55:01.000000 rag_assistant-0.1.3/rag_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:55:14.759526 rag_assistant-0.1.3/rag_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-17 01:55:14.000000 rag_assistant-0.1.3/rag_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 01:55:14.000000 rag_assistant-0.1.3/rag_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 01:55:14.000000 rag_assistant-0.1.3/rag_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 01:55:14.000000 rag_assistant-0.1.3/rag_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 01:55:14.000000 rag_assistant-0.1.3/rag_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 01:55:14.000000 rag_assistant-0.1.3/rag_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 01:55:14.759526 rag_assistant-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-17 01:55:01.000000 rag_assistant-0.1.3/setup.py
```

### Comparing `rag_assistant-0.1.2/PKG-INFO` & `rag_assistant-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag_assistant
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Swarmauri Rag Assistant is part of the swarmaURI framework.
 Home-page: http://github.com/swarmauri/rag_assistant
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -21,9 +21,9 @@
 ## Installation
 ```bash
 pip install rag_assistant==0.1.1 --user
 ```
 
 ## Execution
 ```bash
-! rag_assistant --api_key "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" --db_path "E:\swarmauri_github/prompt_responses.db"
+! rag_assistant --api_key "YOUR API KEY" --db_path "E:\swarmauri_github/prompt_responses.db"
 ```
```

### Comparing `rag_assistant-0.1.2/rag_assistant/RagAssistant.py` & `rag_assistant-0.1.3/rag_assistant/RagAssistant.py`

 * *Files identical despite different names*

### Comparing `rag_assistant-0.1.2/rag_assistant.egg-info/PKG-INFO` & `rag_assistant-0.1.3/rag_assistant.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag_assistant
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Swarmauri Rag Assistant is part of the swarmaURI framework.
 Home-page: http://github.com/swarmauri/rag_assistant
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -21,9 +21,9 @@
 ## Installation
 ```bash
 pip install rag_assistant==0.1.1 --user
 ```
 
 ## Execution
 ```bash
-! rag_assistant --api_key "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" --db_path "E:\swarmauri_github/prompt_responses.db"
+! rag_assistant --api_key "YOUR API KEY" --db_path "E:\swarmauri_github/prompt_responses.db"
 ```
```

### Comparing `rag_assistant-0.1.2/setup.py` & `rag_assistant-0.1.3/setup.py`

 * *Files identical despite different names*

