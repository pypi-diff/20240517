# Comparing `tmp/mosaik-csv-2.0.0.tar.gz` & `tmp/mosaik-csv-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaik-csv-2.0.0.tar", last modified: Tue Nov 21 14:38:39 2023, max compression
+gzip compressed data, was "mosaik-csv-2.0.1.tar", last modified: Fri May 17 08:13:28 2024, max compression
```

## Comparing `mosaik-csv-2.0.0.tar` & `mosaik-csv-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 14:38:39.709509 mosaik-csv-2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-11-21 14:38:16.000000 mosaik-csv-2.0.0/AUTHORS.txt
--rw-rw-rw-   0 root         (0) root         (0)      755 2023-11-21 14:38:16.000000 mosaik-csv-2.0.0/CHANGES.txt
--rw-rw-rw-   0 root         (0) root         (0)    24436 2023-11-21 14:38:16.000000 mosaik-csv-2.0.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-11-21 14:38:16.000000 mosaik-csv-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4845 2023-11-21 14:38:39.709509 mosaik-csv-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2798 2023-11-21 14:38:16.000000 mosaik-csv-2.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-21 14:38:39.709509 mosaik-csv-2.0.0/mosaik_csv.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4845 2023-11-21 14:38:39.000000 mosaik-csv-2.0.0/mosaik_csv.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      343 2023-11-21 14:38:39.000000 mosaik-csv-2.0.0/mosaik_csv.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-21 14:38:39.000000 mosaik-csv-2.0.0/mosaik_csv.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-11-21 14:38:39.000000 mosaik-csv-2.0.0/mosaik_csv.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-11-21 14:38:39.000000 mosaik-csv-2.0.0/mosaik_csv.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-11-21 14:38:39.000000 mosaik-csv-2.0.0/mosaik_csv.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     4254 2023-11-21 14:38:16.000000 mosaik-csv-2.0.0/mosaik_csv.py
--rw-rw-rw-   0 root         (0) root         (0)     3763 2023-11-21 14:38:16.000000 mosaik-csv-2.0.0/mosaik_csv_writer.py
--rw-rw-rw-   0 root         (0) root         (0)      530 2023-11-21 14:38:16.000000 mosaik-csv-2.0.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-11-21 14:38:39.709509 mosaik-csv-2.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1515 2023-11-21 14:38:16.000000 mosaik-csv-2.0.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-11-21 14:38:16.000000 mosaik-csv-2.0.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:13:28.355217 mosaik-csv-2.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-05-17 08:13:04.000000 mosaik-csv-2.0.1/AUTHORS.txt
+-rw-rw-rw-   0 root         (0) root         (0)      850 2024-05-17 08:13:04.000000 mosaik-csv-2.0.1/CHANGES.txt
+-rw-rw-rw-   0 root         (0) root         (0)    24436 2024-05-17 08:13:04.000000 mosaik-csv-2.0.1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-17 08:13:04.000000 mosaik-csv-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4874 2024-05-17 08:13:28.355217 mosaik-csv-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2732 2024-05-17 08:13:04.000000 mosaik-csv-2.0.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:13:28.355217 mosaik-csv-2.0.1/mosaik_csv.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4874 2024-05-17 08:13:28.000000 mosaik-csv-2.0.1/mosaik_csv.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      343 2024-05-17 08:13:28.000000 mosaik-csv-2.0.1/mosaik_csv.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 08:13:28.000000 mosaik-csv-2.0.1/mosaik_csv.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2024-05-17 08:13:28.000000 mosaik-csv-2.0.1/mosaik_csv.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-05-17 08:13:28.000000 mosaik-csv-2.0.1/mosaik_csv.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-17 08:13:28.000000 mosaik-csv-2.0.1/mosaik_csv.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4476 2024-05-17 08:13:04.000000 mosaik-csv-2.0.1/mosaik_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     3763 2024-05-17 08:13:04.000000 mosaik-csv-2.0.1/mosaik_csv_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)      530 2024-05-17 08:13:04.000000 mosaik-csv-2.0.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-05-17 08:13:28.356217 mosaik-csv-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2024-05-17 08:13:04.000000 mosaik-csv-2.0.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-17 08:13:04.000000 mosaik-csv-2.0.1/tox.ini
```

### Comparing `mosaik-csv-2.0.0/CHANGES.txt` & `mosaik-csv-2.0.1/CHANGES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+2.0.1 - 2024-05-17
+------------------
+ - [BUGFIX] Convert numpy data types to python scalars.
+
 2.0.0 - 2023-11-21
 ------------------
 
 - [CHANGE] Use pandas for CSV reader.
 - [NEW] Add CSV writer.
```

### Comparing `mosaik-csv-2.0.0/LICENSE.txt` & `mosaik-csv-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mosaik-csv-2.0.0/PKG-INFO` & `mosaik-csv-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaik-csv
-Version: 2.0.0
+Version: 2.0.1
 Summary: Presents CSV datasets to mosaik as models.
 Home-page: https://gitlab.com/mosaik/components/data/mosaik-csv
 Author: mosaik development team
 Author-email: mosaik@offis.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -77,17 +77,16 @@
         'CSV_writer': {
             'python': 'mosaik_csv_writer:CSVWriter',
         }
     }
     world = mosaik.World(sim_config)
     csv_sim_writer = world.start('CSV_writer', start_date = '01.01.2016 00:00',
                                                date_format='%Y-%m-%d %H:%M:%S', 
-                                               output_file='results.csv',
-                                               print_results=False)
-    csv_writer = csv_sim_writer.Monitor(buff_size = 30 * 60)  # write data after every 30 mins
+                                               output_file='results.csv')
+    csv_writer = csv_sim_writer.CSVWriter(buff_size = 30 * 60)  # write data after every 30 mins
 
 Tests
 =====
 
 You can run the tests with::
 
     $ git clone https://gitlab.com/mosaik/mosaik-csv.git
@@ -96,14 +95,18 @@
     $ pip install -e .
     $ pytest tests
 
 
 Changelog
 =========
 
+2.0.1 - 2024-05-17
+------------------
+ - [BUGFIX] Convert numpy data types to python scalars.
+
 2.0.0 - 2023-11-21
 ------------------
 
 - [CHANGE] Use pandas for CSV reader.
 - [NEW] Add CSV writer.
```

### Comparing `mosaik-csv-2.0.0/README.rst` & `mosaik-csv-2.0.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -51,17 +51,16 @@
         'CSV_writer': {
             'python': 'mosaik_csv_writer:CSVWriter',
         }
     }
     world = mosaik.World(sim_config)
     csv_sim_writer = world.start('CSV_writer', start_date = '01.01.2016 00:00',
                                                date_format='%Y-%m-%d %H:%M:%S', 
-                                               output_file='results.csv',
-                                               print_results=False)
-    csv_writer = csv_sim_writer.Monitor(buff_size = 30 * 60)  # write data after every 30 mins
+                                               output_file='results.csv')
+    csv_writer = csv_sim_writer.CSVWriter(buff_size = 30 * 60)  # write data after every 30 mins
 
 Tests
 =====
 
 You can run the tests with::
 
     $ git clone https://gitlab.com/mosaik/mosaik-csv.git
```

### Comparing `mosaik-csv-2.0.0/mosaik_csv.egg-info/PKG-INFO` & `mosaik-csv-2.0.1/mosaik_csv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaik-csv
-Version: 2.0.0
+Version: 2.0.1
 Summary: Presents CSV datasets to mosaik as models.
 Home-page: https://gitlab.com/mosaik/components/data/mosaik-csv
 Author: mosaik development team
 Author-email: mosaik@offis.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -77,17 +77,16 @@
         'CSV_writer': {
             'python': 'mosaik_csv_writer:CSVWriter',
         }
     }
     world = mosaik.World(sim_config)
     csv_sim_writer = world.start('CSV_writer', start_date = '01.01.2016 00:00',
                                                date_format='%Y-%m-%d %H:%M:%S', 
-                                               output_file='results.csv',
-                                               print_results=False)
-    csv_writer = csv_sim_writer.Monitor(buff_size = 30 * 60)  # write data after every 30 mins
+                                               output_file='results.csv')
+    csv_writer = csv_sim_writer.CSVWriter(buff_size = 30 * 60)  # write data after every 30 mins
 
 Tests
 =====
 
 You can run the tests with::
 
     $ git clone https://gitlab.com/mosaik/mosaik-csv.git
@@ -96,14 +95,18 @@
     $ pip install -e .
     $ pytest tests
 
 
 Changelog
 =========
 
+2.0.1 - 2024-05-17
+------------------
+ - [BUGFIX] Convert numpy data types to python scalars.
+
 2.0.0 - 2023-11-21
 ------------------
 
 - [CHANGE] Use pandas for CSV reader.
 - [NEW] Add CSV writer.
```

### Comparing `mosaik-csv-2.0.0/mosaik_csv.py` & `mosaik-csv-2.0.1/mosaik_csv.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+import numpy as np
 
 import mosaik_api_v3 as mosaik_api
 
 DATE_FORMAT = 'YYYY-MM-DD HH:mm:ss'
 
 SENTINEL = object()
 
@@ -121,15 +122,18 @@
     def get_data(self, outputs):
         data = {}
         for eid, attrs in outputs.items():
             if eid not in self.eids:
                 raise ValueError('Unknown entity ID "%s"' % eid)
             data[eid] = {}
             for attr in attrs:
-                data[eid][attr] = self.cache[attr]
+                if isinstance(self.cache[attr], np.floating) or isinstance(self.cache[attr], np.integer):
+                    data[eid][attr] = self.cache[attr].tolist()
+                else:
+                    data[eid][attr] = str(self.cache[attr])  
 
         return data
 
 
 def main():
     return mosaik_api.start_simulation(CSV(), 'mosaik-csv simulator')
```

### Comparing `mosaik-csv-2.0.0/mosaik_csv_writer.py` & `mosaik-csv-2.0.1/mosaik_csv_writer.py`

 * *Files identical despite different names*

### Comparing `mosaik-csv-2.0.0/requirements.txt` & `mosaik-csv-2.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `mosaik-csv-2.0.0/setup.py` & `mosaik-csv-2.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='mosaik-csv',
-    version='2.0.0',
+    version='2.0.1',
     author='mosaik development team',
     author_email='mosaik@offis.de',
     description=('Presents CSV datasets to mosaik as models.'),
     long_description=(open('README.rst').read() + '\n\n' +
                       open('CHANGES.txt').read() + '\n\n' +
                       open('AUTHORS.txt').read()),
     url='https://gitlab.com/mosaik/components/data/mosaik-csv',
```

