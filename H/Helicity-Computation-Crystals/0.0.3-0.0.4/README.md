# Comparing `tmp/helicity_computation_crystals-0.0.3.tar.gz` & `tmp/helicity_computation_crystals-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helicity_computation_crystals-0.0.3.tar", last modified: Fri May 17 13:35:31 2024, max compression
+gzip compressed data, was "helicity_computation_crystals-0.0.4.tar", last modified: Fri May 17 13:38:55 2024, max compression
```

## Comparing `helicity_computation_crystals-0.0.3.tar` & `helicity_computation_crystals-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:35:31.334504 helicity_computation_crystals-0.0.3/
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:35:31.330505 helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:35:31.330505 helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/
--rw-r--r--   0 fernando  (1000) fernando  (1000)     2732 2024-05-17 13:35:31.000000 helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/PKG-INFO
--rw-rw-r--   0 fernando  (1000) fernando  (1000)      532 2024-05-17 13:35:31.000000 helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/SOURCES.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)        1 2024-05-17 13:35:31.000000 helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/dependency_links.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)       76 2024-05-17 13:35:31.000000 helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/entry_points.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)      135 2024-05-17 13:35:31.000000 helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/requires.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)        1 2024-05-17 13:35:31.000000 helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/top_level.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)    35149 2024-05-17 10:45:38.000000 helicity_computation_crystals-0.0.3/LICENSE
--rw-r--r--   0 fernando  (1000) fernando  (1000)     2732 2024-05-17 13:35:31.334504 helicity_computation_crystals-0.0.3/PKG-INFO
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     1362 2024-05-17 10:45:38.000000 helicity_computation_crystals-0.0.3/README.md
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     1629 2024-05-17 13:35:21.000000 helicity_computation_crystals-0.0.3/pyproject.toml
--rw-rw-r--   0 fernando  (1000) fernando  (1000)       38 2024-05-17 13:35:31.334504 helicity_computation_crystals-0.0.3/setup.cfg
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:38:55.538416 helicity_computation_crystals-0.0.4/
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)    35149 2024-05-17 10:45:38.000000 helicity_computation_crystals-0.0.4/LICENSE
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     2732 2024-05-17 13:38:55.538416 helicity_computation_crystals-0.0.4/PKG-INFO
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     1362 2024-05-17 10:45:38.000000 helicity_computation_crystals-0.0.4/README.md
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     1603 2024-05-17 13:38:48.000000 helicity_computation_crystals-0.0.4/pyproject.toml
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)       38 2024-05-17 13:38:55.538416 helicity_computation_crystals-0.0.4/setup.cfg
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:38:55.534416 helicity_computation_crystals-0.0.4/src/
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:38:55.534416 helicity_computation_crystals-0.0.4/src/Helicity_Computation_Crystals.egg-info/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     2732 2024-05-17 13:38:55.000000 helicity_computation_crystals-0.0.4/src/Helicity_Computation_Crystals.egg-info/PKG-INFO
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)      376 2024-05-17 13:38:55.000000 helicity_computation_crystals-0.0.4/src/Helicity_Computation_Crystals.egg-info/SOURCES.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)        1 2024-05-17 13:38:55.000000 helicity_computation_crystals-0.0.4/src/Helicity_Computation_Crystals.egg-info/dependency_links.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)       76 2024-05-17 13:38:55.000000 helicity_computation_crystals-0.0.4/src/Helicity_Computation_Crystals.egg-info/entry_points.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)      135 2024-05-17 13:38:55.000000 helicity_computation_crystals-0.0.4/src/Helicity_Computation_Crystals.egg-info/requires.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)        1 2024-05-17 13:38:55.000000 helicity_computation_crystals-0.0.4/src/Helicity_Computation_Crystals.egg-info/top_level.txt
```

### Comparing `helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/PKG-INFO` & `helicity_computation_crystals-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Helicity_Computation_Crystals
-Version: 0.0.3
+Version: 0.0.4
 Summary: A script for the computation of handedness in crystalline structures.
 Author-email: "F. Gómez-ortiz" <fgomez@uliege.be>
 License: GPL-3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `helicity_computation_crystals-0.0.3/LICENSE` & `helicity_computation_crystals-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `helicity_computation_crystals-0.0.3/PKG-INFO` & `helicity_computation_crystals-0.0.4/src/Helicity_Computation_Crystals.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Helicity_Computation_Crystals
-Version: 0.0.3
+Version: 0.0.4
 Summary: A script for the computation of handedness in crystalline structures.
 Author-email: "F. Gómez-ortiz" <fgomez@uliege.be>
 License: GPL-3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `helicity_computation_crystals-0.0.3/README.md` & `helicity_computation_crystals-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `helicity_computation_crystals-0.0.3/pyproject.toml` & `helicity_computation_crystals-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Helicity_Computation_Crystals"
-version = "0.0.3"
+version = "0.0.4"
 description = "A script for the computation of handedness in crystalline structures."
 authors = [
     {name = "F. Gómez-ortiz", email = "fgomez@uliege.be"},
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 license = {text = "GPL-3"}
@@ -37,15 +37,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 
 [tool.setuptools.packages.find]
-where = ["Helicity_Computation_Crystals"]
+where = ["src"]
 
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project.scripts]
 helicity_computation = "Helicity_Computation_Crystals:main"
```

