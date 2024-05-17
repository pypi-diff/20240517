# Comparing `tmp/iudex-0.5.2.tar.gz` & `tmp/iudex-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iudex-0.5.2.tar", max compression
+gzip compressed data, was "iudex-0.5.4.tar", max compression
```

## Comparing `iudex-0.5.2.tar` & `iudex-0.5.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-02-26 21:03:01.210390 iudex-0.5.2/LICENSE
--rw-r--r--   0        0        0     1502 2024-05-17 01:14:03.519309 iudex-0.5.2/README.md
--rw-r--r--   0        0        0        0 2024-05-17 01:39:19.649489 iudex-0.5.2/iudex/__init__.py
--rw-r--r--   0        0        0     1502 2024-05-14 23:55:03.479188 iudex-0.5.2/iudex/instrumentation/README.md
--rw-r--r--   0        0        0      106 2024-05-17 01:17:53.127532 iudex-0.5.2/iudex/instrumentation/__init__.py
--rw-r--r--   0        0        0     2821 2024-05-10 20:15:13.224407 iudex-0.5.2/iudex/instrumentation/attributes.py
--rw-r--r--   0        0        0     1974 2024-05-14 23:55:03.479780 iudex-0.5.2/iudex/instrumentation/fastapi.py
--rw-r--r--   0        0        0     6043 2024-05-17 01:33:17.021670 iudex-0.5.2/iudex/instrumentation/instrumentation.py
--rw-r--r--   0        0        0     1517 2024-05-17 01:41:47.528945 iudex-0.5.2/iudex/instrumentation/lambda.py
--rw-r--r--   0        0        0      595 2024-05-17 02:24:14.308169 iudex-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 iudex-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-26 21:03:01.210390 iudex-0.5.4/LICENSE
+-rw-r--r--   0        0        0     1502 2024-05-17 01:14:03.519309 iudex-0.5.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 01:39:19.649489 iudex-0.5.4/iudex/__init__.py
+-rw-r--r--   0        0        0     1502 2024-05-14 23:55:03.479188 iudex-0.5.4/iudex/instrumentation/README.md
+-rw-r--r--   0        0        0      106 2024-05-17 01:17:53.127532 iudex-0.5.4/iudex/instrumentation/__init__.py
+-rw-r--r--   0        0        0     2821 2024-05-10 20:15:13.224407 iudex-0.5.4/iudex/instrumentation/attributes.py
+-rw-r--r--   0        0        0     1974 2024-05-14 23:55:03.479780 iudex-0.5.4/iudex/instrumentation/fastapi.py
+-rw-r--r--   0        0        0     6043 2024-05-17 01:33:17.021670 iudex-0.5.4/iudex/instrumentation/instrumentation.py
+-rw-r--r--   0        0        0     1517 2024-05-17 01:41:47.528945 iudex-0.5.4/iudex/instrumentation/lambda.py
+-rw-r--r--   0        0        0      605 2024-05-17 03:14:13.401787 iudex-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 iudex-0.5.4/PKG-INFO
```

### Comparing `iudex-0.5.2/LICENSE` & `iudex-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iudex-0.5.2/README.md` & `iudex-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.5.2/iudex/instrumentation/README.md` & `iudex-0.5.4/iudex/instrumentation/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.5.2/iudex/instrumentation/attributes.py` & `iudex-0.5.4/iudex/instrumentation/attributes.py`

 * *Files identical despite different names*

### Comparing `iudex-0.5.2/iudex/instrumentation/fastapi.py` & `iudex-0.5.4/iudex/instrumentation/fastapi.py`

 * *Files identical despite different names*

### Comparing `iudex-0.5.2/iudex/instrumentation/instrumentation.py` & `iudex-0.5.4/iudex/instrumentation/instrumentation.py`

 * *Files identical despite different names*

### Comparing `iudex-0.5.2/iudex/instrumentation/lambda.py` & `iudex-0.5.4/iudex/instrumentation/lambda.py`

 * *Files identical despite different names*

### Comparing `iudex-0.5.2/pyproject.toml` & `iudex-0.5.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "iudex"
-version = "0.5.2"
+version = "0.5.4"
 description = ""
 authors = ["Drake Wong <drake@iudex.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-opentelemetry-distro = "~0"
-opentelemetry-instrumentation-fastapi = "~0"
-opentelemetry-exporter-otlp-proto-http = "~1"
+opentelemetry-exporter-otlp-proto-http = "1.20.0"
+opentelemetry-instrumentation-fastapi = "0.41b0"
+opentelemetry-distro = "0.41b0"
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.1"
+fastapi = "<0.111"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.2.0"
-fastapi = "^0.111.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [virtualenvs]
 in-project = true
```

### Comparing `iudex-0.5.2/PKG-INFO` & `iudex-0.5.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: iudex
-Version: 0.5.2
+Version: 0.5.4
 Summary: 
 Author: Drake Wong
 Author-email: drake@iudex.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: opentelemetry-distro (>=0,<1)
-Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1,<2)
-Requires-Dist: opentelemetry-instrumentation-fastapi (>=0,<1)
+Requires-Dist: opentelemetry-distro (==0.41b0)
+Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.20.0)
+Requires-Dist: opentelemetry-instrumentation-fastapi (==0.41b0)
 Description-Content-Type: text/markdown
 
 Instrumenting your Python service to send logs to Iudex just takes a few steps.
 
 # FastAPI
 
 1. Pip install dependencies
```

