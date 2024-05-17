# Comparing `tmp/trust_plutus_namematch-0.3.tar.gz` & `tmp/trust_plutus_namematch-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trust_plutus_namematch-0.3.tar", max compression
+gzip compressed data, was "trust_plutus_namematch-0.5.tar", max compression
```

## Comparing `trust_plutus_namematch-0.3.tar` & `trust_plutus_namematch-0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35821 2024-03-20 09:06:41.708383 trust_plutus_namematch-0.3/LICENSE
--rw-r--r--   0        0        0      474 2024-05-10 06:55:18.842924 trust_plutus_namematch-0.3/pyproject.toml
--rw-r--r--   0        0        0      435 2024-05-10 06:55:13.290252 trust_plutus_namematch-0.3/README.md
--rw-r--r--   0        0        0        0 2024-05-09 10:32:15.022349 trust_plutus_namematch-0.3/trust_plutus_namematch/__init__.py
--rw-r--r--   0        0        0     1515 2024-05-10 06:28:57.924280 trust_plutus_namematch-0.3/trust_plutus_namematch/match.py
--rw-r--r--   0        0        0        0 2024-02-12 07:49:10.008013 trust_plutus_namematch-0.3/trust_plutus_namematch/utils/__init__.py
--rw-r--r--   0        0        0      425 2024-05-09 10:37:36.797518 trust_plutus_namematch-0.3/trust_plutus_namematch/utils/logs.py
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 trust_plutus_namematch-0.3/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-03-20 09:06:41.708383 trust_plutus_namematch-0.5/LICENSE
+-rw-r--r--   0        0        0      491 2024-05-16 11:19:30.761799 trust_plutus_namematch-0.5/pyproject.toml
+-rw-r--r--   0        0        0      435 2024-05-10 06:55:13.290252 trust_plutus_namematch-0.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 10:32:15.022349 trust_plutus_namematch-0.5/trust_plutus_namematch/__init__.py
+-rw-r--r--   0        0        0     1515 2024-05-10 06:28:57.924280 trust_plutus_namematch-0.5/trust_plutus_namematch/match.py
+-rw-r--r--   0        0        0        0 2024-02-12 07:49:10.008013 trust_plutus_namematch-0.5/trust_plutus_namematch/utils/__init__.py
+-rw-r--r--   0        0        0      425 2024-05-09 10:37:36.797518 trust_plutus_namematch-0.5/trust_plutus_namematch/utils/logs.py
+-rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 trust_plutus_namematch-0.5/PKG-INFO
```

### Comparing `trust_plutus_namematch-0.3/LICENSE` & `trust_plutus_namematch-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trust_plutus_namematch-0.3/trust_plutus_namematch/match.py` & `trust_plutus_namematch-0.5/trust_plutus_namematch/match.py`

 * *Files identical despite different names*

### Comparing `trust_plutus_namematch-0.3/PKG-INFO` & `trust_plutus_namematch-0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: trust-plutus-namematch
-Version: 0.3
+Version: 0.5
 Summary: Name match for fund names from ICRA and MILES
 License: OSI Approved :: GNU General Public License v3 (GPLv3)
 Author: Rolf Lobo
-Requires-Python: ==3.10.12
+Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: joblib (>=1.4.2,<2.0.0)
 Requires-Dist: loga (>=1.0.0,<2.0.0)
 Requires-Dist: numpy (==1.25.2)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (==2.0.3)
 Requires-Dist: rapidfuzz (==3.9.0)
 Description-Content-Type: text/markdown
```

