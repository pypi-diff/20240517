# Comparing `tmp/langchain_objectbox-0.1.0a3.tar.gz` & `tmp/langchain_objectbox-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_objectbox-0.1.0a3.tar", max compression
+gzip compressed data, was "langchain_objectbox-0.1.0a4.tar", max compression
```

## Comparing `langchain_objectbox-0.1.0a3.tar` & `langchain_objectbox-0.1.0a4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2024-04-29 16:27:47.475174 langchain_objectbox-0.1.0a3/LICENSE
--rw-r--r--   0        0        0     3874 2024-04-30 14:20:29.497964 langchain_objectbox-0.1.0a3/README.md
--rw-r--r--   0        0        0       86 2024-04-29 16:12:03.665330 langchain_objectbox-0.1.0a3/langchain_objectbox/__init__.py
--rw-r--r--   0        0        0     9651 2024-05-10 14:23:01.506171 langchain_objectbox-0.1.0a3/langchain_objectbox/vectorstores.py
--rw-r--r--   0        0        0      662 2024-05-10 14:42:54.949748 langchain_objectbox-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0     4539 1970-01-01 00:00:00.000000 langchain_objectbox-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-14 14:12:32.626479 langchain_objectbox-0.1.0a4/LICENSE
+-rw-r--r--   0        0        0     3874 2024-05-14 14:12:32.638479 langchain_objectbox-0.1.0a4/README.md
+-rw-r--r--   0        0        0       86 2024-05-14 14:12:32.606479 langchain_objectbox-0.1.0a4/langchain_objectbox/__init__.py
+-rw-r--r--   0        0        0     9651 2024-05-14 14:12:32.674479 langchain_objectbox-0.1.0a4/langchain_objectbox/vectorstores.py
+-rw-r--r--   0        0        0      662 2024-05-17 07:07:36.083644 langchain_objectbox-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0     4545 1970-01-01 00:00:00.000000 langchain_objectbox-0.1.0a4/PKG-INFO
```

### Comparing `langchain_objectbox-0.1.0a3/LICENSE` & `langchain_objectbox-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_objectbox-0.1.0a3/README.md` & `langchain_objectbox-0.1.0a4/README.md`

 * *Files identical despite different names*

### Comparing `langchain_objectbox-0.1.0a3/langchain_objectbox/vectorstores.py` & `langchain_objectbox-0.1.0a4/langchain_objectbox/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langchain_objectbox-0.1.0a3/pyproject.toml` & `langchain_objectbox-0.1.0a4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-objectbox"
-version = "0.1.0a3"
+version = "0.1.0a4"
 description = "Integration package connecting ObjectBox and LangChain"
 authors = ["ObjectBox" ]
 license = "MIT" 
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License"
 ]
 [tool.poetry.dependencies]
 python = "^3.8.1" 
 langchain-core = "^0.1.45"
-objectbox = "0.7.0a10"
+objectbox = "^4.0.0a0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 langchain = "^0.1.16"
 numpy = [ 
     { version = "^1.26", python = "^3.12" },
```

### Comparing `langchain_objectbox-0.1.0a3/PKG-INFO` & `langchain_objectbox-0.1.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-objectbox
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: Integration package connecting ObjectBox and LangChain
 License: MIT
 Author: ObjectBox
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: langchain-core (>=0.1.45,<0.2.0)
-Requires-Dist: objectbox (==0.7.0a10)
+Requires-Dist: objectbox (>=4.0.0a0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # langchain-objectbox
 
 ## About
 
 This package contains the [ObjectBox](https://objectbox.io) integrations for [LangChain](https://www.langchain.com).
```

