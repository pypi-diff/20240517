# Comparing `tmp/fitz_utils-0.0.16.tar.gz` & `tmp/fitz_utils-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitz_utils-0.0.16.tar", max compression
+gzip compressed data, was "fitz_utils-0.0.17.tar", max compression
```

## Comparing `fitz_utils-0.0.16.tar` & `fitz_utils-0.0.17.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      131 2023-10-20 08:58:59.230911 fitz_utils-0.0.16/fitz_utils/__init__.py
--rw-r--r--   0        0        0     1252 2024-01-06 10:09:09.461046 fitz_utils-0.0.16/fitz_utils/processed_doc.py
--rw-r--r--   0        0        0    15172 2024-01-04 07:21:58.507463 fitz_utils-0.0.16/fitz_utils/processed_page.py
--rw-r--r--   0        0        0       30 2023-05-18 02:30:19.428100 fitz_utils-0.0.16/LICENSE
--rw-r--r--   0        0        0      511 2024-01-06 10:10:27.681969 fitz_utils-0.0.16/pyproject.toml
--rw-r--r--   0        0        0      364 2023-10-18 07:47:38.225952 fitz_utils-0.0.16/README.md
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 fitz_utils-0.0.16/PKG-INFO
+-rw-r--r--   0        0        0      131 2024-05-17 02:55:06.955851 fitz_utils-0.0.17/fitz_utils/__init__.py
+-rw-r--r--   0        0        0     1252 2024-05-17 02:55:06.955851 fitz_utils-0.0.17/fitz_utils/processed_doc.py
+-rw-r--r--   0        0        0    15172 2024-05-17 02:55:06.955851 fitz_utils-0.0.17/fitz_utils/processed_page.py
+-rw-r--r--   0        0        0       30 2024-05-17 02:55:06.955851 fitz_utils-0.0.17/LICENSE
+-rw-r--r--   0        0        0      511 2024-05-17 02:56:20.336367 fitz_utils-0.0.17/pyproject.toml
+-rw-r--r--   0        0        0      364 2024-05-17 02:55:06.955851 fitz_utils-0.0.17/README.md
+-rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 fitz_utils-0.0.17/PKG-INFO
```

### Comparing `fitz_utils-0.0.16/fitz_utils/processed_doc.py` & `fitz_utils-0.0.17/fitz_utils/processed_doc.py`

 * *Files identical despite different names*

### Comparing `fitz_utils-0.0.16/fitz_utils/processed_page.py` & `fitz_utils-0.0.17/fitz_utils/processed_page.py`

 * *Files identical despite different names*

### Comparing `fitz_utils-0.0.16/PKG-INFO` & `fitz_utils-0.0.17/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: fitz-utils
-Version: 0.0.16
+Version: 0.0.17
 Summary: Extra functions for use with pymupdf module
 Author: The Walnut AI
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ftfy (>=6.1.1,<7.0.0)
 Requires-Dist: numpy (>=1.26.1,<2.0.0)
 Requires-Dist: pandas (>=2.1.1,<3.0.0)
 Requires-Dist: pymupdf (>=1.20.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 ## Introduction
```

