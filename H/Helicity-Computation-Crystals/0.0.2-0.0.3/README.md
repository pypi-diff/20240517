# Comparing `tmp/helicity_computation_crystals-0.0.2.tar.gz` & `tmp/helicity_computation_crystals-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helicity_computation_crystals-0.0.2.tar", last modified: Fri May 17 13:27:49 2024, max compression
+gzip compressed data, was "helicity_computation_crystals-0.0.3.tar", last modified: Fri May 17 13:35:31 2024, max compression
```

## Comparing `helicity_computation_crystals-0.0.2.tar` & `helicity_computation_crystals-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:27:49.214582 helicity_computation_crystals-0.0.2/
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:27:49.210582 helicity_computation_crystals-0.0.2/Helicity_Computation_Crystals/
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:27:49.214582 helicity_computation_crystals-0.0.2/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/
--rw-r--r--   0 fernando  (1000) fernando  (1000)     2732 2024-05-17 13:27:49.000000 helicity_computation_crystals-0.0.2/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/PKG-INFO
--rw-rw-r--   0 fernando  (1000) fernando  (1000)      532 2024-05-17 13:27:49.000000 helicity_computation_crystals-0.0.2/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/SOURCES.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)        1 2024-05-17 13:27:49.000000 helicity_computation_crystals-0.0.2/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/dependency_links.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)       76 2024-05-17 13:27:49.000000 helicity_computation_crystals-0.0.2/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/entry_points.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)      135 2024-05-17 13:27:49.000000 helicity_computation_crystals-0.0.2/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/requires.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)        1 2024-05-17 13:27:49.000000 helicity_computation_crystals-0.0.2/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/top_level.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)    35149 2024-05-17 10:45:38.000000 helicity_computation_crystals-0.0.2/LICENSE
--rw-r--r--   0 fernando  (1000) fernando  (1000)     2732 2024-05-17 13:27:49.214582 helicity_computation_crystals-0.0.2/PKG-INFO
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     1362 2024-05-17 10:45:38.000000 helicity_computation_crystals-0.0.2/README.md
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     1629 2024-05-17 13:27:39.000000 helicity_computation_crystals-0.0.2/pyproject.toml
--rw-rw-r--   0 fernando  (1000) fernando  (1000)       38 2024-05-17 13:27:49.214582 helicity_computation_crystals-0.0.2/setup.cfg
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:35:31.334504 helicity_computation_crystals-0.0.3/
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:35:31.330505 helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-17 13:35:31.330505 helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     2732 2024-05-17 13:35:31.000000 helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/PKG-INFO
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)      532 2024-05-17 13:35:31.000000 helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/SOURCES.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)        1 2024-05-17 13:35:31.000000 helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/dependency_links.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)       76 2024-05-17 13:35:31.000000 helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/entry_points.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)      135 2024-05-17 13:35:31.000000 helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/requires.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)        1 2024-05-17 13:35:31.000000 helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/top_level.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)    35149 2024-05-17 10:45:38.000000 helicity_computation_crystals-0.0.3/LICENSE
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     2732 2024-05-17 13:35:31.334504 helicity_computation_crystals-0.0.3/PKG-INFO
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     1362 2024-05-17 10:45:38.000000 helicity_computation_crystals-0.0.3/README.md
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     1629 2024-05-17 13:35:21.000000 helicity_computation_crystals-0.0.3/pyproject.toml
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)       38 2024-05-17 13:35:31.334504 helicity_computation_crystals-0.0.3/setup.cfg
```

### Comparing `helicity_computation_crystals-0.0.2/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/PKG-INFO` & `helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Helicity_Computation_Crystals
-Version: 0.0.2
+Version: 0.0.3
 Summary: A script for the computation of handedness in crystalline structures.
 Author-email: "F. Gómez-ortiz" <fgomez@uliege.be>
 License: GPL-3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `helicity_computation_crystals-0.0.2/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/SOURCES.txt` & `helicity_computation_crystals-0.0.3/Helicity_Computation_Crystals/Helicity_Computation_Crystals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helicity_computation_crystals-0.0.2/LICENSE` & `helicity_computation_crystals-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `helicity_computation_crystals-0.0.2/PKG-INFO` & `helicity_computation_crystals-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Helicity_Computation_Crystals
-Version: 0.0.2
+Version: 0.0.3
 Summary: A script for the computation of handedness in crystalline structures.
 Author-email: "F. Gómez-ortiz" <fgomez@uliege.be>
 License: GPL-3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `helicity_computation_crystals-0.0.2/README.md` & `helicity_computation_crystals-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `helicity_computation_crystals-0.0.2/pyproject.toml` & `helicity_computation_crystals-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Helicity_Computation_Crystals"
-version = "0.0.2"
+version = "0.0.3"
 description = "A script for the computation of handedness in crystalline structures."
 authors = [
     {name = "F. Gómez-ortiz", email = "fgomez@uliege.be"},
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 license = {text = "GPL-3"}
```

