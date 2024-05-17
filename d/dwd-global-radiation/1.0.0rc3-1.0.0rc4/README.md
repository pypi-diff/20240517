# Comparing `tmp/dwd_global_radiation-1.0.0rc3.tar.gz` & `tmp/dwd_global_radiation-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwd_global_radiation-1.0.0rc3.tar", last modified: Wed May 15 16:39:44 2024, max compression
+gzip compressed data, was "dwd_global_radiation-1.0.0rc4.tar", last modified: Fri May 17 11:21:39 2024, max compression
```

## Comparing `dwd_global_radiation-1.0.0rc3.tar` & `dwd_global_radiation-1.0.0rc4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-15 16:39:44.141551 dwd_global_radiation-1.0.0rc3/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1065 2024-05-05 09:59:58.000000 dwd_global_radiation-1.0.0rc3/LICENSE
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    21569 2024-05-15 16:39:44.141551 dwd_global_radiation-1.0.0rc3/PKG-INFO
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    20562 2024-05-15 12:29:56.000000 dwd_global_radiation-1.0.0rc3/README.md
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-15 16:39:44.141551 dwd_global_radiation-1.0.0rc3/dwd_global_radiation/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       45 2024-05-07 07:51:24.000000 dwd_global_radiation-1.0.0rc3/dwd_global_radiation/__init__.py
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    23349 2024-05-14 22:45:04.000000 dwd_global_radiation-1.0.0rc3/dwd_global_radiation/global_radiation.py
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    18137 2024-05-15 12:29:31.000000 dwd_global_radiation-1.0.0rc3/dwd_global_radiation/utils.py
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-15 16:39:44.141551 dwd_global_radiation-1.0.0rc3/dwd_global_radiation.egg-info/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    21569 2024-05-15 16:39:44.000000 dwd_global_radiation-1.0.0rc3/dwd_global_radiation.egg-info/PKG-INFO
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)      349 2024-05-15 16:39:44.000000 dwd_global_radiation-1.0.0rc3/dwd_global_radiation.egg-info/SOURCES.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)        1 2024-05-15 16:39:44.000000 dwd_global_radiation-1.0.0rc3/dwd_global_radiation.egg-info/dependency_links.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)      128 2024-05-15 16:39:44.000000 dwd_global_radiation-1.0.0rc3/dwd_global_radiation.egg-info/requires.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       21 2024-05-15 16:39:44.000000 dwd_global_radiation-1.0.0rc3/dwd_global_radiation.egg-info/top_level.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       38 2024-05-15 16:39:44.141551 dwd_global_radiation-1.0.0rc3/setup.cfg
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1656 2024-05-15 16:24:24.000000 dwd_global_radiation-1.0.0rc3/setup.py
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-17 11:21:39.906342 dwd_global_radiation-1.0.0rc4/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1065 2024-05-05 09:59:58.000000 dwd_global_radiation-1.0.0rc4/LICENSE
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-17 11:21:39.906342 dwd_global_radiation-1.0.0rc4/PKG-INFO
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    21423 2024-05-15 22:21:14.000000 dwd_global_radiation-1.0.0rc4/README.md
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-17 11:21:39.902342 dwd_global_radiation-1.0.0rc4/dwd_global_radiation/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       45 2024-05-07 07:51:24.000000 dwd_global_radiation-1.0.0rc4/dwd_global_radiation/__init__.py
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    23928 2024-05-17 10:30:25.000000 dwd_global_radiation-1.0.0rc4/dwd_global_radiation/global_radiation.py
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    18137 2024-05-15 21:06:36.000000 dwd_global_radiation-1.0.0rc4/dwd_global_radiation/utils.py
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-17 11:21:39.906342 dwd_global_radiation-1.0.0rc4/dwd_global_radiation.egg-info/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-17 11:21:39.000000 dwd_global_radiation-1.0.0rc4/dwd_global_radiation.egg-info/PKG-INFO
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)      349 2024-05-17 11:21:39.000000 dwd_global_radiation-1.0.0rc4/dwd_global_radiation.egg-info/SOURCES.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)        1 2024-05-17 11:21:39.000000 dwd_global_radiation-1.0.0rc4/dwd_global_radiation.egg-info/dependency_links.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)      128 2024-05-17 11:21:39.000000 dwd_global_radiation-1.0.0rc4/dwd_global_radiation.egg-info/requires.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       21 2024-05-17 11:21:39.000000 dwd_global_radiation-1.0.0rc4/dwd_global_radiation.egg-info/top_level.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       38 2024-05-17 11:21:39.906342 dwd_global_radiation-1.0.0rc4/setup.cfg
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1656 2024-05-17 10:43:19.000000 dwd_global_radiation-1.0.0rc4/setup.py
```

### Comparing `dwd_global_radiation-1.0.0rc3/LICENSE` & `dwd_global_radiation-1.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.0.0rc3/PKG-INFO` & `dwd_global_radiation-1.0.0rc4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: dwd_global_radiation
-Version: 1.0.0rc3
-Summary: Access and analyze DWD global radiation data and forecasts
-Home-page: https://github.com/aschmere/dwd_global_radiation
-Author: Arno Schmerer
-License: MIT
-Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development :: Libraries
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: beautifulsoup4>=4.12.3
-Requires-Dist: netCDF4>=1.6.5
-Requires-Dist: numpy>=1.26.4
-Requires-Dist: pytz>=2024.1
-Requires-Dist: Requests>=2.31.0
-Requires-Dist: tabulate>=0.9.0
-Requires-Dist: tzlocal>=5.2
-Requires-Dist: xarray>=2024.3.0
-
 DISCLAIMER: This project is a private open source project and is not affiliated with the German public meteorology service institute "Deutscher Wetterdienst" (DWD). However, it uses its publicly available data interfaces. 
 
 # Summary
 The DWD Global Radiation Observation and Forecast Data Library is a python package, which provides convenient access to forecast and observation data regarding Surface Incoming Solar Radiation (SIS) [[1]](#R1) or also known as "Global Horizontal Irradiance" (GHI) issued by the German meteorology service institute "Deutscher Wetterdienst" (DWD). The data currently used by this package covers roughly a geographical area of Germany, Austria and Switzerland. SIS or GHI is the most important input variable for determining the electrical output of photovoltaic systems. Therefore this data is particularly useful in "Smart Home"-scenarios, if you want to correlate the actual output of your photovoltaic system with measured SIS or can even help forecasting this output based on SIS forecast data. SIS data can also be helpful in regulating room heating systems, as solar irradiance can have a big impact on the room temperature as well.
 
 
 For more details regarding Solar irradiance terminology and the global radiation data provided by DWD via its "Open Data" server, see [[2]](#R2).
@@ -51,15 +25,38 @@
 tzlocal==5.2
 xarray==2024.3.0
 ```
 <ins>Note:</ins>The above listed versions of dependant Python packages reflect the versions, on which this package was developed and tested. Typically you would expect, that later versions of these packages will be compatible as well. Earlier versions might also be compatible. The Python version, with which this package
 was developed and tested, is 3.12.3.
 
 The workstation, on which you use Python along with this package, needs internet access, specifically via https protocol to the Open Data server of the DWD [[5]](#R5) in order to retrieve global radiation forecasts and observations.
+# Fast Track
+
+For those, who are quite familiar with Python programming and want to get a real jump start into the most essential parts of this Python package, there is a core workflow without much explanation
+listed below, which can just be executed in an interactive Python console after installation of the package.
+```
+# Import the module
+import dwd_global_radiation as dgr
 
+# Instantiate main object
+objGlobalRadiation=dgr.GlobalRadiation()
+
+# Add location
+objGlobalRadiation.add_location(name="My Home Location", latitude=52.5200, longitude=13.4050)
+
+# Fetch Measurements from DWD
+objGlobalRadiation.fetch_measurements()
+
+# Fetch Forecasts from DWD
+objGlobalRadiation.fetch_forecasts()
+
+# Print Data
+objGlobalRadiation.print_data()
+```
+This will provide a sample output as it is described similarly in chapter "Print Service" further below on this page.
 # Usage
 
 ## Import the Module
 ```
 import dwd_global_radiation as dgr
 ```
 
@@ -260,15 +257,15 @@
         | 2024-05-16 04:00:00 |          0          |
         +---------------------+---------------------+
         | 2024-05-16 05:00:00 |          0.0170898  |
         +---------------------+---------------------+
         | 2024-05-16 06:00:00 |         18.5645     |
         +---------------------+---------------------+
 ```
-
+--
 # References
 <a href="https://www.cmsaf.eu/SharedDocs/Literatur/document/2023/saf_cm_dwd_pum_meteosat_hel_sarah_3_3_pdf" id="R1">[1] Product User Manual Meteosat Solar Surface Radiation and Effective Cloud Albedo Climate Data Records SARAH-3<br>
 <a href="https://www.dwd.de/DE/leistungen/fernerkund_globalstrahlung_sis/fernerkund_globalstrahlung_sis.html" id="R2">[2] DWD - Product Description on Global Radiation<br>
 <a href="https://en.wikipedia.org/wiki/Solar_irradiance" id="R3">[3] Wikipedia - Solar Irradiance: <br>
 <a href="https://docs.python.org/3/library/venv.html" id="R4">[4] Python Documentation - venv — Creation of virtual environments<br>
 <a href="https://opendata.dwd.de/weather/satellite/radiation/" id="R5">[5] Global Radiation Forecast and Observation Data on the Open Data server of the DWD<br>
 <a href="https://www.dwd.de/EN/ourservices/solarenergy/satellite_solarradiation.html" id="R6">[6] DWD - Satellite-based retrieval of surface solar radiation<br>
```

### Comparing `dwd_global_radiation-1.0.0rc3/README.md` & `dwd_global_radiation-1.0.0rc4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: dwd_global_radiation
+Version: 1.0.0rc4
+Summary: Access and analyze DWD global radiation data and forecasts
+Home-page: https://github.com/aschmere/dwd_global_radiation
+Author: Arno Schmerer
+License: MIT
+Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: beautifulsoup4>=4.12.3
+Requires-Dist: netCDF4>=1.6.5
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: pytz>=2024.1
+Requires-Dist: Requests>=2.31.0
+Requires-Dist: tabulate>=0.9.0
+Requires-Dist: tzlocal>=5.2
+Requires-Dist: xarray>=2024.3.0
+
 DISCLAIMER: This project is a private open source project and is not affiliated with the German public meteorology service institute "Deutscher Wetterdienst" (DWD). However, it uses its publicly available data interfaces. 
 
 # Summary
 The DWD Global Radiation Observation and Forecast Data Library is a python package, which provides convenient access to forecast and observation data regarding Surface Incoming Solar Radiation (SIS) [[1]](#R1) or also known as "Global Horizontal Irradiance" (GHI) issued by the German meteorology service institute "Deutscher Wetterdienst" (DWD). The data currently used by this package covers roughly a geographical area of Germany, Austria and Switzerland. SIS or GHI is the most important input variable for determining the electrical output of photovoltaic systems. Therefore this data is particularly useful in "Smart Home"-scenarios, if you want to correlate the actual output of your photovoltaic system with measured SIS or can even help forecasting this output based on SIS forecast data. SIS data can also be helpful in regulating room heating systems, as solar irradiance can have a big impact on the room temperature as well.
 
 
 For more details regarding Solar irradiance terminology and the global radiation data provided by DWD via its "Open Data" server, see [[2]](#R2).
@@ -25,15 +51,38 @@
 tzlocal==5.2
 xarray==2024.3.0
 ```
 <ins>Note:</ins>The above listed versions of dependant Python packages reflect the versions, on which this package was developed and tested. Typically you would expect, that later versions of these packages will be compatible as well. Earlier versions might also be compatible. The Python version, with which this package
 was developed and tested, is 3.12.3.
 
 The workstation, on which you use Python along with this package, needs internet access, specifically via https protocol to the Open Data server of the DWD [[5]](#R5) in order to retrieve global radiation forecasts and observations.
+# Fast Track
+
+For those, who are quite familiar with Python programming and want to get a real jump start into the most essential parts of this Python package, there is a core workflow without much explanation
+listed below, which can just be executed in an interactive Python console after installation of the package.
+```
+# Import the module
+import dwd_global_radiation as dgr
 
+# Instantiate main object
+objGlobalRadiation=dgr.GlobalRadiation()
+
+# Add location
+objGlobalRadiation.add_location(name="My Home Location", latitude=52.5200, longitude=13.4050)
+
+# Fetch Measurements from DWD
+objGlobalRadiation.fetch_measurements()
+
+# Fetch Forecasts from DWD
+objGlobalRadiation.fetch_forecasts()
+
+# Print Data
+objGlobalRadiation.print_data()
+```
+This will provide a sample output as it is described similarly in chapter "Print Service" further below on this page.
 # Usage
 
 ## Import the Module
 ```
 import dwd_global_radiation as dgr
 ```
 
@@ -234,15 +283,15 @@
         | 2024-05-16 04:00:00 |          0          |
         +---------------------+---------------------+
         | 2024-05-16 05:00:00 |          0.0170898  |
         +---------------------+---------------------+
         | 2024-05-16 06:00:00 |         18.5645     |
         +---------------------+---------------------+
 ```
-
+--
 # References
 <a href="https://www.cmsaf.eu/SharedDocs/Literatur/document/2023/saf_cm_dwd_pum_meteosat_hel_sarah_3_3_pdf" id="R1">[1] Product User Manual Meteosat Solar Surface Radiation and Effective Cloud Albedo Climate Data Records SARAH-3<br>
 <a href="https://www.dwd.de/DE/leistungen/fernerkund_globalstrahlung_sis/fernerkund_globalstrahlung_sis.html" id="R2">[2] DWD - Product Description on Global Radiation<br>
 <a href="https://en.wikipedia.org/wiki/Solar_irradiance" id="R3">[3] Wikipedia - Solar Irradiance: <br>
 <a href="https://docs.python.org/3/library/venv.html" id="R4">[4] Python Documentation - venv — Creation of virtual environments<br>
 <a href="https://opendata.dwd.de/weather/satellite/radiation/" id="R5">[5] Global Radiation Forecast and Observation Data on the Open Data server of the DWD<br>
 <a href="https://www.dwd.de/EN/ourservices/solarenergy/satellite_solarradiation.html" id="R6">[6] DWD - Satellite-based retrieval of surface solar radiation<br>
```

### Comparing `dwd_global_radiation-1.0.0rc3/dwd_global_radiation/global_radiation.py` & `dwd_global_radiation-1.0.0rc4/dwd_global_radiation/global_radiation.py`

 * *Files 4% similar despite different names*

```diff
@@ -371,32 +371,48 @@
         ndlats = all_grid_global_rad_data.variables["lat"][:].filled()
         ndlons = all_grid_global_rad_data.variables["lon"][:].filled()
         long_grid, lat_grid = np.meshgrid(ndlons, ndlats)
         coordinates = np.dstack((lat_grid, long_grid)).reshape(-1, 2)
         return all_grid_global_rad_data, coordinates
 
     def _get_nearest_grid_point(self, latitude, longitude, grid_data):
-        all_grid_global_rad_data, coordinates = grid_data
-        distances = utils.haversine(
-            latitude, longitude, coordinates[:, 0], coordinates[:, 1]
-        )
+        all_grid_global_rad_data, _ = grid_data
+
+        # Calculate approximate indices based on the grid resolution of 0.05
+        lat_res = 0.05
+        lon_res = 0.05
+
+        lat_min = np.floor(latitude / lat_res) * lat_res
+        lon_min = np.floor(longitude / lon_res) * lon_res
+
+        # Four closest grid points to check
+        candidate_points = [
+            (lat_min, lon_min),
+            (lat_min, lon_min + lon_res),
+            (lat_min + lat_res, lon_min),
+            (lat_min + lat_res, lon_min + lon_res)
+        ]
+
+        # Compute distances for the four candidate points
+        distances = [
+            utils.haversine(latitude, longitude, lat, lon)
+            for lat, lon in candidate_points
+        ]
+
         nearest_index = np.argmin(distances)
         nearest_distance = round(distances[nearest_index], 3)
+        grid_latitude, grid_longitude = candidate_points[nearest_index]
 
-        lat_index = nearest_index // all_grid_global_rad_data.variables["lat"].shape[0]
-        lon_index = nearest_index % all_grid_global_rad_data.variables["lat"].shape[0]
-
-        grid_latitude = round(
-            all_grid_global_rad_data.variables["lat"][:][lat_index], 2
-        )
-        grid_longitude = round(
-            all_grid_global_rad_data.variables["lon"][:][lon_index], 2
-        )
+        # Find the nearest index in the grid data
+        lat_var = all_grid_global_rad_data.variables["lat"][:]
+        lon_var = all_grid_global_rad_data.variables["lon"][:]
+        lat_index = np.argmin(np.abs(lat_var - grid_latitude))
+        lon_index = np.argmin(np.abs(lon_var - grid_longitude))
 
-        return nearest_index, nearest_distance, grid_latitude, grid_longitude
+        return (lat_index * len(lon_var) + lon_index), nearest_distance, round(grid_latitude, 2), round(grid_longitude, 2)
 
     def _get_measurement_value_from_loaded_data(
         self, all_grid_global_rad_data, nearest_index
     ):
         lat_index = nearest_index // all_grid_global_rad_data.variables["lat"].shape[0]
         lon_index = nearest_index % all_grid_global_rad_data.variables["lat"].shape[0]
         measurement_value = all_grid_global_rad_data.variables["SIS"][:][
```

### Comparing `dwd_global_radiation-1.0.0rc3/dwd_global_radiation/utils.py` & `dwd_global_radiation-1.0.0rc4/dwd_global_radiation/utils.py`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.0.0rc3/dwd_global_radiation.egg-info/PKG-INFO` & `dwd_global_radiation-1.0.0rc4/dwd_global_radiation.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwd_global_radiation
-Version: 1.0.0rc3
+Version: 1.0.0rc4
 Summary: Access and analyze DWD global radiation data and forecasts
 Home-page: https://github.com/aschmere/dwd_global_radiation
 Author: Arno Schmerer
 License: MIT
 Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -51,15 +51,38 @@
 tzlocal==5.2
 xarray==2024.3.0
 ```
 <ins>Note:</ins>The above listed versions of dependant Python packages reflect the versions, on which this package was developed and tested. Typically you would expect, that later versions of these packages will be compatible as well. Earlier versions might also be compatible. The Python version, with which this package
 was developed and tested, is 3.12.3.
 
 The workstation, on which you use Python along with this package, needs internet access, specifically via https protocol to the Open Data server of the DWD [[5]](#R5) in order to retrieve global radiation forecasts and observations.
+# Fast Track
 
+For those, who are quite familiar with Python programming and want to get a real jump start into the most essential parts of this Python package, there is a core workflow without much explanation
+listed below, which can just be executed in an interactive Python console after installation of the package.
+```
+# Import the module
+import dwd_global_radiation as dgr
+
+# Instantiate main object
+objGlobalRadiation=dgr.GlobalRadiation()
+
+# Add location
+objGlobalRadiation.add_location(name="My Home Location", latitude=52.5200, longitude=13.4050)
+
+# Fetch Measurements from DWD
+objGlobalRadiation.fetch_measurements()
+
+# Fetch Forecasts from DWD
+objGlobalRadiation.fetch_forecasts()
+
+# Print Data
+objGlobalRadiation.print_data()
+```
+This will provide a sample output as it is described similarly in chapter "Print Service" further below on this page.
 # Usage
 
 ## Import the Module
 ```
 import dwd_global_radiation as dgr
 ```
 
@@ -260,15 +283,15 @@
         | 2024-05-16 04:00:00 |          0          |
         +---------------------+---------------------+
         | 2024-05-16 05:00:00 |          0.0170898  |
         +---------------------+---------------------+
         | 2024-05-16 06:00:00 |         18.5645     |
         +---------------------+---------------------+
 ```
-
+--
 # References
 <a href="https://www.cmsaf.eu/SharedDocs/Literatur/document/2023/saf_cm_dwd_pum_meteosat_hel_sarah_3_3_pdf" id="R1">[1] Product User Manual Meteosat Solar Surface Radiation and Effective Cloud Albedo Climate Data Records SARAH-3<br>
 <a href="https://www.dwd.de/DE/leistungen/fernerkund_globalstrahlung_sis/fernerkund_globalstrahlung_sis.html" id="R2">[2] DWD - Product Description on Global Radiation<br>
 <a href="https://en.wikipedia.org/wiki/Solar_irradiance" id="R3">[3] Wikipedia - Solar Irradiance: <br>
 <a href="https://docs.python.org/3/library/venv.html" id="R4">[4] Python Documentation - venv — Creation of virtual environments<br>
 <a href="https://opendata.dwd.de/weather/satellite/radiation/" id="R5">[5] Global Radiation Forecast and Observation Data on the Open Data server of the DWD<br>
 <a href="https://www.dwd.de/EN/ourservices/solarenergy/satellite_solarradiation.html" id="R6">[6] DWD - Satellite-based retrieval of surface solar radiation<br>
```

### Comparing `dwd_global_radiation-1.0.0rc3/setup.py` & `dwd_global_radiation-1.0.0rc4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='dwd_global_radiation',
-    version='1.0.0rc3',
+    version='1.0.0rc4',
     packages=find_packages(),
     description='Access and analyze DWD global radiation data and forecasts',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/aschmere/dwd_global_radiation',
     author='Arno Schmerer',
     license='MIT',
```

