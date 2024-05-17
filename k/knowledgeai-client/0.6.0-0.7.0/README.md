# Comparing `tmp/knowledgeai_client-0.6.0.tar.gz` & `tmp/knowledgeai_client-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledgeai_client-0.6.0.tar", max compression
+gzip compressed data, was "knowledgeai_client-0.7.0.tar", max compression
```

## Comparing `knowledgeai_client-0.6.0.tar` & `knowledgeai_client-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1080 2024-02-12 12:45:05.581822 knowledgeai_client-0.6.0/LICENSE
--rw-r--r--   0        0        0     8299 2024-05-03 13:30:46.094584 knowledgeai_client-0.6.0/README.md
--rw-r--r--   0        0        0        0 2024-02-12 12:45:05.582349 knowledgeai_client-0.6.0/knowledgeai/__init__.py
--rw-r--r--   0        0        0      392 2024-05-03 13:30:46.093735 knowledgeai_client-0.6.0/knowledgeai/client/__init__.py
--rw-r--r--   0        0        0     5929 2024-05-03 12:23:23.809674 knowledgeai_client-0.6.0/knowledgeai/client/admin.py
--rw-r--r--   0        0        0    15766 2024-05-03 13:11:24.310541 knowledgeai_client-0.6.0/knowledgeai/client/client.py
--rw-r--r--   0        0        0     2044 2024-04-19 15:19:14.290191 knowledgeai_client-0.6.0/knowledgeai/client/schema.py
--rw-r--r--   0        0        0     4252 2024-05-03 13:30:46.066456 knowledgeai_client-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     9126 1970-01-01 00:00:00.000000 knowledgeai_client-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-02-12 12:45:05.581822 knowledgeai_client-0.7.0/LICENSE
+-rw-r--r--   0        0        0     8366 2024-05-17 14:46:26.223813 knowledgeai_client-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2024-02-12 12:45:05.582349 knowledgeai_client-0.7.0/knowledgeai/__init__.py
+-rw-r--r--   0        0        0      449 2024-05-17 14:45:24.896734 knowledgeai_client-0.7.0/knowledgeai/client/__init__.py
+-rw-r--r--   0        0        0     5922 2024-05-17 13:27:26.218370 knowledgeai_client-0.7.0/knowledgeai/client/admin.py
+-rw-r--r--   0        0        0    16369 2024-05-17 14:03:12.369118 knowledgeai_client-0.7.0/knowledgeai/client/client.py
+-rw-r--r--   0        0        0     2396 2024-05-17 14:02:19.703976 knowledgeai_client-0.7.0/knowledgeai/client/schema.py
+-rw-r--r--   0        0        0     4184 2024-05-17 14:45:24.866573 knowledgeai_client-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     9193 1970-01-01 00:00:00.000000 knowledgeai_client-0.7.0/PKG-INFO
```

### Comparing `knowledgeai_client-0.6.0/LICENSE` & `knowledgeai_client-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `knowledgeai_client-0.6.0/README.md` & `knowledgeai_client-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 
 # Avvia Intelligence - KnowledgeAI Python Client
 
-Version: 0.6.0, (c) 2024 Arvato Systems
+Version: 0.7.0, (c) 2024 Arvato Systems
 
 This library is designed to provide easy access to the KnowledgeAI backend service. It enables users to manage projects, upload documents, and perform various tasks programmatically. The client offers an intuitive interface for seamless integration into Python applications.
 
+## IMPORTANT
+
+Version 0.7.0 requires a **server version > 1.1.0**
+
 ## Installation
 ```bash
 pip install knowledgeai-client
 ```
 ```bash
 poetry add knowledgeai-client
 ```
```

### Comparing `knowledgeai_client-0.6.0/knowledgeai/client/admin.py` & `knowledgeai_client-0.7.0/knowledgeai/client/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,34 +72,34 @@
             HTTPError: If the HTTP request returned an unsuccessful status code.
 
         Example:
             >>> from knowledgeai.schema import IsoLanguage, LLM, Plan, User
             >>> user = User(
             ...     name="pytest",
             ...     company="pytest",
-            ...     language=IsoLanguage.ENGLISH,
+            ...     contact="pytest",
             ...     plan=Plan.BASIC,
-            ...     llm=LLM.OPENAI,
+            ...     active=True,
             ... )
             >>> client.create_user(user)
         """
 
         url: str = self.url + "/admin/user"
         headers: dict[str, str] = {
             "accept": "application/json",
             "Authorization": self.api_key,
             "x-apikey": self.api_key,
             "Content-Type": "application/x-www-form-urlencoded",
         }
         data: dict[str, Any] = {
             "name": user.name,
             "company": user.company,
-            "language": user.language.value,
+            "contact": user.contact,
             "plan": user.plan.value,
-            "llm": user.llm.value,
+            "active": user.active,
         }
 
         response: Response = requests.post(
             url, headers=headers, data=data, timeout=self.timeout
         )
         response.raise_for_status()
         user_dict = json.loads(response.content)
@@ -159,17 +159,17 @@
             "x-apikey": self.api_key,
             "Content-Type": "application/x-www-form-urlencoded",
         }
         data = {
             "api_key": user.api_key,
             "name": user.name,
             "company": user.company,
-            "language": user.language.value,
+            "contact": user.contact if user.contact else "",
             "plan": user.plan.value,
-            "llm": user.llm.value,
+            "active": user.active,
         }
 
         response: Response = requests.put(
             url, headers=headers, data=data, timeout=self.timeout
         )
         response.raise_for_status()
         return User(**response.json())
```

### Comparing `knowledgeai_client-0.6.0/knowledgeai/client/client.py` & `knowledgeai_client-0.7.0/knowledgeai/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 import magic
 from httpx import Response
 from tqdm import tqdm
 
 from knowledgeai.client import (
     LLM,
     AskResponse,
+    DistanceStrategy,
     HttpMethod,
     IsoLanguage,
     Project,
     ProjectConfigKey,
     RetrievedDocument,
     Retriever,
+    SearchType,
     SourceDocument,
 )
 
 log: logging.Logger = logging.getLogger(__name__)
 limits = httpx.Limits(max_keepalive_connections=20, max_connections=None)
 
 
@@ -329,15 +331,14 @@
         """
         url: str = "/project/create"
 
         data: dict[str, str] = {
             "name": project_name,
             "language": language.value,
             "llm": llm.value,
-            "prompt": "x",
         }
 
         if prompt:
             data["prompt"] = prompt
 
         response: Response = self._api_call(HttpMethod.POST, url, data=data)
         project = response.json()
@@ -364,15 +365,15 @@
         """
 
         url: str = "/project/" + str(project.id)
         data = {
             "project_id": project.id,
             "name": project.name,
             "language": project.language.value,
-            "model": project.model.value,
+            "llm": project.llm.value,
             "prompt": project.prompt,
         }
 
         return self._api_call(HttpMethod.PUT, url, data=data)
 
     def update_project_configuration(
         self, project_id: int, key: ProjectConfigKey, value: str
@@ -457,15 +458,25 @@
             question=content["question"],
             answer=content["answer"],
             source_paragraphs=content["source_paragraphs"],
             source_documents=references,
         )
 
     def retrieve(
-        self, project_id: int, query: str, retrieval_type: Retriever = Retriever.default
+        self,
+        project_id: int,
+        query: str,
+        retriever_type: Retriever = Retriever.default,
+        search_type: SearchType = SearchType.MMR,
+        lambda_mult: float = 0.5,
+        top_k: int = 20,
+        top_n: int = 10,
+        semantic_weight: float = 0.5,
+        fulltext_weight: float = 0.5,
+        distance_strategy: DistanceStrategy = DistanceStrategy.COSINE,
     ) -> list[RetrievedDocument]:
         """Retrieves documents for the specified project.
 
         Args:
 
             project_id (int):
                 The ID of the project to retrieve documents from.
@@ -482,19 +493,26 @@
             requests.exceptions.RequestException: If an error occurs.
 
         Example:
             >>> references = client.retrieve(1, "What is the capital of Germany?")
             >>> for reference in references:
             ...     print(reference.content)
         """
-        url: str = "/index/retrieve"
+        url: str = "/retrieve"
         data = {
             "project_id": project_id,
             "query": query,
-            "retriever_type": retrieval_type.value,
+            "retriever_type": retriever_type.value,
+            "search_type": search_type.value,
+            "lambda_mult": lambda_mult,
+            "top_k": top_k,
+            "top_n": top_n,
+            "semantic_weight": semantic_weight,
+            "fulltext_weight": fulltext_weight,
+            "distance_strategy": distance_strategy.value,
         }
 
         response: Response = self._api_call(HttpMethod.POST, url, data=data)
         content = json.loads(response.content)
 
         references: list[RetrievedDocument] = [
             RetrievedDocument(**reference) for reference in content["documents"]
```

### Comparing `knowledgeai_client-0.6.0/knowledgeai/client/schema.py` & `knowledgeai_client-0.7.0/knowledgeai/client/schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from enum import StrEnum
-from typing import Any, List
+from typing import Any
 
 import iso639
 from pydantic import BaseModel, Field
 
 
 class HttpMethod(StrEnum):
     GET = "GET"
     POST = "POST"
     PUT = "PUT"
     DELETE = "DELETE"
 
 
 class ProjectConfigKey(StrEnum):
     BOTSERVICE_APP_ID = "botservice_app_id"
-    BOTSERVICE_APP_PASSWORD = "botservice_app_pwd"  # pragma: allowlist secret
-    BOTSERVICE_SECRET = "botservice_secret"  # pragma: allowlist secret
+    BOTSERVICE_APP_PASSWORD = (
+        "botservice_app_pwd"  # pragma: allowlist secret # noqa S105
+    )
+    BOTSERVICE_SECRET = "botservice_secret"  # pragma: allowlist secret # noqa S105
     WELCOME_MESSAGE = "welcome_message"
     # TODO: eventually add the model configuration parameters here
 
 
 class Plan(StrEnum):
     FREE = "Free"
     BASIC = "Basic"
@@ -34,57 +36,76 @@
 
 class LLM(StrEnum):
     OPENAI = "OpenAI"
     GOOGLE = "Google"
     ANTHROPIC = "Anthropic"
 
 
+class RetrieverType(StrEnum):
+    DEFAULT = "default"
+    MULTIQUERY = "multiquery"
+    COMPRESSION = "compression"
+
+
+class SearchType(StrEnum):
+    MMR = "mmr"
+    SIMILARITY = "similarity"
+
+
+class DistanceStrategy(StrEnum):
+    """Enumerator of the Distance strategies."""
+
+    EUCLIDEAN = "l2"
+    COSINE = "cosine"
+    MAX_INNER_PRODUCT = "inner"
+
+
 class User(BaseModel):
     id: int = Field(default=0)
     api_key: str = Field(default="")
     name: str
     company: str
-    language: IsoLanguage = Field(default=IsoLanguage.GERMAN)
+    contact: str | None = None
     plan: Plan = Field(default=Plan.BASIC)
-    llm: LLM = Field(default=LLM.OPENAI)
+    active: bool = Field(default=True)
 
 
 class ProjectDocument(BaseModel):
     project_id: int
     id: int
     name: str
     hash: str
 
 
 class Project(BaseModel):
     id: int
     name: str
     language: IsoLanguage = Field(default=IsoLanguage.GERMAN)
-    model: LLM = Field(default=LLM.OPENAI)
+    llm: LLM = Field(default=LLM.OPENAI)
     prompt: str | None = None
 
     number_of_documents: int = 0
     storage_size: int = 0
 
-    documents: List[ProjectDocument] = []
+    documents: list[ProjectDocument] = []
     configuration: dict[str, str] = {}
 
 
 class SourceDocument(BaseModel):
     page: str
     content: str
     source: str
     title: str
 
 
 class AskResponse(BaseModel):
     question: str
     answer: str
-    source_paragraphs: List[str]
-    source_documents: List[SourceDocument]
+    source_paragraphs: list[str]
+    source_documents: list[SourceDocument]
 
 
 class Retriever(StrEnum):
     default = "default"
     multiquery = "multiquery"
     compression = "compression"
```

### Comparing `knowledgeai_client-0.6.0/pyproject.toml` & `knowledgeai_client-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "A python client for the Avvia Intelligence - Knowledge AI Rest API"
 homepage    = "https://github.com/arvato-systems-aila-solutions/KnowledgeAI-Python-Client"
 keywords    = ["AI", "Knowledge Retrieval", "arvato systems", "avvia intelligence", "knowledgeai"]
 license     = "MIT"
 name        = "knowledgeai-client"
 packages    = [{ include = "knowledgeai", from = "." }]
 readme      = "README.md"
-version     = "0.6.0"
+version     = "0.7.0"
 
 [tool.poetry.dependencies]
 python = ">=3.11"
 
 httpx             = "0.27.0"
 pydantic          = "2.7.0"
 pydantic-settings = "2.2.1"
@@ -49,15 +49,14 @@
 extend-exclude = [".cache", ".venv", ".venv.mac", "build", "dist"]
 ignore = [
     "PT011",   # pytest-raises-too-broad
     "PT012",   # pytest.raises() block should contain a single simple statement
     "ISC001",  # Implicit string concatenation
     "PLR0913", # Too many arguments in function
     "RUF100",  # unused noqa
-    "N805",    # First argument of a method should be named `self`"
     "N818",    # Exception name {name} should be named with an Error suffix
     "N811",    # Constant {name} imported as non-constant {asname}
     "RUF012",  # Mutable class attributes should be annotated with typing.ClassVar
     "SIM300",  # Yoda conditions are discouraged, use {suggestion} instead
     "C",
 ]
 select = [
```

### Comparing `knowledgeai_client-0.6.0/PKG-INFO` & `knowledgeai_client-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgeai-client
-Version: 0.6.0
+Version: 0.7.0
 Summary: A python client for the Avvia Intelligence - Knowledge AI Rest API
 Home-page: https://github.com/arvato-systems-aila-solutions/KnowledgeAI-Python-Client
 License: MIT
 Keywords: AI,Knowledge Retrieval,arvato systems,avvia intelligence,knowledgeai
 Author: Arvato Systems
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -18,18 +18,22 @@
 Requires-Dist: python-magic (==0.4.27)
 Requires-Dist: tqdm (==4.66.2)
 Description-Content-Type: text/markdown
 
 
 # Avvia Intelligence - KnowledgeAI Python Client
 
-Version: 0.6.0, (c) 2024 Arvato Systems
+Version: 0.7.0, (c) 2024 Arvato Systems
 
 This library is designed to provide easy access to the KnowledgeAI backend service. It enables users to manage projects, upload documents, and perform various tasks programmatically. The client offers an intuitive interface for seamless integration into Python applications.
 
+## IMPORTANT
+
+Version 0.7.0 requires a **server version > 1.1.0**
+
 ## Installation
 ```bash
 pip install knowledgeai-client
 ```
 ```bash
 poetry add knowledgeai-client
 ```
```

