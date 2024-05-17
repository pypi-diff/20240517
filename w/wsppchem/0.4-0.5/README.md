# Comparing `tmp/wsppchem-0.4.tar.gz` & `tmp/wsppchem-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsppchem-0.4.tar", last modified: Fri May 17 16:13:02 2024, max compression
+gzip compressed data, was "wsppchem-0.5.tar", last modified: Fri May 17 16:19:50 2024, max compression
```

## Comparing `wsppchem-0.4.tar` & `wsppchem-0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:13:02.438968 wsppchem-0.4/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-17 16:12:32.000000 wsppchem-0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4643 2024-05-17 16:13:02.438968 wsppchem-0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4156 2024-05-17 16:12:32.000000 wsppchem-0.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 16:13:02.438968 wsppchem-0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      962 2024-05-17 16:12:32.000000 wsppchem-0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:13:02.430967 wsppchem-0.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:13:02.432967 wsppchem-0.4/src/wsppchem/
--rw-r--r--   0 root         (0) root         (0)     3701 2024-05-17 16:12:32.000000 wsppchem-0.4/src/wsppchem/Template.csv
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 16:12:32.000000 wsppchem-0.4/src/wsppchem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:13:02.438968 wsppchem-0.4/src/wsppchem/model_and_scaler/
--rw-r--r--   0 root         (0) root         (0)  3354127 2024-05-17 16:12:32.000000 wsppchem-0.4/src/wsppchem/model_and_scaler/LGBM_model.pkl
--rw-r--r--   0 root         (0) root         (0)    10174 2024-05-17 16:12:32.000000 wsppchem-0.4/src/wsppchem/model_and_scaler/LGBM_scaler.pkl
--rw-r--r--   0 root         (0) root         (0)     9452 2024-05-17 16:12:32.000000 wsppchem-0.4/src/wsppchem/wspp_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:13:02.433967 wsppchem-0.4/src/wsppchem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4643 2024-05-17 16:13:02.000000 wsppchem-0.4/src/wsppchem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-17 16:13:02.000000 wsppchem-0.4/src/wsppchem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 16:13:02.000000 wsppchem-0.4/src/wsppchem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-05-17 16:13:02.000000 wsppchem-0.4/src/wsppchem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-17 16:13:02.000000 wsppchem-0.4/src/wsppchem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:19:50.029486 wsppchem-0.5/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-17 16:19:19.000000 wsppchem-0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4643 2024-05-17 16:19:50.029486 wsppchem-0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4156 2024-05-17 16:19:19.000000 wsppchem-0.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 16:19:50.029486 wsppchem-0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      962 2024-05-17 16:19:19.000000 wsppchem-0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:19:50.013485 wsppchem-0.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:19:50.015485 wsppchem-0.5/src/wsppchem/
+-rw-r--r--   0 root         (0) root         (0)     3701 2024-05-17 16:19:19.000000 wsppchem-0.5/src/wsppchem/Template.csv
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 16:19:19.000000 wsppchem-0.5/src/wsppchem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:19:50.028486 wsppchem-0.5/src/wsppchem/model_and_scaler/
+-rw-r--r--   0 root         (0) root         (0)  3354127 2024-05-17 16:19:20.000000 wsppchem-0.5/src/wsppchem/model_and_scaler/LGBM_model.pkl
+-rw-r--r--   0 root         (0) root         (0)    10174 2024-05-17 16:19:20.000000 wsppchem-0.5/src/wsppchem/model_and_scaler/LGBM_scaler.pkl
+-rw-r--r--   0 root         (0) root         (0)     9875 2024-05-17 16:19:20.000000 wsppchem-0.5/src/wsppchem/wspp_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:19:50.016485 wsppchem-0.5/src/wsppchem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4643 2024-05-17 16:19:49.000000 wsppchem-0.5/src/wsppchem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-17 16:19:49.000000 wsppchem-0.5/src/wsppchem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 16:19:49.000000 wsppchem-0.5/src/wsppchem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-17 16:19:49.000000 wsppchem-0.5/src/wsppchem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-17 16:19:49.000000 wsppchem-0.5/src/wsppchem.egg-info/top_level.txt
```

### Comparing `wsppchem-0.4/LICENSE` & `wsppchem-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wsppchem-0.4/PKG-INFO` & `wsppchem-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsppchem
-Version: 0.4
+Version: 0.5
 Summary: Water Solubility Prediction Project
 Home-page: https://github.com/Nohalyan/WSPP_Projectppchem
 Author: Cossard Lucas and Enzo Venancio
 Author-email: lucas.cossard@epfl.ch and enzo.venancio@epfl.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wsppchem-0.4/README.md` & `wsppchem-0.5/README.md`

 * *Files identical despite different names*

### Comparing `wsppchem-0.4/setup.py` & `wsppchem-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
     name="wsppchem",
-    version="0.4",
+    version="0.5",
     author="Cossard Lucas and Enzo Venancio",
     author_email="lucas.cossard@epfl.ch and enzo.venancio@epfl.ch",
     description="Water Solubility Prediction Project",
     long_description=open('README.md').read() if os.path.exists('README.md') else '',
     long_description_content_type="text/markdown",
     url="https://github.com/Nohalyan/WSPP_Projectppchem",
     packages=find_packages(where='src'),
```

### Comparing `wsppchem-0.4/src/wsppchem/Template.csv` & `wsppchem-0.5/src/wsppchem/Template.csv`

 * *Files identical despite different names*

### Comparing `wsppchem-0.4/src/wsppchem/model_and_scaler/LGBM_model.pkl` & `wsppchem-0.5/src/wsppchem/model_and_scaler/LGBM_model.pkl`

 * *Files identical despite different names*

### Comparing `wsppchem-0.4/src/wsppchem/model_and_scaler/LGBM_scaler.pkl` & `wsppchem-0.5/src/wsppchem/model_and_scaler/LGBM_scaler.pkl`

 * *Files identical despite different names*

### Comparing `wsppchem-0.4/src/wsppchem/wspp_functions.py` & `wsppchem-0.5/src/wsppchem/wspp_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -242,12 +242,21 @@
         logS_prediction = predict_LogS(smiles)
         logS_predictions.append(logS_prediction)
 
     # Add the predicted LogS values to the DataFrame
     df['Predicted_LogS mol/L'] = logS_predictions
 
     # Save the DataFrame with predicted LogS values to a new CSV file
-    output_csv_file = csv_file_path.replace('.csv', '_predicted.csv')
+    output_csv_file = str(Path(csv_file_path).with_name(Path(csv_file_path).stem + '_predicted.csv'))
+    df.to_csv(output_csv_file, index=False)
+    print_space()
+    print(f"Predicted LogS values saved to: {output_csv_file}")
+    print_ascii_art()
+    # Add the predicted LogS values to the DataFrame
+    df['Predicted_LogS mol/L'] = logS_predictions
+
+    # Save the DataFrame with predicted LogS values to a new CSV file
+    output_csv_file = csv_file_path.replace(".csv","_predicted.csv")
     df.to_csv(output_csv_file, index=False)
     print_space()
     print(f"Predicted LogS values saved to: {output_csv_file}")
     print_ascii_art()
```

### Comparing `wsppchem-0.4/src/wsppchem.egg-info/PKG-INFO` & `wsppchem-0.5/src/wsppchem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsppchem
-Version: 0.4
+Version: 0.5
 Summary: Water Solubility Prediction Project
 Home-page: https://github.com/Nohalyan/WSPP_Projectppchem
 Author: Cossard Lucas and Enzo Venancio
 Author-email: lucas.cossard@epfl.ch and enzo.venancio@epfl.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

