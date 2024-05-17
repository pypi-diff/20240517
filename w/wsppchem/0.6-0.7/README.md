# Comparing `tmp/wsppchem-0.6.tar.gz` & `tmp/wsppchem-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsppchem-0.6.tar", last modified: Fri May 17 17:06:32 2024, max compression
+gzip compressed data, was "wsppchem-0.7.tar", last modified: Fri May 17 19:51:26 2024, max compression
```

## Comparing `wsppchem-0.6.tar` & `wsppchem-0.7.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:06:32.358621 wsppchem-0.6/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-17 17:05:59.000000 wsppchem-0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3874 2024-05-17 17:06:32.358621 wsppchem-0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3387 2024-05-17 17:05:59.000000 wsppchem-0.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 17:06:32.359621 wsppchem-0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      962 2024-05-17 17:05:59.000000 wsppchem-0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:06:32.349620 wsppchem-0.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:06:32.350621 wsppchem-0.6/src/wsppchem/
--rw-r--r--   0 root         (0) root         (0)     3701 2024-05-17 17:05:59.000000 wsppchem-0.6/src/wsppchem/Template.csv
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 17:05:59.000000 wsppchem-0.6/src/wsppchem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:06:32.357621 wsppchem-0.6/src/wsppchem/model_and_scaler/
--rw-r--r--   0 root         (0) root         (0)  3354127 2024-05-17 17:05:59.000000 wsppchem-0.6/src/wsppchem/model_and_scaler/LGBM_model.pkl
--rw-r--r--   0 root         (0) root         (0)    10174 2024-05-17 17:05:59.000000 wsppchem-0.6/src/wsppchem/model_and_scaler/LGBM_scaler.pkl
--rw-r--r--   0 root         (0) root         (0)     9982 2024-05-17 17:05:59.000000 wsppchem-0.6/src/wsppchem/wspp_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:06:32.351621 wsppchem-0.6/src/wsppchem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3874 2024-05-17 17:06:32.000000 wsppchem-0.6/src/wsppchem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-17 17:06:32.000000 wsppchem-0.6/src/wsppchem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 17:06:32.000000 wsppchem-0.6/src/wsppchem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-05-17 17:06:32.000000 wsppchem-0.6/src/wsppchem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-17 17:06:32.000000 wsppchem-0.6/src/wsppchem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:51:26.994191 wsppchem-0.7/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-17 19:51:11.000000 wsppchem-0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3875 2024-05-17 19:51:26.994191 wsppchem-0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3388 2024-05-17 19:51:11.000000 wsppchem-0.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 19:51:26.994191 wsppchem-0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      962 2024-05-17 19:51:11.000000 wsppchem-0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:51:26.988190 wsppchem-0.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:51:26.989190 wsppchem-0.7/src/wsppchem/
+-rw-r--r--   0 root         (0) root         (0)     3701 2024-05-17 19:51:11.000000 wsppchem-0.7/src/wsppchem/Template.csv
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 19:51:11.000000 wsppchem-0.7/src/wsppchem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:51:26.994191 wsppchem-0.7/src/wsppchem/model_and_scaler/
+-rw-r--r--   0 root         (0) root         (0)  3354127 2024-05-17 19:51:11.000000 wsppchem-0.7/src/wsppchem/model_and_scaler/LGBM_model.pkl
+-rw-r--r--   0 root         (0) root         (0)    10174 2024-05-17 19:51:11.000000 wsppchem-0.7/src/wsppchem/model_and_scaler/LGBM_scaler.pkl
+-rw-r--r--   0 root         (0) root         (0)     9982 2024-05-17 19:51:11.000000 wsppchem-0.7/src/wsppchem/wspp_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:51:26.990190 wsppchem-0.7/src/wsppchem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3875 2024-05-17 19:51:26.000000 wsppchem-0.7/src/wsppchem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-17 19:51:26.000000 wsppchem-0.7/src/wsppchem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 19:51:26.000000 wsppchem-0.7/src/wsppchem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-17 19:51:26.000000 wsppchem-0.7/src/wsppchem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-17 19:51:26.000000 wsppchem-0.7/src/wsppchem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 19:51:26.994191 wsppchem-0.7/tests/
+-rw-r--r--   0 root         (0) root         (0)     1432 2024-05-17 19:51:11.000000 wsppchem-0.7/tests/test_wspp_functions.py
```

### Comparing `wsppchem-0.6/LICENSE` & `wsppchem-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wsppchem-0.6/PKG-INFO` & `wsppchem-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsppchem
-Version: 0.6
+Version: 0.7
 Summary: Water Solubility Prediction Project
 Home-page: https://github.com/Nohalyan/WSPP_Projectppchem
 Author: Cossard Lucas and Enzo Venancio
 Author-email: lucas.cossard@epfl.ch and enzo.venancio@epfl.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -70,14 +70,15 @@
 ```
 
 2. Import all the functions using the following command.
 ```
 from wsppchem.wspp_functions import *
 ```
 3. Enjoy! 😁
+
 The two main functions of our package are `predict_logS_smiles` and `predict_logS_csv` which can be used in the following way:
 ```
 predict_logS_smiles(*smiles_codes)
 ```
 
 ```
 predict_logS_csv(csv_file_path)
```

### Comparing `wsppchem-0.6/README.md` & `wsppchem-0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 ```
 
 2. Import all the functions using the following command.
 ```
 from wsppchem.wspp_functions import *
 ```
 3. Enjoy! 😁
+
 The two main functions of our package are `predict_logS_smiles` and `predict_logS_csv` which can be used in the following way:
 ```
 predict_logS_smiles(*smiles_codes)
 ```
 
 ```
 predict_logS_csv(csv_file_path)
```

### Comparing `wsppchem-0.6/setup.py` & `wsppchem-0.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
     name="wsppchem",
-    version="0.6",
+    version="0.7",
     author="Cossard Lucas and Enzo Venancio",
     author_email="lucas.cossard@epfl.ch and enzo.venancio@epfl.ch",
     description="Water Solubility Prediction Project",
     long_description=open('README.md').read() if os.path.exists('README.md') else '',
     long_description_content_type="text/markdown",
     url="https://github.com/Nohalyan/WSPP_Projectppchem",
     packages=find_packages(where='src'),
```

### Comparing `wsppchem-0.6/src/wsppchem/Template.csv` & `wsppchem-0.7/src/wsppchem/Template.csv`

 * *Files identical despite different names*

### Comparing `wsppchem-0.6/src/wsppchem/model_and_scaler/LGBM_model.pkl` & `wsppchem-0.7/src/wsppchem/model_and_scaler/LGBM_model.pkl`

 * *Files identical despite different names*

### Comparing `wsppchem-0.6/src/wsppchem/model_and_scaler/LGBM_scaler.pkl` & `wsppchem-0.7/src/wsppchem/model_and_scaler/LGBM_scaler.pkl`

 * *Files identical despite different names*

### Comparing `wsppchem-0.6/src/wsppchem/wspp_functions.py` & `wsppchem-0.7/src/wsppchem/wspp_functions.py`

 * *Files identical despite different names*

### Comparing `wsppchem-0.6/src/wsppchem.egg-info/PKG-INFO` & `wsppchem-0.7/src/wsppchem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsppchem
-Version: 0.6
+Version: 0.7
 Summary: Water Solubility Prediction Project
 Home-page: https://github.com/Nohalyan/WSPP_Projectppchem
 Author: Cossard Lucas and Enzo Venancio
 Author-email: lucas.cossard@epfl.ch and enzo.venancio@epfl.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -70,14 +70,15 @@
 ```
 
 2. Import all the functions using the following command.
 ```
 from wsppchem.wspp_functions import *
 ```
 3. Enjoy! 😁
+
 The two main functions of our package are `predict_logS_smiles` and `predict_logS_csv` which can be used in the following way:
 ```
 predict_logS_smiles(*smiles_codes)
 ```
 
 ```
 predict_logS_csv(csv_file_path)
```

