# Comparing `tmp/fluxional-0.1.7.tar.gz` & `tmp/fluxional-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxional-0.1.7.tar", max compression
+gzip compressed data, was "fluxional-0.1.8.tar", max compression
```

## Comparing `fluxional-0.1.7.tar` & `fluxional-0.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1066 2024-04-28 17:10:39.085356 fluxional-0.1.7/LICENSE
--rw-r--r--   0        0        0     3908 2024-04-29 21:12:21.619975 fluxional-0.1.7/README.md
--rw-r--r--   0        0        0      421 2024-05-15 20:00:12.862573 fluxional-0.1.7/fluxional/__init__.py
--rw-r--r--   0        0        0       85 2024-04-28 18:14:21.913877 fluxional-0.1.7/fluxional/__main__.py
--rw-r--r--   0        0        0     1429 2024-04-28 18:14:21.923877 fluxional-0.1.7/fluxional/cli/__init__.py
--rw-r--r--   0        0        0      397 2024-04-28 18:14:21.923877 fluxional-0.1.7/fluxional/core/__init__.py
--rw-r--r--   0        0        0    21405 2024-05-09 01:45:17.632254 fluxional-0.1.7/fluxional/core/app.py
--rw-r--r--   0        0        0     6976 2024-04-28 18:14:21.933877 fluxional-0.1.7/fluxional/core/core.py
--rw-r--r--   0        0        0     2927 2024-04-28 18:14:21.933877 fluxional-0.1.7/fluxional/core/events.py
--rw-r--r--   0        0        0    11708 2024-04-28 18:14:21.943877 fluxional-0.1.7/fluxional/core/handlers.py
--rw-r--r--   0        0        0        1 2024-04-28 18:14:21.943877 fluxional-0.1.7/fluxional/core/infrastructure/__init__.py
--rw-r--r--   0        0        0    20142 2024-05-15 19:51:13.339223 fluxional-0.1.7/fluxional/core/infrastructure/base.py
--rw-r--r--   0        0        0     7699 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/core/infrastructure/cdk.py
--rw-r--r--   0        0        0     9554 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/core/infrastructure/resources.py
--rw-r--r--   0        0        0      816 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/core/infrastructure/types.py
--rw-r--r--   0        0        0     5818 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/core/logic.py
--rw-r--r--   0        0        0     8343 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/core/settings.py
--rw-r--r--   0        0        0     4045 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/core/tools.py
--rw-r--r--   0        0        0     5158 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/core/types.py
--rw-r--r--   0        0        0       74 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/deployment/__init__.py
--rw-r--r--   0        0        0     1164 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/deployment/constants.py
--rw-r--r--   0        0        0    15517 2024-04-30 22:02:31.375706 fluxional-0.1.7/fluxional/deployment/engine.py
--rw-r--r--   0        0        0      345 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/deployment/exceptions.py
--rw-r--r--   0        0        0        1 2024-04-30 22:01:04.012000 fluxional-0.1.7/fluxional/deployment/utils.py
--rw-r--r--   0        0        0     3652 2024-04-28 18:14:21.963877 fluxional-0.1.7/fluxional/dev/__init__.py
--rw-r--r--   0        0        0     3003 2024-04-28 18:14:21.963877 fluxional-0.1.7/fluxional/dev/client.py
--rw-r--r--   0        0        0     3350 2024-04-28 18:14:21.963877 fluxional-0.1.7/fluxional/dev/runner.py
--rw-r--r--   0        0        0      326 2024-04-28 18:14:21.963877 fluxional-0.1.7/fluxional/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-28 18:14:21.963877 fluxional-0.1.7/fluxional/py.typed
--rw-r--r--   0        0        0      461 2024-04-28 18:14:21.963877 fluxional-0.1.7/fluxional/types.py
--rw-r--r--   0        0        0      935 2024-04-28 18:14:21.963877 fluxional-0.1.7/fluxional/utils.py
--rw-r--r--   0        0        0     1151 2024-05-15 20:00:26.002692 fluxional-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4860 1970-01-01 00:00:00.000000 fluxional-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-28 17:10:39.085356 fluxional-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3908 2024-04-29 21:12:21.619975 fluxional-0.1.8/README.md
+-rw-r--r--   0        0        0      421 2024-05-17 00:45:08.982031 fluxional-0.1.8/fluxional/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-28 18:14:21.913877 fluxional-0.1.8/fluxional/__main__.py
+-rw-r--r--   0        0        0     1429 2024-04-28 18:14:21.923877 fluxional-0.1.8/fluxional/cli/__init__.py
+-rw-r--r--   0        0        0      397 2024-04-28 18:14:21.923877 fluxional-0.1.8/fluxional/core/__init__.py
+-rw-r--r--   0        0        0    21405 2024-05-09 01:45:17.632254 fluxional-0.1.8/fluxional/core/app.py
+-rw-r--r--   0        0        0     6976 2024-04-28 18:14:21.933877 fluxional-0.1.8/fluxional/core/core.py
+-rw-r--r--   0        0        0     2927 2024-04-28 18:14:21.933877 fluxional-0.1.8/fluxional/core/events.py
+-rw-r--r--   0        0        0    11708 2024-04-28 18:14:21.943877 fluxional-0.1.8/fluxional/core/handlers.py
+-rw-r--r--   0        0        0        1 2024-04-28 18:14:21.943877 fluxional-0.1.8/fluxional/core/infrastructure/__init__.py
+-rw-r--r--   0        0        0    20142 2024-05-15 19:51:13.339223 fluxional-0.1.8/fluxional/core/infrastructure/base.py
+-rw-r--r--   0        0        0     7699 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/core/infrastructure/cdk.py
+-rw-r--r--   0        0        0     9554 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/core/infrastructure/resources.py
+-rw-r--r--   0        0        0      816 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/core/infrastructure/types.py
+-rw-r--r--   0        0        0     5818 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/core/logic.py
+-rw-r--r--   0        0        0     8343 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/core/settings.py
+-rw-r--r--   0        0        0     4045 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/core/tools.py
+-rw-r--r--   0        0        0     5158 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/core/types.py
+-rw-r--r--   0        0        0       74 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/deployment/__init__.py
+-rw-r--r--   0        0        0     1164 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/deployment/constants.py
+-rw-r--r--   0        0        0    15517 2024-04-30 22:02:31.375706 fluxional-0.1.8/fluxional/deployment/engine.py
+-rw-r--r--   0        0        0      345 2024-04-28 18:14:21.953877 fluxional-0.1.8/fluxional/deployment/exceptions.py
+-rw-r--r--   0        0        0        1 2024-04-30 22:01:04.012000 fluxional-0.1.8/fluxional/deployment/utils.py
+-rw-r--r--   0        0        0     3652 2024-04-28 18:14:21.963877 fluxional-0.1.8/fluxional/dev/__init__.py
+-rw-r--r--   0        0        0     3003 2024-04-28 18:14:21.963877 fluxional-0.1.8/fluxional/dev/client.py
+-rw-r--r--   0        0        0     3350 2024-04-28 18:14:21.963877 fluxional-0.1.8/fluxional/dev/runner.py
+-rw-r--r--   0        0        0      326 2024-04-28 18:14:21.963877 fluxional-0.1.8/fluxional/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-28 18:14:21.963877 fluxional-0.1.8/fluxional/py.typed
+-rw-r--r--   0        0        0      461 2024-04-28 18:14:21.963877 fluxional-0.1.8/fluxional/types.py
+-rw-r--r--   0        0        0      935 2024-04-28 18:14:21.963877 fluxional-0.1.8/fluxional/utils.py
+-rw-r--r--   0        0        0     1152 2024-05-17 00:45:30.382028 fluxional-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 fluxional-0.1.8/PKG-INFO
```

### Comparing `fluxional-0.1.7/LICENSE` & `fluxional-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/README.md` & `fluxional-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/cli/__init__.py` & `fluxional-0.1.8/fluxional/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/core/app.py` & `fluxional-0.1.8/fluxional/core/app.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/core/core.py` & `fluxional-0.1.8/fluxional/core/core.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/core/events.py` & `fluxional-0.1.8/fluxional/core/events.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/core/handlers.py` & `fluxional-0.1.8/fluxional/core/handlers.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/core/infrastructure/base.py` & `fluxional-0.1.8/fluxional/core/infrastructure/base.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/core/infrastructure/cdk.py` & `fluxional-0.1.8/fluxional/core/infrastructure/cdk.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/core/infrastructure/resources.py` & `fluxional-0.1.8/fluxional/core/infrastructure/resources.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/core/infrastructure/types.py` & `fluxional-0.1.8/fluxional/core/infrastructure/types.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/core/logic.py` & `fluxional-0.1.8/fluxional/core/logic.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/core/settings.py` & `fluxional-0.1.8/fluxional/core/settings.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/core/tools.py` & `fluxional-0.1.8/fluxional/core/tools.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/core/types.py` & `fluxional-0.1.8/fluxional/core/types.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/deployment/constants.py` & `fluxional-0.1.8/fluxional/deployment/constants.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/deployment/engine.py` & `fluxional-0.1.8/fluxional/deployment/engine.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/dev/__init__.py` & `fluxional-0.1.8/fluxional/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/dev/client.py` & `fluxional-0.1.8/fluxional/dev/client.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/dev/runner.py` & `fluxional-0.1.8/fluxional/dev/runner.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/fluxional/utils.py` & `fluxional-0.1.8/fluxional/utils.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.7/pyproject.toml` & `fluxional-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "fluxional"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["fluxional"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">= 3.10 < 4.0"
 boto3 = "^1.29.6"
 python-dotenv = "^1.0.0"
 aws-cdk-lib = {version = "2.114.1", optional = true}
 aws-cdk-aws-apigatewayv2-integrations-alpha = {version = "2.114.1a0", optional = true}
 awscrt = {version = "^0.20.0", optional = true}
 awsiotsdk = {version = "^1.20.0", optional = true}
 docker = "6.1.3"
-typer = "^0.9.0"
+typer = ">=0.9.0"
 rich = "^13.7.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.10.0"
 pytest = "^7.4.2"
 ruff = "^0.1.1"
 coverage = "^7.3.2"
```

### Comparing `fluxional-0.1.7/PKG-INFO` & `fluxional-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxional
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 License: MIT
 Author: fluxional
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -16,15 +16,15 @@
 Requires-Dist: aws-cdk-lib (==2.114.1) ; extra == "all"
 Requires-Dist: awscrt (>=0.20.0,<0.21.0) ; extra == "all" or extra == "dev"
 Requires-Dist: awsiotsdk (>=1.20.0,<2.0.0) ; extra == "all" or extra == "dev"
 Requires-Dist: boto3 (>=1.29.6,<2.0.0)
 Requires-Dist: docker (==6.1.3)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: typer (>=0.9.0)
 Description-Content-Type: text/markdown
 
 # 🚀 AWS Serverless Development All In Python 🐍
 
 #### This is a work in progress. If you have any questions or need help, please reach out to us.
 
 <u>Join our discord community and give us feedback or ask questions:</u>
```

