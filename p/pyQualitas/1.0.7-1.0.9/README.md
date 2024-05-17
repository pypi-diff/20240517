# Comparing `tmp/pyQualitas-1.0.7.tar.gz` & `tmp/pyqualitas-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyQualitas-1.0.7.tar", last modified: Thu Nov 17 07:54:42 2022, max compression
+gzip compressed data, was "pyqualitas-1.0.9.tar", last modified: Fri May 17 15:13:00 2024, max compression
```

## Comparing `pyQualitas-1.0.7.tar` & `pyqualitas-1.0.9.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 07:54:42.210016 pyQualitas-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-11-17 07:53:34.000000 pyQualitas-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2070 2022-11-17 07:54:42.210016 pyQualitas-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-11-17 07:53:34.000000 pyQualitas-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 07:54:42.210016 pyQualitas-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-11-17 07:53:34.000000 pyQualitas-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 07:54:42.202016 pyQualitas-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 07:54:42.206016 pyQualitas-1.0.7/src/pyQualitas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2070 2022-11-17 07:54:42.000000 pyQualitas-1.0.7/src/pyQualitas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-11-17 07:54:42.000000 pyQualitas-1.0.7/src/pyQualitas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 07:54:42.000000 pyQualitas-1.0.7/src/pyQualitas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-11-17 07:54:42.000000 pyQualitas-1.0.7/src/pyQualitas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-17 07:54:42.000000 pyQualitas-1.0.7/src/pyQualitas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 07:54:42.206016 pyQualitas-1.0.7/src/pyqualitas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 07:53:34.000000 pyQualitas-1.0.7/src/pyqualitas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 07:54:42.206016 pyQualitas-1.0.7/src/pyqualitas/checks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 07:53:34.000000 pyQualitas-1.0.7/src/pyqualitas/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-11-17 07:53:34.000000 pyQualitas-1.0.7/src/pyqualitas/checks/arbitarychecks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5966 2022-11-17 07:53:34.000000 pyQualitas-1.0.7/src/pyqualitas/checks/dualdfchecks.py
--rw-r--r--   0 runner    (1001) docker     (121)    14702 2022-11-17 07:53:34.000000 pyQualitas-1.0.7/src/pyqualitas/checks/singledfchecks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 07:54:42.210016 pyQualitas-1.0.7/src/pyqualitas/checksuite/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 07:53:34.000000 pyQualitas-1.0.7/src/pyqualitas/checksuite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-11-17 07:53:34.000000 pyQualitas-1.0.7/src/pyqualitas/checksuite/checksuite.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 07:54:42.210016 pyQualitas-1.0.7/src/pyqualitas/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 07:53:34.000000 pyQualitas-1.0.7/src/pyqualitas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7346 2022-11-17 07:53:34.000000 pyQualitas-1.0.7/src/pyqualitas/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-11-17 07:53:34.000000 pyQualitas-1.0.7/src/pyqualitas/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 07:54:42.210016 pyQualitas-1.0.7/src/pyqualitas/utils/template/
--rw-r--r--   0 runner    (1001) docker     (121)     2496 2022-11-17 07:53:34.000000 pyQualitas-1.0.7/src/pyqualitas/utils/template/TestResult.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:13:00.136782 pyqualitas-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-17 15:13:00.136782 pyqualitas-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 15:13:00.136782 pyqualitas-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:13:00.132782 pyqualitas-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:13:00.136782 pyqualitas-1.0.9/src/pyQualitas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-17 15:13:00.000000 pyqualitas-1.0.9/src/pyQualitas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-17 15:13:00.000000 pyqualitas-1.0.9/src/pyQualitas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:13:00.000000 pyqualitas-1.0.9/src/pyQualitas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-17 15:13:00.000000 pyqualitas-1.0.9/src/pyQualitas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-17 15:13:00.000000 pyqualitas-1.0.9/src/pyQualitas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:13:00.132782 pyqualitas-1.0.9/src/pyqualitas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/src/pyqualitas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:13:00.132782 pyqualitas-1.0.9/src/pyqualitas/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/src/pyqualitas/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/src/pyqualitas/checks/arbitarychecks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/src/pyqualitas/checks/dualdfchecks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14799 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/src/pyqualitas/checks/singledfchecks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:13:00.132782 pyqualitas-1.0.9/src/pyqualitas/checksuite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/src/pyqualitas/checksuite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/src/pyqualitas/checksuite/checksuite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:13:00.136782 pyqualitas-1.0.9/src/pyqualitas/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/src/pyqualitas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/src/pyqualitas/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/src/pyqualitas/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:13:00.136782 pyqualitas-1.0.9/src/pyqualitas/utils/template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/src/pyqualitas/utils/template/TestResult.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:13:00.136782 pyqualitas-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/tests/test_arbitarychecks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/tests/test_checksuite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/tests/test_dualdfchecks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-05-17 15:08:45.000000 pyqualitas-1.0.9/tests/test_singledfchecks.py
```

### Comparing `pyQualitas-1.0.7/LICENSE` & `pyqualitas-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyQualitas-1.0.7/PKG-INFO` & `pyqualitas-1.0.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: pyQualitas
-Version: 1.0.7
-Summary: A project to ensure the data quality using python
-Home-page: https://github.com/IamVenkatesh/pyQuality/wiki
-Author: Venkatesh Venkataramani
-Author-email: venkatesh.venkataramani@gmail.com
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Software Development :: Testing
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 **PyQualitas**
 
 This project aims towards developing a python library ensure quality of the data. This project is an inspiration from deequ and 
 dataflare which are also aimed towards the quality of the data.
 
 **Requirements:**
```

### Comparing `pyQualitas-1.0.7/setup.py` & `pyqualitas-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyQualitas",
-    version="1.0.7",
+    version="1.0.9",
     description="A project to ensure the data quality using python",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Venkatesh Venkataramani",
     author_email="venkatesh.venkataramani@gmail.com",
     url="https://github.com/IamVenkatesh/pyQuality/wiki",
     packages=['pyqualitas', 'pyqualitas/checks', 'pyqualitas/checksuite', 'pyqualitas/utils'],
```

### Comparing `pyQualitas-1.0.7/src/pyqualitas/checks/dualdfchecks.py` & `pyqualitas-1.0.9/src/pyqualitas/checks/dualdfchecks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import os
 from pyqualitas.utils.logger import CustomLogger
 
 
 class DualDataFrameChecks:
     """
         Summary: This class can be instantiated to perform checks available under this class to compare 2 different
         dataframes. The class expects the dataframes to be passed as a parameter during the instantiation.
@@ -11,14 +12,16 @@
         The default log level is 10: Debug.
 
         """
 
     def __init__(self, df1, df2, log_file_location='dualdfchecks.log'):
         self.df1 = df1
         self.df2 = df2
+        if os.path.exists(log_file_location):
+            os.remove(log_file_location)
         if not logging.getLogger(__name__).hasHandlers():
             self.logger_instance = CustomLogger(log_file_location, 10, __name__)
             self.logger = self.logger_instance.instantiate()
         else:
             self.logger = logging.getLogger(__name__)
 
     def check_columns(self):
```

### Comparing `pyQualitas-1.0.7/src/pyqualitas/checks/singledfchecks.py` & `pyqualitas-1.0.9/src/pyqualitas/checks/singledfchecks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import os
 from pyspark.sql import functions
 from pyspark.sql.functions import sum, col, rank, collect_list, asc
 from pyspark.sql.window import Window
 from pyqualitas.utils.logger import CustomLogger
 
 
 class SingleDataFrameChecks:
@@ -13,14 +14,16 @@
     The default log file name is singledfchecks.log. The default log level is 10: Debug.
 
     """
 
     def __init__(self, dataframe, log_file_location='singledfchecks.log'):
 
         self.dataframe = dataframe
+        if os.path.exists(log_file_location):
+            os.remove(log_file_location)
         if not logging.getLogger(__name__).hasHandlers():
             self.logger_instance = CustomLogger(log_file_location, 10, __name__)
             self.logger = self.logger_instance.instantiate()
         else:
             self.logger = logging.getLogger(__name__)
 
     def check_duplicates(self, columns = None):
```

### Comparing `pyQualitas-1.0.7/src/pyqualitas/checksuite/checksuite.py` & `pyqualitas-1.0.9/src/pyqualitas/checksuite/checksuite.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from time import sleep
 
 
 class CheckSuite:
 
-    def __init__(self, checks, retries=10, sleep_time=60):
+    def __init__(self, checks, sleep_time=60):
         self.checks = checks
-        self.retries = retries
         self.sleep_time = sleep_time
         self.results_list = []
 
     def collect_result(self):
         """
         Summary: This function collects the result of the test checks defined by the user
 
         Parameters: Number of retries and the wait time for the tests to complete the execution. Default value is 10, 60
 
-        Output: Returns a List of Tuples with Test Case Name, Test Description and Test Result
+        Output: Returns a List with Test Case Name, Test Description and Test Result
         """
-        for test_name, values in self.checks.items():
-            for test_description, result in values.items():
-                retry_count = 0
-                while retry_count <= self.retries:
-                    if result not in ["Passed", "Failed"]:
-                        sleep(self.sleep_time)
-                        retry_count += 1
-                    else:
+        total_test = len(self.checks)
+        while total_test > 0:
+            for test_name, values in self.checks.items():
+                for test_description, result in values.items():
+                    if result in ["Passed", "Failed"]:
+                        total_test = total_test - 1
                         self.results_list.append([test_name, test_description, result])
-                        break
+                    else:
+                        continue
+            sleep(self.sleep_time)
+                        
         return self.results_list
```

### Comparing `pyQualitas-1.0.7/src/pyqualitas/utils/helper.py` & `pyqualitas-1.0.9/src/pyqualitas/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pyQualitas-1.0.7/src/pyqualitas/utils/logger.py` & `pyqualitas-1.0.9/src/pyqualitas/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyQualitas-1.0.7/src/pyqualitas/utils/template/TestResult.html` & `pyqualitas-1.0.9/src/pyqualitas/utils/template/TestResult.html`

 * *Files identical despite different names*

