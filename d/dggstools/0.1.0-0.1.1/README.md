# Comparing `tmp/dggstools-0.1.0.tar.gz` & `tmp/dggstools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dggstools-0.1.0.tar", last modified: Tue May 14 16:02:46 2024, max compression
+gzip compressed data, was "dggstools-0.1.1.tar", last modified: Fri May 17 10:49:22 2024, max compression
```

## Comparing `dggstools-0.1.0.tar` & `dggstools-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:46.052418 dggstools-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-14 16:02:02.000000 dggstools-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9429 2024-05-14 16:02:46.052418 dggstools-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-05-14 16:02:02.000000 dggstools-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:46.048418 dggstools-0.1.0/dggstools/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-14 16:02:02.000000 dggstools-0.1.0/dggstools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-05-14 16:02:02.000000 dggstools-0.1.0/dggstools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:46.048418 dggstools-0.1.0/dggstools/auids/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-14 16:02:02.000000 dggstools-0.1.0/dggstools/auids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-05-14 16:02:02.000000 dggstools-0.1.0/dggstools/auids/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-05-14 16:02:02.000000 dggstools-0.1.0/dggstools/auids/rhpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:46.048418 dggstools-0.1.0/dggstools/rhpx/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-14 16:02:02.000000 dggstools-0.1.0/dggstools/rhpx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-05-14 16:02:02.000000 dggstools-0.1.0/dggstools/rhpx/raster_to_rhpx.py
--rw-r--r--   0 runner    (1001) docker     (127)    24759 2024-05-14 16:02:02.000000 dggstools-0.1.0/dggstools/rhpx/rhpx_gdf_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    16596 2024-05-14 16:02:02.000000 dggstools-0.1.0/dggstools/rhpx/rhpxutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:46.048418 dggstools-0.1.0/dggstools/rhpx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 16:02:02.000000 dggstools-0.1.0/dggstools/rhpx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-14 16:02:02.000000 dggstools-0.1.0/dggstools/rhpx/utils/rasterutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-14 16:02:02.000000 dggstools-0.1.0/dggstools/rhpx/utils/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-14 16:02:02.000000 dggstools-0.1.0/dggstools/rhpx/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-14 16:02:02.000000 dggstools-0.1.0/dggstools/rhpx/utils/vectorutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    36060 2024-05-14 16:02:02.000000 dggstools-0.1.0/dggstools/rhpx/vector_to_rhpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:46.048418 dggstools-0.1.0/dggstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9429 2024-05-14 16:02:45.000000 dggstools-0.1.0/dggstools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-14 16:02:45.000000 dggstools-0.1.0/dggstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:02:45.000000 dggstools-0.1.0/dggstools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 16:02:45.000000 dggstools-0.1.0/dggstools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-14 16:02:45.000000 dggstools-0.1.0/dggstools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 16:02:45.000000 dggstools-0.1.0/dggstools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-14 16:02:02.000000 dggstools-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-14 16:02:02.000000 dggstools-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:02:46.052418 dggstools-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:02:02.000000 dggstools-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:49:22.145201 dggstools-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-17 10:48:41.000000 dggstools-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-05-17 10:49:22.145201 dggstools-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-05-17 10:48:41.000000 dggstools-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:49:22.141201 dggstools-0.1.1/dggstools/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-17 10:48:41.000000 dggstools-0.1.1/dggstools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-05-17 10:48:41.000000 dggstools-0.1.1/dggstools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:49:22.145201 dggstools-0.1.1/dggstools/auids/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-17 10:48:41.000000 dggstools-0.1.1/dggstools/auids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-05-17 10:48:41.000000 dggstools-0.1.1/dggstools/auids/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-05-17 10:48:41.000000 dggstools-0.1.1/dggstools/auids/rhpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:49:22.145201 dggstools-0.1.1/dggstools/rhpx/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-17 10:48:41.000000 dggstools-0.1.1/dggstools/rhpx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-05-17 10:48:41.000000 dggstools-0.1.1/dggstools/rhpx/raster_to_rhpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24759 2024-05-17 10:48:41.000000 dggstools-0.1.1/dggstools/rhpx/rhpx_gdf_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16596 2024-05-17 10:48:41.000000 dggstools-0.1.1/dggstools/rhpx/rhpxutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:49:22.145201 dggstools-0.1.1/dggstools/rhpx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-17 10:48:41.000000 dggstools-0.1.1/dggstools/rhpx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-17 10:48:41.000000 dggstools-0.1.1/dggstools/rhpx/utils/rasterutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-17 10:48:41.000000 dggstools-0.1.1/dggstools/rhpx/utils/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-17 10:48:41.000000 dggstools-0.1.1/dggstools/rhpx/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-17 10:48:41.000000 dggstools-0.1.1/dggstools/rhpx/utils/vectorutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36060 2024-05-17 10:48:41.000000 dggstools-0.1.1/dggstools/rhpx/vector_to_rhpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:49:22.145201 dggstools-0.1.1/dggstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-05-17 10:49:22.000000 dggstools-0.1.1/dggstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-17 10:49:22.000000 dggstools-0.1.1/dggstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 10:49:22.000000 dggstools-0.1.1/dggstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-17 10:49:22.000000 dggstools-0.1.1/dggstools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-17 10:49:22.000000 dggstools-0.1.1/dggstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 10:49:22.000000 dggstools-0.1.1/dggstools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-17 10:48:41.000000 dggstools-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-17 10:48:41.000000 dggstools-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 10:49:22.145201 dggstools-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 10:48:41.000000 dggstools-0.1.1/setup.py
```

### Comparing `dggstools-0.1.0/LICENSE` & `dggstools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dggstools-0.1.0/PKG-INFO` & `dggstools-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dggstools
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library and command line tool to manipulate raster and vector GIS data in a DGGS (rHEALPix for now).
 Author-email: Rubén Béjar <rbejar@unizar.es>, Sergio Martin-Segura <segura@unizar.es>, "Francisco J. Lopez-Pellicer" <fjlopez@unizar.es>, Javier Nogueras-Iso <jnog@unizar.es>, "F. Javier Zarazaga-Soria" <javy@unizar.es>
 Project-URL: Homepage, https://github.com/IAAA-Lab/dggstools
 Project-URL: Issues, https://github.com/IAAA-Lab/dggstools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -19,39 +19,39 @@
 Requires-Dist: botocore==1.34.37
 Requires-Dist: build==1.0.3
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: click==8.1.2
 Requires-Dist: click-plugins==1.1.1
 Requires-Dist: cligj==0.7.2
 Requires-Dist: cycler==0.11.0
-Requires-Dist: Fiona==1.9.4.post1
+Requires-Dist: fiona==1.9.6
 Requires-Dist: fonttools==4.48.1
 Requires-Dist: GeoAlchemy2==0.12.5
 Requires-Dist: geopandas==0.14.0
 Requires-Dist: jmespath==1.0.0
 Requires-Dist: kiwisolver==1.4.2
-Requires-Dist: matplotlib==3.7.2
+Requires-Dist: matplotlib==3.8.4
 Requires-Dist: munch==2.5.0
 Requires-Dist: networkx==2.8.7
 Requires-Dist: numpy==1.26.4
-Requires-Dist: packaging==21.3
-Requires-Dist: pandas==1.4.3
-Requires-Dist: Pillow==10.2.0
+Requires-Dist: packaging==24.0
+Requires-Dist: pandas==2.2.2
+Requires-Dist: pillow==10.2.0
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: pyarrow==15.0.0
 Requires-Dist: pyogrio==0.7.2
 Requires-Dist: pyparsing==3.0.7
 Requires-Dist: pyproj==3.6.1
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: pytz==2022.1
 Requires-Dist: rasterio==1.3.9
 Requires-Dist: rHEALPixDGGS==0.5.4
 Requires-Dist: s3transfer==0.10.0
 Requires-Dist: scipy==1.12.0
-Requires-Dist: shapely==2.0.1
+Requires-Dist: shapely==2.0.4
 Requires-Dist: six==1.16.0
 Requires-Dist: snuggs==1.4.7
 Requires-Dist: SQLAlchemy==2.0.21
 Requires-Dist: SQLAlchemy-Utils==0.41.1
 Requires-Dist: typer[all]==0.9.0
 Requires-Dist: urllib3==2.0.7
 
@@ -63,31 +63,36 @@
 a DGGS (rHEALPix for now).
 
 **Requirements**
 - Python 3.10 or higher
 - `pip` for installing Python packages
 
 ## Install the package and the command line tool
-1. You can download the latest package released on the GitHub Repository if you want the latest, non-stable version:
-
-Get the .whl file from <https://github.com/IAAA-Lab/dggstools/releases/latest>.
-
-2. Install the package and command line tool
+1. If you want the latest stable version (which is in PyPi):
 
 ```
-pip install ./name-of-the-file-you-have-downloaded.whl
+pip install dggstools
 ```
 
-3. Now you can run dggstools in the command line:
+2. If you prefer the latest non-stable version, you can download the latest package released on the GitHub Repository:
+
+ - Get the .whl file from <https://github.com/IAAA-Lab/dggstools/releases/latest>.
+ -  Install this wheel file:
+
+ ```
+ pip install ./name-of-the-file-you-have-downloaded.whl
+ ```
+
+3. In any case, once installed you can run dggstools in the command line:
 
 ```
 dggstools --help
 ```
 
-You will see something like this:
+And you will see something like this:
 
 ```
 Usage: dggstools [OPTIONS] COMMAND [ARGS]...                                                                                                                          
                                                                                                                                                                        
 ╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --install-completion          Install completion for the current shell.                                                                                             │
 │ --show-completion             Show completion for the current shell, to copy it or customize the installation.                                                      │
```

### Comparing `dggstools-0.1.0/README.md` & `dggstools-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,31 +6,36 @@
 a DGGS (rHEALPix for now).
 
 **Requirements**
 - Python 3.10 or higher
 - `pip` for installing Python packages
 
 ## Install the package and the command line tool
-1. You can download the latest package released on the GitHub Repository if you want the latest, non-stable version:
-
-Get the .whl file from <https://github.com/IAAA-Lab/dggstools/releases/latest>.
-
-2. Install the package and command line tool
+1. If you want the latest stable version (which is in PyPi):
 
 ```
-pip install ./name-of-the-file-you-have-downloaded.whl
+pip install dggstools
 ```
 
-3. Now you can run dggstools in the command line:
+2. If you prefer the latest non-stable version, you can download the latest package released on the GitHub Repository:
+
+ - Get the .whl file from <https://github.com/IAAA-Lab/dggstools/releases/latest>.
+ -  Install this wheel file:
+
+ ```
+ pip install ./name-of-the-file-you-have-downloaded.whl
+ ```
+
+3. In any case, once installed you can run dggstools in the command line:
 
 ```
 dggstools --help
 ```
 
-You will see something like this:
+And you will see something like this:
 
 ```
 Usage: dggstools [OPTIONS] COMMAND [ARGS]...                                                                                                                          
                                                                                                                                                                        
 ╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --install-completion          Install completion for the current shell.                                                                                             │
 │ --show-completion             Show completion for the current shell, to copy it or customize the installation.                                                      │
```

### Comparing `dggstools-0.1.0/dggstools/__main__.py` & `dggstools-0.1.1/dggstools/__main__.py`

 * *Files identical despite different names*

### Comparing `dggstools-0.1.0/dggstools/auids/__init__.py` & `dggstools-0.1.1/dggstools/auids/__init__.py`

 * *Files identical despite different names*

### Comparing `dggstools-0.1.0/dggstools/auids/common.py` & `dggstools-0.1.1/dggstools/auids/common.py`

 * *Files identical despite different names*

### Comparing `dggstools-0.1.0/dggstools/auids/rhpx.py` & `dggstools-0.1.1/dggstools/auids/rhpx.py`

 * *Files identical despite different names*

### Comparing `dggstools-0.1.0/dggstools/rhpx/raster_to_rhpx.py` & `dggstools-0.1.1/dggstools/rhpx/raster_to_rhpx.py`

 * *Files identical despite different names*

### Comparing `dggstools-0.1.0/dggstools/rhpx/rhpx_gdf_helper.py` & `dggstools-0.1.1/dggstools/rhpx/rhpx_gdf_helper.py`

 * *Files identical despite different names*

### Comparing `dggstools-0.1.0/dggstools/rhpx/rhpxutils.py` & `dggstools-0.1.1/dggstools/rhpx/rhpxutils.py`

 * *Files identical despite different names*

### Comparing `dggstools-0.1.0/dggstools/rhpx/utils/rasterutils.py` & `dggstools-0.1.1/dggstools/rhpx/utils/rasterutils.py`

 * *Files identical despite different names*

### Comparing `dggstools-0.1.0/dggstools/rhpx/utils/storage.py` & `dggstools-0.1.1/dggstools/rhpx/utils/storage.py`

 * *Files identical despite different names*

### Comparing `dggstools-0.1.0/dggstools/rhpx/utils/utils.py` & `dggstools-0.1.1/dggstools/rhpx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dggstools-0.1.0/dggstools/rhpx/utils/vectorutils.py` & `dggstools-0.1.1/dggstools/rhpx/utils/vectorutils.py`

 * *Files identical despite different names*

### Comparing `dggstools-0.1.0/dggstools/rhpx/vector_to_rhpx.py` & `dggstools-0.1.1/dggstools/rhpx/vector_to_rhpx.py`

 * *Files identical despite different names*

### Comparing `dggstools-0.1.0/dggstools.egg-info/PKG-INFO` & `dggstools-0.1.1/dggstools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dggstools
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library and command line tool to manipulate raster and vector GIS data in a DGGS (rHEALPix for now).
 Author-email: Rubén Béjar <rbejar@unizar.es>, Sergio Martin-Segura <segura@unizar.es>, "Francisco J. Lopez-Pellicer" <fjlopez@unizar.es>, Javier Nogueras-Iso <jnog@unizar.es>, "F. Javier Zarazaga-Soria" <javy@unizar.es>
 Project-URL: Homepage, https://github.com/IAAA-Lab/dggstools
 Project-URL: Issues, https://github.com/IAAA-Lab/dggstools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -19,39 +19,39 @@
 Requires-Dist: botocore==1.34.37
 Requires-Dist: build==1.0.3
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: click==8.1.2
 Requires-Dist: click-plugins==1.1.1
 Requires-Dist: cligj==0.7.2
 Requires-Dist: cycler==0.11.0
-Requires-Dist: Fiona==1.9.4.post1
+Requires-Dist: fiona==1.9.6
 Requires-Dist: fonttools==4.48.1
 Requires-Dist: GeoAlchemy2==0.12.5
 Requires-Dist: geopandas==0.14.0
 Requires-Dist: jmespath==1.0.0
 Requires-Dist: kiwisolver==1.4.2
-Requires-Dist: matplotlib==3.7.2
+Requires-Dist: matplotlib==3.8.4
 Requires-Dist: munch==2.5.0
 Requires-Dist: networkx==2.8.7
 Requires-Dist: numpy==1.26.4
-Requires-Dist: packaging==21.3
-Requires-Dist: pandas==1.4.3
-Requires-Dist: Pillow==10.2.0
+Requires-Dist: packaging==24.0
+Requires-Dist: pandas==2.2.2
+Requires-Dist: pillow==10.2.0
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: pyarrow==15.0.0
 Requires-Dist: pyogrio==0.7.2
 Requires-Dist: pyparsing==3.0.7
 Requires-Dist: pyproj==3.6.1
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: pytz==2022.1
 Requires-Dist: rasterio==1.3.9
 Requires-Dist: rHEALPixDGGS==0.5.4
 Requires-Dist: s3transfer==0.10.0
 Requires-Dist: scipy==1.12.0
-Requires-Dist: shapely==2.0.1
+Requires-Dist: shapely==2.0.4
 Requires-Dist: six==1.16.0
 Requires-Dist: snuggs==1.4.7
 Requires-Dist: SQLAlchemy==2.0.21
 Requires-Dist: SQLAlchemy-Utils==0.41.1
 Requires-Dist: typer[all]==0.9.0
 Requires-Dist: urllib3==2.0.7
 
@@ -63,31 +63,36 @@
 a DGGS (rHEALPix for now).
 
 **Requirements**
 - Python 3.10 or higher
 - `pip` for installing Python packages
 
 ## Install the package and the command line tool
-1. You can download the latest package released on the GitHub Repository if you want the latest, non-stable version:
-
-Get the .whl file from <https://github.com/IAAA-Lab/dggstools/releases/latest>.
-
-2. Install the package and command line tool
+1. If you want the latest stable version (which is in PyPi):
 
 ```
-pip install ./name-of-the-file-you-have-downloaded.whl
+pip install dggstools
 ```
 
-3. Now you can run dggstools in the command line:
+2. If you prefer the latest non-stable version, you can download the latest package released on the GitHub Repository:
+
+ - Get the .whl file from <https://github.com/IAAA-Lab/dggstools/releases/latest>.
+ -  Install this wheel file:
+
+ ```
+ pip install ./name-of-the-file-you-have-downloaded.whl
+ ```
+
+3. In any case, once installed you can run dggstools in the command line:
 
 ```
 dggstools --help
 ```
 
-You will see something like this:
+And you will see something like this:
 
 ```
 Usage: dggstools [OPTIONS] COMMAND [ARGS]...                                                                                                                          
                                                                                                                                                                        
 ╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --install-completion          Install completion for the current shell.                                                                                             │
 │ --show-completion             Show completion for the current shell, to copy it or customize the installation.                                                      │
```

### Comparing `dggstools-0.1.0/dggstools.egg-info/SOURCES.txt` & `dggstools-0.1.1/dggstools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dggstools-0.1.0/dggstools.egg-info/requires.txt` & `dggstools-0.1.1/dggstools.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 botocore==1.34.37
 build==1.0.3
 certifi==2024.2.2
 click==8.1.2
 click-plugins==1.1.1
 cligj==0.7.2
 cycler==0.11.0
-Fiona==1.9.4.post1
+fiona==1.9.6
 fonttools==4.48.1
 GeoAlchemy2==0.12.5
 geopandas==0.14.0
 jmespath==1.0.0
 kiwisolver==1.4.2
-matplotlib==3.7.2
+matplotlib==3.8.4
 munch==2.5.0
 networkx==2.8.7
 numpy==1.26.4
-packaging==21.3
-pandas==1.4.3
-Pillow==10.2.0
+packaging==24.0
+pandas==2.2.2
+pillow==10.2.0
 psycopg2-binary==2.9.9
 pyarrow==15.0.0
 pyogrio==0.7.2
 pyparsing==3.0.7
 pyproj==3.6.1
 python-dateutil==2.8.2
 pytz==2022.1
 rasterio==1.3.9
 rHEALPixDGGS==0.5.4
 s3transfer==0.10.0
 scipy==1.12.0
-shapely==2.0.1
+shapely==2.0.4
 six==1.16.0
 snuggs==1.4.7
 SQLAlchemy==2.0.21
 SQLAlchemy-Utils==0.41.1
 typer[all]==0.9.0
 urllib3==2.0.7
```

### Comparing `dggstools-0.1.0/pyproject.toml` & `dggstools-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 requires = [
     "setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dggstools"
-version = "0.1.0"
+version = "0.1.1"
 dynamic = ["dependencies"]
 authors = [
   { name="Rubén Béjar", email="rbejar@unizar.es" },
   { name="Sergio Martin-Segura", email="segura@unizar.es" },
   { name="Francisco J. Lopez-Pellicer", email="fjlopez@unizar.es" },
   { name="Javier Nogueras-Iso", email="jnog@unizar.es" },
   { name="F. Javier Zarazaga-Soria", email="javy@unizar.es" },
```

### Comparing `dggstools-0.1.0/requirements.txt` & `dggstools-0.1.1/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 botocore==1.34.37
 build==1.0.3
 certifi==2024.2.2
 click==8.1.2
 click-plugins==1.1.1
 cligj==0.7.2
 cycler==0.11.0
-Fiona==1.9.4.post1
+fiona==1.9.6
 fonttools==4.48.1
 GeoAlchemy2==0.12.5
 geopandas==0.14.0
 jmespath==1.0.0
 kiwisolver==1.4.2
-matplotlib==3.7.2
+matplotlib==3.8.4
 munch==2.5.0
 networkx==2.8.7
 numpy==1.26.4
-packaging==21.3
-pandas==1.4.3
-Pillow==10.2.0
+packaging==24.0
+pandas==2.2.2
+pillow==10.2.0
 psycopg2-binary==2.9.9
 pyarrow==15.0.0
 pyogrio==0.7.2
 pyparsing==3.0.7
 pyproj==3.6.1
 python-dateutil==2.8.2
 pytz==2022.1
 rasterio==1.3.9
 rHEALPixDGGS==0.5.4
 s3transfer==0.10.0
 scipy==1.12.0
-shapely==2.0.1
+shapely==2.0.4
 six==1.16.0
 snuggs==1.4.7
 SQLAlchemy==2.0.21
 SQLAlchemy-Utils==0.41.1
 typer[all]==0.9.0
 urllib3==2.0.7
```

