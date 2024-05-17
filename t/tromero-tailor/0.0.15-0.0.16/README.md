# Comparing `tmp/tromero_tailor-0.0.15.tar.gz` & `tmp/tromero_tailor-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tromero_tailor-0.0.15.tar", last modified: Tue May 14 11:37:29 2024, max compression
+gzip compressed data, was "tromero_tailor-0.0.16.tar", last modified: Fri May 17 14:21:25 2024, max compression
```

## Comparing `tromero_tailor-0.0.15.tar` & `tromero_tailor-0.0.16.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-14 11:37:29.047756 tromero_tailor-0.0.15/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-14 11:37:29.047486 tromero_tailor-0.0.15/PKG-INFO
--rw-r--r--   0 tadhgamin   (501) staff       (20)      942 2024-04-08 16:49:32.000000 tromero_tailor-0.0.15/README.md
--rw-r--r--   0 tadhgamin   (501) staff       (20)       38 2024-05-14 11:37:29.047814 tromero_tailor-0.0.15/setup.cfg
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1633 2024-05-14 11:37:26.000000 tromero_tailor-0.0.15/setup.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-14 11:37:29.045693 tromero_tailor-0.0.15/tests/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     3672 2024-04-17 14:55:07.000000 tromero_tailor-0.0.15/tests/test.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-14 11:37:29.046351 tromero_tailor-0.0.15/tromero_tailor/
--rw-r--r--   0 tadhgamin   (501) staff       (20)       30 2024-04-08 15:07:54.000000 tromero_tailor-0.0.15/tromero_tailor/__init__.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1582 2024-05-14 11:36:40.000000 tromero_tailor-0.0.15/tromero_tailor/tromero_requests.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)      446 2024-04-12 11:06:15.000000 tromero_tailor-0.0.15/tromero_tailor/tromero_utils.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)     2942 2024-05-13 13:42:50.000000 tromero_tailor-0.0.15/tromero_tailor/wrapper.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-14 11:37:29.047161 tromero_tailor-0.0.15/tromero_tailor.egg-info/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-14 11:37:29.000000 tromero_tailor-0.0.15/tromero_tailor.egg-info/PKG-INFO
--rw-r--r--   0 tadhgamin   (501) staff       (20)      341 2024-05-14 11:37:29.000000 tromero_tailor-0.0.15/tromero_tailor.egg-info/SOURCES.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)        1 2024-05-14 11:37:29.000000 tromero_tailor-0.0.15/tromero_tailor.egg-info/dependency_links.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)      304 2024-05-14 11:37:29.000000 tromero_tailor-0.0.15/tromero_tailor.egg-info/requires.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)       15 2024-05-14 11:37:29.000000 tromero_tailor-0.0.15/tromero_tailor.egg-info/top_level.txt
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-17 14:21:25.193234 tromero_tailor-0.0.16/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-17 14:21:25.193012 tromero_tailor-0.0.16/PKG-INFO
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      942 2024-04-08 16:49:32.000000 tromero_tailor-0.0.16/README.md
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       38 2024-05-17 14:21:25.193286 tromero_tailor-0.0.16/setup.cfg
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1633 2024-05-17 14:20:53.000000 tromero_tailor-0.0.16/setup.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-17 14:21:25.191402 tromero_tailor-0.0.16/tests/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     3672 2024-04-17 14:55:07.000000 tromero_tailor-0.0.16/tests/test.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-17 14:21:25.191953 tromero_tailor-0.0.16/tromero_tailor/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       30 2024-04-08 15:07:54.000000 tromero_tailor-0.0.16/tromero_tailor/__init__.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1630 2024-05-17 14:18:24.000000 tromero_tailor-0.0.16/tromero_tailor/tromero_requests.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      446 2024-04-12 11:06:15.000000 tromero_tailor-0.0.16/tromero_tailor/tromero_utils.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     3024 2024-05-17 14:16:30.000000 tromero_tailor-0.0.16/tromero_tailor/wrapper.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-17 14:21:25.192768 tromero_tailor-0.0.16/tromero_tailor.egg-info/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-17 14:21:25.000000 tromero_tailor-0.0.16/tromero_tailor.egg-info/PKG-INFO
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      341 2024-05-17 14:21:25.000000 tromero_tailor-0.0.16/tromero_tailor.egg-info/SOURCES.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)        1 2024-05-17 14:21:25.000000 tromero_tailor-0.0.16/tromero_tailor.egg-info/dependency_links.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      304 2024-05-17 14:21:25.000000 tromero_tailor-0.0.16/tromero_tailor.egg-info/requires.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       15 2024-05-17 14:21:25.000000 tromero_tailor-0.0.16/tromero_tailor.egg-info/top_level.txt
```

### Comparing `tromero_tailor-0.0.15/PKG-INFO` & `tromero_tailor-0.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tromero_tailor
-Version: 0.0.15
+Version: 0.0.16
 Summary: A short description of your package
 Home-page: http://yourpackagehomepage.com
 Author: Tromero
 Author-email: tadhg.amin@tromero.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tromero_tailor-0.0.15/README.md` & `tromero_tailor-0.0.16/README.md`

 * *Files identical despite different names*

### Comparing `tromero_tailor-0.0.15/setup.py` & `tromero_tailor-0.0.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tromero_tailor",  # Replace with your package name
-    version="0.0.15",  # Replace with your package's version
+    version="0.0.16",  # Replace with your package's version
     author="Tromero",  # Replace with your name
     author_email="tadhg.amin@tromero.ai",  # Replace with your email address
     description="A short description of your package",  # Provide a short description
     long_description=open('README.md').read(),  # This will read your long description from README.md
     long_description_content_type='text/markdown',  # Indicates that the long description is in Markdown
     url="http://yourpackagehomepage.com",  # Replace with the URL to your package's homepage
     license="MIT",  # Replace with your chosen license
```

### Comparing `tromero_tailor-0.0.15/tests/test.py` & `tromero_tailor-0.0.16/tests/test.py`

 * *Files identical despite different names*

### Comparing `tromero_tailor-0.0.15/tromero_tailor/tromero_requests.py` & `tromero_tailor-0.0.16/tromero_tailor/tromero_requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,20 +13,21 @@
         response = requests.post(data_url, json=data, headers=headers)
         response.raise_for_status()  # Raises HTTPError for bad responses (4XX, 5XX)
         return response.json()  # Return the JSON response if request was successful
     except Exception as e:
         return {'error': f'An error occurred: {e}', 'status_code': response.status_code if 'response' in locals() else 'N/A'}
     
 
-def tromero_model_create(model, messages, tromero_key, self_hosted=False):
+def tromero_model_create(model, messages, tromero_key, parameters={}, self_hosted=False):
     url = self_hosted_models_url if self_hosted else models_url
     headers = {'Content-Type': 'application/json'}
     data = {
         "adapter_name": model,
         "messages": messages,
+        "parameters": parameters
     }
     headers['X-API-KEY'] = tromero_key
     if self_hosted:
         url = self_hosted_models_url 
     else:
         url = models_url
     try:
```

### Comparing `tromero_tailor-0.0.15/tromero_tailor/wrapper.py` & `tromero_tailor-0.0.16/tromero_tailor/wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,34 +36,34 @@
             return False
         model_names = [m.id for m in models]
         return model in model_names
     
     def create(self, *args, **kwargs):
         input = {"model": kwargs['model'], "messages": kwargs['messages']}
         tags = kwargs.get('tags', [])
-        formatted_kwargs = {k: v for k, v in kwargs.items() if k not in ['model', 'messages']}
+        formatted_kwargs = {k: v for k, v in kwargs.items() if k not in ['model', 'messages', 'tags']}
+        openai_kwargs = {k: v for k, v in kwargs.items() if k not in ['tags']}
         if self.check_model(kwargs['model']):
-            res = Completions.create(self, *args, **kwargs)  
+            res = Completions.create(self, *args, **openai_kwargs)  
             if hasattr(res, 'choices'):
                 usage = res.usage.model_dump()
                 for choice in res.choices:
                     formatted_choice = self._choice_to_dict(choice)
                     self._save_data({"messages": input['messages'] + [formatted_choice['message']],
                                     "model": input['model'],
                                     "kwargs": formatted_kwargs,
                                     "creation_time": str(datetime.datetime.now().isoformat()),
                                     "usage": usage,
                                     "tags": tags
                                     })
         else:
             messages = kwargs['messages']
-            res = tromero_model_create(kwargs['model'], messages, self._client.tromero_key, self._client.self_hosted)
+            res = tromero_model_create(kwargs['model'], messages, self._client.tromero_key, formatted_kwargs, self._client.self_hosted)
             # check if res has field 'generated_text'
             if 'generated_text' in res:
-                print("here")
                 res = mock_openai_format(res['generated_text'])
         return res
 
 
 class MockChat(Chat):
     def __init__(self, client):
         super().__init__(client)
```

### Comparing `tromero_tailor-0.0.15/tromero_tailor.egg-info/PKG-INFO` & `tromero_tailor-0.0.16/tromero_tailor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tromero_tailor
-Version: 0.0.15
+Version: 0.0.16
 Summary: A short description of your package
 Home-page: http://yourpackagehomepage.com
 Author: Tromero
 Author-email: tadhg.amin@tromero.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

