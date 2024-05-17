# Comparing `tmp/traffic_anomaly-0.0.1.tar.gz` & `tmp/traffic_anomaly-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traffic_anomaly-0.0.1.tar", last modified: Wed May 15 05:11:34 2024, max compression
+gzip compressed data, was "traffic_anomaly-1.0.0.tar", last modified: Fri May 17 02:08:14 2024, max compression
```

## Comparing `traffic_anomaly-0.0.1.tar` & `traffic_anomaly-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 05:11:34.186524 traffic_anomaly-0.0.1/
--rw-rw-rw-   0        0        0     1092 2024-04-11 00:30:22.000000 traffic_anomaly-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       52 2024-05-15 04:24:59.000000 traffic_anomaly-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3608 2024-05-15 05:11:34.155272 traffic_anomaly-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3041 2024-05-15 04:56:30.000000 traffic_anomaly-0.0.1/README.md
--rw-rw-rw-   0        0        0      664 2024-05-15 05:11:02.000000 traffic_anomaly-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 05:11:34.233413 traffic_anomaly-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-15 05:11:33.342136 traffic_anomaly-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 05:11:33.639653 traffic_anomaly-0.0.1/src/traffic_anomaly/
--rw-rw-rw-   0        0        0      185 2024-05-15 05:06:41.000000 traffic_anomaly-0.0.1/src/traffic_anomaly/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 05:11:34.045901 traffic_anomaly-0.0.1/src/traffic_anomaly/data/
--rw-rw-rw-   0        0        0    19871 2024-05-13 15:05:18.000000 traffic_anomaly-0.0.1/src/traffic_anomaly/data/sample_data.parquet
--rw-rw-rw-   0        0        0     2303 2024-05-14 21:14:06.000000 traffic_anomaly-0.0.1/src/traffic_anomaly/data/sample_data_groups.parquet
--rw-rw-rw-   0        0        0     3059 2024-05-15 03:46:19.000000 traffic_anomaly-0.0.1/src/traffic_anomaly/decompose.py
--rw-rw-rw-   0        0        0     2873 2024-05-15 03:47:26.000000 traffic_anomaly-0.0.1/src/traffic_anomaly/find_anomaly.py
--rw-rw-rw-   0        0        0      488 2024-05-15 03:02:39.000000 traffic_anomaly-0.0.1/src/traffic_anomaly/sample_data.py
-drwxrwxrwx   0        0        0        0 2024-05-15 05:11:34.124026 traffic_anomaly-0.0.1/src/traffic_anomaly.egg-info/
--rw-rw-rw-   0        0        0     3608 2024-05-15 05:11:33.000000 traffic_anomaly-0.0.1/src/traffic_anomaly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2024-05-15 05:11:33.000000 traffic_anomaly-0.0.1/src/traffic_anomaly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 05:11:33.000000 traffic_anomaly-0.0.1/src/traffic_anomaly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-15 05:11:33.000000 traffic_anomaly-0.0.1/src/traffic_anomaly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-15 05:11:33.000000 traffic_anomaly-0.0.1/src/traffic_anomaly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 02:08:13.176056 traffic_anomaly-1.0.0/
+-rw-rw-rw-   0        0        0     1092 2024-04-11 00:30:22.000000 traffic_anomaly-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0       52 2024-05-15 04:24:59.000000 traffic_anomaly-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3616 2024-05-17 02:08:11.738438 traffic_anomaly-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3041 2024-05-15 04:56:30.000000 traffic_anomaly-1.0.0/README.md
+-rw-rw-rw-   0        0        0      672 2024-05-17 02:02:42.000000 traffic_anomaly-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 02:08:14.269797 traffic_anomaly-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 02:07:35.626978 traffic_anomaly-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 02:07:51.798754 traffic_anomaly-1.0.0/src/traffic_anomaly/
+-rw-rw-rw-   0        0        0      185 2024-05-17 00:42:38.000000 traffic_anomaly-1.0.0/src/traffic_anomaly/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 02:08:06.847263 traffic_anomaly-1.0.0/src/traffic_anomaly/data/
+-rw-rw-rw-   0        0        0   146103 2024-05-17 00:34:07.000000 traffic_anomaly-1.0.0/src/traffic_anomaly/data/sample_counts.parquet
+-rw-rw-rw-   0        0        0    26167 2024-05-17 00:39:49.000000 traffic_anomaly-1.0.0/src/traffic_anomaly/data/sample_travel_times.parquet
+-rw-rw-rw-   0        0        0     6184 2024-05-17 01:20:13.000000 traffic_anomaly-1.0.0/src/traffic_anomaly/decompose.py
+-rw-rw-rw-   0        0        0     6531 2024-05-17 01:25:38.000000 traffic_anomaly-1.0.0/src/traffic_anomaly/find_anomaly.py
+-rw-rw-rw-   0        0        0      507 2024-05-17 00:41:03.000000 traffic_anomaly-1.0.0/src/traffic_anomaly/sample_data.py
+drwxrwxrwx   0        0        0        0 2024-05-17 02:08:09.535074 traffic_anomaly-1.0.0/src/traffic_anomaly.egg-info/
+-rw-rw-rw-   0        0        0     3616 2024-05-17 02:07:23.000000 traffic_anomaly-1.0.0/src/traffic_anomaly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      494 2024-05-17 02:07:31.000000 traffic_anomaly-1.0.0/src/traffic_anomaly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 02:07:27.000000 traffic_anomaly-1.0.0/src/traffic_anomaly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-17 02:07:28.000000 traffic_anomaly-1.0.0/src/traffic_anomaly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-17 02:07:28.000000 traffic_anomaly-1.0.0/src/traffic_anomaly.egg-info/top_level.txt
```

### Comparing `traffic_anomaly-0.0.1/LICENSE` & `traffic_anomaly-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `traffic_anomaly-0.0.1/PKG-INFO` & `traffic_anomaly-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: traffic_anomaly
-Version: 0.0.1
+Version: 1.0.0
 Summary: Robust decomposition and anomaly detection on multiple time series for any SQL backend. Designed for traffic data.
 Author-email: Shawn Strasser <shawn.strasser@odot.oregon.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: duckdb<0.10.2,>=0.9.1
-Requires-Dist: ibis-framework==9.0.0
+Requires-Dist: ibis-framework<=9.0.0,>=8.0.0
 
 # Traffic Anomaly
 
 `traffic_anomaly` is a production ready Python package for robust decomposition and anomaly detection on multiple time series at once. It uses Ibis to integrate with any SQL backend in a production pipeline, or run locally with the included DuckDB backend.
 
 Designed for real world messy traffic data (volumes, travel times), `traffic_anomaly` uses medians to decompose time series into trend, daily, weekly, and residual components. Anomalies are then classified, and Median Absolute Deviation may be used for further robustness. Missing data are handled, and time periods without sufficient data can be thrown out. Check out `example.ipynb` in this repository for a demo.
```

### Comparing `traffic_anomaly-0.0.1/README.md` & `traffic_anomaly-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `traffic_anomaly-0.0.1/pyproject.toml` & `traffic_anomaly-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "traffic_anomaly"
-version = "0.0.1"
+version = "1.0.0"
 authors = [
   { name="Shawn Strasser", email="shawn.strasser@odot.oregon.gov" },
 ]
 description = "Robust decomposition and anomaly detection on multiple time series for any SQL backend. Designed for traffic data."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "duckdb>=0.9.1,<0.10.2",
-    "ibis-framework==9.0.0",
+    "ibis-framework>=8.0.0,<=9.0.0",
 ]
 
 [tools.setuptools]
 include_package_data = true
 package_data = {"traffic_anomaly" = ["data/*"]}
```

### Comparing `traffic_anomaly-0.0.1/src/traffic_anomaly.egg-info/PKG-INFO` & `traffic_anomaly-1.0.0/src/traffic_anomaly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: traffic_anomaly
-Version: 0.0.1
+Version: 1.0.0
 Summary: Robust decomposition and anomaly detection on multiple time series for any SQL backend. Designed for traffic data.
 Author-email: Shawn Strasser <shawn.strasser@odot.oregon.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: duckdb<0.10.2,>=0.9.1
-Requires-Dist: ibis-framework==9.0.0
+Requires-Dist: ibis-framework<=9.0.0,>=8.0.0
 
 # Traffic Anomaly
 
 `traffic_anomaly` is a production ready Python package for robust decomposition and anomaly detection on multiple time series at once. It uses Ibis to integrate with any SQL backend in a production pipeline, or run locally with the included DuckDB backend.
 
 Designed for real world messy traffic data (volumes, travel times), `traffic_anomaly` uses medians to decompose time series into trend, daily, weekly, and residual components. Anomalies are then classified, and Median Absolute Deviation may be used for further robustness. Missing data are handled, and time periods without sufficient data can be thrown out. Check out `example.ipynb` in this repository for a demo.
```

