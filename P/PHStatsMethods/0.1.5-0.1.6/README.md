# Comparing `tmp/phstatsmethods-0.1.5.tar.gz` & `tmp/phstatsmethods-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phstatsmethods-0.1.5.tar", last modified: Fri May 17 14:46:12 2024, max compression
+gzip compressed data, was "phstatsmethods-0.1.6.tar", last modified: Fri May 17 14:59:38 2024, max compression
```

## Comparing `phstatsmethods-0.1.5.tar` & `phstatsmethods-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:12.591575 phstatsmethods-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35170 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:12.587575 phstatsmethods-0.1.5/PHStatsMethods/
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/DSR.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/ISRate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/ISRatio.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/confidence_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/funnels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/means.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/proportions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/quantiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/utils_funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:12.591575 phstatsmethods-0.1.5/PHStatsMethods.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-17 14:46:12.000000 phstatsmethods-0.1.5/PHStatsMethods.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-17 14:46:12.000000 phstatsmethods-0.1.5/PHStatsMethods.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:46:12.000000 phstatsmethods-0.1.5/PHStatsMethods.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-17 14:46:12.000000 phstatsmethods-0.1.5/PHStatsMethods.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 14:46:12.000000 phstatsmethods-0.1.5/PHStatsMethods.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-17 14:46:12.591575 phstatsmethods-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:46:12.591575 phstatsmethods-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:59:38.135342 phstatsmethods-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35170 2024-05-17 14:59:32.000000 phstatsmethods-0.1.6/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:59:38.131342 phstatsmethods-0.1.6/PHStatsMethods/
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-17 14:59:32.000000 phstatsmethods-0.1.6/PHStatsMethods/DSR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-17 14:59:32.000000 phstatsmethods-0.1.6/PHStatsMethods/ISRate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-17 14:59:32.000000 phstatsmethods-0.1.6/PHStatsMethods/ISRatio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-17 14:59:32.000000 phstatsmethods-0.1.6/PHStatsMethods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-17 14:59:32.000000 phstatsmethods-0.1.6/PHStatsMethods/confidence_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-17 14:59:32.000000 phstatsmethods-0.1.6/PHStatsMethods/funnels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-17 14:59:32.000000 phstatsmethods-0.1.6/PHStatsMethods/means.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-17 14:59:32.000000 phstatsmethods-0.1.6/PHStatsMethods/proportions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-17 14:59:32.000000 phstatsmethods-0.1.6/PHStatsMethods/quantiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-17 14:59:32.000000 phstatsmethods-0.1.6/PHStatsMethods/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-17 14:59:32.000000 phstatsmethods-0.1.6/PHStatsMethods/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-17 14:59:32.000000 phstatsmethods-0.1.6/PHStatsMethods/utils_funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-17 14:59:32.000000 phstatsmethods-0.1.6/PHStatsMethods/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:59:38.135342 phstatsmethods-0.1.6/PHStatsMethods.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-17 14:59:38.000000 phstatsmethods-0.1.6/PHStatsMethods.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-17 14:59:38.000000 phstatsmethods-0.1.6/PHStatsMethods.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:59:38.000000 phstatsmethods-0.1.6/PHStatsMethods.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-17 14:59:38.000000 phstatsmethods-0.1.6/PHStatsMethods.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 14:59:38.000000 phstatsmethods-0.1.6/PHStatsMethods.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-17 14:59:38.135342 phstatsmethods-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:59:38.135342 phstatsmethods-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-17 14:59:32.000000 phstatsmethods-0.1.6/setup.py
```

### Comparing `phstatsmethods-0.1.5/LICENSE.md` & `phstatsmethods-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.5/PHStatsMethods/DSR.py` & `phstatsmethods-0.1.6/PHStatsMethods/DSR.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.5/PHStatsMethods/ISRate.py` & `phstatsmethods-0.1.6/PHStatsMethods/ISRate.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.5/PHStatsMethods/ISRatio.py` & `phstatsmethods-0.1.6/PHStatsMethods/ISRatio.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.5/PHStatsMethods/confidence_intervals.py` & `phstatsmethods-0.1.6/PHStatsMethods/confidence_intervals.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.5/PHStatsMethods/funnels.py` & `phstatsmethods-0.1.6/PHStatsMethods/funnels.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.5/PHStatsMethods/means.py` & `phstatsmethods-0.1.6/PHStatsMethods/means.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.5/PHStatsMethods/proportions.py` & `phstatsmethods-0.1.6/PHStatsMethods/proportions.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.5/PHStatsMethods/quantiles.py` & `phstatsmethods-0.1.6/PHStatsMethods/quantiles.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.5/PHStatsMethods/rates.py` & `phstatsmethods-0.1.6/PHStatsMethods/rates.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.5/PHStatsMethods/utils.py` & `phstatsmethods-0.1.6/PHStatsMethods/utils.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.5/PHStatsMethods/utils_funnel.py` & `phstatsmethods-0.1.6/PHStatsMethods/utils_funnel.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.5/PHStatsMethods/validation.py` & `phstatsmethods-0.1.6/PHStatsMethods/validation.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.5/PHStatsMethods.egg-info/PKG-INFO` & `phstatsmethods-0.1.6/PHStatsMethods.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PHStatsMethods
-Version: 0.1.5
+Version: 0.1.6
 Summary: This is a python package to calculate statistics in public health, including indicators for Fingertips.
 Home-page: https://github.com/DataS-DHSC/PHStatsMethods
 Author: Department of Health and Social Care
 Author-email: annabel.westermann@dhsc.gov.uk, hadley.nanayakkara@dhsc.gov.uk, cameron.stewart@dhsc.gov.uk, jack.burden@dhsc.gov.uk, thilaksan.vikneswaran@dhsc.gov.uk, paul.fryers@dhsc.gov.uk, phds@phe.gov.uk
 License: GPL3
 License-File: LICENSE.md
 Requires-Dist: numpy>=1.24.0
```

### Comparing `phstatsmethods-0.1.5/PHStatsMethods.egg-info/SOURCES.txt` & `phstatsmethods-0.1.6/PHStatsMethods.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.5/PKG-INFO` & `phstatsmethods-0.1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PHStatsMethods
-Version: 0.1.5
+Version: 0.1.6
 Summary: This is a python package to calculate statistics in public health, including indicators for Fingertips.
 Home-page: https://github.com/DataS-DHSC/PHStatsMethods
 Author: Department of Health and Social Care
 Author-email: annabel.westermann@dhsc.gov.uk, hadley.nanayakkara@dhsc.gov.uk, cameron.stewart@dhsc.gov.uk, jack.burden@dhsc.gov.uk, thilaksan.vikneswaran@dhsc.gov.uk, paul.fryers@dhsc.gov.uk, phds@phe.gov.uk
 License: GPL3
 License-File: LICENSE.md
 Requires-Dist: numpy>=1.24.0
```

### Comparing `phstatsmethods-0.1.5/setup.py` & `phstatsmethods-0.1.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='PHStatsMethods',
-    version='0.1.5',
+    version='0.1.6',
     packages=['PHStatsMethods'],
     url='https://github.com/DataS-DHSC/PHStatsMethods',
     license='GPL3',
     author='Department of Health and Social Care',
     author_email='annabel.westermann@dhsc.gov.uk, hadley.nanayakkara@dhsc.gov.uk, cameron.stewart@dhsc.gov.uk, jack.burden@dhsc.gov.uk, thilaksan.vikneswaran@dhsc.gov.uk, paul.fryers@dhsc.gov.uk, phds@phe.gov.uk',
     description='This is a python package to calculate statistics in public health, including indicators for Fingertips.',
     long_description='This is a python package to calculate statistics in public health, including indicators for Fingertips.',
```

