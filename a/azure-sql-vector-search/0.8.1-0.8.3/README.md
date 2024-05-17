# Comparing `tmp/azure_sql_vector_search-0.8.1.tar.gz` & `tmp/azure_sql_vector_search-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_sql_vector_search-0.8.1.tar", last modified: Thu May 16 00:10:01 2024, max compression
+gzip compressed data, was "azure_sql_vector_search-0.8.3.tar", last modified: Fri May 17 02:07:59 2024, max compression
```

## Comparing `azure_sql_vector_search-0.8.1.tar` & `azure_sql_vector_search-0.8.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 isekpo     (501) staff       (20)        0 2024-05-16 00:10:01.066294 azure_sql_vector_search-0.8.1/
--rw-r--r--   0 isekpo     (501) staff       (20)     1078 2024-05-14 16:08:51.000000 azure_sql_vector_search-0.8.1/LICENSE
--rw-r--r--   0 isekpo     (501) staff       (20)    11838 2024-05-16 00:10:01.064627 azure_sql_vector_search-0.8.1/PKG-INFO
--rw-r--r--   0 isekpo     (501) staff       (20)    11411 2024-05-16 00:00:37.000000 azure_sql_vector_search-0.8.1/README.md
-drwxr-xr-x   0 isekpo     (501) staff       (20)        0 2024-05-16 00:10:01.028591 azure_sql_vector_search-0.8.1/azure_sql_vector_search/
--rw-r--r--   0 isekpo     (501) staff       (20)      277 2024-05-15 10:49:14.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search/__init__.py
--rw-r--r--   0 isekpo     (501) staff       (20)     8979 2024-05-15 23:51:45.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search/classic_vector_search.py
--rw-r--r--   0 isekpo     (501) staff       (20)      239 2024-05-15 10:53:04.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search/models.py
--rw-r--r--   0 isekpo     (501) staff       (20)     7271 2024-05-15 23:51:58.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search/native_vector_search.py
--rw-r--r--   0 isekpo     (501) staff       (20)     7908 2024-05-15 23:50:08.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search/vector_search_base.py
-drwxr-xr-x   0 isekpo     (501) staff       (20)        0 2024-05-16 00:10:01.047203 azure_sql_vector_search-0.8.1/azure_sql_vector_search.egg-info/
--rw-r--r--   0 isekpo     (501) staff       (20)    11838 2024-05-16 00:10:00.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search.egg-info/PKG-INFO
--rw-r--r--   0 isekpo     (501) staff       (20)      473 2024-05-16 00:10:00.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search.egg-info/SOURCES.txt
--rw-r--r--   0 isekpo     (501) staff       (20)        1 2024-05-16 00:10:00.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search.egg-info/dependency_links.txt
--rw-r--r--   0 isekpo     (501) staff       (20)       47 2024-05-16 00:10:00.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search.egg-info/requires.txt
--rw-r--r--   0 isekpo     (501) staff       (20)       24 2024-05-16 00:10:00.000000 azure_sql_vector_search-0.8.1/azure_sql_vector_search.egg-info/top_level.txt
--rw-r--r--   0 isekpo     (501) staff       (20)       38 2024-05-16 00:10:01.066496 azure_sql_vector_search-0.8.1/setup.cfg
--rw-r--r--   0 isekpo     (501) staff       (20)      689 2024-05-16 00:04:33.000000 azure_sql_vector_search-0.8.1/setup.py
+drwxr-xr-x   0 isekpo     (501) staff       (20)        0 2024-05-17 02:07:59.931257 azure_sql_vector_search-0.8.3/
+-rw-r--r--   0 isekpo     (501) staff       (20)     1078 2024-05-14 16:08:51.000000 azure_sql_vector_search-0.8.3/LICENSE
+-rw-r--r--   0 isekpo     (501) staff       (20)    16655 2024-05-17 02:07:59.929941 azure_sql_vector_search-0.8.3/PKG-INFO
+-rw-r--r--   0 isekpo     (501) staff       (20)    16228 2024-05-16 11:04:13.000000 azure_sql_vector_search-0.8.3/README.md
+drwxr-xr-x   0 isekpo     (501) staff       (20)        0 2024-05-17 02:07:59.913388 azure_sql_vector_search-0.8.3/azure_sql_vector_search/
+-rw-r--r--   0 isekpo     (501) staff       (20)      316 2024-05-17 00:45:12.000000 azure_sql_vector_search-0.8.3/azure_sql_vector_search/__init__.py
+-rw-r--r--   0 isekpo     (501) staff       (20)    10409 2024-05-17 02:00:06.000000 azure_sql_vector_search-0.8.3/azure_sql_vector_search/classic_vector_search.py
+-rw-r--r--   0 isekpo     (501) staff       (20)      400 2024-05-16 22:56:06.000000 azure_sql_vector_search-0.8.3/azure_sql_vector_search/models.py
+-rw-r--r--   0 isekpo     (501) staff       (20)     8644 2024-05-17 02:02:19.000000 azure_sql_vector_search-0.8.3/azure_sql_vector_search/native_vector_search.py
+-rw-r--r--   0 isekpo     (501) staff       (20)     8752 2024-05-16 23:16:18.000000 azure_sql_vector_search-0.8.3/azure_sql_vector_search/vector_search_base.py
+drwxr-xr-x   0 isekpo     (501) staff       (20)        0 2024-05-17 02:07:59.928475 azure_sql_vector_search-0.8.3/azure_sql_vector_search.egg-info/
+-rw-r--r--   0 isekpo     (501) staff       (20)    16655 2024-05-17 02:07:59.000000 azure_sql_vector_search-0.8.3/azure_sql_vector_search.egg-info/PKG-INFO
+-rw-r--r--   0 isekpo     (501) staff       (20)      473 2024-05-17 02:07:59.000000 azure_sql_vector_search-0.8.3/azure_sql_vector_search.egg-info/SOURCES.txt
+-rw-r--r--   0 isekpo     (501) staff       (20)        1 2024-05-17 02:07:59.000000 azure_sql_vector_search-0.8.3/azure_sql_vector_search.egg-info/dependency_links.txt
+-rw-r--r--   0 isekpo     (501) staff       (20)       47 2024-05-17 02:07:59.000000 azure_sql_vector_search-0.8.3/azure_sql_vector_search.egg-info/requires.txt
+-rw-r--r--   0 isekpo     (501) staff       (20)       24 2024-05-17 02:07:59.000000 azure_sql_vector_search-0.8.3/azure_sql_vector_search.egg-info/top_level.txt
+-rw-r--r--   0 isekpo     (501) staff       (20)       38 2024-05-17 02:07:59.931438 azure_sql_vector_search-0.8.3/setup.cfg
+-rw-r--r--   0 isekpo     (501) staff       (20)      729 2024-05-17 02:07:57.000000 azure_sql_vector_search-0.8.3/setup.py
```

### Comparing `azure_sql_vector_search-0.8.1/LICENSE` & `azure_sql_vector_search-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `azure_sql_vector_search-0.8.1/azure_sql_vector_search/classic_vector_search.py` & `azure_sql_vector_search-0.8.3/azure_sql_vector_search/classic_vector_search.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import json
 from typing import Optional
 
 from sqlalchemy import Table, Column, Integer, Float, VARCHAR, MetaData
 from sqlalchemy import event, DDL, text
 
-from azure_sql_vector_search.models import DistanceMetric
+from azure_sql_vector_search.models import DistanceMetric, VectorSearchResult
 from azure_sql_vector_search.vector_search_base import AzureSQLBaseVectorSearchClient
 
 
 class AzureSQLClassicVectorSearchClient(AzureSQLBaseVectorSearchClient):
     """
     AzureSQLClassicVectorSearchClient
 
     Performs classic or traditional vector search queries on tables containing vectors using regular SQL statements
     """
+
     def __init__(self, connection_string, table_name):
 
         super().__init__(connection_string, table_name)
 
         self.azure_sql_vector_metadata_table = None
         self.azure_sql_vector_embeddings_table = None
 
@@ -28,15 +29,16 @@
         self.metadata_object = MetaData()
 
         self.azure_sql_vector_metadata_table = Table(
             self.vector_metadata_table_name,
             self.metadata_object,
             Column("record_id", Integer, primary_key=True, autoincrement=True),
             Column("content", VARCHAR(None)),
-            Column("metadata", VARCHAR(None))
+            Column("metadata", VARCHAR(None)),
+            Column("vector_content", VARCHAR(None))
         )
 
         self.azure_sql_vector_embeddings_table = Table(
             self.vector_embeddings_table_name,
             self.metadata_object,
             Column("record_id", Integer, nullable=False),
             Column("item_id", Integer),
@@ -50,21 +52,52 @@
             "after_create",
             DDL(clustered_column_ddl)
         )
 
         # Creates all applicable tables defined in the constructor IF NOT EXISTS
         self.metadata_object.create_all(self.engine)
 
+    def truncate_tables(self):
+        truncate_embeddings_query = "TRUNCATE TABLE {}".format(self.vector_embeddings_table_name)
+        truncate_metadata_query = "TRUNCATE TABLE {}".format(self.vector_metadata_table_name)
+        connection = self.engine.connect()
+
+        connection.execute(text(truncate_embeddings_query))
+        connection.execute(text(truncate_metadata_query))
+
+        connection.commit()
+        connection.close()
+
+    def delete_by_id(self, record_id: int):
+
+        record_identifier = int(record_id)
+
+        delete_embeddings_query = ("DELETE FROM {} WHERE record_id = {}"
+                                   .format(self.vector_embeddings_table_name, record_identifier))
+
+        delete_metadata_query = ("DELETE FROM {} WHERE record_id = {}"
+                                 .format(self.vector_metadata_table_name, record_identifier))
+
+        connection = self.engine.connect()
+
+        connection.execute(text(delete_embeddings_query))
+        connection.execute(text(delete_metadata_query))
+
+        connection.commit()
+        connection.close()
+
     def insert_row(self, content: str, metadata: dict, embeddings: list[float]):
         AzureSQLBaseVectorSearchClient.validate_vector_magnitude(embeddings)
 
+        vector_content = json.dumps(embeddings)
         metadata_json_string = json.dumps(metadata)
         metadata_insert_statement = (self.azure_sql_vector_metadata_table
                                      .insert()
-                                     .values(content=content, metadata=metadata_json_string))
+                                     .values(content=content, metadata=metadata_json_string,
+                                             vector_content=vector_content))
 
         connection = self.engine.connect()
 
         metadata_result = connection.execute(metadata_insert_statement)
 
         # Retrieves the most recent primary key from the metadata table
         record_id = int(metadata_result.inserted_primary_key[0])
@@ -87,30 +120,30 @@
 
         connection.commit()
         connection.close()
 
         return final_results
 
     def compute_similarity(self, embedding_vectors: list[float], similarity_operation: DistanceMetric, k: int = 4,
-                           filters: Optional[dict[str, object]] = None):
+                           filters: Optional[dict[str, object]] = None) -> list[VectorSearchResult]:
 
         if similarity_operation == DistanceMetric.DOT_PRODUCT:
             return self.inner_product(embedding_vectors, k=k, filters=filters)
 
         elif similarity_operation == DistanceMetric.COSINE_SIMILARITY:
             return self.cosine_similarity(embedding_vectors, k=k, filters=filters)
 
         elif similarity_operation == DistanceMetric.EUCLIDEAN_DISTANCE:
             return self.euclidean_distance(embedding_vectors, k=k, filters=filters)
 
         error_message = "Invalid Similarity Operation {}".format(similarity_operation)
         raise ValueError(error_message)
 
     def cosine_similarity(self, embedding_vectors: list[float], k: int = 4,
-                          filters: Optional[dict[str, object]] = None):
+                          filters: Optional[dict[str, object]] = None) -> list[VectorSearchResult]:
 
         AzureSQLBaseVectorSearchClient.validate_vector_magnitude(embedding_vectors)
         embedding_vectors_string = self.convert_embedding_to_json_array(embedding_vectors)
 
         subquery = (AzureSQLBaseVectorSearchClient
                     .prepare_filter_query(filters, "record_id",
                                           self.vector_metadata_table_name))
@@ -135,15 +168,16 @@
                         v2.record_id
                     order by
                         cosine_similarity DESC
                 """.format(embedding_vectors_string, k, self.vector_embeddings_table_name, subquery)
 
         return self.__compute_similarity(select_statement)
 
-    def inner_product(self, embedding_vectors: list[float], k: int = 4, filters: Optional[dict[str, object]] = None):
+    def inner_product(self, embedding_vectors: list[float], k: int = 4,
+                      filters: Optional[dict[str, object]] = None) -> list[VectorSearchResult]:
 
         AzureSQLBaseVectorSearchClient.validate_vector_magnitude(embedding_vectors)
         embedding_vectors_string = self.convert_embedding_to_json_array(embedding_vectors)
 
         subquery = (AzureSQLBaseVectorSearchClient
                     .prepare_filter_query(filters, "record_id",
                                           self.vector_metadata_table_name))
@@ -163,15 +197,15 @@
                     order by
                         inner_product DESC 
                 """.format(embedding_vectors_string, k, self.vector_embeddings_table_name, subquery)
 
         return self.__compute_similarity(select_statement)
 
     def euclidean_distance(self, embedding_vectors: list[float], k: int = 4,
-                           filters: Optional[dict[str, object]] = None):
+                           filters: Optional[dict[str, object]] = None) -> list[VectorSearchResult]:
 
         AzureSQLBaseVectorSearchClient.validate_vector_magnitude(embedding_vectors)
 
         embedding_vectors_string = self.convert_embedding_to_json_array(embedding_vectors)
 
         subquery = (AzureSQLBaseVectorSearchClient
                     .prepare_filter_query(filters, "record_id",
@@ -191,15 +225,15 @@
                         v2.record_id
                     order by
                         euclidean_distance ASC
                 """.format(embedding_vectors_string, k, self.vector_embeddings_table_name, subquery)
 
         return self.__compute_similarity(select_statement)
 
-    def __compute_similarity(self, select_statement: str) -> list[dict]:
+    def __compute_similarity(self, select_statement: str) -> list[VectorSearchResult]:
         conn = self.engine.connect()
         metadata_table = self.vector_metadata_table_name
         return AzureSQLBaseVectorSearchClient.execute_distance_computation(conn, select_statement, metadata_table)
 
     def __str__(self):
         json_object = {
             "embeddings_table": self.vector_embeddings_table_name,
```

### Comparing `azure_sql_vector_search-0.8.1/azure_sql_vector_search/native_vector_search.py` & `azure_sql_vector_search-0.8.3/azure_sql_vector_search/native_vector_search.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 import json
 from typing import Optional
 
 from sqlalchemy import Table, Column, Integer, VARCHAR, VARBINARY, MetaData
 from sqlalchemy import event, DDL, text
 
-from azure_sql_vector_search.models import DistanceMetric
+from azure_sql_vector_search.models import DistanceMetric, VectorSearchResult
 from azure_sql_vector_search.vector_search_base import AzureSQLBaseVectorSearchClient
 
 
 class AzureSQLNativeVectorSearchClient(AzureSQLBaseVectorSearchClient):
     """
     AzureSQLNativeVectorSearchClient
 
     Performs native vector search queries on tables containing vectors using built-in native functions and operations
 
     """
+
     def __init__(self, connection_string, table_name):
         super().__init__(connection_string, table_name)
 
         self.vector_embeddings_table_name = "{}_embeddings".format(table_name)
         self.vector_metadata_table_name = "{}_metadata".format(table_name)
         self.vector_index_name = "{}_vector_cc".format(self.vector_embeddings_table_name)
 
         self.metadata_object = MetaData()
 
         self.azure_sql_vector_metadata_table = Table(
             self.vector_metadata_table_name,
             self.metadata_object,
             Column("record_id", Integer, primary_key=True, autoincrement=True),
             Column("content", VARCHAR(None)),
-            Column("metadata", VARCHAR(None))
+            Column("metadata", VARCHAR(None)),
+            Column("vector_content", VARCHAR(None))
         )
 
         self.azure_sql_vector_embeddings_table = Table(
             self.vector_embeddings_table_name,
             self.metadata_object,
             Column("record_id", Integer, nullable=False),
             Column("vector_embeddings", VARBINARY(8000))
@@ -46,29 +48,58 @@
             "after_create",
             DDL(clustered_column_ddl)
         )
 
         # Creates all applicable tables defined in the constructor IF NOT EXISTS
         self.metadata_object.create_all(self.engine)
 
+    def truncate_tables(self):
+        truncate_embeddings_query = "TRUNCATE TABLE {}".format(self.vector_embeddings_table_name)
+        truncate_metadata_query = "TRUNCATE TABLE {}".format(self.vector_metadata_table_name)
+        connection = self.engine.connect()
+
+        connection.execute(text(truncate_embeddings_query))
+        connection.execute(text(truncate_metadata_query))
+
+        connection.commit()
+        connection.close()
+
+    def delete_by_id(self, record_id: int):
+        connection = self.engine.connect()
+        record_identifier = int(record_id)
+
+        delete_embeddings_query = ("DELETE FROM {} WHERE record_id = {}"
+                                   .format(self.vector_embeddings_table_name, record_identifier))
+
+        delete_metadata_query = ("DELETE FROM {} WHERE record_id = {}"
+                                 .format(self.vector_metadata_table_name, record_identifier))
+
+        connection.execute(text(delete_embeddings_query))
+        connection.execute(text(delete_metadata_query))
+
+        connection.commit()
+        connection.close()
+
     def insert_row(self, content: str, metadata: dict, embeddings: list[float]):
 
         metadata_json_string = json.dumps(metadata)
+
+        vector_content: str = json.dumps(embeddings)
         metadata_insert_statement = (self.azure_sql_vector_metadata_table
                                      .insert()
-                                     .values(content=content, metadata=metadata_json_string))
+                                     .values(content=content, metadata=metadata_json_string,
+                                             vector_content=vector_content))
 
         connection = self.engine.connect()
 
         metadata_result = connection.execute(metadata_insert_statement)
 
         # Retrieves the most recent primary key from the metadata table
         record_id = int(metadata_result.inserted_primary_key[0])
-        vectors: str = json.dumps(embeddings)
-        vector_string = text("JSON_ARRAY_TO_VECTOR('{}')".format(vectors))
+        vector_string = text("JSON_ARRAY_TO_VECTOR('{}')".format(vector_content))
         vectors_insert_statement = (self.azure_sql_vector_embeddings_table
                                     .insert()
                                     .values(record_id=record_id, vector_embeddings=vector_string))
 
         connection.execute(vectors_insert_statement)
 
         final_results = {
@@ -78,30 +109,30 @@
 
         connection.commit()
         connection.close()
 
         return final_results
 
     def compute_similarity(self, embedding_vectors: list[float], similarity_operation: DistanceMetric, k: int = 4,
-                           filters: Optional[dict[str, object]] = None):
+                           filters: Optional[dict[str, object]] = None) -> list[VectorSearchResult]:
 
         if similarity_operation == DistanceMetric.DOT_PRODUCT:
             return self.inner_product(embedding_vectors, k=k, filters=filters)
 
         elif similarity_operation == DistanceMetric.COSINE_SIMILARITY:
             return self.cosine_similarity(embedding_vectors, k=k, filters=filters)
 
         elif similarity_operation == DistanceMetric.EUCLIDEAN_DISTANCE:
             return self.euclidean_distance(embedding_vectors, k=k, filters=filters)
 
         error_message = "Invalid Similarity Operation {}".format(similarity_operation)
         raise ValueError(error_message)
 
     def cosine_similarity(self, embedding_vectors: list[float], k: int = 4,
-                          filters: Optional[dict[str, object]] = None):
+                          filters: Optional[dict[str, object]] = None) -> list[VectorSearchResult]:
 
         embedding_vectors_string = self.convert_embedding_to_json_array(embedding_vectors)
 
         subquery = (AzureSQLBaseVectorSearchClient
                     .prepare_filter_query(filters, "record_id",
                                           self.vector_metadata_table_name))
 
@@ -111,15 +142,15 @@
                    {}
                    ORDER BY cosine_distance desc
                 """.format(k, embedding_vectors_string, self.vector_embeddings_table_name, subquery)
 
         return self.__compute_similarity(select_statement)
 
     def inner_product(self, embedding_vectors: list[float], k: int = 4,
-                      filters: Optional[dict[str, object]] = None):
+                      filters: Optional[dict[str, object]] = None) -> list[VectorSearchResult]:
 
         embedding_vectors_string = self.convert_embedding_to_json_array(embedding_vectors)
 
         subquery = (AzureSQLBaseVectorSearchClient
                     .prepare_filter_query(filters, "record_id",
                                           self.vector_metadata_table_name))
 
@@ -129,15 +160,15 @@
                            {}
                            ORDER BY inner_product desc
                         """.format(k, embedding_vectors_string, self.vector_embeddings_table_name, subquery)
 
         return self.__compute_similarity(select_statement)
 
     def euclidean_distance(self, embedding_vectors: list[float], k: int = 4,
-                           filters: Optional[dict[str, object]] = None):
+                           filters: Optional[dict[str, object]] = None) -> list[VectorSearchResult]:
 
         embedding_vectors_string = self.convert_embedding_to_json_array(embedding_vectors)
 
         subquery = (AzureSQLBaseVectorSearchClient
                     .prepare_filter_query(filters, "record_id",
                                           self.vector_metadata_table_name))
 
@@ -146,15 +177,15 @@
                            FROM {}
                            {}
                            ORDER BY euclidean_distance asc
                                 """.format(k, embedding_vectors_string, self.vector_embeddings_table_name, subquery)
 
         return self.__compute_similarity(select_statement)
 
-    def __compute_similarity(self, select_statement: str) -> list[dict]:
+    def __compute_similarity(self, select_statement: str) -> list[VectorSearchResult]:
         conn = self.engine.connect()
         metadata_table = self.vector_metadata_table_name
         return AzureSQLBaseVectorSearchClient.execute_distance_computation(conn, select_statement, metadata_table)
 
     def __str__(self):
         json_object = {
             "embeddings_table": self.vector_embeddings_table_name,
```

### Comparing `azure_sql_vector_search-0.8.1/azure_sql_vector_search/vector_search_base.py` & `azure_sql_vector_search-0.8.3/azure_sql_vector_search/vector_search_base.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from abc import abstractmethod
 from typing import Any, Optional
 
 import numpy as np
 from sqlalchemy import create_engine, Connection, text
 from sqlalchemy.engine import URL
 
-from azure_sql_vector_search.models import DistanceMetric
+from azure_sql_vector_search.models import DistanceMetric, VectorSearchResult
 
 
 class AzureSQLBaseVectorSearchClient:
     """
     Base class for Azure SQL Vector Search Clients
     """
 
@@ -31,16 +31,21 @@
         """
         Validates the vector magnitude
 
         :param embeddings:
         :exception Throws an exception if the magnitude is zero
         :return:
         """
+        if embeddings is None or len(embeddings) == 0:
+            raise ValueError("Embeddings cannot be empty")
+
         v_magnitude = AzureSQLBaseVectorSearchClient.vector_magnitude(embeddings)
+
         error_message = ("Vectors with Zero magnitude are not valid: {} has a magnitude of zero".format(embeddings))
+
         if v_magnitude == 0:
             raise ValueError(error_message)
 
     @staticmethod
     def vector_magnitude(embedding: list[float]) -> float:
         """
         Computes the vector magnitude of the embedding
@@ -92,15 +97,16 @@
 
         filter_string = " AND ".join(metadata_filters)
 
         return ("WHERE {} IN (SELECT {} FROM {} WHERE {})".
                 format(id_field_name, id_field_name, subquery_table, filter_string))
 
     @staticmethod
-    def execute_distance_computation(connection: Connection, select_statement: str, metadata_table: str):
+    def execute_distance_computation(connection: Connection,
+                                     select_statement: str, metadata_table: str) -> list[VectorSearchResult]:
 
         sql_statement = text(select_statement)
 
         select_result = connection.execute(sql_statement)
 
         result = select_result.fetchall()
 
@@ -116,91 +122,111 @@
             scoring_results.append({"record_id": record_id_value, "distance_score": score})
 
         if len(scoring_results) == 0:
             return []
 
         record_identifiers_filter = ",".join(record_identifiers)
 
-        metadata_select = ("SELECT record_id, content, metadata FROM {} WHERE record_id IN ({})"
+        metadata_select = ("SELECT record_id, content, metadata, vector_content FROM {} WHERE record_id IN ({})"
                            .format(metadata_table, record_identifiers_filter))
 
         metadata_select_result = connection.execute(text(metadata_select))
         metadata_results = metadata_select_result.fetchall()
 
-        final_results: list[dict] = []
+        final_results: list[VectorSearchResult] = []
 
         result_map: dict = {}
 
         for metadata_row in metadata_results:
             record_id = int(metadata_row[0])
             lookup_key = str(metadata_row[0])
-            metadata_object = {"id": record_id, "content": metadata_row[1], "metadata": metadata_row[2]}
+            vector_content = json.loads(metadata_row[3])
+            metadata_object = {"id": record_id, "content": metadata_row[1],
+                               "metadata": metadata_row[2], "vector_content": vector_content}
             result_map[lookup_key] = metadata_object
 
         for score_object in scoring_results:
             identifier = str(score_object["record_id"])
             row = result_map[identifier]
             row.update(score_object)
             final_results.append(row)
 
         return final_results
 
     @abstractmethod
+    def truncate_tables(self):
+        """
+        Deletes all the records from the vector search tables
+        :return:
+        """
+        pass
+
+    @abstractmethod
+    def delete_by_id(self, record_id: int):
+        """
+        Deletes a specific record from the vector search tables
+        :param record_id:
+        :return:
+        """
+        pass
+
+    @abstractmethod
     def insert_row(self, content: str, metadata: dict, embeddings: list[float]):
         """
         Inserts data into the vector store
 
         :param content: the string content to be inserted
         :param metadata: a dictionary containing the metadata associated with the content
         :param embeddings: a vector representation of the content to be stored in the vector store
         :return:
         """
         pass
 
     @abstractmethod
     def compute_similarity(self, embedding_vectors: list[float], similarity_operation: DistanceMetric, k: int = 4,
-                           filters: Optional[dict[str, object]] = None):
+                           filters: Optional[dict[str, object]] = None) -> list[VectorSearchResult]:
         """
         Computes the Similarity Metric between the query vector and the records in the vector store
 
         :param embedding_vectors: The query vector
         :param similarity_operation: The similarity operation to be performed on the query vector
         :param k: the number of nearest neighbors to return
         :param filters: the dictionary containing the filters to be matched with the metadata
         :return:
         """
         pass
 
     @abstractmethod
     def cosine_similarity(self, embedding_vectors: list[float], k: int = 4,
-                          filters: Optional[dict[str, object]] = None):
+                          filters: Optional[dict[str, object]] = None) -> list[VectorSearchResult]:
         """
         Computes the Cosine Similarity between the query vector and the records in the vector store
 
         :param embedding_vectors: The query vector
         :param k: the number of nearest neighbors to return
         :param filters: the dictionary containing the filters to be matched with the metadata
         :return:
         """
         pass
 
     @abstractmethod
     def inner_product(self, embedding_vectors: list[float], k: int = 4,
-                      filters: Optional[dict[str, object]] = None):
+                      filters: Optional[dict[str, object]] = None) -> list[VectorSearchResult]:
         """
         Computes the Inner or Dot Product between the query vector and the records in the vector store
 
         :param embedding_vectors: The query vector
         :param k: the number of nearest neighbors to return
         :param filters: the dictionary containing the filters to be matched with the metadata
         :return:
         """
+
     @abstractmethod
     def euclidean_distance(self, embedding_vectors: list[float], k: int = 4,
-                           filters: Optional[dict[str, object]] = None):
+                           filters: Optional[dict[str, object]] = None) -> list[VectorSearchResult]:
         """
         Computes the Euclidean Distance between the query vector and the records in the vector store
 
         :param embedding_vectors: The query vector
         :param k: the number of nearest neighbors to return
         :param filters: the dictionary containing the filters to be matched with the metadata
         :return:
```

### Comparing `azure_sql_vector_search-0.8.1/setup.py` & `azure_sql_vector_search-0.8.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     project_long_description = readme_file.read()
 
 project_description = "Azure SQL Vector Search Clients"
 
+PROJECT_VERSION: str = "0.8.3"
+
 setup(
     name='azure_sql_vector_search',
-    version='0.8.1',
+    version=PROJECT_VERSION,
     author='Microsoft Corporation',
     url="https://github.com/projectAcetylcholine/sql_vector_search",
     packages=find_packages(),
     install_requires=['pyodbc >= 5.1.0', 'sqlalchemy >= 2.0.30', 'numpy >= 1.26.4'],
     license='MIT License',
     description=project_description,
     keywords="azure sql vector search langchain",
```

