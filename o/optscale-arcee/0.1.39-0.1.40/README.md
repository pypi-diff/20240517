# Comparing `tmp/optscale_arcee-0.1.39.tar.gz` & `tmp/optscale_arcee-0.1.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optscale_arcee-0.1.39.tar", last modified: Thu Apr 18 12:55:11 2024, max compression
+gzip compressed data, was "optscale_arcee-0.1.40.tar", last modified: Fri May 17 07:13:36 2024, max compression
```

## Comparing `optscale_arcee-0.1.39.tar` & `optscale_arcee-0.1.40.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:11.831022 optscale_arcee-0.1.39/
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-18 12:55:11.831022 optscale_arcee-0.1.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:11.827022 optscale_arcee-0.1.39/optscale_arcee/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/arcee.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:11.831022 optscale_arcee-0.1.39/optscale_arcee/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/collectors/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/collectors/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/collectors/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/collectors/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/collectors/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/name_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:11.831022 optscale_arcee-0.1.39/optscale_arcee/platforms_meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/platforms_meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/platforms_meta/azure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:11.831022 optscale_arcee-0.1.39/optscale_arcee/sender/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/sender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7878 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/sender/sender.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:11.831022 optscale_arcee-0.1.39/optscale_arcee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-18 12:55:11.000000 optscale_arcee-0.1.39/optscale_arcee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-18 12:55:11.000000 optscale_arcee-0.1.39/optscale_arcee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:55:11.000000 optscale_arcee-0.1.39/optscale_arcee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-18 12:55:11.000000 optscale_arcee-0.1.39/optscale_arcee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 12:55:11.000000 optscale_arcee-0.1.39/optscale_arcee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-18 12:55:11.831022 optscale_arcee-0.1.39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:11.831022 optscale_arcee-0.1.39/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/tests/test_platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:13:36.331524 optscale_arcee-0.1.40/
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-17 07:13:36.331524 optscale_arcee-0.1.40/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:13:36.327525 optscale_arcee-0.1.40/optscale_arcee/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/optscale_arcee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/optscale_arcee/arcee.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:13:36.327525 optscale_arcee-0.1.40/optscale_arcee/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/optscale_arcee/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/optscale_arcee/collectors/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/optscale_arcee/collectors/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/optscale_arcee/collectors/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/optscale_arcee/collectors/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/optscale_arcee/collectors/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/optscale_arcee/name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/optscale_arcee/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:13:36.327525 optscale_arcee-0.1.40/optscale_arcee/platforms_meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/optscale_arcee/platforms_meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/optscale_arcee/platforms_meta/azure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:13:36.327525 optscale_arcee-0.1.40/optscale_arcee/sender/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/optscale_arcee/sender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/optscale_arcee/sender/sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/optscale_arcee/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:13:36.331524 optscale_arcee-0.1.40/optscale_arcee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-17 07:13:36.000000 optscale_arcee-0.1.40/optscale_arcee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-17 07:13:36.000000 optscale_arcee-0.1.40/optscale_arcee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 07:13:36.000000 optscale_arcee-0.1.40/optscale_arcee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-17 07:13:36.000000 optscale_arcee-0.1.40/optscale_arcee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 07:13:36.000000 optscale_arcee-0.1.40/optscale_arcee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-17 07:13:36.331524 optscale_arcee-0.1.40/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:13:36.331524 optscale_arcee-0.1.40/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-17 07:13:32.000000 optscale_arcee-0.1.40/tests/test_platform.py
```

### Comparing `optscale_arcee-0.1.39/LICENSE` & `optscale_arcee-0.1.40/LICENSE`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.39/PKG-INFO` & `optscale_arcee-0.1.40/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optscale_arcee
-Version: 0.1.39
+Version: 0.1.40
 Summary: ML profiling tool for OptScale
 Home-page: https://my.optscale.com/
 Author: Hystax
 License: "Apache License 2.0"
 Project-URL: Source, https://github.com/hystax/optscale_arcee
 Keywords: arcee,ml,optscale,finops,mlops
 Requires-Python: <4,>=3.7
@@ -14,15 +14,15 @@
 Requires-Dist: aiofiles==22.1.0
 Requires-Dist: GPUtil==1.4.0
 Requires-Dist: psutil==5.9.2
 
 # Arcee
 ## *The OptScale ML profiling tool by Hystax*
 
-Arcee is a tool that hepls you to integrate ML tasks with [OptScale](https://my.optscale.com/).
+Arcee is a tool that helps you to integrate ML tasks with [OptScale](https://my.optscale.com/).
 This tool can automatically collect executor metadata from cloud and process stats.
 
 ## Installation
 Arcee requires python 3.7+ to run.
 ```sh
 pip install optscale-arcee
 ```
```

### Comparing `optscale_arcee-0.1.39/README.md` & `optscale_arcee-0.1.40/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Arcee
 ## *The OptScale ML profiling tool by Hystax*
 
-Arcee is a tool that hepls you to integrate ML tasks with [OptScale](https://my.optscale.com/).
+Arcee is a tool that helps you to integrate ML tasks with [OptScale](https://my.optscale.com/).
 This tool can automatically collect executor metadata from cloud and process stats.
 
 ## Installation
 Arcee requires python 3.7+ to run.
 ```sh
 pip install optscale-arcee
 ```
```

### Comparing `optscale_arcee-0.1.39/optscale_arcee/arcee.py` & `optscale_arcee-0.1.40/optscale_arcee/arcee.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import warnings
 import time
 import threading
 
 from optscale_arcee.sender.sender import Sender
 from optscale_arcee.collectors.console import (
     acquire_console, release_console)
 from optscale_arcee.name_generator import NameGenerator
@@ -139,32 +138,22 @@
     def model_version_aliases(self, value):
         aliases = set(self._model_version_aliases)
         aliases.add(value)
         self._model_version_aliases = list(aliases)
 
 
 def init(
-    token, task_key=None, run_name=None, endpoint_url=None, ssl=True, period=1,
-        model_key=None
+    token, task_key, run_name=None, endpoint_url=None, ssl=True, period=1
 ):
-    if model_key:
-        warnings.warn(
-            "`model_key` parameter is deprecated and will be removed in the "
-            "future releases, consider using `task_key` instead",
-            UserWarning
-        )
-    if not task_key or model_key:
-        raise TypeError('`task_key` is not provided')
     acquire_console()
-    arcee = Arcee(token, task_key or model_key, endpoint_url, ssl)
+    arcee = Arcee(token, task_key, endpoint_url, ssl)
     name = (
         run_name if run_name is not None else NameGenerator.get_random_name()
     )
-    run_id = asyncio.run(arcee.sender.get_run_id(
-        task_key or model_key, token, name))["id"]
+    run_id = asyncio.run(arcee.sender.get_run_id(task_key, token, name))["id"]
     arcee.run = run_id
     arcee.name = name
     arcee.hb = Job(
         meth_args=(arcee.sender, run_id, token),
         sleep=period,
         shutdown_flag=arcee.shutdown_flag,
     )
@@ -281,40 +270,40 @@
     arcee = Arcee()
     arcee.model = asyncio.run(
         arcee.sender.add_model(
             arcee.token, key
         )
     )
     asyncio.run(
-        arcee.sender.assign_model_run(
-            arcee.model, arcee.run, arcee.token, path=path
+        arcee.sender.create_model_version(
+            arcee.run, arcee.model, arcee.token, path=path
         )
     )
 
 
 def model_version(version):
     arcee = Arcee()
     asyncio.run(
         arcee.sender.add_version(
-            arcee.model, arcee.run, arcee.token, version
+            arcee.run, arcee.model, arcee.token, version
         )
     )
 
 
 def model_version_alias(alias):
     arcee = Arcee()
     arcee.model_version_aliases = alias
     asyncio.run(
         arcee.sender.add_version_aliases(
-            arcee.model, arcee.run, arcee.token, arcee.model_version_aliases
+            arcee.run, arcee.model, arcee.token, arcee.model_version_aliases
         )
     )
 
 
 def model_version_tag(key, value):
     arcee = Arcee()
     arcee.model_version_tags = (key, value)
     asyncio.run(
         arcee.sender.add_version_tags(
-            arcee.model, arcee.run, arcee.token, arcee.model_version_tags
+            arcee.run, arcee.model, arcee.token, arcee.model_version_tags
         )
     )
```

### Comparing `optscale_arcee-0.1.39/optscale_arcee/collectors/console.py` & `optscale_arcee-0.1.40/optscale_arcee/collectors/console.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.39/optscale_arcee/collectors/git.py` & `optscale_arcee-0.1.40/optscale_arcee/collectors/git.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.39/optscale_arcee/collectors/hardware.py` & `optscale_arcee-0.1.40/optscale_arcee/collectors/hardware.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.39/optscale_arcee/collectors/module.py` & `optscale_arcee-0.1.40/optscale_arcee/collectors/module.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.39/optscale_arcee/name_generator.py` & `optscale_arcee-0.1.40/optscale_arcee/name_generator.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.39/optscale_arcee/platform.py` & `optscale_arcee-0.1.40/optscale_arcee/platform.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.39/optscale_arcee/platforms_meta/azure.py` & `optscale_arcee-0.1.40/optscale_arcee/platforms_meta/azure.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.39/optscale_arcee/sender/sender.py` & `optscale_arcee-0.1.40/optscale_arcee/sender/sender.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,30 +168,30 @@
         headers = {"x-api-key": token, "Content-Type": "application/json"}
         model = await self.send_post_request(
             self.endpoint_url + '/models', headers, {"key": key}
         )
         return model.get('_id')
 
     @check_shutdown_flag_set
-    async def assign_model_run(self, model_id, run_id, token, path=None):
+    async def create_model_version(self, run_id, model_id, token, path=None):
         headers = {"x-api-key": token, "Content-Type": "application/json"}
-        uri = f'{self.endpoint_url}/models/{model_id}/runs/{run_id}'
+        uri = f'{self.endpoint_url}/runs/{run_id}/models/{model_id}/version'
         body = {'path': path} if path else {}
         await self.send_post_request(uri, headers, body)
 
     @check_shutdown_flag_set
-    async def patch_model_version(self, model_id, run_id, token, params):
+    async def patch_model_version(self, run_id, model_id, token, params):
         headers = {"x-api-key": token, "Content-Type": "application/json"}
-        uri = f'{self.endpoint_url}/models/{model_id}/runs/{run_id}'
+        uri = f'{self.endpoint_url}/runs/{run_id}/models/{model_id}/version'
         await self.send_patch_request(uri, headers, params)
 
-    async def add_version(self, model_id, run_id, token, version):
+    async def add_version(self, run_id, model_id, token, version):
         body = {'version': str(version)}
-        await self.patch_model_version(model_id, run_id, token, body)
+        await self.patch_model_version(run_id, model_id, token, body)
 
-    async def add_version_aliases(self, model_id, run_id, token, aliases):
+    async def add_version_aliases(self, run_id, model_id, token, aliases):
         body = {'aliases': aliases}
-        await self.patch_model_version(model_id, run_id, token, body)
+        await self.patch_model_version(run_id, model_id, token, body)
 
-    async def add_version_tags(self, model_id, run_id, token, tags):
+    async def add_version_tags(self, run_id, model_id, token, tags):
         body = {'tags': tags}
-        await self.patch_model_version(model_id, run_id, token, body)
+        await self.patch_model_version(run_id, model_id, token, body)
```

### Comparing `optscale_arcee-0.1.39/optscale_arcee/utils.py` & `optscale_arcee-0.1.40/optscale_arcee/utils.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.39/optscale_arcee.egg-info/PKG-INFO` & `optscale_arcee-0.1.40/optscale_arcee.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optscale_arcee
-Version: 0.1.39
+Version: 0.1.40
 Summary: ML profiling tool for OptScale
 Home-page: https://my.optscale.com/
 Author: Hystax
 License: "Apache License 2.0"
 Project-URL: Source, https://github.com/hystax/optscale_arcee
 Keywords: arcee,ml,optscale,finops,mlops
 Requires-Python: <4,>=3.7
@@ -14,15 +14,15 @@
 Requires-Dist: aiofiles==22.1.0
 Requires-Dist: GPUtil==1.4.0
 Requires-Dist: psutil==5.9.2
 
 # Arcee
 ## *The OptScale ML profiling tool by Hystax*
 
-Arcee is a tool that hepls you to integrate ML tasks with [OptScale](https://my.optscale.com/).
+Arcee is a tool that helps you to integrate ML tasks with [OptScale](https://my.optscale.com/).
 This tool can automatically collect executor metadata from cloud and process stats.
 
 ## Installation
 Arcee requires python 3.7+ to run.
 ```sh
 pip install optscale-arcee
 ```
```

### Comparing `optscale_arcee-0.1.39/optscale_arcee.egg-info/SOURCES.txt` & `optscale_arcee-0.1.40/optscale_arcee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.39/setup.cfg` & `optscale_arcee-0.1.40/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = optscale_arcee
-version = 0.1.39
+version = 0.1.40
 author = Hystax
 description = ML profiling tool for OptScale
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = "Apache License 2.0"
 url = https://my.optscale.com/
 project_urls =
```

### Comparing `optscale_arcee-0.1.39/tests/test_data.py` & `optscale_arcee-0.1.40/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.39/tests/test_platform.py` & `optscale_arcee-0.1.40/tests/test_platform.py`

 * *Files identical despite different names*

