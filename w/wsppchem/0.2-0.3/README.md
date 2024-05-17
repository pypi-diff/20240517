# Comparing `tmp/wsppchem-0.2.tar.gz` & `tmp/wsppchem-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsppchem-0.2.tar", last modified: Fri May 17 15:48:48 2024, max compression
+gzip compressed data, was "wsppchem-0.3.tar", last modified: Fri May 17 16:01:46 2024, max compression
```

## Comparing `wsppchem-0.2.tar` & `wsppchem-0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:48:48.405505 wsppchem-0.2/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-17 15:48:14.000000 wsppchem-0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4643 2024-05-17 15:48:48.405505 wsppchem-0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4156 2024-05-17 15:48:14.000000 wsppchem-0.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 15:48:48.406504 wsppchem-0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      946 2024-05-17 15:48:14.000000 wsppchem-0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:48:48.396504 wsppchem-0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:48:48.397504 wsppchem-0.2/src/wsppchem/
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 15:48:14.000000 wsppchem-0.2/src/wsppchem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:48:48.405505 wsppchem-0.2/src/wsppchem/model_and_scaler/
--rw-r--r--   0 root         (0) root         (0)  3354127 2024-05-17 15:48:15.000000 wsppchem-0.2/src/wsppchem/model_and_scaler/LGBM_model.pkl
--rw-r--r--   0 root         (0) root         (0)    10174 2024-05-17 15:48:15.000000 wsppchem-0.2/src/wsppchem/model_and_scaler/LGBM_scaler.pkl
--rw-r--r--   0 root         (0) root         (0)     9138 2024-05-17 15:48:15.000000 wsppchem-0.2/src/wsppchem/wspp_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:48:48.399504 wsppchem-0.2/src/wsppchem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4643 2024-05-17 15:48:48.000000 wsppchem-0.2/src/wsppchem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      352 2024-05-17 15:48:48.000000 wsppchem-0.2/src/wsppchem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 15:48:48.000000 wsppchem-0.2/src/wsppchem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-05-17 15:48:48.000000 wsppchem-0.2/src/wsppchem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-17 15:48:48.000000 wsppchem-0.2/src/wsppchem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:01:46.212942 wsppchem-0.3/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-17 16:01:17.000000 wsppchem-0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4643 2024-05-17 16:01:46.211942 wsppchem-0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4156 2024-05-17 16:01:17.000000 wsppchem-0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 16:01:46.212942 wsppchem-0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      962 2024-05-17 16:01:17.000000 wsppchem-0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:01:46.197940 wsppchem-0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:01:46.202941 wsppchem-0.3/src/wsppchem/
+-rw-r--r--   0 root         (0) root         (0)     3701 2024-05-17 16:01:17.000000 wsppchem-0.3/src/wsppchem/Template.csv
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 16:01:17.000000 wsppchem-0.3/src/wsppchem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:01:46.211942 wsppchem-0.3/src/wsppchem/model_and_scaler/
+-rw-r--r--   0 root         (0) root         (0)  3354127 2024-05-17 16:01:17.000000 wsppchem-0.3/src/wsppchem/model_and_scaler/LGBM_model.pkl
+-rw-r--r--   0 root         (0) root         (0)    10174 2024-05-17 16:01:17.000000 wsppchem-0.3/src/wsppchem/model_and_scaler/LGBM_scaler.pkl
+-rw-r--r--   0 root         (0) root         (0)     9459 2024-05-17 16:01:17.000000 wsppchem-0.3/src/wsppchem/wspp_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:01:46.203941 wsppchem-0.3/src/wsppchem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4643 2024-05-17 16:01:45.000000 wsppchem-0.3/src/wsppchem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-17 16:01:46.000000 wsppchem-0.3/src/wsppchem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 16:01:45.000000 wsppchem-0.3/src/wsppchem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-17 16:01:45.000000 wsppchem-0.3/src/wsppchem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-17 16:01:45.000000 wsppchem-0.3/src/wsppchem.egg-info/top_level.txt
```

### Comparing `wsppchem-0.2/LICENSE` & `wsppchem-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wsppchem-0.2/PKG-INFO` & `wsppchem-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsppchem
-Version: 0.2
+Version: 0.3
 Summary: Water Solubility Prediction Project
 Home-page: https://github.com/Nohalyan/WSPP_Projectppchem
 Author: Cossard Lucas and Enzo Venancio
 Author-email: lucas.cossard@epfl.ch and enzo.venancio@epfl.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wsppchem-0.2/README.md` & `wsppchem-0.3/README.md`

 * *Files identical despite different names*

### Comparing `wsppchem-0.2/setup.py` & `wsppchem-0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
     name="wsppchem",
-    version="0.2",
+    version="0.3",
     author="Cossard Lucas and Enzo Venancio",
     author_email="lucas.cossard@epfl.ch and enzo.venancio@epfl.ch",
     description="Water Solubility Prediction Project",
     long_description=open('README.md').read() if os.path.exists('README.md') else '',
     long_description_content_type="text/markdown",
     url="https://github.com/Nohalyan/WSPP_Projectppchem",
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     package_data={
-        'wsppchem': ['model_and_scaler/*.pkl'],
+        'wsppchem': ['model_and_scaler/*.pkl', 'Template.csv'],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
```

### Comparing `wsppchem-0.2/src/wsppchem/model_and_scaler/LGBM_model.pkl` & `wsppchem-0.3/src/wsppchem/model_and_scaler/LGBM_model.pkl`

 * *Files identical despite different names*

### Comparing `wsppchem-0.2/src/wsppchem/model_and_scaler/LGBM_scaler.pkl` & `wsppchem-0.3/src/wsppchem/model_and_scaler/LGBM_scaler.pkl`

 * *Files identical despite different names*

### Comparing `wsppchem-0.2/src/wsppchem/wspp_functions.py` & `wsppchem-0.3/src/wsppchem/wspp_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,25 +202,31 @@
     print("\nLogS Values:")
     for smiles_code, logS in logS_values.items():
         print(f"The predicted logS value for {smiles_code} is: {logS} mol/L")
     print_ascii_art()
 
 
 
-def predict_logS_csv(csv_file_path):
+def predict_logS_csv(csv_file_path=None):
     """
     Predicts LogS values for SMILES codes stored in a CSV file and saves the predictions to a new CSV file.
 
     Parameters:
-    csv_file_path (str): Path to the CSV file containing SMILES codes in the 'SMILE' column.
+    csv_file_path (str, optional): Path to the CSV file containing SMILES codes in the 'SMILE' column. 
+                                   If not provided, uses the default 'Template.csv'.
 
     Returns:
-    A new CSV file named with '_predicted.csv' at the end containing the SMILES code and thei predicted LogS values.
+    A new CSV file named with '_predicted.csv' at the end containing the SMILES code and their predicted LogS values.
     """
- 
+
+    # Use the default template if no csv_file_path is provided
+    if csv_file_path is None:
+        with pkg_resources.path('wsppchem', 'Template.csv') as default_csv_path:
+            csv_file_path = default_csv_path
+
     # Read the CSV file into a DataFrame
     try:
         df = pd.read_csv(csv_file_path)
     except FileNotFoundError:
         print(f"File {csv_file_path} not found.")
         return
```

### Comparing `wsppchem-0.2/src/wsppchem.egg-info/PKG-INFO` & `wsppchem-0.3/src/wsppchem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsppchem
-Version: 0.2
+Version: 0.3
 Summary: Water Solubility Prediction Project
 Home-page: https://github.com/Nohalyan/WSPP_Projectppchem
 Author: Cossard Lucas and Enzo Venancio
 Author-email: lucas.cossard@epfl.ch and enzo.venancio@epfl.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

