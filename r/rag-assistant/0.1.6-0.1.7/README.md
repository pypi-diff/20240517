# Comparing `tmp/rag_assistant-0.1.6.tar.gz` & `tmp/rag_assistant-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_assistant-0.1.6.tar", last modified: Fri May 17 03:49:42 2024, max compression
+gzip compressed data, was "rag_assistant-0.1.7.tar", last modified: Fri May 17 04:16:33 2024, max compression
```

## Comparing `rag_assistant-0.1.6.tar` & `rag_assistant-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:49:42.332821 rag_assistant-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 03:49:42.332821 rag_assistant-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-17 03:49:30.000000 rag_assistant-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:49:42.332821 rag_assistant-0.1.6/rag_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)    18823 2024-05-17 03:49:30.000000 rag_assistant-0.1.6/rag_assistant/RagAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-17 03:49:30.000000 rag_assistant-0.1.6/rag_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:49:42.332821 rag_assistant-0.1.6/rag_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 03:49:42.000000 rag_assistant-0.1.6/rag_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 03:49:42.000000 rag_assistant-0.1.6/rag_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:49:42.000000 rag_assistant-0.1.6/rag_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 03:49:42.000000 rag_assistant-0.1.6/rag_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 03:49:42.000000 rag_assistant-0.1.6/rag_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 03:49:42.000000 rag_assistant-0.1.6/rag_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:49:42.336821 rag_assistant-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-17 03:49:30.000000 rag_assistant-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:33.794029 rag_assistant-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 04:16:33.794029 rag_assistant-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-17 04:16:23.000000 rag_assistant-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:33.794029 rag_assistant-0.1.7/rag_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)    18864 2024-05-17 04:16:23.000000 rag_assistant-0.1.7/rag_assistant/RagAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-17 04:16:23.000000 rag_assistant-0.1.7/rag_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:33.794029 rag_assistant-0.1.7/rag_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 04:16:33.000000 rag_assistant-0.1.7/rag_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 04:16:33.000000 rag_assistant-0.1.7/rag_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 04:16:33.000000 rag_assistant-0.1.7/rag_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 04:16:33.000000 rag_assistant-0.1.7/rag_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 04:16:33.000000 rag_assistant-0.1.7/rag_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 04:16:33.000000 rag_assistant-0.1.7/rag_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 04:16:33.794029 rag_assistant-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-17 04:16:23.000000 rag_assistant-0.1.7/setup.py
```

### Comparing `rag_assistant-0.1.6/PKG-INFO` & `rag_assistant-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag_assistant
-Version: 0.1.6
+Version: 0.1.7
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
-pip install rag_assistant==0.1.6 --user
+pip install rag_assistant==0.1.7 --user
 ```
 
 ## Execution
 ```bash
 ! rag_assistant --api_key "YOUR API KEY" --db_path "E:\swarmauri_github/prompt_responses.db" --system_context "You are a helpful assistant."
 ```
```

### Comparing `rag_assistant-0.1.6/rag_assistant/RagAssistant.py` & `rag_assistant-0.1.7/rag_assistant/RagAssistant.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     min-height: 80vh !important;
 }
 
 footer {
     display: none !important;
 }
 """
+        self.favicon_path = "./favicon-32x32.png"
         self.setup_gradio_interface()
         
     def initialize_agent(self):
         VS = Doc2VecVectorStore()
         agent = RagAgent(name="Rag", 
                          system_context=self.system_context, 
                          model=self.model, 
@@ -347,37 +348,38 @@
         with gr.Blocks(css = self.css, title="Swarmauri Rag Agent") as self.app:
             gr.TabbedInterface(interface_list=[self.chat, self.retrieval_table, self.document_table], 
                                       tab_names=["chat", "retrieval", "documents"])
 
     
     def launch(self, 
         share: bool = False, 
-        server_name: Optional[str] = None, 
-        favicon_path: Optional[str] = None):
+        server_name: Optional[str] = None
+        #favicon_path: Optional[str] = None
+        ):
 
         kwargs = {}
         kwargs.update({'share': share})
         if server_name:
             kwargs.update({'server_name': server_name})
-        if favicon_path:
-            kwargs.update({'favicon_path': favicon_path})
+
+        kwargs.update({'favicon_path': self.favicon_path})
 
         self.app.launch(**kwargs)
 
 
 def main():
     import argparse
     parser = argparse.ArgumentParser(description="Swarmauri Developer Assistant Command Line Tool")
     parser.add_argument('-api_key', '--api_key', type=str, help='Your api key', required=True)
     parser.add_argument('-provider_model', '--provider_model', type=str, help='Your provider model', required=False)
     parser.add_argument('-system_context', '--system_context', type=str, help='Assistants System Context', required=False)
     parser.add_argument('-db_path', '--db_path', type=str, help='path to sqlite3 db', required=False)
     parser.add_argument('-share', '--share', type=bool, help='Deploy a live app on gradio', required=False)
     parser.add_argument('-server_name', '--server_name', type=str, help='Server name', required=False)
-    parser.add_argument('-favicon_path', '--favicon_path', type=str, help='Path of applicaton favicon', required=False)
+    #parser.add_argument('-favicon_path', '--favicon_path', type=str, help='Path of application favicon', required=False)
     args = parser.parse_args()
 
 
     api_key = args.api_key
     
 
     # Create Assistant
@@ -398,18 +400,18 @@
 
     # If params then modify Assistant's config
     launch_kwargs = {}
     if args.share:
         launch_kwargs.update({'share': args.share})
     if args.server_name:
         launch_kwargs.update({'server_name': args.server_name})
-    if args.favicon_path:
-        launch_kwargs.update({'favicon_path': args.favicon_path})
-    else:
-        launch_kwargs.update({'favicon_path': "favicon-32x32.png"})
+    #if args.favicon_path:
+        #launch_kwargs.update({'favicon_path': args.favicon_path})
+    #else:
+        #launch_kwargs.update({'favicon_path': "favicon-32x32.png"})
 
 
     assistant.initialize_agent()
     assistant.launch(**launch_kwargs)
         
 if __name__ == "__main__":
     main()
```

### Comparing `rag_assistant-0.1.6/rag_assistant.egg-info/PKG-INFO` & `rag_assistant-0.1.7/rag_assistant.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag_assistant
-Version: 0.1.6
+Version: 0.1.7
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
-pip install rag_assistant==0.1.6 --user
+pip install rag_assistant==0.1.7 --user
 ```
 
 ## Execution
 ```bash
 ! rag_assistant --api_key "YOUR API KEY" --db_path "E:\swarmauri_github/prompt_responses.db" --system_context "You are a helpful assistant."
 ```
```

### Comparing `rag_assistant-0.1.6/setup.py` & `rag_assistant-0.1.7/setup.py`

 * *Files identical despite different names*

