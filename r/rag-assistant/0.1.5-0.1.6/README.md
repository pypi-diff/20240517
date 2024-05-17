# Comparing `tmp/rag_assistant-0.1.5.tar.gz` & `tmp/rag_assistant-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_assistant-0.1.5.tar", last modified: Fri May 17 03:39:12 2024, max compression
+gzip compressed data, was "rag_assistant-0.1.6.tar", last modified: Fri May 17 03:49:42 2024, max compression
```

## Comparing `rag_assistant-0.1.5.tar` & `rag_assistant-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:12.882539 rag_assistant-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 03:39:12.882539 rag_assistant-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-17 03:39:01.000000 rag_assistant-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:12.882539 rag_assistant-0.1.5/rag_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)    18823 2024-05-17 03:39:01.000000 rag_assistant-0.1.5/rag_assistant/RagAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-17 03:39:01.000000 rag_assistant-0.1.5/rag_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:12.882539 rag_assistant-0.1.5/rag_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 03:39:12.000000 rag_assistant-0.1.5/rag_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 03:39:12.000000 rag_assistant-0.1.5/rag_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:39:12.000000 rag_assistant-0.1.5/rag_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 03:39:12.000000 rag_assistant-0.1.5/rag_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 03:39:12.000000 rag_assistant-0.1.5/rag_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 03:39:12.000000 rag_assistant-0.1.5/rag_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:39:12.882539 rag_assistant-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-17 03:39:01.000000 rag_assistant-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:49:42.332821 rag_assistant-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 03:49:42.332821 rag_assistant-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-17 03:49:30.000000 rag_assistant-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:49:42.332821 rag_assistant-0.1.6/rag_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)    18823 2024-05-17 03:49:30.000000 rag_assistant-0.1.6/rag_assistant/RagAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-17 03:49:30.000000 rag_assistant-0.1.6/rag_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:49:42.332821 rag_assistant-0.1.6/rag_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 03:49:42.000000 rag_assistant-0.1.6/rag_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 03:49:42.000000 rag_assistant-0.1.6/rag_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:49:42.000000 rag_assistant-0.1.6/rag_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 03:49:42.000000 rag_assistant-0.1.6/rag_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 03:49:42.000000 rag_assistant-0.1.6/rag_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 03:49:42.000000 rag_assistant-0.1.6/rag_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:49:42.336821 rag_assistant-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-17 03:49:30.000000 rag_assistant-0.1.6/setup.py
```

### Comparing `rag_assistant-0.1.5/PKG-INFO` & `rag_assistant-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag_assistant
-Version: 0.1.5
+Version: 0.1.6
 Summary: The Swarmauri Rag Assistant is part of the swarmaURI framework.
 Home-page: http://github.com/swarmauri/rag_assistant
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -16,14 +16,14 @@
 # Swarmauri Rag Assistant
 
 ## Overview
 The Swarmauri Rag Assistant
 
 ## Installation
 ```bash
-pip install rag_assistant==0.1.5 --user
+pip install rag_assistant==0.1.6 --user
 ```
 
 ## Execution
 ```bash
 ! rag_assistant --api_key "YOUR API KEY" --db_path "E:\swarmauri_github/prompt_responses.db" --system_context "You are a helpful assistant."
 ```
```

### Comparing `rag_assistant-0.1.5/rag_assistant/RagAssistant.py` & `rag_assistant-0.1.6/rag_assistant/RagAssistant.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -60,29 +60,29 @@
                             'anthropic_claude-3-haiku-20240307'])
             
         self.model = None
         self.retrieval_table = []
         self.document_table = []
         self.long_term_memory_df = None
         self.last_recall_df = None
+        self.agent = self.initialize_agent()
         self.set_model(model_name)
         self.css = """
 #chat-dialogue-container {
     min-height: 54vh !important;
 }
 
 #document-table-container {
     min-height: 80vh !important;
 }
 
 footer {
     display: none !important;
 }
 """
-        self.agent = self.initialize_agent()
         self.setup_gradio_interface()
         
     def initialize_agent(self):
         VS = Doc2VecVectorStore()
         agent = RagAgent(name="Rag", 
                          system_context=self.system_context, 
                          model=self.model,
```

### Comparing `rag_assistant-0.1.5/rag_assistant.egg-info/PKG-INFO` & `rag_assistant-0.1.6/rag_assistant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag_assistant
-Version: 0.1.5
+Version: 0.1.6
 Summary: The Swarmauri Rag Assistant is part of the swarmaURI framework.
 Home-page: http://github.com/swarmauri/rag_assistant
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -16,14 +16,14 @@
 # Swarmauri Rag Assistant
 
 ## Overview
 The Swarmauri Rag Assistant
 
 ## Installation
 ```bash
-pip install rag_assistant==0.1.5 --user
+pip install rag_assistant==0.1.6 --user
 ```
 
 ## Execution
 ```bash
 ! rag_assistant --api_key "YOUR API KEY" --db_path "E:\swarmauri_github/prompt_responses.db" --system_context "You are a helpful assistant."
 ```
```

### Comparing `rag_assistant-0.1.5/setup.py` & `rag_assistant-0.1.6/setup.py`

 * *Files identical despite different names*

