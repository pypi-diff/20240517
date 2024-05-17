# Comparing `tmp/docmesh_core-0.0.4.tar.gz` & `tmp/docmesh_core-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_core-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_core-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_core-0.0.4.tar` & `docmesh_core-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       10 2024-05-13 04:13:58.033801 docmesh_core-0.0.4/README.md
--rw-r--r--   0        0        0       22 2024-05-16 05:07:40.528095 docmesh_core-0.0.4/docmesh_core/__init__.py
--rw-r--r--   0        0        0     1244 2024-05-15 11:01:49.702507 docmesh_core-0.0.4/docmesh_core/db/__init__.py
--rw-r--r--   0        0        0     1325 2024-05-13 04:13:58.033801 docmesh_core-0.0.4/docmesh_core/db/auth.py
--rw-r--r--   0        0        0    10869 2024-05-15 11:28:37.262344 docmesh_core-0.0.4/docmesh_core/db/neo.py
--rw-r--r--   0        0        0      417 2024-05-15 10:24:49.939048 docmesh_core-0.0.4/docmesh_core/utils/__init__.py
--rw-r--r--   0        0        0      269 2024-05-13 04:13:58.037801 docmesh_core-0.0.4/docmesh_core/utils/graph_utils.py
--rw-r--r--   0        0        0     3857 2024-05-13 11:40:13.918990 docmesh_core-0.0.4/docmesh_core/utils/semantic_scholar.py
--rw-r--r--   0        0        0      750 2024-05-13 04:13:58.037801 docmesh_core-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 docmesh_core-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-05-13 04:13:58.033801 docmesh_core-0.0.5/README.md
+-rw-r--r--   0        0        0       22 2024-05-17 06:23:16.598358 docmesh_core-0.0.5/docmesh_core/__init__.py
+-rw-r--r--   0        0        0     1244 2024-05-15 11:01:49.702507 docmesh_core-0.0.5/docmesh_core/db/__init__.py
+-rw-r--r--   0        0        0     1325 2024-05-13 04:13:58.033801 docmesh_core-0.0.5/docmesh_core/db/auth.py
+-rw-r--r--   0        0        0    10901 2024-05-16 11:05:05.685045 docmesh_core-0.0.5/docmesh_core/db/neo.py
+-rw-r--r--   0        0        0      417 2024-05-15 10:24:49.939048 docmesh_core-0.0.5/docmesh_core/utils/__init__.py
+-rw-r--r--   0        0        0      269 2024-05-13 04:13:58.037801 docmesh_core-0.0.5/docmesh_core/utils/graph_utils.py
+-rw-r--r--   0        0        0     3857 2024-05-13 11:40:13.918990 docmesh_core-0.0.5/docmesh_core/utils/semantic_scholar.py
+-rw-r--r--   0        0        0      750 2024-05-13 04:13:58.037801 docmesh_core-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 docmesh_core-0.0.5/PKG-INFO
```

### Comparing `docmesh_core-0.0.4/docmesh_core/db/__init__.py` & `docmesh_core-0.0.5/docmesh_core/db/__init__.py`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.4/docmesh_core/db/auth.py` & `docmesh_core-0.0.5/docmesh_core/db/auth.py`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.4/docmesh_core/db/neo.py` & `docmesh_core-0.0.5/docmesh_core/db/neo.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,33 +319,34 @@
         )
     )
 
     return df
 
 
 @db.transaction
-def list_unread_influential_papers(entity_name: str, date_time: str) -> DataFrame:
+def list_unread_influential_papers(entity_name: str, date_time: str, n: int) -> DataFrame:
     # XXX: use cypher query language, since OGM is not well supported
     query = """
         MATCH (p:Paper)
         WHERE p.publication_date >= DATETIME($date_time).epochSeconds
         AND NOT EXISTS {
             (p) <-[:read]- (e:Entity)
             WHERE e.name = $entity_name
         }
         RETURN p.title AS title, p.pdf AS pdf
         ORDER BY p.citation_count DESC
-        limit 10;
+        LIMIT $n;
     """
     df = to_dataframe(
         db.cypher_query(
             query,
             params={
                 "entity_name": entity_name,
                 "date_time": date_time,
+                "n": n,
             },
         )
     )
 
     return df
```

### Comparing `docmesh_core-0.0.4/docmesh_core/utils/semantic_scholar.py` & `docmesh_core-0.0.5/docmesh_core/utils/semantic_scholar.py`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.4/pyproject.toml` & `docmesh_core-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.4/PKG-INFO` & `docmesh_core-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmesh_core
-Version: 0.0.4
+Version: 0.0.5
 Summary: Core components for docmesh.
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

