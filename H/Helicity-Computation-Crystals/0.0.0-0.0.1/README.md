# Comparing `tmp/helicity_computation_crystals-0.0.0.tar.gz` & `tmp/helicity_computation_crystals-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helicity_computation_crystals-0.0.0.tar", last modified: Fri May 17 13:10:20 2024, max compression
+gzip compressed data, was "helicity_computation_crystals-0.0.1.tar", last modified: Fri May 17 13:18:08 2024, max compression
```

## Comparing `helicity_computation_crystals-0.0.0.tar` & `helicity_computation_crystals-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:10:20.812564 helicity_computation_crystals-0.0.0/
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:10:20.808564 helicity_computation_crystals-0.0.0/Helicity_Computation_Crystals/
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:10:20.812564 helicity_computation_crystals-0.0.0/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/
--rw-r--r--   0 fernando  (1000) fernando  (1000)     2784 2024-05-17 13:10:20.000000 helicity_computation_crystals-0.0.0/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/PKG-INFO
--rw-rw-r--   0 fernando  (1000) fernando  (1000)      446 2024-05-17 13:10:20.000000 helicity_computation_crystals-0.0.0/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/SOURCES.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)        1 2024-05-17 13:10:20.000000 helicity_computation_crystals-0.0.0/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/dependency_links.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)      157 2024-05-17 13:10:20.000000 helicity_computation_crystals-0.0.0/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/requires.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)        1 2024-05-17 13:10:20.000000 helicity_computation_crystals-0.0.0/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/top_level.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)    35149 2024-05-17 10:45:38.000000 helicity_computation_crystals-0.0.0/LICENSE
--rw-r--r--   0 fernando  (1000) fernando  (1000)     2784 2024-05-17 13:10:20.812564 helicity_computation_crystals-0.0.0/PKG-INFO
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     1362 2024-05-17 10:45:38.000000 helicity_computation_crystals-0.0.0/README.md
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     1589 2024-05-17 13:10:07.000000 helicity_computation_crystals-0.0.0/pyproject.toml
--rw-rw-r--   0 fernando  (1000) fernando  (1000)       38 2024-05-17 13:10:20.812564 helicity_computation_crystals-0.0.0/setup.cfg
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:18:08.895507 helicity_computation_crystals-0.0.1/
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:18:08.895507 helicity_computation_crystals-0.0.1/Helicity_Computation_Crystals/
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:18:08.895507 helicity_computation_crystals-0.0.1/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     2732 2024-05-17 13:18:08.000000 helicity_computation_crystals-0.0.1/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/PKG-INFO
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)      446 2024-05-17 13:18:08.000000 helicity_computation_crystals-0.0.1/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/SOURCES.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)        1 2024-05-17 13:18:08.000000 helicity_computation_crystals-0.0.1/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/dependency_links.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)      135 2024-05-17 13:18:08.000000 helicity_computation_crystals-0.0.1/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/requires.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)        1 2024-05-17 13:18:08.000000 helicity_computation_crystals-0.0.1/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/top_level.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)    35149 2024-05-17 10:45:38.000000 helicity_computation_crystals-0.0.1/LICENSE
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     2732 2024-05-17 13:18:08.895507 helicity_computation_crystals-0.0.1/PKG-INFO
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     1362 2024-05-17 10:45:38.000000 helicity_computation_crystals-0.0.1/README.md
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     1552 2024-05-17 13:17:59.000000 helicity_computation_crystals-0.0.1/pyproject.toml
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)       38 2024-05-17 13:18:08.895507 helicity_computation_crystals-0.0.1/setup.cfg
```

### Comparing `helicity_computation_crystals-0.0.0/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/PKG-INFO` & `helicity_computation_crystals-0.0.1/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Helicity_Computation_Crystals
-Version: 0.0.0
+Version: 0.0.1
 Summary: A script for the computation of handedness in crystalline structures.
 Author-email: "F. Gómez-ortiz" <fgomez@uliege.be>
 License: GPL-3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
@@ -19,17 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: scipy>=1.7.0
-Requires-Dist: sisl>=0.9.0
 Requires-Dist: matplotlib>=3.4.0
-Requires-Dist: ase>=3.19
 Provides-Extra: test
 Requires-Dist: pytest>=6.2.0; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pytest>=6.2.0; extra == "dev"
 Requires-Dist: black>=21.6b0; extra == "dev"
 Requires-Dist: pre-commit>=2.13.0; extra == "dev"
 Requires-Dist: sphinx>=4.1.2; extra == "dev"
```

### Comparing `helicity_computation_crystals-0.0.0/LICENSE` & `helicity_computation_crystals-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `helicity_computation_crystals-0.0.0/PKG-INFO` & `helicity_computation_crystals-0.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Helicity_Computation_Crystals
-Version: 0.0.0
+Version: 0.0.1
 Summary: A script for the computation of handedness in crystalline structures.
 Author-email: "F. Gómez-ortiz" <fgomez@uliege.be>
 License: GPL-3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
@@ -19,17 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: scipy>=1.7.0
-Requires-Dist: sisl>=0.9.0
 Requires-Dist: matplotlib>=3.4.0
-Requires-Dist: ase>=3.19
 Provides-Extra: test
 Requires-Dist: pytest>=6.2.0; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pytest>=6.2.0; extra == "dev"
 Requires-Dist: black>=21.6b0; extra == "dev"
 Requires-Dist: pre-commit>=2.13.0; extra == "dev"
 Requires-Dist: sphinx>=4.1.2; extra == "dev"
```

### Comparing `helicity_computation_crystals-0.0.0/README.md` & `helicity_computation_crystals-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `helicity_computation_crystals-0.0.0/pyproject.toml` & `helicity_computation_crystals-0.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 [project]
 name = "Helicity_Computation_Crystals"
-version = "0.0.0"
+version = "0.0.1"
 description = "A script for the computation of handedness in crystalline structures."
 authors = [
     {name = "F. Gómez-ortiz", email = "fgomez@uliege.be"},
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 license = {text = "GPL-3"}
 dependencies = [
     "numpy>=1.21.0",
     "scipy>=1.7.0",
-    "sisl>=0.9.0",
-    "matplotlib>=3.4.0",
-    "ase>=3.19",
+    "matplotlib>=3.4.0"
 ]
 #scripts = []
 	
 classifiers = [
   # How mature is this project? Common values are
   #   3 - Alpha
   #   4 - Beta
```

