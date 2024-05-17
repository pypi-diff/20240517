# Comparing `tmp/QuaPy-0.1.8.tar.gz` & `tmp/QuaPy-0.1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuaPy-0.1.8.tar", last modified: Wed Feb 14 13:48:33 2024, max compression
+gzip compressed data, was "QuaPy-0.1.8.1.tar", last modified: Fri May 17 12:52:57 2024, max compression
```

## Comparing `QuaPy-0.1.8.tar` & `QuaPy-0.1.8.1.tar`

### file list

```diff
@@ -1,59 +1,55 @@
-drwxrwxr-x   0 moreo     (1000) moreo     (1000)        0 2024-02-14 13:48:33.830253 QuaPy-0.1.8/
--rw-r--r--   0 moreo     (1000) moreo     (1000)     1516 2022-03-08 09:50:52.000000 QuaPy-0.1.8/LICENSE
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     6563 2024-02-14 13:48:33.830253 QuaPy-0.1.8/PKG-INFO
-drwxrwxr-x   0 moreo     (1000) moreo     (1000)        0 2024-02-14 13:48:33.826254 QuaPy-0.1.8/QuaPy.egg-info/
--rw-r--r--   0 moreo     (1000) moreo     (1000)     6563 2024-02-14 13:48:33.000000 QuaPy-0.1.8/QuaPy.egg-info/PKG-INFO
--rw-r--r--   0 moreo     (1000) moreo     (1000)     1226 2024-02-14 13:48:33.000000 QuaPy-0.1.8/QuaPy.egg-info/SOURCES.txt
--rw-r--r--   0 moreo     (1000) moreo     (1000)        1 2024-02-14 13:48:33.000000 QuaPy-0.1.8/QuaPy.egg-info/dependency_links.txt
--rw-r--r--   0 moreo     (1000) moreo     (1000)       69 2024-02-14 13:48:33.000000 QuaPy-0.1.8/QuaPy.egg-info/requires.txt
--rw-r--r--   0 moreo     (1000) moreo     (1000)        6 2024-02-14 13:48:33.000000 QuaPy-0.1.8/QuaPy.egg-info/top_level.txt
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     5287 2024-02-14 13:39:22.000000 QuaPy-0.1.8/README.md
-drwxrwxr-x   0 moreo     (1000) moreo     (1000)        0 2024-02-14 13:48:33.826254 QuaPy-0.1.8/quapy/
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     1329 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/__init__.py
-drwxrwxr-x   0 moreo     (1000) moreo     (1000)        0 2024-02-14 13:48:33.826254 QuaPy-0.1.8/quapy/benchmarking/
--rw-rw-r--   0 moreo     (1000) moreo     (1000)        0 2024-01-29 09:28:42.000000 QuaPy-0.1.8/quapy/benchmarking/__init__.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     8363 2024-02-14 10:13:42.000000 QuaPy-0.1.8/quapy/benchmarking/_base.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)      923 2024-01-29 12:55:56.000000 QuaPy-0.1.8/quapy/benchmarking/typical.py
-drwxrwxr-x   0 moreo     (1000) moreo     (1000)        0 2024-02-14 13:48:33.826254 QuaPy-0.1.8/quapy/classification/
--rw-rw-r--   0 moreo     (1000) moreo     (1000)       21 2022-03-14 15:41:55.000000 QuaPy-0.1.8/quapy/classification/__init__.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    10620 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/classification/calibration.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     4100 2024-02-12 12:02:10.000000 QuaPy-0.1.8/quapy/classification/methods.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    22578 2024-02-12 12:02:10.000000 QuaPy-0.1.8/quapy/classification/neural.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     6591 2024-02-12 12:02:10.000000 QuaPy-0.1.8/quapy/classification/svmperf.py
-drwxrwxr-x   0 moreo     (1000) moreo     (1000)        0 2024-02-14 13:48:33.826254 QuaPy-0.1.8/quapy/data/
--rw-rw-r--   0 moreo     (1000) moreo     (1000)       95 2022-03-14 15:41:55.000000 QuaPy-0.1.8/quapy/data/__init__.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     3634 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/data/_ifcb.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     6445 2024-02-13 15:49:28.000000 QuaPy-0.1.8/quapy/data/_lequa2022.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    26842 2024-02-12 12:02:10.000000 QuaPy-0.1.8/quapy/data/base.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    38310 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/data/datasets.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    11729 2024-02-12 12:02:10.000000 QuaPy-0.1.8/quapy/data/preprocessing.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     4413 2024-02-12 12:02:10.000000 QuaPy-0.1.8/quapy/data/reader.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    15668 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/error.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    10551 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/evaluation.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    15573 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/functional.py
-drwxrwxr-x   0 moreo     (1000) moreo     (1000)        0 2024-02-14 13:48:33.830253 QuaPy-0.1.8/quapy/method/
--rw-rw-r--   0 moreo     (1000) moreo     (1000)      698 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/method/__init__.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    17067 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/method/_kdey.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    18238 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/method/_neural.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    12958 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/method/_threshold_optim.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    66032 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/method/aggregative.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     4270 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/method/base.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    30692 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/method/meta.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     7049 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/method/non_aggregative.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    16053 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/model_selection.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    27620 2024-02-12 12:02:10.000000 QuaPy-0.1.8/quapy/plot.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    22836 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/protocol.py
-drwxrwxr-x   0 moreo     (1000) moreo     (1000)        0 2024-02-14 13:48:33.830253 QuaPy-0.1.8/quapy/tests/
--rw-rw-r--   0 moreo     (1000) moreo     (1000)        0 2023-10-23 09:36:42.000000 QuaPy-0.1.8/quapy/tests/__init__.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)       95 2023-10-23 09:36:42.000000 QuaPy-0.1.8/quapy/tests/test_base.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     2367 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/tests/test_datasets.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     2930 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/tests/test_evaluation.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     1010 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/tests/test_hierarchy.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     2325 2024-02-12 12:02:10.000000 QuaPy-0.1.8/quapy/tests/test_labelcollection.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     8707 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/tests/test_methods.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     4421 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/tests/test_modsel.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     6725 2024-02-12 12:02:10.000000 QuaPy-0.1.8/quapy/tests/test_protocols.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     3938 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/tests/test_replicability.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)    10288 2024-02-14 13:16:50.000000 QuaPy-0.1.8/quapy/util.py
--rw-rw-r--   0 moreo     (1000) moreo     (1000)       38 2024-02-14 13:48:33.830253 QuaPy-0.1.8/setup.cfg
--rw-rw-r--   0 moreo     (1000) moreo     (1000)     6664 2024-02-14 13:16:50.000000 QuaPy-0.1.8/setup.py
+drwxrwxr-x   0 moreo     (1000) moreo     (1000)        0 2024-05-17 12:52:57.516585 QuaPy-0.1.8.1/
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     1516 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/LICENSE
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     6565 2024-05-17 12:52:57.516585 QuaPy-0.1.8.1/PKG-INFO
+drwxrwxr-x   0 moreo     (1000) moreo     (1000)        0 2024-05-17 12:52:57.512585 QuaPy-0.1.8.1/QuaPy.egg-info/
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     6565 2024-05-17 12:52:57.000000 QuaPy-0.1.8.1/QuaPy.egg-info/PKG-INFO
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     1137 2024-05-17 12:52:57.000000 QuaPy-0.1.8.1/QuaPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)        1 2024-05-17 12:52:57.000000 QuaPy-0.1.8.1/QuaPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)       77 2024-05-17 12:52:57.000000 QuaPy-0.1.8.1/QuaPy.egg-info/requires.txt
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)        6 2024-05-17 12:52:57.000000 QuaPy-0.1.8.1/QuaPy.egg-info/top_level.txt
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     5287 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/README.md
+drwxrwxr-x   0 moreo     (1000) moreo     (1000)        0 2024-05-17 12:52:57.516585 QuaPy-0.1.8.1/quapy/
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     1331 2024-05-17 12:51:30.000000 QuaPy-0.1.8.1/quapy/__init__.py
+drwxrwxr-x   0 moreo     (1000) moreo     (1000)        0 2024-05-17 12:52:57.516585 QuaPy-0.1.8.1/quapy/classification/
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)       21 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/classification/__init__.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    10620 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/classification/calibration.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     4100 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/classification/methods.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    22578 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/classification/neural.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     6591 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/classification/svmperf.py
+drwxrwxr-x   0 moreo     (1000) moreo     (1000)        0 2024-05-17 12:52:57.516585 QuaPy-0.1.8.1/quapy/data/
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)       95 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/data/__init__.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     3634 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/data/_ifcb.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     6445 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/data/_lequa2022.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    26842 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/data/base.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    38310 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/data/datasets.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    11729 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/data/preprocessing.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     4413 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/data/reader.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    15668 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/error.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    10551 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/evaluation.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    15573 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/functional.py
+drwxrwxr-x   0 moreo     (1000) moreo     (1000)        0 2024-05-17 12:52:57.516585 QuaPy-0.1.8.1/quapy/method/
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)      698 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/method/__init__.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    17067 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/method/_kdey.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    18238 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/method/_neural.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    12958 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/method/_threshold_optim.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    66032 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/method/aggregative.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     4270 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/method/base.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    30692 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/method/meta.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     7049 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/method/non_aggregative.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    16053 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/model_selection.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    27625 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/plot.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    22836 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/protocol.py
+drwxrwxr-x   0 moreo     (1000) moreo     (1000)        0 2024-05-17 12:52:57.516585 QuaPy-0.1.8.1/quapy/tests/
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)        0 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/tests/__init__.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)       95 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/tests/test_base.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     2367 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/tests/test_datasets.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     2930 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/tests/test_evaluation.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     1010 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/tests/test_hierarchy.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     2325 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/tests/test_labelcollection.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     8707 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/tests/test_methods.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     4421 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/tests/test_modsel.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     6725 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/tests/test_protocols.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     3938 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/tests/test_replicability.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)    10288 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/quapy/util.py
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)       38 2024-05-17 12:52:57.516585 QuaPy-0.1.8.1/setup.cfg
+-rw-rw-r--   0 moreo     (1000) moreo     (1000)     6675 2024-05-17 12:49:45.000000 QuaPy-0.1.8.1/setup.py
```

### Comparing `QuaPy-0.1.8/LICENSE` & `QuaPy-0.1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/PKG-INFO` & `QuaPy-0.1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuaPy
-Version: 0.1.8
+Version: 0.1.8.1
 Summary: QuaPy: a framework for Quantification in Python
 Home-page: https://github.com/HLT-ISTI/QuaPy
 Maintainer: Alejandro Moreo
 Maintainer-email: alejandro.moreo@isti.cnr.it
 Project-URL: Contributors, https://github.com/HLT-ISTI/QuaPy/graphs/contributors
 Project-URL: Bug Reports, https://github.com/HLT-ISTI/QuaPy/issues
 Project-URL: Wiki, https://github.com/HLT-ISTI/QuaPy/wiki
```

### Comparing `QuaPy-0.1.8/QuaPy.egg-info/PKG-INFO` & `QuaPy-0.1.8.1/QuaPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuaPy
-Version: 0.1.8
+Version: 0.1.8.1
 Summary: QuaPy: a framework for Quantification in Python
 Home-page: https://github.com/HLT-ISTI/QuaPy
 Maintainer: Alejandro Moreo
 Maintainer-email: alejandro.moreo@isti.cnr.it
 Project-URL: Contributors, https://github.com/HLT-ISTI/QuaPy/graphs/contributors
 Project-URL: Bug Reports, https://github.com/HLT-ISTI/QuaPy/issues
 Project-URL: Wiki, https://github.com/HLT-ISTI/QuaPy/wiki
```

### Comparing `QuaPy-0.1.8/QuaPy.egg-info/SOURCES.txt` & `QuaPy-0.1.8.1/QuaPy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 quapy/error.py
 quapy/evaluation.py
 quapy/functional.py
 quapy/model_selection.py
 quapy/plot.py
 quapy/protocol.py
 quapy/util.py
-quapy/benchmarking/__init__.py
-quapy/benchmarking/_base.py
-quapy/benchmarking/typical.py
 quapy/classification/__init__.py
 quapy/classification/calibration.py
 quapy/classification/methods.py
 quapy/classification/neural.py
 quapy/classification/svmperf.py
 quapy/data/__init__.py
 quapy/data/_ifcb.py
```

### Comparing `QuaPy-0.1.8/README.md` & `QuaPy-0.1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/__init__.py` & `QuaPy-0.1.8.1/quapy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from . import evaluation
 from . import protocol
 from . import plot
 from . import util
 from . import model_selection
 from . import classification
 
-__version__ = '0.1.8'
+__version__ = '0.1.8.1'
 
 environ = {
     'SAMPLE_SIZE': None,
     'UNK_TOKEN': '[UNK]',
     'UNK_INDEX': 0,
     'PAD_TOKEN': '[PAD]',
     'PAD_INDEX': 1,
```

### Comparing `QuaPy-0.1.8/quapy/classification/calibration.py` & `QuaPy-0.1.8.1/quapy/classification/calibration.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/classification/methods.py` & `QuaPy-0.1.8.1/quapy/classification/methods.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/classification/neural.py` & `QuaPy-0.1.8.1/quapy/classification/neural.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/classification/svmperf.py` & `QuaPy-0.1.8.1/quapy/classification/svmperf.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/data/_ifcb.py` & `QuaPy-0.1.8.1/quapy/data/_ifcb.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/data/_lequa2022.py` & `QuaPy-0.1.8.1/quapy/data/_lequa2022.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/data/base.py` & `QuaPy-0.1.8.1/quapy/data/base.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/data/datasets.py` & `QuaPy-0.1.8.1/quapy/data/datasets.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/data/preprocessing.py` & `QuaPy-0.1.8.1/quapy/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/data/reader.py` & `QuaPy-0.1.8.1/quapy/data/reader.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/error.py` & `QuaPy-0.1.8.1/quapy/error.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/evaluation.py` & `QuaPy-0.1.8.1/quapy/evaluation.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/functional.py` & `QuaPy-0.1.8.1/quapy/functional.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/method/__init__.py` & `QuaPy-0.1.8.1/quapy/method/__init__.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/method/_kdey.py` & `QuaPy-0.1.8.1/quapy/method/_kdey.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/method/_neural.py` & `QuaPy-0.1.8.1/quapy/method/_neural.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/method/_threshold_optim.py` & `QuaPy-0.1.8.1/quapy/method/_threshold_optim.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/method/aggregative.py` & `QuaPy-0.1.8.1/quapy/method/aggregative.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/method/base.py` & `QuaPy-0.1.8.1/quapy/method/base.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/method/meta.py` & `QuaPy-0.1.8.1/quapy/method/meta.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/method/non_aggregative.py` & `QuaPy-0.1.8.1/quapy/method/non_aggregative.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/model_selection.py` & `QuaPy-0.1.8.1/quapy/model_selection.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/plot.py` & `QuaPy-0.1.8.1/quapy/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import defaultdict
 import matplotlib.pyplot as plt
-from matplotlib.cm import get_cmap
+from matplotlib.pyplot import get_cmap
 import numpy as np
 from matplotlib import cm
 from scipy.stats import ttest_ind_from_stats
 from matplotlib.ticker import ScalarFormatter
 import math
 
 import quapy as qp
@@ -563,8 +563,8 @@
 
         method_drifts = y_error(test_prevs_i, estim_prevs_i)
         data[method]['y'] = np.concatenate([data[method]['y'], method_drifts])
 
         if method not in method_order:
             method_order.append(method)
 
-    return data
+    return data
```

### Comparing `QuaPy-0.1.8/quapy/protocol.py` & `QuaPy-0.1.8.1/quapy/protocol.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/tests/test_datasets.py` & `QuaPy-0.1.8.1/quapy/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/tests/test_evaluation.py` & `QuaPy-0.1.8.1/quapy/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/tests/test_hierarchy.py` & `QuaPy-0.1.8.1/quapy/tests/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/tests/test_labelcollection.py` & `QuaPy-0.1.8.1/quapy/tests/test_labelcollection.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/tests/test_methods.py` & `QuaPy-0.1.8.1/quapy/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/tests/test_modsel.py` & `QuaPy-0.1.8.1/quapy/tests/test_modsel.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/tests/test_protocols.py` & `QuaPy-0.1.8.1/quapy/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/tests/test_replicability.py` & `QuaPy-0.1.8.1/quapy/tests/test_replicability.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/quapy/util.py` & `QuaPy-0.1.8.1/quapy/util.py`

 * *Files identical despite different names*

### Comparing `QuaPy-0.1.8/setup.py` & `QuaPy-0.1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     #
     #   py_modules=["my_module"],
     #
     packages=find_packages(include=['quapy', 'quapy.*']),  # Required
 
     python_requires='>=3.8, <4',
 
-    install_requires=['scikit-learn', 'pandas', 'tqdm', 'matplotlib', 'joblib', 'xlrd', 'abstention', 'ucimlrepo'],
+    install_requires=['scikit-learn', 'pandas', 'tqdm', 'matplotlib', 'joblib', 'xlrd', 'abstention', 'ucimlrepo', 'certifi'],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
```

