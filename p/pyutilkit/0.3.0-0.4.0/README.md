# Comparing `tmp/pyutilkit-0.3.0.tar.gz` & `tmp/pyutilkit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutilkit-0.3.0.tar", max compression
+gzip compressed data, was "pyutilkit-0.4.0.tar", max compression
```

## Comparing `pyutilkit-0.3.0.tar` & `pyutilkit-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     7696 2024-05-12 17:26:27.967790 pyutilkit-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     1836 2024-05-13 21:39:43.972463 pyutilkit-0.3.0/docs/README.md
--rw-r--r--   0        0        0     2994 2024-05-14 09:13:56.737771 pyutilkit-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-14 09:14:05.144163 pyutilkit-0.3.0/src/pyutilkit/__init__.py
--rw-r--r--   0        0        0      462 2024-05-12 17:26:28.511050 pyutilkit-0.3.0/src/pyutilkit/classes.py
--rw-r--r--   0        0        0        0 2024-05-12 17:26:28.644365 pyutilkit-0.3.0/src/pyutilkit/data/__init__.py
--rw-r--r--   0        0        0     3866 2024-05-12 17:26:28.644365 pyutilkit-0.3.0/src/pyutilkit/data/timezones.py
--rw-r--r--   0        0        0     1820 2024-05-13 21:39:32.392717 pyutilkit-0.3.0/src/pyutilkit/date_utils.py
--rw-r--r--   0        0        0     1523 2024-05-13 16:50:53.492051 pyutilkit-0.3.0/src/pyutilkit/files.py
--rw-r--r--   0        0        0        0 2024-05-12 17:26:27.967790 pyutilkit-0.3.0/src/pyutilkit/py.typed
--rw-r--r--   0        0        0     2895 2024-05-13 16:50:11.949600 pyutilkit-0.3.0/src/pyutilkit/term.py
--rw-r--r--   0        0        0     1838 2024-05-13 21:39:48.282369 pyutilkit-0.3.0/src/pyutilkit/timing.py
--rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 pyutilkit-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     7696 2024-05-12 17:26:27.967790 pyutilkit-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     1836 2024-05-13 21:39:43.972463 pyutilkit-0.4.0/docs/README.md
+-rw-r--r--   0        0        0     2994 2024-05-17 15:53:29.530466 pyutilkit-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-14 09:14:05.144163 pyutilkit-0.4.0/src/pyutilkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-17 15:52:55.734648 pyutilkit-0.4.0/src/pyutilkit/cache.py
+-rw-r--r--   0        0        0      462 2024-05-12 17:26:28.511050 pyutilkit-0.4.0/src/pyutilkit/classes.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:26:28.644365 pyutilkit-0.4.0/src/pyutilkit/data/__init__.py
+-rw-r--r--   0        0        0     3866 2024-05-12 17:26:28.644365 pyutilkit-0.4.0/src/pyutilkit/data/timezones.py
+-rw-r--r--   0        0        0     1820 2024-05-13 21:39:32.392717 pyutilkit-0.4.0/src/pyutilkit/date_utils.py
+-rw-r--r--   0        0        0     1523 2024-05-13 16:50:53.492051 pyutilkit-0.4.0/src/pyutilkit/files.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:26:27.967790 pyutilkit-0.4.0/src/pyutilkit/py.typed
+-rw-r--r--   0        0        0     2895 2024-05-17 15:10:47.374309 pyutilkit-0.4.0/src/pyutilkit/term.py
+-rw-r--r--   0        0        0     3741 2024-05-17 15:52:24.278781 pyutilkit-0.4.0/src/pyutilkit/timing.py
+-rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 pyutilkit-0.4.0/PKG-INFO
```

### Comparing `pyutilkit-0.3.0/LICENSE.md` & `pyutilkit-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyutilkit-0.3.0/docs/README.md` & `pyutilkit-0.4.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `pyutilkit-0.3.0/pyproject.toml` & `pyutilkit-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "pyutilkit"
-version = "0.3.0"
+version = "0.4.0"
 description = "python's missing batteries"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "docs/README.md"
```

### Comparing `pyutilkit-0.3.0/src/pyutilkit/data/timezones.py` & `pyutilkit-0.4.0/src/pyutilkit/data/timezones.py`

 * *Files identical despite different names*

### Comparing `pyutilkit-0.3.0/src/pyutilkit/date_utils.py` & `pyutilkit-0.4.0/src/pyutilkit/date_utils.py`

 * *Files identical despite different names*

### Comparing `pyutilkit-0.3.0/src/pyutilkit/files.py` & `pyutilkit-0.4.0/src/pyutilkit/files.py`

 * *Files identical despite different names*

### Comparing `pyutilkit-0.3.0/src/pyutilkit/term.py` & `pyutilkit-0.4.0/src/pyutilkit/term.py`

 * *Files identical despite different names*

### Comparing `pyutilkit-0.3.0/PKG-INFO` & `pyutilkit-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutilkit
-Version: 0.3.0
+Version: 0.4.0
 Summary: python's missing batteries
 Home-page: https://pyutilkit.readthedocs.io/en/stable/
 License: LGPL-3.0+
 Keywords: utils
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.9,<4.0
```

