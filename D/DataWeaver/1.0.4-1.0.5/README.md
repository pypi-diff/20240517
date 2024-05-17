# Comparing `tmp/dataweaver-1.0.4.tar.gz` & `tmp/dataweaver-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataweaver-1.0.4.tar", last modified: Thu May 16 09:04:40 2024, max compression
+gzip compressed data, was "dataweaver-1.0.5.tar", last modified: Thu May 16 13:07:53 2024, max compression
```

## Comparing `dataweaver-1.0.4.tar` & `dataweaver-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:40.532630 dataweaver-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-16 09:04:36.000000 dataweaver-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23720 2024-05-16 09:04:40.532630 dataweaver-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23007 2024-05-16 09:04:36.000000 dataweaver-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-16 09:04:36.000000 dataweaver-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:04:40.532630 dataweaver-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:40.528630 dataweaver-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:40.532630 dataweaver-1.0.4/src/DataWeaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23720 2024-05-16 09:04:40.000000 dataweaver-1.0.4/src/DataWeaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-16 09:04:40.000000 dataweaver-1.0.4/src/DataWeaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:04:40.000000 dataweaver-1.0.4/src/DataWeaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 09:04:40.000000 dataweaver-1.0.4/src/DataWeaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 09:04:40.000000 dataweaver-1.0.4/src/DataWeaver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:40.532630 dataweaver-1.0.4/src/data_weaver/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-16 09:04:36.000000 dataweaver-1.0.4/src/data_weaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-16 09:04:36.000000 dataweaver-1.0.4/src/data_weaver/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-16 09:04:36.000000 dataweaver-1.0.4/src/data_weaver/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-16 09:04:36.000000 dataweaver-1.0.4/src/data_weaver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:07:53.229403 dataweaver-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-16 13:07:47.000000 dataweaver-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23720 2024-05-16 13:07:53.229403 dataweaver-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23007 2024-05-16 13:07:47.000000 dataweaver-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-16 13:07:47.000000 dataweaver-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:07:53.229403 dataweaver-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:07:53.225403 dataweaver-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:07:53.229403 dataweaver-1.0.5/src/DataWeaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23720 2024-05-16 13:07:53.000000 dataweaver-1.0.5/src/DataWeaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-16 13:07:53.000000 dataweaver-1.0.5/src/DataWeaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:07:53.000000 dataweaver-1.0.5/src/DataWeaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 13:07:53.000000 dataweaver-1.0.5/src/DataWeaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 13:07:53.000000 dataweaver-1.0.5/src/DataWeaver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:07:53.229403 dataweaver-1.0.5/src/data_weaver/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-16 13:07:47.000000 dataweaver-1.0.5/src/data_weaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-05-16 13:07:47.000000 dataweaver-1.0.5/src/data_weaver/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-16 13:07:47.000000 dataweaver-1.0.5/src/data_weaver/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-16 13:07:47.000000 dataweaver-1.0.5/src/data_weaver/utils.py
```

### Comparing `dataweaver-1.0.4/LICENSE` & `dataweaver-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dataweaver-1.0.4/PKG-INFO` & `dataweaver-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataWeaver
-Version: 1.0.4
+Version: 1.0.5
 Summary: DataWeaver is a Python library for mapping data and transform object to an other. It offers flexible field mapping through a simple configuration object, enabling easy data integration and transformation for analysis and processing.
 Author-email: RICHARD Quentin <richard.quentin88@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/RICHARD-Quentin/DataWeaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dataweaver-1.0.4/README.md` & `dataweaver-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dataweaver-1.0.4/pyproject.toml` & `dataweaver-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DataWeaver"
-version = "1.0.4"
+version = "1.0.5"
 authors = [{name = "RICHARD Quentin", email = "richard.quentin88@gmail.com"}]
 description = "DataWeaver is a Python library for mapping data and transform object to an other. It offers flexible field mapping through a simple configuration object, enabling easy data integration and transformation for analysis and processing."
 readme = "README.md"
 license = {text = "MIT License"}  # Update the license as appropriate
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `dataweaver-1.0.4/src/DataWeaver.egg-info/PKG-INFO` & `dataweaver-1.0.5/src/DataWeaver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataWeaver
-Version: 1.0.4
+Version: 1.0.5
 Summary: DataWeaver is a Python library for mapping data and transform object to an other. It offers flexible field mapping through a simple configuration object, enabling easy data integration and transformation for analysis and processing.
 Author-email: RICHARD Quentin <richard.quentin88@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/RICHARD-Quentin/DataWeaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dataweaver-1.0.4/src/data_weaver/main.py` & `dataweaver-1.0.5/src/data_weaver/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,17 @@
         None
     """
     
     for key, source_key in config.get('mapping').items():
         value = handle_value(data, source_key, key)
         final_result[key] = value
 
+    for key, value in config.get('additionalFields').items():
+        final_result[key] = value
+
 async def process_entry(entry):
     final_result = {}
     flat_object = crush(entry)
     await map_fields(flat_object, final_result)
     return construct(final_result)
 
 async def process_entries(entries):
```

### Comparing `dataweaver-1.0.4/src/data_weaver/transforms.py` & `dataweaver-1.0.5/src/data_weaver/transforms.py`

 * *Files identical despite different names*

### Comparing `dataweaver-1.0.4/src/data_weaver/utils.py` & `dataweaver-1.0.5/src/data_weaver/utils.py`

 * *Files identical despite different names*

