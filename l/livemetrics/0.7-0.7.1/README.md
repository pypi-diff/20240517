# Comparing `tmp/livemetrics-0.7.tar.gz` & `tmp/livemetrics-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livemetrics-0.7.tar", last modified: Wed May 15 13:26:12 2024, max compression
+gzip compressed data, was "livemetrics-0.7.1.tar", last modified: Fri May 17 07:31:48 2024, max compression
```

## Comparing `livemetrics-0.7.tar` & `livemetrics-0.7.1.tar`

### file list

```diff
@@ -1,41 +1,49 @@
-drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 13:26:12.615226 livemetrics-0.7/
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      210 2024-05-15 11:50:56.000000 livemetrics-0.7/AUTHORS.rst
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)    21863 2024-05-15 11:50:56.000000 livemetrics-0.7/LICENSE
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      151 2024-05-15 11:50:56.000000 livemetrics-0.7/MANIFEST.in
--rw-r--r--   0 heurtier  (1000) heurtier  (1000)     2561 2024-05-15 13:26:12.615226 livemetrics-0.7/PKG-INFO
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     1470 2024-05-15 11:50:56.000000 livemetrics-0.7/README.rst
-drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 13:26:12.611226 livemetrics-0.7/docs/
-drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 13:26:12.611226 livemetrics-0.7/docs/_static/
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      785 2024-05-15 11:50:56.000000 livemetrics-0.7/docs/_static/custom.css
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      442 2024-05-15 11:50:56.000000 livemetrics-0.7/docs/conf.py
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     1407 2024-05-15 11:50:56.000000 livemetrics-0.7/docs/index.rst
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     1017 2024-05-15 11:50:56.000000 livemetrics-0.7/docs/modules.rst
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      102 2024-05-15 11:50:56.000000 livemetrics-0.7/docs/requirements.txt
-drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 13:26:12.611226 livemetrics-0.7/livemetrics/
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)    16181 2024-05-15 13:25:18.000000 livemetrics-0.7/livemetrics/__init__.py
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)    17523 2024-05-15 11:50:56.000000 livemetrics-0.7/livemetrics/metrics.py
-drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 13:26:12.615226 livemetrics-0.7/livemetrics.egg-info/
--rw-r--r--   0 heurtier  (1000) heurtier  (1000)     2561 2024-05-15 13:26:12.000000 livemetrics-0.7/livemetrics.egg-info/PKG-INFO
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      763 2024-05-15 13:26:12.000000 livemetrics-0.7/livemetrics.egg-info/SOURCES.txt
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)        1 2024-05-15 13:26:12.000000 livemetrics-0.7/livemetrics.egg-info/dependency_links.txt
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)       79 2024-05-15 13:26:12.000000 livemetrics-0.7/livemetrics.egg-info/entry_points.txt
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)       93 2024-05-15 13:26:12.000000 livemetrics-0.7/livemetrics.egg-info/requires.txt
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)       12 2024-05-15 13:26:12.000000 livemetrics-0.7/livemetrics.egg-info/top_level.txt
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)       90 2024-05-15 11:50:56.000000 livemetrics-0.7/pyproject.toml
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     1025 2024-05-15 13:26:12.615226 livemetrics-0.7/setup.cfg
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)       37 2024-05-15 11:50:56.000000 livemetrics-0.7/setup.py
-drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 13:26:12.615226 livemetrics-0.7/tests/
-drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 13:26:12.615226 livemetrics-0.7/tests/dashboard/
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/dashboard/__init__.py
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      588 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/dashboard/client.py
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2311 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/dashboard/sample.yaml
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     1282 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/dashboard/server.py
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2860 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/dashboard/test_dashboard.py
-drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 13:26:12.615226 livemetrics-0.7/tests/publishers/
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     6368 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/publishers/__init__.py
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2490 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/publishers/test_aiohttp.py
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2900 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/publishers/test_django.py
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2315 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/publishers/test_flask.py
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2574 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/publishers/test_http.py
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      387 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/test_doc.py
--rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2608 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/test_metrics.py
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-17 07:31:48.645786 livemetrics-0.7.1/
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      210 2024-05-15 11:50:56.000000 livemetrics-0.7.1/AUTHORS.rst
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)    21863 2024-05-15 11:50:56.000000 livemetrics-0.7.1/LICENSE
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      259 2024-05-17 07:29:20.000000 livemetrics-0.7.1/MANIFEST.in
+-rw-r--r--   0 heurtier  (1000) heurtier  (1000)     2541 2024-05-17 07:31:48.645786 livemetrics-0.7.1/PKG-INFO
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     1470 2024-05-15 11:50:56.000000 livemetrics-0.7.1/README.rst
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-17 07:31:48.641786 livemetrics-0.7.1/docs/
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-17 07:31:48.641786 livemetrics-0.7.1/docs/_static/
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      785 2024-05-15 11:50:56.000000 livemetrics-0.7.1/docs/_static/custom.css
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      442 2024-05-15 11:50:56.000000 livemetrics-0.7.1/docs/conf.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     1407 2024-05-15 11:50:56.000000 livemetrics-0.7.1/docs/index.rst
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     1017 2024-05-15 11:50:56.000000 livemetrics-0.7.1/docs/modules.rst
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      102 2024-05-15 11:50:56.000000 livemetrics-0.7.1/docs/requirements.txt
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-17 07:31:48.641786 livemetrics-0.7.1/livemetrics/
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)    16183 2024-05-17 07:31:32.000000 livemetrics-0.7.1/livemetrics/__init__.py
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-17 07:31:48.645786 livemetrics-0.7.1/livemetrics/dashboard/
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)    14055 2024-05-15 11:50:56.000000 livemetrics-0.7.1/livemetrics/dashboard/dashboard.html
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     8566 2024-05-15 11:50:56.000000 livemetrics-0.7.1/livemetrics/dashboard/dashboard.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)    17523 2024-05-15 11:50:56.000000 livemetrics-0.7.1/livemetrics/metrics.py
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-17 07:31:48.645786 livemetrics-0.7.1/livemetrics/publishers/
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     8022 2024-05-15 11:50:56.000000 livemetrics-0.7.1/livemetrics/publishers/aiohttp.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     7220 2024-05-15 11:50:56.000000 livemetrics-0.7.1/livemetrics/publishers/django.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     7462 2024-05-15 11:50:56.000000 livemetrics-0.7.1/livemetrics/publishers/flask.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     7560 2024-05-15 11:50:56.000000 livemetrics-0.7.1/livemetrics/publishers/http.py
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-17 07:31:48.645786 livemetrics-0.7.1/livemetrics.egg-info/
+-rw-r--r--   0 heurtier  (1000) heurtier  (1000)     2541 2024-05-17 07:31:48.000000 livemetrics-0.7.1/livemetrics.egg-info/PKG-INFO
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     1154 2024-05-17 07:31:48.000000 livemetrics-0.7.1/livemetrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)        1 2024-05-17 07:31:48.000000 livemetrics-0.7.1/livemetrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)       79 2024-05-17 07:31:48.000000 livemetrics-0.7.1/livemetrics.egg-info/entry_points.txt
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)       86 2024-05-17 07:31:48.000000 livemetrics-0.7.1/livemetrics.egg-info/requires.txt
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)       12 2024-05-17 07:31:48.000000 livemetrics-0.7.1/livemetrics.egg-info/top_level.txt
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)       90 2024-05-15 11:50:56.000000 livemetrics-0.7.1/pyproject.toml
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     1050 2024-05-17 07:31:48.649786 livemetrics-0.7.1/setup.cfg
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)       37 2024-05-15 11:50:56.000000 livemetrics-0.7.1/setup.py
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-17 07:31:48.645786 livemetrics-0.7.1/tests/
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-17 07:31:48.645786 livemetrics-0.7.1/tests/dashboard/
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 11:50:56.000000 livemetrics-0.7.1/tests/dashboard/__init__.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      588 2024-05-15 11:50:56.000000 livemetrics-0.7.1/tests/dashboard/client.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2311 2024-05-15 11:50:56.000000 livemetrics-0.7.1/tests/dashboard/sample.yaml
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     1282 2024-05-15 11:50:56.000000 livemetrics-0.7.1/tests/dashboard/server.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2860 2024-05-15 11:50:56.000000 livemetrics-0.7.1/tests/dashboard/test_dashboard.py
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-17 07:31:48.645786 livemetrics-0.7.1/tests/publishers/
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     6368 2024-05-15 11:50:56.000000 livemetrics-0.7.1/tests/publishers/__init__.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2490 2024-05-15 11:50:56.000000 livemetrics-0.7.1/tests/publishers/test_aiohttp.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2900 2024-05-15 11:50:56.000000 livemetrics-0.7.1/tests/publishers/test_django.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2315 2024-05-15 11:50:56.000000 livemetrics-0.7.1/tests/publishers/test_flask.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2574 2024-05-15 11:50:56.000000 livemetrics-0.7.1/tests/publishers/test_http.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      387 2024-05-15 11:50:56.000000 livemetrics-0.7.1/tests/test_doc.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2608 2024-05-15 11:50:56.000000 livemetrics-0.7.1/tests/test_metrics.py
```

### Comparing `livemetrics-0.7/LICENSE` & `livemetrics-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `livemetrics-0.7/PKG-INFO` & `livemetrics-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livemetrics
-Version: 0.7
+Version: 0.7.1
 Summary: LiveMetrics collector and publisher for Python applications
 Home-page: https://github.com/idemia/python-livemetrics
 Author: attr: livemetrics.__author__
 Author-email: olivier.heurtier@idemia.com
 License: CeCILL-C
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: CeCILL-C Free Software License Agreement (CECILL-C)
 Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: Pillow
 Provides-Extra: aiohttp
 Requires-Dist: aiohttp; extra == "aiohttp"
 Provides-Extra: django
 Requires-Dist: django; extra == "django"
 Provides-Extra: flask
 Requires-Dist: flask; extra == "flask"
 Provides-Extra: dashboard
```

### Comparing `livemetrics-0.7/README.rst` & `livemetrics-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `livemetrics-0.7/docs/_static/custom.css` & `livemetrics-0.7.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `livemetrics-0.7/docs/index.rst` & `livemetrics-0.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `livemetrics-0.7/docs/modules.rst` & `livemetrics-0.7.1/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `livemetrics-0.7/livemetrics/__init__.py` & `livemetrics-0.7.1/livemetrics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 import time
 import collections
 from functools import wraps
 import asyncio
 
 from livemetrics.metrics import *
 
-__version__ = '0.7'
+__version__ = '0.7.1'
 __author__ = "Olivier Heurtier"
 __copyright__ = "IDEMIA"
 __license__ = "CeCILL-C"
 
 if os.name=='posix':
     # XXX make it 2 values (one with data+stack only)
     def get_memory():
```

### Comparing `livemetrics-0.7/livemetrics/metrics.py` & `livemetrics-0.7.1/livemetrics/metrics.py`

 * *Files identical despite different names*

### Comparing `livemetrics-0.7/livemetrics.egg-info/PKG-INFO` & `livemetrics-0.7.1/livemetrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livemetrics
-Version: 0.7
+Version: 0.7.1
 Summary: LiveMetrics collector and publisher for Python applications
 Home-page: https://github.com/idemia/python-livemetrics
 Author: attr: livemetrics.__author__
 Author-email: olivier.heurtier@idemia.com
 License: CeCILL-C
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: CeCILL-C Free Software License Agreement (CECILL-C)
 Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: Pillow
 Provides-Extra: aiohttp
 Requires-Dist: aiohttp; extra == "aiohttp"
 Provides-Extra: django
 Requires-Dist: django; extra == "django"
 Provides-Extra: flask
 Requires-Dist: flask; extra == "flask"
 Provides-Extra: dashboard
```

### Comparing `livemetrics-0.7/setup.cfg` & `livemetrics-0.7.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	License :: CeCILL-C Free Software License Agreement (CECILL-C)
 
 [options]
-packages = find:
+packages = livemetrics
+	livemetrics.publishers
+	livemetrics.dashboard
 include_package_data = True
 python_requires = >=3.8
 test_suite = 
 	tests
-install_requires = 
-	Pillow
 
 [options.extras_require]
 aiohttp = aiohttp
 django = django
 flask = flask
 dashboard = 
 	jinja2
```

### Comparing `livemetrics-0.7/tests/dashboard/client.py` & `livemetrics-0.7.1/tests/dashboard/client.py`

 * *Files identical despite different names*

### Comparing `livemetrics-0.7/tests/dashboard/sample.yaml` & `livemetrics-0.7.1/tests/dashboard/sample.yaml`

 * *Files identical despite different names*

### Comparing `livemetrics-0.7/tests/dashboard/server.py` & `livemetrics-0.7.1/tests/dashboard/server.py`

 * *Files identical despite different names*

### Comparing `livemetrics-0.7/tests/dashboard/test_dashboard.py` & `livemetrics-0.7.1/tests/dashboard/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `livemetrics-0.7/tests/publishers/__init__.py` & `livemetrics-0.7.1/tests/publishers/__init__.py`

 * *Files identical despite different names*

### Comparing `livemetrics-0.7/tests/publishers/test_aiohttp.py` & `livemetrics-0.7.1/tests/publishers/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `livemetrics-0.7/tests/publishers/test_django.py` & `livemetrics-0.7.1/tests/publishers/test_django.py`

 * *Files identical despite different names*

### Comparing `livemetrics-0.7/tests/publishers/test_flask.py` & `livemetrics-0.7.1/tests/publishers/test_flask.py`

 * *Files identical despite different names*

### Comparing `livemetrics-0.7/tests/publishers/test_http.py` & `livemetrics-0.7.1/tests/publishers/test_http.py`

 * *Files identical despite different names*

### Comparing `livemetrics-0.7/tests/test_metrics.py` & `livemetrics-0.7.1/tests/test_metrics.py`

 * *Files identical despite different names*

