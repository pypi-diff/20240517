# Comparing `tmp/ucam_faas-0.4.1.tar.gz` & `tmp/ucam_faas-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucam_faas-0.4.1.tar", max compression
+gzip compressed data, was "ucam_faas-0.6.0.tar", max compression
```

## Comparing `ucam_faas-0.4.1.tar` & `ucam_faas-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3834 2024-04-22 13:48:02.497353 ucam_faas-0.4.1/README.md
--rw-r--r--   0        0        0     3131 2024-05-15 15:44:32.120793 ucam_faas-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     7220 2024-05-14 20:50:10.382759 ucam_faas-0.4.1/ucam_faas/__init__.py
--rw-r--r--   0        0        0      106 2024-05-13 15:59:51.022836 ucam_faas-0.4.1/ucam_faas/exceptions.py
--rw-r--r--   0        0        0      581 2024-05-14 20:50:10.382759 ucam_faas-0.4.1/ucam_faas/testing.py
--rw-r--r--   0        0        0        0 2024-05-15 18:04:14.574051 ucam_faas-0.4.1/ucam_faas/tests/__init__.py
--rw-r--r--   0        0        0     2557 2024-05-15 12:27:32.119929 ucam_faas-0.4.1/ucam_faas/tests/test_ucam_faas.py
--rw-r--r--   0        0        0     5230 1970-01-01 00:00:00.000000 ucam_faas-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     3834 2024-04-22 13:48:17.943519 ucam_faas-0.6.0/README.md
+-rw-r--r--   0        0        0     3131 2024-05-17 09:51:24.289336 ucam_faas-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7220 2024-05-17 09:40:34.340852 ucam_faas-0.6.0/ucam_faas/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-13 16:04:34.383948 ucam_faas-0.6.0/ucam_faas/exceptions.py
+-rw-r--r--   0        0        0      581 2024-05-14 20:49:42.585515 ucam_faas-0.6.0/ucam_faas/testing.py
+-rw-r--r--   0        0        0        0 2024-05-17 10:36:33.665400 ucam_faas-0.6.0/ucam_faas/tests/__init__.py
+-rw-r--r--   0        0        0     2557 2024-05-15 12:27:31.175522 ucam_faas-0.6.0/ucam_faas/tests/test_ucam_faas.py
+-rw-r--r--   0        0        0     5230 1970-01-01 00:00:00.000000 ucam_faas-0.6.0/PKG-INFO
```

### Comparing `ucam_faas-0.4.1/README.md` & `ucam_faas-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ucam_faas-0.4.1/pyproject.toml` & `ucam_faas-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ucam-faas"
-version = "0.4.1"
+version = "0.6.0"
 description = "Opinionated FaaS support framework extending Google's functions-framework"
 authors = ["University of Cambridge Information Services <devops-wilson@uis.cam.ac.uk>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://gitlab.developers.cam.ac.uk/uis/devops/ucam-faas-python/ucam-faas"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ucam_faas-0.4.1/ucam_faas/__init__.py` & `ucam_faas-0.6.0/ucam_faas/__init__.py`

 * *Files identical despite different names*

### Comparing `ucam_faas-0.4.1/ucam_faas/testing.py` & `ucam_faas-0.6.0/ucam_faas/testing.py`

 * *Files identical despite different names*

### Comparing `ucam_faas-0.4.1/ucam_faas/tests/test_ucam_faas.py` & `ucam_faas-0.6.0/ucam_faas/tests/test_ucam_faas.py`

 * *Files identical despite different names*

### Comparing `ucam_faas-0.4.1/PKG-INFO` & `ucam_faas-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucam-faas
-Version: 0.4.1
+Version: 0.6.0
 Summary: Opinionated FaaS support framework extending Google's functions-framework
 Home-page: https://gitlab.developers.cam.ac.uk/uis/devops/ucam-faas-python/ucam-faas
 License: MIT
 Author: University of Cambridge Information Services
 Author-email: devops-wilson@uis.cam.ac.uk
 Requires-Python: >=3.9.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

