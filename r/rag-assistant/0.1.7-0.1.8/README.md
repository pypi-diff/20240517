# Comparing `tmp/rag_assistant-0.1.7.tar.gz` & `tmp/rag_assistant-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_assistant-0.1.7.tar", last modified: Fri May 17 04:16:33 2024, max compression
+gzip compressed data, was "rag_assistant-0.1.8.tar", last modified: Fri May 17 04:20:58 2024, max compression
```

## Comparing `rag_assistant-0.1.7.tar` & `rag_assistant-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:33.794029 rag_assistant-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 04:16:33.794029 rag_assistant-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-17 04:16:23.000000 rag_assistant-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:33.794029 rag_assistant-0.1.7/rag_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)    18864 2024-05-17 04:16:23.000000 rag_assistant-0.1.7/rag_assistant/RagAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-17 04:16:23.000000 rag_assistant-0.1.7/rag_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:16:33.794029 rag_assistant-0.1.7/rag_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 04:16:33.000000 rag_assistant-0.1.7/rag_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 04:16:33.000000 rag_assistant-0.1.7/rag_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 04:16:33.000000 rag_assistant-0.1.7/rag_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 04:16:33.000000 rag_assistant-0.1.7/rag_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 04:16:33.000000 rag_assistant-0.1.7/rag_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 04:16:33.000000 rag_assistant-0.1.7/rag_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 04:16:33.794029 rag_assistant-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-17 04:16:23.000000 rag_assistant-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:58.001101 rag_assistant-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 04:20:58.001101 rag_assistant-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-17 04:20:45.000000 rag_assistant-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:58.001101 rag_assistant-0.1.8/rag_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)    18841 2024-05-17 04:20:45.000000 rag_assistant-0.1.8/rag_assistant/RagAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-17 04:20:45.000000 rag_assistant-0.1.8/rag_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:20:58.001101 rag_assistant-0.1.8/rag_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-17 04:20:57.000000 rag_assistant-0.1.8/rag_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 04:20:57.000000 rag_assistant-0.1.8/rag_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 04:20:57.000000 rag_assistant-0.1.8/rag_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 04:20:57.000000 rag_assistant-0.1.8/rag_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 04:20:57.000000 rag_assistant-0.1.8/rag_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 04:20:57.000000 rag_assistant-0.1.8/rag_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 04:20:58.001101 rag_assistant-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-17 04:20:45.000000 rag_assistant-0.1.8/setup.py
```

### Comparing `rag_assistant-0.1.7/PKG-INFO` & `rag_assistant-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag_assistant
-Version: 0.1.7
+Version: 0.1.8
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
-pip install rag_assistant==0.1.7 --user
+pip install rag_assistant==0.1.8 --user
 ```
 
 ## Execution
 ```bash
 ! rag_assistant --api_key "YOUR API KEY" --db_path "E:\swarmauri_github/prompt_responses.db" --system_context "You are a helpful assistant."
 ```
```

### Comparing `rag_assistant-0.1.7/rag_assistant/RagAssistant.py` & `rag_assistant-0.1.8/rag_assistant/RagAssistant.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 }
 
 footer {
     display: none !important;
 }
 """
         self.favicon_path = "./favicon-32x32.png"
-        self.setup_gradio_interface()
+        
         
     def initialize_agent(self):
         VS = Doc2VecVectorStore()
         agent = RagAgent(name="Rag", 
                          system_context=self.system_context, 
                          model=self.model, 
                          conversation=self.conversation, 
@@ -300,15 +300,15 @@
             with gr.Accordion("See Details", open=False):
                 self.additional_inputs = [
                     gr.Textbox(label="API Key", value=self.api_key or "Enter your API Key"),
                     gr.Dropdown(self.allowed_models, 
                                 value="openai_gpt-3.5-turbo", 
                                 label="Model",
                                 info="Select openai model"),
-                    gr.Textbox(label="System Context", value=self.system_context or "You are a helpful assistant"),
+                    gr.Textbox(label="System Context", value = self.system_context),
                     gr.Checkbox(label="Fixed Retrieval", value=True, interactive=True),
                     gr.Slider(label="Top K", value=10, minimum=0, maximum=100, step=5, interactive=True),
                     gr.Slider(label="Temperature", value=1, minimum=0.0, maximum=1, step=0.01, interactive=True),
                     gr.Slider(label="Max new tokens", value=256, minimum=256, maximum=4096, step=64, interactive=True),
                     gr.Slider(label="Conversation size", value=12, minimum=2, maximum=36, step=2, interactive=True),
                     gr.Slider(label="Session Cache size", value=12, minimum=2, maximum=36, step=2, interactive=True)
                 ]
@@ -358,15 +358,15 @@
 
         kwargs = {}
         kwargs.update({'share': share})
         if server_name:
             kwargs.update({'server_name': server_name})
 
         kwargs.update({'favicon_path': self.favicon_path})
-
+        self.setup_gradio_interface()
         self.app.launch(**kwargs)
 
 
 def main():
     import argparse
     parser = argparse.ArgumentParser(description="Swarmauri Developer Assistant Command Line Tool")
     parser.add_argument('-api_key', '--api_key', type=str, help='Your api key', required=True)
```

### Comparing `rag_assistant-0.1.7/rag_assistant.egg-info/PKG-INFO` & `rag_assistant-0.1.8/rag_assistant.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag_assistant
-Version: 0.1.7
+Version: 0.1.8
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
-pip install rag_assistant==0.1.7 --user
+pip install rag_assistant==0.1.8 --user
 ```
 
 ## Execution
 ```bash
 ! rag_assistant --api_key "YOUR API KEY" --db_path "E:\swarmauri_github/prompt_responses.db" --system_context "You are a helpful assistant."
 ```
```

### Comparing `rag_assistant-0.1.7/setup.py` & `rag_assistant-0.1.8/setup.py`

 * *Files identical despite different names*

