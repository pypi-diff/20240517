# Comparing `tmp/iudex-0.5.0.tar.gz` & `tmp/iudex-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iudex-0.5.0.tar", max compression
+gzip compressed data, was "iudex-0.5.1.tar", max compression
```

## Comparing `iudex-0.5.0.tar` & `iudex-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-02-26 21:03:01.210390 iudex-0.5.0/LICENSE
--rw-r--r--   0        0        0     1502 2024-05-17 01:14:03.519309 iudex-0.5.0/README.md
--rw-r--r--   0        0        0        0 2024-05-17 01:39:19.649489 iudex-0.5.0/iudex/__init__.py
--rw-r--r--   0        0        0     1502 2024-05-14 23:55:03.479188 iudex-0.5.0/iudex/instrumentation/README.md
--rw-r--r--   0        0        0      106 2024-05-17 01:17:53.127532 iudex-0.5.0/iudex/instrumentation/__init__.py
--rw-r--r--   0        0        0     2821 2024-05-10 20:15:13.224407 iudex-0.5.0/iudex/instrumentation/attributes.py
--rw-r--r--   0        0        0     1974 2024-05-14 23:55:03.479780 iudex-0.5.0/iudex/instrumentation/fastapi.py
--rw-r--r--   0        0        0     6043 2024-05-17 01:33:17.021670 iudex-0.5.0/iudex/instrumentation/instrumentation.py
--rw-r--r--   0        0        0     1517 2024-05-17 01:41:47.528945 iudex-0.5.0/iudex/instrumentation/lambda.py
--rw-r--r--   0        0        0      610 2024-05-17 01:42:21.010860 iudex-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 iudex-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-26 21:03:01.210390 iudex-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1502 2024-05-17 01:14:03.519309 iudex-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 01:39:19.649489 iudex-0.5.1/iudex/__init__.py
+-rw-r--r--   0        0        0     1502 2024-05-14 23:55:03.479188 iudex-0.5.1/iudex/instrumentation/README.md
+-rw-r--r--   0        0        0      106 2024-05-17 01:17:53.127532 iudex-0.5.1/iudex/instrumentation/__init__.py
+-rw-r--r--   0        0        0     2821 2024-05-10 20:15:13.224407 iudex-0.5.1/iudex/instrumentation/attributes.py
+-rw-r--r--   0        0        0     1974 2024-05-14 23:55:03.479780 iudex-0.5.1/iudex/instrumentation/fastapi.py
+-rw-r--r--   0        0        0     6043 2024-05-17 01:33:17.021670 iudex-0.5.1/iudex/instrumentation/instrumentation.py
+-rw-r--r--   0        0        0     1517 2024-05-17 01:41:47.528945 iudex-0.5.1/iudex/instrumentation/lambda.py
+-rw-r--r--   0        0        0      610 2024-05-17 02:08:35.829382 iudex-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 iudex-0.5.1/PKG-INFO
```

### Comparing `iudex-0.5.0/LICENSE` & `iudex-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iudex-0.5.0/README.md` & `iudex-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.5.0/iudex/instrumentation/README.md` & `iudex-0.5.1/iudex/instrumentation/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.5.0/iudex/instrumentation/attributes.py` & `iudex-0.5.1/iudex/instrumentation/attributes.py`

 * *Files identical despite different names*

### Comparing `iudex-0.5.0/iudex/instrumentation/fastapi.py` & `iudex-0.5.1/iudex/instrumentation/fastapi.py`

 * *Files identical despite different names*

### Comparing `iudex-0.5.0/iudex/instrumentation/instrumentation.py` & `iudex-0.5.1/iudex/instrumentation/instrumentation.py`

 * *Files identical despite different names*

### Comparing `iudex-0.5.0/iudex/instrumentation/lambda.py` & `iudex-0.5.1/iudex/instrumentation/lambda.py`

 * *Files identical despite different names*

### Comparing `iudex-0.5.0/pyproject.toml` & `iudex-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "iudex"
-version = "0.5.0"
+version = "0.5.1"
 description = ""
 authors = ["Drake Wong <drake@iudex.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 opentelemetry-distro = "^0.45b0"
 opentelemetry-instrumentation-fastapi = "^0.45b0"
-opentelemetry-exporter-otlp-proto-http = "^1.24.0"
+opentelemetry-exporter-otlp-proto-http = "^1.20.0"
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.2.0"
 fastapi = "^0.111.0"
```

### Comparing `iudex-0.5.0/PKG-INFO` & `iudex-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: iudex
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 Author: Drake Wong
 Author-email: drake@iudex.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: opentelemetry-distro (>=0.45b0,<0.46)
-Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1.24.0,<2.0.0)
+Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1.20.0,<2.0.0)
 Requires-Dist: opentelemetry-instrumentation-fastapi (>=0.45b0,<0.46)
 Description-Content-Type: text/markdown
 
 Instrumenting your Python service to send logs to Iudex just takes a few steps.
 
 # FastAPI
```

