# Comparing `tmp/WrenchCL-2.1.0.tar.gz` & `tmp/WrenchCL-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WrenchCL-2.1.0.tar", last modified: Fri May 17 19:51:38 2024, max compression
+gzip compressed data, was "WrenchCL-2.1.1.tar", last modified: Fri May 17 19:55:57 2024, max compression
```

## Comparing `WrenchCL-2.1.0.tar` & `WrenchCL-2.1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.560938 WrenchCL-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-05-17 19:51:38.560938 WrenchCL-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21954 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.552937 WrenchCL-2.1.0/WrenchCL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.556938 WrenchCL-2.1.0/WrenchCL/Connect/
--rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Connect/AwsClientHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Connect/RdsServiceGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Connect/S3ServiceGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Connect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.556938 WrenchCL-2.1.0/WrenchCL/DataFlow/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/DataFlow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/DataFlow/build_return_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/DataFlow/handle_lambda_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/DataFlow/trigger_dataflow_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.556938 WrenchCL-2.1.0/WrenchCL/Decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Decorators/Retryable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Decorators/SingletonClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Decorators/TimedMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.556938 WrenchCL-2.1.0/WrenchCL/Models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.556938 WrenchCL-2.1.0/WrenchCL/Models/OpenAI/
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Models/OpenAI/OpenAIFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15468 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Models/OpenAI/OpenAIGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Models/OpenAI/_ConversationManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Models/OpenAI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.556938 WrenchCL-2.1.0/WrenchCL/Tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Tools/Coalesce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Tools/DictValidator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Tools/FetchMetaData.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Tools/FileTyper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Tools/Image2B64.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Tools/MaybeMonad.py
--rw-r--r--   0 runner    (1001) docker     (127)    28041 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Tools/WrenchLogger.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.560938 WrenchCL-2.1.0/WrenchCL/_Internal/
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/_Internal/_ConfigurationManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/_Internal/_SshTunnelManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/_Internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.556938 WrenchCL-2.1.0/WrenchCL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-05-17 19:51:38.000000 WrenchCL-2.1.0/WrenchCL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-17 19:51:38.000000 WrenchCL-2.1.0/WrenchCL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:51:38.000000 WrenchCL-2.1.0/WrenchCL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-17 19:51:38.000000 WrenchCL-2.1.0/WrenchCL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 19:51:38.000000 WrenchCL-2.1.0/WrenchCL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:51:38.560938 WrenchCL-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-17 19:51:36.000000 WrenchCL-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.540559 WrenchCL-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-05-17 19:55:57.540559 WrenchCL-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21954 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.536559 WrenchCL-2.1.1/WrenchCL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.536559 WrenchCL-2.1.1/WrenchCL/Connect/
+-rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Connect/AwsClientHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Connect/RdsServiceGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Connect/S3ServiceGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Connect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.536559 WrenchCL-2.1.1/WrenchCL/DataFlow/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/DataFlow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/DataFlow/build_return_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/DataFlow/handle_lambda_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/DataFlow/trigger_dataflow_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.536559 WrenchCL-2.1.1/WrenchCL/Decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Decorators/Retryable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Decorators/SingletonClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Decorators/TimedMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.540559 WrenchCL-2.1.1/WrenchCL/Models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.540559 WrenchCL-2.1.1/WrenchCL/Models/OpenAI/
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Models/OpenAI/OpenAIFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15468 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Models/OpenAI/OpenAIGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Models/OpenAI/_ConversationManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Models/OpenAI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.540559 WrenchCL-2.1.1/WrenchCL/Tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Tools/Coalesce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Tools/DictValidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Tools/FetchMetaData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Tools/FileTyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Tools/Image2B64.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Tools/MaybeMonad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28041 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Tools/WrenchLogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/Tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.540559 WrenchCL-2.1.1/WrenchCL/_Internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/_Internal/_ConfigurationManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/_Internal/_SshTunnelManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/_Internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-17 19:55:31.000000 WrenchCL-2.1.1/WrenchCL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:55:57.536559 WrenchCL-2.1.1/WrenchCL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-05-17 19:55:57.000000 WrenchCL-2.1.1/WrenchCL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-17 19:55:57.000000 WrenchCL-2.1.1/WrenchCL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:55:57.000000 WrenchCL-2.1.1/WrenchCL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-17 19:55:57.000000 WrenchCL-2.1.1/WrenchCL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 19:55:57.000000 WrenchCL-2.1.1/WrenchCL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:55:57.540559 WrenchCL-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-17 19:55:56.000000 WrenchCL-2.1.1/setup.py
```

### Comparing `WrenchCL-2.1.0/LICENSE` & `WrenchCL-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/PKG-INFO` & `WrenchCL-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WrenchCL
-Version: 2.1.0
+Version: 2.1.1
 Summary: WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 Home-page: https://github.com/WrenchAI/WrenchCL
 Author: willem@wrench.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.0 Summary: WrenchCL is a
+Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.1 Summary: WrenchCL is a
 comprehensive library designed to facilitate seamless interactions with AWS
 services, OpenAI models, and various utility tools. This package aims to
 streamline the development process by providing robust components for database
 interactions, cloud storage, and AI-powered functionalities. Home-page: https:/
 /github.com/WrenchAI/WrenchCL Author: willem@wrench.ai Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.11
```

### Comparing `WrenchCL-2.1.0/README.md` & `WrenchCL-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Connect/AwsClientHub.py` & `WrenchCL-2.1.1/WrenchCL/Connect/AwsClientHub.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Connect/RdsServiceGateway.py` & `WrenchCL-2.1.1/WrenchCL/Connect/RdsServiceGateway.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Connect/S3ServiceGateway.py` & `WrenchCL-2.1.1/WrenchCL/Connect/S3ServiceGateway.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/DataFlow/build_return_json.py` & `WrenchCL-2.1.1/WrenchCL/DataFlow/build_return_json.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/DataFlow/handle_lambda_response.py` & `WrenchCL-2.1.1/WrenchCL/DataFlow/handle_lambda_response.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/DataFlow/trigger_dataflow_metrics.py` & `WrenchCL-2.1.1/WrenchCL/DataFlow/trigger_dataflow_metrics.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Decorators/Retryable.py` & `WrenchCL-2.1.1/WrenchCL/Decorators/Retryable.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Decorators/SingletonClass.py` & `WrenchCL-2.1.1/WrenchCL/Decorators/SingletonClass.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Decorators/TimedMethod.py` & `WrenchCL-2.1.1/WrenchCL/Decorators/TimedMethod.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Models/OpenAI/OpenAIFactory.py` & `WrenchCL-2.1.1/WrenchCL/Models/OpenAI/OpenAIFactory.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Models/OpenAI/OpenAIGateway.py` & `WrenchCL-2.1.1/WrenchCL/Models/OpenAI/OpenAIGateway.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Models/OpenAI/_ConversationManager.py` & `WrenchCL-2.1.1/WrenchCL/Models/OpenAI/_ConversationManager.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Models/OpenAI/__init__.py` & `WrenchCL-2.1.1/WrenchCL/Models/OpenAI/__init__.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Tools/Coalesce.py` & `WrenchCL-2.1.1/WrenchCL/Tools/Coalesce.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Tools/DictValidator.py` & `WrenchCL-2.1.1/WrenchCL/Tools/DictValidator.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Tools/FetchMetaData.py` & `WrenchCL-2.1.1/WrenchCL/Tools/FetchMetaData.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Tools/FileTyper.py` & `WrenchCL-2.1.1/WrenchCL/Tools/FileTyper.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Tools/Image2B64.py` & `WrenchCL-2.1.1/WrenchCL/Tools/Image2B64.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Tools/MaybeMonad.py` & `WrenchCL-2.1.1/WrenchCL/Tools/MaybeMonad.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/Tools/WrenchLogger.py` & `WrenchCL-2.1.1/WrenchCL/Tools/WrenchLogger.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/_Internal/_ConfigurationManager.py` & `WrenchCL-2.1.1/WrenchCL/_Internal/_ConfigurationManager.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL/_Internal/_SshTunnelManager.py` & `WrenchCL-2.1.1/WrenchCL/_Internal/_SshTunnelManager.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/WrenchCL.egg-info/PKG-INFO` & `WrenchCL-2.1.1/WrenchCL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WrenchCL
-Version: 2.1.0
+Version: 2.1.1
 Summary: WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 Home-page: https://github.com/WrenchAI/WrenchCL
 Author: willem@wrench.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.0 Summary: WrenchCL is a
+Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.1 Summary: WrenchCL is a
 comprehensive library designed to facilitate seamless interactions with AWS
 services, OpenAI models, and various utility tools. This package aims to
 streamline the development process by providing robust components for database
 interactions, cloud storage, and AI-powered functionalities. Home-page: https:/
 /github.com/WrenchAI/WrenchCL Author: willem@wrench.ai Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.11
```

### Comparing `WrenchCL-2.1.0/WrenchCL.egg-info/SOURCES.txt` & `WrenchCL-2.1.1/WrenchCL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.0/setup.py` & `WrenchCL-2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     print(
         "Note: If you encounter issues with python-magic on Windows, please install python-magic-bin manually:\n"
         "pip install python-magic-bin~=0.4.14"
     )
 
 setup(
     name='WrenchCL',
-    version='v2.1.0',
+    version='v2.1.1',
     author='willem@wrench.ai',
     description=(
         'WrenchCL is a comprehensive library designed to facilitate seamless interactions with '
         'AWS services, OpenAI models, and various utility tools. This package aims to streamline '
         'the development process by providing robust components for database interactions, '
         'cloud storage, and AI-powered functionalities.'
     ),
```

