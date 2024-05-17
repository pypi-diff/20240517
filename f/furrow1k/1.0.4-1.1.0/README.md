# Comparing `tmp/furrow1k-1.0.4.tar.gz` & `tmp/furrow1k-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furrow1k-1.0.4.tar", max compression
+gzip compressed data, was "furrow1k-1.1.0.tar", max compression
```

## Comparing `furrow1k-1.0.4.tar` & `furrow1k-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rwxr-xr-x   0        0        0     1068 2024-05-05 22:35:02.889442 furrow1k-1.0.4/LICENSE
--rw-r--r--   0        0        0      657 2024-05-05 22:35:02.901477 furrow1k-1.0.4/README.md
--rw-r--r--   0        0        0      475 2024-05-13 03:46:43.172408 furrow1k-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      110 2024-05-05 22:35:02.934491 furrow1k-1.0.4/src/furrow1k/__init__.py
--rw-r--r--   0        0        0     6818 2024-05-13 02:44:45.928917 furrow1k-1.0.4/src/furrow1k/furrow1k.py
--rw-r--r--   0        0        0     1061 1970-01-01 00:00:00.000000 furrow1k-1.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1068 2024-05-05 22:35:02.889442 furrow1k-1.1.0/LICENSE
+-rw-r--r--   0        0        0      657 2024-05-05 22:35:02.901477 furrow1k-1.1.0/README.md
+-rw-r--r--   0        0        0      475 2024-05-17 03:43:06.212480 furrow1k-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-05-05 22:35:02.934491 furrow1k-1.1.0/src/furrow1k/__init__.py
+-rw-r--r--   0        0        0     4225 2024-05-17 03:42:22.081155 furrow1k-1.1.0/src/furrow1k/furrow1k.py
+-rw-r--r--   0        0        0     4299 2024-05-17 03:28:57.770268 furrow1k-1.1.0/src/furrow1k/questionaire.py
+-rw-r--r--   0        0        0     1061 1970-01-01 00:00:00.000000 furrow1k-1.1.0/PKG-INFO
```

### Comparing `furrow1k-1.0.4/LICENSE` & `furrow1k-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `furrow1k-1.0.4/README.md` & `furrow1k-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `furrow1k-1.0.4/PKG-INFO` & `furrow1k-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furrow1k
-Version: 1.0.4
+Version: 1.1.0
 Summary: Help calculate percentage of salary to contribute to 401k
 License: MIT
 Author: Frank Cao
 Requires-Python: >=3.12.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
```

