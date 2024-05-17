# Comparing `tmp/abses-0.6.4.tar.gz` & `tmp/abses-0.6.4.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abses-0.6.4.tar", max compression
+gzip compressed data, was "abses-0.6.4.post0.tar", max compression
```

## Comparing `abses-0.6.4.tar` & `abses-0.6.4.post0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.6.4/LICENSE
-drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.6.4/LICENSES/
--rw-r--r--   0        0        0     6273 2024-04-10 23:24:41.142521 abses-0.6.4/README.md
--rw-r--r--   0        0        0     1125 2024-05-16 13:00:46.169463 abses-0.6.4/abses/__init__.py
--rw-r--r--   0        0        0     2598 2024-05-16 08:41:24.081841 abses-0.6.4/abses/_bases/bases.py
--rw-r--r--   0        0        0     3124 2024-05-16 03:43:18.344259 abses-0.6.4/abses/_bases/components.py
--rw-r--r--   0        0        0     3128 2024-05-11 09:28:11.068727 abses-0.6.4/abses/_bases/dynamic.py
--rw-r--r--   0        0        0      298 2024-05-11 09:28:11.068876 abses-0.6.4/abses/_bases/errors.py
--rw-r--r--   0        0        0     1564 2024-05-16 11:19:52.124908 abses-0.6.4/abses/_bases/logging.py
--rw-r--r--   0        0        0     6575 2024-05-16 09:25:00.885690 abses-0.6.4/abses/_bases/modules.py
--rw-r--r--   0        0        0     3157 2024-05-16 09:29:06.415637 abses-0.6.4/abses/_bases/objects.py
--rw-r--r--   0        0        0     1098 2024-05-11 09:28:11.069942 abses-0.6.4/abses/_bases/states.py
--rw-r--r--   0        0        0     9755 2024-05-16 07:58:52.452219 abses-0.6.4/abses/actor.py
--rw-r--r--   0        0        0     4979 2024-05-11 09:28:11.070565 abses-0.6.4/abses/cells.py
--rw-r--r--   0        0        0        0 2024-05-11 14:48:58.011285 abses-0.6.4/abses/conf/__init__.py
--rw-r--r--   0        0        0      311 2024-05-16 10:46:33.609412 abses-0.6.4/abses/conf/default.yaml
--rw-r--r--   0        0        0    17578 2024-05-16 08:31:28.732690 abses-0.6.4/abses/container.py
--rw-r--r--   0        0        0      969 2024-05-11 09:28:11.071255 abses-0.6.4/abses/data.py
--rw-r--r--   0        0        0     8957 2024-05-10 03:24:33.872539 abses-0.6.4/abses/decision.py
--rw-r--r--   0        0        0    16424 2024-05-16 12:59:51.694497 abses-0.6.4/abses/experiment.py
--rw-r--r--   0        0        0     3872 2024-05-16 06:59:47.771801 abses-0.6.4/abses/human.py
--rw-r--r--   0        0        0    19386 2024-05-15 07:23:23.061845 abses-0.6.4/abses/links.py
--rw-r--r--   0        0        0    15588 2024-05-16 11:13:35.757091 abses-0.6.4/abses/main.py
--rw-r--r--   0        0        0     8375 2024-05-11 09:28:11.072683 abses-0.6.4/abses/move.py
--rw-r--r--   0        0        0    12661 2024-05-16 09:25:11.727552 abses-0.6.4/abses/nature.py
--rw-r--r--   0        0        0    28765 2024-05-16 09:25:22.458944 abses-0.6.4/abses/patch.py
--rw-r--r--   0        0        0     6802 2024-05-11 09:28:11.073646 abses-0.6.4/abses/random.py
--rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.6.4/abses/selection.py
--rw-r--r--   0        0        0    11767 2024-05-16 08:30:03.748125 abses-0.6.4/abses/sequences.py
--rw-r--r--   0        0        0    15523 2024-05-16 08:29:09.798671 abses-0.6.4/abses/time.py
--rw-r--r--   0        0        0     5391 2024-05-12 02:43:42.296709 abses-0.6.4/abses/tools/func.py
--rw-r--r--   0        0        0      723 2024-04-17 19:21:17.693370 abses-0.6.4/abses/tools/regex.py
--rw-r--r--   0        0        0     1134 2024-05-12 12:57:47.944073 abses-0.6.4/abses/viz/viz_actors.py
--rw-r--r--   0        0        0     1149 2024-05-11 09:28:11.074327 abses-0.6.4/abses/viz/viz_model.py
--rw-r--r--   0        0        0     4620 2024-05-11 09:28:11.074600 abses-0.6.4/abses/viz/viz_nature.py
--rw-r--r--   0        0        0     6148 2024-04-14 20:25:37.202150 abses-0.6.4/data/.DS_Store
--rw-r--r--   0        0        0  1653872 2023-09-03 00:55:23.536915 abses-0.6.4/data/YR_cities.zip
--rw-r--r--   0        0        0   395561 2023-11-13 06:23:20.897117 abses-0.6.4/data/farmland.tif
--rw-r--r--   0        0        0    84033 2023-09-02 23:31:24.485471 abses-0.6.4/data/irr_lands.csv
--rw-r--r--   0        0        0  6726328 2023-03-03 00:57:27.899017 abses-0.6.4/data/precipitation.nc
--rw-r--r--   0        0        0   189444 2024-05-11 09:28:11.085808 abses-0.6.4/icons/fa-regular-400.otf
--rw-r--r--   0        0        0     2760 2024-05-16 13:00:46.169371 abses-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     7290 1970-01-01 00:00:00.000000 abses-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.6.4.post0/LICENSE
+drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.6.4.post0/LICENSES/
+-rw-r--r--   0        0        0     6273 2024-04-10 23:24:41.142521 abses-0.6.4.post0/README.md
+-rw-r--r--   0        0        0     1130 2024-05-16 13:29:48.950759 abses-0.6.4.post0/abses/__init__.py
+-rw-r--r--   0        0        0     2598 2024-05-16 08:41:24.081841 abses-0.6.4.post0/abses/_bases/bases.py
+-rw-r--r--   0        0        0     3124 2024-05-16 03:43:18.344259 abses-0.6.4.post0/abses/_bases/components.py
+-rw-r--r--   0        0        0     3128 2024-05-11 09:28:11.068727 abses-0.6.4.post0/abses/_bases/dynamic.py
+-rw-r--r--   0        0        0      298 2024-05-11 09:28:11.068876 abses-0.6.4.post0/abses/_bases/errors.py
+-rw-r--r--   0        0        0     1564 2024-05-16 11:19:52.124908 abses-0.6.4.post0/abses/_bases/logging.py
+-rw-r--r--   0        0        0     6575 2024-05-16 09:25:00.885690 abses-0.6.4.post0/abses/_bases/modules.py
+-rw-r--r--   0        0        0     3157 2024-05-16 09:29:06.415637 abses-0.6.4.post0/abses/_bases/objects.py
+-rw-r--r--   0        0        0     1098 2024-05-11 09:28:11.069942 abses-0.6.4.post0/abses/_bases/states.py
+-rw-r--r--   0        0        0     9755 2024-05-16 07:58:52.452219 abses-0.6.4.post0/abses/actor.py
+-rw-r--r--   0        0        0     4979 2024-05-11 09:28:11.070565 abses-0.6.4.post0/abses/cells.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:48:58.011285 abses-0.6.4.post0/abses/conf/__init__.py
+-rw-r--r--   0        0        0      311 2024-05-16 10:46:33.609412 abses-0.6.4.post0/abses/conf/default.yaml
+-rw-r--r--   0        0        0    17578 2024-05-16 08:31:28.732690 abses-0.6.4.post0/abses/container.py
+-rw-r--r--   0        0        0      969 2024-05-11 09:28:11.071255 abses-0.6.4.post0/abses/data.py
+-rw-r--r--   0        0        0     8957 2024-05-10 03:24:33.872539 abses-0.6.4.post0/abses/decision.py
+-rw-r--r--   0        0        0    16424 2024-05-16 12:59:51.694497 abses-0.6.4.post0/abses/experiment.py
+-rw-r--r--   0        0        0     3872 2024-05-16 06:59:47.771801 abses-0.6.4.post0/abses/human.py
+-rw-r--r--   0        0        0    19386 2024-05-15 07:23:23.061845 abses-0.6.4.post0/abses/links.py
+-rw-r--r--   0        0        0    15588 2024-05-16 11:13:35.757091 abses-0.6.4.post0/abses/main.py
+-rw-r--r--   0        0        0     8375 2024-05-11 09:28:11.072683 abses-0.6.4.post0/abses/move.py
+-rw-r--r--   0        0        0    12661 2024-05-16 09:25:11.727552 abses-0.6.4.post0/abses/nature.py
+-rw-r--r--   0        0        0    28765 2024-05-16 09:25:22.458944 abses-0.6.4.post0/abses/patch.py
+-rw-r--r--   0        0        0     6802 2024-05-11 09:28:11.073646 abses-0.6.4.post0/abses/random.py
+-rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.6.4.post0/abses/selection.py
+-rw-r--r--   0        0        0    11767 2024-05-16 08:30:03.748125 abses-0.6.4.post0/abses/sequences.py
+-rw-r--r--   0        0        0    15523 2024-05-16 08:29:09.798671 abses-0.6.4.post0/abses/time.py
+-rw-r--r--   0        0        0     5391 2024-05-12 02:43:42.296709 abses-0.6.4.post0/abses/tools/func.py
+-rw-r--r--   0        0        0      723 2024-04-17 19:21:17.693370 abses-0.6.4.post0/abses/tools/regex.py
+-rw-r--r--   0        0        0     1134 2024-05-12 12:57:47.944073 abses-0.6.4.post0/abses/viz/viz_actors.py
+-rw-r--r--   0        0        0     1149 2024-05-11 09:28:11.074327 abses-0.6.4.post0/abses/viz/viz_model.py
+-rw-r--r--   0        0        0     4620 2024-05-11 09:28:11.074600 abses-0.6.4.post0/abses/viz/viz_nature.py
+-rw-r--r--   0        0        0     6148 2024-04-14 20:25:37.202150 abses-0.6.4.post0/data/.DS_Store
+-rw-r--r--   0        0        0  1653872 2023-09-03 00:55:23.536915 abses-0.6.4.post0/data/YR_cities.zip
+-rw-r--r--   0        0        0   395561 2023-11-13 06:23:20.897117 abses-0.6.4.post0/data/farmland.tif
+-rw-r--r--   0        0        0    84033 2023-09-02 23:31:24.485471 abses-0.6.4.post0/data/irr_lands.csv
+-rw-r--r--   0        0        0  6726328 2023-03-03 00:57:27.899017 abses-0.6.4.post0/data/precipitation.nc
+-rw-r--r--   0        0        0   189444 2024-05-11 09:28:11.085808 abses-0.6.4.post0/icons/fa-regular-400.otf
+-rw-r--r--   0        0        0     2769 2024-05-16 13:29:48.949672 abses-0.6.4.post0/pyproject.toml
+-rw-r--r--   0        0        0     7277 1970-01-01 00:00:00.000000 abses-0.6.4.post0/PKG-INFO
```

### Comparing `abses-0.6.4/LICENSE` & `abses-0.6.4.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/README.md` & `abses-0.6.4.post0/README.md`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/__init__.py` & `abses-0.6.4.post0/abses/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "perception",
     "alive_required",
     "time_condition",
     "Experiment",
     "load_data",
     "logger",
 ]
-__version__ = "v0.6.4"
+__version__ = "v0.6.4.post"
 
 from ._bases.logging import logger
 from .actor import Actor, alive_required, perception
 from .container import ActorsList
 from .data import load_data
 from .decision import Decision
 from .experiment import Experiment
```

### Comparing `abses-0.6.4/abses/_bases/bases.py` & `abses-0.6.4.post0/abses/_bases/bases.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/_bases/components.py` & `abses-0.6.4.post0/abses/_bases/components.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/_bases/dynamic.py` & `abses-0.6.4.post0/abses/_bases/dynamic.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/_bases/logging.py` & `abses-0.6.4.post0/abses/_bases/logging.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/_bases/modules.py` & `abses-0.6.4.post0/abses/_bases/modules.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/_bases/objects.py` & `abses-0.6.4.post0/abses/_bases/objects.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/_bases/states.py` & `abses-0.6.4.post0/abses/_bases/states.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/actor.py` & `abses-0.6.4.post0/abses/actor.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/cells.py` & `abses-0.6.4.post0/abses/cells.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/container.py` & `abses-0.6.4.post0/abses/container.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/data.py` & `abses-0.6.4.post0/abses/data.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/decision.py` & `abses-0.6.4.post0/abses/decision.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/experiment.py` & `abses-0.6.4.post0/abses/experiment.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/human.py` & `abses-0.6.4.post0/abses/human.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/links.py` & `abses-0.6.4.post0/abses/links.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/main.py` & `abses-0.6.4.post0/abses/main.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/move.py` & `abses-0.6.4.post0/abses/move.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/nature.py` & `abses-0.6.4.post0/abses/nature.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/patch.py` & `abses-0.6.4.post0/abses/patch.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/random.py` & `abses-0.6.4.post0/abses/random.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/selection.py` & `abses-0.6.4.post0/abses/selection.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/sequences.py` & `abses-0.6.4.post0/abses/sequences.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/time.py` & `abses-0.6.4.post0/abses/time.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/tools/func.py` & `abses-0.6.4.post0/abses/tools/func.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/tools/regex.py` & `abses-0.6.4.post0/abses/tools/regex.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/viz/viz_actors.py` & `abses-0.6.4.post0/abses/viz/viz_actors.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/viz/viz_model.py` & `abses-0.6.4.post0/abses/viz/viz_model.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/abses/viz/viz_nature.py` & `abses-0.6.4.post0/abses/viz/viz_nature.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/data/.DS_Store` & `abses-0.6.4.post0/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/data/YR_cities.zip` & `abses-0.6.4.post0/data/YR_cities.zip`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/data/farmland.tif` & `abses-0.6.4.post0/data/farmland.tif`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/data/irr_lands.csv` & `abses-0.6.4.post0/data/irr_lands.csv`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/data/precipitation.nc` & `abses-0.6.4.post0/data/precipitation.nc`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/icons/fa-regular-400.otf` & `abses-0.6.4.post0/icons/fa-regular-400.otf`

 * *Files identical despite different names*

### Comparing `abses-0.6.4/pyproject.toml` & `abses-0.6.4.post0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.poetry]
 name = "abses"
-version = "0.6.4"
+version = "0.6.4.post"
 description = "ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour."
 authors = ["Shuang Song <songshgeo@gmail.com>"]
 license = "Apache 2.0 License"
 readme = "README.md"
 include = [
   "icons/fa-regular-400.otf",
   "abses/conf/**/*.yaml",
@@ -47,23 +47,23 @@
 [tool.poetry.plugins."hydra.searchpath"]
 abses = "hydra_plugins.abses_searchpath_plugin:ABSESpySearchPathPlugin"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 netcdf4 = ">=1.6"
 hydra-core = "~1.3"
-mesa-geo = "~0.7"
-xarray = "~2024"
+mesa-geo = ">=0.6"
+xarray = ">=2023"
 fiona = ">1.8"
-loguru = "~0.7"
+loguru = ">=0.7"
 rioxarray = ">=0.13"
 pendulum = "~2"
 geopandas = "~0"
 typing-extensions = "~4"
-fontawesome = "~5"
+fontawesome = ">=5"
 seaborn = ">=0.13"
 
 [tool.poetry.group.dev.dependencies]
 pytest-clarity = "^1.0.1"
 pre-commit = "^3.0.1"
 scriv = "^1.2.0"
 pytest = "^7.2.1"
```

### Comparing `abses-0.6.4/PKG-INFO` & `abses-0.6.4.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: abses
-Version: 0.6.4
+Version: 0.6.4.post0
 Summary: ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour.
 License: Apache 2.0 License
 Author: Shuang Song
 Author-email: songshgeo@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fiona (>1.8)
-Requires-Dist: fontawesome (>=5,<6)
+Requires-Dist: fontawesome (>=5)
 Requires-Dist: geopandas (>=0,<1)
 Requires-Dist: hydra-core (>=1.3,<1.4)
-Requires-Dist: loguru (>=0.7,<0.8)
-Requires-Dist: mesa-geo (>=0.7,<0.8)
+Requires-Dist: loguru (>=0.7)
+Requires-Dist: mesa-geo (>=0.6)
 Requires-Dist: netcdf4 (>=1.6)
 Requires-Dist: pendulum (>=2,<3)
 Requires-Dist: rioxarray (>=0.13)
 Requires-Dist: seaborn (>=0.13)
 Requires-Dist: typing-extensions (>=4,<5)
-Requires-Dist: xarray (>=2024,<2025)
+Requires-Dist: xarray (>=2023)
 Description-Content-Type: text/markdown
 
 # ABSESpy: Agent-Based Modeling Framework for Social-Ecological Systems
 
 ![ABSES_banner](https://songshgeo-picgo-1302043007.cos.ap-beijing.myqcloud.com/uPic/CleanShot%202023-10-19%20at%2019.08.12@2x.png)
 
 <div align="center"><p>
```

#### html2text {}

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1 Name: abses Version: 0.6.4 Summary: ABSESpy makes it
-easier to build artificial Social-ecological systems with real GeoSpatial
+Metadata-Version: 2.1 Name: abses Version: 0.6.4.post0 Summary: ABSESpy makes
+it easier to build artificial Social-ecological systems with real GeoSpatial
 datasets and fully incorporate human behaviour. License: Apache 2.0 License
 Author: Shuang Song Author-email: songshgeo@gmail.com Requires-Python:
 >=3.9,<3.12 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: fiona (>1.8) Requires-
-Dist: fontawesome (>=5,<6) Requires-Dist: geopandas (>=0,<1) Requires-Dist:
-hydra-core (>=1.3,<1.4) Requires-Dist: loguru (>=0.7,<0.8) Requires-Dist: mesa-
-geo (>=0.7,<0.8) Requires-Dist: netcdf4 (>=1.6) Requires-Dist: pendulum
-(>=2,<3) Requires-Dist: rioxarray (>=0.13) Requires-Dist: seaborn (>=0.13)
-Requires-Dist: typing-extensions (>=4,<5) Requires-Dist: xarray (>=2024,<2025)
-Description-Content-Type: text/markdown # ABSESpy: Agent-Based Modeling
-Framework for Social-Ecological Systems ![ABSES_banner](https://songshgeo-
-picgo-1302043007.cos.ap-beijing.myqcloud.com/uPic/CleanShot%202023-10-
-19%20at%2019.08.12@2x.png)
+Dist: fontawesome (>=5) Requires-Dist: geopandas (>=0,<1) Requires-Dist: hydra-
+core (>=1.3,<1.4) Requires-Dist: loguru (>=0.7) Requires-Dist: mesa-geo (>=0.6)
+Requires-Dist: netcdf4 (>=1.6) Requires-Dist: pendulum (>=2,<3) Requires-Dist:
+rioxarray (>=0.13) Requires-Dist: seaborn (>=0.13) Requires-Dist: typing-
+extensions (>=4,<5) Requires-Dist: xarray (>=2023) Description-Content-Type:
+text/markdown # ABSESpy: Agent-Based Modeling Framework for Social-Ecological
+Systems ![ABSES_banner](https://songshgeo-picgo-1302043007.cos.ap-
+beijing.myqcloud.com/uPic/CleanShot%202023-10-19%20at%2019.08.12@2x.png)
   _[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]_[_S_t_a_r_s_]_[_I_s_s_u_e_s_]_[_R_e_p_o
 _S_i_z_e_]_[_f_o_l_l_o_w_ _o_n_ _T_w_i_t_t_e_r_]_[_g_i_t_h_u_b_]--- Language: [English Readme] | [ç®ä½ä¸­æ]
                                     **[â
                                  âInstallâ
                             â][Install]** **[â
                              âGetting startedâ
                         â][Getting Started]** **[â
```

