# Comparing `tmp/dja_sepp-0.1.3.tar.gz` & `tmp/dja_sepp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dja_sepp-0.1.3.tar", last modified: Fri May 17 09:28:43 2024, max compression
+gzip compressed data, was "dja_sepp-0.1.4.tar", last modified: Fri May 17 09:30:47 2024, max compression
```

## Comparing `dja_sepp-0.1.3.tar` & `dja_sepp-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:28:43.552432 dja_sepp-0.1.3/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1071 2024-05-16 12:43:35.000000 dja_sepp-0.1.3/LICENSE
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 09:28:43.550953 dja_sepp-0.1.3/PKG-INFO
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1640 2024-05-16 12:32:24.000000 dja_sepp-0.1.3/README.md
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)      813 2024-05-17 09:28:31.000000 dja_sepp-0.1.3/pyproject.toml
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)       38 2024-05-17 09:28:43.552941 dja_sepp-0.1.3/setup.cfg
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:28:43.520357 dja_sepp-0.1.3/src/
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:28:43.538407 dja_sepp-0.1.3/src/dja_sepp/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)      656 2024-05-17 08:37:29.000000 dja_sepp-0.1.3/src/dja_sepp/__init__.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     4778 2024-05-16 12:32:24.000000 dja_sepp-0.1.3/src/dja_sepp/psfex.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     3563 2024-05-17 08:10:03.000000 dja_sepp-0.1.3/src/dja_sepp/s3.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     9073 2024-05-17 08:36:10.000000 dja_sepp-0.1.3/src/dja_sepp/sepp.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    22764 2024-05-17 07:41:45.000000 dja_sepp-0.1.3/src/dja_sepp/sextractor.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6936 2024-05-17 08:36:35.000000 dja_sepp-0.1.3/src/dja_sepp/tiles.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    14100 2024-05-17 09:21:37.000000 dja_sepp-0.1.3/src/dja_sepp/utils.py
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:28:43.548938 dja_sepp-0.1.3/src/dja_sepp.egg-info/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 09:28:43.000000 dja_sepp-0.1.3/src/dja_sepp.egg-info/PKG-INFO
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)      369 2024-05-17 09:28:43.000000 dja_sepp-0.1.3/src/dja_sepp.egg-info/SOURCES.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)        1 2024-05-17 09:28:43.000000 dja_sepp-0.1.3/src/dja_sepp.egg-info/dependency_links.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)       51 2024-05-17 09:28:43.000000 dja_sepp-0.1.3/src/dja_sepp.egg-info/requires.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)        9 2024-05-17 09:28:43.000000 dja_sepp-0.1.3/src/dja_sepp.egg-info/top_level.txt
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:30:47.047640 dja_sepp-0.1.4/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1071 2024-05-16 12:43:35.000000 dja_sepp-0.1.4/LICENSE
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 09:30:47.044618 dja_sepp-0.1.4/PKG-INFO
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1640 2024-05-16 12:32:24.000000 dja_sepp-0.1.4/README.md
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)      804 2024-05-17 09:30:31.000000 dja_sepp-0.1.4/pyproject.toml
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)       38 2024-05-17 09:30:47.048149 dja_sepp-0.1.4/setup.cfg
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:30:47.012886 dja_sepp-0.1.4/src/
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:30:47.028086 dja_sepp-0.1.4/src/dja_sepp/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)      656 2024-05-17 08:37:29.000000 dja_sepp-0.1.4/src/dja_sepp/__init__.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     4778 2024-05-16 12:32:24.000000 dja_sepp-0.1.4/src/dja_sepp/psfex.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     3563 2024-05-17 08:10:03.000000 dja_sepp-0.1.4/src/dja_sepp/s3.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     9073 2024-05-17 08:36:10.000000 dja_sepp-0.1.4/src/dja_sepp/sepp.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    22764 2024-05-17 07:41:45.000000 dja_sepp-0.1.4/src/dja_sepp/sextractor.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6936 2024-05-17 08:36:35.000000 dja_sepp-0.1.4/src/dja_sepp/tiles.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    14100 2024-05-17 09:21:37.000000 dja_sepp-0.1.4/src/dja_sepp/utils.py
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:30:47.042396 dja_sepp-0.1.4/src/dja_sepp.egg-info/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 09:30:46.000000 dja_sepp-0.1.4/src/dja_sepp.egg-info/PKG-INFO
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)      369 2024-05-17 09:30:47.000000 dja_sepp-0.1.4/src/dja_sepp.egg-info/SOURCES.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)        1 2024-05-17 09:30:46.000000 dja_sepp-0.1.4/src/dja_sepp.egg-info/dependency_links.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)       51 2024-05-17 09:30:46.000000 dja_sepp-0.1.4/src/dja_sepp.egg-info/requires.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)        9 2024-05-17 09:30:46.000000 dja_sepp-0.1.4/src/dja_sepp.egg-info/top_level.txt
```

### Comparing `dja_sepp-0.1.3/LICENSE` & `dja_sepp-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.3/PKG-INFO` & `dja_sepp-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dja_sepp
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package to run SourceXtractor++ on the DAWN JWST Archive
 Author-email: Aurélien Genin <aurelien.genin@polytechnique.org>
 Project-URL: Source, https://github.com/AstroAure/DJA-SEpp
 Project-URL: DJA, https://dawn-cph.github.io/dja/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dja_sepp-0.1.3/README.md` & `dja_sepp-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.3/pyproject.toml` & `dja_sepp-0.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dja_sepp"
-version = "0.1.3"
+version = "0.1.4"
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
-mypkg = ["data/*", "data/*"]
+mypkg = ["data/**"]
```

### Comparing `dja_sepp-0.1.3/src/dja_sepp/__init__.py` & `dja_sepp-0.1.4/src/dja_sepp/__init__.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.3/src/dja_sepp/psfex.py` & `dja_sepp-0.1.4/src/dja_sepp/psfex.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.3/src/dja_sepp/s3.py` & `dja_sepp-0.1.4/src/dja_sepp/s3.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.3/src/dja_sepp/sepp.py` & `dja_sepp-0.1.4/src/dja_sepp/sepp.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.3/src/dja_sepp/sextractor.py` & `dja_sepp-0.1.4/src/dja_sepp/sextractor.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.3/src/dja_sepp/tiles.py` & `dja_sepp-0.1.4/src/dja_sepp/tiles.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.3/src/dja_sepp/utils.py` & `dja_sepp-0.1.4/src/dja_sepp/utils.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.3/src/dja_sepp.egg-info/PKG-INFO` & `dja_sepp-0.1.4/src/dja_sepp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dja_sepp
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package to run SourceXtractor++ on the DAWN JWST Archive
 Author-email: Aurélien Genin <aurelien.genin@polytechnique.org>
 Project-URL: Source, https://github.com/AstroAure/DJA-SEpp
 Project-URL: DJA, https://dawn-cph.github.io/dja/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

