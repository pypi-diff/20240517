# Comparing `tmp/ucam_observe-0.1.2.tar.gz` & `tmp/ucam_observe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucam_observe-0.1.2.tar", max compression
+gzip compressed data, was "ucam_observe-0.1.3.tar", max compression
```

## Comparing `ucam_observe-0.1.2.tar` & `ucam_observe-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     2718 2024-05-15 16:08:39.433980 ucam_observe-0.1.2/README.md
--rw-r--r--   0        0        0     1927 2024-05-15 15:58:01.609349 ucam_observe-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      205 2024-05-15 15:58:01.609349 ucam_observe-0.1.2/ucam_observe/__init__.py
--rw-r--r--   0        0        0      243 2024-05-15 15:58:01.609349 ucam_observe-0.1.2/ucam_observe/django.py
--rw-r--r--   0        0        0     2064 2024-05-15 15:58:01.609349 ucam_observe-0.1.2/ucam_observe/logging_config.py
--rw-r--r--   0        0        0     3475 1970-01-01 00:00:00.000000 ucam_observe-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2807 2024-05-16 20:02:51.065395 ucam_observe-0.1.3/README.md
+-rw-r--r--   0        0        0     1927 2024-05-17 11:50:13.943281 ucam_observe-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-05-16 22:08:59.297363 ucam_observe-0.1.3/ucam_observe/__init__.py
+-rw-r--r--   0        0        0      243 2024-05-15 15:58:29.915328 ucam_observe-0.1.3/ucam_observe/django.py
+-rw-r--r--   0        0        0     1295 2024-05-17 12:37:12.018224 ucam_observe-0.1.3/ucam_observe/gunicorn.py
+-rw-r--r--   0        0        0     4840 2024-05-17 12:33:00.939288 ucam_observe-0.1.3/ucam_observe/logging_config.py
+-rw-r--r--   0        0        0     3564 1970-01-01 00:00:00.000000 ucam_observe-0.1.3/PKG-INFO
```

### Comparing `ucam_observe-0.1.2/README.md` & `ucam_observe-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -35,18 +35,22 @@
 
 ## Include Gunicorn structlog configuration in your project
 
 ### Adapt Gunicorn configuration
 In the root of your project, create/amend a gunicorn.conf.py. Add the following code to the file.
 
 ```py
-from ucam_observe.gunicorn_conf import configure_logging
-configure_logging()
+from ucam_observe.gunicorn import (  # noqa F401 used by gunicorn as magic variable
+    logconfig_dict,
+    loglevel,
+)
 ```
 
+**Be sure not to set loglevel via the CLI.**
+
 ### Environment Configuration
 
 #### Log Level
 
 Set the `LOG_LEVEL` environment variable to control the logging level (e.g., DEBUG, INFO, WARNING, ERROR, CRITICAL). This setting adjusts the verbosity of the log outputs:
 
 ```bash
```

### Comparing `ucam_observe-0.1.2/pyproject.toml` & `ucam_observe-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ucam_observe"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python library to aid consistent configuration of logging, metrics (future) and tracing (further in future). Packaging and wiring existing open tooling to work effortlessly on UIS DevOps managed cloud infrastructure."
 license = "MIT"
 readme = "README.md"
 authors = []
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `ucam_observe-0.1.2/PKG-INFO` & `ucam_observe-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucam_observe
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python library to aid consistent configuration of logging, metrics (future) and tracing (further in future). Packaging and wiring existing open tooling to work effortlessly on UIS DevOps managed cloud infrastructure.
 License: MIT
 Requires-Python: >=3.9.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -51,18 +51,22 @@
 
 ## Include Gunicorn structlog configuration in your project
 
 ### Adapt Gunicorn configuration
 In the root of your project, create/amend a gunicorn.conf.py. Add the following code to the file.
 
 ```py
-from ucam_observe.gunicorn_conf import configure_logging
-configure_logging()
+from ucam_observe.gunicorn import (  # noqa F401 used by gunicorn as magic variable
+    logconfig_dict,
+    loglevel,
+)
 ```
 
+**Be sure not to set loglevel via the CLI.**
+
 ### Environment Configuration
 
 #### Log Level
 
 Set the `LOG_LEVEL` environment variable to control the logging level (e.g., DEBUG, INFO, WARNING, ERROR, CRITICAL). This setting adjusts the verbosity of the log outputs:
 
 ```bash
```

