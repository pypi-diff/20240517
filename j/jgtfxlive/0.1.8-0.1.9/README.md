# Comparing `tmp/jgtfxlive-0.1.8.tar.gz` & `tmp/jgtfxlive-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jgtfxlive-0.1.8.tar", last modified: Fri May 17 16:43:45 2024, max compression
+gzip compressed data, was "dist/jgtfxlive-0.1.9.tar", last modified: Fri May 17 16:53:59 2024, max compression
```

## Comparing `jgtfxlive-0.1.8.tar` & `jgtfxlive-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-05-17 13:33:11.000000 jgtfxlive-0.1.8/LICENSE
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      230 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1797 2024-05-17 14:53:59.000000 jgtfxlive-0.1.8/README.md
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    15298 2024-05-17 14:21:24.000000 jgtfxlive-0.1.8/jgtfxlive/LiveChartDataExport.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       36 2024-05-17 13:29:20.000000 jgtfxlive-0.1.8/jgtfxlive/__init__.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive/common_samples/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2987 2024-05-17 13:44:36.000000 jgtfxlive-0.1.8/jgtfxlive/common_samples/BatchOrderMonitor.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     6532 2024-05-17 13:44:36.000000 jgtfxlive-0.1.8/jgtfxlive/common_samples/OrderMonitor.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     7863 2024-05-17 13:44:36.000000 jgtfxlive-0.1.8/jgtfxlive/common_samples/OrderMonitorNetting.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     8644 2024-05-17 13:44:36.000000 jgtfxlive-0.1.8/jgtfxlive/common_samples/TableListenerContainer.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1263 2024-05-17 13:44:36.000000 jgtfxlive-0.1.8/jgtfxlive/common_samples/__init__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     9796 2024-05-17 13:44:36.000000 jgtfxlive-0.1.8/jgtfxlive/common_samples/common.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2847 2024-05-17 16:43:14.000000 jgtfxlive-0.1.8/jgtfxlive/config_generator.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive/ptoLiveChartDataExport/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    15281 2024-05-17 16:36:43.000000 jgtfxlive-0.1.8/jgtfxlive/ptoLiveChartDataExport/LiveChartDataExport.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       36 2024-05-17 14:04:27.000000 jgtfxlive-0.1.8/jgtfxlive/ptoLiveChartDataExport/__init__.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive.egg-info/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      230 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive.egg-info/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      670 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive.egg-info/SOURCES.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive.egg-info/dependency_links.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      136 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive.egg-info/entry_points.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       22 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive.egg-info/requires.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       10 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive.egg-info/top_level.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/setup.cfg
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      645 2024-05-17 16:43:41.000000 jgtfxlive-0.1.8/setup.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:53:59.000000 jgtfxlive-0.1.9/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-05-17 13:33:11.000000 jgtfxlive-0.1.9/LICENSE
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      230 2024-05-17 16:53:59.000000 jgtfxlive-0.1.9/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1797 2024-05-17 14:53:59.000000 jgtfxlive-0.1.9/README.md
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:53:59.000000 jgtfxlive-0.1.9/jgtfxlive/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    15298 2024-05-17 14:21:24.000000 jgtfxlive-0.1.9/jgtfxlive/LiveChartDataExport.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       36 2024-05-17 13:29:20.000000 jgtfxlive-0.1.9/jgtfxlive/__init__.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:53:59.000000 jgtfxlive-0.1.9/jgtfxlive/common_samples/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2987 2024-05-17 13:44:36.000000 jgtfxlive-0.1.9/jgtfxlive/common_samples/BatchOrderMonitor.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     6532 2024-05-17 13:44:36.000000 jgtfxlive-0.1.9/jgtfxlive/common_samples/OrderMonitor.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     7863 2024-05-17 13:44:36.000000 jgtfxlive-0.1.9/jgtfxlive/common_samples/OrderMonitorNetting.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     8644 2024-05-17 13:44:36.000000 jgtfxlive-0.1.9/jgtfxlive/common_samples/TableListenerContainer.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1263 2024-05-17 13:44:36.000000 jgtfxlive-0.1.9/jgtfxlive/common_samples/__init__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     9796 2024-05-17 13:44:36.000000 jgtfxlive-0.1.9/jgtfxlive/common_samples/common.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2844 2024-05-17 16:53:00.000000 jgtfxlive-0.1.9/jgtfxlive/config_generator.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:53:59.000000 jgtfxlive-0.1.9/jgtfxlive/ptoLiveChartDataExport/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    15278 2024-05-17 16:53:40.000000 jgtfxlive-0.1.9/jgtfxlive/ptoLiveChartDataExport/LiveChartDataExport.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       36 2024-05-17 14:04:27.000000 jgtfxlive-0.1.9/jgtfxlive/ptoLiveChartDataExport/__init__.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:53:59.000000 jgtfxlive-0.1.9/jgtfxlive.egg-info/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      230 2024-05-17 16:53:59.000000 jgtfxlive-0.1.9/jgtfxlive.egg-info/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      670 2024-05-17 16:53:59.000000 jgtfxlive-0.1.9/jgtfxlive.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-05-17 16:53:59.000000 jgtfxlive-0.1.9/jgtfxlive.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      136 2024-05-17 16:53:59.000000 jgtfxlive-0.1.9/jgtfxlive.egg-info/entry_points.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       22 2024-05-17 16:53:59.000000 jgtfxlive-0.1.9/jgtfxlive.egg-info/requires.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       10 2024-05-17 16:53:59.000000 jgtfxlive-0.1.9/jgtfxlive.egg-info/top_level.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-05-17 16:53:59.000000 jgtfxlive-0.1.9/setup.cfg
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      645 2024-05-17 16:53:58.000000 jgtfxlive-0.1.9/setup.py
```

### Comparing `jgtfxlive-0.1.8/LICENSE` & `jgtfxlive-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.8/README.md` & `jgtfxlive-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.8/jgtfxlive/LiveChartDataExport.py` & `jgtfxlive-0.1.9/jgtfxlive/LiveChartDataExport.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.8/jgtfxlive/common_samples/BatchOrderMonitor.py` & `jgtfxlive-0.1.9/jgtfxlive/common_samples/BatchOrderMonitor.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.8/jgtfxlive/common_samples/OrderMonitor.py` & `jgtfxlive-0.1.9/jgtfxlive/common_samples/OrderMonitor.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.8/jgtfxlive/common_samples/OrderMonitorNetting.py` & `jgtfxlive-0.1.9/jgtfxlive/common_samples/OrderMonitorNetting.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.8/jgtfxlive/common_samples/TableListenerContainer.py` & `jgtfxlive-0.1.9/jgtfxlive/common_samples/TableListenerContainer.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.8/jgtfxlive/common_samples/__init__.py` & `jgtfxlive-0.1.9/jgtfxlive/common_samples/__init__.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.8/jgtfxlive/common_samples/common.py` & `jgtfxlive-0.1.9/jgtfxlive/common_samples/common.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.8/jgtfxlive/config_generator.py` & `jgtfxlive-0.1.9/jgtfxlive/config_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
   return ET.tostring(config, encoding='utf8', method='xml').decode()
 
 def main():
   import argparse
   parser = argparse.ArgumentParser(description='Generate a configuration file for the ptoLiveChartDataExport')
   parser.add_argument('-i','--instruments', help='The list of instruments to export (comma-separated)')
   parser.add_argument('-t','--timeframes', help='The list of timeframes to export (comma-separated)')
-  parser.add_argument('-o','--outxml', type=str,default="jgtfxliveconfig.xml", help='Output XML file')
+  parser.add_argument('-o','--outxml', type=str,default="fxliveconfig.xml", help='Output XML file')
 
   #data_dir = os.getenv('JGTPY_DATA') or if --data_dir
   parser.add_argument('-d','--data_dir', help='The directory where the data will be saved')
 
 
 
   args = parser.parse_args()
```

### Comparing `jgtfxlive-0.1.8/jgtfxlive/ptoLiveChartDataExport/LiveChartDataExport.py` & `jgtfxlive-0.1.9/jgtfxlive/ptoLiveChartDataExport/LiveChartDataExport.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 def parse_args():
     arg_parser = argparse.ArgumentParser(description='Process command parameters.')
     arg_parser.add_argument('-p',
                             metavar="PASSWORD",
                             required=False,
                             help='Your password.')
-    arg_parser.add_argument('-config', metavar="CONFIG_FILE", default='jgtfxliveconfig.xml',
+    arg_parser.add_argument('-config', metavar="CONFIG_FILE", default='fxliveconfig.xml',
                             help='Config file')
 
     args = arg_parser.parse_args()
     return args
 
 
 verbose = 0
```

### Comparing `jgtfxlive-0.1.8/jgtfxlive.egg-info/SOURCES.txt` & `jgtfxlive-0.1.9/jgtfxlive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.8/setup.py` & `jgtfxlive-0.1.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jgtfxlive',
-    version='0.1.8',
+    version='0.1.9',
     author="GUillaume Isabelle",
     author_email="jgi@jgwill.com",
     url="https://github.com/jgwill/jgtfxlive",
     description='A Python module for live chart data export',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
```

