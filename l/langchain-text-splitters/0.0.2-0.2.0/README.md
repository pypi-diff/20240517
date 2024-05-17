# Comparing `tmp/langchain_text_splitters-0.0.2.tar.gz` & `tmp/langchain_text_splitters-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_text_splitters-0.0.2.tar", max compression
+gzip compressed data, was "langchain_text_splitters-0.2.0.tar", max compression
```

## Comparing `langchain_text_splitters-0.0.2.tar` & `langchain_text_splitters-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1400 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/README.md
--rw-r--r--   0        0        0     2070 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/langchain_text_splitters/__init__.py
--rw-r--r--   0        0        0    11337 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/langchain_text_splitters/base.py
--rw-r--r--   0        0        0    20580 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/langchain_text_splitters/character.py
--rw-r--r--   0        0        0    11558 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/langchain_text_splitters/html.py
--rw-r--r--   0        0        0     4416 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/langchain_text_splitters/json.py
--rw-r--r--   0        0        0      985 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/langchain_text_splitters/konlpy.py
--rw-r--r--   0        0        0      546 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/langchain_text_splitters/latex.py
--rw-r--r--   0        0        0     9172 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/langchain_text_splitters/markdown.py
--rw-r--r--   0        0        0     1042 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/langchain_text_splitters/nltk.py
--rw-r--r--   0        0        0        0 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/langchain_text_splitters/py.typed
--rw-r--r--   0        0        0      539 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/langchain_text_splitters/python.py
--rw-r--r--   0        0        0     2872 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/langchain_text_splitters/sentence_transformers.py
--rw-r--r--   0        0        0     1762 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/langchain_text_splitters/spacy.py
--rw-r--r--   0        0        0     1073 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/langchain_text_splitters/xsl/converting_to_header.xslt
--rw-r--r--   0        0        0     6033 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/langchain_text_splitters/xsl/html_chunks_with_headers.xslt
--rw-r--r--   0        0        0     2727 2024-05-16 03:13:55.132128 langchain_text_splitters-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 langchain_text_splitters-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1400 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/README.md
+-rw-r--r--   0        0        0     2070 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/langchain_text_splitters/__init__.py
+-rw-r--r--   0        0        0    11337 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/langchain_text_splitters/base.py
+-rw-r--r--   0        0        0    20580 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/langchain_text_splitters/character.py
+-rw-r--r--   0        0        0    11558 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/langchain_text_splitters/html.py
+-rw-r--r--   0        0        0     4416 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/langchain_text_splitters/json.py
+-rw-r--r--   0        0        0      985 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/langchain_text_splitters/konlpy.py
+-rw-r--r--   0        0        0      546 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/langchain_text_splitters/latex.py
+-rw-r--r--   0        0        0     9172 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/langchain_text_splitters/markdown.py
+-rw-r--r--   0        0        0     1042 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/langchain_text_splitters/nltk.py
+-rw-r--r--   0        0        0        0 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/langchain_text_splitters/py.typed
+-rw-r--r--   0        0        0      539 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/langchain_text_splitters/python.py
+-rw-r--r--   0        0        0     2872 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/langchain_text_splitters/sentence_transformers.py
+-rw-r--r--   0        0        0     1762 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/langchain_text_splitters/spacy.py
+-rw-r--r--   0        0        0     1073 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/langchain_text_splitters/xsl/converting_to_header.xslt
+-rw-r--r--   0        0        0     6033 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/langchain_text_splitters/xsl/html_chunks_with_headers.xslt
+-rw-r--r--   0        0        0     2720 2024-05-17 20:33:23.903140 langchain_text_splitters-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2242 1970-01-01 00:00:00.000000 langchain_text_splitters-0.2.0/PKG-INFO
```

### Comparing `langchain_text_splitters-0.0.2/README.md` & `langchain_text_splitters-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `langchain_text_splitters-0.0.2/langchain_text_splitters/__init__.py` & `langchain_text_splitters-0.2.0/langchain_text_splitters/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_text_splitters-0.0.2/langchain_text_splitters/base.py` & `langchain_text_splitters-0.2.0/langchain_text_splitters/base.py`

 * *Files identical despite different names*

### Comparing `langchain_text_splitters-0.0.2/langchain_text_splitters/character.py` & `langchain_text_splitters-0.2.0/langchain_text_splitters/character.py`

 * *Files identical despite different names*

### Comparing `langchain_text_splitters-0.0.2/langchain_text_splitters/html.py` & `langchain_text_splitters-0.2.0/langchain_text_splitters/html.py`

 * *Files identical despite different names*

### Comparing `langchain_text_splitters-0.0.2/langchain_text_splitters/json.py` & `langchain_text_splitters-0.2.0/langchain_text_splitters/json.py`

 * *Files identical despite different names*

### Comparing `langchain_text_splitters-0.0.2/langchain_text_splitters/konlpy.py` & `langchain_text_splitters-0.2.0/langchain_text_splitters/konlpy.py`

 * *Files identical despite different names*

### Comparing `langchain_text_splitters-0.0.2/langchain_text_splitters/latex.py` & `langchain_text_splitters-0.2.0/langchain_text_splitters/latex.py`

 * *Files identical despite different names*

### Comparing `langchain_text_splitters-0.0.2/langchain_text_splitters/markdown.py` & `langchain_text_splitters-0.2.0/langchain_text_splitters/markdown.py`

 * *Files identical despite different names*

### Comparing `langchain_text_splitters-0.0.2/langchain_text_splitters/nltk.py` & `langchain_text_splitters-0.2.0/langchain_text_splitters/nltk.py`

 * *Files identical despite different names*

### Comparing `langchain_text_splitters-0.0.2/langchain_text_splitters/python.py` & `langchain_text_splitters-0.2.0/langchain_text_splitters/python.py`

 * *Files identical despite different names*

### Comparing `langchain_text_splitters-0.0.2/langchain_text_splitters/sentence_transformers.py` & `langchain_text_splitters-0.2.0/langchain_text_splitters/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langchain_text_splitters-0.0.2/langchain_text_splitters/spacy.py` & `langchain_text_splitters-0.2.0/langchain_text_splitters/spacy.py`

 * *Files identical despite different names*

### Comparing `langchain_text_splitters-0.0.2/langchain_text_splitters/xsl/converting_to_header.xslt` & `langchain_text_splitters-0.2.0/langchain_text_splitters/xsl/converting_to_header.xslt`

 * *Files identical despite different names*

### Comparing `langchain_text_splitters-0.0.2/langchain_text_splitters/xsl/html_chunks_with_headers.xslt` & `langchain_text_splitters-0.2.0/langchain_text_splitters/xsl/html_chunks_with_headers.xslt`

 * *Files identical despite different names*

### Comparing `langchain_text_splitters-0.0.2/pyproject.toml` & `langchain_text_splitters-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "langchain-text-splitters"
-version = "0.0.2"
+version = "0.2.0"
 description = "LangChain text splitting utilities"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = ">=0.1.28,<0.3"
+langchain-core = "^0.2.0"
 lxml = {version = ">=4.9.3,<6.0", optional = true}
 beautifulsoup4 = {version = "^4.12.3", optional = true}
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
```

### Comparing `langchain_text_splitters-0.0.2/PKG-INFO` & `langchain_text_splitters-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-text-splitters
-Version: 0.0.2
+Version: 0.2.0
 Summary: LangChain text splitting utilities
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: extended-testing
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0) ; extra == "extended-testing"
-Requires-Dist: langchain-core (>=0.1.28,<0.3)
+Requires-Dist: langchain-core (>=0.2.0,<0.3.0)
 Requires-Dist: lxml (>=4.9.3,<6.0) ; extra == "extended-testing"
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Description-Content-Type: text/markdown
 
 # 🦜✂️ LangChain Text Splitters
 
 [![Downloads](https://static.pepy.tech/badge/langchain_text_splitters/month)](https://pepy.tech/project/langchain_text_splitters)
```

