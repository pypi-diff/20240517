# Comparing `tmp/silvimetric-1.2.0.tar.gz` & `tmp/silvimetric-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silvimetric-1.2.0.tar", last modified: Tue May 14 16:41:29 2024, max compression
+gzip compressed data, was "silvimetric-1.2.1.tar", last modified: Fri May 17 15:29:30 2024, max compression
```

## Comparing `silvimetric-1.2.0.tar` & `silvimetric-1.2.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:29.466361 silvimetric-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-14 16:41:17.000000 silvimetric-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-14 16:41:29.466361 silvimetric-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-14 16:41:17.000000 silvimetric-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-14 16:41:17.000000 silvimetric-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:41:29.466361 silvimetric-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:29.458361 silvimetric-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:29.458361 silvimetric-1.2.0/src/silvimetric/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:29.462361 silvimetric-1.2.0/src/silvimetric/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/cli/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:29.462361 silvimetric-1.2.0/src/silvimetric/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/commands/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/commands/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/commands/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/commands/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/commands/shatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:29.462361 silvimetric-1.2.0/src/silvimetric/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10157 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/extents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/names.py
--rw-r--r--   0 runner    (1001) docker     (127)    12541 2024-05-14 16:41:17.000000 silvimetric-1.2.0/src/silvimetric/resources/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:29.466361 silvimetric-1.2.0/src/silvimetric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-14 16:41:29.000000 silvimetric-1.2.0/src/silvimetric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-14 16:41:29.000000 silvimetric-1.2.0/src/silvimetric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:41:29.000000 silvimetric-1.2.0/src/silvimetric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 16:41:29.000000 silvimetric-1.2.0/src/silvimetric.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 16:41:29.000000 silvimetric-1.2.0/src/silvimetric.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:41:29.466361 silvimetric-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_extents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_fusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_shatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-14 16:41:17.000000 silvimetric-1.2.0/tests/test_western.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:29:30.791682 silvimetric-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-17 15:29:20.000000 silvimetric-1.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-17 15:29:30.791682 silvimetric-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-17 15:29:20.000000 silvimetric-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-17 15:29:20.000000 silvimetric-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 15:29:30.791682 silvimetric-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:29:30.783682 silvimetric-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:29:30.783682 silvimetric-1.2.1/src/silvimetric/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:29:30.783682 silvimetric-1.2.1/src/silvimetric/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/cli/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:29:30.787682 silvimetric-1.2.1/src/silvimetric/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/commands/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/commands/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/commands/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/commands/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/commands/shatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:29:30.787682 silvimetric-1.2.1/src/silvimetric/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/resources/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/resources/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/resources/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10157 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/resources/extents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/resources/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/resources/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/resources/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-05-17 15:29:20.000000 silvimetric-1.2.1/src/silvimetric/resources/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:29:30.787682 silvimetric-1.2.1/src/silvimetric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-17 15:29:30.000000 silvimetric-1.2.1/src/silvimetric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-17 15:29:30.000000 silvimetric-1.2.1/src/silvimetric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:29:30.000000 silvimetric-1.2.1/src/silvimetric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-17 15:29:30.000000 silvimetric-1.2.1/src/silvimetric.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 15:29:30.000000 silvimetric-1.2.1/src/silvimetric.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:29:30.787682 silvimetric-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-17 15:29:20.000000 silvimetric-1.2.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-17 15:29:20.000000 silvimetric-1.2.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-17 15:29:20.000000 silvimetric-1.2.1/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-17 15:29:20.000000 silvimetric-1.2.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-17 15:29:20.000000 silvimetric-1.2.1/tests/test_extents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-17 15:29:20.000000 silvimetric-1.2.1/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-17 15:29:20.000000 silvimetric-1.2.1/tests/test_fusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-17 15:29:20.000000 silvimetric-1.2.1/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-05-17 15:29:20.000000 silvimetric-1.2.1/tests/test_shatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-17 15:29:20.000000 silvimetric-1.2.1/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-17 15:29:20.000000 silvimetric-1.2.1/tests/test_western.py
```

### Comparing `silvimetric-1.2.0/LICENSE.txt` & `silvimetric-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/PKG-INFO` & `silvimetric-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silvimetric
-Version: 1.2.0
+Version: 1.2.1
 Summary: A forestry LiDAR processing package
 Author-email: Kyle Mann <kyle@hobu.co>, Howard Butler <howard@hobu.co>
 Maintainer-email: Kyle Mann <kyle@hobu.co>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/hobuinc/silvimetric
 Project-URL: repository, https://github.com/hobuinc/silvimetric
 Classifier: Development Status :: 4 - Beta
```

### Comparing `silvimetric-1.2.0/README.md` & `silvimetric-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/pyproject.toml` & `silvimetric-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/src/silvimetric/__init__.py` & `silvimetric-1.2.1/src/silvimetric/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.2.0'
+__version__ = '1.2.1'
 
 from .resources.bounds import Bounds
 from .resources.extents import Extents
 from .resources.storage import Storage
 from .resources.metric import Metric, Metrics
 from .resources.log import Log
 from .resources.data import Data
```

### Comparing `silvimetric-1.2.0/src/silvimetric/cli/cli.py` & `silvimetric-1.2.1/src/silvimetric/cli/cli.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/src/silvimetric/cli/common.py` & `silvimetric-1.2.1/src/silvimetric/cli/common.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/src/silvimetric/commands/extract.py` & `silvimetric-1.2.1/src/silvimetric/commands/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     driver = gdal.GetDriverByName("GTiff")
     gdal_type = np_to_gdal_types[np.dtype(data.dtype).str]
     tif = driver.Create(str(path), int(xsize), int(ysize), 1, gdal_type)
     tif.SetGeoTransform(transform)
     tif.SetProjection(srs.ExportToWkt())
     tif.GetRasterBand(1).WriteArray(data)
-    tif.GetRasterBand(1).SetNoDataValue(-9999)
+    tif.GetRasterBand(1).SetNoDataValue(np.nan)
     tif.FlushCache()
     tif = None
 
 def get_metrics(data_in: pd.DataFrame, storage: Storage):
     """
     Reruns a metric over this cell. Only called if there is overlapping data.
 
@@ -124,15 +124,15 @@
         # data with overlaps
         redo_data = data.loc[redo_indices][att_list].groupby(['X','Y']).agg(lambda x: list(chain(*x)))
         # data that has no overlaps
         clean_data = data.loc[data.index[~data.index.duplicated(False)]]
 
         storage.config.log.warning('Overlapping data detected. Rerunning metrics over these cells...')
         new_metrics = get_metrics(redo_data.reset_index(), storage)
-        return pd.concat([clean_data, new_metrics]).reset_index()
+    return pd.concat([clean_data, new_metrics]).reset_index()
 
 def extract(config: ExtractConfig) -> None:
     """
     Pull data from database for each desired metric and output them to rasters
 
     :param config: ExtractConfig.
     """
```

### Comparing `silvimetric-1.2.0/src/silvimetric/commands/info.py` & `silvimetric-1.2.1/src/silvimetric/commands/info.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/src/silvimetric/commands/manage.py` & `silvimetric-1.2.1/src/silvimetric/commands/manage.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/src/silvimetric/commands/scan.py` & `silvimetric-1.2.1/src/silvimetric/commands/scan.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/src/silvimetric/commands/shatter.py` & `silvimetric-1.2.1/src/silvimetric/commands/shatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,37 @@
+import dask.diagnostics
+import dask.distributed
 import numpy as np
 import signal
 import datetime
 import copy
 from typing import Generator
 import pandas as pd
 
 import dask
 from dask.distributed import as_completed, futures_of, CancelledError
-from dask.diagnostics import ProgressBar
 import dask.array as da
 import dask.bag as db
-from line_profiler import profile
 
 from .. import Extents, Storage, Data, ShatterConfig
 
-@profile
 def get_data(extents: Extents, filename: str, storage: Storage) -> np.ndarray:
     """
     Execute pipeline and retrieve point cloud data for this extent
 
     :param extents: :class:`silvimetric.resources.extents.Extents` being operated on.
     :param filename: Path to either PDAL pipeline or point cloud.
     :param storage: :class:`silvimetric.resources.storage.Storage` database object.
     :return: Point data array from PDAL.
     """
-    #TODO look at making a record array here
     data = Data(filename, storage.config, bounds = extents.bounds)
     p = data.pipeline
     data.execute()
     return p.get_dataframe(0)
 
-@profile
 def arrange(points: pd.DataFrame, leaf, attrs: list[str]):
     """
     Arrange data to fit key-value TileDB input format.
 
     :param data: Tuple of indices and point data array (xis, yis, data).
     :param leaf: :class:`silvimetric.resources.extents.Extent` being operated on.
     :param attrs: List of attribute names.
@@ -54,84 +51,106 @@
     points.loc[:, 'xi'] = da.floor(points.xi)
     # ceil for y because origin is at top left
     points.loc[:, 'yi'] = da.ceil(points.yi)
 
     return points
 
 
-@profile
 def get_metrics(data_in, storage: Storage):
     """
     Run DataFrames through metric processes
     """
-    if data_in is None:
-        return None
-
     # TODO dependencies on other metrics:
     # - Iterate through metrics and figure out which ones are being used as
     #   dependencies
     # - Remove those from the list and run them first
     # - Then pass them to the metrics that require them as we get there?
 
+    if data_in is None:
+        return None
+
     metric_data = dask.persist(*[ m.do(data_in) for m in storage.config.metrics ])
     return metric_data
 
-@profile
 def agg_list(df: pd.DataFrame):
     """
     Make variable-length point data attributes into lists
     """
     if df is None:
         return None
     grouped = df.groupby(['xi','yi'])
     grouped = grouped.agg(list)
     return grouped.assign(count=lambda x: [len(z) for z in grouped.Z])
 
-@profile
 def join(list_data, metric_data):
     """
     Join the list data and metric DataFrames together
     """
     if list_data is None or metric_data is None:
         return None
     return list_data.join([m for m in metric_data])
 
-@profile
-def write(data_in, tdb):
+def write(data_in, storage, timestamp):
     """
     Write cell data to database
 
     :param data_in: Data to be written to database.
     :param tdb: TileDB write stream.
     :return: Number of points written.
     """
-    if data_in is None or data_in.empty:
-        return 0
 
     # TODO get this working at some point. Look at pandas extensions
     # data_in = data_in.rename(columns={'xi':'X','yi':'Y'})
 
     # tiledb.from_pandas(uri='autzen_db', dataframe=data_in, mode='append',
     #         column_types=dict(data_in.dtypes),
     #         varlen_types=[np.dtype('O')])
 
-    idf = data_in.index.to_frame()
+    if data_in is None or data_in.empty:
+        return 0
+
+    with storage.open('w', timestamp=timestamp) as tdb:
+        idf = data_in.index.to_frame()
+
+        dx = idf['xi'].to_list()
+        dy = idf['yi'].to_list()
+        dt = lambda a: tdb.schema.attr(a).dtype
+        dd = { d: np.fromiter([*[np.array(nd, dt(d)) for nd in data_in[d]], None], object)[:-1] for d in data_in }
+
+        tdb[dx,dy] = dd
+        pc = dd['count'].sum().item()
+        p = copy.deepcopy(pc)
 
-    dx = idf['xi'].to_list()
-    dy = idf['yi'].to_list()
-    dt = lambda a: tdb.schema.attr(a).dtype
-    dd = { d: np.fromiter([*[np.array(nd, dt(d)) for nd in data_in[d]], None], object)[:-1] for d in data_in }
-
-    tdb[dx,dy] = dd
-    pc = dd['count'].sum().item()
-    p = copy.deepcopy(pc)
     del pc, data_in
     return p
 
 Leaves = Generator[Extents, None, None]
+def get_processes(leaves: Leaves, config: ShatterConfig, storage: Storage) -> db.Bag:
+    """ Create dask bags and the order of operations.  """
+
+    ## Handle dask bag transitions through work states
+    attrs = [a.name for a in config.attrs]
+    timestamp = (config.time_slot, config.time_slot)
+
+    # remove any extents that have already been donem, only skip if full overlap
+    leaf_bag: db.Bag = db.from_sequence(leaves)
+    if config.mbr:
+        def mbr_filter(one: Extents):
+            return all(one.disjoint_by_mbr(m) for m in config.mbr)
+        leaf_bag = leaf_bag.filter(mbr_filter)
+
+    points: db.Bag = leaf_bag.map(get_data, config.filename, storage)
+    arranged: db.Bag = points.map(arrange, leaf_bag, attrs)
+    metrics: db.Bag = arranged.map(get_metrics, storage)
+    lists: db.Bag = arranged.map(agg_list)
+    joined: db.Bag = lists.map(join, metrics)
+    writes: db.Bag = joined.map(write, storage, timestamp)
+
+    return writes
+
 def run(leaves: Leaves, config: ShatterConfig, storage: Storage) -> int:
     """
     Coordinate running of shatter process and handle any interruptions
 
     :param leaves: Generator of Leaf nodes.
     :param config: :class:`silvimetric.resources.config.ShatterConfig`
     :param storage: :class:`silvimetric.resources.storage.Storage`
@@ -152,63 +171,45 @@
         config.log.info('Saving config before quitting...')
 
         storage.saveMetadata('shatter', str(config), config.time_slot)
         config.log.info('Quitting.')
 
     signal.signal(signal.SIGINT, kill_gracefully)
 
+    processes = get_processes(leaves, config, storage)
 
-    ## Handle dask bag transitions through work states
-    attrs = [a.name for a in config.attrs]
-    timestamp = (config.time_slot, config.time_slot)
+    ## If dask is distributed, use the futures feature
+    dc = dask.config.get('distributed.client')
+    if isinstance(dc, dask.distributed.Client):
+        pc_futures = futures_of(processes.persist())
+        for batch in as_completed(pc_futures, with_results=True).batches():
+            for future, pack in batch:
+                if isinstance(pack, CancelledError):
+                    continue
+                for pc in pack:
+                    config.point_count = config.point_count + pc
+                    del pc
 
-    with storage.open('w', timestamp=timestamp) as tdb:
-        leaf_bag: db.Bag = db.from_sequence(leaves)
-        if config.mbr:
-            def mbr_filter(one: Extents):
-                return all(one.disjoint_by_mbr(m) for m in config.mbr)
-            leaf_bag = leaf_bag.filter(mbr_filter)
-
-        points: db.Bag = leaf_bag.map(get_data, config.filename, storage)
-        arranged: db.Bag = points.map(arrange, leaf_bag, attrs)
-        metrics: db.Bag = arranged.map(get_metrics, storage)
-        lists: db.Bag = arranged.map(agg_list)
-        joined: db.Bag = lists.map(join, metrics)
-        writes: db.Bag = joined.map(write, tdb)
-
-        ## If dask is distributed, use the futures feature
-        dc = dask.config.get('distributed.client')
-        if isinstance(dc, dask.distributed.Client):
-            pc_futures = futures_of(writes.persist())
-            for batch in as_completed(pc_futures, with_results=True).batches():
-                for future, pack in batch:
-                    if isinstance(pack, CancelledError):
-                        continue
-                    for pc in pack:
-                        config.point_count = config.point_count + pc
-                        del pc
-
-            end_time = datetime.datetime.now().timestamp() * 1000
-            config.end_time = end_time
-            config.finished = True
-
-        ## Handle non-distributed dask scenarios
-        else:
-            config.point_count = sum(writes)
+        end_time = datetime.datetime.now().timestamp() * 1000
+        config.end_time = end_time
+        config.finished = True
+
+    ## Handle non-distributed dask scenarios
+    else:
+        config.point_count = sum(processes)
 
     # modify config to reflect result of shattter process
     config.mbr = storage.mbrs(config.time_slot)
     config.log.debug('Saving shatter metadata')
     config.end_time = datetime.datetime.now().timestamp() * 1000
     config.finished = True
 
     storage.saveMetadata('shatter', str(config), config.time_slot)
     return config.point_count
 
-
 def shatter(config: ShatterConfig) -> int:
     """
     Handle setup and running of shatter process.
     Will look for a config that has already been run before and needs to be
     resumed.
 
     :param config: :class:`silvimetric.resources.config.ShatterConfig`.
```

### Comparing `silvimetric-1.2.0/src/silvimetric/resources/bounds.py` & `silvimetric-1.2.1/src/silvimetric/resources/bounds.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/src/silvimetric/resources/config.py` & `silvimetric-1.2.1/src/silvimetric/resources/config.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/src/silvimetric/resources/data.py` & `silvimetric-1.2.1/src/silvimetric/resources/data.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/src/silvimetric/resources/entry.py` & `silvimetric-1.2.1/src/silvimetric/resources/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     def schema(self) -> Attr:
         raise NotImplementedError
 
     @abstractmethod
     def to_json(self) -> object:
         raise NotImplementedError
 
+    def toJSON(self) -> object:
+        return self.to_json()
+
     @staticmethod
     @abstractmethod
     def from_dict(data: dict):
         raise NotImplementedError
 
     @staticmethod
     @abstractmethod
```

### Comparing `silvimetric-1.2.0/src/silvimetric/resources/extents.py` & `silvimetric-1.2.1/src/silvimetric/resources/extents.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/src/silvimetric/resources/log.py` & `silvimetric-1.2.1/src/silvimetric/resources/log.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/src/silvimetric/resources/metric.py` & `silvimetric-1.2.1/src/silvimetric/resources/metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,18 @@
         return Metric(name, dtype, method, dependencies, filters, attributes)
 
     @staticmethod
     def from_string(data: str):
         j = json.loads(data)
         return Metric.from_dict(j)
 
+    def from_string(data: str):
+        j = json.loads(data)
+        return Metric.from_dict(j)
+
     def __eq__(self, other):
         return (self.name == other.name and
                 self.dtype == other.dtype and
                 self.dependencies == other.dependencies and
                 self._method == other._method,
                 self.attributes == other.attributes,
                 self.filters == other.filters)
```

### Comparing `silvimetric-1.2.0/src/silvimetric/resources/names.py` & `silvimetric-1.2.1/src/silvimetric/resources/names.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/src/silvimetric/resources/storage.py` & `silvimetric-1.2.1/src/silvimetric/resources/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,38 +176,44 @@
         """
         return self.getConfig().metrics
 
     def getDerivedNames(self) -> list[str]:
         # if no attributes are set in the metric, use all
         return [m.entry_name(a.name) for m in self.config.metrics
                 for a in self.config.attrs if not m.attributes or a in m.attributes]
+
     @contextlib.contextmanager
     def open(self, mode:str='r', timestamp=None) -> Generator[tiledb.SparseArray, None, None]:
         """
         Open stream for TileDB database in given mode and at given timestamp.
 
         :param mode: Mode to open TileDB stream in. Valid options are
             'w', 'r', 'm', 'd'., defaults to 'r'.
         :param timestamp: Timestamp to open database at., defaults to None.
         :raises Exception: Incorrect Mode was given, only valid modes are 'w' and 'r'.
         :raises Exception: Path exists and is not a TileDB array.
         :raises Exception: Path does not exist.
         :yield: TileDB array context manager.
         """
+
+        # tiledb and dask have bad interaction with opening an array if
+        # other threads present
+
         if tiledb.object_type(self.config.tdb_dir) == "array":
             if mode in ['w', 'r', 'd', 'm']:
                 tdb = tiledb.open(self.config.tdb_dir, mode, timestamp=timestamp)
             else:
                 raise Exception(f"Given open mode '{mode}' is not valid")
         elif pathlib.Path(self.config.tdb_dir).exists():
             raise Exception(f"Path {self.config.tdb_dir} already exists and is not" +
-                            " initialized for TileDB access.")
+                    " initialized for TileDB access.")
         else:
             raise Exception(f"Path {self.config.tdb_dir} does not exist")
 
+        # return tdb
         try:
             yield tdb
         finally:
             tdb.close()
 
     def reserve_time_slot(self) -> int:
         """
```

### Comparing `silvimetric-1.2.0/src/silvimetric.egg-info/PKG-INFO` & `silvimetric-1.2.1/src/silvimetric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silvimetric
-Version: 1.2.0
+Version: 1.2.1
 Summary: A forestry LiDAR processing package
 Author-email: Kyle Mann <kyle@hobu.co>, Howard Butler <howard@hobu.co>
 Maintainer-email: Kyle Mann <kyle@hobu.co>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/hobuinc/silvimetric
 Project-URL: repository, https://github.com/hobuinc/silvimetric
 Classifier: Development Status :: 4 - Beta
```

### Comparing `silvimetric-1.2.0/src/silvimetric.egg-info/SOURCES.txt` & `silvimetric-1.2.1/src/silvimetric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/tests/test_cli.py` & `silvimetric-1.2.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/tests/test_commands.py` & `silvimetric-1.2.1/tests/test_commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,27 @@
             assert len(h['history']) == 5-i
             idx = i - 1
             manage.delete(tdb_filepath, ids[idx])
 
         h = info.info(tdb_dir=tdb_filepath)
         assert not bool(h['history'])
 
+    def test_311_failure(self, shatter_config, dask_proc_client):
+        # make sure we handle tiledb contexts correctly within dask
+
+        tdb_dir = shatter_config.tdb_dir
+        shatter.shatter(shatter_config)
+
+        i = info.info(tdb_dir)
+        history = i['history'][-1]
+
+        finished_config = ShatterConfig.from_dict(history)
+        sh_id = finished_config.name
+        manage.delete(tdb_dir, sh_id)
+
     def test_restart(self, tdb_filepath, config_split):
         ids = [c.name for c in config_split]
 
         for i in range(1,len(ids)+1):
             h = info.info(tdb_dir=tdb_filepath)
 
             assert bool(h['history'])
```

### Comparing `silvimetric-1.2.0/tests/test_configuration.py` & `silvimetric-1.2.1/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/tests/test_data.py` & `silvimetric-1.2.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/tests/test_extents.py` & `silvimetric-1.2.1/tests/test_extents.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/tests/test_extract.py` & `silvimetric-1.2.1/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/tests/test_metrics.py` & `silvimetric-1.2.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/tests/test_shatter.py` & `silvimetric-1.2.1/tests/test_shatter.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.2.0/tests/test_storage.py` & `silvimetric-1.2.1/tests/test_storage.py`

 * *Files identical despite different names*

