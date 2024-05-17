# Comparing `tmp/large-image-source-rasterio-1.28.2.dev8.tar.gz` & `tmp/large-image-source-rasterio-1.28.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-rasterio-1.28.2.dev8.tar", last modified: Wed Apr 24 20:04:29 2024, max compression
+gzip compressed data, was "large-image-source-rasterio-1.28.3.dev2.tar", last modified: Thu May 16 16:49:52 2024, max compression
```

## Comparing `large-image-source-rasterio-1.28.2.dev8.tar` & `large-image-source-rasterio-1.28.3.dev2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:04:29.270456 large-image-source-rasterio-1.28.2.dev8/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-24 20:04:28.000000 large-image-source-rasterio-1.28.2.dev8/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1097 2024-04-24 20:04:29.270456 large-image-source-rasterio-1.28.2.dev8/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-24 20:04:28.000000 large-image-source-rasterio-1.28.2.dev8/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:04:29.266456 large-image-source-rasterio-1.28.2.dev8/large_image_source_rasterio/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43791 2024-04-24 19:59:45.000000 large-image-source-rasterio-1.28.2.dev8/large_image_source_rasterio/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2024-04-24 19:59:45.000000 large-image-source-rasterio-1.28.2.dev8/large_image_source_rasterio/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:04:29.270456 large-image-source-rasterio-1.28.2.dev8/large_image_source_rasterio.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1097 2024-04-24 20:04:29.000000 large-image-source-rasterio-1.28.2.dev8/large_image_source_rasterio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2024-04-24 20:04:29.000000 large-image-source-rasterio-1.28.2.dev8/large_image_source_rasterio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 20:04:29.000000 large-image-source-rasterio-1.28.2.dev8/large_image_source_rasterio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2024-04-24 20:04:29.000000 large-image-source-rasterio-1.28.2.dev8/large_image_source_rasterio.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2024-04-24 20:04:29.000000 large-image-source-rasterio-1.28.2.dev8/large_image_source_rasterio.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-04-24 20:04:29.000000 large-image-source-rasterio-1.28.2.dev8/large_image_source_rasterio.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-24 19:59:45.000000 large-image-source-rasterio-1.28.2.dev8/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 20:04:29.270456 large-image-source-rasterio-1.28.2.dev8/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2636 2024-04-24 19:59:45.000000 large-image-source-rasterio-1.28.2.dev8/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:49:52.238061 large-image-source-rasterio-1.28.3.dev2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-05-16 16:49:51.000000 large-image-source-rasterio-1.28.3.dev2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1097 2024-05-16 16:49:52.238061 large-image-source-rasterio-1.28.3.dev2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-05-16 16:49:51.000000 large-image-source-rasterio-1.28.3.dev2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:49:52.234061 large-image-source-rasterio-1.28.3.dev2/large_image_source_rasterio/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43791 2024-05-16 16:44:45.000000 large-image-source-rasterio-1.28.3.dev2/large_image_source_rasterio/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2024-05-16 16:44:45.000000 large-image-source-rasterio-1.28.3.dev2/large_image_source_rasterio/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:49:52.238061 large-image-source-rasterio-1.28.3.dev2/large_image_source_rasterio.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1097 2024-05-16 16:49:52.000000 large-image-source-rasterio-1.28.3.dev2/large_image_source_rasterio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2024-05-16 16:49:52.000000 large-image-source-rasterio-1.28.3.dev2/large_image_source_rasterio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-16 16:49:52.000000 large-image-source-rasterio-1.28.3.dev2/large_image_source_rasterio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2024-05-16 16:49:52.000000 large-image-source-rasterio-1.28.3.dev2/large_image_source_rasterio.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2024-05-16 16:49:52.000000 large-image-source-rasterio-1.28.3.dev2/large_image_source_rasterio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-05-16 16:49:52.000000 large-image-source-rasterio-1.28.3.dev2/large_image_source_rasterio.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-05-16 16:44:45.000000 large-image-source-rasterio-1.28.3.dev2/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-16 16:49:52.238061 large-image-source-rasterio-1.28.3.dev2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2636 2024-05-16 16:44:45.000000 large-image-source-rasterio-1.28.3.dev2/setup.py
```

### Comparing `large-image-source-rasterio-1.28.2.dev8/LICENSE` & `large-image-source-rasterio-1.28.3.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.28.2.dev8/PKG-INFO` & `large-image-source-rasterio-1.28.3.dev2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.28.2.dev8
+Version: 1.28.3.dev2
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,18 +13,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: large-image>=1.28.2.dev8
+Requires-Dist: large-image>=1.28.3.dev2
 Requires-Dist: rasterio>=1.3
 Requires-Dist: packaging
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.2.dev8; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.3.dev2; extra == "girder"
 Provides-Extra: all
 Requires-Dist: rio-cogeo; extra == "all"
 
 A rasterio tilesource for large_image.
 
 See the large-image package for more details.
```

### Comparing `large-image-source-rasterio-1.28.2.dev8/README.rst` & `large-image-source-rasterio-1.28.3.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.28.2.dev8/large_image_source_rasterio/__init__.py` & `large-image-source-rasterio-1.28.3.dev2/large_image_source_rasterio/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.28.2.dev8/large_image_source_rasterio/girder_source.py` & `large-image-source-rasterio-1.28.3.dev2/large_image_source_rasterio/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.28.2.dev8/large_image_source_rasterio.egg-info/PKG-INFO` & `large-image-source-rasterio-1.28.3.dev2/large_image_source_rasterio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.28.2.dev8
+Version: 1.28.3.dev2
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,18 +13,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: large-image>=1.28.2.dev8
+Requires-Dist: large-image>=1.28.3.dev2
 Requires-Dist: rasterio>=1.3
 Requires-Dist: packaging
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.2.dev8; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.3.dev2; extra == "girder"
 Provides-Extra: all
 Requires-Dist: rio-cogeo; extra == "all"
 
 A rasterio tilesource for large_image.
 
 See the large-image package for more details.
```

### Comparing `large-image-source-rasterio-1.28.2.dev8/setup.py` & `large-image-source-rasterio-1.28.3.dev2/setup.py`

 * *Files identical despite different names*

