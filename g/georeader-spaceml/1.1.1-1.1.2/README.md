# Comparing `tmp/georeader-spaceml-1.1.1.tar.gz` & `tmp/georeader-spaceml-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "georeader-spaceml-1.1.1.tar", last modified: Thu May  2 08:26:13 2024, max compression
+gzip compressed data, was "georeader-spaceml-1.1.2.tar", last modified: Fri May 17 07:19:40 2024, max compression
```

## Comparing `georeader-spaceml-1.1.1.tar` & `georeader-spaceml-1.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-02 08:26:13.675946 georeader-spaceml-1.1.1/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     7652 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.1/LICENSE
--rw-r--r--   0 gonzalo   (1000) gonzalo   (1000)     9379 2024-05-02 08:26:13.675946 georeader-spaceml-1.1.1/PKG-INFO
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6803 2024-05-02 07:50:25.000000 georeader-spaceml-1.1.1/README.md
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-02 08:26:13.671946 georeader-spaceml-1.1.1/georeader/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)   118602 2023-10-10 04:52:24.000000 georeader-spaceml-1.1.1/georeader/SolarIrradiance_Thuillier.csv
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2180 2024-05-02 08:24:04.000000 georeader-spaceml-1.1.1/georeader/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2549 2023-10-02 08:09:01.000000 georeader-spaceml-1.1.1/georeader/abstract_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5139 2024-04-02 07:44:03.000000 georeader-spaceml-1.1.1/georeader/dataarray.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    28666 2024-05-02 05:57:00.000000 georeader-spaceml-1.1.1/georeader/geotensor.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     9257 2024-02-28 17:48:55.000000 georeader-spaceml-1.1.1/georeader/griddata.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11516 2024-03-01 12:59:18.000000 georeader-spaceml-1.1.1/georeader/mosaic.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11134 2024-01-09 11:32:45.000000 georeader-spaceml-1.1.1/georeader/plot.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    35477 2024-03-05 14:52:32.000000 georeader-spaceml-1.1.1/georeader/rasterio_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     9514 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.1/georeader/rasterize.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    34265 2024-04-03 08:10:54.000000 georeader-spaceml-1.1.1/georeader/read.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-02 08:26:13.675946 georeader-spaceml-1.1.1/georeader/readers/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    57165 2024-05-02 07:44:41.000000 georeader-spaceml-1.1.1/georeader/readers/S2_SAFE_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.1/georeader/readers/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12416 2023-05-05 11:24:40.000000 georeader-spaceml-1.1.1/georeader/readers/download_pv_product.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2454 2024-02-28 16:40:43.000000 georeader-spaceml-1.1.1/georeader/readers/download_utils.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     7268 2024-04-03 08:57:10.000000 georeader-spaceml-1.1.1/georeader/readers/ee_image.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    14121 2024-01-05 10:02:42.000000 georeader-spaceml-1.1.1/georeader/readers/ee_query.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    33154 2024-04-10 11:36:43.000000 georeader-spaceml-1.1.1/georeader/readers/emit.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12527 2024-03-01 21:44:02.000000 georeader-spaceml-1.1.1/georeader/readers/prisma.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    18752 2024-05-02 08:23:57.000000 georeader-spaceml-1.1.1/georeader/readers/probav_image_operational.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2156 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.1/georeader/readers/query_utils.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3991 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.1/georeader/readers/scihubcopernicus_query.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    13864 2024-05-02 07:45:05.000000 georeader-spaceml-1.1.1/georeader/readers/spotvgt_image_operational.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2258 2023-12-21 09:41:42.000000 georeader-spaceml-1.1.1/georeader/readers/tileserver.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12969 2024-03-04 07:44:43.000000 georeader-spaceml-1.1.1/georeader/reflectance.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12131 2023-10-18 15:46:26.000000 georeader-spaceml-1.1.1/georeader/save.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       46 2023-07-13 10:32:41.000000 georeader-spaceml-1.1.1/georeader/save_cog.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5414 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.1/georeader/slices.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3575 2023-09-22 12:24:44.000000 georeader-spaceml-1.1.1/georeader/vectorize.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11423 2024-04-03 08:56:42.000000 georeader-spaceml-1.1.1/georeader/window_utils.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-02 08:26:13.675946 georeader-spaceml-1.1.1/georeader_spaceml.egg-info/
--rw-r--r--   0 gonzalo   (1000) gonzalo   (1000)     9379 2024-05-02 08:26:13.000000 georeader-spaceml-1.1.1/georeader_spaceml.egg-info/PKG-INFO
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1171 2024-05-02 08:26:13.000000 georeader-spaceml-1.1.1/georeader_spaceml.egg-info/SOURCES.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        1 2024-05-02 08:26:13.000000 georeader-spaceml-1.1.1/georeader_spaceml.egg-info/dependency_links.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      513 2024-05-02 08:26:13.000000 georeader-spaceml-1.1.1/georeader_spaceml.egg-info/requires.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       10 2024-05-02 08:26:13.000000 georeader-spaceml-1.1.1/georeader_spaceml.egg-info/top_level.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       38 2024-05-02 08:26:13.679946 georeader-spaceml-1.1.1/setup.cfg
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2780 2023-12-19 08:18:42.000000 georeader-spaceml-1.1.1/setup.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-02 08:26:13.675946 georeader-spaceml-1.1.1/tests/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3796 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.1/tests/test_geotensor.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3583 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.1/tests/test_rasterio_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11460 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.1/tests/test_xarray_utils.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-17 07:19:40.032694 georeader-spaceml-1.1.2/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     7652 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/LICENSE
+-rw-r--r--   0 gonzalo   (1000) gonzalo   (1000)     9379 2024-05-17 07:19:40.032694 georeader-spaceml-1.1.2/PKG-INFO
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6803 2024-05-02 07:50:25.000000 georeader-spaceml-1.1.2/README.md
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-17 07:19:40.028694 georeader-spaceml-1.1.2/georeader/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)   118602 2023-10-10 04:52:24.000000 georeader-spaceml-1.1.2/georeader/SolarIrradiance_Thuillier.csv
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2180 2024-05-02 10:15:20.000000 georeader-spaceml-1.1.2/georeader/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2549 2023-10-02 08:09:01.000000 georeader-spaceml-1.1.2/georeader/abstract_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5394 2024-05-10 11:53:41.000000 georeader-spaceml-1.1.2/georeader/dataarray.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    28666 2024-05-02 05:57:00.000000 georeader-spaceml-1.1.2/georeader/geotensor.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     9257 2024-02-28 17:48:55.000000 georeader-spaceml-1.1.2/georeader/griddata.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11516 2024-03-01 12:59:18.000000 georeader-spaceml-1.1.2/georeader/mosaic.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11134 2024-01-09 11:32:45.000000 georeader-spaceml-1.1.2/georeader/plot.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    35477 2024-03-05 14:52:32.000000 georeader-spaceml-1.1.2/georeader/rasterio_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     9514 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/georeader/rasterize.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    34265 2024-04-03 08:10:54.000000 georeader-spaceml-1.1.2/georeader/read.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-17 07:19:40.032694 georeader-spaceml-1.1.2/georeader/readers/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    57165 2024-05-02 07:44:41.000000 georeader-spaceml-1.1.2/georeader/readers/S2_SAFE_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/georeader/readers/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12416 2023-05-05 11:24:40.000000 georeader-spaceml-1.1.2/georeader/readers/download_pv_product.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2454 2024-02-28 16:40:43.000000 georeader-spaceml-1.1.2/georeader/readers/download_utils.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    10780 2024-05-17 06:24:46.000000 georeader-spaceml-1.1.2/georeader/readers/ee_image.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    14387 2024-05-17 05:51:47.000000 georeader-spaceml-1.1.2/georeader/readers/ee_query.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    33154 2024-04-10 11:36:43.000000 georeader-spaceml-1.1.2/georeader/readers/emit.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12527 2024-03-01 21:44:02.000000 georeader-spaceml-1.1.2/georeader/readers/prisma.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    18752 2024-05-02 08:23:57.000000 georeader-spaceml-1.1.2/georeader/readers/probav_image_operational.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2156 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/georeader/readers/query_utils.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3991 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/georeader/readers/scihubcopernicus_query.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    13869 2024-05-02 10:11:31.000000 georeader-spaceml-1.1.2/georeader/readers/spotvgt_image_operational.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3014 2024-05-17 07:17:50.000000 georeader-spaceml-1.1.2/georeader/readers/tileserver.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12969 2024-03-04 07:44:43.000000 georeader-spaceml-1.1.2/georeader/reflectance.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12131 2023-10-18 15:46:26.000000 georeader-spaceml-1.1.2/georeader/save.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       46 2023-07-13 10:32:41.000000 georeader-spaceml-1.1.2/georeader/save_cog.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5414 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/georeader/slices.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3575 2023-09-22 12:24:44.000000 georeader-spaceml-1.1.2/georeader/vectorize.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11423 2024-04-03 08:56:42.000000 georeader-spaceml-1.1.2/georeader/window_utils.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-17 07:19:40.032694 georeader-spaceml-1.1.2/georeader_spaceml.egg-info/
+-rw-r--r--   0 gonzalo   (1000) gonzalo   (1000)     9379 2024-05-17 07:19:39.000000 georeader-spaceml-1.1.2/georeader_spaceml.egg-info/PKG-INFO
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1171 2024-05-17 07:19:39.000000 georeader-spaceml-1.1.2/georeader_spaceml.egg-info/SOURCES.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        1 2024-05-17 07:19:39.000000 georeader-spaceml-1.1.2/georeader_spaceml.egg-info/dependency_links.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      513 2024-05-17 07:19:39.000000 georeader-spaceml-1.1.2/georeader_spaceml.egg-info/requires.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       10 2024-05-17 07:19:39.000000 georeader-spaceml-1.1.2/georeader_spaceml.egg-info/top_level.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       38 2024-05-17 07:19:40.032694 georeader-spaceml-1.1.2/setup.cfg
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2780 2023-12-19 08:18:42.000000 georeader-spaceml-1.1.2/setup.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-17 07:19:40.032694 georeader-spaceml-1.1.2/tests/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3796 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/tests/test_geotensor.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3583 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/tests/test_rasterio_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11460 2023-04-26 06:58:45.000000 georeader-spaceml-1.1.2/tests/test_xarray_utils.py
```

### Comparing `georeader-spaceml-1.1.1/LICENSE` & `georeader-spaceml-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/PKG-INFO` & `georeader-spaceml-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: georeader-spaceml
-Version: 1.1.1
+Version: 1.1.2
 Summary: Lightweight reader for raster files
 Home-page: https://github.com/spaceml-org/georeader
 Author: Gonzalo Mateo-Garcia
 Keywords: raster reading,rasterio
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `georeader-spaceml-1.1.1/README.md` & `georeader-spaceml-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/SolarIrradiance_Thuillier.csv` & `georeader-spaceml-1.1.2/georeader/SolarIrradiance_Thuillier.csv`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/__init__.py` & `georeader-spaceml-1.1.2/georeader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 import math
 from typing import Tuple, Any, Union
 from shapely.geometry.base import BaseGeometry
 from shapely import Geometry
 from shapely.geometry import shape, mapping
 import rasterio.warp
```

### Comparing `georeader-spaceml-1.1.1/georeader/abstract_reader.py` & `georeader-spaceml-1.1.2/georeader/abstract_reader.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/dataarray.py` & `georeader-spaceml-1.1.2/georeader/dataarray.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,36 +65,39 @@
     nx, ny = shape[1], shape[0]
     x, _ = transform * (np.arange(nx) + 0.5, np.zeros(nx) + 0.5)
     _, y = transform * (np.zeros(ny) + 0.5, np.arange(ny) + 0.5)
 
     return {x_axis_name: x, y_axis_name: y}
 
 
-def toDataArray(x:GeoTensor, x_axis_name:str="x", y_axis_name:str="y") -> xr.DataArray:
+def toDataArray(x:GeoTensor, x_axis_name:str="x", y_axis_name:str="y", extra_coords:Optional[Dict[str, Any]]=None) -> xr.DataArray:
     """
     Convert a GeoTensor to a xr.DataArray object.
 
     Args:
         x (GeoTensor): Input GeoTensor
         x_axis_name (str, optional): name to the x axis. Defaults to "x".
         y_axis_name (str, optional): name to the y axis. Defaults to "y".
+        extra_coords (Optional[Dict[str, Any]], optional): Extra coordinates. Defaults to None.
 
     Returns:
         xr.DataArray: Output xr.DataArray
     """
     coords = getcoords_from_transform_shape(x.transform, x.shape[-2:], 
                                             x_axis_name=x_axis_name, y_axis_name=y_axis_name)
     cords_ordered = OrderedDict()
     for d in x.dims:
-        if d not in coords:
-            cords_ordered[d] = np.arange(x.shape[x.dims.index(d)])
-        else:
+        if (extra_coords is not None) and (d in extra_coords):
+            cords_ordered[d] = extra_coords[d]
+        elif d in coords:
             cords_ordered[d] = coords[d]
+        else:
+            cords_ordered[d] = np.arange(x.shape[x.dims.index(d)])
     
-    return xr.DataArray(x.values, coords=coords, 
+    return xr.DataArray(x.values, coords=cords_ordered, 
                         dims=x.dims,
                         attrs={"crs":x.crs , 
                                "fill_value_default":x.fill_value_default})
 
 
 def fromDataArray(x: xr.DataArray, crs:Optional[Any]=None, 
                   fill_value_default:Optional[Union[float, int]]=None,
```

### Comparing `georeader-spaceml-1.1.1/georeader/geotensor.py` & `georeader-spaceml-1.1.2/georeader/geotensor.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/griddata.py` & `georeader-spaceml-1.1.2/georeader/griddata.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/mosaic.py` & `georeader-spaceml-1.1.2/georeader/mosaic.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/plot.py` & `georeader-spaceml-1.1.2/georeader/plot.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/rasterio_reader.py` & `georeader-spaceml-1.1.2/georeader/rasterio_reader.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/rasterize.py` & `georeader-spaceml-1.1.2/georeader/rasterize.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/read.py` & `georeader-spaceml-1.1.2/georeader/read.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/readers/S2_SAFE_reader.py` & `georeader-spaceml-1.1.2/georeader/readers/S2_SAFE_reader.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/readers/download_pv_product.py` & `georeader-spaceml-1.1.2/georeader/readers/download_pv_product.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/readers/download_utils.py` & `georeader-spaceml-1.1.2/georeader/readers/download_utils.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/readers/ee_query.py` & `georeader-spaceml-1.1.2/georeader/readers/ee_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,27 +91,30 @@
         raise ValueError(f"Tile {tile} not recognized")
 
 
 def query(area:Union[MultiPolygon,Polygon],
           date_start:datetime, date_end:datetime,
           producttype:str='S2', filter_duplicates:bool=True,
           return_collection:bool=False,
-          add_s2cloudless:bool=False)-> Union[gpd.GeoDataFrame, Tuple[gpd.GeoDataFrame, ee.ImageCollection]]:
+          add_s2cloudless:bool=False,
+          extra_metadata_keys:Optional[List[str]]=None
+          )-> Union[gpd.GeoDataFrame, Tuple[gpd.GeoDataFrame, ee.ImageCollection]]:
     """
     Query Landsat and Sentinel-2 products from the Google Earth Engine.
 
     Args:
         area: area to query images in EPSG:4326
         date_start: datetime in a given timezone. If tz not provided UTC will be assumed.
         date_end: datetime in UTC. If tz not provided UTC will be assumed.
         producttype: 'S2', "Landsat"-> {"L8", "L9"}, "both" -> {"S2", "L8", "L9"}, "S2_SR", "L8", "L9"
         filter_duplicates: Filter S2 images that are duplicated
         return_collection: returns also the corresponding image collection
         add_s2cloudless: Adds a column that indicates if the s2cloudless image is available (from collection
             COPERNICUS/S2_CLOUD_PROBABILITY collection)
+        extra_metadata_keys: list of extra metadata keys to add to the geodataframe.
 
     Returns:
         geodataframe with available products in the given area and time range
         if `return_collection` is True it also returns the `ee.ImageCollection` of available images
     """
 
     pol = ee.Geometry(mapping(area))
@@ -165,16 +168,19 @@
         pol)
         img_col = img_col.merge(img_col_l9)
         img_col_l9_t2 = ee.ImageCollection("LANDSAT/LC09/C02/T2_TOA").filterDate(date_start.replace(tzinfo=None),
                                                                    date_end.replace(tzinfo=None)).filterBounds(
         pol)
         img_col = img_col.merge(img_col_l9_t2)
 
+    if extra_metadata_keys is None:
+        extra_metadata_keys = []
+
     geodf = img_collection_to_feature_collection(img_col,
-                                                 ["system:time_start"] + list(keys_query.keys()),
+                                                 ["system:time_start"] + list(keys_query.keys()) + extra_metadata_keys,
                                                 as_geopandas=True, band_crs="B2")
 
     geodf.rename(keys_query, axis=1, inplace=True)
 
     if geodf.shape[0] > 0:
         if (producttype == "Landsat") or (producttype == "both"):
             geodf["collection_name"] = geodf["title"].apply(figure_out_collection_landsat)
@@ -186,15 +192,15 @@
     if producttype == "both":
         img_col_s2 = ee.ImageCollection("COPERNICUS/S2_HARMONIZED").filterDate(date_start.replace(tzinfo=None),
                                                                               date_end.replace(
                                                                                   tzinfo=None)).filterBounds(
             pol)
         keys_query_s2 = {"PRODUCT_ID": "title", 'CLOUDY_PIXEL_PERCENTAGE': "cloudcoverpercentage"}
         geodf_s2 = img_collection_to_feature_collection(img_col_s2,
-                                                        ["system:time_start"] + list(keys_query_s2.keys()),
+                                                        ["system:time_start"] + list(keys_query_s2.keys()) + extra_metadata_keys,
                                                         as_geopandas=True, band_crs="B2")
         geodf_s2["collection_name"] = "COPERNICUS/S2_HARMONIZED"
         geodf_s2.rename(keys_query_s2, axis=1, inplace=True)
         if geodf_s2.shape[0] > 0:
             if geodf.shape[0] == 0:
                 geodf = geodf_s2
             else:
```

### Comparing `georeader-spaceml-1.1.1/georeader/readers/emit.py` & `georeader-spaceml-1.1.2/georeader/readers/emit.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/readers/prisma.py` & `georeader-spaceml-1.1.2/georeader/readers/prisma.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/readers/probav_image_operational.py` & `georeader-spaceml-1.1.2/georeader/readers/probav_image_operational.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/readers/query_utils.py` & `georeader-spaceml-1.1.2/georeader/readers/query_utils.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/readers/scihubcopernicus_query.py` & `georeader-spaceml-1.1.2/georeader/readers/scihubcopernicus_query.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/readers/spotvgt_image_operational.py` & `georeader-spaceml-1.1.2/georeader/readers/spotvgt_image_operational.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from georeader import window_utils, geotensor
 from numbers import Number
 from shapely.geometry import Polygon
 import numpy as np
 import datetime as dt
 from glob import glob
 from pyhdf.SD import SD, SDC
+import warnings
 
 
 FILES = ['1BL', '1BO', 'AG', 'B0', 'B2', 'B3', 'MIR',
          'OG', 'SAA', 'SM', 'SZA', 'VAA', 'VZA', 'WVG']
 
 BANDS_NAMES = ['B0', 'B2', 'B3', 'MIR']
 BANDS_DICT = {k: v for k, v in enumerate(BANDS_NAMES)}
@@ -114,21 +115,21 @@
                                                    width=self.real_shape[1],
                                                    height=self.real_shape[0])
 
         year, month, day = re.match(r'(\d{4})(\d{2})(\d{2})', self.metadata['SEGM_FIRST_DATE']).groups()
         hh, mm, ss = re.match(r'(\d{2})(\d{2})(\d{2})', self.metadata['SEGM_FIRST_TIME']).groups()
 
         self.start_date = dt.datetime(day=int(day), month=int(month), year=int(year),
-                                      hour=int(hh), minute=int(mm), second=int(ss)).strftime("%Y-%m-%d %H:%M:%S")
+                                      hour=int(hh), minute=int(mm), second=int(ss), tzinfo=dt.timezone.utc)
 
         year, month, day = re.match(r'(\d{4})(\d{2})(\d{2})', self.metadata['SEGM_LAST_DATE']).groups()
         hh, mm, ss = re.match(r'(\d{2})(\d{2})(\d{2})', self.metadata['SEGM_LAST_TIME']).groups()
 
         self.end_date = dt.datetime(day=int(day), month=int(month), year=int(year),
-                                    hour=int(hh), minute=int(mm), second=int(ss)).strftime("%Y-%m-%d %H:%M:%S")
+                                    hour=int(hh), minute=int(mm), second=int(ss), tzinfo=dt.timezone.utc)
 
         # self.map_projection_wkt
 
         self.toatoc = "TOA"
 
         self.res_name = '1KM'
```

### Comparing `georeader-spaceml-1.1.1/georeader/readers/tileserver.py` & `georeader-spaceml-1.1.2/georeader/readers/tileserver.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import numpy as np
 import georeader
 from georeader import window_utils
 from georeader import read
 import rasterio.windows
 import rasterio.transform
 from shapely.geometry import box
+from concurrent.futures import ThreadPoolExecutor
 
 def read_from_tileserver(tile_server:str, geometry:Union[Polygon, MultiPolygon],
                          zoom:int=16, crs_geometry:Any="EPSG:4326") -> GeoTensor:
     """
     Queries tiles from a tile server and returns it as a GeoTensor
 
     Args:
@@ -29,27 +30,40 @@
         GeoTensor: GeoTensor with the tile
     """
     if not georeader.compare_crs(crs_geometry, "EPSG:4326"):
         geometry = window_utils.polygon_to_crs(geometry, crs_geometry, "EPSG:4326")
 
     min_lon, min_lat, max_lon, max_lat = geometry.bounds
     tiles = mercantile.tiles(min_lon, min_lat, max_lon, max_lat, zooms=zoom)
-    geotensors = []
-    for tile in tiles:
-        if not box(*mercantile.bounds(tile)).intersects(geometry):
-            continue
+    tiles = [tile for tile in tiles if box(*mercantile.bounds(tile)).intersects(geometry)]
+    # geotensors = []
+    # for tile in tiles:
         
+    #     rsp = requests.get(tile_server.format(x=tile.x, y=tile.y, z=tile.z))
+    #     img = Image.open(BytesIO(rsp.content))
+    #     xmin, ymin, xmax, ymax = window_utils.normalize_bounds(mercantile.xy_bounds(tile))
+    #     img_np = np.array(img).transpose(2,0,1)
+       
+    #     transform = rasterio.transform.from_bounds(west=xmin, south=ymin, east=xmax, north=ymax,
+    #                                                width=img_np.shape[2], height=img_np.shape[1])
+
+    #     geotensors.append(GeoTensor(img_np, transform=transform, crs="EPSG:3857"))
+
+    def read_tile(tile):
         rsp = requests.get(tile_server.format(x=tile.x, y=tile.y, z=tile.z))
         img = Image.open(BytesIO(rsp.content))
         xmin, ymin, xmax, ymax = window_utils.normalize_bounds(mercantile.xy_bounds(tile))
         img_np = np.array(img).transpose(2,0,1)
        
         transform = rasterio.transform.from_bounds(west=xmin, south=ymin, east=xmax, north=ymax,
                                                    width=img_np.shape[2], height=img_np.shape[1])
 
-        geotensors.append(GeoTensor(img_np, transform=transform, crs="EPSG:3857"))
+        return GeoTensor(img_np, transform=transform, crs="EPSG:3857")
+
+    with ThreadPoolExecutor() as executor:
+        geotensors = list(executor.map(lambda tile: read_tile(tile), tiles))
     
     if len(geotensors) == 1:
         return read.read_from_polygon(geotensors[0], polygon=geometry, crs_polygon="EPSG:4326")
     
     return mosaic.spatial_mosaic(geotensors, geometry, 
                                  dst_crs="EPSG:3857", crs_polygon="EPSG:4326")
```

### Comparing `georeader-spaceml-1.1.1/georeader/reflectance.py` & `georeader-spaceml-1.1.2/georeader/reflectance.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/save.py` & `georeader-spaceml-1.1.2/georeader/save.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/slices.py` & `georeader-spaceml-1.1.2/georeader/slices.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/vectorize.py` & `georeader-spaceml-1.1.2/georeader/vectorize.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader/window_utils.py` & `georeader-spaceml-1.1.2/georeader/window_utils.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader_spaceml.egg-info/PKG-INFO` & `georeader-spaceml-1.1.2/georeader_spaceml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: georeader-spaceml
-Version: 1.1.1
+Version: 1.1.2
 Summary: Lightweight reader for raster files
 Home-page: https://github.com/spaceml-org/georeader
 Author: Gonzalo Mateo-Garcia
 Keywords: raster reading,rasterio
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `georeader-spaceml-1.1.1/georeader_spaceml.egg-info/SOURCES.txt` & `georeader-spaceml-1.1.2/georeader_spaceml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/georeader_spaceml.egg-info/requires.txt` & `georeader-spaceml-1.1.2/georeader_spaceml.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/setup.py` & `georeader-spaceml-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/tests/test_geotensor.py` & `georeader-spaceml-1.1.2/tests/test_geotensor.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/tests/test_rasterio_reader.py` & `georeader-spaceml-1.1.2/tests/test_rasterio_reader.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.1.1/tests/test_xarray_utils.py` & `georeader-spaceml-1.1.2/tests/test_xarray_utils.py`

 * *Files identical despite different names*

