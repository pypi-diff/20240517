# Comparing `tmp/llama_index_llms_ollama-0.1.3.tar.gz` & `tmp/llama_index_llms_ollama-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_ollama-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_llms_ollama-0.1.4.tar", max compression
```

## Comparing `llama_index_llms_ollama-0.1.3.tar` & `llama_index_llms_ollama-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       38 2024-04-29 16:10:27.601557 llama_index_llms_ollama-0.1.3/README.md
--rw-r--r--   0        0        0       70 2024-04-29 16:10:27.601557 llama_index_llms_ollama-0.1.3/llama_index/llms/ollama/__init__.py
--rw-r--r--   0        0        0    13809 2024-04-29 16:10:27.601557 llama_index_llms_ollama-0.1.3/llama_index/llms/ollama/base.py
--rw-r--r--   0        0        0     1421 2024-04-29 16:10:27.601557 llama_index_llms_ollama-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 llama_index_llms_ollama-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       38 2024-05-17 20:26:28.909530 llama_index_llms_ollama-0.1.4/README.md
+-rw-r--r--   0        0        0       70 2024-05-17 20:26:28.909530 llama_index_llms_ollama-0.1.4/llama_index/llms/ollama/__init__.py
+-rw-r--r--   0        0        0    12406 2024-05-17 20:26:28.909530 llama_index_llms_ollama-0.1.4/llama_index/llms/ollama/base.py
+-rw-r--r--   0        0        0     1421 2024-05-17 20:26:28.909530 llama_index_llms_ollama-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 llama_index_llms_ollama-0.1.4/PKG-INFO
```

### Comparing `llama_index_llms_ollama-0.1.3/llama_index/llms/ollama/base.py` & `llama_index_llms_ollama-0.1.4/llama_index/llms/ollama/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,56 +144,14 @@
                     ),
                 ),
                 raw=raw,
                 additional_kwargs=get_additional_kwargs(raw, ("message",)),
             )
 
     @llm_chat_callback()
-    async def achat(
-        self, messages: Sequence[ChatMessage], **kwargs: Any
-    ) -> ChatResponse:
-        payload = {
-            "model": self.model,
-            "messages": [
-                {
-                    "role": message.role.value,
-                    "content": message.content,
-                    **message.additional_kwargs,
-                }
-                for message in messages
-            ],
-            "options": self._model_kwargs,
-            "stream": False,
-            **kwargs,
-        }
-
-        if self.json_mode:
-            payload["format"] = "json"
-
-        async with httpx.AsyncClient(timeout=Timeout(self.request_timeout)) as client:
-            response = await client.post(
-                url=f"{self.base_url}/api/chat",
-                json=payload,
-            )
-            response.raise_for_status()
-            raw = response.json()
-            message = raw["message"]
-            return ChatResponse(
-                message=ChatMessage(
-                    content=message.get("content"),
-                    role=MessageRole(message.get("role")),
-                    additional_kwargs=get_additional_kwargs(
-                        message, ("content", "role")
-                    ),
-                ),
-                raw=raw,
-                additional_kwargs=get_additional_kwargs(raw, ("message",)),
-            )
-
-    @llm_chat_callback()
     def stream_chat(
         self, messages: Sequence[ChatMessage], **kwargs: Any
     ) -> ChatResponseGen:
         payload = {
             "model": self.model,
             "messages": [
                 {
```

### Comparing `llama_index_llms_ollama-0.1.3/pyproject.toml` & `llama_index_llms_ollama-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms ollama integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-ollama"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_llms_ollama-0.1.3/PKG-INFO` & `llama_index_llms_ollama-0.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-ollama
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index llms ollama integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

