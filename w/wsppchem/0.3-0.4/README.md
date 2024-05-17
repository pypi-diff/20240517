# Comparing `tmp/wsppchem-0.3.tar.gz` & `tmp/wsppchem-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsppchem-0.3.tar", last modified: Fri May 17 16:01:46 2024, max compression
+gzip compressed data, was "wsppchem-0.4.tar", last modified: Fri May 17 16:13:02 2024, max compression
```

## Comparing `wsppchem-0.3.tar` & `wsppchem-0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:01:46.212942 wsppchem-0.3/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-17 16:01:17.000000 wsppchem-0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4643 2024-05-17 16:01:46.211942 wsppchem-0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4156 2024-05-17 16:01:17.000000 wsppchem-0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 16:01:46.212942 wsppchem-0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      962 2024-05-17 16:01:17.000000 wsppchem-0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:01:46.197940 wsppchem-0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:01:46.202941 wsppchem-0.3/src/wsppchem/
--rw-r--r--   0 root         (0) root         (0)     3701 2024-05-17 16:01:17.000000 wsppchem-0.3/src/wsppchem/Template.csv
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 16:01:17.000000 wsppchem-0.3/src/wsppchem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:01:46.211942 wsppchem-0.3/src/wsppchem/model_and_scaler/
--rw-r--r--   0 root         (0) root         (0)  3354127 2024-05-17 16:01:17.000000 wsppchem-0.3/src/wsppchem/model_and_scaler/LGBM_model.pkl
--rw-r--r--   0 root         (0) root         (0)    10174 2024-05-17 16:01:17.000000 wsppchem-0.3/src/wsppchem/model_and_scaler/LGBM_scaler.pkl
--rw-r--r--   0 root         (0) root         (0)     9459 2024-05-17 16:01:17.000000 wsppchem-0.3/src/wsppchem/wspp_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:01:46.203941 wsppchem-0.3/src/wsppchem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4643 2024-05-17 16:01:45.000000 wsppchem-0.3/src/wsppchem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-17 16:01:46.000000 wsppchem-0.3/src/wsppchem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 16:01:45.000000 wsppchem-0.3/src/wsppchem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-05-17 16:01:45.000000 wsppchem-0.3/src/wsppchem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-17 16:01:45.000000 wsppchem-0.3/src/wsppchem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:13:02.438968 wsppchem-0.4/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-17 16:12:32.000000 wsppchem-0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4643 2024-05-17 16:13:02.438968 wsppchem-0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4156 2024-05-17 16:12:32.000000 wsppchem-0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 16:13:02.438968 wsppchem-0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      962 2024-05-17 16:12:32.000000 wsppchem-0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:13:02.430967 wsppchem-0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:13:02.432967 wsppchem-0.4/src/wsppchem/
+-rw-r--r--   0 root         (0) root         (0)     3701 2024-05-17 16:12:32.000000 wsppchem-0.4/src/wsppchem/Template.csv
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 16:12:32.000000 wsppchem-0.4/src/wsppchem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:13:02.438968 wsppchem-0.4/src/wsppchem/model_and_scaler/
+-rw-r--r--   0 root         (0) root         (0)  3354127 2024-05-17 16:12:32.000000 wsppchem-0.4/src/wsppchem/model_and_scaler/LGBM_model.pkl
+-rw-r--r--   0 root         (0) root         (0)    10174 2024-05-17 16:12:32.000000 wsppchem-0.4/src/wsppchem/model_and_scaler/LGBM_scaler.pkl
+-rw-r--r--   0 root         (0) root         (0)     9452 2024-05-17 16:12:32.000000 wsppchem-0.4/src/wsppchem/wspp_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:13:02.433967 wsppchem-0.4/src/wsppchem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4643 2024-05-17 16:13:02.000000 wsppchem-0.4/src/wsppchem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-17 16:13:02.000000 wsppchem-0.4/src/wsppchem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 16:13:02.000000 wsppchem-0.4/src/wsppchem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-17 16:13:02.000000 wsppchem-0.4/src/wsppchem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-17 16:13:02.000000 wsppchem-0.4/src/wsppchem.egg-info/top_level.txt
```

### Comparing `wsppchem-0.3/LICENSE` & `wsppchem-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wsppchem-0.3/PKG-INFO` & `wsppchem-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsppchem
-Version: 0.3
+Version: 0.4
 Summary: Water Solubility Prediction Project
 Home-page: https://github.com/Nohalyan/WSPP_Projectppchem
 Author: Cossard Lucas and Enzo Venancio
 Author-email: lucas.cossard@epfl.ch and enzo.venancio@epfl.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wsppchem-0.3/README.md` & `wsppchem-0.4/README.md`

 * *Files identical despite different names*

### Comparing `wsppchem-0.3/setup.py` & `wsppchem-0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
     name="wsppchem",
-    version="0.3",
+    version="0.4",
     author="Cossard Lucas and Enzo Venancio",
     author_email="lucas.cossard@epfl.ch and enzo.venancio@epfl.ch",
     description="Water Solubility Prediction Project",
     long_description=open('README.md').read() if os.path.exists('README.md') else '',
     long_description_content_type="text/markdown",
     url="https://github.com/Nohalyan/WSPP_Projectppchem",
     packages=find_packages(where='src'),
```

### Comparing `wsppchem-0.3/src/wsppchem/Template.csv` & `wsppchem-0.4/src/wsppchem/Template.csv`

 * *Files identical despite different names*

### Comparing `wsppchem-0.3/src/wsppchem/model_and_scaler/LGBM_model.pkl` & `wsppchem-0.4/src/wsppchem/model_and_scaler/LGBM_model.pkl`

 * *Files identical despite different names*

### Comparing `wsppchem-0.3/src/wsppchem/model_and_scaler/LGBM_scaler.pkl` & `wsppchem-0.4/src/wsppchem/model_and_scaler/LGBM_scaler.pkl`

 * *Files identical despite different names*

### Comparing `wsppchem-0.3/src/wsppchem/wspp_functions.py` & `wsppchem-0.4/src/wsppchem/wspp_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     
     Description: Predicts the LogS value for one or more  SMILES.
     Usage: Provide one or more valid SMILES codes in a string as input
     Example: predict_logS_smiles("CC(=O)NC1=CC=C(C=C1)O","CN1C=NC2=C1C(=O)N(C(=O)N2C)C")
     
     ==========================================================================================================================================
     
-    print("predict_logS_csv(csv_file_path):
+    predict_logS_csv(csv_file_path):
     
     Description: Predicts LogS values for SMILES codes stored in a CSV file
     Usage: Provide the path to a CSV file containing SMILES codes in the 'SMILE' column (see Template.csv for an example of a valid csv file)
     Example: predict_logS_csv("/content/WSPP_Projectppchem/src/WSPP/Template.csv")
 
     ==========================================================================================================================================
     """
```

### Comparing `wsppchem-0.3/src/wsppchem.egg-info/PKG-INFO` & `wsppchem-0.4/src/wsppchem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsppchem
-Version: 0.3
+Version: 0.4
 Summary: Water Solubility Prediction Project
 Home-page: https://github.com/Nohalyan/WSPP_Projectppchem
 Author: Cossard Lucas and Enzo Venancio
 Author-email: lucas.cossard@epfl.ch and enzo.venancio@epfl.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

