# Comparing `tmp/REMLA-Test-Lib-version-0.0.8.tar.gz` & `tmp/REMLA-Test-Lib-version-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "REMLA-Test-Lib-version-0.0.8.tar", last modified: Fri May 17 09:58:47 2024, max compression
+gzip compressed data, was "REMLA-Test-Lib-version-0.1.0.tar", last modified: Sat May 11 14:06:13 2024, max compression
```

## Comparing `REMLA-Test-Lib-version-0.0.8.tar` & `REMLA-Test-Lib-version-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:58:47.519211 REMLA-Test-Lib-version-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-17 09:58:46.000000 REMLA-Test-Lib-version-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-17 09:58:47.519211 REMLA-Test-Lib-version-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-17 09:58:46.000000 REMLA-Test-Lib-version-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:58:47.519211 REMLA-Test-Lib-version-0.0.8/REMLA_Test_Lib_version/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 09:58:46.000000 REMLA-Test-Lib-version-0.0.8/REMLA_Test_Lib_version/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-17 09:58:46.000000 REMLA-Test-Lib-version-0.0.8/REMLA_Test_Lib_version/VersionUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-17 09:58:46.000000 REMLA-Test-Lib-version-0.0.8/REMLA_Test_Lib_version/VersionUtil2.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:58:46.000000 REMLA-Test-Lib-version-0.0.8/REMLA_Test_Lib_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:58:47.519211 REMLA-Test-Lib-version-0.0.8/REMLA_Test_Lib_version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-17 09:58:47.000000 REMLA-Test-Lib-version-0.0.8/REMLA_Test_Lib_version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-17 09:58:47.000000 REMLA-Test-Lib-version-0.0.8/REMLA_Test_Lib_version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:58:47.000000 REMLA-Test-Lib-version-0.0.8/REMLA_Test_Lib_version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 09:58:47.000000 REMLA-Test-Lib-version-0.0.8/REMLA_Test_Lib_version.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:58:47.519211 REMLA-Test-Lib-version-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-17 09:58:46.000000 REMLA-Test-Lib-version-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:06:13.601704 REMLA-Test-Lib-version-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-11 14:06:12.000000 REMLA-Test-Lib-version-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-11 14:06:13.601704 REMLA-Test-Lib-version-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-11 14:06:12.000000 REMLA-Test-Lib-version-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:06:13.601704 REMLA-Test-Lib-version-0.1.0/REMLA_Test_Lib_version.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-11 14:06:13.000000 REMLA-Test-Lib-version-0.1.0/REMLA_Test_Lib_version.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-11 14:06:13.000000 REMLA-Test-Lib-version-0.1.0/REMLA_Test_Lib_version.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 14:06:13.000000 REMLA-Test-Lib-version-0.1.0/REMLA_Test_Lib_version.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 14:06:13.000000 REMLA-Test-Lib-version-0.1.0/REMLA_Test_Lib_version.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 14:06:13.601704 REMLA-Test-Lib-version-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-11 14:06:12.000000 REMLA-Test-Lib-version-0.1.0/setup.py
```

### Comparing `REMLA-Test-Lib-version-0.0.8/LICENSE` & `REMLA-Test-Lib-version-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `REMLA-Test-Lib-version-0.0.8/PKG-INFO` & `REMLA-Test-Lib-version-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: REMLA-Test-Lib-version
-Version: 0.0.8
+Version: 0.1.0
 Summary: A version-aware library designed to provide robust version management and utility functions
 Home-page: UNKNOWN
 Author: Nick Dubbeldam
 Author-email: nick.dubbeldasm@live.nl
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# LIB-VERSION
+\n# LIB-VERSION
 
 LIB-VERSION is a version-aware library designed to provide robust version management and utility functions. This library is ideal for projects requiring precise version tracking, such as in detailed logging or system monitoring environments.
 
 ## Features
 
 - **Version Retrieval**: Easily retrieve the current library version using the `VersionUtil` class.
 - **Automatic Versioning**: Utilizes Git tags to automatically version the library.
@@ -26,31 +26,32 @@
 
 ## Getting Started
 
 ### Prerequisites
 
 - Git (for versioning)
 - Python 3.x (if using Python)
-- Access to a package registry pip
+- Access to a package registry (e.g., PyPI, npm)
 
 ### Installation
 
 To install Library Name, use the following command:
 
 ```bash
-pip install REMLA-Test-Lib-version
+pip install lib-version
 ```
 
+Replace pip with the package manager relevant to your programming language or environment.
 
 ### Usage
 To retrieve the current version of the library:
 
 ```python
-from REMLA_Test_Lib_version import VersionUtil
-print(VersionUtil.VersionUtil.get_version())
+from version_util import VersionUtil
+print(VersionUtil.get_version())
 ```
 
 ### How Versioning Works
 The library's version is determined by Git tags. When a new tag is pushed to the repository, a CI/CD pipeline updates a VERSION file in the repository with the current tag. This version is then read by the VersionUtil class.
 
 ### Setting up Git Tags
 To create a new version, tag your commit with the version number:
```

### Comparing `REMLA-Test-Lib-version-0.0.8/README.md` & `REMLA-Test-Lib-version-0.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -10,31 +10,32 @@
 
 ## Getting Started
 
 ### Prerequisites
 
 - Git (for versioning)
 - Python 3.x (if using Python)
-- Access to a package registry pip
+- Access to a package registry (e.g., PyPI, npm)
 
 ### Installation
 
 To install Library Name, use the following command:
 
 ```bash
-pip install REMLA-Test-Lib-version
+pip install lib-version
 ```
 
+Replace pip with the package manager relevant to your programming language or environment.
 
 ### Usage
 To retrieve the current version of the library:
 
 ```python
-from REMLA_Test_Lib_version import VersionUtil
-print(VersionUtil.VersionUtil.get_version())
+from version_util import VersionUtil
+print(VersionUtil.get_version())
 ```
 
 ### How Versioning Works
 The library's version is determined by Git tags. When a new tag is pushed to the repository, a CI/CD pipeline updates a VERSION file in the repository with the current tag. This version is then read by the VersionUtil class.
 
 ### Setting up Git Tags
 To create a new version, tag your commit with the version number:
```

### Comparing `REMLA-Test-Lib-version-0.0.8/REMLA_Test_Lib_version.egg-info/PKG-INFO` & `REMLA-Test-Lib-version-0.1.0/REMLA_Test_Lib_version.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: REMLA-Test-Lib-version
-Version: 0.0.8
+Version: 0.1.0
 Summary: A version-aware library designed to provide robust version management and utility functions
 Home-page: UNKNOWN
 Author: Nick Dubbeldam
 Author-email: nick.dubbeldasm@live.nl
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# LIB-VERSION
+\n# LIB-VERSION
 
 LIB-VERSION is a version-aware library designed to provide robust version management and utility functions. This library is ideal for projects requiring precise version tracking, such as in detailed logging or system monitoring environments.
 
 ## Features
 
 - **Version Retrieval**: Easily retrieve the current library version using the `VersionUtil` class.
 - **Automatic Versioning**: Utilizes Git tags to automatically version the library.
@@ -26,31 +26,32 @@
 
 ## Getting Started
 
 ### Prerequisites
 
 - Git (for versioning)
 - Python 3.x (if using Python)
-- Access to a package registry pip
+- Access to a package registry (e.g., PyPI, npm)
 
 ### Installation
 
 To install Library Name, use the following command:
 
 ```bash
-pip install REMLA-Test-Lib-version
+pip install lib-version
 ```
 
+Replace pip with the package manager relevant to your programming language or environment.
 
 ### Usage
 To retrieve the current version of the library:
 
 ```python
-from REMLA_Test_Lib_version import VersionUtil
-print(VersionUtil.VersionUtil.get_version())
+from version_util import VersionUtil
+print(VersionUtil.get_version())
 ```
 
 ### How Versioning Works
 The library's version is determined by Git tags. When a new tag is pushed to the repository, a CI/CD pipeline updates a VERSION file in the repository with the current tag. This version is then read by the VersionUtil class.
 
 ### Setting up Git Tags
 To create a new version, tag your commit with the version number:
```

### Comparing `REMLA-Test-Lib-version-0.0.8/setup.py` & `REMLA-Test-Lib-version-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from setuptools import setup, find_packages
 
 # Read version from the VERSION file
-with open('REMLA_Test_Lib_version/VERSION', 'r') as version_file:
+with open('VERSION', 'r') as version_file:
     version = version_file.read().strip()
 
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-    # long_description = "\\n" + fh.read()
-    long_description = fh.read()
+    long_description = "\\n" + fh.read()
 
 setup(
 name='REMLA-Test-Lib-version',
 version=version,
 author='Nick Dubbeldam',
 author_email='nick.dubbeldasm@live.nl',
 description='A version-aware library designed to provide robust version management and utility functions',
@@ -24,10 +23,8 @@
 packages=find_packages(),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
 'Operating System :: OS Independent',
 ],
 python_requires='>=3.6',
-package_data={'': ['VERSION']},
-include_package_data=True,
 )
```

