# Comparing `tmp/wsppchem-0.5.tar.gz` & `tmp/wsppchem-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsppchem-0.5.tar", last modified: Fri May 17 16:19:50 2024, max compression
+gzip compressed data, was "wsppchem-0.6.tar", last modified: Fri May 17 17:06:32 2024, max compression
```

## Comparing `wsppchem-0.5.tar` & `wsppchem-0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:19:50.029486 wsppchem-0.5/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-17 16:19:19.000000 wsppchem-0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4643 2024-05-17 16:19:50.029486 wsppchem-0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4156 2024-05-17 16:19:19.000000 wsppchem-0.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 16:19:50.029486 wsppchem-0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      962 2024-05-17 16:19:19.000000 wsppchem-0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:19:50.013485 wsppchem-0.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:19:50.015485 wsppchem-0.5/src/wsppchem/
--rw-r--r--   0 root         (0) root         (0)     3701 2024-05-17 16:19:19.000000 wsppchem-0.5/src/wsppchem/Template.csv
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 16:19:19.000000 wsppchem-0.5/src/wsppchem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:19:50.028486 wsppchem-0.5/src/wsppchem/model_and_scaler/
--rw-r--r--   0 root         (0) root         (0)  3354127 2024-05-17 16:19:20.000000 wsppchem-0.5/src/wsppchem/model_and_scaler/LGBM_model.pkl
--rw-r--r--   0 root         (0) root         (0)    10174 2024-05-17 16:19:20.000000 wsppchem-0.5/src/wsppchem/model_and_scaler/LGBM_scaler.pkl
--rw-r--r--   0 root         (0) root         (0)     9875 2024-05-17 16:19:20.000000 wsppchem-0.5/src/wsppchem/wspp_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:19:50.016485 wsppchem-0.5/src/wsppchem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4643 2024-05-17 16:19:49.000000 wsppchem-0.5/src/wsppchem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-17 16:19:49.000000 wsppchem-0.5/src/wsppchem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 16:19:49.000000 wsppchem-0.5/src/wsppchem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-05-17 16:19:49.000000 wsppchem-0.5/src/wsppchem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-17 16:19:49.000000 wsppchem-0.5/src/wsppchem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:06:32.358621 wsppchem-0.6/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-17 17:05:59.000000 wsppchem-0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3874 2024-05-17 17:06:32.358621 wsppchem-0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3387 2024-05-17 17:05:59.000000 wsppchem-0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 17:06:32.359621 wsppchem-0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      962 2024-05-17 17:05:59.000000 wsppchem-0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:06:32.349620 wsppchem-0.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:06:32.350621 wsppchem-0.6/src/wsppchem/
+-rw-r--r--   0 root         (0) root         (0)     3701 2024-05-17 17:05:59.000000 wsppchem-0.6/src/wsppchem/Template.csv
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 17:05:59.000000 wsppchem-0.6/src/wsppchem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:06:32.357621 wsppchem-0.6/src/wsppchem/model_and_scaler/
+-rw-r--r--   0 root         (0) root         (0)  3354127 2024-05-17 17:05:59.000000 wsppchem-0.6/src/wsppchem/model_and_scaler/LGBM_model.pkl
+-rw-r--r--   0 root         (0) root         (0)    10174 2024-05-17 17:05:59.000000 wsppchem-0.6/src/wsppchem/model_and_scaler/LGBM_scaler.pkl
+-rw-r--r--   0 root         (0) root         (0)     9982 2024-05-17 17:05:59.000000 wsppchem-0.6/src/wsppchem/wspp_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:06:32.351621 wsppchem-0.6/src/wsppchem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3874 2024-05-17 17:06:32.000000 wsppchem-0.6/src/wsppchem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-17 17:06:32.000000 wsppchem-0.6/src/wsppchem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 17:06:32.000000 wsppchem-0.6/src/wsppchem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-17 17:06:32.000000 wsppchem-0.6/src/wsppchem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-17 17:06:32.000000 wsppchem-0.6/src/wsppchem.egg-info/top_level.txt
```

### Comparing `wsppchem-0.5/LICENSE` & `wsppchem-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wsppchem-0.5/README.md` & `wsppchem-0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,82 +1,100 @@
+Metadata-Version: 2.1
+Name: wsppchem
+Version: 0.6
+Summary: Water Solubility Prediction Project
+Home-page: https://github.com/Nohalyan/WSPP_Projectppchem
+Author: Cossard Lucas and Enzo Venancio
+Author-email: lucas.cossard@epfl.ch and enzo.venancio@epfl.ch
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![Project Logo](assets/WSPP_logo.png)
 
 <h1 align="center">
 Water Solubility Prediction Project
 </h1>
 
-## Overview
-This project aims to predict the water solubility of chemical compounds using machine learning techniques. The project developed here can be used to estimate the solubility of new compounds only using the SMILES code of the compounds, which can be valuable in various industries such as pharmaceuticals, agriculture, and environmental science.
+## 🔍 Overview 🔎
+This project aims to predict the water solubility of chemical compounds using machine learning techniques. The project developed here can be used to estimate the water solubility of new compounds only using the SMILES code, which can be valuable in various industries such as pharmaceuticals, agriculture, and environmental science.
 In this repository, we are making available the data we used to train and test our models and `.pkl` files containing the optimized parameters of our best model. But more importantly a notebook tracing what we did from the beginning to the end of this project and a package that can predict the water solubility of several SMILEs and of a `.csv` file containing several SMILEs. 
 
-## Project Structure
-The project is structured as follows:
+## 📝 Project Structure 📝
+This project contains two main elements: a Notebook and a Package.
 
-**First, a Notebook containing:**
+**1️⃣ A Notebook containing:**
 - Import Relevant Modules and Libraries
 - Data Collection
 - Data Cleaning
 - Calculation of RDkit Molecular Descriptors
-- Select Machine Learning Models
+- Selection of Machine Learning Models
 - Fine-tuning
 - Analysis of different models
-- Saving of the best trained model and standard scaler
+- Saving of the best trained model and scaler
+
+**2️⃣ A Package containing two main functions:**
 
-**Second, a Package of two main functions containing:**
--  A function tp predict the LogS value for one or more  SMILES
+-  A function to predict the LogS value for one or more  SMILES
 -  A function to predicts LogS values for SMILES codes stored in a CSV file
  
-## Installation
-1. Clone this repository:
+## 🔨 Installation 🔨
+### 🌍 Environment 🌍
+1. clone our repository:
 ```
 git clone https://github.com/Nohalyan/Projetppchem
 ```
-2. Open your terminal or Anaconda Prompt and navigate to the directory `/src/Projectppchem` containing the `ppchem_environment.yml` file and run the following command to create the Conda environment:
+
+2. Open your terminal or Anaconda Prompt and navigate to the directory /WSPP_Projectppchem containing the wsppchem_env_environment.yml file and run the following command to create the Conda environment:
 ```
-conda env create -f ppchem_environment.yml
+conda env create -f environment.yml
 ```
-3. Activate the newly created Conda environment:
+
+3. Activate the environment: After creating the environment, activate it using:
 ```
-conda activate ppchem_environment 
+conda activate wsppchem_env
 ```
 
-## Usage
+4. Verify the environment: To check that all the dependencies are installed correctly, you can list the installed packages:
+```
+conda list
+```
 
-### For the Notebook:
+### 📦 Package 📦
 
-1. **Data Preparation:** Place your dataset in the `data/` directory. Ensure the dataset is formatted correctly with features and labels.
-2. **Exploratory Data Analysis:** Explore the dataset using the Colab notebooks in the `notebooks/` directory to understand the data distribution and relationships.
-3. **Model Training:** Use the scripts in the Colab notebooks in the `notebooks/` directory to preprocess the data, train machine learning models, and save the trained models in the corresponding `models/` directory.
-4. **Model Evaluation:** Evaluate the model performance using the evaluation using the scripts in the Colab notebooks in the `notebooks/` directory.
-5. **Prediction:** Once trained, the models in the models/ directory can be used to predict the water solubility of new compounds by providing the required input features.
-6. 
-### For the Package:
-First, clone our repos
-If you are using a notebook without the environment, you can download the necessary libraries:
+1. Install our package `wsppchem` with a simple pip install.
 ```
-!pip install pandas numpy rdkit tqdm lightgbm
+pip install wsppchem
 ```
 
-Once the repository has been cloned, you can use the following function to import the functions of our pacakge:
+2. Import all the functions using the following command.
 ```
-from Projectppchem.src.WSPP import wspp_functions as wspp
+from wsppchem.wspp_functions import *
 ```
-
+3. Enjoy! 😁
 The two main functions of our package are `predict_logS_smiles` and `predict_logS_csv` which can be used in the following way:
 ```
-wspp.predict_logS_smiles(*smiles_codes) and wspp.predict_logS_csv(csv_file_path)
+predict_logS_smiles(*smiles_codes)
+```
+
 ```
-The first function `wspp.predict_logS_smiles(*smiles_codes)` can be used to predict the LogS value for one or more SMILES at the same time.
-The second fucntion `wspp.predict_logS_csv(csv_file_path)` can be used to predicts LogS values for SMILES codes stored in a CSV file.
-And if you need any help, you can use the function `wspp.help()` which will give you more precise information on the functions as well as an example of how to use them. 
+predict_logS_csv(csv_file_path)
+```
+
+The first function `predict_logS_smiles(*smiles_codes)` can be used to predict the LogS value for one or more SMILES at the same time.
+The second fucntion `predict_logS_csv(csv_file_path)` can be used to predicts LogS values for SMILES codes stored in a CSV file.
+And if you need any help, you can use the function `wspphelp()` which will give you more precise information on the functions as well as an example of how to use them. 
 
-## License
+## 📗 License 📕
 This project is licensed under the MIT License.
 
-## References
+## 📜 References 📜
 This project is based on the code of this Github Jupyter notebook: https://github.com/gashawmg, as well as data from https://github.com/PatWalters. 
 
-## Authors
+## 📖 Authors 📖
 - Cossard Lucas: https://github.com/Nohalyan
 - Venancio Enzo: https://github.com/Enzo-vnc
 
 This project was carried out as part of EPFL's Practical programming in Chemistry course.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wsppchem-0.5/setup.py` & `wsppchem-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
     name="wsppchem",
-    version="0.5",
+    version="0.6",
     author="Cossard Lucas and Enzo Venancio",
     author_email="lucas.cossard@epfl.ch and enzo.venancio@epfl.ch",
     description="Water Solubility Prediction Project",
     long_description=open('README.md').read() if os.path.exists('README.md') else '',
     long_description_content_type="text/markdown",
     url="https://github.com/Nohalyan/WSPP_Projectppchem",
     packages=find_packages(where='src'),
```

### Comparing `wsppchem-0.5/src/wsppchem/Template.csv` & `wsppchem-0.6/src/wsppchem/Template.csv`

 * *Files identical despite different names*

### Comparing `wsppchem-0.5/src/wsppchem/model_and_scaler/LGBM_model.pkl` & `wsppchem-0.6/src/wsppchem/model_and_scaler/LGBM_model.pkl`

 * *Files identical despite different names*

### Comparing `wsppchem-0.5/src/wsppchem/model_and_scaler/LGBM_scaler.pkl` & `wsppchem-0.6/src/wsppchem/model_and_scaler/LGBM_scaler.pkl`

 * *Files identical despite different names*

### Comparing `wsppchem-0.5/src/wsppchem/wspp_functions.py` & `wsppchem-0.6/src/wsppchem/wspp_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,41 +8,43 @@
 from rdkit.Chem import Descriptors
 from rdkit.Chem import rdMolDescriptors 
 from rdkit.ML.Descriptors import MoleculeDescriptors
 from tqdm import tqdm
 from lightgbm import LGBMRegressor
 import importlib.resources as pkg_resources
 import pickle
+from pathlib import Path
 
 
-#============================================================================================================================================
 
+#================================================================================================================================================
 
 
-def wshelp():
+
+def wspphelp():
     print_help= """
     This package contains 2 main functions:  predict_logS_smiles and predict_logS_csv
     
-    ==========================================================================================================================================
+    ==============================================================================================================================================
     
     predict_logS_smiles(smiles_code)
     
     Description: Predicts the LogS value for one or more  SMILES.
     Usage: Provide one or more valid SMILES codes in a string as input
     Example: predict_logS_smiles("CC(=O)NC1=CC=C(C=C1)O","CN1C=NC2=C1C(=O)N(C(=O)N2C)C")
     
-    ==========================================================================================================================================
+    ==============================================================================================================================================
     
     predict_logS_csv(csv_file_path):
     
     Description: Predicts LogS values for SMILES codes stored in a CSV file
     Usage: Provide the path to a CSV file containing SMILES codes in the 'SMILE' column (see Template.csv for an example of a valid csv file)
-    Example: predict_logS_csv("/content/WSPP_Projectppchem/src/WSPP/Template.csv")
+    Example: predict_logS_csv("your_csv_file_path") or predict_logS_csv() if you want to test the function with the "Templater.csv" file provided
 
-    ==========================================================================================================================================
+    ==============================================================================================================================================
     """
     print(print_help)
 
 
 
 def print_space():
     """
```

