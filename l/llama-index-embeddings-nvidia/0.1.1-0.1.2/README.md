# Comparing `tmp/llama_index_embeddings_nvidia-0.1.1.tar.gz` & `tmp/llama_index_embeddings_nvidia-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_nvidia-0.1.1.tar", max compression
+gzip compressed data, was "llama_index_embeddings_nvidia-0.1.2.tar", max compression
```

## Comparing `llama_index_embeddings_nvidia-0.1.1.tar` & `llama_index_embeddings_nvidia-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      694 2024-05-08 14:33:52.759347 llama_index_embeddings_nvidia-0.1.1/README.md
--rw-r--r--   0        0        0       94 2024-05-08 14:33:52.759347 llama_index_embeddings_nvidia-0.1.1/llama_index/embeddings/nvidia/__init__.py
--rw-r--r--   0        0        0     6584 2024-05-08 14:33:52.759347 llama_index_embeddings_nvidia-0.1.1/llama_index/embeddings/nvidia/base.py
--rw-r--r--   0        0        0     1578 2024-05-08 14:33:52.759347 llama_index_embeddings_nvidia-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1253 1970-01-01 00:00:00.000000 llama_index_embeddings_nvidia-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      694 2024-05-17 19:22:01.708840 llama_index_embeddings_nvidia-0.1.2/README.md
+-rw-r--r--   0        0        0       94 2024-05-17 19:22:01.708840 llama_index_embeddings_nvidia-0.1.2/llama_index/embeddings/nvidia/__init__.py
+-rw-r--r--   0        0        0     7164 2024-05-17 19:22:01.708840 llama_index_embeddings_nvidia-0.1.2/llama_index/embeddings/nvidia/base.py
+-rw-r--r--   0        0        0     1578 2024-05-17 19:22:01.708840 llama_index_embeddings_nvidia-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1253 1970-01-01 00:00:00.000000 llama_index_embeddings_nvidia-0.1.2/PKG-INFO
```

### Comparing `llama_index_embeddings_nvidia-0.1.1/README.md` & `llama_index_embeddings_nvidia-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_embeddings_nvidia-0.1.1/llama_index/embeddings/nvidia/base.py` & `llama_index_embeddings_nvidia-0.1.2/llama_index/embeddings/nvidia/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 from llama_index.core.base.llms.generic_utils import get_from_param_or_env
 
 from openai import OpenAI, AsyncOpenAI
 
 BASE_RETRIEVAL_URL = "https://ai.api.nvidia.com/v1/retrieval/nvidia"
 DEFAULT_MODEL = "NV-Embed-QA"
 
+MODEL_ENDPOINT_MAP = {
+    DEFAULT_MODEL: BASE_RETRIEVAL_URL,
+    "snowflake/arctic-embed-l": "https://ai.api.nvidia.com/v1/retrieval/snowflake/arctic-embed-l",
+}
+
 
 class Model(BaseModel):
     id: str
 
 
 class NVIDIAEmbedding(BaseEmbedding):
     """NVIDIA embeddings."""
@@ -65,25 +70,31 @@
         if embed_batch_size > 259:
             raise ValueError("The batch size should not be larger than 259.")
 
         api_key = get_from_param_or_env(
             "api_key", nvidia_api_key or api_key, "NVIDIA_API_KEY", "none"
         )
 
+        # TODO: we should not assume unknown models are at the base url, but
+        #       we cannot error out here because
+        #          NVIDIAEmbedding(model="special").mode("nim", base_url=...)
+        #       is valid usage
+        base_url = MODEL_ENDPOINT_MAP.get(model, BASE_RETRIEVAL_URL)
+
         self._client = OpenAI(
             api_key=api_key,
-            base_url=BASE_RETRIEVAL_URL,
+            base_url=base_url,
             timeout=timeout,
             max_retries=max_retries,
         )
         self._client._custom_headers = {"User-Agent": "llama-index-embeddings-nvidia"}
 
         self._aclient = AsyncOpenAI(
             api_key=api_key,
-            base_url=BASE_RETRIEVAL_URL,
+            base_url=base_url,
             timeout=timeout,
             max_retries=max_retries,
         )
         self._aclient._custom_headers = {"User-Agent": "llama-index-embeddings-nvidia"}
 
         super().__init__(
             model=model,
@@ -91,15 +102,15 @@
             callback_manager=callback_manager,
             **kwargs,
         )
 
     @property
     def available_models(self) -> List[Model]:
         """Get available models."""
-        ids = [DEFAULT_MODEL]
+        ids = MODEL_ENDPOINT_MAP.keys()
         if self._mode == "nim":
             ids = [model.id for model in self._client.models.list()]
         return [Model(id=id) for id in ids]
 
     @classmethod
     def class_name(cls) -> str:
         return "NVIDIAEmbedding"
@@ -112,15 +123,16 @@
         model: Optional[str] = None,
         api_key: Optional[str] = None,
     ) -> "NVIDIAEmbedding":
         if mode == "nim":
             if not base_url:
                 raise ValueError("base_url is required for nim mode")
         if not base_url:
-            base_url = BASE_RETRIEVAL_URL
+            # TODO: we should not assume unknown models are at the base url
+            base_url = MODEL_ENDPOINT_MAP.get(model or self.model, BASE_RETRIEVAL_URL)
 
         self._mode = mode
         if base_url:
             self._client.base_url = base_url
             self._aclient.base_url = base_url
         if model:
             self.model = model
```

### Comparing `llama_index_embeddings_nvidia-0.1.1/pyproject.toml` & `llama_index_embeddings_nvidia-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings nvidia integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-nvidia"
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.9"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_embeddings_nvidia-0.1.1/PKG-INFO` & `llama_index_embeddings_nvidia-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-nvidia
-Version: 0.1.1
+Version: 0.1.2
 Summary: llama-index embeddings nvidia integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

