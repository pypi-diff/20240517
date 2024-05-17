# Comparing `tmp/aws-cdk.aws-pipes-alpha-2.141.0a0.tar.gz` & `tmp/aws-cdk.aws-pipes-alpha-2.142.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cdk.aws-pipes-alpha-2.141.0a0.tar", last modified: Wed May  8 21:37:00 2024, max compression
+gzip compressed data, was "aws-cdk.aws-pipes-alpha-2.142.0a0.tar", last modified: Wed May 15 21:55:15 2024, max compression
```

## Comparing `aws-cdk.aws-pipes-alpha-2.141.0a0.tar` & `aws-cdk.aws-pipes-alpha-2.142.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:37:00.902417 aws-cdk.aws-pipes-alpha-2.141.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2024-05-08 21:36:41.000000 aws-cdk.aws-pipes-alpha-2.141.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-08 21:36:41.000000 aws-cdk.aws-pipes-alpha-2.141.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2024-05-08 21:36:41.000000 aws-cdk.aws-pipes-alpha-2.141.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    17014 2024-05-08 21:37:00.902417 aws-cdk.aws-pipes-alpha-2.141.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16052 2024-05-08 21:36:41.000000 aws-cdk.aws-pipes-alpha-2.141.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-05-08 21:36:41.000000 aws-cdk.aws-pipes-alpha-2.141.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 21:37:00.902417 aws-cdk.aws-pipes-alpha-2.141.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1832 2024-05-08 21:36:41.000000 aws-cdk.aws-pipes-alpha-2.141.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:37:00.902417 aws-cdk.aws-pipes-alpha-2.141.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:37:00.902417 aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:37:00.902417 aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk/aws_pipes_alpha/
--rw-r--r--   0 root         (0) root         (0)   128563 2024-05-08 21:36:41.000000 aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk/aws_pipes_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:37:00.902417 aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk/aws_pipes_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      515 2024-05-08 21:36:41.000000 aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk/aws_pipes_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77638 2024-05-08 21:36:41.000000 aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk/aws_pipes_alpha/_jsii/aws-pipes-alpha@2.141.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 21:36:41.000000 aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk/aws_pipes_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:37:00.902417 aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk.aws_pipes_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17014 2024-05-08 21:37:00.000000 aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk.aws_pipes_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      512 2024-05-08 21:37:00.000000 aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk.aws_pipes_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 21:37:00.000000 aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk.aws_pipes_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2024-05-08 21:37:00.000000 aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk.aws_pipes_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-08 21:37:00.000000 aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk.aws_pipes_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:55:15.033234 aws-cdk.aws-pipes-alpha-2.142.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2024-05-15 21:54:58.000000 aws-cdk.aws-pipes-alpha-2.142.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-15 21:54:58.000000 aws-cdk.aws-pipes-alpha-2.142.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2024-05-15 21:54:58.000000 aws-cdk.aws-pipes-alpha-2.142.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    17014 2024-05-15 21:55:15.033234 aws-cdk.aws-pipes-alpha-2.142.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16052 2024-05-15 21:54:58.000000 aws-cdk.aws-pipes-alpha-2.142.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-05-15 21:54:58.000000 aws-cdk.aws-pipes-alpha-2.142.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 21:55:15.033234 aws-cdk.aws-pipes-alpha-2.142.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-05-15 21:54:58.000000 aws-cdk.aws-pipes-alpha-2.142.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:55:15.033234 aws-cdk.aws-pipes-alpha-2.142.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:55:15.033234 aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:55:15.033234 aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk/aws_pipes_alpha/
+-rw-r--r--   0 root         (0) root         (0)   128547 2024-05-15 21:54:58.000000 aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk/aws_pipes_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:55:15.033234 aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk/aws_pipes_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      515 2024-05-15 21:54:58.000000 aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk/aws_pipes_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77728 2024-05-15 21:54:58.000000 aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk/aws_pipes_alpha/_jsii/aws-pipes-alpha@2.142.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 21:54:58.000000 aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk/aws_pipes_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:55:15.033234 aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk.aws_pipes_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17014 2024-05-15 21:55:14.000000 aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk.aws_pipes_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      512 2024-05-15 21:55:15.000000 aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk.aws_pipes_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 21:55:14.000000 aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk.aws_pipes_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2024-05-15 21:55:14.000000 aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk.aws_pipes_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-15 21:55:14.000000 aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk.aws_pipes_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-pipes-alpha-2.141.0a0/LICENSE` & `aws-cdk.aws-pipes-alpha-2.142.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-pipes-alpha-2.141.0a0/PKG-INFO` & `aws-cdk.aws-pipes-alpha-2.142.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-pipes-alpha
-Version: 2.141.0a0
+Version: 2.142.0a0
 Summary: The CDK Construct Library for Amazon EventBridge Pipes
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-pipes-alpha-2.141.0a0/README.md` & `aws-cdk.aws-pipes-alpha-2.142.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-pipes-alpha-2.141.0a0/setup.py` & `aws-cdk.aws-pipes-alpha-2.142.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-pipes-alpha",
-    "version": "2.141.0.a0",
+    "version": "2.142.0.a0",
     "description": "The CDK Construct Library for Amazon EventBridge Pipes",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_cdk.aws_pipes_alpha",
         "aws_cdk.aws_pipes_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_pipes_alpha._jsii": [
-            "aws-pipes-alpha@2.141.0-alpha.0.jsii.tgz"
+            "aws-pipes-alpha@2.142.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_pipes_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.141.0, <3.0.0",
+        "aws-cdk-lib>=2.142.0, <3.0.0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk/aws_pipes_alpha/__init__.py` & `aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk/aws_pipes_alpha/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1435,21 +1435,20 @@
 
     :stability: experimental
     :exampleMetadata: infused
 
     Example::
 
         # source_queue: sqs.Queue
-        # target_queue: sqs.Queue
+        # target_state_machine: sfn.IStateMachine
         
         
-        pipe_target = targets.SqsTarget(target_queue,
-            input_transformation=pipes.InputTransformation.from_object({
-                "SomeKey": pipes.DynamicInput.from_event_path("$.body")
-            })
+        pipe_target = targets.SfnStateMachine(target_state_machine,
+            input_transformation=pipes.InputTransformation.from_object({"body": "<$.body>"}),
+            invocation_type=targets.StateMachineInvocationType.FIRE_AND_FORGET
         )
         
         pipe = pipes.Pipe(self, "Pipe",
             source=SomeSource(source_queue),
             target=pipe_target
         )
     '''
@@ -2467,21 +2466,19 @@
         :see: https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-pipes-event-source.html
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
             # source_queue: sqs.Queue
-            # target_queue: sqs.Queue
+            # target_state_machine: sfn.IStateMachine
             
             
-            pipe_target = targets.SqsTarget(target_queue,
-                input_transformation=pipes.InputTransformation.from_object({
-                    "SomeKey": pipes.DynamicInput.from_event_path("$.body")
-                })
+            pipe_target = targets.SfnStateMachine(target_state_machine,
+                invocation_type=targets.StateMachineInvocationType.FIRE_AND_FORGET
             )
             
             pipe = pipes.Pipe(self, "Pipe",
                 source=SomeSource(source_queue),
                 target=pipe_target
             )
         '''
```

### Comparing `aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk/aws_pipes_alpha/_jsii/__init__.py` & `aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk/aws_pipes_alpha/_jsii/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@aws-cdk/aws-pipes-alpha",
-    "2.141.0-alpha.0",
+    "2.142.0-alpha.0",
     __name__[0:-6],
-    "aws-pipes-alpha@2.141.0-alpha.0.jsii.tgz",
+    "aws-pipes-alpha@2.142.0-alpha.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk.aws_pipes_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk.aws_pipes_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-pipes-alpha
-Version: 2.141.0a0
+Version: 2.142.0a0
 Summary: The CDK Construct Library for Amazon EventBridge Pipes
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-pipes-alpha-2.141.0a0/src/aws_cdk.aws_pipes_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-pipes-alpha-2.142.0a0/src/aws_cdk.aws_pipes_alpha.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_pipes_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_pipes_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_pipes_alpha.egg-info/requires.txt
 src/aws_cdk.aws_pipes_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_pipes_alpha/__init__.py
 src/aws_cdk/aws_pipes_alpha/py.typed
 src/aws_cdk/aws_pipes_alpha/_jsii/__init__.py
-src/aws_cdk/aws_pipes_alpha/_jsii/aws-pipes-alpha@2.141.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_pipes_alpha/_jsii/aws-pipes-alpha@2.142.0-alpha.0.jsii.tgz
```

