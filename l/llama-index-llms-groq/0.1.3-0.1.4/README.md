# Comparing `tmp/llama_index_llms_groq-0.1.3.tar.gz` & `tmp/llama_index_llms_groq-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_groq-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_llms_groq-0.1.4.tar", max compression
```

## Comparing `llama_index_llms_groq-0.1.3.tar` & `llama_index_llms_groq-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1623 2024-02-23 20:11:45.418073 llama_index_llms_groq-0.1.3/README.md
--rw-r--r--   0        0        0       64 2024-02-23 20:11:45.418254 llama_index_llms_groq-0.1.3/llama_index/llms/groq/__init__.py
--rw-r--r--   0        0        0      697 2024-02-23 20:11:45.418307 llama_index_llms_groq-0.1.3/llama_index/llms/groq/base.py
--rw-r--r--   0        0        0     1449 2024-02-23 20:11:57.587854 llama_index_llms_groq-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 llama_index_llms_groq-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1623 2024-05-17 20:30:04.222396 llama_index_llms_groq-0.1.4/README.md
+-rw-r--r--   0        0        0       64 2024-05-17 20:30:04.222396 llama_index_llms_groq-0.1.4/llama_index/llms/groq/__init__.py
+-rw-r--r--   0        0        0     1265 2024-05-17 20:30:04.222396 llama_index_llms_groq-0.1.4/llama_index/llms/groq/base.py
+-rw-r--r--   0        0        0     1449 2024-05-17 20:30:04.222396 llama_index_llms_groq-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2227 1970-01-01 00:00:00.000000 llama_index_llms_groq-0.1.4/PKG-INFO
```

### Comparing `llama_index_llms_groq-0.1.3/README.md` & `llama_index_llms_groq-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_llms_groq-0.1.3/pyproject.toml` & `llama_index_llms_groq-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms groq integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-groq"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 llama-index-llms-openai-like = "^0.1.3"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_llms_groq-0.1.3/PKG-INFO` & `llama_index_llms_groq-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-groq
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index llms groq integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Requires-Dist: llama-index-llms-openai-like (>=0.1.3,<0.2.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Groq
 
 Welcome to Groq! 🚀 At Groq, we've developed the world's first Language Processing Unit™, or LPU. The Groq LPU has a deterministic, single core streaming architecture that sets the standard for GenAI inference speed with predictable and repeatable performance for any given workload.
```

