# Comparing `tmp/pystac_client-0.7.7.tar.gz` & `tmp/pystac_client-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystac_client-0.7.7.tar", last modified: Fri Apr 19 13:07:43 2024, max compression
+gzip compressed data, was "pystac_client-0.8.0.tar", last modified: Fri May 17 14:16:36 2024, max compression
```

## Comparing `pystac_client-0.7.7.tar` & `pystac_client-0.8.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:07:43.132527 pystac_client-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-19 13:07:19.000000 pystac_client-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 13:07:19.000000 pystac_client-0.7.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-19 13:07:43.132527 pystac_client-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-19 13:07:19.000000 pystac_client-0.7.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:07:43.128527 pystac_client-0.7.7/pystac_client/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    26442 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/collection_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/conformance.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    32798 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/item_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/stac_api_io.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:07:43.128527 pystac_client-0.7.7/pystac_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-19 13:07:43.000000 pystac_client-0.7.7/pystac_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-19 13:07:43.000000 pystac_client-0.7.7/pystac_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:07:43.000000 pystac_client-0.7.7/pystac_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 13:07:43.000000 pystac_client-0.7.7/pystac_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-19 13:07:43.000000 pystac_client-0.7.7/pystac_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 13:07:43.000000 pystac_client-0.7.7/pystac_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:07:43.132527 pystac_client-0.7.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:07:43.128527 pystac_client-0.7.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-19 13:07:19.000000 pystac_client-0.7.7/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    27234 2024-04-19 13:07:19.000000 pystac_client-0.7.7/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-19 13:07:19.000000 pystac_client-0.7.7/tests/test_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    29723 2024-04-19 13:07:19.000000 pystac_client-0.7.7/tests/test_item_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-19 13:07:19.000000 pystac_client-0.7.7/tests/test_stac_api_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:16:36.781440 pystac_client-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-17 14:16:27.000000 pystac_client-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 14:16:27.000000 pystac_client-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-17 14:16:36.781440 pystac_client-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-17 14:16:27.000000 pystac_client-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:16:36.777439 pystac_client-0.8.0/pystac_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26442 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32836 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/item_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/stac_api_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:16:36.777439 pystac_client-0.8.0/pystac_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-17 14:16:36.000000 pystac_client-0.8.0/pystac_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-17 14:16:36.000000 pystac_client-0.8.0/pystac_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:16:36.000000 pystac_client-0.8.0/pystac_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-17 14:16:36.000000 pystac_client-0.8.0/pystac_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-17 14:16:36.000000 pystac_client-0.8.0/pystac_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 14:16:36.000000 pystac_client-0.8.0/pystac_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:16:36.781440 pystac_client-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:16:36.777439 pystac_client-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-05-17 14:16:27.000000 pystac_client-0.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27234 2024-05-17 14:16:27.000000 pystac_client-0.8.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-17 14:16:27.000000 pystac_client-0.8.0/tests/test_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30015 2024-05-17 14:16:27.000000 pystac_client-0.8.0/tests/test_item_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-05-17 14:16:27.000000 pystac_client-0.8.0/tests/test_stac_api_io.py
```

### Comparing `pystac_client-0.7.7/LICENSE` & `pystac_client-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pystac_client-0.7.7/PKG-INFO` & `pystac_client-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystac-client
-Version: 0.7.7
+Version: 0.8.0
 Summary: Python library for working with SpatioTemporal Asset Catalog (STAC) APIs.
 Author-email: Jon Duckworth <duckontheweb@gmail.com>, Matthew Hanson <matt.a.hanson@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/stac-utils/pystac-client
 Project-URL: documentation, https://pystac-client.readthedocs.io
 Project-URL: repository, https://github.com/stac-utils/pystac-client.git
@@ -21,15 +21,15 @@
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.28.2
 Requires-Dist: pystac[validation]>=1.10.0
 Requires-Dist: python-dateutil>=2.8.2
 Provides-Extra: dev
 Requires-Dist: black~=24.0; extra == "dev"
@@ -43,32 +43,32 @@
 Requires-Dist: pytest-benchmark~=4.0.0; extra == "dev"
 Requires-Dist: pytest-console-scripts~=1.4.0; extra == "dev"
 Requires-Dist: pytest-cov~=5.0; extra == "dev"
 Requires-Dist: pytest-recording~=0.13; extra == "dev"
 Requires-Dist: pytest~=8.0; extra == "dev"
 Requires-Dist: recommonmark~=0.7.1; extra == "dev"
 Requires-Dist: requests-mock~=1.12; extra == "dev"
-Requires-Dist: ruff==0.4.0; extra == "dev"
+Requires-Dist: ruff==0.4.4; extra == "dev"
 Requires-Dist: tomli~=2.0; python_version < "3.11" and extra == "dev"
 Requires-Dist: types-python-dateutil<2.10.0,>=2.8.19; extra == "dev"
 Requires-Dist: types-requests~=2.31.0; extra == "dev"
 Requires-Dist: urllib3<2; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: Sphinx~=6.2; extra == "docs"
+Requires-Dist: Sphinx~=7.3; extra == "docs"
 Requires-Dist: boto3~=1.26; extra == "docs"
 Requires-Dist: cartopy~=0.21; extra == "docs"
 Requires-Dist: geojson~=3.1.0; extra == "docs"
 Requires-Dist: geopandas~=0.14.0; extra == "docs"
 Requires-Dist: geoviews~=1.9; extra == "docs"
-Requires-Dist: hvplot~=0.9.0; extra == "docs"
+Requires-Dist: hvplot~=0.10.0; extra == "docs"
 Requires-Dist: ipykernel~=6.22; extra == "docs"
 Requires-Dist: ipython~=8.12; extra == "docs"
 Requires-Dist: jinja2<4.0; extra == "docs"
 Requires-Dist: matplotlib~=3.8; extra == "docs"
-Requires-Dist: myst-parser~=2.0; extra == "docs"
+Requires-Dist: myst-parser~=3.0; extra == "docs"
 Requires-Dist: nbsphinx~=0.9; extra == "docs"
 Requires-Dist: pydata-sphinx-theme~=0.13; extra == "docs"
 Requires-Dist: pygeoif~=1.0; extra == "docs"
 Requires-Dist: scipy~=1.10; extra == "docs"
 Requires-Dist: sphinxcontrib-fulltoc~=1.2; extra == "docs"
 
 # STAC Client <!-- omit in toc -->
@@ -86,15 +86,15 @@
 - [Table of Contents](#table-of-contents)
 - [Installation](#installation)
 - [Documentation](#documentation)
 - [Development](#development)
 
 ## Installation
 
-Install from PyPi. Other than [PySTAC](https://pystac.readthedocs.io) itself, the only dependencies for pystac-client is the Python [requests](https://docs.python-requests.org) and [dateutil](https://dateutil.readthedocs.io) libraries.
+Install from PyPi. Other than [PySTAC](https://pystac.readthedocs.io) itself, the only dependencies for pystac-client are the Python [requests](https://docs.python-requests.org) and [dateutil](https://dateutil.readthedocs.io) libraries.
 
 ```shell
 pip install pystac-client
 ```
 
 ## Documentation
```

### Comparing `pystac_client-0.7.7/README.md` & `pystac_client-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 - [Table of Contents](#table-of-contents)
 - [Installation](#installation)
 - [Documentation](#documentation)
 - [Development](#development)
 
 ## Installation
 
-Install from PyPi. Other than [PySTAC](https://pystac.readthedocs.io) itself, the only dependencies for pystac-client is the Python [requests](https://docs.python-requests.org) and [dateutil](https://dateutil.readthedocs.io) libraries.
+Install from PyPi. Other than [PySTAC](https://pystac.readthedocs.io) itself, the only dependencies for pystac-client are the Python [requests](https://docs.python-requests.org) and [dateutil](https://dateutil.readthedocs.io) libraries.
 
 ```shell
 pip install pystac-client
 ```
 
 ## Documentation
```

### Comparing `pystac_client-0.7.7/pyproject.toml` & `pystac_client-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Scientific/Engineering :: GIS",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dependencies = [
     "requests>=2.28.2",
     "pystac[validation]>=1.10.0",
     "python-dateutil>=2.8.2",
 ]
 dynamic = ["version"]
 
@@ -49,34 +49,34 @@
     "pytest-benchmark~=4.0.0",
     "pytest-console-scripts~=1.4.0",
     "pytest-cov~=5.0",
     "pytest-recording~=0.13",
     "pytest~=8.0",
     "recommonmark~=0.7.1",
     "requests-mock~=1.12",
-    "ruff==0.4.0",
+    "ruff==0.4.4",
     "tomli~=2.0; python_version<'3.11'",
     "types-python-dateutil>=2.8.19,<2.10.0",
     "types-requests~=2.31.0",
     # temporary pin https://github.com/stac-utils/pystac-client/issues/509
     "urllib3<2",
 ]
 docs = [
-    "Sphinx~=6.2",
+    "Sphinx~=7.3",
     "boto3~=1.26",
     "cartopy~=0.21",
     "geojson~=3.1.0",
     "geopandas~=0.14.0",
     "geoviews~=1.9",
-    "hvplot~=0.9.0",
+    "hvplot~=0.10.0",
     "ipykernel~=6.22",
     "ipython~=8.12",
     "jinja2<4.0",
     "matplotlib~=3.8",
-    "myst-parser~=2.0",
+    "myst-parser~=3.0",
     "nbsphinx~=0.9",
     "pydata-sphinx-theme~=0.13",
     "pygeoif~=1.0",
     "scipy~=1.10",
     "sphinxcontrib-fulltoc~=1.2",
 ]
```

### Comparing `pystac_client-0.7.7/pystac_client/_utils.py` & `pystac_client-0.8.0/pystac_client/_utils.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.7.7/pystac_client/cli.py` & `pystac_client-0.8.0/pystac_client/cli.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.7.7/pystac_client/client.py` & `pystac_client-0.8.0/pystac_client/client.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.7.7/pystac_client/collection_client.py` & `pystac_client-0.8.0/pystac_client/collection_client.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.7.7/pystac_client/conformance.py` & `pystac_client-0.8.0/pystac_client/conformance.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.7.7/pystac_client/item_search.py` & `pystac_client-0.8.0/pystac_client/item_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,16 @@
         else:
             bbox = tuple(map(float, value))
 
         return bbox
 
     @staticmethod
     def _to_utc_isoformat(dt: datetime_) -> str:
-        dt = dt.astimezone(timezone.utc)
+        if dt.tzinfo is not None:
+            dt = dt.astimezone(timezone.utc)
         dt = dt.replace(tzinfo=None)
         return f'{dt.isoformat("T")}Z'
 
     def _to_isoformat_range(
         self,
         component: DatetimeOrTimestamp,
     ) -> Tuple[str, Optional[str]]:
```

### Comparing `pystac_client-0.7.7/pystac_client/mixins.py` & `pystac_client-0.8.0/pystac_client/mixins.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.7.7/pystac_client/stac_api_io.py` & `pystac_client-0.8.0/pystac_client/stac_api_io.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.7.7/pystac_client/warnings.py` & `pystac_client-0.8.0/pystac_client/warnings.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.7.7/pystac_client.egg-info/PKG-INFO` & `pystac_client-0.8.0/pystac_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystac-client
-Version: 0.7.7
+Version: 0.8.0
 Summary: Python library for working with SpatioTemporal Asset Catalog (STAC) APIs.
 Author-email: Jon Duckworth <duckontheweb@gmail.com>, Matthew Hanson <matt.a.hanson@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/stac-utils/pystac-client
 Project-URL: documentation, https://pystac-client.readthedocs.io
 Project-URL: repository, https://github.com/stac-utils/pystac-client.git
@@ -21,15 +21,15 @@
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.28.2
 Requires-Dist: pystac[validation]>=1.10.0
 Requires-Dist: python-dateutil>=2.8.2
 Provides-Extra: dev
 Requires-Dist: black~=24.0; extra == "dev"
@@ -43,32 +43,32 @@
 Requires-Dist: pytest-benchmark~=4.0.0; extra == "dev"
 Requires-Dist: pytest-console-scripts~=1.4.0; extra == "dev"
 Requires-Dist: pytest-cov~=5.0; extra == "dev"
 Requires-Dist: pytest-recording~=0.13; extra == "dev"
 Requires-Dist: pytest~=8.0; extra == "dev"
 Requires-Dist: recommonmark~=0.7.1; extra == "dev"
 Requires-Dist: requests-mock~=1.12; extra == "dev"
-Requires-Dist: ruff==0.4.0; extra == "dev"
+Requires-Dist: ruff==0.4.4; extra == "dev"
 Requires-Dist: tomli~=2.0; python_version < "3.11" and extra == "dev"
 Requires-Dist: types-python-dateutil<2.10.0,>=2.8.19; extra == "dev"
 Requires-Dist: types-requests~=2.31.0; extra == "dev"
 Requires-Dist: urllib3<2; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: Sphinx~=6.2; extra == "docs"
+Requires-Dist: Sphinx~=7.3; extra == "docs"
 Requires-Dist: boto3~=1.26; extra == "docs"
 Requires-Dist: cartopy~=0.21; extra == "docs"
 Requires-Dist: geojson~=3.1.0; extra == "docs"
 Requires-Dist: geopandas~=0.14.0; extra == "docs"
 Requires-Dist: geoviews~=1.9; extra == "docs"
-Requires-Dist: hvplot~=0.9.0; extra == "docs"
+Requires-Dist: hvplot~=0.10.0; extra == "docs"
 Requires-Dist: ipykernel~=6.22; extra == "docs"
 Requires-Dist: ipython~=8.12; extra == "docs"
 Requires-Dist: jinja2<4.0; extra == "docs"
 Requires-Dist: matplotlib~=3.8; extra == "docs"
-Requires-Dist: myst-parser~=2.0; extra == "docs"
+Requires-Dist: myst-parser~=3.0; extra == "docs"
 Requires-Dist: nbsphinx~=0.9; extra == "docs"
 Requires-Dist: pydata-sphinx-theme~=0.13; extra == "docs"
 Requires-Dist: pygeoif~=1.0; extra == "docs"
 Requires-Dist: scipy~=1.10; extra == "docs"
 Requires-Dist: sphinxcontrib-fulltoc~=1.2; extra == "docs"
 
 # STAC Client <!-- omit in toc -->
@@ -86,15 +86,15 @@
 - [Table of Contents](#table-of-contents)
 - [Installation](#installation)
 - [Documentation](#documentation)
 - [Development](#development)
 
 ## Installation
 
-Install from PyPi. Other than [PySTAC](https://pystac.readthedocs.io) itself, the only dependencies for pystac-client is the Python [requests](https://docs.python-requests.org) and [dateutil](https://dateutil.readthedocs.io) libraries.
+Install from PyPi. Other than [PySTAC](https://pystac.readthedocs.io) itself, the only dependencies for pystac-client are the Python [requests](https://docs.python-requests.org) and [dateutil](https://dateutil.readthedocs.io) libraries.
 
 ```shell
 pip install pystac-client
 ```
 
 ## Documentation
```

### Comparing `pystac_client-0.7.7/pystac_client.egg-info/SOURCES.txt` & `pystac_client-0.8.0/pystac_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystac_client-0.7.7/pystac_client.egg-info/requires.txt` & `pystac_client-0.8.0/pystac_client.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -14,33 +14,33 @@
 pytest-benchmark~=4.0.0
 pytest-console-scripts~=1.4.0
 pytest-cov~=5.0
 pytest-recording~=0.13
 pytest~=8.0
 recommonmark~=0.7.1
 requests-mock~=1.12
-ruff==0.4.0
+ruff==0.4.4
 types-python-dateutil<2.10.0,>=2.8.19
 types-requests~=2.31.0
 urllib3<2
 
 [dev:python_version < "3.11"]
 tomli~=2.0
 
 [docs]
-Sphinx~=6.2
+Sphinx~=7.3
 boto3~=1.26
 cartopy~=0.21
 geojson~=3.1.0
 geopandas~=0.14.0
 geoviews~=1.9
-hvplot~=0.9.0
+hvplot~=0.10.0
 ipykernel~=6.22
 ipython~=8.12
 jinja2<4.0
 matplotlib~=3.8
-myst-parser~=2.0
+myst-parser~=3.0
 nbsphinx~=0.9
 pydata-sphinx-theme~=0.13
 pygeoif~=1.0
 scipy~=1.10
 sphinxcontrib-fulltoc~=1.2
```

### Comparing `pystac_client-0.7.7/tests/test_cli.py` & `pystac_client-0.8.0/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,9 +279,9 @@
         result = script_runner.run(args, print_result=False)
         assert result.success
 
         with open(path) as f:
             output = json.loads(f.read())
 
         assert isinstance(output, list)
-        assert len(output) == 8, "earth-search does not have 8 collections"
+        assert len(output) == 9, "earth-search does not have 9 collections"
         assert all(c["type"] == "Collection" for c in output)
```

### Comparing `pystac_client-0.7.7/tests/test_client.py` & `pystac_client-0.8.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.7.7/tests/test_collection_client.py` & `pystac_client-0.8.0/tests/test_collection_client.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.7.7/tests/test_item_search.py` & `pystac_client-0.8.0/tests/test_item_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -822,7 +822,16 @@
         url="https://earth-search.aws.element84.com/v1/search",
         collections=["sentinel-2-l2a", "landsat-c2-l2"],
         intersects={"type": "Point", "coordinates": [-105.1019, 40.1672]},
         datetime="2023-10-08",
     )
     collections = set(item.collection_id for item in search.items())
     assert collections == {"sentinel-2-l2a", "landsat-c2-l2"}
+
+
+def test_naive_datetime() -> None:
+    search = ItemSearch(
+        url="https://earth-search.aws.element84.com/v1/search",
+        datetime=datetime(2024, 5, 14, 4, 25, 42, tzinfo=None),
+        method="POST",
+    )
+    assert search.get_parameters()["datetime"] == "2024-05-14T04:25:42Z"
```

### Comparing `pystac_client-0.7.7/tests/test_stac_api_io.py` & `pystac_client-0.8.0/tests/test_stac_api_io.py`

 * *Files identical despite different names*

