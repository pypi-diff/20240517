# Comparing `tmp/gdtransform-0.0.3.tar.gz` & `tmp/gdtransform-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdtransform-0.0.3.tar", last modified: Fri May 17 11:51:08 2024, max compression
+gzip compressed data, was "gdtransform-0.0.4.tar", last modified: Fri May 17 11:55:14 2024, max compression
```

## Comparing `gdtransform-0.0.3.tar` & `gdtransform-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-17 11:51:08.125859 gdtransform-0.0.3/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-17 10:41:53.000000 gdtransform-0.0.3/LICENSE
--rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-17 11:51:08.125859 gdtransform-0.0.3/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       91 2024-05-17 10:41:53.000000 gdtransform-0.0.3/README.md
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      733 2024-05-17 11:50:28.000000 gdtransform-0.0.3/pyproject.toml
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-17 11:51:08.125859 gdtransform-0.0.3/setup.cfg
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-17 11:51:08.125859 gdtransform-0.0.3/src/
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-17 11:51:08.125859 gdtransform-0.0.3/src/gdtransform/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       37 2024-05-17 11:48:59.000000 gdtransform-0.0.3/src/gdtransform/__init__.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      317 2024-05-17 11:51:03.000000 gdtransform-0.0.3/src/gdtransform/transform.py
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-17 11:51:08.125859 gdtransform-0.0.3/src/gdtransform.egg-info/
--rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-17 11:51:08.000000 gdtransform-0.0.3/src/gdtransform.egg-info/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      245 2024-05-17 11:51:08.000000 gdtransform-0.0.3/src/gdtransform.egg-info/SOURCES.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-17 11:51:08.000000 gdtransform-0.0.3/src/gdtransform.egg-info/dependency_links.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-17 11:51:08.000000 gdtransform-0.0.3/src/gdtransform.egg-info/top_level.txt
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-17 11:55:14.303598 gdtransform-0.0.4/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-17 10:41:53.000000 gdtransform-0.0.4/LICENSE
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-17 11:55:14.303598 gdtransform-0.0.4/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       91 2024-05-17 10:41:53.000000 gdtransform-0.0.4/README.md
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      733 2024-05-17 11:54:38.000000 gdtransform-0.0.4/pyproject.toml
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-17 11:55:14.303598 gdtransform-0.0.4/setup.cfg
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-17 11:55:14.303598 gdtransform-0.0.4/src/
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-17 11:55:14.303598 gdtransform-0.0.4/src/gdtransform/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       24 2024-05-17 11:54:27.000000 gdtransform-0.0.4/src/gdtransform/__init__.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      317 2024-05-17 11:51:03.000000 gdtransform-0.0.4/src/gdtransform/transform.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-17 11:55:14.303598 gdtransform-0.0.4/src/gdtransform.egg-info/
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-17 11:55:14.000000 gdtransform-0.0.4/src/gdtransform.egg-info/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      245 2024-05-17 11:55:14.000000 gdtransform-0.0.4/src/gdtransform.egg-info/SOURCES.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-17 11:55:14.000000 gdtransform-0.0.4/src/gdtransform.egg-info/dependency_links.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-17 11:55:14.000000 gdtransform-0.0.4/src/gdtransform.egg-info/top_level.txt
```

### Comparing `gdtransform-0.0.3/LICENSE` & `gdtransform-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gdtransform-0.0.3/PKG-INFO` & `gdtransform-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdtransform
-Version: 0.0.3
+Version: 0.0.4
 Summary: Transformation library to build transformations for Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gdtransform
 Project-URL: Issues, https://github.com/godelgrid/gdtransform/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gdtransform-0.0.3/pyproject.toml` & `gdtransform-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "gdtransform"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "Mayank Bhargava", email = "mbhargava.gd@gmail.com" },
 ]
 description = "Transformation library to build transformations for Godel Grid data platform"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gdtransform-0.0.3/src/gdtransform.egg-info/PKG-INFO` & `gdtransform-0.0.4/src/gdtransform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdtransform
-Version: 0.0.3
+Version: 0.0.4
 Summary: Transformation library to build transformations for Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gdtransform
 Project-URL: Issues, https://github.com/godelgrid/gdtransform/issues
 Classifier: Programming Language :: Python :: 3.10
```

