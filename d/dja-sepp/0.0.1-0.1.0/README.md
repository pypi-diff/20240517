# Comparing `tmp/dja_sepp-0.0.1.tar.gz` & `tmp/dja_sepp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dja_sepp-0.0.1.tar", last modified: Fri May 17 08:36:46 2024, max compression
+gzip compressed data, was "dja_sepp-0.1.0.tar", last modified: Fri May 17 08:37:51 2024, max compression
```

## Comparing `dja_sepp-0.0.1.tar` & `dja_sepp-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 08:36:46.178679 dja_sepp-0.0.1/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1071 2024-05-16 12:43:35.000000 dja_sepp-0.0.1/LICENSE
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 08:36:46.175409 dja_sepp-0.0.1/PKG-INFO
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1640 2024-05-16 12:32:24.000000 dja_sepp-0.0.1/README.md
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)      703 2024-05-16 14:57:24.000000 dja_sepp-0.0.1/pyproject.toml
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)       38 2024-05-17 08:36:46.179683 dja_sepp-0.0.1/setup.cfg
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 08:36:46.146246 dja_sepp-0.0.1/src/
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 08:36:46.163938 dja_sepp-0.0.1/src/dja_sepp/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)      665 2024-05-17 08:32:36.000000 dja_sepp-0.0.1/src/dja_sepp/__init__.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     4778 2024-05-16 12:32:24.000000 dja_sepp-0.0.1/src/dja_sepp/psfex.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     3563 2024-05-17 08:10:03.000000 dja_sepp-0.0.1/src/dja_sepp/s3.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     9073 2024-05-17 08:36:10.000000 dja_sepp-0.0.1/src/dja_sepp/sepp.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    22764 2024-05-17 07:41:45.000000 dja_sepp-0.0.1/src/dja_sepp/sextractor.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6936 2024-05-17 08:36:35.000000 dja_sepp-0.0.1/src/dja_sepp/tiles.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    13791 2024-05-17 08:24:27.000000 dja_sepp-0.0.1/src/dja_sepp/utils.py
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 08:36:46.174395 dja_sepp-0.0.1/src/dja_sepp.egg-info/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 08:36:46.000000 dja_sepp-0.0.1/src/dja_sepp.egg-info/PKG-INFO
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)      369 2024-05-17 08:36:46.000000 dja_sepp-0.0.1/src/dja_sepp.egg-info/SOURCES.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)        1 2024-05-17 08:36:46.000000 dja_sepp-0.0.1/src/dja_sepp.egg-info/dependency_links.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)       51 2024-05-17 08:36:46.000000 dja_sepp-0.0.1/src/dja_sepp.egg-info/requires.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)        9 2024-05-17 08:36:46.000000 dja_sepp-0.0.1/src/dja_sepp.egg-info/top_level.txt
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 08:37:51.526536 dja_sepp-0.1.0/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1071 2024-05-16 12:43:35.000000 dja_sepp-0.1.0/LICENSE
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 08:37:51.523411 dja_sepp-0.1.0/PKG-INFO
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1640 2024-05-16 12:32:24.000000 dja_sepp-0.1.0/README.md
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)      703 2024-05-17 08:37:42.000000 dja_sepp-0.1.0/pyproject.toml
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)       38 2024-05-17 08:37:51.527041 dja_sepp-0.1.0/setup.cfg
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 08:37:51.493027 dja_sepp-0.1.0/src/
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 08:37:51.510192 dja_sepp-0.1.0/src/dja_sepp/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)      656 2024-05-17 08:37:29.000000 dja_sepp-0.1.0/src/dja_sepp/__init__.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     4778 2024-05-16 12:32:24.000000 dja_sepp-0.1.0/src/dja_sepp/psfex.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     3563 2024-05-17 08:10:03.000000 dja_sepp-0.1.0/src/dja_sepp/s3.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     9073 2024-05-17 08:36:10.000000 dja_sepp-0.1.0/src/dja_sepp/sepp.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    22764 2024-05-17 07:41:45.000000 dja_sepp-0.1.0/src/dja_sepp/sextractor.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6936 2024-05-17 08:36:35.000000 dja_sepp-0.1.0/src/dja_sepp/tiles.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    13791 2024-05-17 08:24:27.000000 dja_sepp-0.1.0/src/dja_sepp/utils.py
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 08:37:51.522125 dja_sepp-0.1.0/src/dja_sepp.egg-info/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 08:37:51.000000 dja_sepp-0.1.0/src/dja_sepp.egg-info/PKG-INFO
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)      369 2024-05-17 08:37:51.000000 dja_sepp-0.1.0/src/dja_sepp.egg-info/SOURCES.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)        1 2024-05-17 08:37:51.000000 dja_sepp-0.1.0/src/dja_sepp.egg-info/dependency_links.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)       51 2024-05-17 08:37:51.000000 dja_sepp-0.1.0/src/dja_sepp.egg-info/requires.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)        9 2024-05-17 08:37:51.000000 dja_sepp-0.1.0/src/dja_sepp.egg-info/top_level.txt
```

### Comparing `dja_sepp-0.0.1/LICENSE` & `dja_sepp-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.0.1/PKG-INFO` & `dja_sepp-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dja_sepp
-Version: 0.0.1
+Version: 0.1.0
 Summary: Package to run SourceXtractor++ on the DAWN JWST Archive
 Author-email: Aurélien Genin <aurelien.genin@polytechnique.org>
 Project-URL: Source, https://github.com/AstroAure/DJA-SEpp
 Project-URL: DJA, https://dawn-cph.github.io/dja/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dja_sepp-0.0.1/README.md` & `dja_sepp-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.0.1/pyproject.toml` & `dja_sepp-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dja_sepp"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
     {name="Aurélien Genin", email="aurelien.genin@polytechnique.org"}
 ]
 description = "Package to run SourceXtractor++ on the DAWN JWST Archive"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dja_sepp-0.0.1/src/dja_sepp/__init__.py` & `dja_sepp-0.1.0/src/dja_sepp/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 from .utils import color_dict, channel_dict, channel_color_dict, filters_waveband, add_good_scalebar, save_cutouts, show_source, plot_filters, plot_photometric_spectrum
 from .s3 import find_files, decompress_save, decompress_save_to_S3, save_s3
 from .sextractor import run_sextractor, show_vignets, plot_MuvMAG, hist_CLASS_STAR, plot_SNR_radius, plot_MuvMAG_manual, find_star_line, MUvMAG_star_selection, save_catalog, extract_stars, extract_stars_catalog
 from .psfex import run_psfex, compare_star
-from .sepp import find_images, run_sepp, save_s3, main_tile, main_run
+from .sepp import find_images, run_sepp, main_tile, main_run
 from .tiles import create_tiles, tile_positions, tile_grid, save_tiles, plot_tiles, batch_tiling
```

### Comparing `dja_sepp-0.0.1/src/dja_sepp/psfex.py` & `dja_sepp-0.1.0/src/dja_sepp/psfex.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.0.1/src/dja_sepp/s3.py` & `dja_sepp-0.1.0/src/dja_sepp/s3.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.0.1/src/dja_sepp/sepp.py` & `dja_sepp-0.1.0/src/dja_sepp/sepp.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.0.1/src/dja_sepp/sextractor.py` & `dja_sepp-0.1.0/src/dja_sepp/sextractor.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.0.1/src/dja_sepp/tiles.py` & `dja_sepp-0.1.0/src/dja_sepp/tiles.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.0.1/src/dja_sepp/utils.py` & `dja_sepp-0.1.0/src/dja_sepp/utils.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.0.1/src/dja_sepp.egg-info/PKG-INFO` & `dja_sepp-0.1.0/src/dja_sepp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dja_sepp
-Version: 0.0.1
+Version: 0.1.0
 Summary: Package to run SourceXtractor++ on the DAWN JWST Archive
 Author-email: Aurélien Genin <aurelien.genin@polytechnique.org>
 Project-URL: Source, https://github.com/AstroAure/DJA-SEpp
 Project-URL: DJA, https://dawn-cph.github.io/dja/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

