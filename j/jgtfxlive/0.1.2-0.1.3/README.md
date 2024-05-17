# Comparing `tmp/jgtfxlive-0.1.2.tar.gz` & `tmp/jgtfxlive-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jgtfxlive-0.1.2.tar", last modified: Fri May 17 15:01:16 2024, max compression
+gzip compressed data, was "dist/jgtfxlive-0.1.3.tar", last modified: Fri May 17 15:02:25 2024, max compression
```

## Comparing `jgtfxlive-0.1.2.tar` & `jgtfxlive-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 15:01:16.000000 jgtfxlive-0.1.2/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-05-17 13:33:11.000000 jgtfxlive-0.1.2/LICENSE
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      230 2024-05-17 15:01:16.000000 jgtfxlive-0.1.2/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1797 2024-05-17 14:53:59.000000 jgtfxlive-0.1.2/README.md
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 15:01:16.000000 jgtfxlive-0.1.2/jgtfxlive/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    15298 2024-05-17 14:21:24.000000 jgtfxlive-0.1.2/jgtfxlive/LiveChartDataExport.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       36 2024-05-17 13:29:20.000000 jgtfxlive-0.1.2/jgtfxlive/__init__.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 15:01:16.000000 jgtfxlive-0.1.2/jgtfxlive/common_samples/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2987 2024-05-17 13:44:36.000000 jgtfxlive-0.1.2/jgtfxlive/common_samples/BatchOrderMonitor.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     6532 2024-05-17 13:44:36.000000 jgtfxlive-0.1.2/jgtfxlive/common_samples/OrderMonitor.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     7863 2024-05-17 13:44:36.000000 jgtfxlive-0.1.2/jgtfxlive/common_samples/OrderMonitorNetting.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     8644 2024-05-17 13:44:36.000000 jgtfxlive-0.1.2/jgtfxlive/common_samples/TableListenerContainer.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1263 2024-05-17 13:44:36.000000 jgtfxlive-0.1.2/jgtfxlive/common_samples/__init__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     9796 2024-05-17 13:44:36.000000 jgtfxlive-0.1.2/jgtfxlive/common_samples/common.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2806 2024-05-17 13:38:32.000000 jgtfxlive-0.1.2/jgtfxlive/config_generator.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 15:01:16.000000 jgtfxlive-0.1.2/jgtfxlive/ptoLiveChartDataExport/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    15197 2024-05-17 14:49:49.000000 jgtfxlive-0.1.2/jgtfxlive/ptoLiveChartDataExport/LiveChartDataExport.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       36 2024-05-17 14:04:27.000000 jgtfxlive-0.1.2/jgtfxlive/ptoLiveChartDataExport/__init__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2563 2024-05-17 12:32:37.000000 jgtfxlive-0.1.2/jgtfxlive/ptoLiveChartDataExport/pto_config_generator__240517.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 15:01:16.000000 jgtfxlive-0.1.2/jgtfxlive.egg-info/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      230 2024-05-17 15:01:16.000000 jgtfxlive-0.1.2/jgtfxlive.egg-info/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      735 2024-05-17 15:01:16.000000 jgtfxlive-0.1.2/jgtfxlive.egg-info/SOURCES.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-05-17 15:01:16.000000 jgtfxlive-0.1.2/jgtfxlive.egg-info/dependency_links.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      136 2024-05-17 15:01:16.000000 jgtfxlive-0.1.2/jgtfxlive.egg-info/entry_points.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       22 2024-05-17 15:01:16.000000 jgtfxlive-0.1.2/jgtfxlive.egg-info/requires.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       10 2024-05-17 15:01:16.000000 jgtfxlive-0.1.2/jgtfxlive.egg-info/top_level.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-05-17 15:01:16.000000 jgtfxlive-0.1.2/setup.cfg
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      645 2024-05-17 15:00:17.000000 jgtfxlive-0.1.2/setup.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 15:02:25.000000 jgtfxlive-0.1.3/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-05-17 13:33:11.000000 jgtfxlive-0.1.3/LICENSE
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      230 2024-05-17 15:02:25.000000 jgtfxlive-0.1.3/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1797 2024-05-17 14:53:59.000000 jgtfxlive-0.1.3/README.md
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 15:02:25.000000 jgtfxlive-0.1.3/jgtfxlive/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    15298 2024-05-17 14:21:24.000000 jgtfxlive-0.1.3/jgtfxlive/LiveChartDataExport.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       36 2024-05-17 13:29:20.000000 jgtfxlive-0.1.3/jgtfxlive/__init__.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 15:02:25.000000 jgtfxlive-0.1.3/jgtfxlive/common_samples/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2987 2024-05-17 13:44:36.000000 jgtfxlive-0.1.3/jgtfxlive/common_samples/BatchOrderMonitor.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     6532 2024-05-17 13:44:36.000000 jgtfxlive-0.1.3/jgtfxlive/common_samples/OrderMonitor.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     7863 2024-05-17 13:44:36.000000 jgtfxlive-0.1.3/jgtfxlive/common_samples/OrderMonitorNetting.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     8644 2024-05-17 13:44:36.000000 jgtfxlive-0.1.3/jgtfxlive/common_samples/TableListenerContainer.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1263 2024-05-17 13:44:36.000000 jgtfxlive-0.1.3/jgtfxlive/common_samples/__init__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     9796 2024-05-17 13:44:36.000000 jgtfxlive-0.1.3/jgtfxlive/common_samples/common.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2806 2024-05-17 13:38:32.000000 jgtfxlive-0.1.3/jgtfxlive/config_generator.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 15:02:25.000000 jgtfxlive-0.1.3/jgtfxlive/ptoLiveChartDataExport/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    15197 2024-05-17 14:49:49.000000 jgtfxlive-0.1.3/jgtfxlive/ptoLiveChartDataExport/LiveChartDataExport.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       36 2024-05-17 14:04:27.000000 jgtfxlive-0.1.3/jgtfxlive/ptoLiveChartDataExport/__init__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2563 2024-05-17 12:32:37.000000 jgtfxlive-0.1.3/jgtfxlive/ptoLiveChartDataExport/pto_config_generator__240517.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 15:02:25.000000 jgtfxlive-0.1.3/jgtfxlive.egg-info/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      230 2024-05-17 15:02:25.000000 jgtfxlive-0.1.3/jgtfxlive.egg-info/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      735 2024-05-17 15:02:25.000000 jgtfxlive-0.1.3/jgtfxlive.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-05-17 15:02:25.000000 jgtfxlive-0.1.3/jgtfxlive.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      136 2024-05-17 15:02:25.000000 jgtfxlive-0.1.3/jgtfxlive.egg-info/entry_points.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       22 2024-05-17 15:02:25.000000 jgtfxlive-0.1.3/jgtfxlive.egg-info/requires.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       10 2024-05-17 15:02:25.000000 jgtfxlive-0.1.3/jgtfxlive.egg-info/top_level.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-05-17 15:02:25.000000 jgtfxlive-0.1.3/setup.cfg
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      645 2024-05-17 15:02:24.000000 jgtfxlive-0.1.3/setup.py
```

### Comparing `jgtfxlive-0.1.2/LICENSE` & `jgtfxlive-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.2/README.md` & `jgtfxlive-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.2/jgtfxlive/LiveChartDataExport.py` & `jgtfxlive-0.1.3/jgtfxlive/LiveChartDataExport.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.2/jgtfxlive/common_samples/BatchOrderMonitor.py` & `jgtfxlive-0.1.3/jgtfxlive/common_samples/BatchOrderMonitor.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.2/jgtfxlive/common_samples/OrderMonitor.py` & `jgtfxlive-0.1.3/jgtfxlive/common_samples/OrderMonitor.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.2/jgtfxlive/common_samples/OrderMonitorNetting.py` & `jgtfxlive-0.1.3/jgtfxlive/common_samples/OrderMonitorNetting.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.2/jgtfxlive/common_samples/TableListenerContainer.py` & `jgtfxlive-0.1.3/jgtfxlive/common_samples/TableListenerContainer.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.2/jgtfxlive/common_samples/__init__.py` & `jgtfxlive-0.1.3/jgtfxlive/common_samples/__init__.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.2/jgtfxlive/common_samples/common.py` & `jgtfxlive-0.1.3/jgtfxlive/common_samples/common.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.2/jgtfxlive/config_generator.py` & `jgtfxlive-0.1.3/jgtfxlive/config_generator.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.2/jgtfxlive/ptoLiveChartDataExport/LiveChartDataExport.py` & `jgtfxlive-0.1.3/jgtfxlive/ptoLiveChartDataExport/LiveChartDataExport.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.2/jgtfxlive/ptoLiveChartDataExport/pto_config_generator__240517.py` & `jgtfxlive-0.1.3/jgtfxlive/ptoLiveChartDataExport/pto_config_generator__240517.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.2/jgtfxlive.egg-info/SOURCES.txt` & `jgtfxlive-0.1.3/jgtfxlive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.2/setup.py` & `jgtfxlive-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jgtfxlive',
-    version='0.1.2',
+    version='0.1.3',
     author="GUillaume Isabelle",
     author_email="jgi@jgwill.com",
     url="https://github.com/jgwill/jgtfxlive",
     description='A Python module for live chart data export',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
```

