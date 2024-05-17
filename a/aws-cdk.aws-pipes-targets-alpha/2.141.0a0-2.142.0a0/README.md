# Comparing `tmp/aws-cdk.aws-pipes-targets-alpha-2.141.0a0.tar.gz` & `tmp/aws-cdk.aws-pipes-targets-alpha-2.142.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cdk.aws-pipes-targets-alpha-2.141.0a0.tar", last modified: Wed May  8 21:37:19 2024, max compression
+gzip compressed data, was "aws-cdk.aws-pipes-targets-alpha-2.142.0a0.tar", last modified: Wed May 15 21:55:37 2024, max compression
```

## Comparing `aws-cdk.aws-pipes-targets-alpha-2.141.0a0.tar` & `aws-cdk.aws-pipes-targets-alpha-2.142.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:37:19.554332 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2024-05-08 21:37:09.000000 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-08 21:37:09.000000 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2024-05-08 21:37:09.000000 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     2698 2024-05-08 21:37:19.550332 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1720 2024-05-08 21:37:09.000000 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-05-08 21:37:09.000000 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 21:37:19.554332 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1935 2024-05-08 21:37:09.000000 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:37:19.550332 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:37:19.550332 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:37:19.550332 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/src/aws_cdk/aws_pipes_targets_alpha/
--rw-r--r--   0 root         (0) root         (0)    11967 2024-05-08 21:37:09.000000 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/src/aws_cdk/aws_pipes_targets_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:37:19.550332 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      568 2024-05-08 21:37:09.000000 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22780 2024-05-08 21:37:09.000000 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/aws-pipes-targets-alpha@2.141.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 21:37:09.000000 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/src/aws_cdk/aws_pipes_targets_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:37:19.550332 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2698 2024-05-08 21:37:19.000000 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      592 2024-05-08 21:37:19.000000 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 21:37:19.000000 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      148 2024-05-08 21:37:19.000000 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-08 21:37:19.000000 aws-cdk.aws-pipes-targets-alpha-2.141.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:55:37.329351 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2024-05-15 21:55:27.000000 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-15 21:55:27.000000 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2024-05-15 21:55:27.000000 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4149 2024-05-15 21:55:37.329351 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3171 2024-05-15 21:55:27.000000 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-05-15 21:55:27.000000 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 21:55:37.329351 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1935 2024-05-15 21:55:27.000000 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:55:37.325350 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:55:37.325350 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:55:37.325350 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/src/aws_cdk/aws_pipes_targets_alpha/
+-rw-r--r--   0 root         (0) root         (0)    23616 2024-05-15 21:55:27.000000 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/src/aws_cdk/aws_pipes_targets_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:55:37.329351 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      568 2024-05-15 21:55:27.000000 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28024 2024-05-15 21:55:27.000000 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/aws-pipes-targets-alpha@2.142.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 21:55:27.000000 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/src/aws_cdk/aws_pipes_targets_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:55:37.325350 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4149 2024-05-15 21:55:37.000000 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      592 2024-05-15 21:55:37.000000 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 21:55:37.000000 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2024-05-15 21:55:37.000000 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-15 21:55:37.000000 aws-cdk.aws-pipes-targets-alpha-2.142.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-pipes-targets-alpha-2.141.0a0/LICENSE` & `aws-cdk.aws-pipes-targets-alpha-2.142.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-pipes-targets-alpha-2.141.0a0/setup.py` & `aws-cdk.aws-pipes-targets-alpha-2.142.0a0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-pipes-targets-alpha",
-    "version": "2.141.0.a0",
+    "version": "2.142.0.a0",
     "description": "The CDK Construct Library for Amazon EventBridge Pipes Targets",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "aws_cdk.aws_pipes_targets_alpha",
         "aws_cdk.aws_pipes_targets_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_pipes_targets_alpha._jsii": [
-            "aws-pipes-targets-alpha@2.141.0-alpha.0.jsii.tgz"
+            "aws-pipes-targets-alpha@2.142.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_pipes_targets_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.141.0, <3.0.0",
-        "aws-cdk.aws-pipes-alpha==2.141.0.a0",
+        "aws-cdk-lib>=2.142.0, <3.0.0",
+        "aws-cdk.aws-pipes-alpha==2.142.0.a0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.aws-pipes-targets-alpha-2.141.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/__init__.py` & `aws-cdk.aws-pipes-targets-alpha-2.142.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import aws_cdk.aws_pipes_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@aws-cdk/aws-pipes-targets-alpha",
-    "2.141.0-alpha.0",
+    "2.142.0-alpha.0",
     __name__[0:-6],
-    "aws-pipes-targets-alpha@2.141.0-alpha.0.jsii.tgz",
+    "aws-pipes-targets-alpha@2.142.0-alpha.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-cdk.aws-pipes-targets-alpha-2.141.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-pipes-targets-alpha-2.142.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_pipes_targets_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_pipes_targets_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_pipes_targets_alpha.egg-info/requires.txt
 src/aws_cdk.aws_pipes_targets_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_pipes_targets_alpha/__init__.py
 src/aws_cdk/aws_pipes_targets_alpha/py.typed
 src/aws_cdk/aws_pipes_targets_alpha/_jsii/__init__.py
-src/aws_cdk/aws_pipes_targets_alpha/_jsii/aws-pipes-targets-alpha@2.141.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_pipes_targets_alpha/_jsii/aws-pipes-targets-alpha@2.142.0-alpha.0.jsii.tgz
```
