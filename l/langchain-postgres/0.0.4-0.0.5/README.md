# Comparing `tmp/langchain_postgres-0.0.4.tar.gz` & `tmp/langchain_postgres-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_postgres-0.0.4.tar", max compression
+gzip compressed data, was "langchain_postgres-0.0.5.tar", max compression
```

## Comparing `langchain_postgres-0.0.4.tar` & `langchain_postgres-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-05-15 17:56:55.771859 langchain_postgres-0.0.4/LICENSE
--rw-r--r--   0        0        0     5090 2024-05-15 17:56:55.775859 langchain_postgres-0.0.4/README.md
--rw-r--r--   0        0        0      621 2024-05-15 17:56:55.775859 langchain_postgres-0.0.4/langchain_postgres/__init__.py
--rw-r--r--   0        0        0     2914 2024-05-15 17:56:55.775859 langchain_postgres-0.0.4/langchain_postgres/_utils.py
--rw-r--r--   0        0        0    14033 2024-05-15 17:56:55.775859 langchain_postgres-0.0.4/langchain_postgres/chat_message_histories.py
--rw-r--r--   0        0        0    23519 2024-05-15 17:56:55.775859 langchain_postgres-0.0.4/langchain_postgres/checkpoint.py
--rw-r--r--   0        0        0        0 2024-05-15 17:56:55.775859 langchain_postgres-0.0.4/langchain_postgres/py.typed
--rw-r--r--   0        0        0    49908 2024-05-15 17:56:55.775859 langchain_postgres-0.0.4/langchain_postgres/vectorstores.py
--rw-r--r--   0        0        0     2121 2024-05-15 17:56:55.775859 langchain_postgres-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6014 1970-01-01 00:00:00.000000 langchain_postgres-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-17 15:18:33.805163 langchain_postgres-0.0.5/LICENSE
+-rw-r--r--   0        0        0     5090 2024-05-17 15:18:33.809162 langchain_postgres-0.0.5/README.md
+-rw-r--r--   0        0        0      621 2024-05-17 15:18:33.809162 langchain_postgres-0.0.5/langchain_postgres/__init__.py
+-rw-r--r--   0        0        0     2914 2024-05-17 15:18:33.809162 langchain_postgres-0.0.5/langchain_postgres/_utils.py
+-rw-r--r--   0        0        0    14033 2024-05-17 15:18:33.809162 langchain_postgres-0.0.5/langchain_postgres/chat_message_histories.py
+-rw-r--r--   0        0        0    23519 2024-05-17 15:18:33.809162 langchain_postgres-0.0.5/langchain_postgres/checkpoint.py
+-rw-r--r--   0        0        0        0 2024-05-17 15:18:33.809162 langchain_postgres-0.0.5/langchain_postgres/py.typed
+-rw-r--r--   0        0        0    50367 2024-05-17 15:18:33.809162 langchain_postgres-0.0.5/langchain_postgres/vectorstores.py
+-rw-r--r--   0        0        0     2121 2024-05-17 15:18:33.809162 langchain_postgres-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6014 1970-01-01 00:00:00.000000 langchain_postgres-0.0.5/PKG-INFO
```

### Comparing `langchain_postgres-0.0.4/LICENSE` & `langchain_postgres-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.4/README.md` & `langchain_postgres-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.4/langchain_postgres/__init__.py` & `langchain_postgres-0.0.5/langchain_postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.4/langchain_postgres/_utils.py` & `langchain_postgres-0.0.5/langchain_postgres/_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.4/langchain_postgres/chat_message_histories.py` & `langchain_postgres-0.0.5/langchain_postgres/chat_message_histories.py`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.4/langchain_postgres/checkpoint.py` & `langchain_postgres-0.0.5/langchain_postgres/checkpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.4/langchain_postgres/vectorstores.py` & `langchain_postgres-0.0.5/langchain_postgres/vectorstores.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     "$gte": ">=",
 }
 
 SPECIAL_CASED_OPERATORS = {
     "$in",
     "$nin",
     "$between",
+    "$exists",
 }
 
 TEXT_OPERATORS = {
     "$like",
     "$ilike",
 }
 
@@ -698,21 +699,32 @@
                         )
 
             queried_field = self.EmbeddingStore.cmetadata[field].astext
 
             if operator in {"$in"}:
                 return queried_field.in_([str(val) for val in filter_value])
             elif operator in {"$nin"}:
-                return queried_field.nin_([str(val) for val in filter_value])
+                return ~queried_field.in_([str(val) for val in filter_value])
             elif operator in {"$like"}:
                 return queried_field.like(filter_value)
             elif operator in {"$ilike"}:
                 return queried_field.ilike(filter_value)
             else:
                 raise NotImplementedError()
+        elif operator == "$exists":
+            if not isinstance(filter_value, bool):
+                raise ValueError(
+                    "Expected a boolean value for $exists "
+                    f"operator, but got: {filter_value}"
+                )
+            condition = func.jsonb_exists(
+                self.EmbeddingStore.cmetadata,
+                field,
+            )
+            return ~condition if filter_value else condition
         else:
             raise NotImplementedError()
 
     def _create_filter_clause_deprecated(self, key, value):  # type: ignore[no-untyped-def]
         """Deprecated functionality.
 
         This is for backwards compatibility with the JSON based schema for metadata.
```

### Comparing `langchain_postgres-0.0.4/pyproject.toml` & `langchain_postgres-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-postgres"
-version = "0.0.4"
+version = "0.0.5"
 description = "An integration package connecting Postgres and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-postgres"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `langchain_postgres-0.0.4/PKG-INFO` & `langchain_postgres-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-postgres
-Version: 0.0.4
+Version: 0.0.5
 Summary: An integration package connecting Postgres and LangChain
 Home-page: https://github.com/langchain-ai/langchain-postgres
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

