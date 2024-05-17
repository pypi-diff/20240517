# Comparing `tmp/pyselenscrapr-0.0.4.tar.gz` & `tmp/pyselenscrapr-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyselenscrapr-0.0.4.tar", last modified: Thu May 16 21:11:47 2024, max compression
+gzip compressed data, was "pyselenscrapr-0.0.5.tar", last modified: Fri May 17 21:23:09 2024, max compression
```

## Comparing `pyselenscrapr-0.0.4.tar` & `pyselenscrapr-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:11:47.303024 pyselenscrapr-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:11:47.299024 pyselenscrapr-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:11:47.299024 pyselenscrapr-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-16 21:11:47.303024 pyselenscrapr-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:11:47.299024 pyselenscrapr-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:11:47.299024 pyselenscrapr-0.0.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/docs/source/pyselenscrapr.rst
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:11:47.303024 pyselenscrapr-0.0.4/pyselenscrapr/
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/pyselenscrapr/ScrapingBackend.py
--rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/pyselenscrapr/ScrapingBot.py
--rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/pyselenscrapr/ScrapingLogic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/pyselenscrapr/ScrapingStep.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/pyselenscrapr/ScrapingStepGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/pyselenscrapr/ScrapingStepLoop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/pyselenscrapr/ScrapingStepPagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/pyselenscrapr/ValidationError.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/pyselenscrapr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:11:47.303024 pyselenscrapr-0.0.4/pyselenscrapr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-16 21:11:47.000000 pyselenscrapr-0.0.4/pyselenscrapr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-16 21:11:47.000000 pyselenscrapr-0.0.4/pyselenscrapr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:11:47.000000 pyselenscrapr-0.0.4/pyselenscrapr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 21:11:47.000000 pyselenscrapr-0.0.4/pyselenscrapr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 21:11:47.000000 pyselenscrapr-0.0.4/pyselenscrapr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-16 21:11:35.000000 pyselenscrapr-0.0.4/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 21:11:47.303024 pyselenscrapr-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:23:09.043532 pyselenscrapr-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:23:09.035532 pyselenscrapr-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:23:09.039533 pyselenscrapr-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-17 21:23:09.043532 pyselenscrapr-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:23:09.039533 pyselenscrapr-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:23:09.039533 pyselenscrapr-0.0.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/docs/source/pyselenscrapr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:23:09.039533 pyselenscrapr-0.0.5/pyselenscrapr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/pyselenscrapr/ScrapingBackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13161 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/pyselenscrapr/ScrapingBot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/pyselenscrapr/ScrapingLogic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/pyselenscrapr/ScrapingStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/pyselenscrapr/ScrapingStepGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/pyselenscrapr/ScrapingStepLoop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/pyselenscrapr/ScrapingStepPagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/pyselenscrapr/ValidationError.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/pyselenscrapr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:23:09.043532 pyselenscrapr-0.0.5/pyselenscrapr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-17 21:23:09.000000 pyselenscrapr-0.0.5/pyselenscrapr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-17 21:23:09.000000 pyselenscrapr-0.0.5/pyselenscrapr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:23:09.000000 pyselenscrapr-0.0.5/pyselenscrapr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-17 21:23:09.000000 pyselenscrapr-0.0.5/pyselenscrapr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 21:23:09.000000 pyselenscrapr-0.0.5/pyselenscrapr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-17 21:22:57.000000 pyselenscrapr-0.0.5/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 21:23:09.043532 pyselenscrapr-0.0.5/setup.cfg
```

### Comparing `pyselenscrapr-0.0.4/.github/workflows/pypi.yml` & `pyselenscrapr-0.0.5/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.4/LICENSE` & `pyselenscrapr-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.4/PKG-INFO` & `pyselenscrapr-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyselenscrapr
-Version: 0.0.4
+Version: 0.0.5
 Summary: A web scraping library for selenium and beautifulsoup
 Author-email: donnercody <donnercody86@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
```

### Comparing `pyselenscrapr-0.0.4/README.rst` & `pyselenscrapr-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.4/docs/Makefile` & `pyselenscrapr-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.4/docs/make.bat` & `pyselenscrapr-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.4/docs/source/conf.py` & `pyselenscrapr-0.0.5/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import sys
 sys.path.insert(0, os.path.abspath(os.path.join("..", "..")))
 
 project = 'PySelenScrapr'
 copyright = '2024, Thoren Lederer'
 author = 'donnercody'
 
-release = '0.0.4'
-version = '0.0.4'
+release = '0.0.5'
+version = '0.0.5'
 
 # -- General configuration
 
 extensions = [
     'sphinx.ext.duration',
     'sphinx.ext.doctest',
     'sphinx.ext.autodoc',
```

### Comparing `pyselenscrapr-0.0.4/docs/source/index.rst` & `pyselenscrapr-0.0.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.4/docs/source/pyselenscrapr.rst` & `pyselenscrapr-0.0.5/docs/source/pyselenscrapr.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.4/docs/source/usage.rst` & `pyselenscrapr-0.0.5/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.4/pyselenscrapr/ScrapingBackend.py` & `pyselenscrapr-0.0.5/pyselenscrapr/ScrapingBackend.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.4/pyselenscrapr/ScrapingBot.py` & `pyselenscrapr-0.0.5/pyselenscrapr/ScrapingBot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging as log
 import time
 from typing import Callable
 
+import numpy as np
 import pandas as pd
 from typing import Union
 from pyselenscrapr.ScrapingBackend import IScrapingBackend
 from pyselenscrapr.ScrapingLogic import ScrapingLogic
 from pyselenscrapr.ScrapingStep import ScrapingStep, ScrapingStepInterval, ScrapingStepErrorHandling
 from pyselenscrapr.ScrapingStepGroup import ScrapingStepGroup
 
@@ -297,15 +298,15 @@
     # Data handling
     ##############################################################################################################
 
     def get_converted_data(self, data):
         retdata = {}
         for key, value in data.items():
             if isinstance(value, pd.DataFrame):
-                retdata[key] = value.to_dict(orient='records')
+                retdata[key] = value.replace({np.nan:None}).to_dict(orient='records')
             else:
                 retdata[key] = value
 
         return retdata
 
     def save_backend_data(self, data):
         try:
```

### Comparing `pyselenscrapr-0.0.4/pyselenscrapr/ScrapingLogic.py` & `pyselenscrapr-0.0.5/pyselenscrapr/ScrapingLogic.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.4/pyselenscrapr/ScrapingStep.py` & `pyselenscrapr-0.0.5/pyselenscrapr/ScrapingStep.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.4/pyselenscrapr/ScrapingStepLoop.py` & `pyselenscrapr-0.0.5/pyselenscrapr/ScrapingStepLoop.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.4/pyselenscrapr/ScrapingStepPagination.py` & `pyselenscrapr-0.0.5/pyselenscrapr/ScrapingStepPagination.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.4/pyselenscrapr.egg-info/PKG-INFO` & `pyselenscrapr-0.0.5/pyselenscrapr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyselenscrapr
-Version: 0.0.4
+Version: 0.0.5
 Summary: A web scraping library for selenium and beautifulsoup
 Author-email: donnercody <donnercody86@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
```

### Comparing `pyselenscrapr-0.0.4/pyselenscrapr.egg-info/SOURCES.txt` & `pyselenscrapr-0.0.5/pyselenscrapr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.4/sample.py` & `pyselenscrapr-0.0.5/sample.py`

 * *Files identical despite different names*

