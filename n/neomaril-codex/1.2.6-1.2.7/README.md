# Comparing `tmp/neomaril-codex-1.2.6.tar.gz` & `tmp/neomaril-codex-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neomaril-codex-1.2.6.tar", last modified: Thu Feb  1 15:06:05 2024, max compression
+gzip compressed data, was "neomaril-codex-1.2.7.tar", last modified: Thu Feb  1 16:19:56 2024, max compression
```

## Comparing `neomaril-codex-1.2.6.tar` & `neomaril-codex-1.2.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2024-02-01 15:06:05.297560 neomaril-codex-1.2.6/
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1060 2023-03-06 17:55:16.000000 neomaril-codex-1.2.6/LICENSE.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       24 2023-03-13 13:54:26.000000 neomaril-codex-1.2.6/MANIFEST.in
--rw-r--r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1372 2024-02-01 15:06:05.297560 neomaril-codex-1.2.6/PKG-INFO
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      733 2024-01-17 17:28:06.000000 neomaril-codex-1.2.6/README.md
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      118 2024-01-24 18:46:38.000000 neomaril-codex-1.2.6/requirements.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       79 2024-02-01 15:06:05.301560 neomaril-codex-1.2.6/setup.cfg
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1029 2024-02-01 15:04:57.000000 neomaril-codex-1.2.6/setup.py
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2024-02-01 15:06:05.293560 neomaril-codex-1.2.6/src/
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2024-02-01 15:06:05.297560 neomaril-codex-1.2.6/src/neomaril_codex/
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-02-08 17:56:54.000000 neomaril-codex-1.2.6/src/neomaril_codex/__init__.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1221 2023-11-21 19:18:17.000000 neomaril-codex-1.2.6/src/neomaril_codex/__utils.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    13773 2023-11-09 12:39:19.000000 neomaril-codex-1.2.6/src/neomaril_codex/base.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      858 2023-08-09 19:49:20.000000 neomaril-codex-1.2.6/src/neomaril_codex/exceptions.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     4487 2023-03-06 17:39:34.000000 neomaril-codex-1.2.6/src/neomaril_codex/logging.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    46079 2024-02-01 15:04:26.000000 neomaril-codex-1.2.6/src/neomaril_codex/model.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    13163 2023-12-04 20:06:58.000000 neomaril-codex-1.2.6/src/neomaril_codex/pipeline.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    35563 2024-02-01 15:04:22.000000 neomaril-codex-1.2.6/src/neomaril_codex/preprocessing.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    49344 2024-02-01 15:04:08.000000 neomaril-codex-1.2.6/src/neomaril_codex/training.py
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2024-02-01 15:06:05.297560 neomaril-codex-1.2.6/src/neomaril_codex.egg-info/
--rw-r--r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1372 2024-02-01 15:06:05.000000 neomaril-codex-1.2.6/src/neomaril_codex.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      596 2024-02-01 15:06:05.000000 neomaril-codex-1.2.6/src/neomaril_codex.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2024-02-01 15:06:05.000000 neomaril-codex-1.2.6/src/neomaril_codex.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-06-20 13:32:01.000000 neomaril-codex-1.2.6/src/neomaril_codex.egg-info/not-zip-safe
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      119 2024-02-01 15:06:05.000000 neomaril-codex-1.2.6/src/neomaril_codex.egg-info/requires.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       15 2024-02-01 15:06:05.000000 neomaril-codex-1.2.6/src/neomaril_codex.egg-info/top_level.txt
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2024-02-01 16:19:56.254965 neomaril-codex-1.2.7/
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1060 2023-03-06 17:55:16.000000 neomaril-codex-1.2.7/LICENSE.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       24 2023-03-13 13:54:26.000000 neomaril-codex-1.2.7/MANIFEST.in
+-rw-r--r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1407 2024-02-01 16:19:56.254965 neomaril-codex-1.2.7/PKG-INFO
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      733 2024-01-17 17:28:06.000000 neomaril-codex-1.2.7/README.md
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      138 2024-02-01 16:08:39.000000 neomaril-codex-1.2.7/requirements.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       79 2024-02-01 16:19:56.254965 neomaril-codex-1.2.7/setup.cfg
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1003 2024-02-01 16:09:48.000000 neomaril-codex-1.2.7/setup.py
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2024-02-01 16:19:56.246965 neomaril-codex-1.2.7/src/
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2024-02-01 16:19:56.250965 neomaril-codex-1.2.7/src/neomaril_codex/
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-02-08 17:56:54.000000 neomaril-codex-1.2.7/src/neomaril_codex/__init__.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1221 2023-11-21 19:18:17.000000 neomaril-codex-1.2.7/src/neomaril_codex/__utils.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    13773 2023-11-09 12:39:19.000000 neomaril-codex-1.2.7/src/neomaril_codex/base.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      858 2023-08-09 19:49:20.000000 neomaril-codex-1.2.7/src/neomaril_codex/exceptions.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     4487 2023-03-06 17:39:34.000000 neomaril-codex-1.2.7/src/neomaril_codex/logging.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    46079 2024-02-01 15:04:26.000000 neomaril-codex-1.2.7/src/neomaril_codex/model.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    13163 2023-12-04 20:06:58.000000 neomaril-codex-1.2.7/src/neomaril_codex/pipeline.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    35563 2024-02-01 15:04:22.000000 neomaril-codex-1.2.7/src/neomaril_codex/preprocessing.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    49344 2024-02-01 15:04:08.000000 neomaril-codex-1.2.7/src/neomaril_codex/training.py
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2024-02-01 16:19:56.254965 neomaril-codex-1.2.7/src/neomaril_codex.egg-info/
+-rw-r--r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1407 2024-02-01 16:19:56.000000 neomaril-codex-1.2.7/src/neomaril_codex.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      596 2024-02-01 16:19:56.000000 neomaril-codex-1.2.7/src/neomaril_codex.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2024-02-01 16:19:56.000000 neomaril-codex-1.2.7/src/neomaril_codex.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2024-02-01 16:17:13.000000 neomaril-codex-1.2.7/src/neomaril_codex.egg-info/not-zip-safe
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      139 2024-02-01 16:19:56.000000 neomaril-codex-1.2.7/src/neomaril_codex.egg-info/requires.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       15 2024-02-01 16:19:56.000000 neomaril-codex-1.2.7/src/neomaril_codex.egg-info/top_level.txt
```

### Comparing `neomaril-codex-1.2.6/LICENSE.txt` & `neomaril-codex-1.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.2.6/PKG-INFO` & `neomaril-codex-1.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: neomaril-codex
-Version: 1.2.6
+Version: 1.2.7
 Summary: Python tools for interact with Neomaril
 Home-page: https://datarisk-io.github.io/mlops-neomaril-codex/
-Download-URL: https://github.com/datarisk-io/mlops-neomaril-codex/archive/refs/tags/v1.2.6.tar.gz
+Download-URL: https://github.com/datarisk-io/mlops-neomaril-codex/archive/refs/tags/v1.2.7.tar.gz
 Author: Datarisk
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests==2.31.0
 Requires-Dist: loguru==0.6.0
 Requires-Dist: pyyaml
 Requires-Dist: python-dotenv==0.21.0
 Requires-Dist: cachetools
 Requires-Dist: cloudpickle>=2.0.0
 Requires-Dist: pyarrow>=1.0.0
 Requires-Dist: pandas>=1.0.0
+Requires-Dist: lazy-imports==0.3.1
 
 # Neomaril Codex
 
 For the brazilian portuguese README, click [here :brazil:](./README.pt-br.md).
 
 ## About
```

### Comparing `neomaril-codex-1.2.6/README.md` & `neomaril-codex-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.2.6/setup.py` & `neomaril-codex-1.2.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from os.path import join
-
 from setuptools import setup, find_packages
 
 MODULE_NAME = 'neomaril-codex'
 MODULE_NAME_IMPORT = 'neomaril_codex'
 REPO_NAME = 'mlops-neomaril-codex'
-MODULE_VERSION='1.2.6'
+MODULE_VERSION='1.2.7'
 
 
 def requirements_from_pip(filename='requirements.txt'):
     with open(filename, 'r') as pip:
         return [l.strip() for l in pip if not l.startswith('#') and l.strip()]
```

### Comparing `neomaril-codex-1.2.6/src/neomaril_codex/__utils.py` & `neomaril-codex-1.2.7/src/neomaril_codex/__utils.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.2.6/src/neomaril_codex/base.py` & `neomaril-codex-1.2.7/src/neomaril_codex/base.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.2.6/src/neomaril_codex/exceptions.py` & `neomaril-codex-1.2.7/src/neomaril_codex/exceptions.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.2.6/src/neomaril_codex/logging.py` & `neomaril-codex-1.2.7/src/neomaril_codex/logging.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.2.6/src/neomaril_codex/model.py` & `neomaril-codex-1.2.7/src/neomaril_codex/model.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.2.6/src/neomaril_codex/pipeline.py` & `neomaril-codex-1.2.7/src/neomaril_codex/pipeline.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.2.6/src/neomaril_codex/preprocessing.py` & `neomaril-codex-1.2.7/src/neomaril_codex/preprocessing.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.2.6/src/neomaril_codex/training.py` & `neomaril-codex-1.2.7/src/neomaril_codex/training.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.2.6/src/neomaril_codex.egg-info/PKG-INFO` & `neomaril-codex-1.2.7/src/neomaril_codex.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: neomaril-codex
-Version: 1.2.6
+Version: 1.2.7
 Summary: Python tools for interact with Neomaril
 Home-page: https://datarisk-io.github.io/mlops-neomaril-codex/
-Download-URL: https://github.com/datarisk-io/mlops-neomaril-codex/archive/refs/tags/v1.2.6.tar.gz
+Download-URL: https://github.com/datarisk-io/mlops-neomaril-codex/archive/refs/tags/v1.2.7.tar.gz
 Author: Datarisk
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests==2.31.0
 Requires-Dist: loguru==0.6.0
 Requires-Dist: pyyaml
 Requires-Dist: python-dotenv==0.21.0
 Requires-Dist: cachetools
 Requires-Dist: cloudpickle>=2.0.0
 Requires-Dist: pyarrow>=1.0.0
 Requires-Dist: pandas>=1.0.0
+Requires-Dist: lazy-imports==0.3.1
 
 # Neomaril Codex
 
 For the brazilian portuguese README, click [here :brazil:](./README.pt-br.md).
 
 ## About
```

### Comparing `neomaril-codex-1.2.6/src/neomaril_codex.egg-info/SOURCES.txt` & `neomaril-codex-1.2.7/src/neomaril_codex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

