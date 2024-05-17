# Comparing `tmp/rag_assistant-0.1.3.tar.gz` & `tmp/rag_assistant-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_assistant-0.1.3.tar", last modified: Fri May 17 01:55:14 2024, max compression
+gzip compressed data, was "rag_assistant-0.1.4.tar", last modified: Fri May 17 03:29:14 2024, max compression
```

## Comparing `rag_assistant-0.1.3.tar` & `rag_assistant-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:55:14.759526 rag_assistant-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-17 01:55:14.759526 rag_assistant-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-17 01:55:01.000000 rag_assistant-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:55:14.755526 rag_assistant-0.1.3/rag_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)    18763 2024-05-17 01:55:01.000000 rag_assistant-0.1.3/rag_assistant/RagAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-17 01:55:01.000000 rag_assistant-0.1.3/rag_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:55:14.759526 rag_assistant-0.1.3/rag_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-17 01:55:14.000000 rag_assistant-0.1.3/rag_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 01:55:14.000000 rag_assistant-0.1.3/rag_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 01:55:14.000000 rag_assistant-0.1.3/rag_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 01:55:14.000000 rag_assistant-0.1.3/rag_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 01:55:14.000000 rag_assistant-0.1.3/rag_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 01:55:14.000000 rag_assistant-0.1.3/rag_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 01:55:14.759526 rag_assistant-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-17 01:55:01.000000 rag_assistant-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:29:14.941553 rag_assistant-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 03:29:14.941553 rag_assistant-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-17 03:29:07.000000 rag_assistant-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:29:14.937553 rag_assistant-0.1.4/rag_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)    18823 2024-05-17 03:29:07.000000 rag_assistant-0.1.4/rag_assistant/RagAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-17 03:29:07.000000 rag_assistant-0.1.4/rag_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:29:14.941553 rag_assistant-0.1.4/rag_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 03:29:14.000000 rag_assistant-0.1.4/rag_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 03:29:14.000000 rag_assistant-0.1.4/rag_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:29:14.000000 rag_assistant-0.1.4/rag_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 03:29:14.000000 rag_assistant-0.1.4/rag_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 03:29:14.000000 rag_assistant-0.1.4/rag_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 03:29:14.000000 rag_assistant-0.1.4/rag_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:29:14.941553 rag_assistant-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-17 03:29:07.000000 rag_assistant-0.1.4/setup.py
```

### Comparing `rag_assistant-0.1.3/PKG-INFO` & `rag_assistant-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag_assistant
-Version: 0.1.3
+Version: 0.1.4
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
-pip install rag_assistant==0.1.1 --user
+pip install rag_assistant==0.1.3 --user
 ```
 
 ## Execution
 ```bash
-! rag_assistant --api_key "YOUR API KEY" --db_path "E:\swarmauri_github/prompt_responses.db"
+! rag_assistant --api_key "YOUR API KEY" --db_path "E:\swarmauri_github/prompt_responses.db" --system_context "You are a helpful assistant."
 ```
```

### Comparing `rag_assistant-0.1.3/rag_assistant/RagAssistant.py` & `rag_assistant-0.1.4/rag_assistant/RagAssistant.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,29 +60,29 @@
                             'anthropic_claude-3-haiku-20240307'])
             
         self.model = None
         self.retrieval_table = []
         self.document_table = []
         self.long_term_memory_df = None
         self.last_recall_df = None
-        self.agent = self.initialize_agent()
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
+        self.agent = self.initialize_agent()
         self.setup_gradio_interface()
         
     def initialize_agent(self):
         VS = Doc2VecVectorStore()
         agent = RagAgent(name="Rag", 
                          system_context=self.system_context, 
                          model=self.model, 
@@ -345,15 +345,19 @@
             self.save_button.click(self.save_df, inputs=[self.data_frame])
 
         with gr.Blocks(css = self.css, title="Swarmauri Rag Agent") as self.app:
             gr.TabbedInterface(interface_list=[self.chat, self.retrieval_table, self.document_table], 
                                       tab_names=["chat", "retrieval", "documents"])
 
     
-    def launch(self, share: bool = False, server_name: Optional[str] = None, favicon_path: Optional[str] = None):
+    def launch(self, 
+        share: bool = False, 
+        server_name: Optional[str] = None, 
+        favicon_path: Optional[str] = None):
+
         kwargs = {}
         kwargs.update({'share': share})
         if server_name:
             kwargs.update({'server_name': server_name})
         if favicon_path:
             kwargs.update({'favicon_path': favicon_path})
 
@@ -397,13 +401,15 @@
     if args.share:
         launch_kwargs.update({'share': args.share})
     if args.server_name:
         launch_kwargs.update({'server_name': args.server_name})
     if args.favicon_path:
         launch_kwargs.update({'favicon_path': args.favicon_path})
     else:
-        launch_kwargs.update({'favicon_path': "./favicon-32x32.png"})
+        launch_kwargs.update({'favicon_path': "favicon-32x32.png"})
+
 
+    assistant.initialize_agent()
     assistant.launch(**launch_kwargs)
         
 if __name__ == "__main__":
     main()
```

### Comparing `rag_assistant-0.1.3/rag_assistant.egg-info/PKG-INFO` & `rag_assistant-0.1.4/rag_assistant.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag_assistant
-Version: 0.1.3
+Version: 0.1.4
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
-pip install rag_assistant==0.1.1 --user
+pip install rag_assistant==0.1.3 --user
 ```
 
 ## Execution
 ```bash
-! rag_assistant --api_key "YOUR API KEY" --db_path "E:\swarmauri_github/prompt_responses.db"
+! rag_assistant --api_key "YOUR API KEY" --db_path "E:\swarmauri_github/prompt_responses.db" --system_context "You are a helpful assistant."
 ```
```

### Comparing `rag_assistant-0.1.3/setup.py` & `rag_assistant-0.1.4/setup.py`

 * *Files identical despite different names*

