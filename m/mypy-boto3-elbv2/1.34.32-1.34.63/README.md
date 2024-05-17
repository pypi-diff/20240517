# Comparing `tmp/mypy-boto3-elbv2-1.34.32.tar.gz` & `tmp/mypy-boto3-elbv2-1.34.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elbv2-1.34.32.tar", last modified: Wed Jan 31 20:32:21 2024, max compression
+gzip compressed data, was "mypy-boto3-elbv2-1.34.63.tar", last modified: Thu Mar 14 19:19:06 2024, max compression
```

## Comparing `mypy-boto3-elbv2-1.34.32.tar` & `mypy-boto3-elbv2-1.34.63.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 20:32:21.829901 mypy-boto3-elbv2-1.34.32/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-31 20:31:50.000000 mypy-boto3-elbv2-1.34.32/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14918 2024-01-31 20:32:21.829901 mypy-boto3-elbv2-1.34.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-01-31 20:31:50.000000 mypy-boto3-elbv2-1.34.32/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 20:32:21.829901 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-01-31 20:31:50.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-01-31 20:31:50.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-01-31 20:31:50.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41662 2024-01-31 20:31:51.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    41659 2024-01-31 20:31:50.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-01-31 20:31:51.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-01-31 20:31:51.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-01-31 20:31:51.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-01-31 20:31:51.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 20:31:50.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    48995 2024-01-31 20:31:52.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    48995 2024-01-31 20:31:51.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-31 20:31:50.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-01-31 20:31:51.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-01-31 20:31:51.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 20:32:21.829901 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14918 2024-01-31 20:32:21.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-31 20:32:21.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 20:32:21.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 20:32:21.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-31 20:32:21.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-31 20:32:21.000000 mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 20:32:21.829901 mypy-boto3-elbv2-1.34.32/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-01-31 20:31:50.000000 mypy-boto3-elbv2-1.34.32/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:19:06.894544 mypy-boto3-elbv2-1.34.63/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-14 19:18:39.000000 mypy-boto3-elbv2-1.34.63/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14918 2024-03-14 19:19:06.894544 mypy-boto3-elbv2-1.34.63/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-03-14 19:18:39.000000 mypy-boto3-elbv2-1.34.63/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:19:06.890544 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-03-14 19:18:39.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-03-14 19:18:39.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-14 19:18:39.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41662 2024-03-14 19:18:39.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41659 2024-03-14 19:18:39.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12954 2024-03-14 19:18:40.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12954 2024-03-14 19:18:40.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-03-14 19:18:39.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-03-14 19:18:39.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 19:18:39.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    49008 2024-03-14 19:18:41.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49008 2024-03-14 19:18:40.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-14 19:18:39.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-03-14 19:18:40.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-03-14 19:18:39.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:19:06.890544 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14918 2024-03-14 19:19:06.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-14 19:19:06.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 19:19:06.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 19:19:06.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-14 19:19:06.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-14 19:19:06.000000 mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 19:19:06.894544 mypy-boto3-elbv2-1.34.63/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-03-14 19:18:39.000000 mypy-boto3-elbv2-1.34.63/setup.py
```

### Comparing `mypy-boto3-elbv2-1.34.32/LICENSE` & `mypy-boto3-elbv2-1.34.63/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.34.32/PKG-INFO` & `mypy-boto3-elbv2-1.34.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elbv2
-Version: 1.34.32
-Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.34.32 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.63
+Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.34.63 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elbv2)](https://pepy.tech/project/mypy-boto3-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancingv2 1.34.32](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[boto3.ElasticLoadBalancingv2 1.34.63](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-elbv2-1.34.32/README.md` & `mypy-boto3-elbv2-1.34.63/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elbv2)](https://pepy.tech/project/mypy-boto3-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancingv2 1.34.32](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[boto3.ElasticLoadBalancingv2 1.34.63](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/__init__.py` & `mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/__init__.pyi` & `mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/__main__.py` & `mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticLoadBalancingv2 1.34.32\n"
-        "Version:         1.34.32\n"
-        "Builder version: 7.23.1\n"
+        "Type annotations for boto3.ElasticLoadBalancingv2 1.34.63\n"
+        "Version:         1.34.63\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.32")
+    print("1.34.63")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/client.py` & `mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/client.pyi` & `mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/literals.py` & `mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -148,14 +149,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -271,15 +273,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -459,14 +460,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/literals.pyi` & `mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -148,14 +149,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -271,15 +273,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -459,14 +460,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/paginator.py` & `mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/paginator.pyi` & `mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/type_defs.py` & `mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,18 +294,18 @@
         "IsDefault": NotRequired[bool],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": NotRequired[str],
```

### Comparing `mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/type_defs.pyi` & `mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -294,18 +294,18 @@
         "IsDefault": NotRequired[bool],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": NotRequired[str],
```

### Comparing `mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/waiter.py` & `mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2/waiter.pyi` & `mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2.egg-info/PKG-INFO` & `mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elbv2
-Version: 1.34.32
-Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.34.32 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.63
+Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.34.63 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elbv2)](https://pepy.tech/project/mypy-boto3-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancingv2 1.34.32](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[boto3.ElasticLoadBalancingv2 1.34.63](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-elbv2-1.34.32/mypy_boto3_elbv2.egg-info/SOURCES.txt` & `mypy-boto3-elbv2-1.34.63/mypy_boto3_elbv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.34.32/setup.py` & `mypy-boto3-elbv2-1.34.63/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elbv2",
-    version="1.34.32",
+    version="1.34.63",
     packages=["mypy_boto3_elbv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.ElasticLoadBalancingv2 1.34.32 service generated with mypy-boto3-builder 7.23.1",
+    description="Type annotations for boto3.ElasticLoadBalancingv2 1.34.63 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

