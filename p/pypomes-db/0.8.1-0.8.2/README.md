# Comparing `tmp/pypomes_db-0.8.1.tar.gz` & `tmp/pypomes_db-0.8.2.tar.gz`

## Comparing `pypomes_db-0.8.1.tar` & `pypomes_db-0.8.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.8.1/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    11837 2020-02-02 00:00:00.000000 pypomes_db-0.8.1/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.8.1/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    18101 2020-02-02 00:00:00.000000 pypomes_db-0.8.1/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.1/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.8.1/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    15231 2020-02-02 00:00:00.000000 pypomes_db-0.8.1/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.8.1/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.8.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.8.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.1/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.8.2/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 pypomes_db-0.8.2/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    31355 2020-02-02 00:00:00.000000 pypomes_db-0.8.2/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    18614 2020-02-02 00:00:00.000000 pypomes_db-0.8.2/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.2/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.8.2/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    15231 2020-02-02 00:00:00.000000 pypomes_db-0.8.2/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.8.2/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.8.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.8.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.2/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.8.2/PKG-INFO
```

### Comparing `pypomes_db-0.8.1/src/pypomes_db/__init__.py` & `pypomes_db-0.8.2/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.1/src/pypomes_db/db_common.py` & `pypomes_db-0.8.2/src/pypomes_db/db_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #   {APP_PREFIX}_DB_HOST
 #   {APP_PREFIX}_DB_PORT
 #   {APP_PREFIX}_DB_CLIENT  (for oracle)
 #   {APP_PREFIX}_DB_DRIVER  (for sqlserver)
 # 2. alternatively, specify a comma-separated list of engines in
 #   {APP_PREFIX}_DB_ENGINES
 #   and for each engine, specify the set above, replacing 'DB' with
-#   'MSQL', 'ORCL', 'PG', and 'SQLS', respectively for engines listed above
+#   'MSQL', 'ORCL', 'PG', and 'SQLS', respectively for the engines listed above
 
 _DB_CONN_DATA: dict = {}
 _DB_ENGINES: list[str] = []
 if env_get_str(f"{APP_PREFIX}_DB_ENGINE",  None):
     _default_setup: bool = True
     _DB_ENGINES.append(env_get_str(f"{APP_PREFIX}_DB_ENGINE"))
 else:
```

### Comparing `pypomes_db-0.8.1/src/pypomes_db/db_pomes.py` & `pypomes_db-0.8.2/src/pypomes_db/db_pomes.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,30 +97,36 @@
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: True if the trial connection succeeded, False otherwise
     """
     # initialize the return variable
     result: bool = False
 
-    curr_engine: str = _assert_engine(errors=errors,
+    # initialize the local errors list
+    op_errors: list[str] = []
+
+    curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     proceed: bool = True
     if curr_engine == "oracle":
         from . import oracle_pomes
         # noinspection PyProtectedMember
-        proceed = oracle_pomes.initialize(errors=errors,
+        proceed = oracle_pomes.initialize(errors=op_errors,
                                           logger=logger)
     if proceed:
-        conn: Any = db_connect(errors=errors,
+        conn: Any = db_connect(errors=op_errors,
                                engine=curr_engine,
                                logger=logger)
         if conn:
             conn.close()
             result = True
 
+    # acknowledge eventual local errors
+    errors.extend(op_errors)
+
     return result
 
 
 def db_connect(errors: list[str] | None,
                engine: str = None,
                logger: Logger = None) -> Any:
     """
@@ -132,31 +138,37 @@
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the connection to the database
     """
     # initialize the return variable
     result: Any = None
 
-    curr_engine: str = _assert_engine(errors=errors,
+    # initialize the local errors list
+    op_errors: list[str] = []
+
+    curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_connect(errors=errors,
+        result = oracle_pomes.db_connect(errors=op_errors,
                                          logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.db_connect(errors=errors,
+        result = postgres_pomes.db_connect(errors=op_errors,
                                            logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_connect(errors=errors,
+        result = sqlserver_pomes.db_connect(errors=op_errors,
                                             logger=logger)
 
+    # acknowledge eventual local errors
+    errors.extend(op_errors)
+
     return result
 
 
 def db_exists(errors: list[str],
               table: str,
               where_attrs: list[str] = None,
               where_vals: tuple = None,
@@ -175,26 +187,32 @@
     :param where_attrs: the search attributes
     :param where_vals: the values for the search attributes
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: True if at least one tuple was found
     """
+    # initialize the local errors list
+    op_errors: list[str] = []
+
     # noinspection PyDataSource
     sel_stmt: str = "SELECT * FROM " + table
     if where_attrs:
         sel_stmt += " WHERE " + "".join(f"{attr} = %s AND " for attr in where_attrs)[0:-5]
-    rec: tuple = db_select_one(errors=errors,
+    rec: tuple = db_select_one(errors=op_errors,
                                sel_stmt=sel_stmt,
                                where_vals=where_vals,
                                require_nonempty=False,
                                engine = engine,
                                conn=conn,
                                logger=logger)
-    result: bool = None if errors else rec is not None
+    result: bool = None if op_errors else rec is not None
+
+    # acknowledge eventual local errors
+    errors.extend(op_errors)
 
     return result
 
 
 def db_select_one(errors: list[str] | None,
                   sel_stmt: str,
                   where_vals: tuple = None,
@@ -215,24 +233,30 @@
     :param where_vals: values to be associated with the search criteria
     :param require_nonempty: defines whether an empty search should be considered an error
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
+    # initialize the local errors list
+    op_errors: list[str] = []
+
     require_min: int = 1 if require_nonempty else None
-    reply: list[tuple] = db_select_all(errors=errors,
+    reply: list[tuple] = db_select_all(errors=op_errors,
                                        sel_stmt=sel_stmt,
                                        where_vals=where_vals,
                                        require_min=require_min,
                                        require_max=1,
                                        engine = engine,
                                        conn=conn,
                                        logger=logger)
 
+    # acknowledge eventual local errors
+    errors.extend(op_errors)
+
     return reply[0] if reply else None
 
 
 def db_select_all(errors: list[str] | None,
                   sel_stmt: str,
                   where_vals: tuple = None,
                   require_min: int = None,
@@ -258,46 +282,52 @@
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] | None = None
 
-    curr_engine: str = _assert_engine(errors=errors,
+    # initialize the local errors list
+    op_errors: list[str] = []
+
+    curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_select_all(errors=errors,
+        result = oracle_pomes.db_select_all(errors=op_errors,
                                             sel_stmt=sel_stmt,
                                             where_vals=where_vals,
                                             require_min=require_min,
                                             require_max=require_max,
                                             conn=conn,
                                             logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.db_select_all(errors=errors,
+        result = postgres_pomes.db_select_all(errors=op_errors,
                                               sel_stmt=sel_stmt,
                                               where_vals=where_vals,
                                               require_min=require_min,
                                               require_max=require_max,
                                               conn=conn,
                                               logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_select_all(errors=errors,
+        result = sqlserver_pomes.db_select_all(errors=op_errors,
                                                sel_stmt=sel_stmt,
                                                where_vals=where_vals,
                                                require_min=require_min,
                                                require_max=require_max,
                                                conn=conn,
                                                logger=logger)
 
+    # acknowledge eventual local errors
+    errors.extend(op_errors)
+
     return result
 
 
 def db_insert(errors: list[str] | None,
               insert_stmt: str,
               insert_vals: tuple,
               engine: str = None,
@@ -312,20 +342,28 @@
     :param insert_stmt: the INSERT command
     :param insert_vals: the values to be inserted
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the number of inserted tuples (0 ou 1), or None if an error occurred
     """
-    return db_execute(errors=errors,
-                      exc_stmt=insert_stmt,
-                      bind_vals=insert_vals,
-                      engine=engine,
-                      conn=conn,
-                      logger=logger)
+    # initialize the local errors list
+    op_errors: list[str] = []
+
+    result: int = db_execute(errors=op_errors,
+                             exc_stmt=insert_stmt,
+                             bind_vals=insert_vals,
+                             engine=engine,
+                             conn=conn,
+                             logger=logger)
+
+    # acknowledge eventual local errors
+    errors.extend(op_errors)
+
+    return result
 
 
 def db_update(errors: list[str] | None,
               update_stmt: str,
               update_vals: tuple = None,
               where_vals: tuple = None,
               engine: str = None,
@@ -343,27 +381,35 @@
     :param update_vals: the values for the update operation
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the number of updated tuples, or None if an error occurred
     """
+    # initialize the local errors list
+    op_errors: list[str] = []
+
     bind_vals: tuple | None = None
     if update_vals and where_vals:
         bind_vals = update_vals + where_vals
     elif update_vals:
         bind_vals = update_vals
     elif where_vals:
         bind_vals = where_vals
-    return db_execute(errors=errors,
-                      exc_stmt=update_stmt,
-                      bind_vals=bind_vals,
-                      engine=engine,
-                      conn=conn,
-                      logger=logger)
+    result: int = db_execute(errors=op_errors,
+                             exc_stmt=update_stmt,
+                             bind_vals=bind_vals,
+                             engine=engine,
+                             conn=conn,
+                             logger=logger)
+
+    # acknowledge eventual local errors
+    errors.extend(op_errors)
+
+    return result
 
 
 def db_delete(errors: list[str] | None,
               delete_stmt: str,
               where_vals: tuple = None,
               engine: str = None,
               conn: Any = None,
@@ -378,20 +424,28 @@
     :param delete_stmt: the DELETE command
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the number of deleted tuples, or None if an error occurred
     """
-    return db_execute(errors=errors,
-                      exc_stmt=delete_stmt,
-                      bind_vals=where_vals,
-                      engine=engine,
-                      conn=conn,
-                      logger=logger)
+    # initialize the local errors list
+    op_errors: list[str] = []
+
+    result: int = db_execute(errors=op_errors,
+                             exc_stmt=delete_stmt,
+                             bind_vals=where_vals,
+                             engine=engine,
+                             conn=conn,
+                             logger=logger)
+
+    # acknowledge eventual local errors
+    errors.extend(op_errors)
+
+    return result
 
 
 def db_bulk_insert(errors: list[str] | None,
                    insert_stmt: str,
                    insert_vals: list[tuple],
                    engine: str = None,
                    conn: Any = None,
@@ -408,52 +462,58 @@
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
-    curr_engine: str = _assert_engine(errors, engine)
+    # initialize the local errors list
+    op_errors: list[str] = []
+
+    curr_engine: str = _assert_engine(op_errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_bulk_insert(errors=errors,
+        result = oracle_pomes.db_bulk_insert(errors=op_errors,
                                              insert_stmt=insert_stmt,
                                              insert_vals=insert_vals,
                                              conn=conn,
                                              logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.db_bulk_insert(errors=errors,
+        result = postgres_pomes.db_bulk_insert(errors=op_errors,
                                                insert_stmt=insert_stmt,
                                                insert_vals=insert_vals,
                                                conn=conn,
                                                logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_bulk_insert(errors=errors,
+        result = sqlserver_pomes.db_bulk_insert(errors=op_errors,
                                                 insert_stmt=insert_stmt,
                                                 insert_vals=insert_vals,
                                                 conn=conn,
                                                 logger=logger)
 
+    # acknowledge eventual local errors
+    errors.extend(op_errors)
+
     return result
 
 
 def db_update_lob(errors: list[str],
-                 lob_table: str,
-                 lob_column: str,
-                 pk_columns: list[str],
-                 pk_vals: tuple,
-                 lob_file: str | Path,
-                 chunk_size: int,
-                 engine: str = None,
-                 conn: Any = None,
-                 logger: Logger = None) -> None:
+                  lob_table: str,
+                  lob_column: str,
+                  pk_columns: list[str],
+                  pk_vals: tuple,
+                  lob_file: str | Path,
+                  chunk_size: int,
+                  engine: str = None,
+                  conn: Any = None,
+                  logger: Logger = None) -> None:
     """
     Update a large binary objects (LOB) in the given table and column.
 
     :param errors: incidental error messages
     :param lob_table: the table to be update with the new LOB
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
@@ -461,51 +521,57 @@
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: number of LOBs effectively copied
     """
-    curr_engine: str = _assert_engine(errors, engine)
+    # initialize the local errors list
+    op_errors: list[str] = []
+
+    curr_engine: str = _assert_engine(op_errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        oracle_pomes.db_update_lob(errors=errors,
+        oracle_pomes.db_update_lob(errors=op_errors,
                                    lob_table=lob_table,
                                    lob_column=lob_column,
                                    pk_columns=pk_columns,
                                    pk_vals=pk_vals,
                                    lob_file=lob_file,
                                    chunk_size=chunk_size,
                                    conn=conn,
                                    logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        postgres_pomes.db_update_lob(errors=errors,
+        postgres_pomes.db_update_lob(errors=op_errors,
                                      lob_table=lob_table,
                                      lob_column=lob_column,
                                      pk_columns=pk_columns,
                                      pk_vals=pk_vals,
                                      lob_file=lob_file,
                                      chunk_size=chunk_size,
                                      conn=conn,
                                      logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        sqlserver_pomes.db_update_lob(errors=errors,
+        sqlserver_pomes.db_update_lob(errors=op_errors,
                                       lob_table=lob_table,
                                       lob_column=lob_column,
                                       pk_columns=pk_columns,
                                       pk_vals=pk_vals,
                                       lob_file=lob_file,
                                       chunk_size=chunk_size,
                                       conn=conn,
                                       logger=logger)
 
+    # acknowledge eventual local errors
+    errors.extend(op_errors)
+
 
 def db_execute(errors: list[str] | None,
                exc_stmt: str,
                bind_vals: tuple = None,
                engine: str = None,
                conn: Any = None,
                logger: Logger = None) -> int:
@@ -527,39 +593,45 @@
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
-    curr_engine: str = _assert_engine(errors, engine)
+    # initialize the local errors list
+    op_errors: list[str] = []
+
+    curr_engine: str = _assert_engine(op_errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_execute(errors=errors,
+        result = oracle_pomes.db_execute(errors=op_errors,
                                          exc_stmt=exc_stmt,
                                          bind_vals=bind_vals,
                                          conn=conn,
                                          logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.db_execute(errors=errors,
+        result = postgres_pomes.db_execute(errors=op_errors,
                                            exc_stmt=exc_stmt,
                                            bind_vals=bind_vals,
                                            conn=conn,
                                            logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_execute(errors=errors,
+        result = sqlserver_pomes.db_execute(errors=op_errors,
                                             exc_stmt=exc_stmt,
                                             bind_vals=bind_vals,
                                             conn=conn,
                                             logger=logger)
 
+    # acknowledge eventual local errors
+    errors.extend(op_errors)
+
     return result
 
 
 def db_call_function(errors: list[str] | None,
                      func_name: str,
                      func_vals: tuple = None,
                      engine: str = None,
@@ -577,39 +649,45 @@
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the data returned by the function
     """
     # initialize the return variable
     result: Any = None
 
-    curr_engine: str = _assert_engine(errors, engine)
+    # initialize the local errors list
+    op_errors: list[str] = []
+
+    curr_engine: str = _assert_engine(op_errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_call_function(errors=errors,
+        result = oracle_pomes.db_call_function(errors=op_errors,
                                                func_name=func_name,
                                                func_vals=func_vals,
                                                conn=conn,
                                                logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.db_call_procedure(errors=errors,
+        result = postgres_pomes.db_call_procedure(errors=op_errors,
                                                   proc_name=func_name,
                                                   proc_vals=func_vals,
                                                   conn=conn,
                                                   logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_call_procedure(errors=errors,
+        result = sqlserver_pomes.db_call_procedure(errors=op_errors,
                                                    proc_name=func_name,
                                                    proc_vals=func_vals,
                                                    conn=conn,
                                                    logger=logger)
 
+    # acknowledge eventual local errors
+    errors.extend(op_errors)
+
     return result
 
 
 def db_call_procedure(errors: list[str] | None,
                       proc_name: str,
                       proc_vals: tuple = None,
                       engine: str = None,
@@ -627,33 +705,39 @@
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: Any = None
 
-    curr_engine: str = _assert_engine(errors, engine)
+    # initialize the local errors list
+    op_errors: list[str] = []
+
+    curr_engine: str = _assert_engine(op_errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_call_procedure(errors=errors,
+        result = oracle_pomes.db_call_procedure(errors=op_errors,
                                                 proc_name=proc_name,
                                                 proc_vals=proc_vals,
                                                 conn=conn,
                                                 logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.db_call_procedure(errors=errors,
+        result = postgres_pomes.db_call_procedure(errors=op_errors,
                                                   proc_name=proc_name,
                                                   proc_vals=proc_vals,
                                                   conn=conn,
                                                   logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_call_procedure(errors=errors,
+        result = sqlserver_pomes.db_call_procedure(errors=op_errors,
                                                    proc_name=proc_name,
                                                    proc_vals=proc_vals,
                                                    conn=conn,
                                                    logger=logger)
 
+    # acknowledge eventual local errors
+    errors.extend(op_errors)
+
     return result
```

### Comparing `pypomes_db-0.8.1/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.8.2/src/pypomes_db/migration_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,26 +34,29 @@
     :param source_columns: the colums to be migrated
     :param target_engine: the destination database engine type
     :param target_table: the table to write the data to (defaults to the source table)
     :param target_columns: the columns to write the data to (defaults to the source columns)
     :param source_conn: the connection to the source database (obtains a new one, if not specified)
     :param target_conn: the connection to the destination database (obtains a new one, if not specified)
     :param where_clause: the criteria for tuple selection
-    :param batch_size: the maximum number of tuples in to migrate in each batch, or 0 or None for no limit
+    :param batch_size: the maximum number of tuples to migrate in each batch, or 0 or None for no limit
     :param logger: optional logger
-    :return: number of tuples effectively migrated
+    :return: the number of tuples effectively migrated
     """
     # initialize the return variable
     result: int = 0
 
+    # initialize the local errors list
+    op_errors: list[str] = []
+
     # make sure to have connections to the source and destination databases
-    curr_source_conn: Any = source_conn or db_connect(errors=errors,
+    curr_source_conn: Any = source_conn or db_connect(op_errors=op_errors,
                                                       engine=source_engine,
                                                       logger=logger)
-    curr_target_conn: Any = target_conn or db_connect(errors=errors,
+    curr_target_conn: Any = target_conn or db_connect(op_errors=op_errors,
                                                       engine=target_engine,
                                                       logger=logger)
 
     # make sure to have a target table
     if not target_table:
         target_table = source_table
 
@@ -182,19 +185,22 @@
         if curr_target_conn and not target_conn:
             curr_target_conn.close()
 
     # log the migration finish
     _db_log(logger=logger,
             engine=source_engine,
             err_msg=err_msg,
-            errors=errors,
+            errors=op_errors,
             stmt=(f"Migrated {result} tuples, "
                   f"from {source_engine}.{source_table} "
                   f"to {target_engine}.{target_table}"))
 
+    # acknowledge eventual local errors
+    errors.extend(op_errors)
+
     return result
 
 def db_migrate_lobs(errors: list[str],
                     source_engine: str,
                     source_table: str,
                     source_lob_column: str,
                     source_pk_columns: list[str],
@@ -226,24 +232,27 @@
     :param target_lob_column: the column to write the lob to (defaults to the source column)
     :param target_pk_columns: columns making up a primary key, or a unique identifier for a tuple, in target database
     :param source_conn: the connection to the source database (obtains a new one, if not specified)
     :param target_conn: the connection to the destination database (obtains a new one, if not specified)
     :param where_clause: the criteria for tuple selection
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param logger: optional logger
-    :return: number of LOBs effectively migrated
+    :return: the number of LOBs effectively migrated
     """
     # initialize the return variable
     result: int = 0
 
+    # initialize the local errors list
+    op_errors: list[str] = []
+
     # make sure to have connections to the source and destination databases
-    curr_source_conn: Any = source_conn or db_connect(errors=errors,
+    curr_source_conn: Any = source_conn or db_connect(op_errors=op_errors,
                                                       engine=source_engine,
                                                       logger=logger)
-    curr_target_conn: Any = target_conn or db_connect(errors=errors,
+    curr_target_conn: Any = target_conn or db_connect(op_errors=op_errors,
                                                       engine=target_engine,
                                                       logger=logger)
 
     # make sure to have a target table
     if not target_table:
         target_table = source_table
 
@@ -331,27 +340,30 @@
                         pass
                     case "oracle":
                         ora_lob.write(data=lob_data,
                                       offset=offset)
                     case "postgres":
                         from psycopg2 import Binary
                         # remove append indication on first update
-                        if offset == 1:
-                            update_pg: str = update_stmt.replace(f"{target_lob_column} || ", "")
-                        else:
-                            update_pg: str = update_stmt
+                        update_pg: str = update_stmt if offset > 1 else \
+                                         update_stmt.replace(f"{target_lob_column} || ", "")
+
                         # string data may come from LOB (Oracle's NCLOB is a good example)
                         col_data: str | Binary = Binary(lob_data) if isinstance(lob_data, bytes) else lob_data
                         target_cursor.execute(query=update_pg,
                                               vars=(col_data, *pk_vals))
                     case "sqlserver":
                         from pyodbc import Binary
+                        # remove append indication on first update
+                        update_sqls: str = update_stmt if offset > 1 else \
+                                           update_stmt.replace(f"{target_lob_column} || ", "")
+
                         # string data may come from LOB (Oracle's NCLOB is a good example)
                         col_data: str | Binary = Binary(lob_data) if isinstance(lob_data, bytes) else lob_data
-                        target_cursor.execute(sql=update_stmt,
+                        target_cursor.execute(sql=update_sqls,
                                               params=(col_data, *pk_vals))
                 # read the next chunk
                 offset += size
                 lob_data = lob.read(offset=offset,
                                     amount=chunk_size)
 
             # increment the LOB migration counter, if applicable
@@ -386,13 +398,16 @@
         if curr_target_conn and not target_conn:
             curr_target_conn.close()
 
     # log the migration finish
     _db_log(logger=logger,
             engine=source_engine,
             err_msg=err_msg,
-            errors=errors,
+            errors=op_errors,
             stmt=(f"Migrated {result} LOBs, "
                   f"from {source_engine}.{source_table}.{source_lob_column} "
                   f"to {target_engine}.{target_table}.{target_lob_column}"))
 
+    # acknowledge eventual local errors
+    errors.extend(op_errors)
+
     return result
```

### Comparing `pypomes_db-0.8.1/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.8.2/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.1/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.8.2/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.1/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.8.2/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.1/LICENSE` & `pypomes_db-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.1/pyproject.toml` & `pypomes_db-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.8.1"
+version = "0.8.2"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

