# Comparing `tmp/target-duckdb-0.6.0.tar.gz` & `tmp/target_duckdb-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target-duckdb-0.6.0.tar", last modified: Wed Jul 12 20:40:17 2023, max compression
+gzip compressed data, was "target_duckdb-0.7.0.tar", last modified: Fri May 17 13:18:46 2024, max compression
```

## Comparing `target-duckdb-0.6.0.tar` & `target_duckdb-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-07-12 20:40:17.973100 target-duckdb-0.6.0/
--rw-r--r--   0 jwills     (501) staff       (20)    10409 2022-12-17 04:32:30.000000 target-duckdb-0.6.0/LICENSE
--rw-r--r--   0 jwills     (501) staff       (20)     6313 2023-07-12 20:40:17.972989 target-duckdb-0.6.0/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)     5928 2023-07-12 14:08:00.000000 target-duckdb-0.6.0/README.md
--rw-r--r--   0 jwills     (501) staff       (20)       38 2023-07-12 20:40:17.973132 target-duckdb-0.6.0/setup.cfg
--rw-r--r--   0 jwills     (501) staff       (20)     1008 2023-07-11 20:26:39.000000 target-duckdb-0.6.0/setup.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-07-12 20:40:17.972137 target-duckdb-0.6.0/target_duckdb/
--rw-r--r--   0 jwills     (501) staff       (20)    15373 2023-07-12 14:08:05.000000 target-duckdb-0.6.0/target_duckdb/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)    23362 2023-07-12 14:08:05.000000 target-duckdb-0.6.0/target_duckdb/db_sync.py
--rw-r--r--   0 jwills     (501) staff       (20)      685 2023-01-24 22:42:31.000000 target-duckdb-0.6.0/target_duckdb/logger.py
--rw-r--r--   0 jwills     (501) staff       (20)      370 2022-12-17 04:32:30.000000 target-duckdb-0.6.0/target_duckdb/logging.conf
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-07-12 20:40:17.972842 target-duckdb-0.6.0/target_duckdb.egg-info/
--rw-r--r--   0 jwills     (501) staff       (20)     6313 2023-07-12 20:40:17.000000 target-duckdb-0.6.0/target_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)      352 2023-07-12 20:40:17.000000 target-duckdb-0.6.0/target_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 jwills     (501) staff       (20)        1 2023-07-12 20:40:17.000000 target-duckdb-0.6.0/target_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 jwills     (501) staff       (20)       53 2023-07-12 20:40:17.000000 target-duckdb-0.6.0/target_duckdb.egg-info/entry_points.txt
--rw-r--r--   0 jwills     (501) staff       (20)       65 2023-07-12 20:40:17.000000 target-duckdb-0.6.0/target_duckdb.egg-info/requires.txt
--rw-r--r--   0 jwills     (501) staff       (20)       14 2023-07-12 20:40:17.000000 target-duckdb-0.6.0/target_duckdb.egg-info/top_level.txt
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-05-17 13:18:46.913087 target_duckdb-0.7.0/
+-rw-r--r--   0 jwills     (501) staff       (20)    10409 2022-12-17 04:32:30.000000 target_duckdb-0.7.0/LICENSE
+-rw-r--r--   0 jwills     (501) staff       (20)     6497 2024-05-17 13:18:46.912906 target_duckdb-0.7.0/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)     5928 2023-07-31 18:20:19.000000 target_duckdb-0.7.0/README.md
+-rw-r--r--   0 jwills     (501) staff       (20)       38 2024-05-17 13:18:46.913122 target_duckdb-0.7.0/setup.cfg
+-rw-r--r--   0 jwills     (501) staff       (20)     1009 2024-05-17 02:55:17.000000 target_duckdb-0.7.0/setup.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-05-17 13:18:46.911757 target_duckdb-0.7.0/target_duckdb/
+-rw-r--r--   0 jwills     (501) staff       (20)    15373 2023-07-31 18:20:19.000000 target_duckdb-0.7.0/target_duckdb/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)    24088 2024-05-17 02:54:37.000000 target_duckdb-0.7.0/target_duckdb/db_sync.py
+-rw-r--r--   0 jwills     (501) staff       (20)      685 2023-01-24 22:42:31.000000 target_duckdb-0.7.0/target_duckdb/logger.py
+-rw-r--r--   0 jwills     (501) staff       (20)      370 2022-12-17 04:32:30.000000 target_duckdb-0.7.0/target_duckdb/logging.conf
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2024-05-17 13:18:46.912597 target_duckdb-0.7.0/target_duckdb.egg-info/
+-rw-r--r--   0 jwills     (501) staff       (20)     6497 2024-05-17 13:18:46.000000 target_duckdb-0.7.0/target_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)      352 2024-05-17 13:18:46.000000 target_duckdb-0.7.0/target_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        1 2024-05-17 13:18:46.000000 target_duckdb-0.7.0/target_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       53 2024-05-17 13:18:46.000000 target_duckdb-0.7.0/target_duckdb.egg-info/entry_points.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       66 2024-05-17 13:18:46.000000 target_duckdb-0.7.0/target_duckdb.egg-info/requires.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       14 2024-05-17 13:18:46.000000 target_duckdb-0.7.0/target_duckdb.egg-info/top_level.txt
```

### Comparing `target-duckdb-0.6.0/LICENSE` & `target_duckdb-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `target-duckdb-0.6.0/PKG-INFO` & `target_duckdb-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: target-duckdb
-Version: 0.6.0
+Version: 0.7.0
 Summary: Singer.io target for loading data into DuckDB
 Home-page: https://github.com/jwills/target-duckdb
 Author: Josh Wills
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: jsonschema>=3.2.0
+Requires-Dist: duckdb==0.10.2
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pylint; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 
 # target-duckdb
 
 [![License: Apache2](https://img.shields.io/badge/License-Apache2-yellow.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [Singer](https://www.singer.io/) target that loads data into DuckDB following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).
```

### Comparing `target-duckdb-0.6.0/README.md` & `target_duckdb-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `target-duckdb-0.6.0/setup.py` & `target_duckdb-0.7.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 from setuptools import setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="target-duckdb",
-    version="0.6.0",
+    version="0.7.0",
     description="Singer.io target for loading data into DuckDB",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh Wills",
     url="https://github.com/jwills/target-duckdb",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3 :: Only",
     ],
     py_modules=["target_duckdb"],
     install_requires=[
         "jsonschema>=3.2.0",
-        "duckdb>=0.7.0",
+        "duckdb==0.10.2",
     ],
     extras_require={
         "test": [
             "pytest",
             "pylint",
             "pytest-cov",
         ]
```

### Comparing `target-duckdb-0.6.0/target_duckdb/__init__.py` & `target_duckdb-0.7.0/target_duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `target-duckdb-0.6.0/target_duckdb/db_sync.py` & `target_duckdb-0.7.0/target_duckdb/db_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,17 +323,17 @@
         stream_dict = stream_name_to_dict(stream_name)
         table_name = stream_dict["table_name"]
         pg_table_name = table_name.replace(".", "_").replace("-", "_").lower()
 
         if without_schema:
             return f'"{pg_table_name.lower()}"'
         elif self.catalog_name:
-            return f'{self.catalog_name}.{self.schema_name}."{pg_table_name.lower()}"'
+            return f'"{self.catalog_name}"."{self.schema_name}"."{pg_table_name.lower()}"'
         else:
-            return f'{self.schema_name}."{pg_table_name.lower()}"'
+            return f'"{self.schema_name}"."{pg_table_name.lower()}"'
 
     def record_primary_key_string(self, record):
         if len(self.stream_schema_message["key_properties"]) == 0:
             return None
         flatten = flatten_record(
             record, self.flatten_schema, max_level=self.data_flattening_max_level
         )
@@ -380,15 +380,15 @@
                 f,
                 delimiter=self.delimiter,
                 quotechar=self.quotechar,
                 quoting=csv.QUOTE_MINIMAL,
             )
             for record in records:
                 csvwriter.writerow(self.record_to_flattened(record))
-        cur.execute("COPY {} FROM '{}'".format(temp_table, temp_file_csv))
+        cur.execute("COPY {} FROM '{}' WITH (new_line '\\r\\n')".format(temp_table, temp_file_csv))
 
         if len(self.stream_schema_message["key_properties"]) > 0:
             cur.execute(self.update_from_temp_table(temp_table))
         cur.execute(self.insert_from_temp_table(temp_table))
         cur.execute(f"DROP TABLE {temp_table}")
         os.unlink(temp_file_csv)
 
@@ -418,14 +418,18 @@
 
     def update_from_temp_table(self, temp_table):
         stream_schema_message = self.stream_schema_message
         primary_key_columns = set(primary_column_names(self.stream_schema_message))
         columns = [x for x in self.column_names() if x not in primary_key_columns]
         table = self.table_name(stream_schema_message["stream"])
 
+        if not columns:
+            # Nothing to do if all of the columns are PKs
+            return
+
         return """UPDATE {} as s SET {} FROM {} t
         WHERE {}
         """.format(
             table,
             ", ".join(["{}=t.{}".format(c, c) for c in columns]),
             temp_table,
             self.primary_key_condition("t"),
@@ -499,30 +503,45 @@
             table
         )
         self.logger.info("Deleting rows from '%s' table... %s", table, query)
         self.logger.info("DELETE %s", len(self.query(query)))
 
     def create_schema_if_not_exists(self, table_columns_cache=None):
         schema_name = self.schema_name
+        catalog_name = self.catalog_name
         schema_rows = 0
 
         # table_columns_cache is an optional pre-collected list of available objects in DuckDB
         if table_columns_cache:
             schema_rows = list(
                 filter(lambda x: x["TABLE_SCHEMA"] == schema_name, table_columns_cache)
             )
         # Query realtime if not pre-collected
+        elif catalog_name:
+            schema_rows = self.query(
+                "SELECT LOWER(schema_name) schema_name, LOWER(catalog_name) catalog_name "
+                "FROM information_schema.schemata "
+                "WHERE LOWER(schema_name) = ? AND LOWER(catalog_name) = ?",
+                (
+                    schema_name.lower(),
+                    catalog_name.lower(),
+                ),
+            )
         else:
             schema_rows = self.query(
                 "SELECT LOWER(schema_name) schema_name FROM information_schema.schemata WHERE LOWER(schema_name) = ?",
                 (schema_name.lower(),),
             )
 
         if len(schema_rows) == 0:
-            query = "CREATE SCHEMA IF NOT EXISTS {}".format(schema_name)
+            if catalog_name:
+                query = f'CREATE SCHEMA IF NOT EXISTS "{catalog_name}"."{schema_name}"'
+            else:
+                query = f'CREATE SCHEMA IF NOT EXISTS "{schema_name}"'
+
             self.logger.info(
                 "Schema '%s' does not exist. Creating... %s", schema_name, query
             )
             self.query(query)
 
     def get_tables(self):
         if self.catalog_name:
```

### Comparing `target-duckdb-0.6.0/target_duckdb/logger.py` & `target_duckdb-0.7.0/target_duckdb/logger.py`

 * *Files identical despite different names*

### Comparing `target-duckdb-0.6.0/target_duckdb.egg-info/PKG-INFO` & `target_duckdb-0.7.0/target_duckdb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: target-duckdb
-Version: 0.6.0
+Version: 0.7.0
 Summary: Singer.io target for loading data into DuckDB
 Home-page: https://github.com/jwills/target-duckdb
 Author: Josh Wills
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: jsonschema>=3.2.0
+Requires-Dist: duckdb==0.10.2
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pylint; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 
 # target-duckdb
 
 [![License: Apache2](https://img.shields.io/badge/License-Apache2-yellow.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [Singer](https://www.singer.io/) target that loads data into DuckDB following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).
```

