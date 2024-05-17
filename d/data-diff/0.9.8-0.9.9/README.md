# Comparing `tmp/data_diff-0.9.8.tar.gz` & `tmp/data_diff-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_diff-0.9.8.tar", max compression
+gzip compressed data, was "data_diff-0.9.9.tar", max compression
```

## Comparing `data_diff-0.9.8.tar` & `data_diff-0.9.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.9.8/LICENSE
--rw-r--r--   0        0        0    10185 2023-10-10 17:50:38.424368 data_diff-0.9.8/README.md
--rw-r--r--   0        0        0     8890 2023-10-02 19:39:47.061643 data_diff-0.9.8/data_diff/__init__.py
--rw-r--r--   0        0        0    18650 2023-10-23 20:09:05.018207 data_diff-0.9.8/data_diff/__main__.py
--rw-r--r--   0        0        0        0 2023-10-02 19:39:47.062259 data_diff-0.9.8/data_diff/abcs/__init__.py
--rw-r--r--   0        0        0      174 2023-10-02 20:03:14.207661 data_diff-0.9.8/data_diff/abcs/compiler.py
--rw-r--r--   0        0        0     4631 2023-10-23 20:09:05.018766 data_diff-0.9.8/data_diff/abcs/database_types.py
--rw-r--r--   0        0        0      156 2023-10-02 19:39:47.063071 data_diff-0.9.8/data_diff/cloud/__init__.py
--rw-r--r--   0        0        0    11591 2023-10-02 19:39:47.063221 data_diff-0.9.8/data_diff/cloud/data_source.py
--rw-r--r--   0        0        0    10548 2023-10-09 17:07:25.434981 data_diff-0.9.8/data_diff/cloud/datafold_api.py
--rw-r--r--   0        0        0     4379 2023-08-15 16:53:54.334973 data_diff-0.9.8/data_diff/config.py
--rw-r--r--   0        0        0     1072 2023-10-23 20:09:05.019106 data_diff-0.9.8/data_diff/databases/__init__.py
--rw-r--r--   0        0        0    10595 2023-10-03 18:50:55.133846 data_diff-0.9.8/data_diff/databases/_connect.py
--rw-r--r--   0        0        0    45327 2023-10-25 18:07:52.996096 data_diff-0.9.8/data_diff/databases/base.py
--rw-r--r--   0        0        0     9791 2023-10-25 18:07:52.996599 data_diff-0.9.8/data_diff/databases/bigquery.py
--rw-r--r--   0        0        0     6607 2023-10-25 18:07:52.996922 data_diff-0.9.8/data_diff/databases/clickhouse.py
--rw-r--r--   0        0        0     6875 2023-10-25 18:07:52.997211 data_diff-0.9.8/data_diff/databases/databricks.py
--rw-r--r--   0        0        0     5375 2023-10-25 18:07:52.997710 data_diff-0.9.8/data_diff/databases/duckdb.py
--rw-r--r--   0        0        0     6588 2023-10-25 18:07:52.998158 data_diff-0.9.8/data_diff/databases/mssql.py
--rw-r--r--   0        0        0     4081 2023-10-25 18:07:52.998485 data_diff-0.9.8/data_diff/databases/mysql.py
--rw-r--r--   0        0        0     6140 2023-10-25 18:07:52.998781 data_diff-0.9.8/data_diff/databases/oracle.py
--rw-r--r--   0        0        0     5843 2023-10-25 18:07:52.999176 data_diff-0.9.8/data_diff/databases/postgresql.py
--rw-r--r--   0        0        0     6067 2023-10-25 18:07:52.999428 data_diff-0.9.8/data_diff/databases/presto.py
--rw-r--r--   0        0        0     6367 2023-10-25 16:36:14.169918 data_diff-0.9.8/data_diff/databases/redshift.py
--rw-r--r--   0        0        0     5993 2023-10-25 18:07:52.999668 data_diff-0.9.8/data_diff/databases/snowflake.py
--rw-r--r--   0        0        0     1407 2023-10-25 16:36:14.170875 data_diff-0.9.8/data_diff/databases/trino.py
--rw-r--r--   0        0        0     4753 2023-10-25 18:07:53.000130 data_diff-0.9.8/data_diff/databases/vertica.py
--rw-r--r--   0        0        0    20565 2023-10-02 19:39:47.065899 data_diff-0.9.8/data_diff/dbt.py
--rw-r--r--   0        0        0     1734 2023-09-13 16:36:06.164822 data_diff-0.9.8/data_diff/dbt_config_validators.py
--rw-r--r--   0        0        0    21848 2023-10-13 21:53:34.897428 data_diff-0.9.8/data_diff/dbt_parser.py
--rw-r--r--   0        0        0    14602 2023-10-25 16:36:14.171755 data_diff-0.9.8/data_diff/diff_tables.py
--rw-r--r--   0        0        0     2419 2023-08-22 21:53:29.909954 data_diff-0.9.8/data_diff/errors.py
--rw-r--r--   0        0        0     9768 2023-10-02 20:03:14.212053 data_diff-0.9.8/data_diff/format.py
--rw-r--r--   0        0        0     9776 2023-10-25 16:36:14.171913 data_diff-0.9.8/data_diff/hashdiff_tables.py
--rw-r--r--   0        0        0     2024 2023-10-02 20:03:14.212330 data_diff-0.9.8/data_diff/info_tree.py
--rw-r--r--   0        0        0    15834 2023-10-10 17:50:38.426417 data_diff-0.9.8/data_diff/joindiff_tables.py
--rw-r--r--   0        0        0     7663 2023-10-02 20:03:14.212683 data_diff-0.9.8/data_diff/lexicographic_space.py
--rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.9.8/data_diff/parse_time.py
--rw-r--r--   0        0        0        0 2023-10-13 21:53:34.897541 data_diff-0.9.8/data_diff/py.typed
--rw-r--r--   0        0        0        0 2023-10-02 19:39:47.066892 data_diff-0.9.8/data_diff/queries/__init__.py
--rw-r--r--   0        0        0     5304 2023-10-02 19:39:47.066983 data_diff-0.9.8/data_diff/queries/api.py
--rw-r--r--   0        0        0    23004 2023-10-25 16:36:14.172098 data_diff-0.9.8/data_diff/queries/ast_classes.py
--rw-r--r--   0        0        0      346 2023-10-02 20:03:14.213049 data_diff-0.9.8/data_diff/queries/base.py
--rw-r--r--   0        0        0      658 2023-10-02 20:03:14.213158 data_diff-0.9.8/data_diff/queries/extras.py
--rw-r--r--   0        0        0     1474 2023-10-02 19:39:47.067336 data_diff-0.9.8/data_diff/query_utils.py
--rw-r--r--   0        0        0      749 2023-10-02 20:03:14.213490 data_diff-0.9.8/data_diff/schema.py
--rw-r--r--   0        0        0    11040 2023-10-23 20:08:22.581458 data_diff-0.9.8/data_diff/table_segment.py
--rw-r--r--   0        0        0     2980 2023-10-02 20:03:14.213820 data_diff-0.9.8/data_diff/thread_utils.py
--rw-r--r--   0        0        0     5960 2023-10-02 19:39:47.067973 data_diff-0.9.8/data_diff/tracking.py
--rw-r--r--   0        0        0    15527 2023-10-15 23:04:05.726434 data_diff-0.9.8/data_diff/utils.py
--rw-r--r--   0        0        0       22 2023-10-25 18:08:09.596960 data_diff-0.9.8/data_diff/version.py
--rwxr-xr-x   0        0        0     2780 2023-10-25 18:08:04.267274 data_diff-0.9.8/pyproject.toml
--rw-r--r--   0        0        0    12635 1970-01-01 00:00:00.000000 data_diff-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.9.9/LICENSE
+-rw-r--r--   0        0        0    10185 2023-10-10 17:50:38.424368 data_diff-0.9.9/README.md
+-rw-r--r--   0        0        0     8890 2023-10-02 19:39:47.061643 data_diff-0.9.9/data_diff/__init__.py
+-rw-r--r--   0        0        0    18650 2023-10-30 16:35:48.033393 data_diff-0.9.9/data_diff/__main__.py
+-rw-r--r--   0        0        0        0 2023-10-02 19:39:47.062259 data_diff-0.9.9/data_diff/abcs/__init__.py
+-rw-r--r--   0        0        0      174 2023-10-02 20:03:14.207661 data_diff-0.9.9/data_diff/abcs/compiler.py
+-rw-r--r--   0        0        0     4631 2023-10-30 16:35:48.033606 data_diff-0.9.9/data_diff/abcs/database_types.py
+-rw-r--r--   0        0        0      156 2023-10-02 19:39:47.063071 data_diff-0.9.9/data_diff/cloud/__init__.py
+-rw-r--r--   0        0        0    11591 2023-10-02 19:39:47.063221 data_diff-0.9.9/data_diff/cloud/data_source.py
+-rw-r--r--   0        0        0    10548 2023-10-09 17:07:25.434981 data_diff-0.9.9/data_diff/cloud/datafold_api.py
+-rw-r--r--   0        0        0     4379 2023-08-15 16:53:54.334973 data_diff-0.9.9/data_diff/config.py
+-rw-r--r--   0        0        0     1072 2023-10-30 16:35:48.033745 data_diff-0.9.9/data_diff/databases/__init__.py
+-rw-r--r--   0        0        0    10595 2023-10-03 18:50:55.133846 data_diff-0.9.9/data_diff/databases/_connect.py
+-rw-r--r--   0        0        0    45327 2023-10-30 20:11:35.207576 data_diff-0.9.9/data_diff/databases/base.py
+-rw-r--r--   0        0        0     9857 2023-10-30 20:11:39.191039 data_diff-0.9.9/data_diff/databases/bigquery.py
+-rw-r--r--   0        0        0     6607 2023-10-30 16:35:48.034778 data_diff-0.9.9/data_diff/databases/clickhouse.py
+-rw-r--r--   0        0        0     6875 2023-10-30 16:35:48.035215 data_diff-0.9.9/data_diff/databases/databricks.py
+-rw-r--r--   0        0        0     5375 2023-10-30 16:35:48.035531 data_diff-0.9.9/data_diff/databases/duckdb.py
+-rw-r--r--   0        0        0     6588 2023-10-30 16:35:48.035790 data_diff-0.9.9/data_diff/databases/mssql.py
+-rw-r--r--   0        0        0     4081 2023-10-30 16:35:48.035990 data_diff-0.9.9/data_diff/databases/mysql.py
+-rw-r--r--   0        0        0     6140 2023-10-30 16:35:48.036239 data_diff-0.9.9/data_diff/databases/oracle.py
+-rw-r--r--   0        0        0     5843 2023-10-30 20:11:35.208227 data_diff-0.9.9/data_diff/databases/postgresql.py
+-rw-r--r--   0        0        0     6067 2023-10-30 16:35:48.036704 data_diff-0.9.9/data_diff/databases/presto.py
+-rw-r--r--   0        0        0     6367 2023-10-30 16:35:48.037124 data_diff-0.9.9/data_diff/databases/redshift.py
+-rw-r--r--   0        0        0     5993 2023-10-30 16:35:48.037376 data_diff-0.9.9/data_diff/databases/snowflake.py
+-rw-r--r--   0        0        0     1407 2023-10-30 16:35:48.037767 data_diff-0.9.9/data_diff/databases/trino.py
+-rw-r--r--   0        0        0     4753 2023-10-30 16:35:48.038020 data_diff-0.9.9/data_diff/databases/vertica.py
+-rw-r--r--   0        0        0    20565 2023-10-02 19:39:47.065899 data_diff-0.9.9/data_diff/dbt.py
+-rw-r--r--   0        0        0     1734 2023-09-13 16:36:06.164822 data_diff-0.9.9/data_diff/dbt_config_validators.py
+-rw-r--r--   0        0        0    21848 2023-10-30 16:35:48.038468 data_diff-0.9.9/data_diff/dbt_parser.py
+-rw-r--r--   0        0        0    14602 2023-10-30 16:35:48.038876 data_diff-0.9.9/data_diff/diff_tables.py
+-rw-r--r--   0        0        0     2419 2023-08-22 21:53:29.909954 data_diff-0.9.9/data_diff/errors.py
+-rw-r--r--   0        0        0     9768 2023-10-02 20:03:14.212053 data_diff-0.9.9/data_diff/format.py
+-rw-r--r--   0        0        0     9776 2023-10-30 16:35:48.039209 data_diff-0.9.9/data_diff/hashdiff_tables.py
+-rw-r--r--   0        0        0     2024 2023-10-02 20:03:14.212330 data_diff-0.9.9/data_diff/info_tree.py
+-rw-r--r--   0        0        0    15834 2023-10-10 17:50:38.426417 data_diff-0.9.9/data_diff/joindiff_tables.py
+-rw-r--r--   0        0        0     7663 2023-10-02 20:03:14.212683 data_diff-0.9.9/data_diff/lexicographic_space.py
+-rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.9.9/data_diff/parse_time.py
+-rw-r--r--   0        0        0        0 2023-10-30 16:35:48.039249 data_diff-0.9.9/data_diff/py.typed
+-rw-r--r--   0        0        0        0 2023-10-02 19:39:47.066892 data_diff-0.9.9/data_diff/queries/__init__.py
+-rw-r--r--   0        0        0     5304 2023-10-02 19:39:47.066983 data_diff-0.9.9/data_diff/queries/api.py
+-rw-r--r--   0        0        0    23004 2023-10-30 16:35:48.039812 data_diff-0.9.9/data_diff/queries/ast_classes.py
+-rw-r--r--   0        0        0      346 2023-10-02 20:03:14.213049 data_diff-0.9.9/data_diff/queries/base.py
+-rw-r--r--   0        0        0      658 2023-10-02 20:03:14.213158 data_diff-0.9.9/data_diff/queries/extras.py
+-rw-r--r--   0        0        0     1474 2023-10-02 19:39:47.067336 data_diff-0.9.9/data_diff/query_utils.py
+-rw-r--r--   0        0        0      749 2023-10-02 20:03:14.213490 data_diff-0.9.9/data_diff/schema.py
+-rw-r--r--   0        0        0    11040 2023-10-23 20:08:22.581458 data_diff-0.9.9/data_diff/table_segment.py
+-rw-r--r--   0        0        0     2980 2023-10-02 20:03:14.213820 data_diff-0.9.9/data_diff/thread_utils.py
+-rw-r--r--   0        0        0     5960 2023-10-02 19:39:47.067973 data_diff-0.9.9/data_diff/tracking.py
+-rw-r--r--   0        0        0    15527 2023-10-15 23:04:05.726434 data_diff-0.9.9/data_diff/utils.py
+-rw-r--r--   0        0        0       22 2023-10-30 20:12:00.804982 data_diff-0.9.9/data_diff/version.py
+-rwxr-xr-x   0        0        0     2780 2023-10-30 20:11:57.019036 data_diff-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0    12635 1970-01-01 00:00:00.000000 data_diff-0.9.9/PKG-INFO
```

### Comparing `data_diff-0.9.8/LICENSE` & `data_diff-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/README.md` & `data_diff-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/__init__.py` & `data_diff-0.9.9/data_diff/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/__main__.py` & `data_diff-0.9.9/data_diff/__main__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/abcs/database_types.py` & `data_diff-0.9.9/data_diff/abcs/database_types.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/cloud/data_source.py` & `data_diff-0.9.9/data_diff/cloud/data_source.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/cloud/datafold_api.py` & `data_diff-0.9.9/data_diff/cloud/datafold_api.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/config.py` & `data_diff-0.9.9/data_diff/config.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/databases/__init__.py` & `data_diff-0.9.9/data_diff/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/databases/_connect.py` & `data_diff-0.9.9/data_diff/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/databases/base.py` & `data_diff-0.9.9/data_diff/databases/base.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/databases/bigquery.py` & `data_diff-0.9.9/data_diff/databases/bigquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,25 +189,26 @@
 
     def __init__(self, project, *, dataset, bigquery_credentials=None, **kw):
         super().__init__()
         credentials = bigquery_credentials
         bigquery = import_bigquery()
 
         keyfile = kw.pop("keyfile", None)
+        impersonate_service_account = kw.pop("impersonate_service_account", None)
         if keyfile:
             bigquery_service_account = import_bigquery_service_account()
             credentials = bigquery_service_account.Credentials.from_service_account_file(
                 keyfile,
                 scopes=["https://www.googleapis.com/auth/cloud-platform"],
             )
-        elif kw.get("impersonate_service_account"):
+        elif impersonate_service_account:
             bigquery_service_account_impersonation = import_bigquery_service_account_impersonation()
             credentials = bigquery_service_account_impersonation.Credentials(
                 source_credentials=credentials,
-                target_principal=kw["impersonate_service_account"],
+                target_principal=impersonate_service_account,
                 target_scopes=["https://www.googleapis.com/auth/cloud-platform"],
             )
 
         self._client = bigquery.Client(project=project, credentials=credentials, **kw)
         self.project = project
         self.dataset = dataset
```

### Comparing `data_diff-0.9.8/data_diff/databases/clickhouse.py` & `data_diff-0.9.9/data_diff/databases/clickhouse.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/databases/databricks.py` & `data_diff-0.9.9/data_diff/databases/databricks.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/databases/duckdb.py` & `data_diff-0.9.9/data_diff/databases/duckdb.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/databases/mssql.py` & `data_diff-0.9.9/data_diff/databases/mssql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/databases/mysql.py` & `data_diff-0.9.9/data_diff/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/databases/oracle.py` & `data_diff-0.9.9/data_diff/databases/oracle.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/databases/postgresql.py` & `data_diff-0.9.9/data_diff/databases/postgresql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/databases/presto.py` & `data_diff-0.9.9/data_diff/databases/presto.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/databases/redshift.py` & `data_diff-0.9.9/data_diff/databases/redshift.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/databases/snowflake.py` & `data_diff-0.9.9/data_diff/databases/snowflake.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/databases/trino.py` & `data_diff-0.9.9/data_diff/databases/trino.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/databases/vertica.py` & `data_diff-0.9.9/data_diff/databases/vertica.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/dbt.py` & `data_diff-0.9.9/data_diff/dbt.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/dbt_config_validators.py` & `data_diff-0.9.9/data_diff/dbt_config_validators.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/dbt_parser.py` & `data_diff-0.9.9/data_diff/dbt_parser.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/diff_tables.py` & `data_diff-0.9.9/data_diff/diff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/errors.py` & `data_diff-0.9.9/data_diff/errors.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/format.py` & `data_diff-0.9.9/data_diff/format.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/hashdiff_tables.py` & `data_diff-0.9.9/data_diff/hashdiff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/info_tree.py` & `data_diff-0.9.9/data_diff/info_tree.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/joindiff_tables.py` & `data_diff-0.9.9/data_diff/joindiff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/lexicographic_space.py` & `data_diff-0.9.9/data_diff/lexicographic_space.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/parse_time.py` & `data_diff-0.9.9/data_diff/parse_time.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/queries/api.py` & `data_diff-0.9.9/data_diff/queries/api.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/queries/ast_classes.py` & `data_diff-0.9.9/data_diff/queries/ast_classes.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/queries/extras.py` & `data_diff-0.9.9/data_diff/queries/extras.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/query_utils.py` & `data_diff-0.9.9/data_diff/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/schema.py` & `data_diff-0.9.9/data_diff/schema.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/table_segment.py` & `data_diff-0.9.9/data_diff/table_segment.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/thread_utils.py` & `data_diff-0.9.9/data_diff/thread_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/tracking.py` & `data_diff-0.9.9/data_diff/tracking.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/data_diff/utils.py` & `data_diff-0.9.9/data_diff/utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.9.8/pyproject.toml` & `data_diff-0.9.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-diff"
-version = "0.9.8"
+version = "0.9.9"
 description = "Command-line tool and Python library to efficiently diff rows across two different databases."
 authors = ["Datafold <data-diff@datafold.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/datafold/data-diff"
 documentation = ""
 classifiers = [
```

### Comparing `data_diff-0.9.8/PKG-INFO` & `data_diff-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-diff
-Version: 0.9.8
+Version: 0.9.9
 Summary: Command-line tool and Python library to efficiently diff rows across two different databases.
 Home-page: https://github.com/datafold/data-diff
 License: MIT
 Author: Datafold
 Author-email: data-diff@datafold.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: data-diff Version: 0.9.8 Summary: Command-line tool
+Metadata-Version: 2.1 Name: data-diff Version: 0.9.9 Summary: Command-line tool
 and Python library to efficiently diff rows across two different databases.
 Home-page: https://github.com/datafold/data-diff License: MIT Author: Datafold
 Author-email: data-diff@datafold.com Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Environment ::
 Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
 Administrators Classifier: License :: OSI Approved :: MIT License Classifier:
```

