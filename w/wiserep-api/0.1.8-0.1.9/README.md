# Comparing `tmp/wiserep_api-0.1.8.tar.gz` & `tmp/wiserep_api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiserep_api-0.1.8.tar", last modified: Fri Mar 22 12:23:13 2024, max compression
+gzip compressed data, was "wiserep_api-0.1.9.tar", last modified: Fri May 17 09:42:17 2024, max compression
```

## Comparing `wiserep_api-0.1.8.tar` & `wiserep_api-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-03-22 12:23:13.169285 wiserep_api-0.1.8/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1080 2023-05-02 06:17:37.000000 wiserep_api-0.1.8/LICENSE
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       51 2023-05-04 05:31:12.000000 wiserep_api-0.1.8/MANIFEST.in
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5319 2024-03-22 12:23:13.169285 wiserep_api-0.1.8/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4722 2023-08-02 10:35:44.000000 wiserep_api-0.1.8/README.md
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       35 2024-03-22 10:14:38.000000 wiserep_api-0.1.8/requirements.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2024-03-22 12:23:13.169285 wiserep_api-0.1.8/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1134 2023-05-04 05:33:37.000000 wiserep_api-0.1.8/setup.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-03-22 12:23:13.165285 wiserep_api-0.1.8/tests/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2022-06-28 14:16:32.000000 wiserep_api-0.1.8/tests/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2395 2024-03-22 12:20:41.000000 wiserep_api-0.1.8/tests/test_download_spectra.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1268 2023-07-25 08:20:56.000000 wiserep_api-0.1.8/tests/test_properties.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      475 2023-05-04 07:25:36.000000 wiserep_api-0.1.8/tests/test_search.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-03-22 12:23:13.169285 wiserep_api-0.1.8/wiserep_api/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      305 2023-07-07 11:18:07.000000 wiserep_api-0.1.8/wiserep_api/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2024-03-22 12:21:34.000000 wiserep_api-0.1.8/wiserep_api/_version.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3688 2023-07-07 11:22:26.000000 wiserep_api-0.1.8/wiserep_api/api.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4006 2023-11-20 15:03:35.000000 wiserep_api-0.1.8/wiserep_api/properties.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3433 2023-05-04 03:46:52.000000 wiserep_api-0.1.8/wiserep_api/search.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3427 2023-05-04 08:34:32.000000 wiserep_api-0.1.8/wiserep_api/snid.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6905 2024-03-22 12:18:57.000000 wiserep_api-0.1.8/wiserep_api/spectra.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-03-22 12:23:13.169285 wiserep_api-0.1.8/wiserep_api/static/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      744 2023-05-04 01:46:48.000000 wiserep_api-0.1.8/wiserep_api/static/spectral_types.json
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-03-22 12:23:13.169285 wiserep_api-0.1.8/wiserep_api.egg-info/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5319 2024-03-22 12:23:13.000000 wiserep_api-0.1.8/wiserep_api.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      521 2024-03-22 12:23:13.000000 wiserep_api-0.1.8/wiserep_api.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2024-03-22 12:23:13.000000 wiserep_api-0.1.8/wiserep_api.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       35 2024-03-22 12:23:13.000000 wiserep_api-0.1.8/wiserep_api.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       18 2024-03-22 12:23:13.000000 wiserep_api-0.1.8/wiserep_api.egg-info/top_level.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-17 09:42:17.175399 wiserep_api-0.1.9/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1080 2023-05-02 06:17:37.000000 wiserep_api-0.1.9/LICENSE
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       51 2023-05-04 05:31:12.000000 wiserep_api-0.1.9/MANIFEST.in
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5300 2024-05-17 09:42:17.175399 wiserep_api-0.1.9/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4703 2024-04-22 09:12:45.000000 wiserep_api-0.1.9/README.md
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       35 2024-03-22 10:14:38.000000 wiserep_api-0.1.9/requirements.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2024-05-17 09:42:17.175399 wiserep_api-0.1.9/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1134 2023-05-04 05:33:37.000000 wiserep_api-0.1.9/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-17 09:42:17.175399 wiserep_api-0.1.9/tests/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2022-06-28 14:16:32.000000 wiserep_api-0.1.9/tests/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2395 2024-03-22 12:20:41.000000 wiserep_api-0.1.9/tests/test_download_spectra.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1268 2023-07-25 08:20:56.000000 wiserep_api-0.1.9/tests/test_properties.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      475 2023-05-04 07:25:36.000000 wiserep_api-0.1.9/tests/test_search.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-17 09:42:17.175399 wiserep_api-0.1.9/wiserep_api/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      305 2023-07-07 11:18:07.000000 wiserep_api-0.1.9/wiserep_api/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2024-05-17 09:41:11.000000 wiserep_api-0.1.9/wiserep_api/_version.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3688 2023-07-07 11:22:26.000000 wiserep_api-0.1.9/wiserep_api/api.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4006 2023-11-20 15:03:35.000000 wiserep_api-0.1.9/wiserep_api/properties.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3433 2023-05-04 03:46:52.000000 wiserep_api-0.1.9/wiserep_api/search.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3427 2023-05-04 08:34:32.000000 wiserep_api-0.1.9/wiserep_api/snid.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7275 2024-05-17 09:40:17.000000 wiserep_api-0.1.9/wiserep_api/spectra.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-17 09:42:17.175399 wiserep_api-0.1.9/wiserep_api/static/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      744 2023-05-04 01:46:48.000000 wiserep_api-0.1.9/wiserep_api/static/spectral_types.json
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-17 09:42:17.175399 wiserep_api-0.1.9/wiserep_api.egg-info/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5300 2024-05-17 09:42:17.000000 wiserep_api-0.1.9/wiserep_api.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      521 2024-05-17 09:42:17.000000 wiserep_api-0.1.9/wiserep_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2024-05-17 09:42:17.000000 wiserep_api-0.1.9/wiserep_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       35 2024-05-17 09:42:17.000000 wiserep_api-0.1.9/wiserep_api.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       18 2024-05-17 09:42:17.000000 wiserep_api-0.1.9/wiserep_api.egg-info/top_level.txt
```

### Comparing `wiserep_api-0.1.8/LICENSE` & `wiserep_api-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.8/PKG-INFO` & `wiserep_api-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiserep_api
-Version: 0.1.8
+Version: 0.1.9
 Summary: API to access WiserRep data from command lines
 Home-page: https://github.com/temuller/wiserep_api
 Author: Tomás Enrique Müller-Bravo
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: astropy
 Requires-Dist: requests
 Requires-Dist: lxml
 
 # WiseRep API
-API to access WiserRep data from command lines
+API to access WiserRep data
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fwiserep_api-blue.svg?style=flat)](https://github.com/temuller/wiserep_api)
 [![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/temuller/wiserep_api/blob/master/LICENSE)
 ![Python Version](https://img.shields.io/badge/Python-3.9%2B-blue)
 [![PyPI](https://img.shields.io/pypi/v/wiserep_api?label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/wiserep_api/)
 [![DOI](https://zenodo.org/badge/635179400.svg)](https://zenodo.org/badge/latestdoi/635179400)
```

### Comparing `wiserep_api-0.1.8/README.md` & `wiserep_api-0.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # WiseRep API
-API to access WiserRep data from command lines
+API to access WiserRep data
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fwiserep_api-blue.svg?style=flat)](https://github.com/temuller/wiserep_api)
 [![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/temuller/wiserep_api/blob/master/LICENSE)
 ![Python Version](https://img.shields.io/badge/Python-3.9%2B-blue)
 [![PyPI](https://img.shields.io/pypi/v/wiserep_api?label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/wiserep_api/)
 [![DOI](https://zenodo.org/badge/635179400.svg)](https://zenodo.org/badge/latestdoi/635179400)
```

### Comparing `wiserep_api-0.1.8/setup.py` & `wiserep_api-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.8/tests/test_download_spectra.py` & `wiserep_api-0.1.9/tests/test_download_spectra.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.8/tests/test_properties.py` & `wiserep_api-0.1.9/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.8/wiserep_api/api.py` & `wiserep_api-0.1.9/wiserep_api/api.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.8/wiserep_api/properties.py` & `wiserep_api-0.1.9/wiserep_api/properties.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.8/wiserep_api/search.py` & `wiserep_api-0.1.9/wiserep_api/search.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.8/wiserep_api/snid.py` & `wiserep_api-0.1.9/wiserep_api/snid.py`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.8/wiserep_api/spectra.py` & `wiserep_api-0.1.9/wiserep_api/spectra.py`

 * *Files 17% similar despite different names*

```diff
@@ -102,15 +102,26 @@
     if verbose is True:
         print(f"Found {len(fits_urls)} URLs with spectra (FITS): {fits_urls}")
 
     # retrieve table with spectra information
     spec_table = pd.read_html(StringIO(response.text), match='Spec. ID')[0]
     if isinstance(spec_table['Spec. ID'], pd.core.frame.DataFrame) is True:
         # from multi-index to the usual dataframe
-        spec_table = pd.DataFrame({col[0]:spec_table[col[0]][col[1]].values for col in spec_table.columns})
+        spec_dict = {col[0]:None for col in spec_table.columns}
+
+        for col in spec_dict.keys():
+            series = spec_table[col].copy()
+            for sub_col in spec_table[col].columns:
+                series = series[sub_col]
+            spec_dict[col] = series.values
+
+        spec_table = pd.DataFrame(spec_dict)
+        # remove extra columns
+        columns = [col for col in spec_table.columns if 'Unnamed' not in col]
+        spec_table = spec_table[columns]
     
     # download ASCII spectra
     if file_type == "ascii" or file_type is None:
         ascii_files = []
         for url in txt_urls:
             # skip filesspec_df = spec_df[::2]  # every other row is just crap
```

### Comparing `wiserep_api-0.1.8/wiserep_api/static/spectral_types.json` & `wiserep_api-0.1.9/wiserep_api/static/spectral_types.json`

 * *Files identical despite different names*

### Comparing `wiserep_api-0.1.8/wiserep_api.egg-info/PKG-INFO` & `wiserep_api-0.1.9/wiserep_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiserep_api
-Version: 0.1.8
+Version: 0.1.9
 Summary: API to access WiserRep data from command lines
 Home-page: https://github.com/temuller/wiserep_api
 Author: Tomás Enrique Müller-Bravo
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: astropy
 Requires-Dist: requests
 Requires-Dist: lxml
 
 # WiseRep API
-API to access WiserRep data from command lines
+API to access WiserRep data
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fwiserep_api-blue.svg?style=flat)](https://github.com/temuller/wiserep_api)
 [![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/temuller/wiserep_api/blob/master/LICENSE)
 ![Python Version](https://img.shields.io/badge/Python-3.9%2B-blue)
 [![PyPI](https://img.shields.io/pypi/v/wiserep_api?label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/wiserep_api/)
 [![DOI](https://zenodo.org/badge/635179400.svg)](https://zenodo.org/badge/latestdoi/635179400)
```

### Comparing `wiserep_api-0.1.8/wiserep_api.egg-info/SOURCES.txt` & `wiserep_api-0.1.9/wiserep_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

