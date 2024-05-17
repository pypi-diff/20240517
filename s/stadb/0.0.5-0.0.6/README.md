# Comparing `tmp/stadb-0.0.5.tar.gz` & `tmp/stadb-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stadb-0.0.5.tar", last modified: Wed Apr 24 13:07:51 2024, max compression
+gzip compressed data, was "stadb-0.0.6.tar", last modified: Fri May 17 07:47:19 2024, max compression
```

## Comparing `stadb-0.0.5.tar` & `stadb-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-24 13:07:51.901108 stadb-0.0.5/
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     1069 2024-04-04 09:35:28.000000 stadb-0.0.5/LICENSE
--rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-04-24 13:07:51.901108 stadb-0.0.5/PKG-INFO
--rw-rw-r--   0 enoc      (1000) enoc      (1000)      565 2024-04-24 13:07:47.000000 stadb-0.0.5/README.md
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     2281 2024-04-24 13:07:47.000000 stadb-0.0.5/pyproject.toml
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       38 2024-04-24 13:07:51.901108 stadb-0.0.5/setup.cfg
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-24 13:07:51.897108 stadb-0.0.5/src/
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-24 13:07:51.901108 stadb-0.0.5/src/stadb/
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       43 2024-04-04 10:50:06.000000 stadb-0.0.5/src/stadb/__init__.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     1262 2024-04-04 11:35:04.000000 stadb-0.0.5/src/stadb/logger.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     5895 2024-04-04 14:18:57.000000 stadb-0.0.5/src/stadb/postgresql.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)    42168 2024-04-24 13:07:19.000000 stadb-0.0.5/src/stadb/sensorthings.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)    12469 2024-04-04 12:39:51.000000 stadb-0.0.5/src/stadb/timescaledb.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     4356 2024-04-04 11:29:48.000000 stadb-0.0.5/src/stadb/utils.py
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-24 13:07:51.901108 stadb-0.0.5/src/stadb.egg-info/
--rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-04-24 13:07:51.000000 stadb-0.0.5/src/stadb.egg-info/PKG-INFO
--rw-rw-r--   0 enoc      (1000) enoc      (1000)      344 2024-04-24 13:07:51.000000 stadb-0.0.5/src/stadb.egg-info/SOURCES.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)        1 2024-04-24 13:07:51.000000 stadb-0.0.5/src/stadb.egg-info/dependency_links.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       50 2024-04-24 13:07:51.000000 stadb-0.0.5/src/stadb.egg-info/requires.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       11 2024-04-24 13:07:51.000000 stadb-0.0.5/src/stadb.egg-info/top_level.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)      234 2024-04-04 10:49:56.000000 stadb-0.0.5/src/test.py
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-05-17 07:47:19.031623 stadb-0.0.6/
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     1069 2024-04-04 09:35:28.000000 stadb-0.0.6/LICENSE
+-rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-05-17 07:47:19.031623 stadb-0.0.6/PKG-INFO
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)      565 2024-05-17 07:41:36.000000 stadb-0.0.6/README.md
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     2281 2024-05-17 07:41:36.000000 stadb-0.0.6/pyproject.toml
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       38 2024-05-17 07:47:19.031623 stadb-0.0.6/setup.cfg
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-05-17 07:47:19.027623 stadb-0.0.6/src/
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-05-17 07:47:19.031623 stadb-0.0.6/src/stadb/
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       43 2024-04-04 10:50:06.000000 stadb-0.0.6/src/stadb/__init__.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     1262 2024-04-04 11:35:04.000000 stadb-0.0.6/src/stadb/logger.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     5895 2024-04-04 14:18:57.000000 stadb-0.0.6/src/stadb/postgresql.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)    42138 2024-04-25 06:45:45.000000 stadb-0.0.6/src/stadb/sensorthings.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)    12469 2024-04-04 12:39:51.000000 stadb-0.0.6/src/stadb/timescaledb.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     4356 2024-04-04 11:29:48.000000 stadb-0.0.6/src/stadb/utils.py
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-05-17 07:47:19.031623 stadb-0.0.6/src/stadb.egg-info/
+-rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-05-17 07:47:19.000000 stadb-0.0.6/src/stadb.egg-info/PKG-INFO
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)      344 2024-05-17 07:47:19.000000 stadb-0.0.6/src/stadb.egg-info/SOURCES.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)        1 2024-05-17 07:47:19.000000 stadb-0.0.6/src/stadb.egg-info/dependency_links.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       50 2024-05-17 07:47:19.000000 stadb-0.0.6/src/stadb.egg-info/requires.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       11 2024-05-17 07:47:19.000000 stadb-0.0.6/src/stadb.egg-info/top_level.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)      234 2024-04-04 10:49:56.000000 stadb-0.0.6/src/test.py
```

### Comparing `stadb-0.0.5/LICENSE` & `stadb-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stadb-0.0.5/PKG-INFO` & `stadb-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadb
-Version: 0.0.5
+Version: 0.0.6
 Summary: SensorThings API database connector for advanced functionalities
 Author-email: Enoc Martínez <enoc.martinez@upc.edu>
 Maintainer-email: Enoc Martínez <enoc.martinez@upc.edu>
 License: MIT License
         
         Copyright (c) 2024 EnocMartinez
         
@@ -51,10 +51,10 @@
 Database connector for SensorThings API database for advanced interaction. It is based on [FROST-Server](https://github.com/FraunhoferIOSB/FROST-Server) implementation.
 
 It also adds specific support for time-series data by extending the database with [TimescaleDB](https://www.timescale.com/), which allows for faster queries and optimized storage. 
 
 ### Contact info ###
 
 * **author**: Enoc Martínez  
-* **version**: 0.0.5
+* **version**: 0.0.6
 * **organization**: Universitat Politècnica de Catalunya (UPC)  
 * **contact**: enoc.martinez@upc.edu
```

### Comparing `stadb-0.0.5/README.md` & `stadb-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,10 +2,10 @@
 Database connector for SensorThings API database for advanced interaction. It is based on [FROST-Server](https://github.com/FraunhoferIOSB/FROST-Server) implementation.
 
 It also adds specific support for time-series data by extending the database with [TimescaleDB](https://www.timescale.com/), which allows for faster queries and optimized storage. 
 
 ### Contact info ###
 
 * **author**: Enoc Martínez  
-* **version**: 0.0.5
+* **version**: 0.0.6
 * **organization**: Universitat Politècnica de Catalunya (UPC)  
 * **contact**: enoc.martinez@upc.edu
```

### Comparing `stadb-0.0.5/pyproject.toml` & `stadb-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 
 
 [project]
 
 name = "stadb"  # REQUIRED, is the only field that cannot be marked as dynamic.
-version = "0.0.5"  # REQUIRED, although can be dynamic
+version = "0.0.6"  # REQUIRED, although can be dynamic
 description = "SensorThings API database connector for advanced functionalities"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["sta", "setuptools", "development", "sensorthings"]
 
 authors = [
```

### Comparing `stadb-0.0.5/src/stadb/logger.py` & `stadb-0.0.6/src/stadb/logger.py`

 * *Files identical despite different names*

### Comparing `stadb-0.0.5/src/stadb/postgresql.py` & `stadb-0.0.6/src/stadb/postgresql.py`

 * *Files identical despite different names*

### Comparing `stadb-0.0.5/src/stadb/sensorthings.py` & `stadb-0.0.6/src/stadb/sensorthings.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         :param port:
         :param db_name:
         :param db_user:
         :param db_password:
         :param logger:
         """
         PgDatabaseConnector.__init__(self, host, port, db_name, db_user, db_password, logger)
+        self.host = host
         LoggerSuperclass.__init__(self, logger, "STA DB")
         self.info("Initialize database connector...")
         self.__sensor_properties = {}
 
         if timescaledb:
             self.timescale = TimescaleDB(self, logger)
         else:
@@ -260,16 +261,15 @@
 
         return {key: value for key, value in response}
 
     def value_from_query(self, query, debug=False):
         """
         Run a single value from a query
         """
-        self.exec_query(query, debug=debug)
-        response = self.cursor.fetchall()
+        response = self.exec_query(query, debug=debug)
         try:
             r = response[0][0]
         except IndexError:
             raise LookupError("query produced no results")
         return r
 
     def inject_to_timeseries(self, df, datastreams, max_rows=100000, disable_triggers=False,
@@ -936,16 +936,15 @@
 
     def sql_copy_csv(self, filename, table="OBSERVATIONS", delimiter=","):
         """
         Execute a COPY query to copy from a local CSV file to a database
         :return:
         """
         query = "COPY public.\"%s\" FROM '%s' DELIMITER '%s' CSV HEADER;" % (table, filename, delimiter)
-        self.cursor.execute(query)
-        self.connection.commit()
+        self.exec_query(query, fetch=False)
 
     def get_last_observation_id(self):
         """
         Gets last observation in database
         :return:
         """
         query = "SELECT \"ID\" FROM public.\"OBSERVATIONS\" ORDER BY \"ID\" DESC LIMIT 1"
```

### Comparing `stadb-0.0.5/src/stadb/timescaledb.py` & `stadb-0.0.6/src/stadb/timescaledb.py`

 * *Files identical despite different names*

### Comparing `stadb-0.0.5/src/stadb/utils.py` & `stadb-0.0.6/src/stadb/utils.py`

 * *Files identical despite different names*

### Comparing `stadb-0.0.5/src/stadb.egg-info/PKG-INFO` & `stadb-0.0.6/src/stadb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadb
-Version: 0.0.5
+Version: 0.0.6
 Summary: SensorThings API database connector for advanced functionalities
 Author-email: Enoc Martínez <enoc.martinez@upc.edu>
 Maintainer-email: Enoc Martínez <enoc.martinez@upc.edu>
 License: MIT License
         
         Copyright (c) 2024 EnocMartinez
         
@@ -51,10 +51,10 @@
 Database connector for SensorThings API database for advanced interaction. It is based on [FROST-Server](https://github.com/FraunhoferIOSB/FROST-Server) implementation.
 
 It also adds specific support for time-series data by extending the database with [TimescaleDB](https://www.timescale.com/), which allows for faster queries and optimized storage. 
 
 ### Contact info ###
 
 * **author**: Enoc Martínez  
-* **version**: 0.0.5
+* **version**: 0.0.6
 * **organization**: Universitat Politècnica de Catalunya (UPC)  
 * **contact**: enoc.martinez@upc.edu
```

