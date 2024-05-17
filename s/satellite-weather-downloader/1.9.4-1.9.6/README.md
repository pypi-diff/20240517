# Comparing `tmp/satellite_weather_downloader-1.9.4.tar.gz` & `tmp/satellite_weather_downloader-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satellite_weather_downloader-1.9.4.tar", max compression
+gzip compressed data, was "satellite_weather_downloader-1.9.6.tar", max compression
```

## Comparing `satellite_weather_downloader-1.9.4.tar` & `satellite_weather_downloader-1.9.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35149 2024-03-07 21:43:41.437977 satellite_weather_downloader-1.9.4/LICENSE
--rw-r--r--   0        0        0     3051 2024-03-07 21:43:41.437977 satellite_weather_downloader-1.9.4/README.md
--rw-r--r--   0        0        0     2005 2024-03-07 21:44:43.126313 satellite_weather_downloader-1.9.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-07 21:43:41.441977 satellite_weather_downloader-1.9.4/satellite/__init__.py
--rw-r--r--   0        0        0      223 2024-03-07 21:43:41.441977 satellite_weather_downloader-1.9.4/satellite/downloader/__init__.py
--rw-r--r--   0        0        0    11195 2024-03-07 21:43:41.441977 satellite_weather_downloader-1.9.4/satellite/downloader/extract_reanalysis.py
--rw-r--r--   0        0        0       52 2024-03-07 21:43:41.441977 satellite_weather_downloader-1.9.4/satellite/downloader/reanalysis/__init__.py
--rw-r--r--   0        0        0    12112 2024-03-07 21:43:41.441977 satellite_weather_downloader-1.9.4/satellite/downloader/reanalysis/api_vars.py
--rw-r--r--   0        0        0    15990 2024-03-07 21:43:41.441977 satellite_weather_downloader-1.9.4/satellite/downloader/reanalysis/prompt.py
--rw-r--r--   0        0        0     2907 2024-03-07 21:43:41.441977 satellite_weather_downloader-1.9.4/satellite/downloader/request.py
--rw-r--r--   0        0        0      325 2024-03-07 21:43:41.441977 satellite_weather_downloader-1.9.4/satellite/weather/__init__.py
--rw-r--r--   0        0        0       28 2024-03-07 21:43:41.441977 satellite_weather_downloader-1.9.4/satellite/weather/brazil/DSEI/__init__.py
--rw-r--r--   0        0        0     1299 2024-03-07 21:43:41.441977 satellite_weather_downloader-1.9.4/satellite/weather/brazil/DSEI/areas.py
--rw-r--r--   0        0        0       11 2024-03-07 21:43:41.441977 satellite_weather_downloader-1.9.4/satellite/weather/brazil/DSEI/areas_dsei.cst
--rw-r--r--   0        0        0     9413 2024-03-07 21:43:41.445977 satellite_weather_downloader-1.9.4/satellite/weather/brazil/DSEI/areas_dsei.dbf
--rw-r--r--   0        0        0      417 2024-03-07 21:43:41.445977 satellite_weather_downloader-1.9.4/satellite/weather/brazil/DSEI/areas_dsei.prj
--rw-r--r--   0        0        0 11174984 2024-03-07 21:43:41.501977 satellite_weather_downloader-1.9.4/satellite/weather/brazil/DSEI/areas_dsei.shp
--rw-r--r--   0        0        0      372 2024-03-07 21:43:41.501977 satellite_weather_downloader-1.9.4/satellite/weather/brazil/DSEI/areas_dsei.shx
--rw-r--r--   0        0        0       85 2024-03-07 21:43:41.501977 satellite_weather_downloader-1.9.4/satellite/weather/brazil/__init__.py
--rw-r--r--   0        0        0     3320 2024-03-07 21:43:41.501977 satellite_weather_downloader-1.9.4/satellite/weather/brazil/extract_coordinates.py
--rw-r--r--   0        0        0     1398 2024-03-07 21:43:41.501977 satellite_weather_downloader-1.9.4/satellite/weather/brazil/extract_latlons.py
--rw-r--r--   0        0        0  1175431 2024-03-07 21:43:41.505977 satellite_weather_downloader-1.9.4/satellite/weather/brazil/municipios.json
--rw-r--r--   0        0        0    10168 2024-03-07 21:43:41.505977 satellite_weather_downloader-1.9.4/satellite/weather/copebr.py
--rw-r--r--   0        0        0     2542 2024-03-07 21:43:41.505977 satellite_weather_downloader-1.9.4/satellite/weather/dsei.py
--rw-r--r--   0        0        0     4777 1970-01-01 00:00:00.000000 satellite_weather_downloader-1.9.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-11-12 22:13:16.538097 satellite_weather_downloader-1.9.6/LICENSE
+-rw-r--r--   0        0        0     3051 2023-11-12 22:13:16.538097 satellite_weather_downloader-1.9.6/README.md
+-rw-r--r--   0        0        0     2006 2024-05-17 20:27:41.647470 satellite_weather_downloader-1.9.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-12 22:13:16.542097 satellite_weather_downloader-1.9.6/satellite/__init__.py
+-rw-r--r--   0        0        0      223 2023-11-12 22:13:16.554097 satellite_weather_downloader-1.9.6/satellite/downloader/__init__.py
+-rw-r--r--   0        0        0    11195 2024-02-19 19:47:21.561446 satellite_weather_downloader-1.9.6/satellite/downloader/extract_reanalysis.py
+-rw-r--r--   0        0        0       52 2023-11-12 22:13:16.546097 satellite_weather_downloader-1.9.6/satellite/downloader/reanalysis/__init__.py
+-rw-r--r--   0        0        0    12112 2023-11-12 22:13:16.550097 satellite_weather_downloader-1.9.6/satellite/downloader/reanalysis/api_vars.py
+-rw-r--r--   0        0        0    15990 2023-11-12 22:13:16.550097 satellite_weather_downloader-1.9.6/satellite/downloader/reanalysis/prompt.py
+-rw-r--r--   0        0        0     2907 2023-11-12 22:13:16.554097 satellite_weather_downloader-1.9.6/satellite/downloader/request.py
+-rw-r--r--   0        0        0      325 2023-11-12 22:13:16.554097 satellite_weather_downloader-1.9.6/satellite/weather/__init__.py
+-rw-r--r--   0        0        0       28 2023-11-12 22:13:16.590098 satellite_weather_downloader-1.9.6/satellite/weather/brazil/DSEI/__init__.py
+-rw-r--r--   0        0        0     1299 2023-11-12 22:13:16.562097 satellite_weather_downloader-1.9.6/satellite/weather/brazil/DSEI/areas.py
+-rw-r--r--   0        0        0       11 2023-11-12 22:13:16.566097 satellite_weather_downloader-1.9.6/satellite/weather/brazil/DSEI/areas_dsei.cst
+-rw-r--r--   0        0        0     9413 2023-11-12 22:13:16.566097 satellite_weather_downloader-1.9.6/satellite/weather/brazil/DSEI/areas_dsei.dbf
+-rw-r--r--   0        0        0      417 2023-11-12 22:13:16.566097 satellite_weather_downloader-1.9.6/satellite/weather/brazil/DSEI/areas_dsei.prj
+-rw-r--r--   0        0        0 11174984 2023-11-12 22:13:16.590098 satellite_weather_downloader-1.9.6/satellite/weather/brazil/DSEI/areas_dsei.shp
+-rw-r--r--   0        0        0      372 2023-11-12 22:13:16.590098 satellite_weather_downloader-1.9.6/satellite/weather/brazil/DSEI/areas_dsei.shx
+-rw-r--r--   0        0        0       85 2023-11-12 22:13:16.562097 satellite_weather_downloader-1.9.6/satellite/weather/brazil/__init__.py
+-rw-r--r--   0        0        0     3320 2024-02-19 19:47:21.477444 satellite_weather_downloader-1.9.6/satellite/weather/brazil/extract_coordinates.py
+-rw-r--r--   0        0        0     1398 2024-02-19 19:47:21.469444 satellite_weather_downloader-1.9.6/satellite/weather/brazil/extract_latlons.py
+-rw-r--r--   0        0        0  1175431 2023-12-21 12:24:01.426567 satellite_weather_downloader-1.9.6/satellite/weather/brazil/municipios.json
+-rw-r--r--   0        0        0    10384 2024-05-16 21:24:43.738241 satellite_weather_downloader-1.9.6/satellite/weather/copebr.py
+-rw-r--r--   0        0        0     2542 2023-11-12 22:13:16.558097 satellite_weather_downloader-1.9.6/satellite/weather/dsei.py
+-rw-r--r--   0        0        0     4767 1970-01-01 00:00:00.000000 satellite_weather_downloader-1.9.6/PKG-INFO
```

### Comparing `satellite_weather_downloader-1.9.4/LICENSE` & `satellite_weather_downloader-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.9.4/README.md` & `satellite_weather_downloader-1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.9.4/pyproject.toml` & `satellite_weather_downloader-1.9.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "satellite-weather-downloader"
-version = "1.9.4"  # changed by semantic-release
+version = "1.9.6"  # changed by semantic-release
 description = "The modules available in this package are designed to capture and proccess satellite data from Copernicus"
 readme = "README.md"
 authors = ["Luã Bida Vacaro <luabidaa@gmail.com>"]
 maintainers = ["Luã Bida Vacaro <luabidaa@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/osl-incubator/satellite-weather-downloader"
 homepage = "https://github.com/osl-incubator/satellite-weather-downloader"
@@ -41,15 +41,15 @@
 loguru = "^0.6.0"
 amqp = "^5.1.1"
 requests = "^2.28.2"
 prompt-toolkit = "^3.0.36"
 geopandas = "^0.12.2"
 matplotlib = "^3.6.3"
 shapely = ">=2.0.3"
-dask = "^2023.3.1"
+dask = ">=2024.5.0"
 xarray = ">=2023.7.0"
 gdal = "^3.8.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4"
 jupyterlab = "^3.4.8"
 seaborn = "^0.12.1"
```

### Comparing `satellite_weather_downloader-1.9.4/satellite/downloader/extract_reanalysis.py` & `satellite_weather_downloader-1.9.6/satellite/downloader/extract_reanalysis.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.9.4/satellite/downloader/reanalysis/api_vars.py` & `satellite_weather_downloader-1.9.6/satellite/downloader/reanalysis/api_vars.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.9.4/satellite/downloader/reanalysis/prompt.py` & `satellite_weather_downloader-1.9.6/satellite/downloader/reanalysis/prompt.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.9.4/satellite/downloader/request.py` & `satellite_weather_downloader-1.9.6/satellite/downloader/request.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.9.4/satellite/weather/brazil/DSEI/areas.py` & `satellite_weather_downloader-1.9.6/satellite/weather/brazil/DSEI/areas.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.9.4/satellite/weather/brazil/DSEI/areas_dsei.dbf` & `satellite_weather_downloader-1.9.6/satellite/weather/brazil/DSEI/areas_dsei.dbf`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.9.4/satellite/weather/brazil/DSEI/areas_dsei.shp` & `satellite_weather_downloader-1.9.6/satellite/weather/brazil/DSEI/areas_dsei.shp`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.9.4/satellite/weather/brazil/extract_coordinates.py` & `satellite_weather_downloader-1.9.6/satellite/weather/brazil/extract_coordinates.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.9.4/satellite/weather/brazil/extract_latlons.py` & `satellite_weather_downloader-1.9.6/satellite/weather/brazil/extract_latlons.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.9.4/satellite/weather/brazil/municipios.json` & `satellite_weather_downloader-1.9.6/satellite/weather/brazil/municipios.json`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.9.4/satellite/weather/copebr.py` & `satellite_weather_downloader-1.9.6/satellite/weather/copebr.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,18 @@
 
     def to_dataframe(self, geocodes: Union[list, int], raw: bool = False):
         df = _final_dataframe(dataset=self._ds, geocodes=geocodes, raw=raw)
 
         if type(df) == dask.dataframe.core.DataFrame:
             df = df.compute()
 
+        columns_to_round = list(set(df.columns).difference(set(["date", "geocodigo"])))
+
+        df[columns_to_round] = df[columns_to_round].map(lambda x: np.round(x, 4))
+
         df = df.reset_index(drop=True)
 
         return df
 
     def to_sql(
         self,
         geocodes: Union[list, int],
@@ -279,14 +283,15 @@
 
 def _reduce_by(ds: xr.Dataset, func, prefix: str):
     """
     Applies a function to each coordinate in the dataset and
     replace the `data_vars` names to it's corresponding prefix.
     """
     ds = ds.apply(func=func)
+    # ds = ds.map(lambda x: np.round(x, 4))
     return ds.rename(
         dict(
             zip(
                 list(ds.data_vars),
                 list(map(lambda x: f"{x}_{prefix}", list(ds.data_vars))),
             )
         )
```

### Comparing `satellite_weather_downloader-1.9.4/satellite/weather/dsei.py` & `satellite_weather_downloader-1.9.6/satellite/weather/dsei.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.9.4/PKG-INFO` & `satellite_weather_downloader-1.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satellite-weather-downloader
-Version: 1.9.4
+Version: 1.9.6
 Summary: The modules available in this package are designed to capture and proccess satellite data from Copernicus
 Home-page: https://github.com/osl-incubator/satellite-weather-downloader
 License: GNU GPL v3.0
 Author: Luã Bida Vacaro
 Author-email: luabidaa@gmail.com
 Maintainer: Luã Bida Vacaro
 Maintainer-email: luabidaa@gmail.com
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: SQLAlchemy (>=2.0.28)
 Requires-Dist: amqp (>=5.1.1,<6.0.0)
 Requires-Dist: cdsapi (>=0.5.1,<0.6.0)
-Requires-Dist: dask (>=2023.3.1,<2024.0.0)
+Requires-Dist: dask (>=2024.5.0)
 Requires-Dist: gdal (>=3.8.4,<4.0.0)
 Requires-Dist: geopandas (>=0.12.2,<0.13.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: matplotlib (>=3.6.3,<4.0.0)
 Requires-Dist: netCDF4 (>=1.6.1,<2.0.0)
 Requires-Dist: numpy (>=1.16.4)
 Requires-Dist: pandas (>=2.0.0)
```

