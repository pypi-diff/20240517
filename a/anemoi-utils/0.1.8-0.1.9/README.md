# Comparing `tmp/anemoi_utils-0.1.8.tar.gz` & `tmp/anemoi_utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemoi_utils-0.1.8.tar", last modified: Tue May  7 09:05:12 2024, max compression
+gzip compressed data, was "anemoi_utils-0.1.9.tar", last modified: Fri May 17 13:44:30 2024, max compression
```

## Comparing `anemoi_utils-0.1.8.tar` & `anemoi_utils-0.1.9.tar`

### file list

```diff
@@ -1,53 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.993716 anemoi_utils-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.985716 anemoi_utils-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.985716 anemoi_utils-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-05-07 09:05:12.993716 anemoi_utils-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.989716 anemoi_utils-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.989716 anemoi_utils-0.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.989716 anemoi_utils-0.1.8/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/installing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.989716 anemoi_utils-0.1.8/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/modules/checkpoints.rst
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/modules/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/modules/dates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/modules/grib.rst
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/modules/humanize.rst
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/modules/provenance.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/modules/text.rst
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:05:12.993716 anemoi_utils-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.985716 anemoi_utils-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.985716 anemoi_utils-0.1.8/src/anemoi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.989716 anemoi_utils-0.1.8/src/anemoi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 09:05:12.000000 anemoi_utils-0.1.8/src/anemoi/utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/grib.py
--rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/provenance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/src/anemoi/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.993716 anemoi_utils-0.1.8/src/anemoi_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-05-07 09:05:12.000000 anemoi_utils-0.1.8/src/anemoi_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-07 09:05:12.000000 anemoi_utils-0.1.8/src/anemoi_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:05:12.000000 anemoi_utils-0.1.8/src/anemoi_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-07 09:05:12.000000 anemoi_utils-0.1.8/src/anemoi_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 09:05:12.000000 anemoi_utils-0.1.8/src/anemoi_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:05:12.993716 anemoi_utils-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-07 09:05:02.000000 anemoi_utils-0.1.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.853158 anemoi_utils-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.841158 anemoi_utils-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.845158 anemoi_utils-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-05-17 13:44:30.853158 anemoi_utils-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.845158 anemoi_utils-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.845158 anemoi_utils-0.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.845158 anemoi_utils-0.1.9/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/installing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.845158 anemoi_utils-0.1.9/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/modules/checkpoints.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/modules/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/modules/dates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/modules/grib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/modules/humanize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/modules/provenance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/modules/text.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 13:44:30.853158 anemoi_utils-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.845158 anemoi_utils-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.841158 anemoi_utils-0.1.9/src/anemoi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.849158 anemoi_utils-0.1.9/src/anemoi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 13:44:30.000000 anemoi_utils-0.1.9/src/anemoi/utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/grib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/humanize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.849158 anemoi_utils-0.1.9/src/anemoi/utils/mars/
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/mars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/mars/mars.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.849158 anemoi_utils-0.1.9/src/anemoi_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-05-17 13:44:30.000000 anemoi_utils-0.1.9/src/anemoi_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-17 13:44:30.000000 anemoi_utils-0.1.9/src/anemoi_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:44:30.000000 anemoi_utils-0.1.9/src/anemoi_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-17 13:44:30.000000 anemoi_utils-0.1.9/src/anemoi_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 13:44:30.000000 anemoi_utils-0.1.9/src/anemoi_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.849158 anemoi_utils-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/tests/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/tests/test_utils.py
```

### Comparing `anemoi_utils-0.1.8/.github/workflows/python-publish.yml` & `anemoi_utils-0.1.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/.gitignore` & `anemoi_utils-0.1.9/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -181,7 +181,8 @@
 
 _build/
 ?
 ?.*
 ~*
 *.sync
 _version.py
+*.code-workspace
```

### Comparing `anemoi_utils-0.1.8/.pre-commit-config.yaml` & `anemoi_utils-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/LICENSE` & `anemoi_utils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/PKG-INFO` & `anemoi_utils-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,14 +219,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: tomli
+Requires-Dist: pyyaml
 Provides-Extra: provenance
 Requires-Dist: GitPython; extra == "provenance"
 Requires-Dist: nvsmi; extra == "provenance"
 Provides-Extra: text
 Requires-Dist: termcolor; extra == "text"
 Provides-Extra: grib
 Requires-Dist: requests; extra == "grib"
```

### Comparing `anemoi_utils-0.1.8/README.md` & `anemoi_utils-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/docs/Makefile` & `anemoi_utils-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/docs/_static/logo.png` & `anemoi_utils-0.1.9/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/docs/_static/style.css` & `anemoi_utils-0.1.9/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/docs/conf.py` & `anemoi_utils-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/docs/index.rst` & `anemoi_utils-0.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/docs/installing.rst` & `anemoi_utils-0.1.9/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/pyproject.toml` & `anemoi_utils-0.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "tomli", # Only needed before 3.11
+    "pyyaml",
 ]
 
 [project.optional-dependencies]
 provenance = ["GitPython", "nvsmi"]
 
 text = ["termcolor"]
 
@@ -84,7 +85,10 @@
 Repository = "https://github.com/ecmwf/anemoi-utils/"
 Issues = "https://github.com/ecmwf/anemoi-utils/issues"
 # Changelog = "https://github.com/ecmwf/anemoi-utils/CHANGELOG.md"
 
 
 [tool.setuptools_scm]
 version_file = "src/anemoi/utils/_version.py"
+
+[tool.setuptools.package-data]
+"anemoi.utils.mars" = ["*.yaml"]
```

### Comparing `anemoi_utils-0.1.8/src/anemoi/utils/caching.py` & `anemoi_utils-0.1.9/src/anemoi/utils/caching.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/src/anemoi/utils/checkpoints.py` & `anemoi_utils-0.1.9/src/anemoi/utils/checkpoints.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/src/anemoi/utils/config.py` & `anemoi_utils-0.1.9/src/anemoi/utils/config.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/src/anemoi/utils/dates.py` & `anemoi_utils-0.1.9/src/anemoi/utils/dates.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,14 +6,24 @@
 # nor does it submit to any jurisdiction.
 
 
 import calendar
 import datetime
 
 
+def normalise_frequency(frequency):
+    if isinstance(frequency, int):
+        return frequency
+    assert isinstance(frequency, str), (type(frequency), frequency)
+
+    unit = frequency[-1].lower()
+    v = int(frequency[:-1])
+    return {"h": v, "d": v * 24}[unit]
+
+
 def no_time_zone(date):
     """Remove time zone information from a date.
 
     Parameters
     ----------
     date : datetime.datetime
         A datetime object.
@@ -23,14 +33,15 @@
     datetime.datetime
         The datetime object without time zone information.
     """
 
     return date.replace(tzinfo=None)
 
 
+# this function is use in anemoi-datasets
 def as_datetime(date):
     """Convert a date to a datetime object, removing any time zone information.
 
     Parameters
     ----------
     date : datetime.date or datetime.datetime or str
         The date to convert.
@@ -158,19 +169,23 @@
         reference_dates : _type_
             _description_
         years : int, optional
             _description_, by default 20
         """
 
         self.reference_dates = reference_dates
-        self.years = (1, years + 1)
+
+        if isinstance(years, list):
+            self.years = years
+        else:
+            self.years = range(1, years + 1)
 
     def __iter__(self):
         for reference_date in self.reference_dates:
-            for year in range(*self.years):
+            for year in self.years:
                 if reference_date.month == 2 and reference_date.day == 29:
                     date = datetime.datetime(reference_date.year - year, 2, 28)
                 else:
                     date = datetime.datetime(reference_date.year - year, reference_date.month, reference_date.day)
                 yield (date, reference_date)
 
 
@@ -242,7 +257,65 @@
 
         Parameters
         ----------
         year : int
             _description_
         """
         super().__init__(datetime.datetime(year, 9, 1), datetime.datetime(year, 11, 30), **kwargs)
+
+
+class ConcatDateTimes:
+    def __init__(self, *dates):
+        if len(dates) == 1 and isinstance(dates[0], list):
+            dates = dates[0]
+
+        self.dates = dates
+
+    def __iter__(self):
+        for date in self.dates:
+            yield from date
+
+
+class EnumDateTimes:
+    def __init__(self, dates):
+        self.dates = dates
+
+    def __iter__(self):
+        for date in self.dates:
+            yield as_datetime(date)
+
+
+def datetimes_factory(*args, **kwargs):
+    if args and kwargs:
+        raise ValueError("Cannot provide both args and kwargs for a list of dates")
+
+    if not args and not kwargs:
+        raise ValueError("No dates provided")
+
+    if kwargs:
+        name = kwargs.get("name")
+
+        if name == "hindcast":
+            reference_dates = kwargs["reference_dates"]
+            reference_dates = datetimes_factory(reference_dates)
+            years = kwargs["years"]
+            return HindcastDatesTimes(reference_dates=reference_dates, years=years)
+
+        kwargs = kwargs.copy()
+        if "frequency" in kwargs:
+            freq = kwargs.pop("frequency")
+            kwargs["increment"] = normalise_frequency(freq)
+        return DateTimes(**kwargs)
+
+    if not any((isinstance(x, dict) or isinstance(x, list)) for x in args):
+        return EnumDateTimes(args)
+
+    if len(args) == 1:
+        a = args[0]
+
+        if isinstance(a, dict):
+            return datetimes_factory(**a)
+
+        if isinstance(a, list):
+            return datetimes_factory(*a)
+
+    return ConcatDateTimes(*[datetimes_factory(a) for a in args])
```

### Comparing `anemoi_utils-0.1.8/src/anemoi/utils/grib.py` & `anemoi_utils-0.1.9/src/anemoi/utils/grib.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/src/anemoi/utils/humanize.py` & `anemoi_utils-0.1.9/src/anemoi/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/src/anemoi/utils/provenance.py` & `anemoi_utils-0.1.9/src/anemoi/utils/provenance.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/src/anemoi/utils/text.py` & `anemoi_utils-0.1.9/src/anemoi/utils/text.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.8/src/anemoi_utils.egg-info/PKG-INFO` & `anemoi_utils-0.1.9/src/anemoi_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,14 +219,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: tomli
+Requires-Dist: pyyaml
 Provides-Extra: provenance
 Requires-Dist: GitPython; extra == "provenance"
 Requires-Dist: nvsmi; extra == "provenance"
 Provides-Extra: text
 Requires-Dist: termcolor; extra == "text"
 Provides-Extra: grib
 Requires-Dist: requests; extra == "grib"
```

### Comparing `anemoi_utils-0.1.8/src/anemoi_utils.egg-info/SOURCES.txt` & `anemoi_utils-0.1.9/src/anemoi_utils.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 src/anemoi/utils/checkpoints.py
 src/anemoi/utils/config.py
 src/anemoi/utils/dates.py
 src/anemoi/utils/grib.py
 src/anemoi/utils/humanize.py
 src/anemoi/utils/provenance.py
 src/anemoi/utils/text.py
+src/anemoi/utils/mars/__init__.py
+src/anemoi/utils/mars/mars.yaml
 src/anemoi_utils.egg-info/PKG-INFO
 src/anemoi_utils.egg-info/SOURCES.txt
 src/anemoi_utils.egg-info/dependency_links.txt
 src/anemoi_utils.egg-info/requires.txt
 src/anemoi_utils.egg-info/top_level.txt
 tests/requirements.txt
+tests/test_dates.py
 tests/test_utils.py
```

### Comparing `anemoi_utils-0.1.8/tests/test_utils.py` & `anemoi_utils-0.1.9/tests/test_utils.py`

 * *Files identical despite different names*

