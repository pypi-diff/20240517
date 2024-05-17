# Comparing `tmp/mariadb_sqlbuilder-1.1.tar.gz` & `tmp/mariadb_sqlbuilder-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mariadb_sqlbuilder-1.1.tar", last modified: Wed May 15 22:50:59 2024, max compression
+gzip compressed data, was "mariadb_sqlbuilder-1.1.1.tar", last modified: Fri May 17 08:50:17 2024, max compression
```

## Comparing `mariadb_sqlbuilder-1.1.tar` & `mariadb_sqlbuilder-1.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:50:59.295782 mariadb_sqlbuilder-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:50:59.295782 mariadb_sqlbuilder-1.1/MariaDB_SQLBuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-15 22:50:59.000000 mariadb_sqlbuilder-1.1/MariaDB_SQLBuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-15 22:50:59.000000 mariadb_sqlbuilder-1.1/MariaDB_SQLBuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 22:50:59.000000 mariadb_sqlbuilder-1.1/MariaDB_SQLBuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 22:50:59.000000 mariadb_sqlbuilder-1.1/MariaDB_SQLBuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 22:50:59.000000 mariadb_sqlbuilder-1.1/MariaDB_SQLBuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-15 22:50:59.295782 mariadb_sqlbuilder-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:50:59.291782 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:50:59.295782 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15951 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/base_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/delete_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/dict_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/exists_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/insert_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/join_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/select_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/update_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/upsert_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/exepetions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:50:59.295782 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/conditions_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/connection_dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/filter_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/subquery_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/validator_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:50:59.295782 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/sqlscript/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/sqlscript/splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 22:50:59.295782 mariadb_sqlbuilder-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-15 22:50:51.000000 mariadb_sqlbuilder-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:50:17.695752 mariadb_sqlbuilder-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:50:17.695752 mariadb_sqlbuilder-1.1.1/MariaDB_SQLBuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-17 08:50:17.000000 mariadb_sqlbuilder-1.1.1/MariaDB_SQLBuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-17 08:50:17.000000 mariadb_sqlbuilder-1.1.1/MariaDB_SQLBuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:50:17.000000 mariadb_sqlbuilder-1.1.1/MariaDB_SQLBuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 08:50:17.000000 mariadb_sqlbuilder-1.1.1/MariaDB_SQLBuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-17 08:50:17.000000 mariadb_sqlbuilder-1.1.1/MariaDB_SQLBuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-17 08:50:17.695752 mariadb_sqlbuilder-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:50:17.691752 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:50:17.691752 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15971 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/base_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/delete_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/dict_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/exists_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/insert_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/join_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/select_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/update_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/upsert_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/exepetions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:50:17.695752 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/helpful/
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/helpful/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/helpful/conditions_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/helpful/connection_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/helpful/filter_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/helpful/subquery_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/helpful/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/helpful/validator_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:50:17.695752 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/sqlscript/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/sqlscript/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:50:17.695752 mariadb_sqlbuilder-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-17 08:50:13.000000 mariadb_sqlbuilder-1.1.1/setup.py
```

### Comparing `mariadb_sqlbuilder-1.1/LICENSE` & `mariadb_sqlbuilder-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/MariaDB_SQLBuilder.egg-info/PKG-INFO` & `mariadb_sqlbuilder-1.1.1/MariaDB_SQLBuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MariaDB-SQLBuilder
-Version: 1.1
+Version: 1.1.1
 Summary: MariaDB SQL Builder is a simple way to use Maria SQL. Use your own SQL or use the integrated Maria SQL Builder tool.
 Home-page: https://github.com/princessmiku/MariaDB-SQLBuilder
 Author: Miku
 Author-email: 
 License: LGPL 2.1
 Keywords: database,mariadb,sql,builder,script builder,mariadb sql
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mariadb_sqlbuilder-1.1/MariaDB_SQLBuilder.egg-info/SOURCES.txt` & `mariadb_sqlbuilder-1.1.1/MariaDB_SQLBuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/PKG-INFO` & `mariadb_sqlbuilder-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MariaDB-SQLBuilder
-Version: 1.1
+Version: 1.1.1
 Summary: MariaDB SQL Builder is a simple way to use Maria SQL. Use your own SQL or use the integrated Maria SQL Builder tool.
 Home-page: https://github.com/princessmiku/MariaDB-SQLBuilder
 Author: Miku
 Author-email: 
 License: LGPL 2.1
 Keywords: database,mariadb,sql,builder,script builder,mariadb sql
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mariadb_sqlbuilder-1.1/README.md` & `mariadb_sqlbuilder-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/__init__.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/__init__.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/base_builder.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/base_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,15 +150,19 @@
             elif isinstance(expression, str):
                 expression_list_str: str = _get_tcn(self.tb, expression)
             else:
                 expression_list_str: str = str(expression)
 
             sql_script = value.get_sql()[:-1]
             sql_values = value.values_for_execute
-            self.__conditions.append(self._as_conditions_dict(f"{expression_list_str} IN ({sql_script})", sql_values))
+            self.__conditions.append(
+                self._as_conditions_dict(
+                    f"{expression_list_str} IN ({sql_script})", sql_values
+                )
+            )
         elif isinstance(expression, str):
             self.__conditions.append(self._as_conditions_dict(
                 f"{_get_tcn(self.tb, expression)} IN ?", str(value))
             )
         else:
             self.__conditions.append(
                 self._as_conditions_dict(
@@ -186,15 +190,19 @@
             elif isinstance(expression, str):
                 expression_list_str: str = _get_tcn(self.tb, expression)
             else:
                 expression_list_str: str = str(expression)
             sql_script = value.get_sql()[:-1]
             sql_values = value.values_for_execute
 
-            self.__conditions.append(self._as_conditions_dict(f"{expression_list_str} IN ({sql_script})", sql_values))
+            self.__conditions.append(
+                self._as_conditions_dict(
+                    f"{expression_list_str} IN ({sql_script})", sql_values
+                )
+            )
 
         elif isinstance(expression, str):
             self.__conditions.append(
                 self._as_conditions_dict(
                     f"{_get_tcn(self.tb, expression)} NOT IN ?",
                     str(value)
                 )
@@ -259,19 +267,19 @@
             if value1 > value2:
                 raise BetweenValueIsBigger("Value 1 is bigger then value 2")
         from .select_builder import SelectBuilder
         if isinstance(expression, str):
             if isinstance(value1, SelectBuilder):
                 value1 = f"({value1.get_sql()[:-1]})"
             else:
-                value1 = _transform_value_valid(value1)
+                value1 = value1
             if isinstance(value2, SelectBuilder):
                 value2 = f"({value2.get_sql()[:-1]})"
             else:
-                value2 = _transform_value_valid(value2)
+                value2 = value2
             self.__conditions.append(self._as_conditions_dict(
                 f"{_get_tcn(self.tb, expression)} "
                 f"BETWEEN ? "
                 f"AND ?", [value1, value2])
             )
         else:
             self.__conditions.append(self._as_conditions_dict(
@@ -296,24 +304,24 @@
             if value1 > value2:
                 raise BetweenValueIsBigger("Value 1 is bigger then value 2")
         from .select_builder import SelectBuilder
         if isinstance(expression, str):
             if isinstance(value1, SelectBuilder):
                 value1 = f"({value1.get_sql()[:-1]})"
             else:
-                value1 = _transform_value_valid(value1)
+                value1 = value1
             if isinstance(value2, SelectBuilder):
                 value2 = f"({value2.get_sql()[:-1]})"
             else:
-                value2 = _transform_value_valid(value2)
-                self.__conditions.append(self._as_conditions_dict(
-                    f"{_get_tcn(self.tb, expression)} "
-                    f"NOT BETWEEN ? "
-                    f"AND ?", [value1, value2])
-                )
+                value2 = value2
+            self.__conditions.append(self._as_conditions_dict(
+                f"{_get_tcn(self.tb, expression)} "
+                f"NOT BETWEEN ? "
+                f"AND ?", [value1, value2])
+            )
         else:
             self.__conditions.append(self._as_conditions_dict(
                 f"{expression} "
                 f"NOT BETWEEN ? "
                 f"AND ?", [value1, value2])
             )
         return self
```

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/delete_builder.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/delete_builder.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/dict_converter.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/dict_converter.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/exists_builder.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/exists_builder.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/insert_builder.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/insert_builder.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/join_builder.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/join_builder.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/select_builder.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/select_builder.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/update_builder.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/update_builder.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/builder/upsert_builder.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/builder/upsert_builder.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/connector.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/connector.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/exepetions.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/exepetions.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/arithmetic.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/helpful/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/conditions_saver.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/helpful/conditions_saver.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/connection_dummy.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/helpful/connection_dummy.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/validator.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/helpful/validator.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/helpful/validator_dummy.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/helpful/validator_dummy.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/mariadb_sqlbuilder/sqlscript/splitter.py` & `mariadb_sqlbuilder-1.1.1/mariadb_sqlbuilder/sqlscript/splitter.py`

 * *Files identical despite different names*

### Comparing `mariadb_sqlbuilder-1.1/setup.py` & `mariadb_sqlbuilder-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
-VERSION = '1.1'
+VERSION = '1.1.1'
 
 setup(
     name='MariaDB-SQLBuilder',
     long_description=README,
     long_description_content_type="text/markdown",
     version=VERSION,
     packages=[
```

