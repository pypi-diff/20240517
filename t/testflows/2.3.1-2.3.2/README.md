# Comparing `tmp/testflows-2.3.1.tar.gz` & `tmp/testflows-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows-2.3.1.tar", last modified: Wed May  8 15:01:29 2024, max compression
+gzip compressed data, was "testflows-2.3.2.tar", last modified: Fri May 17 13:30:38 2024, max compression
```

## Comparing `testflows-2.3.1.tar` & `testflows-2.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:01:29.047178 testflows-2.3.1/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2024-03-14 16:48:03.000000 testflows-2.3.1/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     2767 2024-05-08 15:01:29.047178 testflows-2.3.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2231 2024-03-14 16:48:03.000000 testflows-2.3.1/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-08 15:01:29.047178 testflows-2.3.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1758 2024-05-08 15:00:51.000000 testflows-2.3.1/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:01:29.047178 testflows-2.3.1/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:01:29.047178 testflows-2.3.1/testflows/version/
--rw-rw-r--   0 user      (1000) user      (1000)      739 2024-03-14 16:48:03.000000 testflows-2.3.1/testflows/version/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:01:29.047178 testflows-2.3.1/testflows.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     2767 2024-05-08 15:01:29.000000 testflows-2.3.1/testflows.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      252 2024-05-08 15:01:29.000000 testflows-2.3.1/testflows.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-08 15:01:29.000000 testflows-2.3.1/testflows.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-08 15:01:29.000000 testflows-2.3.1/testflows.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)      231 2024-05-08 15:01:29.000000 testflows-2.3.1/testflows.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2024-05-08 15:01:29.000000 testflows-2.3.1/testflows.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-17 13:30:38.150912 testflows-2.3.2/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2024-03-14 16:48:03.000000 testflows-2.3.2/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     2767 2024-05-17 13:30:38.150912 testflows-2.3.2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2231 2024-03-14 16:48:03.000000 testflows-2.3.2/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-17 13:30:38.150912 testflows-2.3.2/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1758 2024-05-17 13:29:48.000000 testflows-2.3.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-17 13:30:38.150912 testflows-2.3.2/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-17 13:30:38.150912 testflows-2.3.2/testflows/version/
+-rw-rw-r--   0 user      (1000) user      (1000)      739 2024-03-14 16:48:03.000000 testflows-2.3.2/testflows/version/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-17 13:30:38.150912 testflows-2.3.2/testflows.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2767 2024-05-17 13:30:38.000000 testflows-2.3.2/testflows.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      252 2024-05-17 13:30:38.000000 testflows-2.3.2/testflows.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-17 13:30:38.000000 testflows-2.3.2/testflows.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-08 15:01:29.000000 testflows-2.3.2/testflows.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)      231 2024-05-17 13:30:38.000000 testflows-2.3.2/testflows.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2024-05-17 13:30:38.000000 testflows-2.3.2/testflows.egg-info/top_level.txt
```

### Comparing `testflows-2.3.1/LICENSE` & `testflows-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows-2.3.1/PKG-INFO` & `testflows-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows
-Version: 2.3.1
+Version: 2.3.2
 Summary: TestFlows.com Open-Source Software Testing Framework
 Home-page: https://github.com/testflows/testflows
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows-2.3.1/README.md` & `testflows-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `testflows-2.3.1/setup.py` & `testflows-2.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setup(
     name="testflows",
-    version="2.3.1",
+    version="2.3.2",
     description="TestFlows.com Open-Source Software Testing Framework",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/testflows/testflows",
     classifiers=[
@@ -32,15 +32,15 @@
         "Operating System :: POSIX :: Linux",
     ],
     python_requires=">=3.8",
     license="Apache-2.0",
     packages=["testflows.version"],
     zip_safe=False,
     install_requires=[
-        "testflows.core==2.0.240508.1150015",
+        "testflows.core==2.0.240517.1132809",
         "testflows.asserts==7.0.231001.1010150",
         "testflows.stash==1.1.230317.1211113",
         "testflows.uexpect==1.7.230414.1210501",
         "testflows.connect==1.7.230414.1210340",
         "testflows.database==1.6.200713.1142213",
     ],
     extras_require={"dev": []},
```

### Comparing `testflows-2.3.1/testflows/version/__init__.py` & `testflows-2.3.2/testflows/version/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows-2.3.1/testflows.egg-info/PKG-INFO` & `testflows-2.3.2/testflows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows
-Version: 2.3.1
+Version: 2.3.2
 Summary: TestFlows.com Open-Source Software Testing Framework
 Home-page: https://github.com/testflows/testflows
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

