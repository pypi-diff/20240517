# Comparing `tmp/dq_check-0.3.2.tar.gz` & `tmp/dq_check-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dq_check-0.3.2.tar", last modified: Thu May 16 03:48:34 2024, max compression
+gzip compressed data, was "dq_check-0.3.3.tar", last modified: Thu May 16 13:20:31 2024, max compression
```

## Comparing `dq_check-0.3.2.tar` & `dq_check-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-16 03:48:34.389885 dq_check-0.3.2/
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-16 03:48:34.389465 dq_check-0.3.2/PKG-INFO
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2440 2024-05-12 21:16:29.000000 dq_check-0.3.2/README.md
--rw-r--r--   0 rohan.goel   (502) staff       (20)      327 2024-05-16 03:47:54.000000 dq_check-0.3.2/pyproject.toml
--rw-r--r--   0 rohan.goel   (502) staff       (20)      131 2024-05-16 03:48:34.390942 dq_check-0.3.2/setup.cfg
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-16 03:48:34.381247 dq_check-0.3.2/src/
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-16 03:48:34.384051 dq_check-0.3.2/src/dq_check/
--rw-r--r--   0 rohan.goel   (502) staff       (20)       29 2024-05-05 04:45:50.000000 dq_check-0.3.2/src/dq_check/__init__.py
--rw-r--r--   0 rohan.goel   (502) staff       (20)    16289 2024-05-16 03:40:41.000000 dq_check-0.3.2/src/dq_check/dq_check.py
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-16 03:48:34.388420 dq_check-0.3.2/src/dq_check.egg-info/
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-16 03:48:34.000000 dq_check-0.3.2/src/dq_check.egg-info/PKG-INFO
--rw-r--r--   0 rohan.goel   (502) staff       (20)      263 2024-05-16 03:48:34.000000 dq_check-0.3.2/src/dq_check.egg-info/SOURCES.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)        1 2024-05-16 03:48:34.000000 dq_check-0.3.2/src/dq_check.egg-info/dependency_links.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)       15 2024-05-16 03:48:34.000000 dq_check-0.3.2/src/dq_check.egg-info/requires.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)        9 2024-05-16 03:48:34.000000 dq_check-0.3.2/src/dq_check.egg-info/top_level.txt
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-16 13:20:31.226602 dq_check-0.3.3/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-16 13:20:31.226255 dq_check-0.3.3/PKG-INFO
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2440 2024-05-12 21:16:29.000000 dq_check-0.3.3/README.md
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      327 2024-05-16 13:20:04.000000 dq_check-0.3.3/pyproject.toml
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      131 2024-05-16 13:20:31.227375 dq_check-0.3.3/setup.cfg
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-16 13:20:31.218479 dq_check-0.3.3/src/
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-16 13:20:31.221379 dq_check-0.3.3/src/dq_check/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)       29 2024-05-05 04:45:50.000000 dq_check-0.3.3/src/dq_check/__init__.py
+-rw-r--r--   0 rohan.goel   (502) staff       (20)    16294 2024-05-16 13:19:09.000000 dq_check-0.3.3/src/dq_check/dq_check.py
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-16 13:20:31.225587 dq_check-0.3.3/src/dq_check.egg-info/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-16 13:20:31.000000 dq_check-0.3.3/src/dq_check.egg-info/PKG-INFO
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      263 2024-05-16 13:20:31.000000 dq_check-0.3.3/src/dq_check.egg-info/SOURCES.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)        1 2024-05-16 13:20:31.000000 dq_check-0.3.3/src/dq_check.egg-info/dependency_links.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)       15 2024-05-16 13:20:31.000000 dq_check-0.3.3/src/dq_check.egg-info/requires.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)        9 2024-05-16 13:20:31.000000 dq_check-0.3.3/src/dq_check.egg-info/top_level.txt
```

### Comparing `dq_check-0.3.2/PKG-INFO` & `dq_check-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq_check
-Version: 0.3.2
+Version: 0.3.3
 Summary: A data quality check module for Spark
 Author-email: rohan goel <rohan.goel@databricks.com>
 Description-Content-Type: text/markdown
 Requires-Dist: pyspark
 Requires-Dist: pandas
 
 ## dq_check
```

### Comparing `dq_check-0.3.2/README.md` & `dq_check-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `dq_check-0.3.2/src/dq_check/dq_check.py` & `dq_check-0.3.3/src/dq_check/dq_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,30 +205,31 @@
             client = self.azure_sql_client
         else:
             print(F"Invalid table type. It should either be delta or asql")
 
         #create audit schema if not exists
         try:
             if audit_catalog:
-                client.read_sql(F'CREATE SCHEMA IF NOT EXISTS {audit_catalog}.{audit_schema}')
+                self.spark.sql(F'CREATE SCHEMA IF NOT EXISTS {audit_catalog}.{audit_schema}')
             else:
-                client.read_sql(F'CREATE SCHEMA IF NOT EXISTS {audit_schema}')
+                self.spark.sql(F'CREATE SCHEMA IF NOT EXISTS {audit_schema}')
         except Exception as e:
             raise Exception(F"User does not have create schema permission for audit table."
                             F"Please make sure audit table schema is available or user has permission to create it."
                             F"Please check error below {e}")
 
         
         #validate sql
 
         table_cols,sql_tables = self.parse_sql_query(sql_query)
 
-        # table validation
-        if table_name_only not in sql_query:
-            raise ValueError(f"table {table_name_only} not in sql from clause {sql_query}")
+        # table validation for sample data
+        if table_name not in sql_query:
+            raise ValueError(f"table {table_name} not in sql from clause {sql_query}")
+
         
         if '*' not in table_cols:
           #primary key validation
           if set(primary_keys) - set(table_cols):
                   if not agg_ind:
                       agg_without_pk_ind = 'n'
                       raise ValueError(f"primary key {primary_keys} not in sql select clause {table_cols}")
```

### Comparing `dq_check-0.3.2/src/dq_check.egg-info/PKG-INFO` & `dq_check-0.3.3/src/dq_check.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq_check
-Version: 0.3.2
+Version: 0.3.3
 Summary: A data quality check module for Spark
 Author-email: rohan goel <rohan.goel@databricks.com>
 Description-Content-Type: text/markdown
 Requires-Dist: pyspark
 Requires-Dist: pandas
 
 ## dq_check
```

