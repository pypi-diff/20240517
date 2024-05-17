# Comparing `tmp/langchain_google_vertexai-1.0.3.tar.gz` & `tmp/langchain_google_vertexai-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_google_vertexai-1.0.3.tar", max compression
+gzip compressed data, was "langchain_google_vertexai-1.0.4.tar", max compression
```

## Comparing `langchain_google_vertexai-1.0.3.tar` & `langchain_google_vertexai-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1072 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/LICENSE
--rw-r--r--   0        0        0     2594 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/README.md
--rw-r--r--   0        0        0     1853 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/__init__.py
--rw-r--r--   0        0        0     3255 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/_anthropic_utils.py
--rw-r--r--   0        0        0    11995 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/_base.py
--rw-r--r--   0        0        0      151 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/_enums.py
--rw-r--r--   0        0        0     8169 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/_image_utils.py
--rw-r--r--   0        0        0     6623 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/_utils.py
--rw-r--r--   0        0        0     2511 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/callbacks.py
--rw-r--r--   0        0        0     6062 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/chains.py
--rw-r--r--   0        0        0    41816 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/chat_models.py
--rw-r--r--   0        0        0    16445 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/embeddings.py
--rw-r--r--   0        0        0     9948 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/functions_utils.py
--rw-r--r--   0        0        0    13960 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/gemma.py
--rw-r--r--   0        0        0    12145 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/llms.py
--rw-r--r--   0        0        0     8536 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/model_garden.py
--rw-r--r--   0        0        0        0 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/py.typed
--rw-r--r--   0        0        0      471 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/__init__.py
--rw-r--r--   0        0        0     4679 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/_sdk_manager.py
--rw-r--r--   0        0        0     6103 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/_searcher.py
--rw-r--r--   0        0        0     5436 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/_utils.py
--rw-r--r--   0        0        0     8050 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/document_storage.py
--rw-r--r--   0        0        0    15958 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/vectorstores.py
--rw-r--r--   0        0        0    18548 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/langchain_google_vertexai/vision_models.py
--rw-r--r--   0        0        0     3343 2024-05-01 15:31:52.754938 langchain_google_vertexai-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 langchain_google_vertexai-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-17 15:58:22.276395 langchain_google_vertexai-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2594 2024-05-17 15:58:22.276395 langchain_google_vertexai-1.0.4/README.md
+-rw-r--r--   0        0        0     2064 2024-05-17 15:58:22.276395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/__init__.py
+-rw-r--r--   0        0        0     3255 2024-05-17 15:58:22.276395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/_anthropic_utils.py
+-rw-r--r--   0        0        0    13944 2024-05-17 15:58:22.276395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/_base.py
+-rw-r--r--   0        0        0      151 2024-05-17 15:58:22.276395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/_enums.py
+-rw-r--r--   0        0        0     8383 2024-05-17 15:58:22.276395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/_image_utils.py
+-rw-r--r--   0        0        0     7667 2024-05-17 15:58:22.276395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/_utils.py
+-rw-r--r--   0        0        0     2511 2024-05-17 15:58:22.276395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/callbacks.py
+-rw-r--r--   0        0        0     6017 2024-05-17 15:58:22.276395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/chains.py
+-rw-r--r--   0        0        0    45651 2024-05-17 15:58:22.276395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/chat_models.py
+-rw-r--r--   0        0        0    16445 2024-05-17 15:58:22.276395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/embeddings.py
+-rw-r--r--   0        0        0    12843 2024-05-17 15:58:22.280395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/functions_utils.py
+-rw-r--r--   0        0        0    13960 2024-05-17 15:58:22.280395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/gemma.py
+-rw-r--r--   0        0        0    12191 2024-05-17 15:58:22.280395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/llms.py
+-rw-r--r--   0        0        0     8673 2024-05-17 15:58:22.280395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/model_garden.py
+-rw-r--r--   0        0        0        0 2024-05-17 15:58:22.280395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/py.typed
+-rw-r--r--   0        0        0      471 2024-05-17 15:58:22.280395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/vectorstores/__init__.py
+-rw-r--r--   0        0        0     4679 2024-05-17 15:58:22.280395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/vectorstores/_sdk_manager.py
+-rw-r--r--   0        0        0     6103 2024-05-17 15:58:22.280395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/vectorstores/_searcher.py
+-rw-r--r--   0        0        0     5436 2024-05-17 15:58:22.280395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/vectorstores/_utils.py
+-rw-r--r--   0        0        0     8050 2024-05-17 15:58:22.280395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/vectorstores/document_storage.py
+-rw-r--r--   0        0        0    15958 2024-05-17 15:58:22.280395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/vectorstores/vectorstores.py
+-rw-r--r--   0        0        0    18548 2024-05-17 15:58:22.280395 langchain_google_vertexai-1.0.4/langchain_google_vertexai/vision_models.py
+-rw-r--r--   0        0        0     3561 2024-05-17 15:58:22.280395 langchain_google_vertexai-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3611 1970-01-01 00:00:00.000000 langchain_google_vertexai-1.0.4/PKG-INFO
```

### Comparing `langchain_google_vertexai-1.0.3/LICENSE` & `langchain_google_vertexai-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.3/README.md` & `langchain_google_vertexai-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/__init__.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+from google.cloud.aiplatform_v1beta1.types import (
+    FunctionCallingConfig,
+    FunctionDeclaration,
+    Schema,
+    ToolConfig,
+    Type,
+)
+
 from langchain_google_vertexai._enums import HarmBlockThreshold, HarmCategory
 from langchain_google_vertexai.chains import create_structured_runnable
 from langchain_google_vertexai.chat_models import ChatVertexAI
 from langchain_google_vertexai.embeddings import VertexAIEmbeddings
 from langchain_google_vertexai.functions_utils import (
     PydanticFunctionsOutputParser,
-    ToolConfig,
 )
 from langchain_google_vertexai.gemma import (
     GemmaChatLocalHF,
     GemmaChatLocalKaggle,
     GemmaChatVertexAIModelGarden,
     GemmaLocalHF,
     GemmaLocalKaggle,
@@ -29,32 +36,36 @@
     VertexAIImageEditorChat,
     VertexAIImageGeneratorChat,
     VertexAIVisualQnAChat,
 )
 
 __all__ = [
     "ChatVertexAI",
-    "GemmaVertexAIModelGarden",
-    "GemmaChatVertexAIModelGarden",
-    "GemmaLocalKaggle",
+    "create_structured_runnable",
+    "DataStoreDocumentStorage",
+    "FunctionCallingConfig",
+    "FunctionDeclaration",
+    "GCSDocumentStorage",
+    "GemmaChatLocalHF",
     "GemmaChatLocalKaggle",
+    "GemmaChatVertexAIModelGarden",
     "GemmaLocalHF",
-    "GemmaChatLocalHF",
-    "VertexAIEmbeddings",
-    "VertexAI",
-    "VertexAIModelGarden",
+    "GemmaLocalKaggle",
+    "GemmaVertexAIModelGarden",
     "HarmBlockThreshold",
     "HarmCategory",
     "PydanticFunctionsOutputParser",
+    "Schema",
     "ToolConfig",
-    "create_structured_runnable",
+    "Type",
+    "VectorSearchVectorStore",
+    "VectorSearchVectorStoreDatastore",
+    "VectorSearchVectorStoreGCS",
+    "VertexAI",
+    "VertexAIEmbeddings",
     "VertexAIImageCaptioning",
     "VertexAIImageCaptioningChat",
     "VertexAIImageEditorChat",
     "VertexAIImageGeneratorChat",
+    "VertexAIModelGarden",
     "VertexAIVisualQnAChat",
-    "DataStoreDocumentStorage",
-    "GCSDocumentStorage",
-    "VectorSearchVectorStore",
-    "VectorSearchVectorStoreDatastore",
-    "VectorSearchVectorStoreGCS",
 ]
```

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/_anthropic_utils.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/_anthropic_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/_base.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,122 @@
 from __future__ import annotations
 
 from concurrent.futures import Executor
 from typing import Any, ClassVar, Dict, List, Optional
 
 import vertexai  # type: ignore[import-untyped]
 from google.api_core.client_options import ClientOptions
+from google.cloud.aiplatform import initializer
+from google.cloud.aiplatform.constants import base as constants
 from google.cloud.aiplatform.gapic import (
     PredictionServiceAsyncClient,
     PredictionServiceClient,
 )
 from google.cloud.aiplatform.models import Prediction
+from google.cloud.aiplatform_v1beta1.services.prediction_service import (
+    PredictionServiceAsyncClient as v1beta1PredictionServiceAsyncClient,
+)
+from google.cloud.aiplatform_v1beta1.services.prediction_service import (
+    PredictionServiceClient as v1beta1PredictionServiceClient,
+)
 from google.protobuf import json_format
 from google.protobuf.struct_pb2 import Value
 from langchain_core.outputs import Generation, LLMResult
 from langchain_core.pydantic_v1 import BaseModel, Field, root_validator
 from vertexai.language_models import (  # type: ignore[import-untyped]
     TextGenerationModel,
 )
-from vertexai.preview.language_models import (  # type: ignore[import-untyped]
+from vertexai.preview.language_models import (  # type: ignore
     ChatModel as PreviewChatModel,
 )
 from vertexai.preview.language_models import (
     CodeChatModel as PreviewCodeChatModel,
 )
 
 from langchain_google_vertexai._enums import HarmBlockThreshold, HarmCategory
 from langchain_google_vertexai._utils import (
+    GoogleModelFamily,
     get_client_info,
     get_user_agent,
-    is_codey_model,
     is_gemini_model,
 )
 
 _PALM_DEFAULT_MAX_OUTPUT_TOKENS = TextGenerationModel._DEFAULT_MAX_OUTPUT_TOKENS
 _PALM_DEFAULT_TEMPERATURE = 0.0
 _PALM_DEFAULT_TOP_P = 0.95
 _PALM_DEFAULT_TOP_K = 40
+_DEFAULT_LOCATION = "us-central1"
 
 
 class _VertexAIBase(BaseModel):
     client: Any = None  #: :meta private:
+    async_client: Any = None  #: :meta private:
     project: Optional[str] = None
     "The default GCP project to use when making Vertex API calls."
-    location: str = "us-central1"
+    location: str = _DEFAULT_LOCATION
     "The default location to use when making API calls."
     request_parallelism: int = 5
     "The amount of parallelism allowed for requests issued to VertexAI models. "
     "Default is 5."
     max_retries: int = 6
     """The maximum number of retries to make when generating."""
     task_executor: ClassVar[Optional[Executor]] = Field(default=None, exclude=True)
     stop: Optional[List[str]] = Field(default=None, alias="stop_sequences")
     "Optional list of stop words to use when generating."
     model_name: Optional[str] = Field(default=None, alias="model")
     "Underlying model name."
+    model_family: Optional[GoogleModelFamily] = None
+    full_model_name: Optional[str] = None
+    """The full name of the model's endpoint."""
 
     class Config:
         """Configuration for this pydantic object."""
 
         allow_population_by_field_name = True
 
     @root_validator(pre=True)
-    def validate_params(cls, values: dict) -> dict:
+    def validate_params_base(cls, values: dict) -> dict:
         if "model" in values and "model_name" not in values:
             values["model_name"] = values.pop("model")
+        if values.get("project") is None:
+            values["project"] = initializer.global_config.project
         return values
 
+    @property
+    def prediction_client(self) -> v1beta1PredictionServiceClient:
+        """Returns PredictionServiceClient."""
+        if self.client is None:
+            client_options = {
+                "api_endpoint": f"{self.location}-{constants.PREDICTION_API_BASE_PATH}"
+            }
+            self.client = v1beta1PredictionServiceClient(
+                client_options=client_options,
+                client_info=get_client_info(module=self._user_agent),
+            )
+        return self.client
+
+    @property
+    def async_prediction_client(self) -> v1beta1PredictionServiceAsyncClient:
+        """Returns PredictionServiceClient."""
+        if self.async_client is None:
+            client_options = {
+                "api_endpoint": f"{self.location}-{constants.PREDICTION_API_BASE_PATH}"
+            }
+            self.async_client = v1beta1PredictionServiceAsyncClient(
+                client_options=ClientOptions(**client_options),
+                client_info=get_client_info(module=self._user_agent),
+            )
+        return self.async_client
+
+    @property
+    def _user_agent(self) -> str:
+        """Gets the User Agent."""
+        _, user_agent = get_user_agent(f"{type(self).__name__}_{self.model_name}")
+        return user_agent
+
 
 class _VertexAICommon(_VertexAIBase):
     client_preview: Any = None  #: :meta private:
     model_name: str = Field(default=None, alias="model")
     "Underlying model name."
     temperature: Optional[float] = None
     "Sampling temperature, it controls the degree of randomness in token selection."
@@ -103,52 +150,51 @@
                 HarmCategory.HARM_CATEGORY_HARASSMENT: HarmBlockThreshold.BLOCK_LOW_AND_ABOVE,
                 HarmCategory.HARM_CATEGORY_SEXUALLY_EXPLICIT: HarmBlockThreshold.BLOCK_NONE,
             }
             """  # noqa: E501
 
     api_transport: Optional[str] = None
     """The desired API transport method, can be either 'grpc' or 'rest'"""
-
     api_endpoint: Optional[str] = None
     """The desired API endpoint, e.g., us-central1-aiplatform.googleapis.com"""
+    tuned_model_name: Optional[str] = None
+    """The name of a tuned model. If tuned_model_name is passed
+    model_name will be used to determine the model family
+    """
 
     @property
-    def _llm_type(self) -> str:
-        return "vertexai"
-
-    @property
-    def is_codey_model(self) -> bool:
-        return is_codey_model(self.model_name)
+    def _is_gemini_model(self) -> bool:
+        return is_gemini_model(self.model_family)  # type: ignore[arg-type]
 
     @property
-    def _is_gemini_model(self) -> bool:
-        return is_gemini_model(self.model_name)
+    def _llm_type(self) -> str:
+        return "vertexai"
 
     @property
     def _identifying_params(self) -> Dict[str, Any]:
         """Gets the identifying parameters."""
         return {**{"model_name": self.model_name}, **self._default_params}
 
     @property
     def _default_params(self) -> Dict[str, Any]:
-        if self._is_gemini_model:
+        if self.model_family == GoogleModelFamily.GEMINI:
             default_params = {}
         else:
             default_params = {
                 "temperature": _PALM_DEFAULT_TEMPERATURE,
                 "max_output_tokens": _PALM_DEFAULT_MAX_OUTPUT_TOKENS,
                 "top_p": _PALM_DEFAULT_TOP_P,
                 "top_k": _PALM_DEFAULT_TOP_K,
             }
         params = {
             "temperature": self.temperature,
             "max_output_tokens": self.max_output_tokens,
             "candidate_count": self.n,
         }
-        if not self.is_codey_model:
+        if not self.model_family == GoogleModelFamily.CODEY:
             params.update(
                 {
                     "top_k": self.top_k,
                     "top_p": self.top_p,
                 }
             )
         updated_params = {}
@@ -156,20 +202,14 @@
             default_value = default_params.get(param_name)
             if param_value is not None or default_value is not None:
                 updated_params[param_name] = (
                     param_value if param_value is not None else default_value
                 )
         return updated_params
 
-    @property
-    def _user_agent(self) -> str:
-        """Gets the User Agent."""
-        _, user_agent = get_user_agent(f"{type(self).__name__}_{self.model_name}")
-        return user_agent
-
     @classmethod
     def _init_vertexai(cls, values: Dict) -> None:
         vertexai.init(
             project=values.get("project"),
             location=values.get("location"),
             credentials=values.get("credentials"),
             api_transport=values.get("api_transport"),
@@ -205,15 +245,14 @@
         is_palm_chat_model = isinstance(
             self.client_preview, PreviewChatModel
         ) or isinstance(self.client_preview, PreviewCodeChatModel)
         if is_palm_chat_model:
             result = self.client_preview.start_chat().count_tokens(text)
         else:
             result = self.client_preview.count_tokens([text])
-
         return result.total_tokens
 
 
 class _BaseVertexAIModelGarden(_VertexAIBase):
     """Large language models served from Vertex AI Model Garden."""
 
     async_client: Any = None  #: :meta private:
```

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/_image_utils.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/_image_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import re
 from enum import Enum
 from typing import Dict, Union
 from urllib.parse import urlparse
 
 import requests
 from google.cloud import storage
+from google.cloud.aiplatform_v1beta1.types.content import Part as GapicPart
 from vertexai.generative_models import Image, Part  # type: ignore
 
 
 class Route(Enum):
     """Image Loading Route"""
 
     GOOGLE_CLOUD_STORAGE = 1
@@ -103,14 +104,18 @@
             bytes_ = self._bytes_from_url(image_string)
 
         if route == Route.LOCAL_FILE:
             bytes_ = self._bytes_from_file(image_string)
 
         return Part.from_image(Image.from_bytes(bytes_))
 
+    def load_gapic_part(self, image_string: str) -> GapicPart:
+        part = self.load_part(image_string)
+        return part._raw_part
+
     def _route(self, image_string: str) -> Route:
         if image_string.startswith("gs://"):
             return Route.GOOGLE_CLOUD_STORAGE
 
         if image_string.startswith("data:image/"):
             return Route.BASE64
```

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/_utils.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Utilities to init Vertex AI."""
 
 import dataclasses
 import re
+from enum import Enum, auto
 from importlib import metadata
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import google.api_core
 import proto  # type: ignore[import-untyped]
 from google.api_core.gapic_v1.client_info import ClientInfo
 from google.cloud import storage  # type: ignore[attr-defined, unused-ignore]
@@ -90,32 +91,54 @@
     client_library_version, user_agent = get_user_agent(module)
     return ClientInfo(
         client_library_version=client_library_version,
         user_agent=user_agent,
     )
 
 
+def _format_model_name(model: str, project: str, location: str) -> str:
+    if "/" not in model:
+        model = "publishers/google/models/" + model
+    if model.startswith("models/"):
+        model = "publishers/google/" + model
+    if model.startswith("publishers/"):
+        return f"projects/{project}/locations/{location}/{model}"
+    return model
+
+
 def load_image_from_gcs(path: str, project: Optional[str] = None) -> Image:
     """Loads an Image from GCS."""
     gcs_client = storage.Client(project=project)
     pieces = path.split("/")
     blobs = list(gcs_client.list_blobs(pieces[2], prefix="/".join(pieces[3:])))
     if len(blobs) > 1:
         raise ValueError(f"Found more than one candidate for {path}!")
     return Image.from_bytes(blobs[0].download_as_bytes())
 
 
-def is_codey_model(model_name: str) -> bool:
-    """Returns True if the model name is a Codey model."""
-    return "code" in model_name
+class GoogleModelFamily(str, Enum):
+    GEMINI = auto()
+    GEMINI_ADVANCED = auto()
+    CODEY = auto()
+    PALM = auto()
+
+    @classmethod
+    def _missing_(cls, value: Any) -> "GoogleModelFamily":
+        if "gemini" in value.lower():
+            return GoogleModelFamily.GEMINI
+        if "code" in value.lower():
+            return GoogleModelFamily.CODEY
+        elif "bison" in value.lower():
+            return GoogleModelFamily.PALM
+        return GoogleModelFamily.GEMINI
 
 
-def is_gemini_model(model_name: str) -> bool:
+def is_gemini_model(model_family: GoogleModelFamily) -> bool:
     """Returns True if the model name is a Gemini model."""
-    return model_name is not None and "gemini" in model_name
+    return model_family in [GoogleModelFamily.GEMINI, GoogleModelFamily.GEMINI_ADVANCED]
 
 
 def get_generation_info(
     candidate: Union[TextGenerationResponse, Candidate],
     is_gemini: bool,
     *,
     stream: bool = False,
@@ -134,17 +157,24 @@
                 for rating in candidate.safety_ratings
             ],
             "citation_metadata": (
                 proto.Message.to_dict(candidate.citation_metadata)
                 if candidate.citation_metadata
                 else None
             ),
+            "usage_metadata": usage_metadata,
         }
-        if usage_metadata:
-            info["usage_metadata"] = usage_metadata
+        try:
+            if candidate.grounding_metadata:
+                info["grounding_metadata"] = proto.Message.to_dict(
+                    candidate.grounding_metadata
+                )
+        except AttributeError:
+            pass
+        info = {k: v for k, v in info.items() if v is not None}
     # https://cloud.google.com/vertex-ai/docs/generative-ai/model-reference/text-chat#response_body
     else:
         info = dataclasses.asdict(candidate)
         info.pop("text")
         info = {k: v for k, v in info.items() if not k.startswith("_")}
         if usage_metadata:
             info_usage_metadata = {}
```

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/callbacks.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/callbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/chains.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/chains.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,23 @@
     Dict,
     Optional,
     Sequence,
     Type,
     Union,
 )
 
+import google.cloud.aiplatform_v1beta1.types as gapic
 from langchain_core.output_parsers import (
     BaseGenerationOutputParser,
     BaseOutputParser,
     StrOutputParser,
 )
 from langchain_core.prompts import BasePromptTemplate, ChatPromptTemplate
 from langchain_core.pydantic_v1 import BaseModel
 from langchain_core.runnables import Runnable
-from vertexai.generative_models._generative_models import (  # type: ignore
-    ToolConfig,
-)
 
 from langchain_google_vertexai.functions_utils import PydanticFunctionsOutputParser
 
 
 def get_output_parser(
     functions: Sequence[Type[BaseModel]],
 ) -> Union[BaseOutputParser, BaseGenerationOutputParser]:
@@ -55,15 +53,15 @@
 ) -> Runnable:
     names = [schema.schema()["title"] for schema in functions]
     if hasattr(llm, "is_gemini_advanced") and llm._is_gemini_advanced:  # type: ignore
         llm_with_functions = llm.bind(
             functions=functions,
             tool_config={
                 "function_calling_config": {
-                    "mode": ToolConfig.FunctionCallingConfig.Mode.ANY,
+                    "mode": gapic.FunctionCallingConfig.Mode.ANY,
                     "allowed_function_names": names,
                 }
             },
         )
     else:
         llm_with_functions = llm.bind(
             functions=functions,
```

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/chat_models.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/chat_models.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,16 +21,14 @@
     cast,
     Literal,
     TypedDict,
     overload,
 )
 
 import proto  # type: ignore[import-untyped]
-from google.cloud.aiplatform_v1beta1.types.content import Part as GapicPart
-from google.cloud.aiplatform_v1beta1.types.tool import FunctionCall
 from google.cloud.aiplatform import telemetry
 
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain_core.language_models import LanguageModelInput
@@ -56,18 +54,14 @@
     PydanticToolsParser,
 )
 from langchain_core.output_parsers.openai_tools import parse_tool_calls
 from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult
 from langchain_core.pydantic_v1 import BaseModel, root_validator, Field
 from langchain_core.runnables import Runnable, RunnablePassthrough
 from vertexai.generative_models import (  # type: ignore
-    Candidate,
-    Content,
-    GenerativeModel,
-    Part,
     Tool as VertexTool,
 )
 from vertexai.generative_models._generative_models import (  # type: ignore
     ToolConfig,
     SafetySettingsType,
     GenerationConfigType,
     GenerationResponse,
@@ -83,38 +77,60 @@
 from vertexai.preview.language_models import (  # type: ignore
     ChatModel as PreviewChatModel,
 )
 from vertexai.preview.language_models import (
     CodeChatModel as PreviewCodeChatModel,
 )
 
-from langchain_google_vertexai._base import (
-    _VertexAICommon,
+from google.cloud.aiplatform_v1beta1.types import (
+    Candidate,
+    Part,
+    HarmCategory,
+    Content,
+    FunctionCall,
+    FunctionResponse,
+    GenerateContentRequest,
+    GenerationConfig,
+    SafetySetting,
+    Tool as GapicTool,
+    ToolConfig as GapicToolConfig,
 )
+from langchain_google_vertexai._base import _VertexAICommon, GoogleModelFamily
 from langchain_google_vertexai._image_utils import ImageBytesLoader
 from langchain_google_vertexai._utils import (
     create_retry_decorator,
     get_generation_info,
-    is_codey_model,
-    is_gemini_model,
+    _format_model_name,
 )
 from langchain_google_vertexai.functions_utils import (
     _format_tool_config,
     _ToolConfigDict,
     _tool_choice_to_tool_config,
     _ToolChoiceType,
-    _FunctionDeclarationLike,
-    _VertexToolDict,
-    _format_to_vertex_tool,
-    _format_functions_to_vertex_tool_dict,
+    _ToolsType,
+    _format_to_gapic_tool,
 )
 
 logger = logging.getLogger(__name__)
 
 
+_allowed_params = [
+    "temperature",
+    "top_k",
+    "top_p",
+    "response_mime_type",
+    "temperature",
+    "max_output_tokens",
+    "presence_penalty",
+    "frequency_penalty",
+    "candidate_count",
+]
+_allowed_params_prediction_service = ["request", "timeout", "metadata"]
+
+
 @dataclass
 class _ChatHistory:
     """Represents a context and a history of messages."""
 
     history: List[ChatMessage] = field(default_factory=list)
     context: Optional[str] = None
 
@@ -160,25 +176,25 @@
 def _parse_chat_history_gemini(
     history: List[BaseMessage],
     project: Optional[str] = None,
     convert_system_message_to_human: Optional[bool] = False,
 ) -> tuple[Content | None, list[Content]]:
     def _convert_to_prompt(part: Union[str, Dict]) -> Part:
         if isinstance(part, str):
-            return Part.from_text(part)
+            return Part(text=part)
 
         if not isinstance(part, Dict):
             raise ValueError(
                 f"Message's content is expected to be a dict, got {type(part)}!"
             )
         if part["type"] == "text":
-            return Part.from_text(part["text"])
+            return Part(text=part["text"])
         if part["type"] == "image_url":
             path = part["image_url"]["url"]
-            return ImageBytesLoader(project=project).load_part(path)
+            return ImageBytesLoader(project=project).load_gapic_part(path)
 
         raise ValueError("Only text and image_url types are supported!")
 
     def _convert_to_parts(message: BaseMessage) -> List[Part]:
         raw_content = message.content
         if isinstance(raw_content, str):
             raw_content = [raw_content]
@@ -228,32 +244,30 @@
             for tc in message.tool_calls:
                 function_call = FunctionCall(
                     {
                         "name": tc["name"],
                         "args": tc["args"],
                     }
                 )
-                gapic_part = GapicPart(function_call=function_call)
-                parts.append(Part._from_gapic(gapic_part))
+                parts.append(Part(function_call=function_call))
 
             vertex_messages.append(Content(role=role, parts=parts))
         elif isinstance(message, FunctionMessage):
             role = "function"
 
-            part = Part.from_function_response(
-                name=message.name,
-                response={
-                    "content": message.content,
-                },
+            part = Part(
+                function_response=FunctionResponse(
+                    name=message.name, response={"content": message.content}
+                )
             )
 
             prev_content = vertex_messages[-1]
             prev_content_is_function = prev_content and prev_content.role == "function"
             if prev_content_is_function:
-                parts = prev_content.parts
+                parts = list(prev_content.parts)
                 parts.append(part)
                 # replacing last message
                 vertex_messages[-1] = Content(role=role, parts=parts)
                 continue
 
             parts = [part]
 
@@ -275,25 +289,27 @@
                         raise ValueError(
                             (
                                 "Message name is empty and can't find"
                                 + f"corresponding tool call for id: '${tool_call_id}'"
                             )
                         )
                     name = tool_call["name"]
-            part = Part.from_function_response(
-                name=name,
-                response={
-                    "content": message.content,
-                },
+            part = Part(
+                function_response=FunctionResponse(
+                    name=name,
+                    response={
+                        "content": message.content,
+                    },
+                )
             )
 
             prev_content = vertex_messages[-1]
             prev_content_is_function = prev_content and prev_content.role == "function"
             if prev_content_is_function:
-                parts = prev_content.parts
+                parts = list(prev_content.parts)
                 parts.append(part)
                 # replacing last message
                 vertex_messages[-1] = Content(role=role, parts=parts)
                 continue
 
             parts = [part]
 
@@ -370,16 +386,16 @@
 
     for part in response_candidate.content.parts:
         try:
             text: Optional[str] = part.text
         except AttributeError:
             text = None
 
-        if text is not None:
-            if content is None:
+        if text:
+            if not content:
                 content = text
             elif isinstance(content, str):
                 content = [content, text]
             elif isinstance(content, list):
                 content.append(text)
             else:
                 raise Exception("Unexpected content type")
@@ -400,20 +416,21 @@
             function_call_args_dict = proto.Message.to_dict(part.function_call)["args"]
             function_call["arguments"] = json.dumps(
                 {k: function_call_args_dict[k] for k in function_call_args_dict}
             )
             additional_kwargs["function_call"] = function_call
 
             if streaming:
+                index = function_call.get("index")
                 tool_call_chunks.append(
                     ToolCallChunk(
                         name=function_call.get("name"),
                         args=function_call.get("arguments"),
                         id=function_call.get("id", str(uuid.uuid4())),
-                        index=function_call.get("index"),
+                        index=int(index) if index else None,
                     )
                 )
             else:
                 try:
                     tool_calls_dicts = parse_tool_calls(
                         [{"function": function_call}],
                         return_id=False,
@@ -467,15 +484,23 @@
         max_retries=max_retries, run_manager=run_manager
     )
 
     @retry_decorator
     def _completion_with_retry_inner(generation_method: Callable, **kwargs: Any) -> Any:
         return generation_method(**kwargs)
 
-    return _completion_with_retry_inner(generation_method, **kwargs)
+    params = (
+        {k: v for k, v in kwargs.items() if k in _allowed_params_prediction_service}
+        if kwargs.get("is_gemini")
+        else kwargs
+    )
+    return _completion_with_retry_inner(
+        generation_method,
+        **params,
+    )
 
 
 async def _acompletion_with_retry(
     generation_method: Callable,
     *,
     max_retries: int,
     run_manager: Optional[CallbackManagerForLLMRun] = None,
@@ -488,27 +513,31 @@
 
     @retry_decorator
     async def _completion_with_retry_inner(
         generation_method: Callable, **kwargs: Any
     ) -> Any:
         return await generation_method(**kwargs)
 
-    return await _completion_with_retry_inner(generation_method, **kwargs)
+    params = (
+        {k: v for k, v in kwargs.items() if k in _allowed_params_prediction_service}
+        if kwargs.get("is_gemini")
+        else kwargs
+    )
+    return await _completion_with_retry_inner(
+        generation_method,
+        **params,
+    )
 
 
 class ChatVertexAI(_VertexAICommon, BaseChatModel):
     """`Vertex AI` Chat large language models API."""
 
     model_name: str = Field(default="chat-bison", alias="model")
     "Underlying model name."
     examples: Optional[List[BaseMessage]] = None
-    tuned_model_name: Optional[str] = None
-    """The name of a tuned model. If tuned_model_name is passed
-    model_name will be used to determine the model family
-    """
     convert_system_message_to_human: bool = False
     """[Deprecated] Since new Gemini models support setting a System Message,
     setting this parameter to True is discouraged.
     """
 
     def __init__(self, *, model_name: Optional[str] = None, **kwargs: Any) -> None:
         """Needed for mypy typing to recognize model_name as a valid arg."""
@@ -530,56 +559,64 @@
     def get_lc_namespace(cls) -> List[str]:
         """Get the namespace of the langchain object."""
         return ["langchain", "chat_models", "vertexai"]
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that the python package exists in environment."""
-        is_gemini = is_gemini_model(values["model_name"])
-        safety_settings = values["safety_settings"]
+        safety_settings = values.get("safety_settings")
         tuned_model_name = values.get("tuned_model_name")
+        values["model_family"] = GoogleModelFamily(values["model_name"])
 
-        if safety_settings and not is_gemini:
-            raise ValueError("Safety settings are only supported for Gemini models")
+        if values.get("full_model_name") is not None:
+            pass
+        elif values.get("tuned_model_name") is not None:
+            values["full_model_name"] = _format_model_name(
+                values["tuned_model_name"],
+                location=values["location"],
+                project=values["project"],
+            )
+        else:
+            values["full_model_name"] = _format_model_name(
+                values["model_name"],
+                location=values["location"],
+                project=values["project"],
+            )
 
-        cls._init_vertexai(values)
+        if safety_settings and values["model_family"] not in [
+            GoogleModelFamily.GEMINI,
+            GoogleModelFamily.GEMINI_ADVANCED,
+        ]:
+            raise ValueError("Safety settings are only supported for Gemini models")
 
         if tuned_model_name:
             generative_model_name = values["tuned_model_name"]
         else:
             generative_model_name = values["model_name"]
 
-        if is_gemini:
-            values["client"] = GenerativeModel(
-                model_name=generative_model_name,
-                safety_settings=safety_settings,
-            )
-            values["client_preview"] = GenerativeModel(
-                model_name=generative_model_name,
-                safety_settings=safety_settings,
-            )
-        else:
-            if is_codey_model(values["model_name"]):
+        if values["model_family"] not in [
+            GoogleModelFamily.GEMINI,
+            GoogleModelFamily.GEMINI_ADVANCED,
+        ]:
+            cls._init_vertexai(values)
+            if values["model_family"] == GoogleModelFamily.CODEY:
                 model_cls = CodeChatModel
                 model_cls_preview = PreviewCodeChatModel
             else:
                 model_cls = ChatModel
                 model_cls_preview = PreviewChatModel
             values["client"] = model_cls.from_pretrained(generative_model_name)
             values["client_preview"] = model_cls_preview.from_pretrained(
                 generative_model_name
             )
         return values
 
     @property
     def _is_gemini_advanced(self) -> bool:
-        try:
-            return float(self.model_name.split("-")[1]) > 1.0
-        except (ValueError, IndexError):
-            return False
+        return self.model_family == GoogleModelFamily.GEMINI_ADVANCED
 
     def _generate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         stream: Optional[bool] = None,
@@ -603,26 +640,167 @@
         if stream is True or (stream is None and self.streaming):
             stream_iter = self._stream(
                 messages, stop=stop, run_manager=run_manager, **kwargs
             )
             return generate_from_stream(stream_iter)
         if not self._is_gemini_model:
             return self._generate_non_gemini(messages, stop=stop, **kwargs)
+        return self._generate_gemini(
+            messages=messages,
+            stop=stop,
+            run_manager=run_manager,
+            is_gemini=True,
+            **kwargs,
+        )
 
-        client, contents = self._gemini_client_and_contents(messages)
-        params = self._gemini_params(stop=stop, **kwargs)
-        with telemetry.tool_context_manager(self._user_agent):
-            response = _completion_with_retry(
-                client.generate_content,
-                max_retries=self.max_retries,
-                contents=contents,
-                **params,
+    def _generation_config_gemini(
+        self,
+        stop: Optional[List[str]] = None,
+        stream: bool = False,
+        **kwargs,
+    ) -> GenerationConfig:
+        """Prepares GenerationConfig part of the request.
+
+        https://cloud.google.com/vertex-ai/docs/reference/rpc/google.cloud.aiplatform.v1beta1#generationconfig
+        """
+        return GenerationConfig(
+            **self._prepare_params(
+                stop=stop,
+                stream=stream,
+                **{k: v for k, v in kwargs.items() if k in _allowed_params},
             )
+        )
+
+    def _safety_settings_gemini(
+        self, safety_settings: Optional[SafetySettingsType]
+    ) -> Optional[Sequence[SafetySetting]]:
+        """Prepares SafetySetting part of the request.
+
+        https://cloud.google.com/vertex-ai/docs/reference/rpc/google.cloud.aiplatform.v1beta1#safetysetting
+        """
+        if safety_settings is None:
+            return None
+        if isinstance(safety_settings, list):
+            return safety_settings
+        if isinstance(safety_settings, dict):
+            formatted_safety_settings = []
+            for category, threshold in safety_settings.items():
+                if isinstance(category, str):
+                    category = HarmCategory[category]  # type: ignore[misc]
+                if isinstance(threshold, str):
+                    threshold = SafetySetting.HarmBlockThreshold[threshold]  # type: ignore[misc]
+
+                formatted_safety_settings.append(
+                    SafetySetting(
+                        category=HarmCategory(category),
+                        threshold=SafetySetting.HarmBlockThreshold(threshold),
+                    )
+                )
+            return formatted_safety_settings
+        raise ValueError("safety_settings should be either")
+
+    def _prepare_request_gemini(
+        self,
+        messages: List[BaseMessage],
+        stop: Optional[List[str]] = None,
+        stream: bool = False,
+        tools: Optional[_ToolsType] = None,
+        functions: Optional[_ToolsType] = None,
+        tool_config: Optional[Union[_ToolConfigDict, ToolConfig]] = None,
+        safety_settings: Optional[SafetySettingsType] = None,
+        **kwargs,
+    ) -> GenerateContentRequest:
+        system_instruction, contents = _parse_chat_history_gemini(messages)
+        formatted_tools = self._tools_gemini(tools=tools, functions=functions)
+        tool_config = self._tool_config_gemini(tool_config=tool_config)
+        return GenerateContentRequest(
+            contents=contents,
+            system_instruction=system_instruction,
+            tools=formatted_tools,
+            tool_config=tool_config,
+            safety_settings=self._safety_settings_gemini(safety_settings),
+            generation_config=self._generation_config_gemini(
+                stream=stream, stop=stop, **kwargs
+            ),
+            model=self.full_model_name,
+        )
+
+    def _generate_gemini(
+        self,
+        messages: List[BaseMessage],
+        stop: Optional[List[str]] = None,
+        run_manager: Optional[CallbackManagerForLLMRun] = None,
+        **kwargs: Any,
+    ) -> ChatResult:
+        request = self._prepare_request_gemini(messages=messages, stop=stop, **kwargs)
+        response = _completion_with_retry(
+            self.prediction_client.generate_content,
+            max_retries=self.max_retries,
+            request=request,
+            **kwargs,
+        )
+        return self._gemini_response_to_chat_result(response)
+
+    async def _agenerate_gemini(
+        self,
+        messages: List[BaseMessage],
+        stop: Optional[List[str]] = None,
+        run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
+        **kwargs: Any,
+    ) -> ChatResult:
+        response = await _acompletion_with_retry(
+            self.async_prediction_client.generate_content,
+            max_retries=self.max_retries,
+            request=self._prepare_request_gemini(
+                messages=messages, stop=stop, **kwargs
+            ),
+            is_gemini=True,
+            **kwargs,
+        )
         return self._gemini_response_to_chat_result(response)
 
+    def get_num_tokens(self, text: str) -> int:
+        """Get the number of tokens present in the text."""
+        if self._is_gemini_model:
+            # https://cloud.google.com/vertex-ai/docs/reference/rpc/google.cloud.aiplatform.v1beta1#counttokensrequest
+            _, contents = _parse_chat_history_gemini([HumanMessage(content=text)])
+            response = self.prediction_client.count_tokens(
+                {
+                    "endpoint": self.full_model_name,
+                    "model": self.full_model_name,
+                    "contents": contents,
+                }
+            )
+            return response.total_tokens
+        else:
+            return super().get_num_tokens(text=text)
+
+    def _tools_gemini(
+        self,
+        tools: Optional[_ToolsType] = None,
+        functions: Optional[_ToolsType] = None,
+    ) -> Optional[Sequence[GapicTool]]:
+        if tools and functions:
+            logger.warning(
+                "Binding tools and functions together is not supported.",
+                "Only tools will be used",
+            )
+        if tools:
+            return [_format_to_gapic_tool(tools)]
+        if functions:
+            return [_format_to_gapic_tool(functions)]
+        return None
+
+    def _tool_config_gemini(
+        self, tool_config: Optional[Union[_ToolConfigDict, ToolConfig]] = None
+    ) -> Optional[GapicToolConfig]:
+        if tool_config and not isinstance(tool_config, ToolConfig):
+            return _format_tool_config(cast(_ToolConfigDict, tool_config))
+        return None
+
     def _generate_non_gemini(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> ChatResult:
         kwargs.pop("safety_settings", None)
@@ -680,24 +858,20 @@
         if "stream" in kwargs:
             kwargs.pop("stream")
             logger.warning("ChatVertexAI does not currently support async streaming.")
 
         if not self._is_gemini_model:
             return await self._agenerate_non_gemini(messages, stop=stop, **kwargs)
 
-        client, contents = self._gemini_client_and_contents(messages)
-        params = self._gemini_params(stop=stop, **kwargs)
-        with telemetry.tool_context_manager(self._user_agent):
-            response = await _acompletion_with_retry(
-                client.generate_content_async,
-                max_retries=self.max_retries,
-                contents=contents,
-                **params,
-            )
-        return self._gemini_response_to_chat_result(response)
+        return await self._agenerate_gemini(
+            messages=messages,
+            stop=stop,
+            run_manager=run_manager,
+            **kwargs,
+        )
 
     async def _agenerate_non_gemini(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> ChatResult:
@@ -740,25 +914,34 @@
         **kwargs: Any,
     ) -> Iterator[ChatGenerationChunk]:
         if not self._is_gemini_model:
             yield from self._stream_non_gemini(
                 messages, stop=stop, run_manager=run_manager, **kwargs
             )
             return
+        yield from self._stream_gemini(
+            messages=messages, stop=stop, run_manager=run_manager, **kwargs
+        )
+        return
 
-        client, contents = self._gemini_client_and_contents(messages)
-        params = self._gemini_params(stop=stop, stream=True, **kwargs)
-        with telemetry.tool_context_manager(self._user_agent):
-            response_iter = _completion_with_retry(
-                client.generate_content,
-                max_retries=self.max_retries,
-                contents=contents,
-                stream=True,
-                **params,
-            )
+    def _stream_gemini(
+        self,
+        messages: List[BaseMessage],
+        stop: Optional[List[str]] = None,
+        run_manager: Optional[CallbackManagerForLLMRun] = None,
+        **kwargs: Any,
+    ) -> Iterator[ChatGenerationChunk]:
+        request = self._prepare_request_gemini(messages=messages, stop=stop, **kwargs)
+        response_iter = _completion_with_retry(
+            self.prediction_client.stream_generate_content,
+            max_retries=self.max_retries,
+            request=request,
+            is_gemini=True,
+            **kwargs,
+        )
         for response_chunk in response_iter:
             chunk = self._gemini_chunk_to_generation_chunk(response_chunk)
             if run_manager and isinstance(chunk.message.content, str):
                 run_manager.on_llm_new_token(chunk.message.content)
             yield chunk
 
     def _stream_non_gemini(
@@ -794,28 +977,28 @@
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> AsyncIterator[ChatGenerationChunk]:
         if not self._is_gemini_model:
             raise NotImplementedError()
-        client, contents = self._gemini_client_and_contents(messages)
-        params = self._gemini_params(stop=stop, stream=True, **kwargs)
-        with telemetry.tool_context_manager(self._user_agent):
-            async for response_chunk in await _acompletion_with_retry(
-                client.generate_content_async,
-                max_retries=self.max_retries,
-                contents=contents,
-                stream=True,
-                **params,
-            ):
-                chunk = self._gemini_chunk_to_generation_chunk(response_chunk)
-                if run_manager and isinstance(chunk.message.content, str):
-                    await run_manager.on_llm_new_token(chunk.message.content)
-                yield chunk
+        request = self._prepare_request_gemini(messages=messages, stop=stop, **kwargs)
+
+        response_iter = _acompletion_with_retry(
+            self.async_prediction_client.stream_generate_content,
+            max_retries=self.max_retries,
+            request=request,
+            is_gemini=True,
+            **kwargs,
+        )
+        async for response_chunk in await response_iter:
+            chunk = self._gemini_chunk_to_generation_chunk(response_chunk)
+            if run_manager and isinstance(chunk.message.content, str):
+                await run_manager.on_llm_new_token(chunk.message.content)
+            yield chunk
 
     def with_structured_output(
         self,
         schema: Union[Dict, Type[BaseModel]],
         *,
         include_raw: bool = False,
         **kwargs: Any,
@@ -925,15 +1108,15 @@
             )
             return {"raw": llm} | parser_with_fallback
         else:
             return llm | parser
 
     def bind_tools(
         self,
-        tools: Sequence[Union[_FunctionDeclarationLike, VertexTool]],
+        tools: _ToolsType,
         tool_config: Optional[_ToolConfigDict] = None,
         *,
         tool_choice: Optional[Union[_ToolChoiceType, bool]] = None,
         **kwargs: Any,
     ) -> Runnable[LanguageModelInput, BaseMessage]:
         """Bind tool-like objects to this chat model.
 
@@ -948,95 +1131,36 @@
                 :class:`~langchain.runnable.Runnable` constructor.
         """
         if tool_choice and tool_config:
             raise ValueError(
                 "Must specify at most one of tool_choice and tool_config, received "
                 f"both:\n\n{tool_choice=}\n\n{tool_config=}"
             )
-        vertexai_tools: List[_VertexToolDict] = []
-        vertexai_functions = []
-        for schema in tools:
-            if isinstance(schema, VertexTool):
-                vertexai_tools.append(
-                    {"function_declarations": schema.to_dict()["function_declarations"]}
-                )
-            elif isinstance(schema, dict) and "function_declarations" in schema:
-                vertexai_tools.append(cast(_VertexToolDict, schema))
-            else:
-                vertexai_functions.append(schema)
-        vertexai_tools.append(_format_functions_to_vertex_tool_dict(vertexai_functions))
+        vertexai_tool = _format_to_gapic_tool(tools)
         if tool_choice:
-            all_names = [
-                f["name"] for vt in vertexai_tools for f in vt["function_declarations"]
-            ]
+            all_names = [f["name"] for f in vertexai_tool.function_declarations]
             tool_config = _tool_choice_to_tool_config(tool_choice, all_names)
         # Bind dicts for easier serialization/deserialization.
-        return self.bind(tools=vertexai_tools, tool_config=tool_config, **kwargs)
+        return self.bind(tools=[vertexai_tool], tool_config=tool_config, **kwargs)
 
     def _start_chat(
         self, history: _ChatHistory, **kwargs: Any
     ) -> Union[ChatSession, CodeChatSession]:
-        if not self.is_codey_model:
+        if self.model_family == GoogleModelFamily.CODEY:
             return self.client.start_chat(
                 context=history.context, message_history=history.history, **kwargs
             )
         else:
             return self.client.start_chat(message_history=history.history, **kwargs)
 
-    def _gemini_params(
-        self,
-        *,
-        stop: Optional[List[str]] = None,
-        stream: bool = False,
-        tools: Optional[List[Union[_VertexToolDict, VertexTool]]] = None,
-        functions: Optional[List[_FunctionDeclarationLike]] = None,
-        tool_config: Optional[Union[_ToolConfigDict, ToolConfig]] = None,
-        safety_settings: Optional[SafetySettingsType] = None,
-        **kwargs: Any,
-    ) -> _GeminiGenerateContentKwargs:
-        generation_config = self._prepare_params(stop=stop, stream=stream, **kwargs)
-        if tools:
-            tools = [_format_to_vertex_tool(tool) for tool in tools]
-        elif functions:
-            tools = [_format_to_vertex_tool(functions)]
-        else:
-            pass
-
-        if tool_config and not isinstance(tool_config, ToolConfig):
-            tool_config = _format_tool_config(cast(_ToolConfigDict, tool_config))
-
-        return _GeminiGenerateContentKwargs(
-            generation_config=generation_config,
-            tools=tools,
-            tool_config=tool_config,
-            safety_settings=safety_settings,
-        )
-
-    def _gemini_client_and_contents(
-        self, messages: List[BaseMessage]
-    ) -> tuple[GenerativeModel, list[Content]]:
-        system, contents = _parse_chat_history_gemini(
-            messages,
-            project=self.project,
-            convert_system_message_to_human=self.convert_system_message_to_human,
-        )
-        # TODO: Store default client params explicitly so private params don't have to
-        # be accessed, like _safety_settings.
-        client = GenerativeModel(
-            model_name=self.model_name,
-            system_instruction=system,
-            safety_settings=self.client._safety_settings,
-        )
-        return client, contents
-
     def _gemini_response_to_chat_result(
         self, response: GenerationResponse
     ) -> ChatResult:
         generations = []
-        usage = response.to_dict().get("usage_metadata")
+        usage = proto.Message.to_dict(response.usage_metadata)
         for candidate in response.candidates:
             info = get_generation_info(candidate, is_gemini=True, usage_metadata=usage)
             message = _parse_response_candidate(candidate)
             generations.append(ChatGeneration(message=message, generation_info=info))
         if not response.candidates:
             message = AIMessage(content="")
             if usage:
@@ -1048,26 +1172,27 @@
             )
         return ChatResult(generations=generations)
 
     def _gemini_chunk_to_generation_chunk(
         self, response_chunk: GenerationResponse
     ) -> ChatGenerationChunk:
         # return an empty completion message if there's no candidates
-        usage_metadata = response_chunk.to_dict().get("usage_metadata")
+        usage_metadata = proto.Message.to_dict(response_chunk.usage_metadata)
         if not response_chunk.candidates:
             message = AIMessageChunk(content="")
             if usage_metadata:
                 generation_info = {"usage_metadata": usage_metadata}
             else:
                 generation_info = {}
         else:
             top_candidate = response_chunk.candidates[0]
             message = _parse_response_candidate(top_candidate, streaming=True)
             generation_info = get_generation_info(
                 top_candidate,
                 is_gemini=True,
-                usage_metadata=usage_metadata,
+                # TODO: uncomment when merging ints is fixed
+                # usage_metadata=usage_metadata,
             )
         return ChatGenerationChunk(
             message=message,
             generation_info=generation_info,
         )
```

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/embeddings.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/functions_utils.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/functions_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,183 +1,239 @@
 from __future__ import annotations
 
 import json
+import logging
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Literal,
     Optional,
+    Sequence,
     Type,
     TypedDict,
     Union,
+    cast,
 )
 
+import google.cloud.aiplatform_v1beta1.types as gapic
+import vertexai.generative_models as vertexai  # type: ignore
 from langchain_core.exceptions import OutputParserException
 from langchain_core.output_parsers import BaseOutputParser
 from langchain_core.outputs import ChatGeneration, Generation
-from langchain_core.pydantic_v1 import BaseModel, Field
+from langchain_core.pydantic_v1 import BaseModel
 from langchain_core.tools import BaseTool
 from langchain_core.tools import tool as callable_as_lc_tool
 from langchain_core.utils.function_calling import FunctionDescription
 from langchain_core.utils.json_schema import dereference_refs
-from vertexai.generative_models import FunctionDeclaration  # type: ignore
-from vertexai.generative_models import Tool as VertexTool
 
-# FIXME: vertexai is not exporting ToolConfig
-from vertexai.generative_models._generative_models import ToolConfig  # type: ignore
+logger = logging.getLogger(__name__)
 
-
-def _format_pydantic_to_vertex_function(
-    pydantic_model: Type[BaseModel],
-) -> FunctionDescription:
-    schema = pydantic_model.schema()
-
-    return {
-        "name": schema["title"],
-        "description": schema.get("description", ""),
-        "parameters": _get_parameters_from_schema(schema=schema),
-    }
+_FunctionDeclarationLike = Union[
+    BaseTool,
+    Type[BaseModel],
+    FunctionDescription,
+    Callable,
+    vertexai.FunctionDeclaration,
+    Dict[str, Any],
+]
+_GoogleSearchRetrievalLike = Union[
+    gapic.GoogleSearchRetrieval,
+    Dict[str, Any],
+]
+_RetrievalLike = Union[gapic.Retrieval, Dict[str, Any]]
 
 
-def _format_base_tool_to_vertex_function(tool: BaseTool) -> FunctionDescription:
-    "Format tool into the Vertex function API."
-    if tool.args_schema:
-        schema = tool.args_schema.schema()
+class _ToolDictLike(TypedDict):
+    function_declarations: Optional[List[_FunctionDeclarationLike]]
+    google_search_retrieval: Optional[_GoogleSearchRetrievalLike]
+    retrieval: Optional[_RetrievalLike]
 
-        return {
-            "name": tool.name or schema["title"],
-            "description": tool.description or schema["description"],
-            "parameters": _get_parameters_from_schema(schema=schema),
-        }
-    else:
-        return {
-            "name": tool.name,
-            "description": tool.description,
-            "parameters": {
-                "properties": {
-                    "__arg1": {"type": "string"},
-                },
-                "required": ["__arg1"],
-                "type": "object",
-            },
-        }
 
+_ToolsType = Sequence[
+    Union[gapic.Tool, vertexai.Tool, _ToolDictLike, _FunctionDeclarationLike]
+]
 
-def _format_to_vertex_function_dict(
-    tool: Union[BaseTool, Type[BaseModel], dict, Callable, FunctionDeclaration],
-) -> FunctionDescription:
-    "Format tool into the Vertex function declaration."
-    if isinstance(tool, BaseTool):
-        return _format_base_tool_to_vertex_function(tool)
-    elif isinstance(tool, type) and issubclass(tool, BaseModel):
-        return _format_pydantic_to_vertex_function(tool)
-    elif isinstance(tool, dict):
-        return {
-            "name": tool["name"],
-            "description": tool["description"],
-            "parameters": _get_parameters_from_schema(tool["parameters"]),
-        }
-    elif isinstance(tool, FunctionDeclaration):
-        tool_dict = tool.to_dict()
-        return FunctionDescription(
-            name=tool_dict["name"],
-            description=tool_dict["description"],
-            parameters=tool_dict["parameters"],
-        )
-    elif callable(tool):
-        return _format_base_tool_to_vertex_function(callable_as_lc_tool()(tool))
-    else:
-        raise ValueError(f"Unsupported tool call type {tool}")
+_ALLOWED_SCHEMA_FIELDS = []
+_ALLOWED_SCHEMA_FIELDS.extend([f.name for f in gapic.Schema()._pb.DESCRIPTOR.fields])
+_ALLOWED_SCHEMA_FIELDS.extend(
+    [
+        f
+        for f in gapic.Schema.to_dict(
+            gapic.Schema(), preserving_proto_field_name=False
+        ).keys()
+    ]
+)
+_ALLOWED_SCHEMA_FIELDS_SET = set(_ALLOWED_SCHEMA_FIELDS)
 
 
-_FunctionDeclarationLike = Union[
-    BaseTool, Type[BaseModel], dict, Callable, FunctionDeclaration
-]
+def _format_json_schema_to_gapic(schema: Dict[str, Any]) -> Dict[str, Any]:
+    converted_schema: Dict[str, Any] = {}
+    for key, value in schema.items():
+        if key == "definitions":
+            continue
+        elif key == "items":
+            converted_schema["items"] = _format_json_schema_to_gapic(value)
+        elif key == "properties":
+            if "properties" not in converted_schema:
+                converted_schema["properties"] = {}
+            for pkey, pvalue in value.items():
+                converted_schema["properties"][pkey] = _format_json_schema_to_gapic(
+                    pvalue
+                )
+            continue
+        elif key in ["type", "_type"]:
+            converted_schema["type"] = str(value).upper()
+        elif key not in _ALLOWED_SCHEMA_FIELDS_SET:
+            logger.warning(f"Key '{key}' is not supported in schema, ignoring")
+        else:
+            converted_schema[key] = value
+    return converted_schema
 
 
-class _VertexToolDict(TypedDict):
-    function_declarations: List[FunctionDescription]
+def _dict_to_gapic_schema(schema: Dict[str, Any]) -> gapic.Schema:
+    dereferenced_schema = dereference_refs(schema)
+    formatted_schema = _format_json_schema_to_gapic(dereferenced_schema)
+    json_schema = json.dumps(formatted_schema)
+    return gapic.Schema.from_json(json_schema)
 
 
-def _format_functions_to_vertex_tool_dict(
-    functions: List[_FunctionDeclarationLike],
-) -> _VertexToolDict:
-    "Format tools into the Vertex Tool instance."
-    function_declarations = [_format_to_vertex_function_dict(fn) for fn in functions]
-    return _VertexToolDict(function_declarations=function_declarations)
-
-
-def _format_to_vertex_tool(
-    tool: Union[VertexTool, _VertexToolDict, List[_FunctionDeclarationLike]],
-) -> VertexTool:
-    if isinstance(tool, VertexTool):
-        return tool
-    elif isinstance(tool, (list, dict)):
-        tool = (
-            _format_functions_to_vertex_tool_dict(tool)
-            if isinstance(tool, list)
-            else tool
-        )
-        return VertexTool(
-            function_declarations=[
-                FunctionDeclaration(**fd) for fd in tool["function_declarations"]
-            ]
+def _format_base_tool_to_function_declaration(
+    tool: BaseTool,
+) -> gapic.FunctionDeclaration:
+    "Format tool into the Vertex function API."
+    if not tool.args_schema:
+        return gapic.FunctionDeclaration(
+            name=tool.name,
+            description=tool.description,
+            parameters=gapic.Schema(
+                type=gapic.Type.OBJECT,
+                properties={
+                    "__arg1": gapic.Schema(type=gapic.Type.STRING),
+                },
+                required=["__arg1"],
+            ),
         )
-    else:
-        raise ValueError(f"Unexpected tool value:\n\n{tool=}")
 
+    schema = tool.args_schema.schema()
+    parameters = _dict_to_gapic_schema(schema)
 
-def _format_tool_config(tool_config: _ToolConfigDict) -> Union[ToolConfig, None]:
-    if "function_calling_config" not in tool_config:
-        raise ValueError(
-            "Invalid ToolConfig, missing 'function_calling_config' key. Received:\n\n"
-            f"{tool_config=}"
-        )
-    return ToolConfig(
-        function_calling_config=ToolConfig.FunctionCallingConfig(
-            **tool_config["function_calling_config"]
-        )
+    return gapic.FunctionDeclaration(
+        name=tool.name or schema.get("title"),
+        description=tool.description or schema.get("description"),
+        parameters=parameters,
     )
 
 
-class ParametersSchema(BaseModel):
-    """
-    This is a schema of currently supported definitions in function calling.
-    We need explicitly exclude `definitions` field
-    as it is not currently supported.
+def _format_pydantic_to_function_declaration(
+    pydantic_model: Type[BaseModel],
+) -> gapic.FunctionDeclaration:
+    schema = pydantic_model.schema()
 
-    All other fields will be passed through (as extra fields are allowed)
-    and intercepted on `google.cloud.aiplatform` level
-    """
+    return gapic.FunctionDeclaration(
+        name=schema["title"],
+        description=schema.get("description", ""),
+        parameters=_dict_to_gapic_schema(schema),
+    )
 
-    definitions: Optional[Any] = Field(exclude=True)
-    items: Optional["ParametersSchema"]
-    properties: Optional[Dict[str, "ParametersSchema"]]
 
-    class Config:
-        extra = "allow"
+def _format_dict_to_function_declaration(
+    tool: Union[FunctionDescription, Dict[str, Any]],
+) -> gapic.FunctionDeclaration:
+    return gapic.FunctionDeclaration(
+        name=tool.get("name"),
+        description=tool.get("description"),
+        parameters=_dict_to_gapic_schema(tool.get("parameters", {})),
+    )
 
 
-def _get_parameters_from_schema(schema: Dict[str, Any]) -> Dict[str, Any]:
-    """Given a schema, format the parameters key to match VertexAI
-    expected input.
+def _format_vertex_to_function_declaration(
+    tool: vertexai.FunctionDeclaration,
+) -> gapic.FunctionDeclaration:
+    tool_dict = tool.to_dict()
+    return _format_dict_to_function_declaration(tool_dict)
 
-    Args:
-        schema: Dictionary that must have the following keys.
 
-    Returns:
-        Dictionary with the formatted parameters.
-    """
+def _format_to_gapic_function_declaration(
+    tool: _FunctionDeclarationLike,
+) -> gapic.FunctionDeclaration:
+    "Format tool into the Vertex function declaration."
+    if isinstance(tool, BaseTool):
+        return _format_base_tool_to_function_declaration(tool)
+    elif isinstance(tool, type) and issubclass(tool, BaseModel):
+        return _format_pydantic_to_function_declaration(tool)
+    elif callable(tool):
+        return _format_base_tool_to_function_declaration(callable_as_lc_tool()(tool))
+    elif isinstance(tool, vertexai.FunctionDeclaration):
+        return _format_vertex_to_function_declaration(tool)
+    elif isinstance(tool, dict):
+        return _format_dict_to_function_declaration(tool)
+    else:
+        raise ValueError(f"Unsupported tool call type {tool}")
 
-    dereferenced_schema = dereference_refs(schema)
-    model = ParametersSchema.parse_obj(dereferenced_schema)
 
-    return model.dict(exclude_unset=True)
+def _format_to_gapic_tool(
+    tools: _ToolsType,
+) -> gapic.Tool:
+    gapic_tool = gapic.Tool()
+    for tool in tools:
+        if any(f in gapic_tool for f in ["google_search_retrieval", "retrieval"]):
+            raise ValueError(
+                "Providing multiple retrieval, google_search_retrieval"
+                " or mixing with function_declarations is not supported"
+            )
+        if isinstance(tool, (gapic.Tool, vertexai.Tool)):
+            rt = (
+                tool if isinstance(tool, gapic.Tool) else tool._raw_tool  # type: ignore
+            )
+            if "retrieval" in rt:
+                gapic_tool.retrieval = rt.retrieval
+            if "google_search_retrieval" in rt:
+                gapic_tool.google_search_retrieval = rt.google_search_retrieval
+            if "function_declarations" in rt:
+                gapic_tool.function_declarations.extend(rt.function_declarations)
+        elif isinstance(tool, dict):
+            # not _ToolDictLike
+            if not any(
+                f in tool
+                for f in [
+                    "function_declarations",
+                    "google_search_retrieval",
+                    "retrieval",
+                ]
+            ):
+                fd = _format_to_gapic_function_declaration(tool)
+                gapic_tool.function_declarations.append(fd)
+                continue
+            # _ToolDictLike
+            tool = cast(_ToolDictLike, tool)
+            if "function_declarations" in tool:
+                function_declarations = tool["function_declarations"]
+                if not isinstance(tool["function_declarations"], list):
+                    raise ValueError(
+                        "function_declarations should be a list"
+                        f"got '{type(function_declarations)}'"
+                    )
+                if function_declarations:
+                    fds = [
+                        _format_to_gapic_function_declaration(fd)
+                        for fd in function_declarations
+                    ]
+                    gapic_tool.function_declarations.extend(fds)
+            if "google_search_retrieval" in tool:
+                gapic_tool.google_search_retrieval = gapic.GoogleSearchRetrieval(
+                    tool["google_search_retrieval"]
+                )
+            if "retrieval" in tool:
+                gapic_tool.retrieval = gapic.Retrieval(tool["retrieval"])
+        else:
+            fd = _format_to_gapic_function_declaration(tool)
+            gapic_tool.function_declarations.append(fd)
+    return gapic_tool
 
 
 class PydanticFunctionsOutputParser(BaseOutputParser):
     """Parse an output as a pydantic object.
 
     This parser is used to parse the output of a ChatModel that uses
     Google Vertex function format to invoke functions.
@@ -238,44 +294,57 @@
             raise OutputParserException(f"Could not parse function call: {message}")
 
     def parse(self, text: str) -> BaseModel:
         raise ValueError("Can only parse messages")
 
 
 class _FunctionCallingConfigDict(TypedDict):
-    mode: ToolConfig.FunctionCallingConfig.Mode
+    mode: Union[gapic.FunctionCallingConfig.Mode, int]
     allowed_function_names: Optional[List[str]]
 
 
 class _ToolConfigDict(TypedDict):
     function_calling_config: _FunctionCallingConfigDict
 
 
 _ToolChoiceType = Union[
     dict, List[str], str, Literal["auto", "none", "any"], Literal[True]
 ]
 
 
+def _format_tool_config(tool_config: _ToolConfigDict) -> Union[gapic.ToolConfig, None]:
+    if "function_calling_config" not in tool_config:
+        raise ValueError(
+            "Invalid ToolConfig, missing 'function_calling_config' key. Received:\n\n"
+            f"{tool_config=}"
+        )
+    return gapic.ToolConfig(
+        function_calling_config=gapic.FunctionCallingConfig(
+            **tool_config["function_calling_config"]
+        )
+    )
+
+
 def _tool_choice_to_tool_config(
     tool_choice: _ToolChoiceType,
     all_names: List[str],
 ) -> _ToolConfigDict:
     allowed_function_names: Optional[List[str]] = None
     if tool_choice is True or tool_choice == "any":
-        mode = ToolConfig.FunctionCallingConfig.Mode.ANY
+        mode = gapic.FunctionCallingConfig.Mode.ANY
         allowed_function_names = all_names
     elif tool_choice == "auto":
-        mode = ToolConfig.FunctionCallingConfig.Mode.AUTO
+        mode = gapic.FunctionCallingConfig.Mode.AUTO
     elif tool_choice == "none":
-        mode = ToolConfig.FunctionCallingConfig.Mode.NONE
+        mode = gapic.FunctionCallingConfig.Mode.NONE
     elif isinstance(tool_choice, str):
-        mode = ToolConfig.FunctionCallingConfig.Mode.ANY
+        mode = gapic.FunctionCallingConfig.Mode.ANY
         allowed_function_names = [tool_choice]
     elif isinstance(tool_choice, list):
-        mode = ToolConfig.FunctionCallingConfig.Mode.ANY
+        mode = gapic.FunctionCallingConfig.Mode.ANY
         allowed_function_names = tool_choice
     elif isinstance(tool_choice, dict):
         if "mode" in tool_choice:
             mode = tool_choice["mode"]
             allowed_function_names = tool_choice.get("allowed_function_names")
         elif "function_calling_config" in tool_choice:
             mode = tool_choice["function_calling_config"]["mode"]
```

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/gemma.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/gemma.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/llms.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,18 @@
 from vertexai.preview.language_models import (  # type: ignore[import-untyped]
     CodeGenerationModel as PreviewCodeGenerationModel,
 )
 from vertexai.preview.language_models import (
     TextGenerationModel as PreviewTextGenerationModel,
 )
 
-from langchain_google_vertexai._base import (
-    _VertexAICommon,
-)
+from langchain_google_vertexai._base import GoogleModelFamily, _VertexAICommon
 from langchain_google_vertexai._utils import (
     create_retry_decorator,
     get_generation_info,
-    is_codey_model,
     is_gemini_model,
 )
 
 
 def _completion_with_retry(
     llm: VertexAI,
     prompt: List[Union[str, Image]],
@@ -137,23 +134,23 @@
         """Get the namespace of the langchain object."""
         return ["langchain", "llms", "vertexai"]
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that the python package exists in environment."""
         tuned_model_name = values.get("tuned_model_name")
-        model_name = values["model_name"]
         safety_settings = values["safety_settings"]
-        is_gemini = is_gemini_model(values["model_name"])
+        values["model_family"] = GoogleModelFamily(values["model_name"])
+        is_gemini = is_gemini_model(values["model_family"])
         cls._init_vertexai(values)
 
         if safety_settings and (not is_gemini or tuned_model_name):
             raise ValueError("Safety settings are only supported for Gemini models")
 
-        if is_codey_model(model_name):
+        if values["model_family"] == GoogleModelFamily.CODEY:
             model_cls = CodeGenerationModel
             preview_model_cls = PreviewCodeGenerationModel
         elif is_gemini:
             model_cls = GenerativeModel
             preview_model_cls = GenerativeModel
         else:
             model_cls = TextGenerationModel
```

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/model_garden.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/model_garden.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 
 
 class ChatAnthropicVertex(_VertexAICommon, BaseChatModel):
     async_client: Any = None  #: :meta private:
     model_name: Optional[str] = Field(default=None, alias="model")  # type: ignore[assignment]
     "Underlying model name."
     max_output_tokens: int = Field(default=1024, alias="max_tokens")
+    access_token: Optional[str] = None
 
     class Config:
         """Configuration for this pydantic object."""
 
         allow_population_by_field_name = True
 
     @root_validator()
@@ -113,19 +114,21 @@
             AsyncAnthropicVertex,
         )
 
         values["client"] = AnthropicVertex(
             project_id=values["project"],
             region=values["location"],
             max_retries=values["max_retries"],
+            access_token=values["access_token"],
         )
         values["async_client"] = AsyncAnthropicVertex(
             project_id=values["project"],
             region=values["location"],
             max_retries=values["max_retries"],
+            access_token=values["access_token"],
         )
         return values
 
     @property
     def _default_params(self):
         return {
             "model": self.model_name,
```

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/_sdk_manager.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/vectorstores/_sdk_manager.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/_searcher.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/vectorstores/_searcher.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/_utils.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/vectorstores/_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/document_storage.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/vectorstores/document_storage.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/vectorstores/vectorstores.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/vectorstores/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.3/langchain_google_vertexai/vision_models.py` & `langchain_google_vertexai-1.0.4/langchain_google_vertexai/vision_models.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-1.0.3/pyproject.toml` & `langchain_google_vertexai-1.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 [tool.poetry]
 name = "langchain-google-vertexai"
-
-version = "1.0.3"
+version = "1.0.4"
 description = "An integration package connecting Google VertexAI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-google"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain-google/tree/main/libs/vertexai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.42"
+langchain-core = ">=0.1.42,<0.3"
 google-cloud-aiplatform = "^1.47.0"
 google-cloud-storage = "^2.14.0"
-types-requests = "^2.31.0"
-types-protobuf = "^4.24.0.4"
 # optional dependencies
-anthropic = {extras = ["vertexai"], version = ">=0.23.0,<1", optional = true}
+anthropic = { extras = ["vertexai"], version = ">=0.23.0,<1", optional = true }
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
-langchain = "^0.1.6"
+langchain = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/langchain" }
+langchain-text-splitters = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/text-splitters" }
 types-requests = "^2.31.0.20231231"
 types-protobuf = "^4.24.0.4"
 numexpr = "^2.8.6"
 google-api-python-client = "^2.117.0"
-langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
+langchain-core = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core" }
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
@@ -57,19 +55,21 @@
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^1"
 types-google-cloud-ndb = "^2.2.0.20240106"
-langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
+types-protobuf = "^4.24.0.4"
+types-requests = "^2.31.0"
+langchain-core = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core" }
 
 
 [tool.poetry.group.dev.dependencies]
-langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
+langchain-core = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core" }
 
 [tool.poetry.extras]
 anthropic = ["anthropic"]
 
 [tool.ruff]
 select = [
   "E", # pycodestyle
```

### Comparing `langchain_google_vertexai-1.0.3/PKG-INFO` & `langchain_google_vertexai-1.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: langchain-google-vertexai
-Version: 1.0.3
+Version: 1.0.4
 Summary: An integration package connecting Google VertexAI and LangChain
 Home-page: https://github.com/langchain-ai/langchain-google
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: anthropic
 Requires-Dist: anthropic[vertexai] (>=0.23.0,<1) ; extra == "anthropic"
 Requires-Dist: google-cloud-aiplatform (>=1.47.0,<2.0.0)
 Requires-Dist: google-cloud-storage (>=2.14.0,<3.0.0)
-Requires-Dist: langchain-core (>=0.1.42,<0.2.0)
-Requires-Dist: types-protobuf (>=4.24.0.4,<5.0.0.0)
-Requires-Dist: types-requests (>=2.31.0,<3.0.0)
+Requires-Dist: langchain-core (>=0.1.42,<0.3)
 Project-URL: Repository, https://github.com/langchain-ai/langchain-google
 Project-URL: Source Code, https://github.com/langchain-ai/langchain-google/tree/main/libs/vertexai
 Description-Content-Type: text/markdown
 
 # langchain-google-vertexai
 
 This package contains the LangChain integrations for Google Cloud generative models.
```

