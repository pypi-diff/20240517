# Comparing `tmp/llama_index_readers_s3-0.1.7.tar.gz` & `tmp/llama_index_readers_s3-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_s3-0.1.7.tar", max compression
+gzip compressed data, was "llama_index_readers_s3-0.1.8.tar", max compression
```

## Comparing `llama_index_readers_s3-0.1.7.tar` & `llama_index_readers_s3-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1552 2024-03-28 20:25:46.514060 llama_index_readers_s3-0.1.7/README.md
--rw-r--r--   0        0        0       73 2024-03-13 22:17:44.756075 llama_index_readers_s3-0.1.7/llama_index/readers/s3/__init__.py
--rw-r--r--   0        0        0     4421 2024-04-12 19:45:28.956786 llama_index_readers_s3-0.1.7/llama_index/readers/s3/base.py
--rw-r--r--   0        0        0     1646 2024-04-12 19:50:39.070945 llama_index_readers_s3-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2319 1970-01-01 00:00:00.000000 llama_index_readers_s3-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1433 2024-05-09 15:57:03.700786 llama_index_readers_s3-0.1.8/README.md
+-rw-r--r--   0        0        0       73 2024-03-13 22:17:44.756075 llama_index_readers_s3-0.1.8/llama_index/readers/s3/__init__.py
+-rw-r--r--   0        0        0     6642 2024-05-17 17:33:12.047252 llama_index_readers_s3-0.1.8/llama_index/readers/s3/base.py
+-rw-r--r--   0        0        0     1654 2024-05-17 17:33:12.047497 llama_index_readers_s3-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 llama_index_readers_s3-0.1.8/PKG-INFO
```

### Comparing `llama_index_readers_s3-0.1.7/pyproject.toml` & `llama_index_readers_s3-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 description = "llama-index readers s3 integration"
 exclude = ["**/BUILD"]
 keywords = ["amazon web services", "aws s3", "bucket"]
 license = "MIT"
 maintainers = ["thejessezhang"]
 name = "llama-index-readers-s3"
 readme = "README.md"
-version = "0.1.7"
+version = "0.1.8"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.1"
+llama-index-core = "^0.10.37.post1"
 llama-index-readers-file = "^0.1.12"
-s3fs = "^2024.3.1"
+s3fs = ">=2024.3.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_readers_s3-0.1.7/PKG-INFO` & `llama_index_readers_s3-0.1.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-s3
-Version: 0.1.7
+Version: 0.1.8
 Summary: llama-index readers s3 integration
 License: MIT
 Keywords: amazon web services,aws s3,bucket
 Author: Your Name
 Author-email: you@example.com
 Maintainer: thejessezhang
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.37.post1,<0.11.0)
 Requires-Dist: llama-index-readers-file (>=0.1.12,<0.2.0)
-Requires-Dist: s3fs (>=2024.3.1,<2025.0.0)
+Requires-Dist: s3fs (>=2024.3.1)
 Description-Content-Type: text/markdown
 
 # S3 File or Directory Loader
 
 This loader parses any file stored on S3, or the entire Bucket (with an optional prefix filter) if no particular file is specified. When initializing `S3Reader`, you may pass in your [AWS Access Key](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_access-keys.html). If none are found, the loader assumes they are stored in `~/.aws/credentials`.
 
 All files are parsed with `SimpleDirectoryReader`. Hence, you may also specify a custom `file_extractor`, relying on any of the loaders in this library (or your own)!
@@ -43,9 +43,9 @@
     key="dictionary.txt",
     aws_access_id="[ACCESS_KEY_ID]",
     aws_access_secret="[ACCESS_KEY_SECRET]",
 )
 documents = loader.load_data()
 ```
 
-This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/run-llama/llama_index/tree/main/llama_index) and/or subsequently used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent.
+This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/run-llama/llama_index/).
```

