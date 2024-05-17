# Comparing `tmp/large-image-source-vips-1.28.3.dev2.tar.gz` & `tmp/large-image-source-vips-1.28.3.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-vips-1.28.3.dev2.tar", last modified: Thu May 16 16:50:48 2024, max compression
+gzip compressed data, was "large-image-source-vips-1.28.3.dev4.tar", last modified: Fri May 17 20:25:05 2024, max compression
```

## Comparing `large-image-source-vips-1.28.3.dev2.tar` & `large-image-source-vips-1.28.3.dev4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:50:48.102145 large-image-source-vips-1.28.3.dev2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-05-16 16:50:47.000000 large-image-source-vips-1.28.3.dev2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1031 2024-05-16 16:50:48.102145 large-image-source-vips-1.28.3.dev2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-05-16 16:50:47.000000 large-image-source-vips-1.28.3.dev2/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:50:48.102145 large-image-source-vips-1.28.3.dev2/large_image_source_vips/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25562 2024-05-16 16:44:45.000000 large-image-source-vips-1.28.3.dev2/large_image_source_vips/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2024-05-16 16:44:45.000000 large-image-source-vips-1.28.3.dev2/large_image_source_vips/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:50:48.102145 large-image-source-vips-1.28.3.dev2/large_image_source_vips.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1031 2024-05-16 16:50:47.000000 large-image-source-vips-1.28.3.dev2/large_image_source_vips.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-05-16 16:50:48.000000 large-image-source-vips-1.28.3.dev2/large_image_source_vips.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-16 16:50:47.000000 large-image-source-vips-1.28.3.dev2/large_image_source_vips.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-05-16 16:50:47.000000 large-image-source-vips-1.28.3.dev2/large_image_source_vips.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2024-05-16 16:50:47.000000 large-image-source-vips-1.28.3.dev2/large_image_source_vips.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-05-16 16:50:47.000000 large-image-source-vips-1.28.3.dev2/large_image_source_vips.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-05-16 16:44:45.000000 large-image-source-vips-1.28.3.dev2/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-16 16:50:48.102145 large-image-source-vips-1.28.3.dev2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2483 2024-05-16 16:44:45.000000 large-image-source-vips-1.28.3.dev2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-17 20:25:05.881371 large-image-source-vips-1.28.3.dev4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-05-17 20:25:05.000000 large-image-source-vips-1.28.3.dev4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1031 2024-05-17 20:25:05.881371 large-image-source-vips-1.28.3.dev4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-05-17 20:25:05.000000 large-image-source-vips-1.28.3.dev4/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-17 20:25:05.877370 large-image-source-vips-1.28.3.dev4/large_image_source_vips/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25562 2024-05-17 20:19:31.000000 large-image-source-vips-1.28.3.dev4/large_image_source_vips/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2024-05-17 20:19:31.000000 large-image-source-vips-1.28.3.dev4/large_image_source_vips/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-17 20:25:05.881371 large-image-source-vips-1.28.3.dev4/large_image_source_vips.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1031 2024-05-17 20:25:05.000000 large-image-source-vips-1.28.3.dev4/large_image_source_vips.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-05-17 20:25:05.000000 large-image-source-vips-1.28.3.dev4/large_image_source_vips.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-17 20:25:05.000000 large-image-source-vips-1.28.3.dev4/large_image_source_vips.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-05-17 20:25:05.000000 large-image-source-vips-1.28.3.dev4/large_image_source_vips.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2024-05-17 20:25:05.000000 large-image-source-vips-1.28.3.dev4/large_image_source_vips.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-05-17 20:25:05.000000 large-image-source-vips-1.28.3.dev4/large_image_source_vips.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-05-17 20:19:31.000000 large-image-source-vips-1.28.3.dev4/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-17 20:25:05.881371 large-image-source-vips-1.28.3.dev4/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2483 2024-05-17 20:19:31.000000 large-image-source-vips-1.28.3.dev4/setup.py
```

### Comparing `large-image-source-vips-1.28.3.dev2/LICENSE` & `large-image-source-vips-1.28.3.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.28.3.dev2/PKG-INFO` & `large-image-source-vips-1.28.3.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-vips
-Version: 1.28.3.dev2
+Version: 1.28.3.dev4
 Summary: A libvips tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: large-image>=1.28.3.dev2
+Requires-Dist: large-image>=1.28.3.dev4
 Requires-Dist: numpy
 Requires-Dist: packaging
 Requires-Dist: pyvips
 Provides-Extra: girder
 Requires-Dist: girder-large-image; extra == "girder"
 
 A libvips tilesource for large_image.
```

### Comparing `large-image-source-vips-1.28.3.dev2/README.rst` & `large-image-source-vips-1.28.3.dev4/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.28.3.dev2/large_image_source_vips/__init__.py` & `large-image-source-vips-1.28.3.dev4/large_image_source_vips/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.28.3.dev2/large_image_source_vips.egg-info/PKG-INFO` & `large-image-source-vips-1.28.3.dev4/large_image_source_vips.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-vips
-Version: 1.28.3.dev2
+Version: 1.28.3.dev4
 Summary: A libvips tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: large-image>=1.28.3.dev2
+Requires-Dist: large-image>=1.28.3.dev4
 Requires-Dist: numpy
 Requires-Dist: packaging
 Requires-Dist: pyvips
 Provides-Extra: girder
 Requires-Dist: girder-large-image; extra == "girder"
 
 A libvips tilesource for large_image.
```

### Comparing `large-image-source-vips-1.28.3.dev2/setup.py` & `large-image-source-vips-1.28.3.dev4/setup.py`

 * *Files identical despite different names*

