# Comparing `tmp/tkmatrix-0.9.2.tar.gz` & `tmp/tkmatrix-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkmatrix-0.9.2.tar", last modified: Tue May 14 19:52:44 2024, max compression
+gzip compressed data, was "tkmatrix-0.9.3.tar", last modified: Fri May 17 15:58:12 2024, max compression
```

## Comparing `tkmatrix-0.9.2.tar` & `tkmatrix-0.9.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:52:44.713580 tkmatrix-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-14 19:52:44.713580 tkmatrix-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:52:44.713580 tkmatrix-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:52:44.713580 tkmatrix-0.9.2/tkmatrix/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/tkmatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10197 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/tkmatrix/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:52:44.713580 tkmatrix-0.9.2/tkmatrix/custom_algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/tkmatrix/custom_algorithms/BlsCustomSearchAlgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/tkmatrix/custom_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/tkmatrix/custom_algorithms/custom_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/tkmatrix/inject_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/tkmatrix/inject_rv_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/tkmatrix/programmatic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/tkmatrix/properties.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/tkmatrix/rv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:52:44.713580 tkmatrix-0.9.2/tkmatrix/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/tkmatrix/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/tkmatrix/tests/test_tkmatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    44005 2024-05-14 19:52:36.000000 tkmatrix-0.9.2/tkmatrix/tkmatrix_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:52:44.713580 tkmatrix-0.9.2/tkmatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-14 19:52:44.000000 tkmatrix-0.9.2/tkmatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-14 19:52:44.000000 tkmatrix-0.9.2/tkmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:52:44.000000 tkmatrix-0.9.2/tkmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-14 19:52:44.000000 tkmatrix-0.9.2/tkmatrix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 19:52:44.000000 tkmatrix-0.9.2/tkmatrix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:58:12.828687 tkmatrix-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-17 15:58:12.828687 tkmatrix-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 15:58:12.828687 tkmatrix-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:58:12.828687 tkmatrix-0.9.3/tkmatrix/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/tkmatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10197 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/tkmatrix/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:58:12.828687 tkmatrix-0.9.3/tkmatrix/custom_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/tkmatrix/custom_algorithms/BlsCustomSearchAlgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/tkmatrix/custom_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/tkmatrix/custom_algorithms/custom_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/tkmatrix/inject_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/tkmatrix/inject_rv_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/tkmatrix/programmatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/tkmatrix/properties.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/tkmatrix/rv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:58:12.828687 tkmatrix-0.9.3/tkmatrix/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/tkmatrix/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/tkmatrix/tests/test_tkmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44005 2024-05-17 15:58:03.000000 tkmatrix-0.9.3/tkmatrix/tkmatrix_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:58:12.828687 tkmatrix-0.9.3/tkmatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-17 15:58:12.000000 tkmatrix-0.9.3/tkmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-17 15:58:12.000000 tkmatrix-0.9.3/tkmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:58:12.000000 tkmatrix-0.9.3/tkmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-17 15:58:12.000000 tkmatrix-0.9.3/tkmatrix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 15:58:12.000000 tkmatrix-0.9.3/tkmatrix.egg-info/top_level.txt
```

### Comparing `tkmatrix-0.9.2/LICENSE` & `tkmatrix-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.2/PKG-INFO` & `tkmatrix-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkmatrix
-Version: 0.9.2
+Version: 0.9.3
 Summary: ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
 Home-page: https://github.com/PlanetHunters/tkmatrix
 Author: M. Dévora-Pajares & F.J. Pozuelos
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="400px" src="https://github.com/martindevora/tkmatrix/blob/master/images/matrix.jpg?raw=true">
```

### Comparing `tkmatrix-0.9.2/README.md` & `tkmatrix-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.2/setup.py` & `tkmatrix-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = "0.9.2"
+version = "0.9.3"
 setuptools.setup(
     name="tkmatrix",
     version=version,
     author="M. Dévora-Pajares & F.J. Pozuelos",
     author_email="mdevorapajares@protonmail.com",
     description="ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets",
     long_description=long_description,
@@ -21,15 +21,15 @@
     ],
     python_requires='>=3.10',
     install_requires=['argparse==1.4.0',
                         'beautifulsoup4==4.9.3',
                         'configparser==5.0.1',
                         "corner==2.1.0",
                         "ellc==1.8.5",
-                        "lcbuilder==0.18.2",
+                        "lcbuilder==0.18.3",
                         "mock==4.0.3",
                         'pyparsing==2.4.7', # Matplotlib dependency
                         "seaborn==0.11.1",
                         'setuptools>=41.0.0',
                         "sklearn==0.0"
     ]
 )
```

### Comparing `tkmatrix-0.9.2/tkmatrix/__main__.py` & `tkmatrix-0.9.3/tkmatrix/__main__.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.2/tkmatrix/custom_algorithms/BlsCustomSearchAlgorithm.py` & `tkmatrix-0.9.3/tkmatrix/custom_algorithms/BlsCustomSearchAlgorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
             sde = results.power[max_power_index].value / np.nanmedian(results.power).value
             t0 = results.transit_time_at_max_power.value
             duration = results.duration_at_max_power.value
             found_period = results.period_at_max_power.value
             intransit_result = transit_mask(time, found_period, 2 * duration, t0)
             real_intransit_result = transit_mask(time, found_period, duration, t0)
             oot_flux = flux[~real_intransit_result]
-            snr = np.abs(np.nanmean(1 - real_intransit_result)) / np.nanstd(oot_flux) * (len(real_intransit_result) ** 0.5)
+            it_flux = flux[real_intransit_result]
+            snr = np.abs(np.nanmean(1 - it_flux)) / np.nanstd(oot_flux) * (len(it_flux) ** 0.5)
             if snr >= min_snr:
                 time = time[~intransit_result]
                 flux = flux[~intransit_result]
                 time, flux = cleaned_array(time, flux)
                 if results.transit_time is not None and len(results.transit_time) > 0:
                     print(f"Selecting signal with mode {signal_selection_mode}")
                     if signal_selection_mode == 'period-epoch':
```

### Comparing `tkmatrix-0.9.2/tkmatrix/custom_algorithms/custom_search.py` & `tkmatrix-0.9.3/tkmatrix/custom_algorithms/custom_search.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.2/tkmatrix/inject_model.py` & `tkmatrix-0.9.3/tkmatrix/inject_model.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.2/tkmatrix/inject_rv_model.py` & `tkmatrix-0.9.3/tkmatrix/inject_rv_model.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.2/tkmatrix/programmatic.py` & `tkmatrix-0.9.3/tkmatrix/programmatic.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.2/tkmatrix/properties.yaml` & `tkmatrix-0.9.3/tkmatrix/properties.yaml`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.2/tkmatrix/rv.py` & `tkmatrix-0.9.3/tkmatrix/rv.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.2/tkmatrix/tests/test_tkmatrix.py` & `tkmatrix-0.9.3/tkmatrix/tests/test_tkmatrix.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.2/tkmatrix/tkmatrix_class.py` & `tkmatrix-0.9.3/tkmatrix/tkmatrix_class.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.9.2/tkmatrix.egg-info/PKG-INFO` & `tkmatrix-0.9.3/tkmatrix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkmatrix
-Version: 0.9.2
+Version: 0.9.3
 Summary: ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
 Home-page: https://github.com/PlanetHunters/tkmatrix
 Author: M. Dévora-Pajares & F.J. Pozuelos
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="400px" src="https://github.com/martindevora/tkmatrix/blob/master/images/matrix.jpg?raw=true">
```

### Comparing `tkmatrix-0.9.2/tkmatrix.egg-info/SOURCES.txt` & `tkmatrix-0.9.3/tkmatrix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

