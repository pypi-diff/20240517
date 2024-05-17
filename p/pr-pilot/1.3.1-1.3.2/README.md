# Comparing `tmp/pr_pilot-1.3.1.tar.gz` & `tmp/pr_pilot-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_pilot-1.3.1.tar", last modified: Wed Apr 24 20:23:24 2024, max compression
+gzip compressed data, was "pr_pilot-1.3.2.tar", last modified: Thu Apr 25 23:14:40 2024, max compression
```

## Comparing `pr_pilot-1.3.1.tar` & `pr_pilot-1.3.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:23:24.753994 pr_pilot-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-24 20:23:24.753994 pr_pilot-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:23:24.753994 pr_pilot-1.3.1/pr_pilot/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:23:24.753994 pr_pilot-1.3.1/pr_pilot/api/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/api/task_creation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/api/task_retrieval_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26236 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15420 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:23:24.753994 pr_pilot-1.3.1/pr_pilot/models/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/models/bad_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/models/not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/models/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/models/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:23:24.753994 pr_pilot-1.3.1/pr_pilot/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/test/test_bad_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/test/test_not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/test/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/test/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/test/test_task_creation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/test/test_task_retrieval_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:23:24.753994 pr_pilot-1.3.1/pr_pilot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-24 20:23:24.000000 pr_pilot-1.3.1/pr_pilot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-24 20:23:24.000000 pr_pilot-1.3.1/pr_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:23:24.000000 pr_pilot-1.3.1/pr_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 20:23:24.000000 pr_pilot-1.3.1/pr_pilot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 20:23:24.000000 pr_pilot-1.3.1/pr_pilot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 20:23:24.753994 pr_pilot-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:14:40.986191 pr_pilot-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-25 23:14:40.982191 pr_pilot-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:14:40.982191 pr_pilot-1.3.2/pr_pilot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:14:40.982191 pr_pilot-1.3.2/pr_pilot/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/api/task_creation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/api/task_retrieval_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26236 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15420 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:14:40.982191 pr_pilot-1.3.2/pr_pilot/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/models/bad_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/models/not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/models/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:14:40.982191 pr_pilot-1.3.2/pr_pilot/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/test/test_bad_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/test/test_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/test/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/test/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/test/test_task_creation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/test/test_task_retrieval_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/pr_pilot/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 23:14:40.982191 pr_pilot-1.3.2/pr_pilot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-25 23:14:40.000000 pr_pilot-1.3.2/pr_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-25 23:14:40.000000 pr_pilot-1.3.2/pr_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 23:14:40.000000 pr_pilot-1.3.2/pr_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 23:14:40.000000 pr_pilot-1.3.2/pr_pilot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 23:14:40.000000 pr_pilot-1.3.2/pr_pilot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 23:14:40.986191 pr_pilot-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-25 23:14:36.000000 pr_pilot-1.3.2/setup.py
```

### Comparing `pr_pilot-1.3.1/LICENSE` & `pr_pilot-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/PKG-INFO` & `pr_pilot-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr_pilot
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python SDK for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-python
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr_pilot Version: 1.3.1 Summary: Python SDK for PR
+Metadata-Version: 2.1 Name: pr_pilot Version: 1.3.2 Summary: Python SDK for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-python Author: Marco Lamina Author-email:
 marco@pr-pilot.ai License: GPL-3.0 Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pydantic==2.7.0 Requires-Dist:
 urllib3==2.2.1 Requires-Dist: python-dateutil==2.9.0 Requires-Dist:
```

### Comparing `pr_pilot-1.3.1/README.md` & `pr_pilot-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/__init__.py` & `pr_pilot-1.3.2/pr_pilot/__init__.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/api/task_creation_api.py` & `pr_pilot-1.3.2/pr_pilot/api/task_creation_api.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/api/task_retrieval_api.py` & `pr_pilot-1.3.2/pr_pilot/api/task_retrieval_api.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/api_client.py` & `pr_pilot-1.3.2/pr_pilot/api_client.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/api_response.py` & `pr_pilot-1.3.2/pr_pilot/api_response.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/configuration.py` & `pr_pilot-1.3.2/pr_pilot/configuration.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/exceptions.py` & `pr_pilot-1.3.2/pr_pilot/exceptions.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/models/bad_request.py` & `pr_pilot-1.3.2/pr_pilot/models/bad_request.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/models/not_found.py` & `pr_pilot-1.3.2/pr_pilot/models/not_found.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/models/prompt.py` & `pr_pilot-1.3.2/pr_pilot/models/prompt.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/models/task.py` & `pr_pilot-1.3.2/pr_pilot/models/task.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/rest.py` & `pr_pilot-1.3.2/pr_pilot/rest.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/test/test_bad_request.py` & `pr_pilot-1.3.2/pr_pilot/test/test_bad_request.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/test/test_not_found.py` & `pr_pilot-1.3.2/pr_pilot/test/test_not_found.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/test/test_prompt.py` & `pr_pilot-1.3.2/pr_pilot/test/test_prompt.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/test/test_task.py` & `pr_pilot-1.3.2/pr_pilot/test/test_task.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/test/test_task_creation_api.py` & `pr_pilot-1.3.2/pr_pilot/test/test_task_creation_api.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/test/test_task_retrieval_api.py` & `pr_pilot-1.3.2/pr_pilot/test/test_task_retrieval_api.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/pr_pilot/util.py` & `pr_pilot-1.3.2/pr_pilot/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,13 +87,16 @@
         if time.time() - start_time > MAX_RESULT_WAIT_TIME:
             raise TimeoutError("The task took too long to complete.")
         if log:
             logger.info(f"Task status: {task.status}. Waiting for completion...")
         task = get_task(task.id)
 
         time.sleep(POLL_INTERVAL)
+    set_github_action_output("task-result", task.result)
     if write_step_summary:
         dashboard_url = f"https://app.pr-pilot.ai/dashboard/tasks/{str(task.id)}/"
         markdown_link = f"📋 **[Log]({dashboard_url})**"
         set_github_step_summary(f"---\n\n{task.result}\n\n---\n{markdown_link}")
-        set_github_action_output("task-result", task.result)
+    if task.status == "failed":
+        raise ValueError(f"Task failed: {task.result}")
+
     return task.result
```

### Comparing `pr_pilot-1.3.1/pr_pilot.egg-info/PKG-INFO` & `pr_pilot-1.3.2/pr_pilot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr_pilot
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python SDK for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-python
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr_pilot Version: 1.3.1 Summary: Python SDK for PR
+Metadata-Version: 2.1 Name: pr_pilot Version: 1.3.2 Summary: Python SDK for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-python Author: Marco Lamina Author-email:
 marco@pr-pilot.ai License: GPL-3.0 Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pydantic==2.7.0 Requires-Dist:
 urllib3==2.2.1 Requires-Dist: python-dateutil==2.9.0 Requires-Dist:
```

### Comparing `pr_pilot-1.3.1/pr_pilot.egg-info/SOURCES.txt` & `pr_pilot-1.3.2/pr_pilot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.1/setup.py` & `pr_pilot-1.3.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_dir = path.abspath(path.dirname(__file__))
 requirements_path = path.join(this_dir, 'requirements.txt')
 with open(requirements_path) as f:
     required = f.read().splitlines()
 
 setup(
     name='pr_pilot',
-    version='1.3.1',
+    version='1.3.2',
     packages=find_packages(),
     install_requires=required,
     python_requires='>=3.6',
     author='Marco Lamina',
     author_email='marco@pr-pilot.ai',
     description='Python SDK for PR Pilot, a text-to-task automation platform for Github.',
     long_description=open('README.md').read(),
```

