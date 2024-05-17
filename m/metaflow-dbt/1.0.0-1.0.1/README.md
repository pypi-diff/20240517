# Comparing `tmp/metaflow_dbt-1.0.0.tar.gz` & `tmp/metaflow_dbt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow_dbt-1.0.0.tar", last modified: Wed May  8 20:05:24 2024, max compression
+gzip compressed data, was "metaflow_dbt-1.0.1.tar", last modified: Fri May 17 10:18:52 2024, max compression
```

## Comparing `metaflow_dbt-1.0.0.tar` & `metaflow_dbt-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:24.304743 metaflow_dbt-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-08 20:05:15.000000 metaflow_dbt-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-08 20:05:24.304743 metaflow_dbt-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-08 20:05:15.000000 metaflow_dbt-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:24.300743 metaflow_dbt-1.0.0/metaflow_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-08 20:05:24.000000 metaflow_dbt-1.0.0/metaflow_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-08 20:05:24.000000 metaflow_dbt-1.0.0/metaflow_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:05:24.000000 metaflow_dbt-1.0.0/metaflow_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 20:05:24.000000 metaflow_dbt-1.0.0/metaflow_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-08 20:05:24.000000 metaflow_dbt-1.0.0/metaflow_dbt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:24.296743 metaflow_dbt-1.0.0/metaflow_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:24.296743 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:24.300743 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-08 20:05:15.000000 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/cmd/dbt_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-05-08 20:05:15.000000 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/cmd/flow_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:05:15.000000 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/cmd/mfextinit_dbt_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:24.300743 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/config/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-08 20:05:15.000000 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/config/mfextinit_dbt_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:24.300743 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:24.296743 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/plugins/cards/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:24.300743 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/plugins/cards/dbt_docs/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-08 20:05:15.000000 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/plugins/cards/dbt_docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:24.300743 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/plugins/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-08 20:05:15.000000 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/plugins/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-05-08 20:05:15.000000 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/plugins/dbt/dbt_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17940 2024-05-08 20:05:15.000000 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/plugins/dbt/dbt_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 20:05:15.000000 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/plugins/mfextinit_dbt_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:24.300743 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/toplevel/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 20:05:15.000000 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/toplevel/mfextinit_dbt_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-08 20:05:15.000000 metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/toplevel/toplevel.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:05:24.304743 metaflow_dbt-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 20:05:15.000000 metaflow_dbt-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:18:52.165545 metaflow_dbt-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-17 10:18:30.000000 metaflow_dbt-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-17 10:18:52.165545 metaflow_dbt-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-17 10:18:30.000000 metaflow_dbt-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:18:52.165545 metaflow_dbt-1.0.1/metaflow_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-17 10:18:52.000000 metaflow_dbt-1.0.1/metaflow_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-17 10:18:52.000000 metaflow_dbt-1.0.1/metaflow_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 10:18:52.000000 metaflow_dbt-1.0.1/metaflow_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-17 10:18:52.000000 metaflow_dbt-1.0.1/metaflow_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 10:18:52.000000 metaflow_dbt-1.0.1/metaflow_dbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:18:52.157545 metaflow_dbt-1.0.1/metaflow_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:18:52.161545 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:18:52.161545 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-17 10:18:30.000000 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/cmd/dbt_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-05-17 10:18:30.000000 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/cmd/flow_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 10:18:30.000000 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/cmd/mfextinit_dbt_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:18:52.161545 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-17 10:18:30.000000 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/config/mfextinit_dbt_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:18:52.161545 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:18:52.161545 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/plugins/cards/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:18:52.161545 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/plugins/cards/dbt_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-17 10:18:30.000000 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/plugins/cards/dbt_docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:18:52.161545 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/plugins/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-17 10:18:30.000000 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/plugins/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-05-17 10:18:30.000000 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/plugins/dbt/dbt_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17940 2024-05-17 10:18:30.000000 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/plugins/dbt/dbt_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-17 10:18:30.000000 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/plugins/mfextinit_dbt_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:18:52.165545 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/toplevel/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 10:18:30.000000 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/toplevel/mfextinit_dbt_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-17 10:18:30.000000 metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/toplevel/toplevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 10:18:52.165545 metaflow_dbt-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-17 10:18:30.000000 metaflow_dbt-1.0.1/setup.py
```

### Comparing `metaflow_dbt-1.0.0/LICENSE` & `metaflow_dbt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow_dbt-1.0.0/PKG-INFO` & `metaflow_dbt-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-dbt
-Version: 1.0.0
+Version: 1.0.1
 Summary: DBT extension for Metaflow
 Author: Outerbounds
 Author-email: help@outerbounds.co
 License: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `metaflow_dbt-1.0.0/README.md` & `metaflow_dbt-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `metaflow_dbt-1.0.0/metaflow_dbt.egg-info/PKG-INFO` & `metaflow_dbt-1.0.1/metaflow_dbt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-dbt
-Version: 1.0.0
+Version: 1.0.1
 Summary: DBT extension for Metaflow
 Author: Outerbounds
 Author-email: help@outerbounds.co
 License: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `metaflow_dbt-1.0.0/metaflow_dbt.egg-info/SOURCES.txt` & `metaflow_dbt-1.0.1/metaflow_dbt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/cmd/dbt_cmd.py` & `metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/cmd/dbt_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 @click.pass_obj
 def generate(obj, ci=False):
     conf = {
         "project_dir": "./",
         "flow_name": "DBTFlow",
         "remote_config": False,
         "flow_decorators": {
+            # TODO: make this configurable
+            "conda_base": {"attr": 'packages={"dbt-postgres": ">=1.7.0"}'}
             # "trigger_event": False
         },
         "step_decorators": {
             # "secrets": False,
             # "environment": False,
             # "retry": False
         },
```

### Comparing `metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/cmd/flow_generator.py` & `metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/cmd/flow_generator.py`

 * *Files identical despite different names*

### Comparing `metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/plugins/dbt/__init__.py` & `metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/plugins/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/plugins/dbt/dbt_decorator.py` & `metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/plugins/dbt/dbt_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow_dbt-1.0.0/metaflow_extensions/dbt_ext/plugins/dbt/dbt_executor.py` & `metaflow_dbt-1.0.1/metaflow_extensions/dbt_ext/plugins/dbt/dbt_executor.py`

 * *Files identical despite different names*

### Comparing `metaflow_dbt-1.0.0/setup.py` & `metaflow_dbt-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_namespace_packages
 
-version = "1.0.0"
+version = "1.0.1"
 
 setup(
     name="metaflow-dbt",
     version=version,
     description="DBT extension for Metaflow",
     long_description=open("README.md").read(),
     author="Outerbounds",
```

