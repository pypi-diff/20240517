# Comparing `tmp/socketwrench-1.8.9.tar.gz` & `tmp/socketwrench-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketwrench-1.8.9.tar", last modified: Thu May 16 19:53:36 2024, max compression
+gzip compressed data, was "socketwrench-1.9.0.tar", last modified: Thu May 16 21:03:37 2024, max compression
```

## Comparing `socketwrench-1.8.9.tar` & `socketwrench-1.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:53:36.706524 socketwrench-1.8.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-16 19:53:32.000000 socketwrench-1.8.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 19:53:32.000000 socketwrench-1.8.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 19:53:36.702524 socketwrench-1.8.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-16 19:53:32.000000 socketwrench-1.8.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-16 19:53:32.000000 socketwrench-1.8.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:53:36.706524 socketwrench-1.8.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:53:36.698524 socketwrench-1.8.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:53:36.702524 socketwrench-1.8.9/src/socketwrench/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 19:53:32.000000 socketwrench-1.8.9/src/socketwrench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 19:53:32.000000 socketwrench-1.8.9/src/socketwrench/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-16 19:53:32.000000 socketwrench-1.8.9/src/socketwrench/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    26774 2024-05-16 19:53:32.000000 socketwrench-1.8.9/src/socketwrench/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-16 19:53:32.000000 socketwrench-1.8.9/src/socketwrench/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:53:36.702524 socketwrench-1.8.9/src/socketwrench/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-16 19:53:32.000000 socketwrench-1.8.9/src/socketwrench/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:53:36.702524 socketwrench-1.8.9/src/socketwrench/resources/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-16 19:53:32.000000 socketwrench-1.8.9/src/socketwrench/resources/playground/panels.js
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 19:53:32.000000 socketwrench-1.8.9/src/socketwrench/resources/playground/playground.html
--rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-16 19:53:32.000000 socketwrench-1.8.9/src/socketwrench/resources/playground/playground.js
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-16 19:53:32.000000 socketwrench-1.8.9/src/socketwrench/resources/swagger.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:53:36.702524 socketwrench-1.8.9/src/socketwrench/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:53:32.000000 socketwrench-1.8.9/src/socketwrench/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-16 19:53:32.000000 socketwrench-1.8.9/src/socketwrench/samples/file_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-16 19:53:32.000000 socketwrench-1.8.9/src/socketwrench/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-16 19:53:32.000000 socketwrench-1.8.9/src/socketwrench/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 19:53:32.000000 socketwrench-1.8.9/src/socketwrench/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    30708 2024-05-16 19:53:32.000000 socketwrench-1.8.9/src/socketwrench/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:53:36.702524 socketwrench-1.8.9/src/socketwrench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 19:53:36.000000 socketwrench-1.8.9/src/socketwrench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 19:53:36.000000 socketwrench-1.8.9/src/socketwrench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:53:36.000000 socketwrench-1.8.9/src/socketwrench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 19:53:36.000000 socketwrench-1.8.9/src/socketwrench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:03:37.203793 socketwrench-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-16 21:03:32.000000 socketwrench-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 21:03:32.000000 socketwrench-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 21:03:37.203793 socketwrench-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-16 21:03:32.000000 socketwrench-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-16 21:03:32.000000 socketwrench-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 21:03:37.203793 socketwrench-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:03:37.199793 socketwrench-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:03:37.203793 socketwrench-1.9.0/src/socketwrench/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 21:03:32.000000 socketwrench-1.9.0/src/socketwrench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 21:03:32.000000 socketwrench-1.9.0/src/socketwrench/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-16 21:03:32.000000 socketwrench-1.9.0/src/socketwrench/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26918 2024-05-16 21:03:32.000000 socketwrench-1.9.0/src/socketwrench/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-16 21:03:32.000000 socketwrench-1.9.0/src/socketwrench/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:03:37.203793 socketwrench-1.9.0/src/socketwrench/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-16 21:03:32.000000 socketwrench-1.9.0/src/socketwrench/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:03:37.203793 socketwrench-1.9.0/src/socketwrench/resources/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-16 21:03:32.000000 socketwrench-1.9.0/src/socketwrench/resources/playground/panels.js
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 21:03:32.000000 socketwrench-1.9.0/src/socketwrench/resources/playground/playground.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-16 21:03:32.000000 socketwrench-1.9.0/src/socketwrench/resources/playground/playground.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-16 21:03:32.000000 socketwrench-1.9.0/src/socketwrench/resources/swagger.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:03:37.203793 socketwrench-1.9.0/src/socketwrench/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:03:32.000000 socketwrench-1.9.0/src/socketwrench/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-16 21:03:32.000000 socketwrench-1.9.0/src/socketwrench/samples/file_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-16 21:03:32.000000 socketwrench-1.9.0/src/socketwrench/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-16 21:03:32.000000 socketwrench-1.9.0/src/socketwrench/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 21:03:32.000000 socketwrench-1.9.0/src/socketwrench/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30708 2024-05-16 21:03:32.000000 socketwrench-1.9.0/src/socketwrench/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:03:37.203793 socketwrench-1.9.0/src/socketwrench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 21:03:37.000000 socketwrench-1.9.0/src/socketwrench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 21:03:37.000000 socketwrench-1.9.0/src/socketwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:03:37.000000 socketwrench-1.9.0/src/socketwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 21:03:37.000000 socketwrench-1.9.0/src/socketwrench.egg-info/top_level.txt
```

### Comparing `socketwrench-1.8.9/LICENSE` & `socketwrench-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.9/PKG-INFO` & `socketwrench-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.9
+Version: 1.9.0
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.8.9/README.md` & `socketwrench-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.9/pyproject.toml` & `socketwrench-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketwrench"
-version = "1.8.9"
+version = "1.9.0"
 description = "A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger."
 readme = "README.md"
 authors = [{ name = "Torin Halsted", email = "modularizer@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
```

### Comparing `socketwrench-1.8.9/src/socketwrench/__init__.py` & `socketwrench-1.9.0/src/socketwrench/__init__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.9/src/socketwrench/__main__.py` & `socketwrench-1.9.0/src/socketwrench/__main__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.9/src/socketwrench/connection.py` & `socketwrench-1.9.0/src/socketwrench/connection.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.9/src/socketwrench/handlers.py` & `socketwrench-1.9.0/src/socketwrench/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,16 @@
         if value.isdigit() or (value.startswith("-") and value[1:].isdigit()):
             return float(value)
     if _typehint_matches(typehint, [bool, inspect._empty]):
         if value.lower() in ["false", "f", "no", "n"]:
             return False
         if value.lower() in ["true", "t", "yes", "y"]:
             return True
+    if value.lower() in ["none", "null"] and _typehint_matches(typehint, [None]) or not _typehint_matches(typehint, [str]):
+        return None
     if _typehint_matches(typehint, [bool]):
         if value.lower() in ["0"]:
             return False
         if value.lower() in ["1", "ok"]:
             return True
     if _typehint_matches(typehint, [list, inspect._empty]):
         if value.startswith("[") and value.endswith("]"):
```

### Comparing `socketwrench-1.8.9/src/socketwrench/openapi.py` & `socketwrench-1.9.0/src/socketwrench/openapi.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.9/src/socketwrench/resources/favicon.ico` & `socketwrench-1.9.0/src/socketwrench/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.9/src/socketwrench/resources/playground/panels.js` & `socketwrench-1.9.0/src/socketwrench/resources/playground/panels.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.9/src/socketwrench/resources/playground/playground.html` & `socketwrench-1.9.0/src/socketwrench/resources/playground/playground.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.9/src/socketwrench/resources/playground/playground.js` & `socketwrench-1.9.0/src/socketwrench/resources/playground/playground.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.9/src/socketwrench/resources/swagger.html` & `socketwrench-1.9.0/src/socketwrench/resources/swagger.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.9/src/socketwrench/samples/file_sample.py` & `socketwrench-1.9.0/src/socketwrench/samples/file_sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.9/src/socketwrench/samples/sample.py` & `socketwrench-1.9.0/src/socketwrench/samples/sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.9/src/socketwrench/server.py` & `socketwrench-1.9.0/src/socketwrench/server.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.9/src/socketwrench/tags.py` & `socketwrench-1.9.0/src/socketwrench/tags.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.9/src/socketwrench/types.py` & `socketwrench-1.9.0/src/socketwrench/types.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.9/src/socketwrench.egg-info/PKG-INFO` & `socketwrench-1.9.0/src/socketwrench.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.9
+Version: 1.9.0
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.8.9/src/socketwrench.egg-info/SOURCES.txt` & `socketwrench-1.9.0/src/socketwrench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

