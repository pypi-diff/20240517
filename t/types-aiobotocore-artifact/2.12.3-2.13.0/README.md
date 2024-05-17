# Comparing `tmp/types-aiobotocore-artifact-2.12.3.tar.gz` & `tmp/types_aiobotocore_artifact-2.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-artifact-2.12.3.tar", last modified: Fri Apr 12 01:16:54 2024, max compression
+gzip compressed data, was "types_aiobotocore_artifact-2.13.0.tar", last modified: Fri May 17 01:21:51 2024, max compression
```

## Comparing `types-aiobotocore-artifact-2.12.3.tar` & `types_aiobotocore_artifact-2.13.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:16:54.689356 types-aiobotocore-artifact-2.12.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 01:00:48.000000 types-aiobotocore-artifact-2.12.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-04-12 01:16:54.689356 types-aiobotocore-artifact-2.12.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-04-12 01:00:48.000000 types-aiobotocore-artifact-2.12.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 01:16:54.689356 types-aiobotocore-artifact-2.12.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-12 01:00:48.000000 types-aiobotocore-artifact-2.12.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:16:54.689356 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-12 01:00:48.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-12 01:00:48.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-12 01:00:48.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-12 01:00:48.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-04-12 01:00:48.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-04-12 01:00:48.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-04-12 01:00:48.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-12 01:00:48.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-12 01:00:48.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 01:00:48.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-12 01:00:49.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-12 01:00:49.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 01:00:48.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:16:54.689356 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-04-12 01:16:54.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-12 01:16:54.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:16:54.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:16:54.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 01:16:54.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 01:16:54.000000 types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:51.827122 types_aiobotocore_artifact-2.13.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-17 01:04:16.000000 types_aiobotocore_artifact-2.13.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-05-17 01:21:51.827122 types_aiobotocore_artifact-2.13.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-05-17 01:04:16.000000 types_aiobotocore_artifact-2.13.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 01:21:51.827122 types_aiobotocore_artifact-2.13.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-17 01:04:15.000000 types_aiobotocore_artifact-2.13.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:51.827122 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-17 01:04:16.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-17 01:04:16.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-17 01:04:16.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-05-17 01:04:16.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-05-17 01:04:16.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-05-17 01:04:16.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-05-17 01:04:16.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-17 01:04:16.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-17 01:04:16.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 01:04:16.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-17 01:04:16.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-17 01:04:16.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-17 01:04:16.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:51.827122 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-05-17 01:21:51.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-17 01:21:51.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 01:21:51.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 01:21:51.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-17 01:21:51.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 01:21:51.000000 types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-artifact-2.12.3/LICENSE` & `types_aiobotocore_artifact-2.13.0/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.3/PKG-INFO` & `types_aiobotocore_artifact-2.13.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-artifact
-Version: 2.12.3
-Summary: Type annotations for aiobotocore.Artifact 2.12.3 service generated with mypy-boto3-builder 7.23.2
+Version: 2.13.0
+Summary: Type annotations for aiobotocore.Artifact 2.13.0 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_artifact/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-artifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-artifact)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_artifact/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-artifact)](https://pepy.tech/project/types-aiobotocore-artifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Artifact 2.12.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
+[aiobotocore.Artifact 2.13.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-artifact docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_artifact/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-artifact-2.12.3/README.md` & `types_aiobotocore_artifact-2.13.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-artifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-artifact)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_artifact/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-artifact)](https://pepy.tech/project/types-aiobotocore-artifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Artifact 2.12.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
+[aiobotocore.Artifact 2.13.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-artifact docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_artifact/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-artifact-2.12.3/setup.py` & `types_aiobotocore_artifact-2.13.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-artifact",
-    version="2.12.3",
+    version="2.13.0",
     packages=["types_aiobotocore_artifact"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for aiobotocore.Artifact 2.12.3 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for aiobotocore.Artifact 2.13.0 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

### Comparing `types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/__init__.py` & `types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/__init__.pyi` & `types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/__main__.py` & `types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Artifact 2.12.3\n"
-        "Version:         2.12.3\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for aiobotocore.Artifact 2.13.0\n"
+        "Version:         2.13.0\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_artifact//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.12.3")
+    print("2.13.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/client.py` & `types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/client.pyi` & `types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/literals.py` & `types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -124,24 +125,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -338,14 +341,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/literals.pyi` & `types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -124,24 +125,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -338,14 +341,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/paginator.py` & `types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/paginator.pyi` & `types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/type_defs.py` & `types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact/type_defs.pyi` & `types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact.egg-info/PKG-INFO` & `types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-artifact
-Version: 2.12.3
-Summary: Type annotations for aiobotocore.Artifact 2.12.3 service generated with mypy-boto3-builder 7.23.2
+Version: 2.13.0
+Summary: Type annotations for aiobotocore.Artifact 2.13.0 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_artifact/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-artifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-artifact)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_artifact/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-artifact)](https://pepy.tech/project/types-aiobotocore-artifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Artifact 2.12.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
+[aiobotocore.Artifact 2.13.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-artifact docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_artifact/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-artifact-2.12.3/types_aiobotocore_artifact.egg-info/SOURCES.txt` & `types_aiobotocore_artifact-2.13.0/types_aiobotocore_artifact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

