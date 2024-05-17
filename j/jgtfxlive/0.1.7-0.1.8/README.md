# Comparing `tmp/jgtfxlive-0.1.7.tar.gz` & `tmp/jgtfxlive-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jgtfxlive-0.1.7.tar", last modified: Fri May 17 16:35:45 2024, max compression
+gzip compressed data, was "dist/jgtfxlive-0.1.8.tar", last modified: Fri May 17 16:43:45 2024, max compression
```

## Comparing `jgtfxlive-0.1.7.tar` & `jgtfxlive-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:35:45.000000 jgtfxlive-0.1.7/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-05-17 13:33:11.000000 jgtfxlive-0.1.7/LICENSE
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      230 2024-05-17 16:35:45.000000 jgtfxlive-0.1.7/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1797 2024-05-17 14:53:59.000000 jgtfxlive-0.1.7/README.md
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:35:45.000000 jgtfxlive-0.1.7/jgtfxlive/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    15298 2024-05-17 14:21:24.000000 jgtfxlive-0.1.7/jgtfxlive/LiveChartDataExport.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       36 2024-05-17 13:29:20.000000 jgtfxlive-0.1.7/jgtfxlive/__init__.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:35:45.000000 jgtfxlive-0.1.7/jgtfxlive/common_samples/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2987 2024-05-17 13:44:36.000000 jgtfxlive-0.1.7/jgtfxlive/common_samples/BatchOrderMonitor.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     6532 2024-05-17 13:44:36.000000 jgtfxlive-0.1.7/jgtfxlive/common_samples/OrderMonitor.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     7863 2024-05-17 13:44:36.000000 jgtfxlive-0.1.7/jgtfxlive/common_samples/OrderMonitorNetting.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     8644 2024-05-17 13:44:36.000000 jgtfxlive-0.1.7/jgtfxlive/common_samples/TableListenerContainer.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1263 2024-05-17 13:44:36.000000 jgtfxlive-0.1.7/jgtfxlive/common_samples/__init__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     9796 2024-05-17 13:44:36.000000 jgtfxlive-0.1.7/jgtfxlive/common_samples/common.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2827 2024-05-17 15:05:43.000000 jgtfxlive-0.1.7/jgtfxlive/config_generator.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:35:45.000000 jgtfxlive-0.1.7/jgtfxlive/ptoLiveChartDataExport/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    15281 2024-05-17 16:34:53.000000 jgtfxlive-0.1.7/jgtfxlive/ptoLiveChartDataExport/LiveChartDataExport.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       36 2024-05-17 14:04:27.000000 jgtfxlive-0.1.7/jgtfxlive/ptoLiveChartDataExport/__init__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2563 2024-05-17 12:32:37.000000 jgtfxlive-0.1.7/jgtfxlive/ptoLiveChartDataExport/pto_config_generator__240517.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:35:45.000000 jgtfxlive-0.1.7/jgtfxlive.egg-info/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      230 2024-05-17 16:35:45.000000 jgtfxlive-0.1.7/jgtfxlive.egg-info/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      735 2024-05-17 16:35:45.000000 jgtfxlive-0.1.7/jgtfxlive.egg-info/SOURCES.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-05-17 16:35:45.000000 jgtfxlive-0.1.7/jgtfxlive.egg-info/dependency_links.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      136 2024-05-17 16:35:45.000000 jgtfxlive-0.1.7/jgtfxlive.egg-info/entry_points.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       22 2024-05-17 16:35:45.000000 jgtfxlive-0.1.7/jgtfxlive.egg-info/requires.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       10 2024-05-17 16:35:45.000000 jgtfxlive-0.1.7/jgtfxlive.egg-info/top_level.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-05-17 16:35:45.000000 jgtfxlive-0.1.7/setup.cfg
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      645 2024-05-17 16:35:34.000000 jgtfxlive-0.1.7/setup.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-05-17 13:33:11.000000 jgtfxlive-0.1.8/LICENSE
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      230 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1797 2024-05-17 14:53:59.000000 jgtfxlive-0.1.8/README.md
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    15298 2024-05-17 14:21:24.000000 jgtfxlive-0.1.8/jgtfxlive/LiveChartDataExport.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       36 2024-05-17 13:29:20.000000 jgtfxlive-0.1.8/jgtfxlive/__init__.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive/common_samples/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2987 2024-05-17 13:44:36.000000 jgtfxlive-0.1.8/jgtfxlive/common_samples/BatchOrderMonitor.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     6532 2024-05-17 13:44:36.000000 jgtfxlive-0.1.8/jgtfxlive/common_samples/OrderMonitor.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     7863 2024-05-17 13:44:36.000000 jgtfxlive-0.1.8/jgtfxlive/common_samples/OrderMonitorNetting.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     8644 2024-05-17 13:44:36.000000 jgtfxlive-0.1.8/jgtfxlive/common_samples/TableListenerContainer.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1263 2024-05-17 13:44:36.000000 jgtfxlive-0.1.8/jgtfxlive/common_samples/__init__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     9796 2024-05-17 13:44:36.000000 jgtfxlive-0.1.8/jgtfxlive/common_samples/common.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2847 2024-05-17 16:43:14.000000 jgtfxlive-0.1.8/jgtfxlive/config_generator.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive/ptoLiveChartDataExport/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    15281 2024-05-17 16:36:43.000000 jgtfxlive-0.1.8/jgtfxlive/ptoLiveChartDataExport/LiveChartDataExport.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       36 2024-05-17 14:04:27.000000 jgtfxlive-0.1.8/jgtfxlive/ptoLiveChartDataExport/__init__.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive.egg-info/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      230 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive.egg-info/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      670 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      136 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive.egg-info/entry_points.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       22 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive.egg-info/requires.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       10 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/jgtfxlive.egg-info/top_level.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-05-17 16:43:45.000000 jgtfxlive-0.1.8/setup.cfg
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      645 2024-05-17 16:43:41.000000 jgtfxlive-0.1.8/setup.py
```

### Comparing `jgtfxlive-0.1.7/LICENSE` & `jgtfxlive-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.7/README.md` & `jgtfxlive-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.7/jgtfxlive/LiveChartDataExport.py` & `jgtfxlive-0.1.8/jgtfxlive/LiveChartDataExport.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.7/jgtfxlive/common_samples/BatchOrderMonitor.py` & `jgtfxlive-0.1.8/jgtfxlive/common_samples/BatchOrderMonitor.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.7/jgtfxlive/common_samples/OrderMonitor.py` & `jgtfxlive-0.1.8/jgtfxlive/common_samples/OrderMonitor.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.7/jgtfxlive/common_samples/OrderMonitorNetting.py` & `jgtfxlive-0.1.8/jgtfxlive/common_samples/OrderMonitorNetting.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.7/jgtfxlive/common_samples/TableListenerContainer.py` & `jgtfxlive-0.1.8/jgtfxlive/common_samples/TableListenerContainer.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.7/jgtfxlive/common_samples/__init__.py` & `jgtfxlive-0.1.8/jgtfxlive/common_samples/__init__.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.7/jgtfxlive/common_samples/common.py` & `jgtfxlive-0.1.8/jgtfxlive/common_samples/common.py`

 * *Files identical despite different names*

### Comparing `jgtfxlive-0.1.7/jgtfxlive/config_generator.py` & `jgtfxlive-0.1.8/jgtfxlive/config_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,20 +42,20 @@
 
   # Return the XML as a string
   return ET.tostring(config, encoding='utf8', method='xml').decode()
 
 def main():
   import argparse
   parser = argparse.ArgumentParser(description='Generate a configuration file for the ptoLiveChartDataExport')
-  parser.add_argument('--instruments', help='The list of instruments to export (comma-separated)')
-  parser.add_argument('--timeframes', help='The list of timeframes to export (comma-separated)')
-  parser.add_argument('--outxml', type=str,default="jgtfxliveconfig.xml", help='Output XML file')
+  parser.add_argument('-i','--instruments', help='The list of instruments to export (comma-separated)')
+  parser.add_argument('-t','--timeframes', help='The list of timeframes to export (comma-separated)')
+  parser.add_argument('-o','--outxml', type=str,default="jgtfxliveconfig.xml", help='Output XML file')
 
   #data_dir = os.getenv('JGTPY_DATA') or if --data_dir
-  parser.add_argument('--data_dir', help='The directory where the data will be saved')
+  parser.add_argument('-d','--data_dir', help='The directory where the data will be saved')
 
 
 
   args = parser.parse_args()
   instruments = args.instruments
   timeframes = args.timeframes
   data_dir =  args.data_dir or os.getenv('JGTPY_DATA')
```

### Comparing `jgtfxlive-0.1.7/jgtfxlive/ptoLiveChartDataExport/LiveChartDataExport.py` & `jgtfxlive-0.1.8/jgtfxlive/ptoLiveChartDataExport/LiveChartDataExport.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
     dt_separator = find_in_tree(settings, "DateTimeSeparator").text
     if dt_separator == '' or dt_separator is None:
         dt_separator = ' '
     fdp = find_in_tree(settings, "FormatDecimalPlaces").text
     tzone = find_in_tree(settings, "Timezone").text
 
     if tzone != 'EST' and tzone != 'UTC' and tzone != 'Local':
-        print('Timezone is not recognized, using EST')
+        print('Timezone is not recognized, using UTC')
         tzone = 'UTC' #Default timezone
 
     print("=============================")
     print("User ID: " + str_user_id)
     print("URL: " + str_url)
     print("Connection: " + str_connection)
     #print("Session ID: " + str_session_id)
```

### Comparing `jgtfxlive-0.1.7/jgtfxlive.egg-info/SOURCES.txt` & `jgtfxlive-0.1.8/jgtfxlive.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,9 +13,8 @@
 jgtfxlive/common_samples/BatchOrderMonitor.py
 jgtfxlive/common_samples/OrderMonitor.py
 jgtfxlive/common_samples/OrderMonitorNetting.py
 jgtfxlive/common_samples/TableListenerContainer.py
 jgtfxlive/common_samples/__init__.py
 jgtfxlive/common_samples/common.py
 jgtfxlive/ptoLiveChartDataExport/LiveChartDataExport.py
-jgtfxlive/ptoLiveChartDataExport/__init__.py
-jgtfxlive/ptoLiveChartDataExport/pto_config_generator__240517.py
+jgtfxlive/ptoLiveChartDataExport/__init__.py
```

### Comparing `jgtfxlive-0.1.7/setup.py` & `jgtfxlive-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jgtfxlive',
-    version='0.1.7',
+    version='0.1.8',
     author="GUillaume Isabelle",
     author_email="jgi@jgwill.com",
     url="https://github.com/jgwill/jgtfxlive",
     description='A Python module for live chart data export',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
```

