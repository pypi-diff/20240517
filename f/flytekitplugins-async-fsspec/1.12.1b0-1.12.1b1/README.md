# Comparing `tmp/flytekitplugins_async_fsspec-1.12.1b0.tar.gz` & `tmp/flytekitplugins_async_fsspec-1.12.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins_async_fsspec-1.12.1b0.tar", last modified: Thu May  9 17:17:07 2024, max compression
+gzip compressed data, was "flytekitplugins_async_fsspec-1.12.1b1.tar", last modified: Thu May 16 22:53:09 2024, max compression
```

## Comparing `flytekitplugins_async_fsspec-1.12.1b0.tar` & `flytekitplugins_async_fsspec-1.12.1b1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:17:07.173829 flytekitplugins_async_fsspec-1.12.1b0/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-09 17:17:07.173829 flytekitplugins_async_fsspec-1.12.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-09 17:16:42.000000 flytekitplugins_async_fsspec-1.12.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:17:07.169829 flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:17:07.169829 flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins/async_fsspec/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-09 17:16:42.000000 flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins/async_fsspec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:17:07.169829 flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins/async_fsspec/s3fs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:16:42.000000 flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins/async_fsspec/s3fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-09 17:16:42.000000 flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins/async_fsspec/s3fs/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-05-09 17:16:42.000000 flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins/async_fsspec/s3fs/s3fs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:17:07.173829 flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins_async_fsspec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-09 17:17:07.000000 flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins_async_fsspec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-09 17:17:07.000000 flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins_async_fsspec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:17:07.000000 flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins_async_fsspec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-09 17:17:07.000000 flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins_async_fsspec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 17:17:07.000000 flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins_async_fsspec.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 17:17:07.000000 flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins_async_fsspec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 17:17:07.000000 flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins_async_fsspec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 17:17:07.173829 flytekitplugins_async_fsspec-1.12.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-09 17:17:06.000000 flytekitplugins_async_fsspec-1.12.1b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:17:07.169829 flytekitplugins_async_fsspec-1.12.1b0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-05-09 17:16:42.000000 flytekitplugins_async_fsspec-1.12.1b0/tests/test_s3fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:09.987138 flytekitplugins_async_fsspec-1.12.1b1/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-16 22:53:09.987138 flytekitplugins_async_fsspec-1.12.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-16 22:52:45.000000 flytekitplugins_async_fsspec-1.12.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:09.983138 flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:09.983138 flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins/async_fsspec/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-16 22:52:45.000000 flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins/async_fsspec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:09.983138 flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins/async_fsspec/s3fs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:52:45.000000 flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins/async_fsspec/s3fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-16 22:52:45.000000 flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins/async_fsspec/s3fs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-05-16 22:52:45.000000 flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins/async_fsspec/s3fs/s3fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:09.987138 flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins_async_fsspec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-16 22:53:09.000000 flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins_async_fsspec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 22:53:09.000000 flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins_async_fsspec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:53:09.000000 flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins_async_fsspec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 22:53:09.000000 flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins_async_fsspec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 22:53:09.000000 flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins_async_fsspec.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 22:53:09.000000 flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins_async_fsspec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 22:53:09.000000 flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins_async_fsspec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:53:09.987138 flytekitplugins_async_fsspec-1.12.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-16 22:53:09.000000 flytekitplugins_async_fsspec-1.12.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:09.987138 flytekitplugins_async_fsspec-1.12.1b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-05-16 22:52:45.000000 flytekitplugins_async_fsspec-1.12.1b1/tests/test_s3fs.py
```

### Comparing `flytekitplugins_async_fsspec-1.12.1b0/PKG-INFO` & `flytekitplugins_async_fsspec-1.12.1b1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-async-fsspec
-Version: 1.12.1b0
+Version: 1.12.1b1
 Summary: This package holds the data persistence plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_async_fsspec-1.12.1b0/README.md` & `flytekitplugins_async_fsspec-1.12.1b1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins/async_fsspec/s3fs/s3fs.py` & `flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins/async_fsspec/s3fs/s3fs.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins_async_fsspec.egg-info/PKG-INFO` & `flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins_async_fsspec.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-async-fsspec
-Version: 1.12.1b0
+Version: 1.12.1b1
 Summary: This package holds the data persistence plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_async_fsspec-1.12.1b0/flytekitplugins_async_fsspec.egg-info/SOURCES.txt` & `flytekitplugins_async_fsspec-1.12.1b1/flytekitplugins_async_fsspec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins_async_fsspec-1.12.1b0/setup.py` & `flytekitplugins_async_fsspec-1.12.1b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "async_fsspec"
 
 microlib_name = "flytekitplugins-async-fsspec"
 
 plugin_requires = ["flytekit"]
 
-__version__ = "1.12.1b0"
+__version__ = "1.12.1b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the data persistence plugins for flytekit",
```

### Comparing `flytekitplugins_async_fsspec-1.12.1b0/tests/test_s3fs.py` & `flytekitplugins_async_fsspec-1.12.1b1/tests/test_s3fs.py`

 * *Files identical despite different names*

