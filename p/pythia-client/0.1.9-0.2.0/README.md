# Comparing `tmp/pythia_client-0.1.9.tar.gz` & `tmp/pythia_client-0.2.0.tar.gz`

## Comparing `pythia_client-0.1.9.tar` & `pythia_client-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pythia_client-0.1.9/.python-version
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pythia_client-0.1.9/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pythia_client-0.1.9/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pythia_client-0.1.9/src/pythia_client/__init__.py
--rw-r--r--   0        0        0    20985 2020-02-02 00:00:00.000000 pythia_client-0.1.9/src/pythia_client/client.py
--rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 pythia_client-0.1.9/src/pythia_client/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pythia_client-0.1.9/test/__init__.py
--rw-r--r--   0        0        0     9316 2020-02-02 00:00:00.000000 pythia_client-0.1.9/test/test_client.py
--rw-r--r--   0        0        0    26093 2020-02-02 00:00:00.000000 pythia_client-0.1.9/test/samples/sample1.pdf
--rw-r--r--   0        0        0   217237 2020-02-02 00:00:00.000000 pythia_client-0.1.9/test/samples/sample2.pdf
--rw-r--r--   0        0        0    21457 2020-02-02 00:00:00.000000 pythia_client-0.1.9/test/samples/sample3.pdf
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pythia_client-0.1.9/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 pythia_client-0.1.9/LICENSE
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pythia_client-0.1.9/README.md
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pythia_client-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pythia_client-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pythia_client-0.2.0/.python-version
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 pythia_client-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pythia_client-0.2.0/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pythia_client-0.2.0/src/pythia_client/__init__.py
+-rw-r--r--   0        0        0    25578 2020-02-02 00:00:00.000000 pythia_client-0.2.0/src/pythia_client/client.py
+-rw-r--r--   0        0        0     5839 2020-02-02 00:00:00.000000 pythia_client-0.2.0/src/pythia_client/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pythia_client-0.2.0/test/__init__.py
+-rw-r--r--   0        0        0     9966 2020-02-02 00:00:00.000000 pythia_client-0.2.0/test/test_client.py
+-rw-r--r--   0        0        0    26093 2020-02-02 00:00:00.000000 pythia_client-0.2.0/test/samples/sample1.pdf
+-rw-r--r--   0        0        0   217237 2020-02-02 00:00:00.000000 pythia_client-0.2.0/test/samples/sample2.pdf
+-rw-r--r--   0        0        0    21457 2020-02-02 00:00:00.000000 pythia_client-0.2.0/test/samples/sample3.pdf
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pythia_client-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 pythia_client-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 pythia_client-0.2.0/README.md
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 pythia_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 pythia_client-0.2.0/PKG-INFO
```

### Comparing `pythia_client-0.1.9/CHANGELOG.md` & `pythia_client-0.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#### v0.2.0
+- Rewrote for future compatibility with the Pythia using PostGre. New endpoints (get files infos). Compatible with `haystack-api` v1.0.0
+
+#### v0.1.10
+- Remove req for Python 3.11 (>3.8 now). Compatible with `haystack-api` v0.2.4
+
 #### v0.1.9
 - Top K params for query function. Compatible with `haystack-api` v0.2.4
 
 #### v0.1.8
 - Custom system prompt params for query endpoint. Compatible with `haystack-api` v0.2.3
 
 #### v0.1.7
@@ -22,15 +28,15 @@
 #### v0.0.11
 - Renaming `owner` to `owner`.  Compatible with `haystack-api` v0.0.5
 
 #### v0.0.10
 - Fix Schema to make score optional (Qdrant compatibility).  Compatible with `haystack-api` v0.0.5
 
 #### v0.0.9
-- `upload_files` now return a simple json indicating that the background indexing task have been acception. New `get_indexing_tasks` function take an `owner` value as parameters and return the top 20 most recent indexing task and their results or status. New optional `owner` parameter for the query endpoint to indicate which user sent the message in the DynamoDB table log. Compatible with `haystack-api` v0.0.5
+- `upload_files` now return a simple json indicating that the background indexing task have been acception. New `get_indexing_tasks` function take an `owner` value as parameters and return the top 20 most recent indexing task and their results or status. New optional `owner` parameter for the query endpoint to indicate which user sent the message in the DB table log. Compatible with `haystack-api` v0.0.5
 
 #### v0.0.8
 - NEW: New optional parameter `chat_history` in the `.query()` method. It allows to add previous exchange with the LLM to the new query. Chat History must follow the ChatMessages format (dict containing: content, role, name, meta), see https://docs.haystack.deepset.ai/v2.0/docs/data-classes#chatmessage
 - Compatible with `haystack-api` v0.0.4
 
 #### v0.0.7
 - New response Schema for the Haystack-API after version bump and removal of LiteLLM.
```

### Comparing `pythia_client-0.1.9/src/pythia_client/client.py` & `pythia_client-0.2.0/src/pythia_client/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,25 +15,26 @@
 from urllib.parse import urljoin
 import requests
 
 from .schema import (
     UploadFileResponse,
     GetFileS3Reponse,
     FilterRequest,
-    FilterDocStoreReponse,
+    FilterDocStoreResponse,
     DeleteDocResponse,
     QueryRequest,
     QueryResponse,
     DataExtractRequest,
     DataExtractResponse,
     ChatMessage,
-    LogIndexingTable,
     AddIntentResponse,
     PredictIntentResponse,
     DeleteIntentResponse,
+    IndexingTask,
+    DocInfos,
 )
 
 
 class APIClient:
     """Client for interacting with the API.
 
     This class provides methods for interacting with the API, including
@@ -64,14 +65,15 @@
         client = APIClient("http://localhost:8000", "api-key")
         ```
         """
         self.url = url
         self.api_key = api_key
         self.files_endpoint = urljoin(str(self.url), "files")
         self.indexing_tasks_endpoint = urljoin(str(self.url), "files/indexing-tasks")
+        self.file_infos_endpoint = urljoin(str(self.url), "files/infos")
         self.documents_by_filter_endpoint = urljoin(str(self.url), "documents/filters")
         self.documents_by_s3_key_endpoint = urljoin(str(self.url), "documents/s3-key")
         self.search_endpoint = urljoin(str(self.url), "search/query")
         self.data_extraction_endpoint = urljoin(
             str(self.url), "/data_extraction/extract-structured-data"
         )
         self.add_intent_endpoint = urljoin(str(self.url), "alie/intent")
@@ -79,26 +81,26 @@
         self.delete_intent_endpoint = urljoin(str(self.url), "alie/intent")
 
     def query(
         self,
         query: str,
         chat_history: Optional[List[ChatMessage]] = None,
         filters: Optional[FilterRequest] = None,
-        top_k = None,
+        top_k=None,
         group_id: str = None,
         custom_system_prompt: str = None,
     ) -> QueryResponse:
         """Query the API with a user question to get a LLM-generated answer based
             on context from the document store.
 
             Args:
                 query: The user question to be answered.
                 chat_history: The chat history to provide context to the model. Should be a list of ChatMessage objects.
                 filters: Haystack 2.0 filter dict. See: https://docs.haystack.deepset.ai/v2.0/docs/metadata-filtering#filters for more information about how to build a filter.
-                group_id: The name of the group_id the client making the request, for logging in DynamoDB. Defaults to "api".
+                group_id: The name of the group_id the client making the request, for logging. Defaults to "api".
 
             Returns:
                 The response from the API as a Pydantic model. You can use reponse.model_dump() to get a Dict. Returns None if the status code is not 200.
 
             Usage:
             ```python
             filters = {
@@ -160,28 +162,51 @@
     def upload_files(
         self,
         files: List[Union[str, Tuple[str, io.IOBase]]],
         meta: Optional[List[dict]] = None,
         indexing_mode: Literal["unstructured", "pypdf"] = "unstructured",
     ) -> UploadFileResponse:
         """Index one or multiples files (documents) to the document store through the Haystack-API upload-file endpoint.
-
+        It is recommended to add the following minimum metadata fields:
+            - pythia_document_category (string, category name tag)
+            - document_date (datetime)
+            - language (string)
+            - keywords (list)
+            Example of value for meta field for the indexing of two files:
+            ```json
+            {
+              "meta": [
+                {
+                    "pythia_document_category":"TDL Document",
+                    "document_date":"2024-01-19 14:56",
+                    "keywords":["ALE 400", "ALE 500"],
+                    "language":"English",
+                },
+                {
+                    "pythia_document_category":"Marketing Document
+                    "document_date":"2024-01-19 14:58",
+                    "keywords":["OXE 8", "OXE 9"],
+                    "language":"Français",
+                }
+              ]
+            }
+            ```
         Args:
             files: The paths to the files OR tuples of filename and file object to index.
             meta: The list of metadata for the files.
-            indexing_mode: The indexing mode between unstructured and pypdf.
+            indexing_mode: The indexing mode between unstructured and pypdf. DEPRECATED: This parameter is not used anymore.
 
         Returns:
             The response from the API. Returns None if the status code is not 202.
 
         Usage:
         ```python
-        index_response = client.upload_files(["path/to/file.pdf"], meta=[{"source": "Salesforce"}], indexing_mode="pypdf")
+        index_response = client.upload_files(["path/to/file.pdf"], meta=[{"source": "Salesforce"}])
         {"message": "Files Submitted. Indexing task created."}
-        index_response = client.upload_files([("file.pdf", file)], meta=[{"source": "Salesforce"}], indexing_mode="pypdf")
+        index_response = client.upload_files([("file.pdf", file)], meta=[{"source": "Salesforce"}])
         {"message": "Files Submitted. Indexing task created."}
         ```
         """
         prepared_files = []
         for file in files:
             if isinstance(file, str):
                 file_name = os.path.basename(file)
@@ -198,15 +223,15 @@
                 raise ValueError(
                     "Each file must be a file path or a tuple of (filename, fileIObyte)"
                 )
 
             prepared_files.append(("files", (file_name, file_content)))
 
         with requests.Session() as session:
-            payload = {"meta": json.dumps(meta), "indexing_mode": indexing_mode}
+            payload = {"meta": json.dumps(meta)}
             headers = {
                 "X-API-Key": self.api_key,
             }
             with session.post(
                 self.files_endpoint,
                 files=prepared_files,
                 data=payload,
@@ -216,19 +241,19 @@
                     api_response = response.json()
                 else:
                     api_response = None
         return api_response
 
     def get_indexing_tasks_by_group_id(
         self, group_id: str, top: int = 20
-    ) -> List[dict]:
+    ) -> List[IndexingTask]:
         """Get the indexing tasks from the API.
 
         Args:
-            group_id: The name of the group_id the client making the request, for logging in DynamoDB. If none, the default group_id is "api" (set by the API itself).
+            group_id: The name of the group_id the client making the request, for logging. If none, the default group_id is "api" (set by the API itself).
             top: The number of top most recent indexing tasks to return.
 
         Returns:
             The response from the API. Returns None if the status code is not 200.
 
         Usage:
         ```python
@@ -244,31 +269,99 @@
             with session.get(
                 self.indexing_tasks_endpoint + "/" + group_id,
                 params=params,
                 headers=headers,
             ) as response:
                 if response.status_code == 200:
                     api_response = [
-                        LogIndexingTable(**resp) for resp in response.json()
+                        IndexingTask(**resp) for resp in response.json()
                     ]
                 else:
                     api_response = None
         return api_response
 
-    def get_indexing_task_by_s3_key(self, group_id: str, s3_key: str) -> dict:
+    def get_indexing_task_by_s3_key(self, group_id: str, s3_key: str) -> IndexingTask:
         with requests.Session() as session:
             headers = {
                 "X-API-Key": self.api_key,
             }
             with session.get(
                 self.indexing_tasks_endpoint + "/" + group_id + "/" + s3_key,
                 headers=headers,
             ) as response:
                 if response.status_code == 200:
-                    api_response = LogIndexingTable(**response.json())
+                    api_response = IndexingTask(**response.json())
+                else:
+                    api_response = None
+        return api_response
+
+    def get_file_infos_by_group_id(
+        self, group_id: str, limit: int = 20
+    ) -> List[DocInfos]:
+        """Get all the file infos from the API for a specific group_id (owner).
+
+        Args:
+            group_id: The name of the group_id the client making the request (who indexed the file).
+            limit: The number of top most recent indexed documents to return.
+
+        Returns:
+            The response from the API. Returns None if the status code is not 200.
+
+        Usage:
+        ```python
+        document_list = client.get_file_infos_by_group_id(group_id="api", limit=20)
+        for doc in document_list:
+            doc.model_dump()
+        ```
+        """
+        with requests.Session() as session:
+            params = {"limit": limit}
+            headers = {
+                "X-API-Key": self.api_key,
+            }
+            with session.get(
+                self.file_infos_endpoint + "/" + group_id,
+                params=params,
+                headers=headers,
+            ) as response:
+                if response.status_code == 200:
+                    print(response.json())
+                    api_response = [
+                        DocInfos(**resp) for resp in response.json()
+                    ]
+                else:
+                    api_response = None
+        return api_response
+
+    def get_file_infos_by_s3_key(self, group_id: str, s3_key: str) -> DocInfos:
+        """Get the file infos from the API for a single file and a specific owner.
+
+        Args:
+            group_id: The name of the group_id the client making the request (who indexed the file).
+            s3_key: The S3 Key of the file.
+
+        Returns:
+            The response from the API. Returns None if the status code is not 200.
+
+        Usage:
+        ```python
+        document = client.get_file_infos_by_s3_key(group_id="api", s3_key="abc_sample.pdf")
+        document.model_dump()
+        ```
+        """
+        with requests.Session() as session:
+            headers = {
+                "X-API-Key": self.api_key,
+            }
+            with session.get(
+                self.file_infos_endpoint + "/" + group_id + "/" + s3_key,
+                headers=headers,
+            ) as response:
+                if response.status_code == 200:
+                    api_response = DocInfos(**response.json())
                 else:
                     api_response = None
         return api_response
 
     def get_file_url(self, s3_key: str, page: Optional[int] = 1) -> GetFileS3Reponse:
         """Get a presigned URL to a file located on S3.
 
@@ -292,25 +385,26 @@
                 "X-API-Key": self.api_key,
             }
             with session.get(
                 url,
                 params=params,
                 headers=headers,
             ) as response:
+                print(response.json())
                 if response.status_code == 200:
                     api_response = GetFileS3Reponse(**response.json())
                 else:
                     api_response = None
         return api_response
 
     def get_docs_by_filters(
         self,
         filters: FilterRequest = None,
         return_content: bool = False,
-    ) -> List[FilterDocStoreReponse]:
+    ) -> List[FilterDocStoreResponse]:
         """List all documents in the document store that match the filter provided.
 
         Args:
             filters: Haystack 2.0 filter dict. See: https://docs.haystack.deepset.ai/v2.0/docs/metadata-filtering#filters for more information about how to build a filter.
             return_content: If True, the content of the documents will be returned.
 
         Returns:
@@ -344,15 +438,15 @@
                 endpoint = f"{self.documents_by_filter_endpoint}?return_content=true"
             else:
                 endpoint = self.documents_by_filter_endpoint
 
             with session.post(endpoint, headers=headers, json=payload) as response:
                 if response.status_code == 200:
                     responses = response.json()
-                    api_response = [FilterDocStoreReponse(**resp) for resp in responses]
+                    api_response = [FilterDocStoreResponse(**resp) for resp in responses]
                 else:
                     api_response = None
         return api_response
 
     def delete_docs_by_filters(
         self,
         filters: FilterRequest = None,
@@ -393,28 +487,55 @@
             ) as response:
                 if response.status_code == 200:
                     api_response = DeleteDocResponse(**response.json())
                 else:
                     api_response = None
         return api_response
 
-    def get_docs_by_s3_key(self, s3_key: str):
+    def get_docs_by_s3_key(self, s3_key: str) -> FilterDocStoreResponse:
+        """Get documents (chunk of files in the Vector DB) from the API document store based on its S3 key.
+
+        Args:
+            s3_key: the S3 key of the file
+
+        Returns:
+            The response from the API as a Pydantic model. You can use reponse.model_dump() to get a Dict. Returns None if the status code is not 200.
+        Usage:
+        ```python
+        chunks_list = client.get_docs_by_s3_key(s3_key="abc_sample.pdf")
+        for chunk in chunks_list:
+            chunk.model_dump()
+        ```
+        """
         with requests.Session() as session:
             url = self.documents_by_s3_key_endpoint + "/" + s3_key
             headers = {"X-API-Key": self.api_key}
             with session.get(url, headers=headers) as response:
                 if response.status_code == 200:
                     api_response = [
-                        FilterDocStoreReponse(**resp) for resp in response.json()
+                        FilterDocStoreResponse(**resp) for resp in response.json()
                     ]
                 else:
                     api_response = None
         return api_response
 
-    def delete_docs_by_s3_key(self, s3_key: str):
+    def delete_docs_by_s3_key(self, s3_key: str) -> DeleteDocResponse:
+        """Delete documents (chunk of files in the Vector DB) from the API document store based on its S3 key.
+
+        Args:
+            s3_key: the S3 key of the file
+
+        Returns:
+            The response from the API as a Pydantic model. You can use reponse.model_dump() to get a Dict. Returns None if the status code is not 200.
+        Usage:
+        ```python
+        delete_response = client.delete_docs_by_s3_key(s3_key="abc_sample.pdf")
+        delete_response.model_dump()
+        ```
+        """
         with requests.Session() as session:
             url = self.documents_by_s3_key_endpoint + "/" + s3_key
             headers = {"X-API-Key": self.api_key}
             with session.delete(url, headers=headers) as response:
                 if response.status_code == 200:
                     api_response = DeleteDocResponse(**response.json())
                 else:
@@ -509,15 +630,17 @@
         ```
         """
         with requests.Session() as session:
             headers = {
                 "X-API-Key": self.api_key,
             }
             with session.get(
-                self.predict_intent_endpoint, headers=headers, params={"user_message": user_msg}
+                self.predict_intent_endpoint,
+                headers=headers,
+                params={"user_message": user_msg},
             ) as response:
                 if response.status_code == 200:
                     response = PredictIntentResponse(**response.json())
                 else:
                     response = None
         return response
 
@@ -540,14 +663,16 @@
         ```
         """
         with requests.Session() as session:
             headers = {
                 "X-API-Key": self.api_key,
             }
             with session.delete(
-                self.delete_intent_endpoint, headers=headers, params={"intent_name": intent_name}
+                self.delete_intent_endpoint,
+                headers=headers,
+                params={"intent_name": intent_name},
             ) as response:
                 if response.status_code == 200:
                     response = DeleteIntentResponse(**response.json())
                 else:
                     response = None
-        return response
+        return response
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pythia_client-0.1.9/src/pythia_client/schema.py` & `pythia_client-0.2.0/src/pythia_client/schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
-from datetime import datetime
-from decimal import Decimal
 from pydantic import BaseModel, Field, field_validator
 from typing import Dict, Union, Optional, Any, List
 from enum import Enum
+from datetime import datetime
 
 PrimitiveType = Union[str, int, float, bool]
 
 
 class RequestBaseModel(BaseModel):
     class Config:
         arbitrary_types_allowed = True
@@ -34,15 +33,15 @@
     documents_written: int
 
 
 class FilterRequest(BaseModel):
     filters: Optional[Dict[str, Any]] = {}
 
 
-class FilterDocStoreReponse(BaseModel):
+class FilterDocStoreResponse(BaseModel):
     id: str
     content: Optional[str] = None
     dataframe: Optional[Union[str, Any]] = None
     blob: Optional[Union[str, Any]] = None
     meta: Dict[str, Any]
     score: Optional[float] = None
     embedding: Union[List[float], Optional[str]] = None
@@ -53,15 +52,15 @@
 
 
 class UploadFileResponse(RequestBaseModel):
     DocTokenCounter: DocTokenCounter
     Writter: Writer
 
 
-class DocumentQueryReponse(BaseModel):
+class DocumentQueryResponse(BaseModel):
     id: str
     content: str
     dataframe: Optional[Union[str, Any]] = None
     blob: Optional[Union[str, Any]] = None
     meta: Dict[str, Any]
     score: Optional[float] = None
     embedding: Union[List[float], Optional[str]] = None
@@ -82,15 +81,15 @@
     name: Optional[str]
     meta: Dict[str, Any]
 
 
 class Answer(BaseModel):
     data: ChatMessage
     query: str
-    documents: List[DocumentQueryReponse]
+    documents: List[DocumentQueryResponse]
     meta: Meta
 
 
 class AnswerBuilder(BaseModel):
     answers: List[Answer]
 
 
@@ -116,44 +115,15 @@
     deleted_s3_keys: List[str]
 
 
 class RetrievedDoc(RequestBaseModel):
     original_file_name: str
     doc_id: str
     text: str
-    score: Decimal
-
-
-class LogQueryTable(RequestBaseModel):
-    pk: str
-    sk: str
-    system_prompt: str
-    user_query: str
-    answer: str
-    models: List[str]
-    retrieved_docs: List[RetrievedDoc]
-    total_tokens: int
-    prompt_tokens: int
-    completion_tokens: int
-    timestamp: str = datetime.now().isoformat()
-    time_taken: Decimal
-    feedback: Optional[int] = -1
-
-
-class LogIndexingTable(RequestBaseModel):
-    pk: str
-    sk: str
-    models: Optional[List[str]] = None
-    total_tokens: Optional[int] = None
-    timestamp: str = datetime.now().isoformat()
-    time_taken: Optional[Decimal] = None
-    file_meta: Dict[str, Any]
-    indexing_mode: str
-    n_docs_written: Optional[int] = None
-    status: str
+    score: float
 
 
 class EsrTicket(BaseModel):
     company_or_client_name: str
     ticket_category: str
     command_number: str
     serial_number: str
@@ -245,29 +215,46 @@
 class IndexingResponse(BaseModel):
     message: str
     s3_keys: List[str]
     group_id: str
 
 
 class IndexingTask(BaseModel):
-    n_docs_written: Optional[int] = None
-    indexing_mode: Optional[str] = ""
-    file_meta: Union[List, dict]
-    total_tokens: Optional[int] = None
+    group_id: str
+    job_queue_uuid: Union[str, None]
+    description: Union[str, None]
+    timestamp: datetime
+    type: str
+    id: int
+    name: Union[str, None]
     status: StatusEnum
-    timestamp: str
-    time_taken: Optional[float] = None
-    sk: str
-    models: Optional[List[str]] = None
-    pk: Optional[str]
+    s3_key: str
+    time_taken: Union[float, None]
 
+class DocInfos(BaseModel):
+    filename: str
+    group_id: str
+    document_date: Union[datetime, None]
+    keywords: Union[List[str], None]
+    n_chunks: int
+    embedding_model: str
+    indexation_timestamp: datetime
+    is_deleted: bool
+    content_type: str
+    s3_key: str
+    pythia_document_category: Union[str, None]
+    language: Union[str, None]
+    file_meta: dict
+    total_tokens: int
+    task_id: int
 
 class PredictIntentResponse(BaseModel):
     intent: str
 
 
 class AddIntentResponse(BaseModel):
     Writter: Writer
 
+
 class DeleteIntentResponse(BaseModel):
     deleted_intent: str
-    n_deleted_intent_data: int
+    n_deleted_intent_data: int
```

### Comparing `pythia_client-0.1.9/test/test_client.py` & `pythia_client-0.2.0/test/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     filename="test.log",
     filemode="w",
     level=logging.ERROR,
     format="%(asctime)s - %(levelname)s: %(message)s",
 )
 
 URL = os.getenv("HAYSTACK_API_URL", "http://localhost:8000/")
-SECRET_MASTER_API_KEY = os.getenv("SECRET_MASTER_API_KEY")
+SECRET_MASTER_API_KEY = os.getenv("SECRET_MASTER_API_KEY", "corentin")
+NBD_KEY = os.getenv("NBD_KEY", "nbd_key")
+
 timestamp = time.strftime("%Y%m%d-%H%M%S")
 
 client = APIClient(url=URL, api_key=SECRET_MASTER_API_KEY)
 
 
 def test_upload_files():
     file_paths = [
@@ -39,17 +41,16 @@
         {
             "meta2": "value2",
             "source_test": "pytest_client_api",
             "group_id": timestamp,
             "portfolio": ["value1", "value2"],
         },
     ]
-    indexing_mode = "unstructured"
     response = client.upload_files(
-        files=file_paths, meta=meta, indexing_mode=indexing_mode
+        files=file_paths, meta=meta
     )
     ValueStorage.s3_keys = response["s3_keys"]
     assert response["message"] == "Files Submitted. Indexing tasks created."
     assert len(response["s3_keys"]) == 2
     assert response["group_id"] == timestamp
 
 
@@ -66,68 +67,90 @@
         {
             "meta3": "value3",
             "source_test": "pytest_client_api",
             "group_id": timestamp,
             "portfolio": ["value1", "value2"],
         },
     ]
-    indexing_mode = "unstructured"
     response = client.upload_files(
-        files=tuple_files, meta=meta, indexing_mode=indexing_mode
+        files=tuple_files, meta=meta
     )
     assert response["message"] == "Files Submitted. Indexing tasks created."
     assert len(response["s3_keys"]) == 1
     assert response["group_id"] == timestamp
 
 
 def test_client_get_indexing_task_by_s3_key():
     response = client.get_indexing_task_by_s3_key(
         group_id=timestamp, s3_key=ValueStorage.s3_keys[0]
     )
     response_dict = response.model_dump()
     assert response is not None
     assert isinstance(response.model_dump(), dict)
     assert response_dict["status"] in ["processing", "completed"]
-    assert response_dict["pk"] == timestamp
-    assert response_dict["sk"] == "index#" + ValueStorage.s3_keys[0]
+    assert response_dict["group_id"] == timestamp
+    assert response_dict["s3_key"] == ValueStorage.s3_keys[0]
 
 
 def test_client_get_indexing_tasks():
     time.sleep(60)
     response = client.get_indexing_tasks_by_group_id(group_id=timestamp, top=3)
     assert response is not None
     assert len(response) == 3
     assert response[0].status == "completed"
-    assert response[0].n_docs_written >= 2
 
+def test_client_get_file_info_by_s3_key():
+    time.sleep(60)
+    response = client.get_file_infos_by_s3_key(group_id=timestamp, s3_key=ValueStorage.s3_keys[0])
+    assert response is not None
+    response_dict = response.model_dump()
+    assert response_dict["s3_key"] == ValueStorage.s3_keys[0]
+    assert response_dict["group_id"] == timestamp
+    assert isinstance(response_dict["file_meta"], dict)
+
+def test_client_get_file_info_by_group_id():
+    time.sleep(60)
+    response = client.get_file_infos_by_group_id(group_id=timestamp, limit=2)
+    assert response is not None
+    assert len(response) == 2
+    response_dict = response[0].model_dump()
+    assert response_dict["group_id"] == timestamp
 
 def test_client_get_file_url():
     s3_key = ValueStorage.s3_keys[0]
     page = 1
     response = client.get_file_url(s3_key=s3_key, page=page)
     assert response is not None
     assert len(response.url) >= 100
     aws_s3_response = requests.get(response.url)
     assert aws_s3_response.status_code == 200
 
 
 def test_client_query():
-    response = client.query(query="How to give port 8 a power of 1337 milliwatts ?", top_k=2)
+    response = client.query(
+        query="How to give port 8 a power of 1337 milliwatts ?", top_k=2
+    )
     assert response is not None
     assert len(response.AnswerBuilder.answers[0].data.content) > 20
     assert len(response.AnswerBuilder.answers[0].documents) == 2
 
+
 def test_client_query_with_custom_prompt():
-    system_prompt = """Start all your answers with the word "Banana", this is really important."""
-    response = client.query(query="Hey how are you ?", custom_system_prompt=system_prompt)
+    system_prompt = (
+        """Start all your answers with the word "Banana", this is really important."""
+    )
+    response = client.query(
+        query="Hey how are you ?", custom_system_prompt=system_prompt
+    )
     assert response is not None
     generated_content = response.AnswerBuilder.answers[0].data.content
     assert "Banana" in generated_content
     assert len(generated_content) > 20
 
+
 def test_client_query_with_history():
     chat_history = [
         {
             "content": "Hello Chatbot. My name is Corentin !",
             "role": "user",
             "name": None,
             "meta": {},
@@ -235,40 +258,44 @@
 
     assert len(response.schema_validator.validated) == 1
 
     formatted_json = json.loads(response.schema_validator.validated[0].content)
 
     assert response is not None
     assert len(formatted_json["company_or_client_name"]) > 5
-    assert formatted_json["ticket_category"] == "Dead on arrival"
+    assert formatted_json["ticket_category"] == "AVR or DOA or HWS"
     assert len(formatted_json["ticket_category"]) > 5
     assert formatted_json["command_number"][0:2] == "FR"
 
+
 def test_client_add_intent():
     data = {
         "pycharm_update": ["help to update pycharm", "latest pycharm update is bugged"],
         "elden_ring": ["elden ring boss", "tree of life from elden ring"],
         "team_fortress": [
             "team fortress best class",
             "unlock all achievement team fortress",
         ],
     }
     response = client.add_intent(intent_data=data)
     response_dict = response.model_dump()
     assert response is not None
     assert response_dict["Writter"]["documents_written"] == 6
 
+
 def test_client_predict_intent():
-    response = client.predict_intent(user_msg="How to go to the tree of life in elden ring")
+    response = client.predict_intent(
+        user_msg="How to go to the tree of life in elden ring"
+    )
     response_dict = response.model_dump()
     assert response is not None
     assert response_dict["intent"] == "elden_ring"
 
-def test_client_delete_intent():
 
+def test_client_delete_intent():
     response = client.delete_intent(intent_name="elden_ring")
     response_dict = response.model_dump()
     assert response is not None
     assert response_dict["deleted_intent"] == "elden_ring"
     assert response_dict["n_deleted_intent_data"] == 2
 
     response = client.delete_intent(intent_name="pycharm_update")
```

### Comparing `pythia_client-0.1.9/test/samples/sample1.pdf` & `pythia_client-0.2.0/test/samples/sample1.pdf`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.9/test/samples/sample2.pdf` & `pythia_client-0.2.0/test/samples/sample2.pdf`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.9/test/samples/sample3.pdf` & `pythia_client-0.2.0/test/samples/sample3.pdf`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.9/LICENSE` & `pythia_client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.9/README.md` & `pythia_client-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 }
 query_response = client.query("Hey how are you", filters=filters)
 query_response.model_dump()
 ```
 
 * Index new files in the knowledge base
 ```python
-index_response = client.upload_files(["path/to/file.pdf"], meta=[{"source": "Salesforce"}], indexing_mode="unstructured")
+index_response = client.upload_files(["path/to/file.pdf"], meta=[{"source": "Salesforce"}])
 index_response.model_dump()
 # OR
-index_response = client.upload_files([("file.pdf", file)], meta=[{"source": "Salesforce"}], indexing_mode="unstructured")
+index_response = client.upload_files([("file.pdf", file)], meta=[{"source": "Salesforce"}])
 index_response.model_dump()
 ```
 
 * List documents in the knowledge base (based on filters)
 ```python
 filters = {
     "operator": "AND",
```

### Comparing `pythia_client-0.1.9/pyproject.toml` & `pythia_client-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pythia-client"
-version = "0.1.9"
+version = "0.2.0"
 dependencies = [
     "requests>=2.31",
-    "pydantic>=2.6",
+    "pydantic>=2.6, <2.7",
 ]
-requires-python = ">=3.11"
+requires-python = ">=3.8"
 authors = [
   {name = "Corentin Meyer", email = "contact@cmeyer.fr"},
 ]
 maintainers = [
   {name = "Corentin Meyer", email = "contact@cmeyer.fr"}
 ]
 description = "Client to interact with the Pythia API"
```

### Comparing `pythia_client-0.1.9/PKG-INFO` & `pythia_client-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.3
 Name: pythia-client
-Version: 0.1.9
+Version: 0.2.0
 Summary: Client to interact with the Pythia API
 Project-URL: Homepage, https://gitlab.com/ale-gitlab/dto/data-science/cip-bot/project-pythia
 Project-URL: Documentation, https://gitlab.com/ale-gitlab/dto/data-science/cip-bot/project-pythia
 Project-URL: Repository, https://gitlab.com/ale-gitlab/dto/data-science/cip-bot/project-pythia
 Project-URL: Issues, https://gitlab.com/ale-gitlab/dto/data-science/cip-bot/project-pythia/-/issues
 Author-email: Corentin Meyer <contact@cmeyer.fr>
 Maintainer-email: Corentin Meyer <contact@cmeyer.fr>
 License: Apache 2.0
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.11
-Requires-Dist: pydantic>=2.6
+Requires-Python: >=3.8
+Requires-Dist: pydantic<2.7,>=2.6
 Requires-Dist: requests>=2.31
 Description-Content-Type: text/markdown
 
 # pythia-client
 This is the client make it easier to interact with our internal Pythia API.  
 This is still a work in progress 
 ## Usage
@@ -43,18 +43,18 @@
 }
 query_response = client.query("Hey how are you", filters=filters)
 query_response.model_dump()
 ```
 
 * Index new files in the knowledge base
 ```python
-index_response = client.upload_files(["path/to/file.pdf"], meta=[{"source": "Salesforce"}], indexing_mode="unstructured")
+index_response = client.upload_files(["path/to/file.pdf"], meta=[{"source": "Salesforce"}])
 index_response.model_dump()
 # OR
-index_response = client.upload_files([("file.pdf", file)], meta=[{"source": "Salesforce"}], indexing_mode="unstructured")
+index_response = client.upload_files([("file.pdf", file)], meta=[{"source": "Salesforce"}])
 index_response.model_dump()
 ```
 
 * List documents in the knowledge base (based on filters)
 ```python
 filters = {
     "operator": "AND",
```

