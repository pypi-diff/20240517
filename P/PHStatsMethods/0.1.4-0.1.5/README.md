# Comparing `tmp/phstatsmethods-0.1.4.tar.gz` & `tmp/phstatsmethods-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phstatsmethods-0.1.4.tar", last modified: Fri May 17 13:56:09 2024, max compression
+gzip compressed data, was "phstatsmethods-0.1.5.tar", last modified: Fri May 17 14:46:12 2024, max compression
```

## Comparing `phstatsmethods-0.1.4.tar` & `phstatsmethods-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:56:09.831334 phstatsmethods-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35170 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:56:09.831334 phstatsmethods-0.1.4/PHStatsMethods.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-17 13:56:09.000000 phstatsmethods-0.1.4/PHStatsMethods.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 13:56:09.000000 phstatsmethods-0.1.4/PHStatsMethods.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:56:09.000000 phstatsmethods-0.1.4/PHStatsMethods.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-17 13:56:09.000000 phstatsmethods-0.1.4/PHStatsMethods.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 13:56:09.000000 phstatsmethods-0.1.4/PHStatsMethods.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-17 13:56:09.831334 phstatsmethods-0.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:56:09.831334 phstatsmethods-0.1.4/ph_statistical_methods/
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/DSR.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/ISRate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/ISRatio.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/confidence_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/funnels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/means.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/proportions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/quantiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/utils_funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/ph_statistical_methods/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 13:56:09.831334 phstatsmethods-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-17 13:56:03.000000 phstatsmethods-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:12.591575 phstatsmethods-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35170 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:12.587575 phstatsmethods-0.1.5/PHStatsMethods/
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/DSR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/ISRate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/ISRatio.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/confidence_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/funnels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/means.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/proportions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/quantiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/utils_funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/PHStatsMethods/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:12.591575 phstatsmethods-0.1.5/PHStatsMethods.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-17 14:46:12.000000 phstatsmethods-0.1.5/PHStatsMethods.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-17 14:46:12.000000 phstatsmethods-0.1.5/PHStatsMethods.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:46:12.000000 phstatsmethods-0.1.5/PHStatsMethods.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-17 14:46:12.000000 phstatsmethods-0.1.5/PHStatsMethods.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 14:46:12.000000 phstatsmethods-0.1.5/PHStatsMethods.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-17 14:46:12.591575 phstatsmethods-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:46:12.591575 phstatsmethods-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-17 14:46:08.000000 phstatsmethods-0.1.5/setup.py
```

### Comparing `phstatsmethods-0.1.4/LICENSE.md` & `phstatsmethods-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.4/ph_statistical_methods/DSR.py` & `phstatsmethods-0.1.5/PHStatsMethods/DSR.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.4/ph_statistical_methods/ISRate.py` & `phstatsmethods-0.1.5/PHStatsMethods/ISRate.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.4/ph_statistical_methods/ISRatio.py` & `phstatsmethods-0.1.5/PHStatsMethods/ISRatio.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.4/ph_statistical_methods/confidence_intervals.py` & `phstatsmethods-0.1.5/PHStatsMethods/confidence_intervals.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.4/ph_statistical_methods/funnels.py` & `phstatsmethods-0.1.5/PHStatsMethods/funnels.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.4/ph_statistical_methods/means.py` & `phstatsmethods-0.1.5/PHStatsMethods/means.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.4/ph_statistical_methods/proportions.py` & `phstatsmethods-0.1.5/PHStatsMethods/proportions.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.4/ph_statistical_methods/quantiles.py` & `phstatsmethods-0.1.5/PHStatsMethods/quantiles.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.4/ph_statistical_methods/rates.py` & `phstatsmethods-0.1.5/PHStatsMethods/rates.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.4/ph_statistical_methods/utils.py` & `phstatsmethods-0.1.5/PHStatsMethods/utils.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.4/ph_statistical_methods/utils_funnel.py` & `phstatsmethods-0.1.5/PHStatsMethods/utils_funnel.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.4/ph_statistical_methods/validation.py` & `phstatsmethods-0.1.5/PHStatsMethods/validation.py`

 * *Files identical despite different names*

