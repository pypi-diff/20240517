# Comparing `tmp/peaka-1.0.1.tar.gz` & `tmp/peaka-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peaka-1.0.1.tar", last modified: Tue Apr 16 15:03:03 2024, max compression
+gzip compressed data, was "peaka-1.1.0.tar", last modified: Fri May 17 11:48:27 2024, max compression
```

## Comparing `peaka-1.0.1.tar` & `peaka-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ozanbatuhanceylan   (501) staff       (20)        0 2024-04-16 15:03:03.859570 peaka-1.0.1/
--rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)    11357 2024-04-05 11:37:15.000000 peaka-1.0.1/LICENSE
--rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)     3540 2024-04-16 15:03:03.859264 peaka-1.0.1/PKG-INFO
--rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)     2097 2024-04-16 14:48:13.000000 peaka-1.0.1/README.md
-drwxr-xr-x   0 ozanbatuhanceylan   (501) staff       (20)        0 2024-04-16 15:03:03.856552 peaka-1.0.1/peaka/
--rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)        0 2024-04-05 11:38:44.000000 peaka-1.0.1/peaka/__init__.py
--rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)     1002 2024-04-05 12:22:16.000000 peaka-1.0.1/peaka/dbapi.py
-drwxr-xr-x   0 ozanbatuhanceylan   (501) staff       (20)        0 2024-04-16 15:03:03.858096 peaka-1.0.1/peaka/sqlalchemy/
--rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)        0 2024-04-05 11:38:44.000000 peaka-1.0.1/peaka/sqlalchemy/__init__.py
--rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)     1153 2024-04-05 11:38:44.000000 peaka-1.0.1/peaka/sqlalchemy/dialect.py
-drwxr-xr-x   0 ozanbatuhanceylan   (501) staff       (20)        0 2024-04-16 15:03:03.858549 peaka-1.0.1/peaka.egg-info/
--rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)     3540 2024-04-16 15:03:03.000000 peaka-1.0.1/peaka.egg-info/PKG-INFO
--rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)      292 2024-04-16 15:03:03.000000 peaka-1.0.1/peaka.egg-info/SOURCES.txt
--rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)        1 2024-04-16 15:03:03.000000 peaka-1.0.1/peaka.egg-info/dependency_links.txt
--rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)       68 2024-04-16 15:03:03.000000 peaka-1.0.1/peaka.egg-info/entry_points.txt
--rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)       79 2024-04-16 15:03:03.000000 peaka-1.0.1/peaka.egg-info/requires.txt
--rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)        6 2024-04-16 15:03:03.000000 peaka-1.0.1/peaka.egg-info/top_level.txt
--rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)       38 2024-04-16 15:03:03.859629 peaka-1.0.1/setup.cfg
--rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)     4348 2024-04-16 15:02:07.000000 peaka-1.0.1/setup.py
+drwxr-xr-x   0 ozanbatuhanceylan   (501) staff       (20)        0 2024-05-17 11:48:27.640010 peaka-1.1.0/
+-rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)    11357 2024-04-05 11:37:15.000000 peaka-1.1.0/LICENSE
+-rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)     3570 2024-05-17 11:48:27.639646 peaka-1.1.0/PKG-INFO
+-rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)     2127 2024-05-17 11:47:27.000000 peaka-1.1.0/README.md
+drwxr-xr-x   0 ozanbatuhanceylan   (501) staff       (20)        0 2024-05-17 11:48:27.637081 peaka-1.1.0/peaka/
+-rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)        0 2024-04-05 11:38:44.000000 peaka-1.1.0/peaka/__init__.py
+-rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)     1149 2024-05-17 11:47:27.000000 peaka-1.1.0/peaka/dbapi.py
+drwxr-xr-x   0 ozanbatuhanceylan   (501) staff       (20)        0 2024-05-17 11:48:27.638395 peaka-1.1.0/peaka/sqlalchemy/
+-rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)        0 2024-04-05 11:38:44.000000 peaka-1.1.0/peaka/sqlalchemy/__init__.py
+-rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)     1153 2024-04-05 11:38:44.000000 peaka-1.1.0/peaka/sqlalchemy/dialect.py
+drwxr-xr-x   0 ozanbatuhanceylan   (501) staff       (20)        0 2024-05-17 11:48:27.638865 peaka-1.1.0/peaka.egg-info/
+-rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)     3570 2024-05-17 11:48:27.000000 peaka-1.1.0/peaka.egg-info/PKG-INFO
+-rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)      292 2024-05-17 11:48:27.000000 peaka-1.1.0/peaka.egg-info/SOURCES.txt
+-rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)        1 2024-05-17 11:48:27.000000 peaka-1.1.0/peaka.egg-info/dependency_links.txt
+-rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)       68 2024-05-17 11:48:27.000000 peaka-1.1.0/peaka.egg-info/entry_points.txt
+-rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)       79 2024-05-17 11:48:27.000000 peaka-1.1.0/peaka.egg-info/requires.txt
+-rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)        6 2024-05-17 11:48:27.000000 peaka-1.1.0/peaka.egg-info/top_level.txt
+-rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)       38 2024-05-17 11:48:27.640082 peaka-1.1.0/setup.cfg
+-rw-r--r--   0 ozanbatuhanceylan   (501) staff       (20)     4348 2024-05-17 11:47:27.000000 peaka-1.1.0/setup.py
```

### Comparing `peaka-1.0.1/LICENSE` & `peaka-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peaka-1.0.1/PKG-INFO` & `peaka-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peaka
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Python client for Peaka
 Home-page: https://docs.peaka.com/db-drivers/python
 Author: Peaka
 Author-email: integrations@peaka.com
 Keywords: data,peaka
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -51,20 +51,20 @@
 $ pip install peaka
 ```
 
 **Quick Start**
 
 Use the DBAPI interface to query Peaka:
 
-You can call the `connect_to_peaka` method with your Peaka `api_key`. `catalog`, `schema` and `timezone` are the optional parameters.
+You can call the `connect_to_peaka` method with your Peaka `api_key`. `catalog`, `schema`, `timezone` and `zone` are the optional parameters.
 
 ```python
 from peaka.dbapi import connect_to_peaka
 
-conn = connect_to_peaka(api_key="<YOUR_API_KEY>", catalog="<CATALOG_NAME>", schema="<SCHEMA_NAME>", timezone="<TIMEZONE>")
+conn = connect_to_peaka(api_key="<YOUR_API_KEY>", catalog="<CATALOG_NAME>", schema="<SCHEMA_NAME>", timezone="<TIMEZONE>", zone="<'eu' | 'us'>")
     
 cur = conn.cursor()
 cur.execute("SELECT * FROM <table_name>")
 rows = cur.fetchall()
 ```
 
 You can query your `table` directly, if you enter the `catalog` and `schema` when you connect.
```

### Comparing `peaka-1.0.1/README.md` & `peaka-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 $ pip install peaka
 ```
 
 **Quick Start**
 
 Use the DBAPI interface to query Peaka:
 
-You can call the `connect_to_peaka` method with your Peaka `api_key`. `catalog`, `schema` and `timezone` are the optional parameters.
+You can call the `connect_to_peaka` method with your Peaka `api_key`. `catalog`, `schema`, `timezone` and `zone` are the optional parameters.
 
 ```python
 from peaka.dbapi import connect_to_peaka
 
-conn = connect_to_peaka(api_key="<YOUR_API_KEY>", catalog="<CATALOG_NAME>", schema="<SCHEMA_NAME>", timezone="<TIMEZONE>")
+conn = connect_to_peaka(api_key="<YOUR_API_KEY>", catalog="<CATALOG_NAME>", schema="<SCHEMA_NAME>", timezone="<TIMEZONE>", zone="<'eu' | 'us'>")
     
 cur = conn.cursor()
 cur.execute("SELECT * FROM <table_name>")
 rows = cur.fetchall()
 ```
 
 You can query your `table` directly, if you enter the `catalog` and `schema` when you connect.
```

### Comparing `peaka-1.0.1/peaka/dbapi.py` & `peaka-1.1.0/peaka/dbapi.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 """Module providing a function that connecting to Peaka."""
 from trino.dbapi import connect
 
 
-def connect_to_peaka(api_key, catalog=None, schema=None, timezone=None):
+def connect_to_peaka(api_key, catalog=None, schema=None, timezone=None, zone="us"):
     """
     Function to connect to Peaka database.
 
     Args:
     - api_key (str): The API key required for authentication.
     - catalog (str): Optional. The catalog to connect to.
     - schema (str): Optional. The schema to connect to.
     - timezone (str): Optional. The timezone for the connection.
 
     Returns:
     - Connection object: Connection object to the Peaka database.
     """
+    # Define zone based host name
+    host = ""
+    if zone == "eu":
+        host = "dbc.eu.peaka.studio"
+    else:
+        host = "dbc.peaka.studio"
 
     # Setting up connection arguments
     args = {
-        "host": "dbc.peaka.studio",
+        "host": host,
         "port": 4567,
         "http_scheme": "HTTPS",
         "extra_credential": [("peakaKey", api_key)],
         "catalog": catalog,
         "schema": schema,
         "timezone": timezone
     }
```

### Comparing `peaka-1.0.1/peaka/sqlalchemy/dialect.py` & `peaka-1.1.0/peaka/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `peaka-1.0.1/peaka.egg-info/PKG-INFO` & `peaka-1.1.0/peaka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peaka
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Python client for Peaka
 Home-page: https://docs.peaka.com/db-drivers/python
 Author: Peaka
 Author-email: integrations@peaka.com
 Keywords: data,peaka
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -51,20 +51,20 @@
 $ pip install peaka
 ```
 
 **Quick Start**
 
 Use the DBAPI interface to query Peaka:
 
-You can call the `connect_to_peaka` method with your Peaka `api_key`. `catalog`, `schema` and `timezone` are the optional parameters.
+You can call the `connect_to_peaka` method with your Peaka `api_key`. `catalog`, `schema`, `timezone` and `zone` are the optional parameters.
 
 ```python
 from peaka.dbapi import connect_to_peaka
 
-conn = connect_to_peaka(api_key="<YOUR_API_KEY>", catalog="<CATALOG_NAME>", schema="<SCHEMA_NAME>", timezone="<TIMEZONE>")
+conn = connect_to_peaka(api_key="<YOUR_API_KEY>", catalog="<CATALOG_NAME>", schema="<SCHEMA_NAME>", timezone="<TIMEZONE>", zone="<'eu' | 'us'>")
     
 cur = conn.cursor()
 cur.execute("SELECT * FROM <table_name>")
 rows = cur.fetchall()
 ```
 
 You can query your `table` directly, if you enter the `catalog` and `schema` when you connect.
```

### Comparing `peaka-1.0.1/setup.py` & `peaka-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="peaka",
-    version="1.0.1",
+    version="1.1.0",
     description="A Python client for Peaka",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://docs.peaka.com/db-drivers/python",
     author="Peaka",
     author_email="integrations@peaka.com",
     # Classifiers help users find your project by categorizing it.
```

