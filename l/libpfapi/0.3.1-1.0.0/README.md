# Comparing `tmp/libpfapi-0.3.1.tar.gz` & `tmp/libpfapi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libpfapi-0.3.1.tar", last modified: Fri May 17 12:12:57 2024, max compression
+gzip compressed data, was "libpfapi-1.0.0.tar", last modified: Fri May 17 11:45:27 2024, max compression
```

## Comparing `libpfapi-0.3.1.tar` & `libpfapi-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 rafaelcsw   (502) staff       (20)        0 2024-05-17 12:12:57.724660 libpfapi-0.3.1/
--rw-r--r--   0 rafaelcsw   (502) staff       (20)    11341 2024-05-17 10:11:13.000000 libpfapi-0.3.1/LICENSE
--rw-r--r--   0 rafaelcsw   (502) staff       (20)      959 2024-05-17 12:12:57.724466 libpfapi-0.3.1/PKG-INFO
--rw-r--r--   0 rafaelcsw   (502) staff       (20)      399 2024-05-17 09:06:21.000000 libpfapi-0.3.1/README.md
-drwxr-xr-x   0 rafaelcsw   (502) staff       (20)        0 2024-05-17 12:12:57.720752 libpfapi-0.3.1/libpfapi/
--rw-r--r--   0 rafaelcsw   (502) staff       (20)        0 2024-04-26 15:14:24.000000 libpfapi-0.3.1/libpfapi/__init__.py
--rw-r--r--   0 rafaelcsw   (502) staff       (20)    39558 2024-05-17 09:06:21.000000 libpfapi-0.3.1/libpfapi/api.py
--rw-r--r--   0 rafaelcsw   (502) staff       (20)      450 2024-04-26 15:14:24.000000 libpfapi-0.3.1/libpfapi/exceptions.py
-drwxr-xr-x   0 rafaelcsw   (502) staff       (20)        0 2024-05-17 12:12:57.724099 libpfapi-0.3.1/libpfapi/models/
--rw-r--r--   0 rafaelcsw   (502) staff       (20)      259 2024-04-26 15:14:24.000000 libpfapi-0.3.1/libpfapi/models/__init__.py
--rw-r--r--   0 rafaelcsw   (502) staff       (20)     3058 2024-04-26 15:14:24.000000 libpfapi-0.3.1/libpfapi/models/base.py
--rw-r--r--   0 rafaelcsw   (502) staff       (20)     6898 2024-04-26 15:14:24.000000 libpfapi-0.3.1/libpfapi/models/baselayer.py
--rw-r--r--   0 rafaelcsw   (502) staff       (20)     1861 2024-04-26 15:14:24.000000 libpfapi-0.3.1/libpfapi/models/category.py
--rw-r--r--   0 rafaelcsw   (502) staff       (20)     1452 2024-04-26 15:14:24.000000 libpfapi-0.3.1/libpfapi/models/corridor.py
--rw-r--r--   0 rafaelcsw   (502) staff       (20)     8123 2024-04-26 15:14:24.000000 libpfapi-0.3.1/libpfapi/models/cost.py
--rw-r--r--   0 rafaelcsw   (502) staff       (20)    13402 2024-04-26 15:14:24.000000 libpfapi-0.3.1/libpfapi/models/layer.py
--rw-r--r--   0 rafaelcsw   (502) staff       (20)    14496 2024-04-26 15:14:24.000000 libpfapi-0.3.1/libpfapi/models/layerconfig.py
--rw-r--r--   0 rafaelcsw   (502) staff       (20)     7605 2024-04-26 15:14:24.000000 libpfapi-0.3.1/libpfapi/models/project.py
--rw-r--r--   0 rafaelcsw   (502) staff       (20)     1422 2024-04-26 15:14:24.000000 libpfapi-0.3.1/libpfapi/models/rmap.py
--rw-r--r--   0 rafaelcsw   (502) staff       (20)    25677 2024-04-26 15:14:24.000000 libpfapi-0.3.1/libpfapi/models/scenario.py
--rw-r--r--   0 rafaelcsw   (502) staff       (20)     3234 2024-04-26 15:14:24.000000 libpfapi-0.3.1/libpfapi/models/scenarioconfig.py
--rw-r--r--   0 rafaelcsw   (502) staff       (20)     3865 2024-04-26 15:14:24.000000 libpfapi-0.3.1/libpfapi/models/scenariopath.py
--rw-r--r--   0 rafaelcsw   (502) staff       (20)     2878 2024-04-26 15:14:24.000000 libpfapi-0.3.1/libpfapi/task.py
-drwxr-xr-x   0 rafaelcsw   (502) staff       (20)        0 2024-05-17 12:12:57.724286 libpfapi-0.3.1/libpfapi.egg-info/
--rw-r--r--   0 rafaelcsw   (502) staff       (20)      959 2024-05-17 12:12:57.000000 libpfapi-0.3.1/libpfapi.egg-info/PKG-INFO
--rw-r--r--   0 rafaelcsw   (502) staff       (20)      608 2024-05-17 12:12:57.000000 libpfapi-0.3.1/libpfapi.egg-info/SOURCES.txt
--rw-r--r--   0 rafaelcsw   (502) staff       (20)        1 2024-05-17 12:12:57.000000 libpfapi-0.3.1/libpfapi.egg-info/dependency_links.txt
--rw-r--r--   0 rafaelcsw   (502) staff       (20)        9 2024-05-17 12:12:57.000000 libpfapi-0.3.1/libpfapi.egg-info/top_level.txt
--rw-r--r--   0 rafaelcsw   (502) staff       (20)      676 2024-05-17 12:12:27.000000 libpfapi-0.3.1/pyproject.toml
--rw-r--r--   0 rafaelcsw   (502) staff       (20)       38 2024-05-17 12:12:57.724706 libpfapi-0.3.1/setup.cfg
--rw-r--r--   0 rafaelcsw   (502) staff       (20)      121 2024-04-26 15:14:24.000000 libpfapi-0.3.1/setup.py
+drwxr-xr-x   0 rafaelcsw   (502) staff       (20)        0 2024-05-17 11:45:27.220754 libpfapi-1.0.0/
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)    11341 2024-05-17 10:11:13.000000 libpfapi-1.0.0/LICENSE
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)      959 2024-05-17 11:45:27.220584 libpfapi-1.0.0/PKG-INFO
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)      399 2024-05-17 09:06:21.000000 libpfapi-1.0.0/README.md
+drwxr-xr-x   0 rafaelcsw   (502) staff       (20)        0 2024-05-17 11:45:27.216870 libpfapi-1.0.0/libpfapi/
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)        0 2024-04-26 15:14:24.000000 libpfapi-1.0.0/libpfapi/__init__.py
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)    39558 2024-05-17 09:06:21.000000 libpfapi-1.0.0/libpfapi/api.py
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)      450 2024-04-26 15:14:24.000000 libpfapi-1.0.0/libpfapi/exceptions.py
+drwxr-xr-x   0 rafaelcsw   (502) staff       (20)        0 2024-05-17 11:45:27.220238 libpfapi-1.0.0/libpfapi/models/
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)      259 2024-04-26 15:14:24.000000 libpfapi-1.0.0/libpfapi/models/__init__.py
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)     3058 2024-04-26 15:14:24.000000 libpfapi-1.0.0/libpfapi/models/base.py
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)     6898 2024-04-26 15:14:24.000000 libpfapi-1.0.0/libpfapi/models/baselayer.py
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)     1861 2024-04-26 15:14:24.000000 libpfapi-1.0.0/libpfapi/models/category.py
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)     1452 2024-04-26 15:14:24.000000 libpfapi-1.0.0/libpfapi/models/corridor.py
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)     8123 2024-04-26 15:14:24.000000 libpfapi-1.0.0/libpfapi/models/cost.py
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)    13402 2024-04-26 15:14:24.000000 libpfapi-1.0.0/libpfapi/models/layer.py
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)    14496 2024-04-26 15:14:24.000000 libpfapi-1.0.0/libpfapi/models/layerconfig.py
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)     7605 2024-04-26 15:14:24.000000 libpfapi-1.0.0/libpfapi/models/project.py
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)     1422 2024-04-26 15:14:24.000000 libpfapi-1.0.0/libpfapi/models/rmap.py
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)    25677 2024-04-26 15:14:24.000000 libpfapi-1.0.0/libpfapi/models/scenario.py
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)     3234 2024-04-26 15:14:24.000000 libpfapi-1.0.0/libpfapi/models/scenarioconfig.py
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)     3865 2024-04-26 15:14:24.000000 libpfapi-1.0.0/libpfapi/models/scenariopath.py
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)     2878 2024-04-26 15:14:24.000000 libpfapi-1.0.0/libpfapi/task.py
+drwxr-xr-x   0 rafaelcsw   (502) staff       (20)        0 2024-05-17 11:45:27.220407 libpfapi-1.0.0/libpfapi.egg-info/
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)      959 2024-05-17 11:45:27.000000 libpfapi-1.0.0/libpfapi.egg-info/PKG-INFO
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)      608 2024-05-17 11:45:27.000000 libpfapi-1.0.0/libpfapi.egg-info/SOURCES.txt
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)        1 2024-05-17 11:45:27.000000 libpfapi-1.0.0/libpfapi.egg-info/dependency_links.txt
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)        9 2024-05-17 11:45:27.000000 libpfapi-1.0.0/libpfapi.egg-info/top_level.txt
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)      676 2024-05-17 11:16:15.000000 libpfapi-1.0.0/pyproject.toml
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)       38 2024-05-17 11:45:27.220798 libpfapi-1.0.0/setup.cfg
+-rw-r--r--   0 rafaelcsw   (502) staff       (20)      121 2024-04-26 15:14:24.000000 libpfapi-1.0.0/setup.py
```

### Comparing `libpfapi-0.3.1/LICENSE` & `libpfapi-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libpfapi-0.3.1/PKG-INFO` & `libpfapi-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libpfapi
-Version: 0.3.1
+Version: 1.0.0
 Summary: Base library providing basic pathfinder REST api access utilities
 Author-email: Jordi Castells <jordi.castells@gilytics.com>, Rafael Ruiz <rafael.romero@gilytics.com>
 Project-URL: Homepage, https://www.gilytics.com/
 Project-URL: Issues, https://www.gilytics.com/faqs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `libpfapi-0.3.1/libpfapi/api.py` & `libpfapi-1.0.0/libpfapi/api.py`

 * *Files identical despite different names*

### Comparing `libpfapi-0.3.1/libpfapi/models/base.py` & `libpfapi-1.0.0/libpfapi/models/base.py`

 * *Files identical despite different names*

### Comparing `libpfapi-0.3.1/libpfapi/models/baselayer.py` & `libpfapi-1.0.0/libpfapi/models/baselayer.py`

 * *Files identical despite different names*

### Comparing `libpfapi-0.3.1/libpfapi/models/category.py` & `libpfapi-1.0.0/libpfapi/models/category.py`

 * *Files identical despite different names*

### Comparing `libpfapi-0.3.1/libpfapi/models/corridor.py` & `libpfapi-1.0.0/libpfapi/models/corridor.py`

 * *Files identical despite different names*

### Comparing `libpfapi-0.3.1/libpfapi/models/cost.py` & `libpfapi-1.0.0/libpfapi/models/cost.py`

 * *Files identical despite different names*

### Comparing `libpfapi-0.3.1/libpfapi/models/layer.py` & `libpfapi-1.0.0/libpfapi/models/layer.py`

 * *Files identical despite different names*

### Comparing `libpfapi-0.3.1/libpfapi/models/layerconfig.py` & `libpfapi-1.0.0/libpfapi/models/layerconfig.py`

 * *Files identical despite different names*

### Comparing `libpfapi-0.3.1/libpfapi/models/project.py` & `libpfapi-1.0.0/libpfapi/models/project.py`

 * *Files identical despite different names*

### Comparing `libpfapi-0.3.1/libpfapi/models/rmap.py` & `libpfapi-1.0.0/libpfapi/models/rmap.py`

 * *Files identical despite different names*

### Comparing `libpfapi-0.3.1/libpfapi/models/scenario.py` & `libpfapi-1.0.0/libpfapi/models/scenario.py`

 * *Files identical despite different names*

### Comparing `libpfapi-0.3.1/libpfapi/models/scenarioconfig.py` & `libpfapi-1.0.0/libpfapi/models/scenarioconfig.py`

 * *Files identical despite different names*

### Comparing `libpfapi-0.3.1/libpfapi/models/scenariopath.py` & `libpfapi-1.0.0/libpfapi/models/scenariopath.py`

 * *Files identical despite different names*

### Comparing `libpfapi-0.3.1/libpfapi/task.py` & `libpfapi-1.0.0/libpfapi/task.py`

 * *Files identical despite different names*

### Comparing `libpfapi-0.3.1/libpfapi.egg-info/PKG-INFO` & `libpfapi-1.0.0/libpfapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libpfapi
-Version: 0.3.1
+Version: 1.0.0
 Summary: Base library providing basic pathfinder REST api access utilities
 Author-email: Jordi Castells <jordi.castells@gilytics.com>, Rafael Ruiz <rafael.romero@gilytics.com>
 Project-URL: Homepage, https://www.gilytics.com/
 Project-URL: Issues, https://www.gilytics.com/faqs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `libpfapi-0.3.1/libpfapi.egg-info/SOURCES.txt` & `libpfapi-1.0.0/libpfapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libpfapi-0.3.1/pyproject.toml` & `libpfapi-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.5.1", "requests~=2.31.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "libpfapi"
-version = "0.3.1"
+version = "1.0.0"
 authors = [
     { name="Jordi Castells", email="jordi.castells@gilytics.com" },
     { name="Rafael Ruiz", email="rafael.romero@gilytics.com" },
 ]
 description = "Base library providing basic pathfinder REST api access utilities"
 readme = "README.md"
 requires-python = ">=3.8"
```

