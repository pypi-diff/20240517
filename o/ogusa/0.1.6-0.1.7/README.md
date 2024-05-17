# Comparing `tmp/ogusa-0.1.6.tar.gz` & `tmp/ogusa-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogusa-0.1.6.tar", last modified: Thu May  9 00:20:24 2024, max compression
+gzip compressed data, was "ogusa-0.1.7.tar", last modified: Fri May 17 14:30:42 2024, max compression
```

## Comparing `ogusa-0.1.6.tar` & `ogusa-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:20:24.110449 ogusa-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-09 00:20:19.000000 ogusa-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-05-09 00:20:24.110449 ogusa-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-09 00:20:19.000000 ogusa-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:20:24.110449 ogusa-0.1.6/ogusa/
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/bequest_transmission.py
--rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/calibrate_chi_n.py
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/deterministic_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/estimate_beta_j.py
--rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/get_micro_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/income.py
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/labor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/macro_params.py
--rw-r--r--   0 runner    (1001) docker     (127)  2040787 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/ogusa_default_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/psid_data_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/psid_summ_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/transfer_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/wealth.py
--rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-05-09 00:20:20.000000 ogusa-0.1.6/ogusa/wealthinit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:20:24.110449 ogusa-0.1.6/ogusa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-05-09 00:20:24.000000 ogusa-0.1.6/ogusa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-09 00:20:24.000000 ogusa-0.1.6/ogusa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 00:20:24.000000 ogusa-0.1.6/ogusa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-09 00:20:24.000000 ogusa-0.1.6/ogusa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 00:20:24.000000 ogusa-0.1.6/ogusa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 00:20:20.000000 ogusa-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 00:20:24.110449 ogusa-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-09 00:20:20.000000 ogusa-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:30:42.150529 ogusa-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-17 14:30:38.000000 ogusa-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-05-17 14:30:42.150529 ogusa-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-17 14:30:38.000000 ogusa-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:30:42.146529 ogusa-0.1.7/ogusa/
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/bequest_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13985 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/calibrate_chi_n.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/deterministic_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/estimate_beta_j.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/get_micro_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/income.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/labor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/macro_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2040787 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/ogusa_default_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18074 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/psid_data_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/psid_summ_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/transfer_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/wealth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-05-17 14:30:38.000000 ogusa-0.1.7/ogusa/wealthinit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:30:42.150529 ogusa-0.1.7/ogusa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-05-17 14:30:42.000000 ogusa-0.1.7/ogusa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-17 14:30:42.000000 ogusa-0.1.7/ogusa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:30:42.000000 ogusa-0.1.7/ogusa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 14:30:42.000000 ogusa-0.1.7/ogusa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 14:30:42.000000 ogusa-0.1.7/ogusa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-17 14:30:38.000000 ogusa-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:30:42.150529 ogusa-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-17 14:30:38.000000 ogusa-0.1.7/setup.py
```

### Comparing `ogusa-0.1.6/LICENSE` & `ogusa-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/PKG-INFO` & `ogusa-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogusa
-Version: 0.1.6
+Version: 0.1.7
 Summary: USA calibration for OG-Core
 Home-page: https://github.com/PSLmodels/OG-USA/
 Download-URL: https://github.com/PSLmodels/OG-USA/
 Author: Jason DeBacker and Richard W. Evans
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Issue Tracker, https://github.com/PSLmodels/OG-USA/issues
 Keywords: USA calibration of large scale overlapping generations model of fiscal policy
```

### Comparing `ogusa-0.1.6/README.md` & `ogusa-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa/bequest_transmission.py` & `ogusa-0.1.7/ogusa/bequest_transmission.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa/calibrate.py` & `ogusa-0.1.7/ogusa/calibrate.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa/calibrate_chi_n.py` & `ogusa-0.1.7/ogusa/calibrate_chi_n.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa/constants.py` & `ogusa-0.1.7/ogusa/constants.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa/deterministic_profiles.py` & `ogusa-0.1.7/ogusa/deterministic_profiles.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa/estimate_beta_j.py` & `ogusa-0.1.7/ogusa/estimate_beta_j.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa/get_micro_data.py` & `ogusa-0.1.7/ogusa/get_micro_data.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa/income.py` & `ogusa-0.1.7/ogusa/income.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa/labor.py` & `ogusa-0.1.7/ogusa/labor.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa/macro_params.py` & `ogusa-0.1.7/ogusa/macro_params.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa/ogusa_default_parameters.json` & `ogusa-0.1.7/ogusa/ogusa_default_parameters.json`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa/psid_data_setup.py` & `ogusa-0.1.7/ogusa/psid_data_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 import pandas as pd
 import os
 import pickle
 from pandas_datareader import data as web
 import datetime
 from linearmodels import PanelOLS
 from rpy2.robjects import r
+from rpy2.robjects import conversion
+from rpy2.robjects import default_converter
 from rpy2.robjects import pandas2ri
+from rpy2.robjects.packages import importr
 from ogusa.constants import PSID_NOMINAL_VARS, PSID_CONSTANT_VARS
 
+
 pandas2ri.activate()
 pd.options.mode.chained_assignment = "raise"
 
 CURDIR = os.path.split(os.path.abspath(__file__))[0]
 
 
 def prep_data(data="psid1968to2015.RData"):
@@ -30,15 +34,17 @@
 
     Returns:
         panel_li (Pandas DataFrame): household level data with lifetime
             income groups defined
     """
     # Read data from R into pandas dataframe
     r["load"](os.path.join(CURDIR, "..", "data", "PSID", data))
-    raw_df = r("psid_df")
+    raw_r_df = r("psid_df")
+    with (default_converter + pandas2ri.converter).context():
+        raw_df = conversion.get_conversion().rpy2py(raw_r_df)
 
     # Create unique identifier for each household
     # note that will define a new household if head or spouse changes
     # keep only current heads
     # before 1983, head is relation.head == 1, 1983+ head is given by
     # relation.head == 10
```

### Comparing `ogusa-0.1.6/ogusa/psid_summ_stats.py` & `ogusa-0.1.7/ogusa/psid_summ_stats.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa/transfer_distribution.py` & `ogusa-0.1.7/ogusa/transfer_distribution.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa/utils.py` & `ogusa-0.1.7/ogusa/utils.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa/wealth.py` & `ogusa-0.1.7/ogusa/wealth.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa/wealthinit.py` & `ogusa-0.1.7/ogusa/wealthinit.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/ogusa.egg-info/PKG-INFO` & `ogusa-0.1.7/ogusa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogusa
-Version: 0.1.6
+Version: 0.1.7
 Summary: USA calibration for OG-Core
 Home-page: https://github.com/PSLmodels/OG-USA/
 Download-URL: https://github.com/PSLmodels/OG-USA/
 Author: Jason DeBacker and Richard W. Evans
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Issue Tracker, https://github.com/PSLmodels/OG-USA/issues
 Keywords: USA calibration of large scale overlapping generations model of fiscal policy
```

### Comparing `ogusa-0.1.6/ogusa.egg-info/SOURCES.txt` & `ogusa-0.1.7/ogusa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.6/setup.py` & `ogusa-0.1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as readme_file:
     longdesc = readme_file.read()
 
 setuptools.setup(
     name="ogusa",
-    version="0.1.6",
+    version="0.1.7",
     author="Jason DeBacker and Richard W. Evans",
     license="CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
     description="USA calibration for OG-Core",
     long_description_content_type="text/markdown",
     long_description=longdesc,
     keywords="USA calibration of large scale overlapping generations model of fiscal policy",
     url="https://github.com/PSLmodels/OG-USA/",
@@ -28,15 +28,15 @@
         "pandas>=1.2.5",
         "matplotlib",
         "dask>=2.30.0",
         "distributed>=2.30.1",
         "paramtools>=0.15.0",
         "taxcalc>=3.0.0",
         "requests",
-        "rpy2<=3.5.11",
+        "rpy2>=3.5.12",
         "pandas-datareader",
         "xlwt",
         "openpyxl>=3.1.2",
         "statsmodels",
         "linearmodels",
         "wheel",
         "ogcore",
```

