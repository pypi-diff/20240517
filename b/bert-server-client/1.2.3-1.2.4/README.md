# Comparing `tmp/bert_server_client-1.2.3.tar.gz` & `tmp/bert_server_client-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert_server_client-1.2.3.tar", last modified: Tue May 14 13:56:40 2024, max compression
+gzip compressed data, was "bert_server_client-1.2.4.tar", last modified: Fri May 17 07:36:18 2024, max compression
```

## Comparing `bert_server_client-1.2.3.tar` & `bert_server_client-1.2.4.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:56:40.414595 bert_server_client-1.2.3/
--rw-r--r--   0 root         (0) root         (0)      320 2024-05-14 13:56:40.414595 bert_server_client-1.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6220 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:56:40.411595 bert_server_client-1.2.3/bert_server_client/
--rw-rw-rw-   0 root         (0) root         (0)       31 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5034 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:56:40.413595 bert_server_client-1.2.3/bert_server_client/schema/
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4291 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/schema/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1520 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/schema/embedding.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/schema/health_check.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/schema/zmq_message_header.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:56:40.414595 bert_server_client-1.2.3/bert_server_client/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2863 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/tests/client_integration_tests.py
--rw-rw-rw-   0 root         (0) root         (0)     2086 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4221 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/tests/test_client.py
--rw-rw-rw-   0 root         (0) root         (0)     3035 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/tests/test_msgpack.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/bert_server_client/tests/test_zmq_message_header.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:56:40.412595 bert_server_client-1.2.3/bert_server_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      320 2024-05-14 13:56:40.000000 bert_server_client-1.2.3/bert_server_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2024-05-14 13:56:40.000000 bert_server_client-1.2.3/bert_server_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 13:56:40.000000 bert_server_client-1.2.3/bert_server_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2024-05-14 13:56:40.000000 bert_server_client-1.2.3/bert_server_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-14 13:56:40.000000 bert_server_client-1.2.3/bert_server_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      754 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 13:56:40.414595 bert_server_client-1.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      740 2024-05-14 13:56:38.000000 bert_server_client-1.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 07:36:18.183812 bert_server_client-1.2.4/
+-rw-r--r--   0 root         (0) root         (0)      320 2024-05-17 07:36:18.182812 bert_server_client-1.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6220 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 07:36:18.179812 bert_server_client-1.2.4/bert_server_client/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/bert_server_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5034 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/bert_server_client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/bert_server_client/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 07:36:18.181812 bert_server_client-1.2.4/bert_server_client/schema/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/bert_server_client/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4291 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/bert_server_client/schema/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      301 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/bert_server_client/schema/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/bert_server_client/schema/embedding.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/bert_server_client/schema/health_check.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/bert_server_client/schema/split.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/bert_server_client/schema/zmq_message_header.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 07:36:18.182812 bert_server_client-1.2.4/bert_server_client/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/bert_server_client/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2863 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/bert_server_client/tests/client_integration_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     2086 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/bert_server_client/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4221 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/bert_server_client/tests/test_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3035 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/bert_server_client/tests/test_msgpack.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/bert_server_client/tests/test_zmq_message_header.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 07:36:18.180812 bert_server_client-1.2.4/bert_server_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      320 2024-05-17 07:36:18.000000 bert_server_client-1.2.4/bert_server_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      865 2024-05-17 07:36:18.000000 bert_server_client-1.2.4/bert_server_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 07:36:18.000000 bert_server_client-1.2.4/bert_server_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-05-17 07:36:18.000000 bert_server_client-1.2.4/bert_server_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-17 07:36:18.000000 bert_server_client-1.2.4/bert_server_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      754 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 07:36:18.183812 bert_server_client-1.2.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      740 2024-05-17 07:36:15.000000 bert_server_client-1.2.4/setup.py
```

### Comparing `bert_server_client-1.2.3/README.md` & `bert_server_client-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.2.3/bert_server_client/client.py` & `bert_server_client-1.2.4/bert_server_client/client.py`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.2.3/bert_server_client/error.py` & `bert_server_client-1.2.4/bert_server_client/error.py`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.2.3/bert_server_client/schema/base.py` & `bert_server_client-1.2.4/bert_server_client/schema/base.py`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.2.3/bert_server_client/schema/embedding.py` & `bert_server_client-1.2.4/bert_server_client/schema/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Union, List, Optional, Dict, Any
 from dataclasses import dataclass, field
 from uuid import UUID
 
 from bert_server_client.schema.base import Base
+from bert_server_client.schema.split import Split
 
 
 @dataclass
 class Embedding:
     object: str
     index: int
     embedding: List[float]
@@ -25,15 +26,15 @@
     model: Optional[str] = field(default=None)
     usage: Optional[EmbeddingUsage] = field(default=None)
 
 
 @dataclass
 class EmbeddingQueryResponse(Base):
     object: str
-    data: List[str]
+    data: List[Split]
     model: Optional[str] = field(default=None)
     usage: Optional[EmbeddingUsage] = field(default=None)
 
 
 @dataclass
 class EmbeddingRequest(Base):
     input: Union[str, List[str]]
```

### Comparing `bert_server_client-1.2.3/bert_server_client/schema/zmq_message_header.py` & `bert_server_client-1.2.4/bert_server_client/schema/zmq_message_header.py`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.2.3/bert_server_client/tests/client_integration_tests.py` & `bert_server_client-1.2.4/bert_server_client/tests/client_integration_tests.py`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.2.3/bert_server_client/tests/test_base.py` & `bert_server_client-1.2.4/bert_server_client/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.2.3/bert_server_client/tests/test_client.py` & `bert_server_client-1.2.4/bert_server_client/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.2.3/bert_server_client/tests/test_msgpack.py` & `bert_server_client-1.2.4/bert_server_client/tests/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.2.3/bert_server_client/tests/test_zmq_message_header.py` & `bert_server_client-1.2.4/bert_server_client/tests/test_zmq_message_header.py`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.2.3/bert_server_client.egg-info/SOURCES.txt` & `bert_server_client-1.2.4/bert_server_client.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 bert_server_client.egg-info/PKG-INFO
 bert_server_client.egg-info/SOURCES.txt
 bert_server_client.egg-info/dependency_links.txt
 bert_server_client.egg-info/requires.txt
 bert_server_client.egg-info/top_level.txt
 bert_server_client/schema/__init__.py
 bert_server_client/schema/base.py
+bert_server_client/schema/document.py
 bert_server_client/schema/embedding.py
 bert_server_client/schema/health_check.py
+bert_server_client/schema/split.py
 bert_server_client/schema/zmq_message_header.py
 bert_server_client/tests/__init__.py
 bert_server_client/tests/client_integration_tests.py
 bert_server_client/tests/test_base.py
 bert_server_client/tests/test_client.py
 bert_server_client/tests/test_msgpack.py
 bert_server_client/tests/test_zmq_message_header.py
```

### Comparing `bert_server_client-1.2.3/pyproject.toml` & `bert_server_client-1.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bert_server_client-1.2.3/setup.py` & `bert_server_client-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bert_server_client",
-    version="1.2.3",
+    version="1.2.4",
     packages=find_packages(),
     package_data={'bert_server_client': ['schema/*']},
     author="Anil Aydiner",
     author_email="a.aydiner@qimia.de",
     description="A ZMQ client interface for Bert server",
     long_description="A ZMQ client interface for Bert server",
     url="https://gitlab.com/qimiaio/qimia-ai-dev/bert-server-client",
```

