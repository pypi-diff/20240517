# Comparing `tmp/phstatsmethods-0.1.3.tar.gz` & `tmp/phstatsmethods-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phstatsmethods-0.1.3.tar", last modified: Fri May 17 13:54:24 2024, max compression
+gzip compressed data, was "phstatsmethods-0.1.4.tar", last modified: Fri May 17 13:56:09 2024, max compression
```

## Comparing `phstatsmethods-0.1.3.tar` & `phstatsmethods-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:54:24.414511 phstatsmethods-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35170 2024-05-17 13:54:21.000000 phstatsmethods-0.1.3/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:54:24.410511 phstatsmethods-0.1.3/PHStatsMethods.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-17 13:54:24.000000 phstatsmethods-0.1.3/PHStatsMethods.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 13:54:24.000000 phstatsmethods-0.1.3/PHStatsMethods.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:54:24.000000 phstatsmethods-0.1.3/PHStatsMethods.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-17 13:54:24.000000 phstatsmethods-0.1.3/PHStatsMethods.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 13:54:24.000000 phstatsmethods-0.1.3/PHStatsMethods.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-17 13:54:24.414511 phstatsmethods-0.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:54:24.410511 phstatsmethods-0.1.3/ph_statistical_methods/
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-17 13:54:21.000000 phstatsmethods-0.1.3/ph_statistical_methods/DSR.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-17 13:54:21.000000 phstatsmethods-0.1.3/ph_statistical_methods/ISRate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-17 13:54:21.000000 phstatsmethods-0.1.3/ph_statistical_methods/ISRatio.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:54:21.000000 phstatsmethods-0.1.3/ph_statistical_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-17 13:54:21.000000 phstatsmethods-0.1.3/ph_statistical_methods/confidence_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-17 13:54:21.000000 phstatsmethods-0.1.3/ph_statistical_methods/funnels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-17 13:54:21.000000 phstatsmethods-0.1.3/ph_statistical_methods/means.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-17 13:54:21.000000 phstatsmethods-0.1.3/ph_statistical_methods/proportions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-17 13:54:21.000000 phstatsmethods-0.1.3/ph_statistical_methods/quantiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-17 13:54:21.000000 phstatsmethods-0.1.3/ph_statistical_methods/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-17 13:54:21.000000 phstatsmethods-0.1.3/ph_statistical_methods/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-17 13:54:21.000000 phstatsmethods-0.1.3/ph_statistical_methods/utils_funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-17 13:54:21.000000 phstatsmethods-0.1.3/ph_statistical_methods/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 13:54:24.414511 phstatsmethods-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-17 13:54:21.000000 phstatsmethods-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:56:09.831334 phstatsmethods-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35170 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:56:09.831334 phstatsmethods-0.1.4/PHStatsMethods.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-17 13:56:09.000000 phstatsmethods-0.1.4/PHStatsMethods.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 13:56:09.000000 phstatsmethods-0.1.4/PHStatsMethods.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:56:09.000000 phstatsmethods-0.1.4/PHStatsMethods.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-17 13:56:09.000000 phstatsmethods-0.1.4/PHStatsMethods.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 13:56:09.000000 phstatsmethods-0.1.4/PHStatsMethods.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-17 13:56:09.831334 phstatsmethods-0.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:56:09.831334 phstatsmethods-0.1.4/ph_statistical_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/DSR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/ISRate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/ISRatio.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/confidence_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/funnels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/means.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/proportions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/quantiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/utils_funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 13:56:09.831334 phstatsmethods-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/setup.py
```

### Comparing `phstatsmethods-0.1.3/LICENSE.md` & `phstatsmethods-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.3/PHStatsMethods.egg-info/PKG-INFO` & `phstatsmethods-0.1.4/PHStatsMethods.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PHStatsMethods
-Version: 0.1.3
+Version: 0.1.4
 Summary: This is a python package to calculate statistics in public health, including indicators for Fingertips.
 Home-page: https://github.com/DataS-DHSC/PH_statistical_methods
 Author: Department of Health and Social Care
 Author-email: annabel.westermann@dhsc.gov.uk, phds@phe.gov.uk
 License: GPL3
 License-File: LICENSE.md
 Requires-Dist: numpy>=1.24.0
```

### Comparing `phstatsmethods-0.1.3/PHStatsMethods.egg-info/SOURCES.txt` & `phstatsmethods-0.1.4/PHStatsMethods.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.3/PKG-INFO` & `phstatsmethods-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PHStatsMethods
-Version: 0.1.3
+Version: 0.1.4
 Summary: This is a python package to calculate statistics in public health, including indicators for Fingertips.
 Home-page: https://github.com/DataS-DHSC/PH_statistical_methods
 Author: Department of Health and Social Care
 Author-email: annabel.westermann@dhsc.gov.uk, phds@phe.gov.uk
 License: GPL3
 License-File: LICENSE.md
 Requires-Dist: numpy>=1.24.0
```

### Comparing `phstatsmethods-0.1.3/ph_statistical_methods/DSR.py` & `phstatsmethods-0.1.4/ph_statistical_methods/DSR.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.3/ph_statistical_methods/ISRate.py` & `phstatsmethods-0.1.4/ph_statistical_methods/ISRate.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.3/ph_statistical_methods/ISRatio.py` & `phstatsmethods-0.1.4/ph_statistical_methods/ISRatio.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.3/ph_statistical_methods/confidence_intervals.py` & `phstatsmethods-0.1.4/ph_statistical_methods/confidence_intervals.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.3/ph_statistical_methods/funnels.py` & `phstatsmethods-0.1.4/ph_statistical_methods/funnels.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.3/ph_statistical_methods/means.py` & `phstatsmethods-0.1.4/ph_statistical_methods/means.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.3/ph_statistical_methods/proportions.py` & `phstatsmethods-0.1.4/ph_statistical_methods/proportions.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.3/ph_statistical_methods/quantiles.py` & `phstatsmethods-0.1.4/ph_statistical_methods/quantiles.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.3/ph_statistical_methods/rates.py` & `phstatsmethods-0.1.4/ph_statistical_methods/rates.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.3/ph_statistical_methods/utils.py` & `phstatsmethods-0.1.4/ph_statistical_methods/utils.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.3/ph_statistical_methods/utils_funnel.py` & `phstatsmethods-0.1.4/ph_statistical_methods/utils_funnel.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.3/ph_statistical_methods/validation.py` & `phstatsmethods-0.1.4/ph_statistical_methods/validation.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.3/setup.py` & `phstatsmethods-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='PHStatsMethods',
-    version='0.1.3',
+    version='0.1.4',
     packages=['ph_statistical_methods'],
     url='https://github.com/DataS-DHSC/PH_statistical_methods',
     license='GPL3',
     author='Department of Health and Social Care',
     author_email='annabel.westermann@dhsc.gov.uk, phds@phe.gov.uk',
     description='This is a python package to calculate statistics in public health, including indicators for Fingertips.',
     long_description='longer description',
```

