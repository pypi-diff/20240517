# Comparing `tmp/hal9-2.1.1.tar.gz` & `tmp/hal9-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hal9-2.1.1.tar", max compression
+gzip compressed data, was "hal9-2.1.2.tar", max compression
```

## Comparing `hal9-2.1.1.tar` & `hal9-2.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2951 2024-05-17 21:31:04.546605 hal9-2.1.1/README.md
--rw-r--r--   0        0        0       86 2024-05-17 21:31:04.478605 hal9-2.1.1/hal9/__init__.py
--rw-r--r--   0        0        0     1220 2024-05-17 21:31:04.478605 hal9-2.1.1/hal9/cli.py
--rw-r--r--   0        0        0      634 2024-05-17 21:31:04.478605 hal9-2.1.1/hal9/create.py
--rw-r--r--   0        0        0      574 2024-05-17 21:31:04.478605 hal9-2.1.1/hal9/deploy.py
--rw-r--r--   0        0        0      531 2024-05-17 21:31:04.478605 hal9-2.1.1/hal9/run.py
--rw-r--r--   0        0        0      352 2024-05-17 21:31:04.478605 hal9-2.1.1/hal9/targets/docker.py
--rw-r--r--   0        0        0     2061 2024-05-17 21:31:04.478605 hal9-2.1.1/hal9/targets/hal9.py
--rw-r--r--   0        0        0       42 2024-05-17 21:31:04.478605 hal9-2.1.1/hal9/templates/docker/Dockerfile
--rw-r--r--   0        0        0       58 2024-05-17 21:31:04.478605 hal9-2.1.1/hal9/templates/openai/app.py
--rw-r--r--   0        0        0      434 2024-05-17 21:31:04.478605 hal9-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 hal9-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2951 2024-05-17 21:37:53.967241 hal9-2.1.2/README.md
+-rw-r--r--   0        0        0       86 2024-05-17 21:37:53.895241 hal9-2.1.2/hal9/__init__.py
+-rw-r--r--   0        0        0     1220 2024-05-17 21:37:53.895241 hal9-2.1.2/hal9/cli.py
+-rw-r--r--   0        0        0      634 2024-05-17 21:37:53.895241 hal9-2.1.2/hal9/create.py
+-rw-r--r--   0        0        0      574 2024-05-17 21:37:53.895241 hal9-2.1.2/hal9/deploy.py
+-rw-r--r--   0        0        0      531 2024-05-17 21:37:53.895241 hal9-2.1.2/hal9/run.py
+-rw-r--r--   0        0        0      352 2024-05-17 21:37:53.895241 hal9-2.1.2/hal9/targets/docker.py
+-rw-r--r--   0        0        0     2021 2024-05-17 21:37:53.899241 hal9-2.1.2/hal9/targets/hal9.py
+-rw-r--r--   0        0        0       42 2024-05-17 21:37:53.899241 hal9-2.1.2/hal9/templates/docker/Dockerfile
+-rw-r--r--   0        0        0       38 2024-05-17 21:37:53.899241 hal9-2.1.2/hal9/templates/openai/app.py
+-rw-r--r--   0        0        0      434 2024-05-17 21:37:53.899241 hal9-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 hal9-2.1.2/PKG-INFO
```

### Comparing `hal9-2.1.1/README.md` & `hal9-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hal9-2.1.1/hal9/cli.py` & `hal9-2.1.2/hal9/cli.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.1/hal9/create.py` & `hal9-2.1.2/hal9/create.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.1/hal9/deploy.py` & `hal9-2.1.2/hal9/deploy.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.1/hal9/run.py` & `hal9-2.1.2/hal9/run.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.1/hal9/targets/hal9.py` & `hal9-2.1.2/hal9/targets/hal9.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
     with zipfile.ZipFile(zip_path, 'w', zipfile.ZIP_DEFLATED) as zipf:
         for root, dirs, files in os.walk(path):
             for file in files:
                 file_path = os.path.join(root, file)
                 zipf.write(file_path, os.path.relpath(file_path, path))
     
-    print(f"Created {zip_path}")
     return zip_path
 
 def request_deploy(path :str, url :str) -> str:
     project_name = project_from_path(path)
     zip_path = create_deployment(path)
 
     unixtime = int(time.time())
@@ -42,26 +41,25 @@
 
     payload = {
         'filename': upload_name,
         'content': encoded_content,
         'type': 'ability',
     }
 
-    print(f'Uploading {upload_name}')
-
     headers = {
         'Content-Type': 'application/json',
         'ApiKey': os.environ['HAL9_TOKEN'],
     }
     response = requests.post(url + '/api/v1/asset', headers = headers, data = json.dumps(payload))
     
     if not response.ok:
         response.raise_for_status()
 
     response_data = response.json()
+    print(response_data['url'])
 
 def deploy(path :str, url :str) -> str:
     if 'HAL9_TOKEN' in os.environ:
         hal9_token = os.environ['HAL9_TOKEN']
     else:
         exit('HAL9_TOKEN environment variable missing, see https://hal9.com/deploy')
         # hal9_token = browser_login()
```

### Comparing `hal9-2.1.1/PKG-INFO` & `hal9-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hal9
-Version: 2.1.1
+Version: 2.1.2
 Summary: 
 Author: Javier Luraschi
 Author-email: javier@hal9.ai
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

