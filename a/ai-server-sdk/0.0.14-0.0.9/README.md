# Comparing `tmp/ai-server-sdk-0.0.14.tar.gz` & `tmp/ai-server-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-server-sdk-0.0.14.tar", last modified: Thu Nov 30 19:46:25 2023, max compression
+gzip compressed data, was "ai-server-sdk-0.0.9.tar", last modified: Tue Oct 17 00:09:46 2023, max compression
```

## Comparing `ai-server-sdk-0.0.14.tar` & `ai-server-sdk-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-11-30 19:46:25.249596 ai-server-sdk-0.0.14/
--rw-rw-rw-   0        0        0     6194 2023-11-30 19:46:25.246596 ai-server-sdk-0.0.14/PKG-INFO
--rw-rw-rw-   0        0        0     5914 2023-11-14 16:34:58.000000 ai-server-sdk-0.0.14/README.md
-drwxrwxrwx   0        0        0        0 2023-11-30 19:46:25.184595 ai-server-sdk-0.0.14/ai_server/
--rw-rw-rw-   0        0        0      162 2023-11-27 17:03:58.000000 ai-server-sdk-0.0.14/ai_server/__init__.py
--rw-rw-rw-   0        0        0       37 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.14/ai_server/config.py
-drwxrwxrwx   0        0        0        0 2023-11-30 19:46:25.188594 ai-server-sdk-0.0.14/ai_server/py_client/
--rw-rw-rw-   0        0        0      143 2023-11-14 14:34:29.000000 ai-server-sdk-0.0.14/ai_server/py_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-30 19:46:25.212594 ai-server-sdk-0.0.14/ai_server/py_client/server_resources/
--rw-rw-rw-   0        0        0      253 2023-11-14 14:24:16.000000 ai-server-sdk-0.0.14/ai_server/py_client/server_resources/__init__.py
--rw-rw-rw-   0        0        0     4488 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.14/ai_server/py_client/server_resources/gaas_gpt_database.py
--rw-rw-rw-   0        0        0     1372 2023-09-22 21:59:46.000000 ai-server-sdk-0.0.14/ai_server/py_client/server_resources/gaas_gpt_driver.py
--rw-rw-rw-   0        0        0     3860 2023-11-13 22:50:15.000000 ai-server-sdk-0.0.14/ai_server/py_client/server_resources/gaas_gpt_model.py
--rw-rw-rw-   0        0        0     4966 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.14/ai_server/py_client/server_resources/gaas_gpt_storage.py
--rw-rw-rw-   0        0        0     4361 2023-11-14 14:59:23.000000 ai-server-sdk-0.0.14/ai_server/py_client/server_resources/gaas_gpt_vector.py
--rw-rw-rw-   0        0        0    12291 2023-11-30 19:45:56.000000 ai-server-sdk-0.0.14/ai_server/py_client/server_resources/gaas_rest_server.py
--rw-rw-rw-   0        0        0     6951 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.14/ai_server/py_client/server_resources/gaas_server_proxy.py
-drwxrwxrwx   0        0        0        0 2023-11-30 19:46:25.217595 ai-server-sdk-0.0.14/ai_server/py_client/server_resources/huggingface/
--rw-rw-rw-   0        0        0        0 2023-10-05 16:23:13.000000 ai-server-sdk-0.0.14/ai_server/py_client/server_resources/huggingface/__init__.py
--rw-rw-rw-   0        0        0      641 2023-10-06 15:51:53.000000 ai-server-sdk-0.0.14/ai_server/py_client/server_resources/huggingface/pretrain_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-11-30 19:46:25.227595 ai-server-sdk-0.0.14/ai_server/utils/
--rw-rw-rw-   0        0        0       72 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.14/ai_server/utils/__init__.py
--rw-rw-rw-   0        0        0       49 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.14/ai_server/utils/_constants_manager.py
--rw-rw-rw-   0        0        0      731 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.14/ai_server/utils/_stdout.py
-drwxrwxrwx   0        0        0        0 2023-11-30 19:46:25.243594 ai-server-sdk-0.0.14/ai_server_sdk.egg-info/
--rw-rw-rw-   0        0        0     6194 2023-11-30 19:46:25.000000 ai-server-sdk-0.0.14/ai_server_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      945 2023-11-30 19:46:25.000000 ai-server-sdk-0.0.14/ai_server_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-30 19:46:25.000000 ai-server-sdk-0.0.14/ai_server_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-11-30 19:46:25.000000 ai-server-sdk-0.0.14/ai_server_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-11-30 19:46:25.000000 ai-server-sdk-0.0.14/ai_server_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-30 19:46:25.250595 ai-server-sdk-0.0.14/setup.cfg
--rw-rw-rw-   0        0        0      623 2023-11-27 18:47:24.000000 ai-server-sdk-0.0.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-17 00:09:46.753161 ai-server-sdk-0.0.9/
+-rw-rw-rw-   0        0        0     5138 2023-10-17 00:09:46.751174 ai-server-sdk-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4909 2023-10-17 00:09:33.000000 ai-server-sdk-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-10-17 00:09:46.714097 ai-server-sdk-0.0.9/ai_server/
+-rw-rw-rw-   0        0        0      163 2023-10-05 16:26:33.000000 ai-server-sdk-0.0.9/ai_server/__init__.py
+-rw-rw-rw-   0        0        0       37 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/config.py
+drwxrwxrwx   0        0        0        0 2023-10-17 00:09:46.716087 ai-server-sdk-0.0.9/ai_server/py_client/
+-rw-rw-rw-   0        0        0      188 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/py_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-10-17 00:09:46.731095 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/
+-rw-rw-rw-   0        0        0      210 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/__init__.py
+-rw-rw-rw-   0        0        0     4488 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_gpt_database.py
+-rw-rw-rw-   0        0        0     1372 2023-09-22 21:59:46.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_gpt_driver.py
+-rw-rw-rw-   0        0        0     3965 2023-10-05 16:25:52.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_gpt_model.py
+-rw-rw-rw-   0        0        0     4966 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_gpt_storage.py
+-rw-rw-rw-   0        0        0     9820 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_rest_server.py
+-rw-rw-rw-   0        0        0     6951 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_server_proxy.py
+drwxrwxrwx   0        0        0        0 2023-10-17 00:09:46.735094 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/huggingface/
+-rw-rw-rw-   0        0        0        0 2023-10-05 16:23:13.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/huggingface/__init__.py
+-rw-rw-rw-   0        0        0      641 2023-10-06 15:51:53.000000 ai-server-sdk-0.0.9/ai_server/py_client/server_resources/huggingface/pretrain_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-10-17 00:09:46.740142 ai-server-sdk-0.0.9/ai_server/utils/
+-rw-rw-rw-   0        0        0       72 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/utils/__init__.py
+-rw-rw-rw-   0        0        0       49 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/utils/_constants_manager.py
+-rw-rw-rw-   0        0        0      731 2023-09-22 21:09:44.000000 ai-server-sdk-0.0.9/ai_server/utils/_stdout.py
+drwxrwxrwx   0        0        0        0 2023-10-17 00:09:46.749148 ai-server-sdk-0.0.9/ai_server_sdk.egg-info/
+-rw-rw-rw-   0        0        0     5138 2023-10-17 00:09:46.000000 ai-server-sdk-0.0.9/ai_server_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      889 2023-10-17 00:09:46.000000 ai-server-sdk-0.0.9/ai_server_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-17 00:09:46.000000 ai-server-sdk-0.0.9/ai_server_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-10-17 00:09:46.000000 ai-server-sdk-0.0.9/ai_server_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-10-17 00:09:46.000000 ai-server-sdk-0.0.9/ai_server_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-10-17 00:09:46.753161 ai-server-sdk-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-10-17 00:08:56.000000 ai-server-sdk-0.0.9/setup.py
```

### Comparing `ai-server-sdk-0.0.14/PKG-INFO` & `ai-server-sdk-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: ai-server-sdk
-Version: 0.0.14
+Version: 0.0.9
 Summary: Utility package to connect to AI Server instances.
 Author: Thomas Trankle
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
-Requires-Dist: pandas
-Requires-Dist: jsonpickle
 
 # **AI Server**
 
 *ai-server-sdk* is a python client SDK to connect to the AI Server
 
 ## Using this package you can:
 
@@ -37,64 +35,36 @@
 ```python
 >>> import ai_server
 
 # define access keys
 >>> loginKeys = {"secretKey":"<your_secret_key>","accessKey":"<your_access_key>"}
 
 # create connection object by passing in the secret key, access key and base url for the api
->>> server_connection = ai_server.RESTServer(
-...     access_key=loginKeys['accessKey'],
-...     secret_key=loginKeys['secretKey'],
-...     base='<Your deployed server Monolith URL>'
-... )
+>>> server_connection = ai_server.RESTServer(access_key=loginKeys['accessKey'], secret_key=loginKeys['secretKey'], base='<Your deployed server Monolith URL>')
 ```
 
 ### Inference with different Model Engines
 ```python
 # define a question and grab the engine id from the server
 >>> question = 'What is the capital of France?'
 >>> engine_id = "2c6de0ff-62e0-4dd0-8380-782ac4d40245"
 
-### Option 1 - Use ModelEngine directly
+### Option 1 - User ModelEngine directly
 >>> model = ai_server.ModelEngine(engine_id = engine_id, insight_id = server_connection.cur_insight)
 >>> model.ask(question = question)
 [{'response': 'The capital of France is Paris.',
   'messageId': '0a80c2ce-76f9-4466-b2a2-8455e4cab34a',
   'roomId': '28261853-0e41-49b0-8a50-df34e8c62a19'}]
 
 ### Option 2 - Use the Driver class
 >>> driver = ai_server.Driver(insight_id = server_connection.cur_insight)
 >>> driver.run_model(question = question, engine_id = engine_id)
 ['The capital of France is Paris.']
 ```
 
-### Interact with a Vector Database by adding document(s), querying, and removing document(s)
-```python
-# grab the engine id from the server
->>> engine_id = "221a50a4-060c-4aa8-8b7c-e2bc97ee3396"
-
-# initialize the connection to the vector database
->>> vectorEngine = ai_server.VectorEngine(
-...     engine_id = engine_id, 
-...     insight_id = server_connection.cur_insight
-... )
-
-# Add document(s) that have been uploaded to the insight
->>> vectorEngine.addDocument(file_paths = ['fileName1.pdf', 'fileName2.pdf', ..., 'fileNameX.pdf'])
-
-# Perform a nearest neighbor search on the embedded documents
->>> vectorEngine.nearestNeighbor(search_statement = 'Sample Search Statement', limit = 5)
-
-# List all the documents the vector database currently comprises of
->>> vectorEngine.listDocuments()
-
-# Remove document(s) from the vector database
->>> vectorEngine.removeDocument(file_names = ['fileName1.pdf', 'fileName2.pdf', ..., 'fileNameX.pdf'])
-```
-
 ### Connect to Databases and execute create, read, and delete operations
 
 #### Run the passed string query against the engine.  The query passed must be in the structure that the specific engine implementation.
 ```python
 # Create an relation to database based on the engine identifier
 >>> engine_id = "4a1f9466-4e6d-49cd-894d-7d22182344cd"
 >>> database = ai_server.DatabaseEngine(engine_id = engine_id, insight_id=a.cur_insight)
```

### Comparing `ai-server-sdk-0.0.14/README.md` & `ai-server-sdk-0.0.9/ai_server_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: ai-server-sdk
+Version: 0.0.9
+Summary: Utility package to connect to AI Server instances.
+Author: Thomas Trankle
+License: MIT
+Description-Content-Type: text/markdown
+Requires-Dist: requests
+
 # **AI Server**
 
 *ai-server-sdk* is a python client SDK to connect to the AI Server
 
 ## Using this package you can:
 
  - Inference with Models you have acces to within the server
@@ -26,64 +35,36 @@
 ```python
 >>> import ai_server
 
 # define access keys
 >>> loginKeys = {"secretKey":"<your_secret_key>","accessKey":"<your_access_key>"}
 
 # create connection object by passing in the secret key, access key and base url for the api
->>> server_connection = ai_server.RESTServer(
-...     access_key=loginKeys['accessKey'],
-...     secret_key=loginKeys['secretKey'],
-...     base='<Your deployed server Monolith URL>'
-... )
+>>> server_connection = ai_server.RESTServer(access_key=loginKeys['accessKey'], secret_key=loginKeys['secretKey'], base='<Your deployed server Monolith URL>')
 ```
 
 ### Inference with different Model Engines
 ```python
 # define a question and grab the engine id from the server
 >>> question = 'What is the capital of France?'
 >>> engine_id = "2c6de0ff-62e0-4dd0-8380-782ac4d40245"
 
-### Option 1 - Use ModelEngine directly
+### Option 1 - User ModelEngine directly
 >>> model = ai_server.ModelEngine(engine_id = engine_id, insight_id = server_connection.cur_insight)
 >>> model.ask(question = question)
 [{'response': 'The capital of France is Paris.',
   'messageId': '0a80c2ce-76f9-4466-b2a2-8455e4cab34a',
   'roomId': '28261853-0e41-49b0-8a50-df34e8c62a19'}]
 
 ### Option 2 - Use the Driver class
 >>> driver = ai_server.Driver(insight_id = server_connection.cur_insight)
 >>> driver.run_model(question = question, engine_id = engine_id)
 ['The capital of France is Paris.']
 ```
 
-### Interact with a Vector Database by adding document(s), querying, and removing document(s)
-```python
-# grab the engine id from the server
->>> engine_id = "221a50a4-060c-4aa8-8b7c-e2bc97ee3396"
-
-# initialize the connection to the vector database
->>> vectorEngine = ai_server.VectorEngine(
-...     engine_id = engine_id, 
-...     insight_id = server_connection.cur_insight
-... )
-
-# Add document(s) that have been uploaded to the insight
->>> vectorEngine.addDocument(file_paths = ['fileName1.pdf', 'fileName2.pdf', ..., 'fileNameX.pdf'])
-
-# Perform a nearest neighbor search on the embedded documents
->>> vectorEngine.nearestNeighbor(search_statement = 'Sample Search Statement', limit = 5)
-
-# List all the documents the vector database currently comprises of
->>> vectorEngine.listDocuments()
-
-# Remove document(s) from the vector database
->>> vectorEngine.removeDocument(file_names = ['fileName1.pdf', 'fileName2.pdf', ..., 'fileNameX.pdf'])
-```
-
 ### Connect to Databases and execute create, read, and delete operations
 
 #### Run the passed string query against the engine.  The query passed must be in the structure that the specific engine implementation.
 ```python
 # Create an relation to database based on the engine identifier
 >>> engine_id = "4a1f9466-4e6d-49cd-894d-7d22182344cd"
 >>> database = ai_server.DatabaseEngine(engine_id = engine_id, insight_id=a.cur_insight)
@@ -157,8 +138,8 @@
  'pixelReturn': [{'pixelId': '3',
    'pixelExpression': '1 + 1 ;',
    'isMeta': False,
    'output': 2,
    'operationType': ['OPERATION']}]}
 ```
 
----
+---
```

### Comparing `ai-server-sdk-0.0.14/ai_server/py_client/server_resources/gaas_gpt_database.py` & `ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_gpt_database.py`

 * *Files identical despite different names*

### Comparing `ai-server-sdk-0.0.14/ai_server/py_client/server_resources/gaas_gpt_driver.py` & `ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_gpt_driver.py`

 * *Files identical despite different names*

### Comparing `ai-server-sdk-0.0.14/ai_server/py_client/server_resources/gaas_gpt_model.py` & `ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_gpt_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,21 +7,50 @@
   def __init__(self, engine_id=None, insight_id=None):
     assert engine_id is not None 
     super().__init__()
     self.engine_id = engine_id
     self.insight_id = insight_id
     print_output("initialized")
     
-  def ask(
-        self, 
-        question:str = None, 
-        context:str = None, 
-        insight_id:str = None, 
-        param_dict: dict = None
-    ) -> list:
+  def embeddings(self, strings_to_encode = None, insight_id=None, param_dict=None):
+    '''
+    If I model has embeddings enabled, pass in a string to get the embedded response
+
+    Args:
+        question (`str`):
+            A user's access key is a unique identifier used for authentication and authorization. It will allow users or applications to access specific resources or perform designated actions within an ai-server instance.
+        insight_id (`str`):
+            Unique identifier for the temporal worksapce where actions are being isolated
+        param_dict (`dict`):
+            Optional
+    '''
+    assert strings_to_encode is not None
+    if isinstance(strings_to_encode,str):
+      strings_to_encode = [strings_to_encode]
+    assert isinstance(strings_to_encode, list)
+    if insight_id is None:
+      insight_id = self.insight_id
+    assert insight_id is not None
+    epoc = super().get_next_epoc()
+    return super().call(
+                      epoc = epoc, 
+                      engine_type='Model', 
+                      engine_id=self.engine_id, 
+                      insight_id=insight_id, 
+                      method_name='embeddings', 
+                      method_args=[strings_to_encode, insight_id, param_dict],
+                      method_arg_types=['java.util.List', 'prerna.om.Insight', 'java.util.Map']
+                      )
+    
+  def ask(self, 
+          question:str = None, 
+          context:str = None, 
+          insight_id:str = None, 
+          param_dict: dict = None
+          ) -> list:
     '''
     Connect to a database an execute SQL against it to create a pandas frame
 
     Args:
         question (`str`):
             The single string question you are asking a an LLM
         context (`str`):
@@ -43,59 +72,23 @@
     assert question is not None
     if insight_id is None:
       insight_id = self.insight_id
     # should I assert for insight_id as well I think I should
     assert insight_id is not None    
     epoc = super().get_next_epoc()
     return super().call(
-        epoc=epoc, 
-        engine_type='Model', 
-        engine_id=self.engine_id, 
-        method_name='ask', 
-        method_args=[question,context,insight_id, param_dict],
-        method_arg_types=['java.lang.String', 'java.lang.String', 'prerna.om.Insight', 'java.util.Map'],
-        insight_id = insight_id
-    )
+                        epoc=epoc, 
+                        engine_type='Model', 
+                        engine_id=self.engine_id, 
+                        method_name='ask', 
+                        method_args=[question,context,insight_id, param_dict],
+                        method_arg_types=['java.lang.String', 'java.lang.String', 'prerna.om.Insight', 'java.util.Map'],
+                        insight_id = insight_id
+                        )
   
-  def embeddings(self, strings_to_embed = None, insight_id=None, param_dict=None):
-    '''
-    If I model has embeddings enabled, pass in a string to get the embedded response
+  def as_pretrained_model(self):
+    from .huggingface.pretrain_wrapper import HuggingFaceConfig, HuggingFacePretrainedModel
+    return HuggingFacePretrainedModel(config = HuggingFaceConfig(), model_engine = self)
 
-    Args:
-        question (`str`):
-            A user's access key is a unique identifier used for authentication and authorization. It will allow users or applications to access specific resources or perform designated actions within an ai-server instance.
-        insight_id (`str`):
-            Unique identifier for the temporal worksapce where actions are being isolated
-        param_dict (`dict`):
-            Optional
-    '''
-    assert strings_to_embed is not None
-    if isinstance(strings_to_embed,str):
-      strings_to_embed = [strings_to_embed]
-    assert isinstance(strings_to_embed, list)
-    if insight_id is None:
-      insight_id = self.insight_id
-    assert insight_id is not None
-    epoc = super().get_next_epoc()
-    return super().call(
-        epoc = epoc, 
-        engine_type='Model', 
-        engine_id=self.engine_id, 
-        insight_id=insight_id, 
-        method_name='embeddings', 
-        method_args=[strings_to_embed, insight_id, param_dict],
-        method_arg_types=['java.util.List', 'prerna.om.Insight', 'java.util.Map']
-    )
-
-  def get_model_type(self, insight_id:str = None):
-    if insight_id is None:
-      insight_id = self.insight_id
-    epoc = super().get_next_epoc()
-    return super().call(
-        epoc = epoc, 
-        engine_type='Model', 
-        engine_id=self.engine_id, 
-        insight_id=insight_id, 
-        method_name='getModelType', 
-        method_args=[],
-        method_arg_types=[]
-    )
+    
+    
+
```

### Comparing `ai-server-sdk-0.0.14/ai_server/py_client/server_resources/gaas_gpt_storage.py` & `ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_gpt_storage.py`

 * *Files identical despite different names*

### Comparing `ai-server-sdk-0.0.14/ai_server/py_client/server_resources/gaas_rest_server.py` & `ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_rest_server.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,254 +1,240 @@
 import requests
 import json
-from typing import Any, List, Dict, Optional
+from typing import Any
 from ...utils._stdout import print_output
 import pandas as pd
-import base64
 
 class RESTServer():
-    """RESTServer to make calls to a ai server instance
+  """RESTServer to make calls to a ai server instance
 
-    Example:
+  Example:
 
-    ```python
-    >>> import ai_server
+  ```python
+  >>> import ai_server
 
-    # define access keys
-    >>> loginKeys = {"secretKey":"<your_secret_key>","accessKey":"<your_access_key>"}
+  # define access keys
+  >>> loginKeys = {"secretKey":"<your_secret_key>","accessKey":"<your_access_key>"}
 
-    # create connection object by passing in the secret key, access key and base url for the api
-    >>> server_connection = ai_server.RESTServer(access_key=loginKeys['accessKey'], secret_key=loginKeys['secretKey'], base='<Your deployed server Monolith URL>')
-    ```
-    """
-    # register the server for proxy call
-    da_server = None
+  # create connection object by passing in the secret key, access key and base url for the api
+  >>> server_connection = ai_server.RESTServer(access_key=loginKeys['accessKey'], secret_key=loginKeys['secretKey'], base='<Your deployed server Monolith URL>')
+  ```
+  """
+  # register the server for proxy call
+  da_server = None
 
-    def __init__(self, access_key:str = None, secret_key:str = None, base:str = None):
-        """
-        Args:
-            access_key (`str`):
-                A user's access key is a unique identifier used for authentication and authorization. It will allow users or applications to access specific resources or perform designated actions within an ai-server instance.
-            secret_key (`str`):
-                A user's confidential and securely stored piece of information that complements an access key, used in cryptographic processes to validate identity and ensure secure communication
-            base (`str`):
-                main url to access the server api
-        """
-        self.access_key = access_key
-        self.secret_key = secret_key
-        self.main_url = base
-        if self.main_url.endswith('\/'):
-            self.main_url = self.main_url[:-1]
-        self.auth_headers = {}
-        self.login()
-        self.connected = True
-        self.open_insights = set()
-        self.cur_insight = self.make_new_insight() # automatically create an insight for the user
-        RESTServer.da_server = self
-        self.monitors = {}
-    
-    def login(self):
-        """
-        register / validate the users secret & access key combination. 
-        
-        Store the cookies to be used for other api calls after authentication
-        """
-        combined = self.access_key + ":" + self.secret_key
-        combined_enc = base64.b64encode(combined.encode('ascii'))
-        headers = {'Authorization': f"Basic {combined_enc.decode('ascii')}"}
-        self.auth_headers = headers.copy()
-        print_output(self.auth_headers)
-        headers.update({'disableRedirect':'true'})
-        #login url
-        api_url = "/auth/whoami"
-        url = self.main_url + api_url
-
-        self.r = requests.get(url, headers=headers)
-        self.r.raise_for_status()
-
-        # display the login response
-        print_output(self.r.json())
-        self.cookies = self.r.cookies
-        # display the cookies
-        print_output(self.cookies)
-        
-    def get_auth_headers(self):
-        return self.auth_headers
+  def __init__(self, access_key:str = None, secret_key:str = None, base:str = None):
+    """
+    Args:
+        access_key (`str`):
+            A user's access key is a unique identifier used for authentication and authorization. It will allow users or applications to access specific resources or perform designated actions within an ai-server instance.
+        secret_key (`str`):
+            A user's confidential and securely stored piece of information that complements an access key, used in cryptographic processes to validate identity and ensure secure communication
+        base (`str`):
+            main url to access the server api
+    """
+    self.access_key = access_key
+    self.secret_key = secret_key
+    self.main_url = base
+    self.login()
+    self.connected = True
+    self.open_insights = set()
+    self.cur_insight = self.make_new_insight() # automatically create an insight for the user
+    RESTServer.da_server = self
+    self.monitors = {}
     
-    def get_openai_endpoint(self):
-        return self.main_url + "/model/openai"
-
-    def make_new_insight(self) -> str:
-        """
-        create a new temporal space to operate within the ai-server. An insight is directoly associated with a user
-        """
-        if not self.connected:
-            return "Please login"
+  def login(self):
+    """
+    register / validate the users secret & access key combination. 
     
-        pixel_payload = {}
-        pixel_payload.update({'expression':'META | true', 'insightId':'new'})
-        api_url = "/engine/runPixel"
-        response = requests.post(self.main_url + api_url, cookies = self.cookies, data=pixel_payload)
-
-        # raise HTTP error if one occurs
-        response.raise_for_status()
-
-        json_output = response.json()
-        # display the pixel response
-        print_output(json_output)
+    Store the cookies to be used for other api calls after authentication
+    """
+    import base64
+    combined = self.access_key + ":" + self.secret_key
+    combined_enc = base64.b64encode(combined.encode('ascii'))
+    headers = {'authorization': f"Basic {combined_enc.decode('ascii')}"}
+    headers.update({'disableRedirect':'true'})
+    #login url
+    api_url = "/auth/whoami"
+    url = self.main_url + api_url
+
+    self.r = requests.get(url, headers=headers)
+    self.r.raise_for_status()
+
+    # display the login response
+    print_output(self.r.json())
+    self.cookies = self.r.cookies
+    # display the cookies
+    print_output(self.cookies)
     
-        self.cur_insight = json_output['insightID']
-        self.open_insights.add(self.cur_insight)
-
-        print_output(f"Current open insights are -- {self.open_insights}")
-
-        return self.cur_insight
   
-    def run_pixel(
-        self, 
-        payload:str = None, 
-        insight_id:str | None = None, 
-        full_response:bool = False
-    ):
-        '''
-        /api/engine/runPixel is the AI server's primary endpoint that consumes a flexible payload. The payload must contain two parameters, namely:
-        1.) expression - The @payload passed is placed here and must comply and be defined in the Server's DSL (Pixel) which dictates what action should be taken
-        2.) insightId - the temporal workspace identifier which isoloates the actions being performed
-
-        Args:
-        payload (`str`):
-            DSL (Pixel) instruction on what specific action should be performed 
-        insight_id (`str`):
-            Unique identifier for the temporal worksapce where actions are being isolated
-
-            insight_id Options are:
-
-                - insight_id = '' -> Creates a temporary one time insight created but is not stored /     cannot be referenced for future state
-                - insight_id = 'new' -> Creates a new insight which can be referenced in the same sesssion
-                - insight_id = '<uuid/guid string>' -> Uses an existing insight id that exists in the user session
-
-        full_response (`bool`):
-            Indicate whether to return the full json response or only the actions output
-        '''
-        # going to create an insight if insight not available
-        if not self.connected:
-            return "Please login"
+  def make_new_insight(self) -> str:
+    """
+    create a new temporal space to operate within the ai-server. An insight is directoly associated with a user
+    """
+    if not self.connected:
+      return "Please login"
     
-        if insight_id is None:
-            insight_id = self.cur_insight
-            # still null :(
-            if insight_id is None:
-                print_output("insight_id and self.cur_insight are both undefined. Creating new insight")
-                self.cur_insight = self.make_new_insight()
-                insight_id = self.cur_insight
-
-        print_output(f"Current insight_id is set to {insight_id}")
-
-        pixel_payload = {}
-        pixel_payload.update({'expression':payload})
-        pixel_payload.update({'insightId':insight_id})
-
-        api_url = "/engine/runPixel";
-        response = requests.post(self.main_url + api_url, cookies = self.cookies, data=pixel_payload)
-        if full_response:
-            return response.json()
-        else:
-            return self.get_pixel_output(response.json())
+    pixel_payload = {}
+    pixel_payload.update({'expression':'META | true', 'insightId':'new'})
+    api_url = "/engine/runPixel"
+    response = requests.post(self.main_url + api_url, cookies = self.cookies, data=pixel_payload)
+
+    # raise HTTP error if one occurs
+    response.raise_for_status()
+
+    json_output = response.json()
+    # display the pixel response
+    print_output(json_output)
     
-    def get_pixel_output(self, payload:dict = None) -> Any | list:
-        '''
-        Utility method to grab the output of runPixel call
-        '''
-        print_output(payload)
-        main_output = payload['pixelReturn'][0]['output']
-        if isinstance(main_output, list):
-            output = main_output[0]
-        else:
-            output = main_output
-        return output
-        
-    def logout(self):
-        '''Close the connection'''
-        # define the logout endpoint
-        api_url = "/logout/all"
-
-        # make the request
-        requests.get(self.main_url + api_url, cookies = self.cookies)
-
-        # reset the connection attributes for the class
-        self.cookies = None
-        self.connected = False
+    self.cur_insight = json_output['insightID']
+    self.open_insights.add(self.cur_insight)
 
-    def send_request(self, input_payload:dict) -> None:
-        '''
-        Constructs the payload for various server resources such as ModelEngine, StorageEngine and DatabaseEngine when the server is an instance of RESTServer
+    print_output(f"Current open insights are -- {self.open_insights}")
 
-        Args:
-        input_payload (`dict`):
-            the actual payload being sent to the AI Server
-        '''
-        
-        # this is a synchronous call
-        # but I dont want to bother the server proxy and leave it as is
-        epoc = input_payload['epoc']
-
-        input_payload_message = json.dumps(input_payload)
-        print_output(input_payload_message)
-
-        # escape the quotes
-        #input_payload_message = json.dumps(input_payload_message)
-        # RemoteEngineRun is responsible for handling ModelEngine, StorageEngine and DatabaseEngine via RESTServer
-        func = "RemoteEngineRun(payload=\"<e>" + input_payload_message + "</e>\");"
-        output_payload_message = self.run_pixel(payload=func, insight_id=input_payload['insightId'])
-        if epoc in self.monitors:
-            condition = self.monitors[epoc]
-            self.monitors.update({epoc: output_payload_message})
+    return self.cur_insight
   
-    def get_open_insights(self) -> list:
-        '''
-        Utility method to get a list of insight IDs the user has created after the connection was made
-        '''
-        # MyOpenInsights is pre0defined server level reactor to handle the action of getting the insightIds
-        open_insights = self.run_pixel(payload = 'MyOpenInsights();')
+  def run_pixel(self, 
+                payload:str = None, 
+                insight_id:str | None = None, 
+                full_response:bool = False):
+    '''
+    /api/engine/runPixel is the AI server's primary endpoint that consumes a flexible payload. The payload must contain two parameters, namely:
+      1.) expression - The @payload passed is placed here and must comply and be defined in the Server's DSL (Pixel) which dictates what action should be taken
+      2.) insightId - the temporal workspace identifier which isoloates the actions being performed
+
+    Args:
+      payload (`str`):
+          DSL (Pixel) instruction on what specific action should be performed 
+      insight_id (`str`):
+          Unique identifier for the temporal worksapce where actions are being isolated
+
+          insight_id Options are:
+
+            - insight_id = '' -> Creates a temporary one time insight created but is not stored /     cannot be referenced for future state
+            - insight_id = 'new' -> Creates a new insight which can be referenced in the same sesssion
+            - insight_id = '<uuid/guid string>' -> Uses an existing insight id that exists in the user session
+
+      full_response (`bool`):
+          Indicate whether to return the full json response or only the actions output
+    '''
+    # going to create an insight if insight not available
+    if not self.connected:
+      return "Please login"
     
-        # keep track of the open insights within the python object itself
-        self.open_insights = set(open_insights)
-
-        # return a list of insight ids
-        return open_insights
+    if insight_id is None:
+      insight_id = self.cur_insight
+       # still null :(
+      if insight_id is None:
+        print_output("insight_id and self.cur_insight are both undefined. Creating new insight")
+        self.cur_insight = self.make_new_insight()
+        insight_id = self.cur_insight
+
+    print_output(f"Current insight_id is set to {insight_id}")
+
+    pixel_payload = {}
+    pixel_payload.update({'expression':payload})
+    pixel_payload.update({'insightId':insight_id})
+
+    api_url = "/engine/runPixel";
+    response = requests.post(self.main_url + api_url, cookies = self.cookies, data=pixel_payload)
+    if full_response:
+      return response.json()
+    else:
+      return self.get_pixel_output(response.json())
     
-    def drop_insights(self, insight_ids: str | list) -> None:
-        '''
-        Utility method close given insight(s)
-
-        Args:
-        insight_ids (`str` | `list`):
-            a single insight or a list of insights the user wishes to close
+  def get_pixel_output(self, payload:dict = None) -> Any | list:
+    '''
+    Utility method to grab the output of runPixel call
+    '''
+    print_output(payload)
+    main_output = payload['pixelReturn'][0]['output']
+    if isinstance(main_output, list):
+      output = main_output[0]
+    else:
+      output = main_output
+    return output
+    
+  def logout(self):
+    '''Close the connection'''
+    # define the logout endpoint
+    api_url = "/logout/all"
+
+    # make the request
+    requests.get(self.main_url + api_url, cookies = self.cookies)
+
+    # reset the connection attributes for the class
+    self.cookies = None
+    self.connected = False
+
+  def send_request(self, input_payload:dict) -> None:
+    '''
+    Constructs the payload for various server resources such as ModelEngine, StorageEngine and DatabaseEngine when the server is an instance of RESTServer
+
+    Args:
+      input_payload (`dict`):
+          the actual payload being sent to the AI Server
+    '''
+    
+    # this is a synchronous call
+    # but I dont want to bother the server proxy and leave it as is
+    epoc = input_payload['epoc']
+
+    input_payload_message = json.dumps(input_payload)
+    print_output(input_payload_message)
+
+    # escape the quotes
+    #input_payload_message = json.dumps(input_payload_message)
+    # RemoteEngineRun is responsible for handling ModelEngine, StorageEngine and DatabaseEngine via RESTServer
+    func = "RemoteEngineRun(payload=\"<e>" + input_payload_message + "</e>\");"
+    output_payload_message = self.run_pixel(payload=func, insight_id=input_payload['insightId'])
+    if epoc in self.monitors:
+      condition = self.monitors[epoc]
+      self.monitors.update({epoc: output_payload_message})
+  
+  def get_open_insights(self) -> list:
+    '''
+    Utility method to get a list of insight IDs the user has created after the connection was made
+    '''
+    # MyOpenInsights is pre0defined server level reactor to handle the action of getting the insightIds
+    open_insights = self.run_pixel(payload = 'MyOpenInsights();')
+    
+    # keep track of the open insights within the python object itself
+    self.open_insights = set(open_insights)
 
-        By Default, the current / working insight is set to the first insight in open_insights
-        '''
-        if isinstance(insight_ids,list):
-            for id in insight_ids:
-                self.run_pixel(insight_id = id,payload = 'DropInsight();')
-                self.open_insights.discard(id)
-        else:
-            self.run_pixel(insight_id = insight_ids,payload = 'DropInsight();')
-            self.open_insights.discard(insight_ids)
-
-        if (len(self.open_insights) > 0):
-            self.cur_insight = self.open_insights[0]
-        else:
-            self.cur_insight = None
-
-    def import_data_product(
-        self, 
-        project_id:str = None, 
-        insight_id:str = None, 
-        sql:str = None
-    ) -> pd.DataFrame | None:
+    # return a list of insight ids
+    return open_insights
+  
+  def drop_insights(self, insight_ids: str | list) -> None:
+    '''
+    Utility method close given insight(s)
+
+    Args:
+      insight_ids (`str` | `list`):
+          a single insight or a list of insights the user wishes to close
+
+    By Default, the current / working insight is set to the first insight in open_insights
+    '''
+    if isinstance(insight_ids,list):
+      for id in insight_ids:
+         self.run_pixel(insight_id = id,payload = 'DropInsight();')
+         self.open_insights.discard(id)
+    else:
+      self.run_pixel(insight_id = insight_ids,payload = 'DropInsight();')
+      self.open_insights.discard(insight_ids)
+
+    if (len(self.open_insights) > 0):
+       self.cur_insight = self.open_insights[0]
+    else:
+       self.cur_insight = None
+
+  def import_data_product(self, 
+                          project_id:str = None, 
+                          insight_id:str = None, 
+                          sql:str = None) -> pd.DataFrame | None:
         '''
         If an insight is saved, the data within it becomes a data product and is accessible via a REST API
 
         Args:
         project_id (`str`):
             Given project/app unique identifier 
         insight_id (`str`):
@@ -274,52 +260,8 @@
       
         try:
             return pd.DataFrame(response['dataArray'], columns=response['columns'])
         except:
             try:
                 return pd.DataFrame(response['data'], columns=response['columns'])
             except:
-                return None
-            
-    def upload_files(
-        self, 
-        files:List[str], 
-        insight_id:str = None, 
-        project_id:str = None, 
-        path:str = None
-    ) -> List[str]:
-        # .../Monolith/api/uploadFile/baseUpload?insightId=de43ce0d-db2e-4ab9-a807-336bb86c4ea0&projectId=4c14bc58-973f-4293-87ed-a5d32c24f418&path=version/assets/
-        if isinstance(files,str):
-            files = [files]
-            
-        param = ''
-        path = path or ''
-        
-        if insight_id or project_id or path:
-            if insight_id == None:
-                insight_id = self.cur_insight
-            param += f'insightId={insight_id}'
-            
-            if project_id:
-                if param:
-                    param += '&'
-                param += f'projectId={project_id}'
-            
-            if path:
-                if param:
-                    param += '&'
-                param += f'path={path}'
-            param = f'?{param}'
-        
-        url = f'{self.main_url}/uploadFile/baseUpload{param}'
-        
-        insight_file_paths = []
-        for filepath in files:
-            with open(filepath, 'rb') as fobj:
-                response = requests.post(
-                    url, 
-                    cookies = self.cookies,
-                    files={'file': fobj}
-                )
-                insight_file_paths.append(response.json()[0]['fileName'])
-                
-        return insight_file_paths
+                return None
```

### Comparing `ai-server-sdk-0.0.14/ai_server/py_client/server_resources/gaas_server_proxy.py` & `ai-server-sdk-0.0.9/ai_server/py_client/server_resources/gaas_server_proxy.py`

 * *Files identical despite different names*

### Comparing `ai-server-sdk-0.0.14/ai_server/py_client/server_resources/huggingface/pretrain_wrapper.py` & `ai-server-sdk-0.0.9/ai_server/py_client/server_resources/huggingface/pretrain_wrapper.py`

 * *Files identical despite different names*

### Comparing `ai-server-sdk-0.0.14/ai_server/utils/_stdout.py` & `ai-server-sdk-0.0.9/ai_server/utils/_stdout.py`

 * *Files identical despite different names*

### Comparing `ai-server-sdk-0.0.14/ai_server_sdk.egg-info/SOURCES.txt` & `ai-server-sdk-0.0.9/ai_server_sdk.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 ai_server/config.py
 ai_server/py_client/__init__.py
 ai_server/py_client/server_resources/__init__.py
 ai_server/py_client/server_resources/gaas_gpt_database.py
 ai_server/py_client/server_resources/gaas_gpt_driver.py
 ai_server/py_client/server_resources/gaas_gpt_model.py
 ai_server/py_client/server_resources/gaas_gpt_storage.py
-ai_server/py_client/server_resources/gaas_gpt_vector.py
 ai_server/py_client/server_resources/gaas_rest_server.py
 ai_server/py_client/server_resources/gaas_server_proxy.py
 ai_server/py_client/server_resources/huggingface/__init__.py
 ai_server/py_client/server_resources/huggingface/pretrain_wrapper.py
 ai_server/utils/__init__.py
 ai_server/utils/_constants_manager.py
 ai_server/utils/_stdout.py
```

### Comparing `ai-server-sdk-0.0.14/setup.py` & `ai-server-sdk-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from setuptools import find_packages, setup
 
-with open('README.md','r') as f:
-    long_description = f.read()
-    
+with open('README.md','r') as fh:
+    long_description = fh.read()
+
 setup(
     name="ai-server-sdk",                     # This is the name of the package
-    version="0.0.14",
+    version="0.0.9",
     packages=find_packages(),
-    install_requires=[
-        'requests', 
-        'pandas', 
-        'jsonpickle'
-    ], 
+    install_requires=['requests',], 
     author="Thomas Trankle",                     # Full name of the author
     description="Utility package to connect to AI Server instances.",
     license="MIT",
     long_description = long_description,
     long_description_content_type = 'text/markdown'
 )
```

