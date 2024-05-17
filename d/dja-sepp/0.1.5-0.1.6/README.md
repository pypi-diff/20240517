# Comparing `tmp/dja_sepp-0.1.5.tar.gz` & `tmp/dja_sepp-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dja_sepp-0.1.5.tar", last modified: Fri May 17 09:36:03 2024, max compression
+gzip compressed data, was "dja_sepp-0.1.6.tar", last modified: Fri May 17 09:38:01 2024, max compression
```

## Comparing `dja_sepp-0.1.5.tar` & `dja_sepp-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:36:03.952486 dja_sepp-0.1.5/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1071 2024-05-16 12:43:35.000000 dja_sepp-0.1.5/LICENSE
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 09:36:03.950406 dja_sepp-0.1.5/PKG-INFO
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1640 2024-05-16 12:32:24.000000 dja_sepp-0.1.5/README.md
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)      806 2024-05-17 09:35:48.000000 dja_sepp-0.1.5/pyproject.toml
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)       38 2024-05-17 09:36:03.952990 dja_sepp-0.1.5/setup.cfg
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:36:03.911651 dja_sepp-0.1.5/src/
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:36:03.932234 dja_sepp-0.1.5/src/dja_sepp/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)      656 2024-05-17 08:37:29.000000 dja_sepp-0.1.5/src/dja_sepp/__init__.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     4778 2024-05-16 12:32:24.000000 dja_sepp-0.1.5/src/dja_sepp/psfex.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     3563 2024-05-17 08:10:03.000000 dja_sepp-0.1.5/src/dja_sepp/s3.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     9073 2024-05-17 08:36:10.000000 dja_sepp-0.1.5/src/dja_sepp/sepp.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    22764 2024-05-17 07:41:45.000000 dja_sepp-0.1.5/src/dja_sepp/sextractor.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6936 2024-05-17 08:36:35.000000 dja_sepp-0.1.5/src/dja_sepp/tiles.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    14100 2024-05-17 09:21:37.000000 dja_sepp-0.1.5/src/dja_sepp/utils.py
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:36:03.948345 dja_sepp-0.1.5/src/dja_sepp.egg-info/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 09:36:03.000000 dja_sepp-0.1.5/src/dja_sepp.egg-info/PKG-INFO
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)      369 2024-05-17 09:36:03.000000 dja_sepp-0.1.5/src/dja_sepp.egg-info/SOURCES.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)        1 2024-05-17 09:36:03.000000 dja_sepp-0.1.5/src/dja_sepp.egg-info/dependency_links.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)       51 2024-05-17 09:36:03.000000 dja_sepp-0.1.5/src/dja_sepp.egg-info/requires.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)        9 2024-05-17 09:36:03.000000 dja_sepp-0.1.5/src/dja_sepp.egg-info/top_level.txt
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:38:01.745075 dja_sepp-0.1.6/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1071 2024-05-16 12:43:35.000000 dja_sepp-0.1.6/LICENSE
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 09:38:01.743131 dja_sepp-0.1.6/PKG-INFO
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1640 2024-05-16 12:32:24.000000 dja_sepp-0.1.6/README.md
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)      835 2024-05-17 09:37:49.000000 dja_sepp-0.1.6/pyproject.toml
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)       38 2024-05-17 09:38:01.745582 dja_sepp-0.1.6/setup.cfg
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:38:01.714939 dja_sepp-0.1.6/src/
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:38:01.731727 dja_sepp-0.1.6/src/dja_sepp/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)      656 2024-05-17 08:37:29.000000 dja_sepp-0.1.6/src/dja_sepp/__init__.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     4778 2024-05-16 12:32:24.000000 dja_sepp-0.1.6/src/dja_sepp/psfex.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     3563 2024-05-17 08:10:03.000000 dja_sepp-0.1.6/src/dja_sepp/s3.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     9073 2024-05-17 08:36:10.000000 dja_sepp-0.1.6/src/dja_sepp/sepp.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    22764 2024-05-17 07:41:45.000000 dja_sepp-0.1.6/src/dja_sepp/sextractor.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6936 2024-05-17 08:36:35.000000 dja_sepp-0.1.6/src/dja_sepp/tiles.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    14100 2024-05-17 09:21:37.000000 dja_sepp-0.1.6/src/dja_sepp/utils.py
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:38:01.741010 dja_sepp-0.1.6/src/dja_sepp.egg-info/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 09:38:01.000000 dja_sepp-0.1.6/src/dja_sepp.egg-info/PKG-INFO
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)      369 2024-05-17 09:38:01.000000 dja_sepp-0.1.6/src/dja_sepp.egg-info/SOURCES.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)        1 2024-05-17 09:38:01.000000 dja_sepp-0.1.6/src/dja_sepp.egg-info/dependency_links.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)       51 2024-05-17 09:38:01.000000 dja_sepp-0.1.6/src/dja_sepp.egg-info/requires.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)        9 2024-05-17 09:38:01.000000 dja_sepp-0.1.6/src/dja_sepp.egg-info/top_level.txt
```

### Comparing `dja_sepp-0.1.5/LICENSE` & `dja_sepp-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.5/PKG-INFO` & `dja_sepp-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dja_sepp
-Version: 0.1.5
+Version: 0.1.6
 Summary: Package to run SourceXtractor++ on the DAWN JWST Archive
 Author-email: Aurélien Genin <aurelien.genin@polytechnique.org>
 Project-URL: Source, https://github.com/AstroAure/DJA-SEpp
 Project-URL: DJA, https://dawn-cph.github.io/dja/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dja_sepp-0.1.5/README.md` & `dja_sepp-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.5/pyproject.toml` & `dja_sepp-0.1.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dja_sepp"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
     {name="Aurélien Genin", email="aurelien.genin@polytechnique.org"}
 ]
 description = "Package to run SourceXtractor++ on the DAWN JWST Archive"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -29,8 +29,8 @@
 Source = "https://github.com/AstroAure/DJA-SEpp"
 DJA = "https://dawn-cph.github.io/dja/"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-"mypkg.data" = ["**"]
+"mypkg.data" = ["NIRCam_Filters-Throughput/*.txt"]
```

### Comparing `dja_sepp-0.1.5/src/dja_sepp/__init__.py` & `dja_sepp-0.1.6/src/dja_sepp/__init__.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.5/src/dja_sepp/psfex.py` & `dja_sepp-0.1.6/src/dja_sepp/psfex.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.5/src/dja_sepp/s3.py` & `dja_sepp-0.1.6/src/dja_sepp/s3.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.5/src/dja_sepp/sepp.py` & `dja_sepp-0.1.6/src/dja_sepp/sepp.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.5/src/dja_sepp/sextractor.py` & `dja_sepp-0.1.6/src/dja_sepp/sextractor.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.5/src/dja_sepp/tiles.py` & `dja_sepp-0.1.6/src/dja_sepp/tiles.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.5/src/dja_sepp/utils.py` & `dja_sepp-0.1.6/src/dja_sepp/utils.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.5/src/dja_sepp.egg-info/PKG-INFO` & `dja_sepp-0.1.6/src/dja_sepp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dja_sepp
-Version: 0.1.5
+Version: 0.1.6
 Summary: Package to run SourceXtractor++ on the DAWN JWST Archive
 Author-email: Aurélien Genin <aurelien.genin@polytechnique.org>
 Project-URL: Source, https://github.com/AstroAure/DJA-SEpp
 Project-URL: DJA, https://dawn-cph.github.io/dja/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

