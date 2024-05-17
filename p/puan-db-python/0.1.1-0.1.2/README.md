# Comparing `tmp/puan_db_python-0.1.1.tar.gz` & `tmp/puan_db_python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puan_db_python-0.1.1.tar", max compression
+gzip compressed data, was "puan_db_python-0.1.2.tar", max compression
```

## Comparing `puan_db_python-0.1.1.tar` & `puan_db_python-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,7 @@
--rw-r--r--   0        0        0     2131 2024-04-26 14:13:18.316480 puan_db_python-0.1.1/README.md
--rw-r--r--   0        0        0    12558 2024-05-07 11:50:27.331963 puan_db_python-0.1.1/puan_db_python/__init__.py
--rw-r--r--   0        0        0      313 2024-05-07 11:50:47.022961 puan_db_python-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 puan_db_python-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2131 2024-04-26 14:13:18.316480 puan_db_python-0.1.2/README.md
+-rw-r--r--   0        0        0     9110 2024-05-07 11:50:12.903621 puan_db_python-0.1.2/puan_db_pb2.py
+-rw-r--r--   0        0        0    10307 2024-05-07 11:50:12.903754 puan_db_python-0.1.2/puan_db_pb2.pyi
+-rw-r--r--   0        0        0    37826 2024-05-07 11:59:09.129985 puan_db_python-0.1.2/puan_db_pb2_grpc.py
+-rw-r--r--   0        0        0    12558 2024-05-07 12:00:51.767857 puan_db_python-0.1.2/puan_db_python/__init__.py
+-rw-r--r--   0        0        0      408 2024-05-07 12:01:51.233816 puan_db_python-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 puan_db_python-0.1.2/PKG-INFO
```

### Comparing `puan_db_python-0.1.1/README.md` & `puan_db_python-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `puan_db_python-0.1.1/puan_db_python/__init__.py` & `puan_db_python-0.1.2/puan_db_python/__init__.py`

 * *Files identical despite different names*

### Comparing `puan_db_python-0.1.1/PKG-INFO` & `puan_db_python-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puan-db-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

