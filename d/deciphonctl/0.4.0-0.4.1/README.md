# Comparing `tmp/deciphonctl-0.4.0.tar.gz` & `tmp/deciphonctl-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphonctl-0.4.0.tar", max compression
+gzip compressed data, was "deciphonctl-0.4.1.tar", max compression
```

## Comparing `deciphonctl-0.4.0.tar` & `deciphonctl-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1063 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/LICENSE
--rw-r--r--   0        0        0       15 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/__init__.py
--rw-r--r--   0        0        0       28 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/__main__.py
--rw-r--r--   0        0        0     6028 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/cli.py
--rw-r--r--   0        0        0      755 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/consumer.py
--rw-r--r--   0        0        0      677 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/download.py
--rw-r--r--   0        0        0     1088 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/files.py
--rw-r--r--   0        0        0     2386 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/models.py
--rw-r--r--   0        0        0      107 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/permissions.py
--rw-r--r--   0        0        0     3479 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/presser.py
--rw-r--r--   0        0        0     1242 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/progress.py
--rw-r--r--   0        0        0      423 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/progress_informer.py
--rw-r--r--   0        0        0      871 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/progress_logger.py
--rw-r--r--   0        0        0     3230 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/scanner.py
--rw-r--r--   0        0        0     5858 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/sched.py
--rw-r--r--   0        0        0      435 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/settings.py
--rw-r--r--   0        0        0      387 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/signals.py
--rw-r--r--   0        0        0      305 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/url.py
--rw-r--r--   0        0        0     1055 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/deciphonctl/worker.py
--rw-r--r--   0        0        0      818 2023-11-30 11:24:08.234888 deciphonctl-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 deciphonctl-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/LICENSE
+-rw-r--r--   0        0        0       15 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/__main__.py
+-rw-r--r--   0        0        0     6028 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/cli.py
+-rw-r--r--   0        0        0      755 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/consumer.py
+-rw-r--r--   0        0        0      677 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/download.py
+-rw-r--r--   0        0        0     1088 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/files.py
+-rw-r--r--   0        0        0     2386 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/models.py
+-rw-r--r--   0        0        0      107 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/permissions.py
+-rw-r--r--   0        0        0     3479 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/presser.py
+-rw-r--r--   0        0        0     1242 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/progress.py
+-rw-r--r--   0        0        0      423 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/progress_informer.py
+-rw-r--r--   0        0        0      871 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/progress_logger.py
+-rw-r--r--   0        0        0     3230 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/scanner.py
+-rw-r--r--   0        0        0     5858 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/sched.py
+-rw-r--r--   0        0        0      435 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/settings.py
+-rw-r--r--   0        0        0      387 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/signals.py
+-rw-r--r--   0        0        0      305 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/url.py
+-rw-r--r--   0        0        0     1055 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/deciphonctl/worker.py
+-rw-r--r--   0        0        0      792 2024-05-16 23:56:07.142718 deciphonctl-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 deciphonctl-0.4.1/PKG-INFO
```

### Comparing `deciphonctl-0.4.0/LICENSE` & `deciphonctl-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.0/deciphonctl/cli.py` & `deciphonctl-0.4.1/deciphonctl/cli.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.0/deciphonctl/consumer.py` & `deciphonctl-0.4.1/deciphonctl/consumer.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.0/deciphonctl/download.py` & `deciphonctl-0.4.1/deciphonctl/download.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.0/deciphonctl/files.py` & `deciphonctl-0.4.1/deciphonctl/files.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.0/deciphonctl/models.py` & `deciphonctl-0.4.1/deciphonctl/models.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.0/deciphonctl/presser.py` & `deciphonctl-0.4.1/deciphonctl/presser.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.0/deciphonctl/progress.py` & `deciphonctl-0.4.1/deciphonctl/progress.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.0/deciphonctl/progress_logger.py` & `deciphonctl-0.4.1/deciphonctl/progress_logger.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.0/deciphonctl/scanner.py` & `deciphonctl-0.4.1/deciphonctl/scanner.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.0/deciphonctl/sched.py` & `deciphonctl-0.4.1/deciphonctl/sched.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.0/deciphonctl/worker.py` & `deciphonctl-0.4.1/deciphonctl/worker.py`

 * *Files identical despite different names*

### Comparing `deciphonctl-0.4.0/pyproject.toml` & `deciphonctl-0.4.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [tool.poetry]
 name = "deciphonctl"
-version = "0.4.0"
+version = "0.4.1"
 description = "Control Deciphon server."
 authors = ["Danilo Horta <horta@ebi.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "deciphonctl" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-typer = "^0"
-requests = "^2"
-pydantic = "^2"
-pydantic-settings = "^2"
-fasta-reader = "^3"
-deciphon = ">=0.11.0"
-deciphon-core = ">=0.19.0"
-loguru = "^0"
-deciphon-sched = ">=0.11.2"
-paho-mqtt = "^1.6.1"
-requests-toolbelt = "^1.0.0"
+typer = "^0.12"
+requests = "^2.31"
+pydantic = "^2.7"
+pydantic-settings = "^2.2"
+fasta-reader = "^3.0"
+deciphon = "^0.13"
+deciphon-core = "^0.23"
+loguru = "^0.7"
+requests-toolbelt = "^1.0"
+paho-mqtt = "^2.1"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.3.2"
-uvicorn = "^0"
-deciphon-sched = { version = ">=0.11.2", extras = ["testing"] }
+deciphon-sched = { version = "^0.11", extras = ["testing"] }
+pytest = "^8.2"
+uvicorn = "^0.29"
 
 [tool.pytest.ini_options]
 pythonpath = ["."]
 
 [tool.poetry.scripts]
 deciphonctl = 'deciphonctl.cli:app'
```

### Comparing `deciphonctl-0.4.0/PKG-INFO` & `deciphonctl-0.4.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: deciphonctl
-Version: 0.4.0
+Version: 0.4.1
 Summary: Control Deciphon server.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: deciphon (>=0.11.0)
-Requires-Dist: deciphon-core (>=0.19.0)
-Requires-Dist: deciphon-sched (>=0.11.2)
-Requires-Dist: fasta-reader (>=3,<4)
-Requires-Dist: loguru (>=0,<1)
-Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
-Requires-Dist: pydantic (>=2,<3)
-Requires-Dist: pydantic-settings (>=2,<3)
-Requires-Dist: requests (>=2,<3)
-Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
-Requires-Dist: typer (>=0,<1)
+Requires-Dist: deciphon (>=0.13,<0.14)
+Requires-Dist: deciphon-core (>=0.23,<0.24)
+Requires-Dist: fasta-reader (>=3.0,<4.0)
+Requires-Dist: loguru (>=0.7,<0.8)
+Requires-Dist: paho-mqtt (>=2.1,<3.0)
+Requires-Dist: pydantic (>=2.7,<3.0)
+Requires-Dist: pydantic-settings (>=2.2,<3.0)
+Requires-Dist: requests (>=2.31,<3.0)
+Requires-Dist: requests-toolbelt (>=1.0,<2.0)
+Requires-Dist: typer (>=0.12,<0.13)
 Description-Content-Type: text/markdown
 
 # deciphon-ctl
```

