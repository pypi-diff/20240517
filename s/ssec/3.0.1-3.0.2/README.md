# Comparing `tmp/ssec-3.0.1.tar.gz` & `tmp/ssec-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssec-3.0.1.tar", last modified: Thu May 16 10:43:18 2024, max compression
+gzip compressed data, was "ssec-3.0.2.tar", last modified: Thu May 16 10:56:57 2024, max compression
```

## Comparing `ssec-3.0.1.tar` & `ssec-3.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:43:18.230273 ssec-3.0.1/
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     1063 2024-05-06 10:30:34.000000 ssec-3.0.1/LICENSE
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     7168 2024-05-16 10:43:18.220273 ssec-3.0.1/PKG-INFO
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     5929 2024-05-15 12:02:38.000000 ssec-3.0.1/README.md
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     3731 2024-05-16 10:42:39.000000 ssec-3.0.1/pyproject.toml
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)       38 2024-05-16 10:43:18.230273 ssec-3.0.1/setup.cfg
-drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:43:18.220273 ssec-3.0.1/src/
-drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:43:18.220273 ssec-3.0.1/src/ssec/
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      117 2024-05-15 12:02:38.000000 ssec-3.0.1/src/ssec/__init__.py
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     5416 2024-05-16 10:39:02.000000 ssec-3.0.1/src/ssec/common.py
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     1187 2024-05-16 09:37:29.000000 ssec-3.0.1/src/ssec/constants.py
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      384 2024-05-16 09:40:43.000000 ssec-3.0.1/src/ssec/event.py
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)       57 2024-05-15 12:02:38.000000 ssec-3.0.1/src/ssec/py.typed
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     7822 2024-05-16 10:41:21.000000 ssec-3.0.1/src/ssec/stream.py
-drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:43:18.220273 ssec-3.0.1/src/ssec.egg-info/
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     7168 2024-05-16 10:43:18.000000 ssec-3.0.1/src/ssec.egg-info/PKG-INFO
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      308 2024-05-16 10:43:18.000000 ssec-3.0.1/src/ssec.egg-info/SOURCES.txt
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)        1 2024-05-16 10:43:18.000000 ssec-3.0.1/src/ssec.egg-info/dependency_links.txt
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      112 2024-05-16 10:43:18.000000 ssec-3.0.1/src/ssec.egg-info/requires.txt
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)        5 2024-05-16 10:43:18.000000 ssec-3.0.1/src/ssec.egg-info/top_level.txt
+drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:56:57.299827 ssec-3.0.2/
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     1063 2024-05-06 10:30:34.000000 ssec-3.0.2/LICENSE
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     7168 2024-05-16 10:56:57.299827 ssec-3.0.2/PKG-INFO
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     5929 2024-05-15 12:02:38.000000 ssec-3.0.2/README.md
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     3731 2024-05-16 10:56:30.000000 ssec-3.0.2/pyproject.toml
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)       38 2024-05-16 10:56:57.299827 ssec-3.0.2/setup.cfg
+drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:56:57.299827 ssec-3.0.2/src/
+drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:56:57.299827 ssec-3.0.2/src/ssec/
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      117 2024-05-15 12:02:38.000000 ssec-3.0.2/src/ssec/__init__.py
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     5503 2024-05-16 10:55:38.000000 ssec-3.0.2/src/ssec/common.py
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     1187 2024-05-16 09:37:29.000000 ssec-3.0.2/src/ssec/constants.py
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      384 2024-05-16 09:40:43.000000 ssec-3.0.2/src/ssec/event.py
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)       57 2024-05-15 12:02:38.000000 ssec-3.0.2/src/ssec/py.typed
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     7822 2024-05-16 10:41:21.000000 ssec-3.0.2/src/ssec/stream.py
+drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:56:57.299827 ssec-3.0.2/src/ssec.egg-info/
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     7168 2024-05-16 10:56:57.000000 ssec-3.0.2/src/ssec.egg-info/PKG-INFO
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      308 2024-05-16 10:56:57.000000 ssec-3.0.2/src/ssec.egg-info/SOURCES.txt
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)        1 2024-05-16 10:56:57.000000 ssec-3.0.2/src/ssec.egg-info/dependency_links.txt
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      112 2024-05-16 10:56:57.000000 ssec-3.0.2/src/ssec.egg-info/requires.txt
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)        5 2024-05-16 10:56:57.000000 ssec-3.0.2/src/ssec.egg-info/top_level.txt
```

### Comparing `ssec-3.0.1/LICENSE` & `ssec-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ssec-3.0.1/PKG-INFO` & `ssec-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssec
-Version: 3.0.1
+Version: 3.0.2
 Summary: Synchronous and asynchronous library for server-sent events.
 Author-email: "J. Baudisch" <justin.baudisch@hsbi.de>
 Maintainer-email: "J. Baudisch" <justin.baudisch@hsbi.de>
 Project-URL: Repository, https://github.com/sharly-project/ssec
 Keywords: Network,Synchronous,Asynchronous,Server-sent events
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `ssec-3.0.1/README.md` & `ssec-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ssec-3.0.1/pyproject.toml` & `ssec-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools"]
 
 [project]
 name = "ssec"
-version = "3.0.1"
+version = "3.0.2"
 description = "Synchronous and asynchronous library for server-sent events."
 readme = "README.md"
 requires-python = ">=3.12"
 authors = [
   { name = "J. Baudisch", email = "justin.baudisch@hsbi.de" },
 ]
 maintainers = [{ name = "J. Baudisch", email = "justin.baudisch@hsbi.de" }]
```

### Comparing `ssec-3.0.1/src/ssec/common.py` & `ssec-3.0.2/src/ssec/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,19 @@
 
             yield Event(
                 event_type,
                 event_data,
                 origin=config.origin,
                 last_event_id=config.last_event_id,
             )
+
+            # Reset buffers.
+            event_type = ""
+            event_data = ""
+
             continue
 
         # If the line starts with a U+003A COLON character (:) -> Ignore the line.
         if line.startswith(DELIMITER):
             continue
 
         name, _, value = line.partition(DELIMITER)
```

### Comparing `ssec-3.0.1/src/ssec/constants.py` & `ssec-3.0.2/src/ssec/constants.py`

 * *Files identical despite different names*

### Comparing `ssec-3.0.1/src/ssec/stream.py` & `ssec-3.0.2/src/ssec/stream.py`

 * *Files identical despite different names*

### Comparing `ssec-3.0.1/src/ssec.egg-info/PKG-INFO` & `ssec-3.0.2/src/ssec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssec
-Version: 3.0.1
+Version: 3.0.2
 Summary: Synchronous and asynchronous library for server-sent events.
 Author-email: "J. Baudisch" <justin.baudisch@hsbi.de>
 Maintainer-email: "J. Baudisch" <justin.baudisch@hsbi.de>
 Project-URL: Repository, https://github.com/sharly-project/ssec
 Keywords: Network,Synchronous,Asynchronous,Server-sent events
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

