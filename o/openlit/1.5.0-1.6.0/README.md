# Comparing `tmp/openlit-1.5.0.tar.gz` & `tmp/openlit-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlit-1.5.0.tar", max compression
+gzip compressed data, was "openlit-1.6.0.tar", max compression
```

## Comparing `openlit-1.5.0.tar` & `openlit-1.6.0.tar`

### file list

```diff
@@ -1,44 +1,47 @@
--rw-r--r--   0        0        0    11357 2024-05-16 12:58:46.987118 openlit-1.5.0/LICENSE
--rw-r--r--   0        0        0    10846 2024-05-16 12:58:46.987118 openlit-1.5.0/README.md
--rw-r--r--   0        0        0      966 2024-05-16 12:58:46.987118 openlit-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     4651 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/__helpers.py
--rw-r--r--   0        0        0     9647 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/__init__.py
--rw-r--r--   0        0        0     1955 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0    16026 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/anthropic/anthropic.py
--rw-r--r--   0        0        0    16068 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/anthropic/async_anthropic.py
--rw-r--r--   0        0        0     1540 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/bedrock/__init__.py
--rw-r--r--   0        0        0    22278 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/bedrock/bedrock.py
--rw-r--r--   0        0        0     3253 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0    10407 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/chroma/chroma.py
--rw-r--r--   0        0        0     1920 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0    20381 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/cohere/cohere.py
--rw-r--r--   0        0        0     1911 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/groq/__init__.py
--rw-r--r--   0        0        0    19084 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/groq/async_groq.py
--rw-r--r--   0        0        0    19048 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/groq/groq.py
--rw-r--r--   0        0        0     1758 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/haystack/__init__.py
--rw-r--r--   0        0        0     3891 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/haystack/haystack.py
--rw-r--r--   0        0        0     2531 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     7639 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/langchain/langchain.py
--rw-r--r--   0        0        0     1973 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     4048 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/llamaindex/llamaindex.py
--rw-r--r--   0        0        0     3156 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/mistral/__init__.py
--rw-r--r--   0        0        0    21361 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/mistral/async_mistral.py
--rw-r--r--   0        0        0    21212 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/mistral/mistral.py
--rw-r--r--   0        0        0    16265 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0    46297 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/openai/async_azure_openai.py
--rw-r--r--   0        0        0    45841 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/openai/async_openai.py
--rw-r--r--   0        0        0    46091 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/openai/azure_openai.py
--rw-r--r--   0        0        0    46522 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/openai/openai.py
--rw-r--r--   0        0        0     2526 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     8765 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/pinecone/pinecone.py
--rw-r--r--   0        0        0     4799 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0    14436 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/qdrant/qdrant.py
--rw-r--r--   0        0        0     1478 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/transformers/__init__.py
--rw-r--r--   0        0        0     7592 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/transformers/transformers.py
--rw-r--r--   0        0        0     6079 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/vertexai/__init__.py
--rw-r--r--   0        0        0    52372 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/vertexai/async_vertexai.py
--rw-r--r--   0        0        0    52125 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/instrumentation/vertexai/vertexai.py
--rw-r--r--   0        0        0     4291 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/otel/metrics.py
--rw-r--r--   0        0        0     3712 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/otel/tracing.py
--rw-r--r--   0        0        0     6168 2024-05-16 12:58:46.987118 openlit-1.5.0/src/openlit/semcov/__init__.py
--rw-r--r--   0        0        0    12146 1970-01-01 00:00:00.000000 openlit-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-17 10:26:35.699756 openlit-1.6.0/LICENSE
+-rw-r--r--   0        0        0    10913 2024-05-17 10:26:35.699756 openlit-1.6.0/README.md
+-rw-r--r--   0        0        0      966 2024-05-17 10:26:35.699756 openlit-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4651 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/__helpers.py
+-rw-r--r--   0        0        0     9781 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/__init__.py
+-rw-r--r--   0        0        0     1955 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0    16026 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/anthropic/anthropic.py
+-rw-r--r--   0        0        0    16068 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/anthropic/async_anthropic.py
+-rw-r--r--   0        0        0     1540 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0    22278 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/bedrock/bedrock.py
+-rw-r--r--   0        0        0     3253 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0    10407 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/chroma/chroma.py
+-rw-r--r--   0        0        0     1920 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0    20381 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/cohere/cohere.py
+-rw-r--r--   0        0        0     1911 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/groq/__init__.py
+-rw-r--r--   0        0        0    19084 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/groq/async_groq.py
+-rw-r--r--   0        0        0    19048 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/groq/groq.py
+-rw-r--r--   0        0        0     1758 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/haystack/__init__.py
+-rw-r--r--   0        0        0     3891 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/haystack/haystack.py
+-rw-r--r--   0        0        0     2531 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     7639 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/langchain/langchain.py
+-rw-r--r--   0        0        0     1973 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     4048 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/llamaindex/llamaindex.py
+-rw-r--r--   0        0        0     3156 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/mistral/__init__.py
+-rw-r--r--   0        0        0    21361 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/mistral/async_mistral.py
+-rw-r--r--   0        0        0    21212 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/mistral/mistral.py
+-rw-r--r--   0        0        0     3812 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/ollama/__init__.py
+-rw-r--r--   0        0        0    28991 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/ollama/async_ollama.py
+-rw-r--r--   0        0        0    28901 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/ollama/ollama.py
+-rw-r--r--   0        0        0    16265 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0    46297 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/openai/async_azure_openai.py
+-rw-r--r--   0        0        0    45841 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/openai/async_openai.py
+-rw-r--r--   0        0        0    46091 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/openai/azure_openai.py
+-rw-r--r--   0        0        0    46522 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/openai/openai.py
+-rw-r--r--   0        0        0     2526 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     8765 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/pinecone/pinecone.py
+-rw-r--r--   0        0        0     4799 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0    14436 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/qdrant/qdrant.py
+-rw-r--r--   0        0        0     1478 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/transformers/__init__.py
+-rw-r--r--   0        0        0     7592 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/transformers/transformers.py
+-rw-r--r--   0        0        0     6079 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/vertexai/__init__.py
+-rw-r--r--   0        0        0    52372 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/vertexai/async_vertexai.py
+-rw-r--r--   0        0        0    52125 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/instrumentation/vertexai/vertexai.py
+-rw-r--r--   0        0        0     4291 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/otel/metrics.py
+-rw-r--r--   0        0        0     3712 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/otel/tracing.py
+-rw-r--r--   0        0        0     6204 2024-05-17 10:26:35.699756 openlit-1.6.0/src/openlit/semcov/__init__.py
+-rw-r--r--   0        0        0    12213 1970-01-01 00:00:00.000000 openlit-1.6.0/PKG-INFO
```

### Comparing `openlit-1.5.0/LICENSE` & `openlit-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/README.md` & `openlit-1.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 This project adheres to the [Semantic Conventions](https://github.com/open-telemetry/semantic-conventions/tree/main/docs/gen-ai) proposed by the OpenTelemetry community. You can check out the current definitions [here](src/openlit/semcov/__init__.py).
 
 ## What can be Auto Instrumented?
 
 ### LLMs
 - [✅ OpenAI](https://docs.openlit.io/latest/integrations/openai)
+- [✅ Ollama](https://docs.openlit.io/latest/integrations/ollama)
 - [✅ Anthropic](https://docs.openlit.io/latest/integrations/anthropic)
 - [✅ Cohere](https://docs.openlit.io/latest/integrations/cohere)
 - [✅ Mistral](https://docs.openlit.io/latest/integrations/mistral)
 - [✅ Azure OpenAI](https://docs.openlit.io/latest/integrations/azure-openai)
 - [✅ HuggingFace Transformers](https://docs.openlit.io/latest/integrations/huggingface)
 - [✅ Amazon Bedrock](https://docs.openlit.io/latest/integrations/bedrock)
 - [✅ Vertex AI](https://docs.openlit.io/latest/integrations/vertexai)
```

### Comparing `openlit-1.5.0/pyproject.toml` & `openlit-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openlit"
-version = "1.5.0"
+version = "1.6.0"
 description = "OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects"
 authors = ["OpenLIT"]
 repository = "https://github.com/openlit/openlit/tree/main/openlit/python"
 readme = "README.md"
 homepage = "https://github.com/openlit/openlit/tree/main/openlit/python"
 keywords = ["OpenTelemetry", "otel", "otlp","llm", "tracing", "openai", "anthropic", "claude", "cohere", "llm monitoring", "observability", "monitoring", "gpt", "Generative AI", "chatGPT"]
```

### Comparing `openlit-1.5.0/src/openlit/__helpers.py` & `openlit-1.6.0/src/openlit/__helpers.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/__init__.py` & `openlit-1.6.0/src/openlit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from openlit.instrumentation.openai import OpenAIInstrumentor
 from openlit.instrumentation.anthropic import AnthropicInstrumentor
 from openlit.instrumentation.cohere import CohereInstrumentor
 from openlit.instrumentation.mistral import MistralInstrumentor
 from openlit.instrumentation.bedrock import BedrockInstrumentor
 from openlit.instrumentation.vertexai import VertexAIInstrumentor
 from openlit.instrumentation.groq import GroqInstrumentor
+from openlit.instrumentation.ollama import OllamaInstrumentor
 from openlit.instrumentation.langchain import LangChainInstrumentor
 from openlit.instrumentation.llamaindex import LlamaIndexInstrumentor
 from openlit.instrumentation.haystack import HaystackInstrumentor
 from openlit.instrumentation.chroma import ChromaInstrumentor
 from openlit.instrumentation.pinecone import PineconeInstrumentor
 from openlit.instrumentation.qdrant import QdrantInstrumentor
 from openlit.instrumentation.transformers import TransformersInstrumentor
@@ -150,14 +151,15 @@
         "openai": "openai",
         "anthropic": "anthropic",  
         "cohere": "cohere",  
         "mistral": "mistralai",
         "bedrock": "boto3",
         "vertexai": "vertexai",
         "groq": "groq",
+        "ollama": "ollama",
         "langchain": "langchain",
         "llama_index": "llama_index",
         "haystack": "haystack",
         "chroma": "chromadb",
         "pinecone": "pinecone",
         "qdrant": "qdrant_client",
         "transformers": "transformers"
@@ -202,14 +204,15 @@
             "openai": OpenAIInstrumentor(),
             "anthropic": AnthropicInstrumentor(),
             "cohere": CohereInstrumentor(),
             "mistral": MistralInstrumentor(),
             "bedrock": BedrockInstrumentor(),
             "vertexai": VertexAIInstrumentor(),
             "groq": GroqInstrumentor(),
+            "ollama": OllamaInstrumentor(),
             "langchain": LangChainInstrumentor(),
             "llama_index": LlamaIndexInstrumentor(),
             "haystack": HaystackInstrumentor(),
             "chroma": ChromaInstrumentor(),
             "pinecone": PineconeInstrumentor(),
             "qdrant": QdrantInstrumentor(),
             "transformers": TransformersInstrumentor()
```

### Comparing `openlit-1.5.0/src/openlit/instrumentation/anthropic/__init__.py` & `openlit-1.6.0/src/openlit/instrumentation/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/anthropic/anthropic.py` & `openlit-1.6.0/src/openlit/instrumentation/anthropic/anthropic.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/anthropic/async_anthropic.py` & `openlit-1.6.0/src/openlit/instrumentation/anthropic/async_anthropic.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/bedrock/__init__.py` & `openlit-1.6.0/src/openlit/instrumentation/bedrock/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/bedrock/bedrock.py` & `openlit-1.6.0/src/openlit/instrumentation/bedrock/bedrock.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/chroma/__init__.py` & `openlit-1.6.0/src/openlit/instrumentation/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/chroma/chroma.py` & `openlit-1.6.0/src/openlit/instrumentation/chroma/chroma.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/cohere/__init__.py` & `openlit-1.6.0/src/openlit/instrumentation/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/cohere/cohere.py` & `openlit-1.6.0/src/openlit/instrumentation/cohere/cohere.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/groq/__init__.py` & `openlit-1.6.0/src/openlit/instrumentation/groq/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/groq/async_groq.py` & `openlit-1.6.0/src/openlit/instrumentation/groq/async_groq.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/groq/groq.py` & `openlit-1.6.0/src/openlit/instrumentation/groq/groq.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/haystack/__init__.py` & `openlit-1.6.0/src/openlit/instrumentation/haystack/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/haystack/haystack.py` & `openlit-1.6.0/src/openlit/instrumentation/haystack/haystack.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/langchain/__init__.py` & `openlit-1.6.0/src/openlit/instrumentation/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/langchain/langchain.py` & `openlit-1.6.0/src/openlit/instrumentation/langchain/langchain.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/llamaindex/__init__.py` & `openlit-1.6.0/src/openlit/instrumentation/llamaindex/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/llamaindex/llamaindex.py` & `openlit-1.6.0/src/openlit/instrumentation/llamaindex/llamaindex.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/mistral/__init__.py` & `openlit-1.6.0/src/openlit/instrumentation/mistral/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/mistral/async_mistral.py` & `openlit-1.6.0/src/openlit/instrumentation/mistral/async_mistral.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/mistral/mistral.py` & `openlit-1.6.0/src/openlit/instrumentation/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/openai/__init__.py` & `openlit-1.6.0/src/openlit/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/openai/async_azure_openai.py` & `openlit-1.6.0/src/openlit/instrumentation/openai/async_azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/openai/async_openai.py` & `openlit-1.6.0/src/openlit/instrumentation/openai/async_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/openai/azure_openai.py` & `openlit-1.6.0/src/openlit/instrumentation/openai/azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/openai/openai.py` & `openlit-1.6.0/src/openlit/instrumentation/openai/openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/pinecone/__init__.py` & `openlit-1.6.0/src/openlit/instrumentation/pinecone/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/pinecone/pinecone.py` & `openlit-1.6.0/src/openlit/instrumentation/pinecone/pinecone.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/qdrant/__init__.py` & `openlit-1.6.0/src/openlit/instrumentation/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/qdrant/qdrant.py` & `openlit-1.6.0/src/openlit/instrumentation/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/transformers/__init__.py` & `openlit-1.6.0/src/openlit/instrumentation/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/transformers/transformers.py` & `openlit-1.6.0/src/openlit/instrumentation/transformers/transformers.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/vertexai/__init__.py` & `openlit-1.6.0/src/openlit/instrumentation/vertexai/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/vertexai/async_vertexai.py` & `openlit-1.6.0/src/openlit/instrumentation/vertexai/async_vertexai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/instrumentation/vertexai/vertexai.py` & `openlit-1.6.0/src/openlit/instrumentation/vertexai/vertexai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/otel/metrics.py` & `openlit-1.6.0/src/openlit/otel/metrics.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/otel/tracing.py` & `openlit-1.6.0/src/openlit/otel/tracing.py`

 * *Files identical despite different names*

### Comparing `openlit-1.5.0/src/openlit/semcov/__init__.py` & `openlit-1.6.0/src/openlit/semcov/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     GEN_AI_SYSTEM_AZURE_OPENAI = "azure_openai"
     GEN_AI_SYSTEM_ANTHROPIC = "anthropic"
     GEN_AI_SYSTEM_COHERE = "cohere"
     GEN_AI_SYSTEM_MISTRAL = "mistral"
     GEN_AI_SYSTEM_BEDROCK = "bedrock"
     GEN_AI_SYSTEM_VERTEXAI = "vertexai"
     GEN_AI_SYSTEM_GROQ = "groq"
+    GEN_AI_SYSTEM_OLLAMA = "ollama"
     GEN_AI_SYSTEM_LANGCHAIN = "langchain"
     GEN_AI_SYSTEM_LLAMAINDEX = "llama_index"
     GEN_AI_SYSTEM_HAYSTACK = "haystack"
 
     # Vector DB
     DB_REQUESTS = "db.total.requests"
     DB_SYSTEM = "db.system"
```

### Comparing `openlit-1.5.0/PKG-INFO` & `openlit-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlit
-Version: 1.5.0
+Version: 1.6.0
 Summary: OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects
 Home-page: https://github.com/openlit/openlit/tree/main/openlit/python
 Keywords: OpenTelemetry,otel,otlp,llm,tracing,openai,anthropic,claude,cohere,llm monitoring,observability,monitoring,gpt,Generative AI,chatGPT
 Author: OpenLIT
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -46,14 +46,15 @@
 
 This project adheres to the [Semantic Conventions](https://github.com/open-telemetry/semantic-conventions/tree/main/docs/gen-ai) proposed by the OpenTelemetry community. You can check out the current definitions [here](src/openlit/semcov/__init__.py).
 
 ## What can be Auto Instrumented?
 
 ### LLMs
 - [✅ OpenAI](https://docs.openlit.io/latest/integrations/openai)
+- [✅ Ollama](https://docs.openlit.io/latest/integrations/ollama)
 - [✅ Anthropic](https://docs.openlit.io/latest/integrations/anthropic)
 - [✅ Cohere](https://docs.openlit.io/latest/integrations/cohere)
 - [✅ Mistral](https://docs.openlit.io/latest/integrations/mistral)
 - [✅ Azure OpenAI](https://docs.openlit.io/latest/integrations/azure-openai)
 - [✅ HuggingFace Transformers](https://docs.openlit.io/latest/integrations/huggingface)
 - [✅ Amazon Bedrock](https://docs.openlit.io/latest/integrations/bedrock)
 - [✅ Vertex AI](https://docs.openlit.io/latest/integrations/vertexai)
```

