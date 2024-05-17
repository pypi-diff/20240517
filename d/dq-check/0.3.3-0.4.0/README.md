# Comparing `tmp/dq_check-0.3.3.tar.gz` & `tmp/dq_check-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dq_check-0.3.3.tar", last modified: Thu May 16 13:20:31 2024, max compression
+gzip compressed data, was "dq_check-0.4.0.tar", last modified: Fri May 17 04:48:50 2024, max compression
```

## Comparing `dq_check-0.3.3.tar` & `dq_check-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-16 13:20:31.226602 dq_check-0.3.3/
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-16 13:20:31.226255 dq_check-0.3.3/PKG-INFO
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2440 2024-05-12 21:16:29.000000 dq_check-0.3.3/README.md
--rw-r--r--   0 rohan.goel   (502) staff       (20)      327 2024-05-16 13:20:04.000000 dq_check-0.3.3/pyproject.toml
--rw-r--r--   0 rohan.goel   (502) staff       (20)      131 2024-05-16 13:20:31.227375 dq_check-0.3.3/setup.cfg
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-16 13:20:31.218479 dq_check-0.3.3/src/
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-16 13:20:31.221379 dq_check-0.3.3/src/dq_check/
--rw-r--r--   0 rohan.goel   (502) staff       (20)       29 2024-05-05 04:45:50.000000 dq_check-0.3.3/src/dq_check/__init__.py
--rw-r--r--   0 rohan.goel   (502) staff       (20)    16294 2024-05-16 13:19:09.000000 dq_check-0.3.3/src/dq_check/dq_check.py
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-16 13:20:31.225587 dq_check-0.3.3/src/dq_check.egg-info/
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-16 13:20:31.000000 dq_check-0.3.3/src/dq_check.egg-info/PKG-INFO
--rw-r--r--   0 rohan.goel   (502) staff       (20)      263 2024-05-16 13:20:31.000000 dq_check-0.3.3/src/dq_check.egg-info/SOURCES.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)        1 2024-05-16 13:20:31.000000 dq_check-0.3.3/src/dq_check.egg-info/dependency_links.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)       15 2024-05-16 13:20:31.000000 dq_check-0.3.3/src/dq_check.egg-info/requires.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)        9 2024-05-16 13:20:31.000000 dq_check-0.3.3/src/dq_check.egg-info/top_level.txt
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-17 04:48:50.528087 dq_check-0.4.0/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-17 04:48:50.527859 dq_check-0.4.0/PKG-INFO
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2440 2024-05-12 21:16:29.000000 dq_check-0.4.0/README.md
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      327 2024-05-17 04:47:38.000000 dq_check-0.4.0/pyproject.toml
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      131 2024-05-17 04:48:50.528808 dq_check-0.4.0/setup.cfg
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-17 04:48:50.520299 dq_check-0.4.0/src/
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-17 04:48:50.522842 dq_check-0.4.0/src/dq_check/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)       29 2024-05-05 04:45:50.000000 dq_check-0.4.0/src/dq_check/__init__.py
+-rw-r--r--   0 rohan.goel   (502) staff       (20)    17516 2024-05-17 04:47:15.000000 dq_check-0.4.0/src/dq_check/dq_check.py
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-17 04:48:50.527275 dq_check-0.4.0/src/dq_check.egg-info/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-17 04:48:50.000000 dq_check-0.4.0/src/dq_check.egg-info/PKG-INFO
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      263 2024-05-17 04:48:50.000000 dq_check-0.4.0/src/dq_check.egg-info/SOURCES.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)        1 2024-05-17 04:48:50.000000 dq_check-0.4.0/src/dq_check.egg-info/dependency_links.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)       15 2024-05-17 04:48:50.000000 dq_check-0.4.0/src/dq_check.egg-info/requires.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)        9 2024-05-17 04:48:50.000000 dq_check-0.4.0/src/dq_check.egg-info/top_level.txt
```

### Comparing `dq_check-0.3.3/PKG-INFO` & `dq_check-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq_check
-Version: 0.3.3
+Version: 0.4.0
 Summary: A data quality check module for Spark
 Author-email: rohan goel <rohan.goel@databricks.com>
 Description-Content-Type: text/markdown
 Requires-Dist: pyspark
 Requires-Dist: pandas
 
 ## dq_check
```

### Comparing `dq_check-0.3.3/README.md` & `dq_check-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dq_check-0.3.3/src/dq_check/dq_check.py` & `dq_check-0.4.0/src/dq_check/dq_check.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,25 +110,27 @@
         return columns, tables
         
     def perform_dq_check(self,
                          table_type: str,
                          table_name: str,
                          primary_keys: List[str],
                          sql_query: str,
+                         check_type:str,
                          where_clause: Optional[str] = None,
                          quality_threshold_percentage: int = 5,
                          chunk_size:int = 200) -> tuple:
         """
         Perform data quality checks on a specified table using a given SQL query and save the results into a Delta table.
 
         Args:
             table_type (str): The type of the table ('delta' or 'asql').
             table_name (str): The name of the table.
             primary_keys (List[str]): List of primary key columns. 
             sql_query (str): The data quality check query.
+            check_type(str): This would either be record_check or agg_check. record_check for dq checks that dont have aggregates
             where_clause(str): where clause to get sample data for DQE check
             quality_threshold_percentage (int): Quality threshold percentage (default is 5%).
             chunk_size (int): how many pks per record in audit log table.
 
         Returns:
         Tuple[str, float]: Tuple containing:
             - Status of the data quality check ('Passed' or 'Failed').
@@ -139,27 +141,35 @@
         """
 
         # Validate input parameters
 
         # if not isinstance(self.spark, SparkSession):
         #     raise ValueError("Invalid input: 'spark' must be an instance of SparkSession.")
         
-        if table_type not in ['delta', 'asql']:
+        if table_type.lower() not in ['delta', 'asql']:
             raise ValueError("Invalid input: 'table_type' must be 'delta' or 'asql'.")
         
         if not isinstance(table_name, str) or not table_name:
             raise ValueError("Invalid input: 'table_name' must be a non-empty string.")
         
         table_dot_cnt = table_name.count(".")
         if not (table_dot_cnt == 2 or table_dot_cnt == 1):
             raise ValueError("Invalid input: 'table_name' must be a non-empty string and with (catalog and schema name) for delta or with schema name only for asql.")
         
-        if not isinstance(primary_keys, list) or not all(isinstance(key, str) for key in primary_keys):
-            raise ValueError("Invalid input: 'primary_keys' must be a list of strings.")
+        if check_type.lower() not in ['record_check', 'agg_check']:
+            raise ValueError("Invalid input: 'check_type' must be 'record_check' or 'agg_check'.")
         
+        if check_type.lower() == 'record_check':
+            if not isinstance(primary_keys, list) or not all(isinstance(key, str) for key in primary_keys) or len(primary_keys) == 0:
+                raise ValueError("Invalid input: 'primary_keys' must be a non-empty list of strings.")
+        else:
+            if not isinstance(primary_keys, list) or len(primary_keys) != 0:
+                raise ValueError("Invalid input: 'primary_keys' for agg_check must be empty list [].")
+
+            
         if not isinstance(sql_query, str) or not sql_query:
             raise ValueError("Invalid input: 'sql_query' must be a non-empty string.")
         
         if where_clause is not None and not isinstance(where_clause, str):
             raise ValueError("Invalid input: 'where_clause' must be a string if provided.")
         
         if not isinstance(quality_threshold_percentage, int) or quality_threshold_percentage < 0 or quality_threshold_percentage > 100:
@@ -168,16 +178,17 @@
         audit_dot_cnt = self.audit_table_name.count(".")
         if not isinstance(self.audit_table_name, str) or not self.audit_table_name or not audit_dot_cnt == 2 :
             raise ValueError("Invalid input: 'audit_table_name' must be a non-empty string and with catalog and schema name.")
         
         #remove colon at end if present
         sql_query = sql_query.replace(';','')
         # Check if the query contains aggregation functions
-        aggregates = ['min', 'max', 'avg', 'sum', 'count', 'group by']
-        agg_ind = next(('y' for i in aggregates if i in sql_query.lower()), None)
+        #aggregates = ['min', 'max', 'avg', 'sum', 'count', 'group by']
+        #agg_ind = next(('y' for i in aggregates if i in sql_query.lower()), None)
+        agg_ind = 'y' if check_type == 'agg_check' else None
         
         #get catalog,schema,table for DQ table
         table_dtls = table_name.split(".")
         catalog = table_dtls[0] if table_dot_cnt == 2 else None
         schema = table_dtls[-2]
         table_name_only = table_dtls[-1]
         
@@ -221,31 +232,37 @@
         #validate sql
 
         table_cols,sql_tables = self.parse_sql_query(sql_query)
 
         # table validation for sample data
         if table_name not in sql_query:
             raise ValueError(f"table {table_name} not in sql from clause {sql_query}")
-
-        
-        if '*' not in table_cols:
-          #primary key validation
-          if set(primary_keys) - set(table_cols):
-                  if not agg_ind:
-                      agg_without_pk_ind = 'n'
-                      raise ValueError(f"primary key {primary_keys} not in sql select clause {table_cols}")
-                  else:
-                      agg_without_pk_ind = 'y'
-          else:
-            agg_without_pk_ind = 'n'
-        else:
-            agg_without_pk_ind = 'n'
         
-        print(F"agg_without_pk_ind is {agg_without_pk_ind}")
 
+        
+        # if '*' not in table_cols:
+        #   #primary key validation
+        #   if set(primary_keys) - set(table_cols):
+        #           if not agg_ind:
+        #               agg_without_pk_ind = 'n'
+        #               raise ValueError(f"primary key {primary_keys} not in sql select clause {table_cols}")
+        #           else:
+        #               agg_without_pk_ind = 'y'
+        #   else:
+        #     agg_without_pk_ind = 'n'
+        # else:
+        #     agg_without_pk_ind = 'n'
+        
+        # print(F"agg_without_pk_ind is {agg_without_pk_ind}")
+
+        if check_type.lower() == "record_check":
+            if '*' not in sql_query:
+                if set(primary_keys) - set(table_cols):
+                    raise ValueError(f"primary key {primary_keys} not in sql select clause {table_cols}")
+                
         #### DQ check logic     
 
         #get total count from table for batch id
         total_count_sql = f"with sql_sample as ({sql_stmt}) select count(*) as tot_cnt from sql_sample"
         print(F"total count sql:{total_count_sql}")
         #create dq check sql
         #dq_sql = f"with sql_sample as ({sql_stmt}) " + sql_query.replace(table_name,'sql_sample')
@@ -264,47 +281,51 @@
 
         df_dq_count = client.read_sql(dq_count_sql)
         df_total_count = client.read_sql(total_count_sql)
         dq_count = list(df_dq_count.first().asDict().values())[0]
         total_count = list(df_total_count.first().asDict().values())[0]
 
         print(F"dq_cnt and total_cnt are {dq_count} and {total_count}")
-        # Calculate percentage score of failed records
+
         percentage_score = round((dq_count / total_count) * 100,2)
         # Determine the status based on the quality threshold
-        if not agg_ind or agg_without_pk_ind == 'n':
+        if check_type.lower() == 'record_check':
+            # Calculate percentage score of failed records
             status = "Passed" if percentage_score <= quality_threshold_percentage else "Failed"
         elif dq_count > 0:
             status = "Failed"
+            #percentage_score = 0.00
         else:
             status = "Passed"
+            #percentage_score = 0.00
         # Collect primary keys of failed records
         failed_primary_keys = {}
         #failed_primary_keys_sample = {}
-        sort_col = primary_keys[0]
-        if agg_without_pk_ind == 'n':
+        if check_type.lower() == 'record_check':
+            sort_col = primary_keys[0]
             try:
                 df_failed_primary_keys = client.read_sql(dq_primary_key_sql)
 
                 #below will be met incase of when there are no failed records.
 
                 if df_failed_primary_keys.count() == 0:
                    df_failed_primary_keys = client.read_sql(F'select "" as {sort_col}') 
                 # add all pk cols to df_failed_primary_keys df
                    for pk in primary_keys:
                        if pk != sort_col:
                             df_failed_primary_keys = df_failed_primary_keys.withColumn(pk,lit(''))
             except Exception as e:
                 raise KeyError(F"primary keys {primary_keys} are not found in table {table_name}. Please see error below \n {e}")
         else:
-            df_failed_primary_keys = client.read_sql(F'select "" as {sort_col}')
-                # add all pk cols to df_failed_primary_keys df
-            for pk in primary_keys:
-                if pk != sort_col:
-                    df_failed_primary_keys = df_failed_primary_keys.withColumn(pk,lit(''))
+            df_failed_primary_keys = client.read_sql(F'select "NA" as pk')
+            primary_keys = ['pk']
+            #     # add all pk cols to df_failed_primary_keys df
+            # for pk in primary_keys:
+            #     if pk != sort_col:
+            #         df_failed_primary_keys = df_failed_primary_keys.withColumn(pk,lit(''))
 
         df_failed_primary_keys = df_failed_primary_keys.withColumn("constant",lit(1))
         window_spec = Window.orderBy("constant")
 
         df_with_row_number = df_failed_primary_keys.withColumn("Seq",row_number().over(window_spec))
         df_with_chunk = df_with_row_number.withColumn("ChunkNo",((col("Seq")/chunk_size) - 0.05).cast('int') + 1)
 
@@ -317,29 +338,30 @@
         # Prepare expressions for create_map dynamically
         map_exprs = [(lit(column).alias("Key"), col(column).alias("Value")) for column in primary_keys]
 
         # Create a single map column for all columns
         map_expr = create_map(*[expr for expr in sum(map_exprs, ())])
 
         # Add the map column to the DataFrame
-        df_mapped_values = df_aggregated.withColumn("FailedRecordsKeys", map_expr)
+        df_mapped_values = df_aggregated.withColumn("FailedRecordsKeys", map_expr) 
 
         audit_log_df = (df_mapped_values.withColumn("UniqueCheckID",lit(str(uuid.uuid4())))
                                 .withColumn("RunId",lit(self.run_id))
                                 .withColumn("CheckTimestamp",current_timestamp())
                                 .withColumn("TableName",lit(table_name))
                                 .withColumn("TableType",lit(table_type))
+                                .withColumn("CheckType",lit(check_type))
                                 .withColumn("QueryUsed",lit(sql_query))
                                 .withColumn("Status",lit(status))
                                 .withColumn("FailedRecordCount",lit(dq_count))
                                 .withColumn("PercentageScore",lit(percentage_score))
                                 .withColumn("CurrentUser",current_user())
                                 .drop(*primary_keys)
                                 .select("UniqueCheckID","RunId","CheckTimestamp","TableName"
-                                        ,"TableType","QueryUsed","Status","FailedRecordCount","PercentageScore","FailedRecordsKeys","CurrentUser")
+                                        ,"TableType","CheckType","QueryUsed","Status","FailedRecordCount","PercentageScore","FailedRecordsKeys","CurrentUser")
                                 )
 
         print(F"Appending DQE results to table {self.audit_table_name}")    
 
         # Write the audit log data into the Delta table
         #display(audit_log_df)
         audit_log_df.write.format("delta").option("mergeSchema", "true").mode("append").saveAsTable(self.audit_table_name)
```

### Comparing `dq_check-0.3.3/src/dq_check.egg-info/PKG-INFO` & `dq_check-0.4.0/src/dq_check.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq_check
-Version: 0.3.3
+Version: 0.4.0
 Summary: A data quality check module for Spark
 Author-email: rohan goel <rohan.goel@databricks.com>
 Description-Content-Type: text/markdown
 Requires-Dist: pyspark
 Requires-Dist: pandas
 
 ## dq_check
```

