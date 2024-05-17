# Comparing `tmp/PROMINENT_methylation-0.1.5.tar.gz` & `tmp/PROMINENT_methylation-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PROMINENT_methylation-0.1.5.tar", last modified: Fri May 17 10:45:17 2024, max compression
+gzip compressed data, was "PROMINENT_methylation-0.1.6.tar", last modified: Fri May 17 10:57:45 2024, max compression
```

## Comparing `PROMINENT_methylation-0.1.5.tar` & `PROMINENT_methylation-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 laz64    (157829) hpark    (16579)        0 2024-05-17 10:45:17.661071 PROMINENT_methylation-0.1.5/
--rw-r--r--   0 laz64    (157829) hpark    (16579)      289 2024-05-17 10:45:17.659652 PROMINENT_methylation-0.1.5/PKG-INFO
-drwxr-xr-x   0 laz64    (157829) hpark    (16579)        0 2024-05-17 10:45:17.617134 PROMINENT_methylation-0.1.5/PROMINENT_methylation/
--rw-r--r--   0 laz64    (157829) hpark    (16579)       37 2024-05-17 10:43:41.000000 PROMINENT_methylation-0.1.5/PROMINENT_methylation/__init__.py
--rw-r--r--   0 laz64    (157829) hpark    (16579)     1489 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.5/PROMINENT_methylation/dataprep.py
--rw-r--r--   0 laz64    (157829) hpark    (16579)     2775 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.5/PROMINENT_methylation/interpret.py
--rwxr-xr-x   0 laz64    (157829) hpark    (16579)     7051 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.5/PROMINENT_methylation/model.py
--rw-r--r--   0 laz64    (157829) hpark    (16579)     3426 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.5/PROMINENT_methylation/scores.py
--rwxr-xr-x   0 laz64    (157829) hpark    (16579)    56770 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.5/PROMINENT_methylation/train.py
--rw-r--r--   0 laz64    (157829) hpark    (16579)     3394 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.5/PROMINENT_methylation/train_test.py
--rwxr-xr-x   0 laz64    (157829) hpark    (16579)     1586 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.5/PROMINENT_methylation/utils.py
-drwxr-xr-x   0 laz64    (157829) hpark    (16579)        0 2024-05-17 10:45:17.652938 PROMINENT_methylation-0.1.5/PROMINENT_methylation.egg-info/
--rw-r--r--   0 laz64    (157829) hpark    (16579)      289 2024-05-17 10:45:16.000000 PROMINENT_methylation-0.1.5/PROMINENT_methylation.egg-info/PKG-INFO
--rw-r--r--   0 laz64    (157829) hpark    (16579)      554 2024-05-17 10:45:16.000000 PROMINENT_methylation-0.1.5/PROMINENT_methylation.egg-info/SOURCES.txt
--rw-r--r--   0 laz64    (157829) hpark    (16579)        1 2024-05-17 10:45:16.000000 PROMINENT_methylation-0.1.5/PROMINENT_methylation.egg-info/dependency_links.txt
--rw-r--r--   0 laz64    (157829) hpark    (16579)      287 2024-05-17 10:45:16.000000 PROMINENT_methylation-0.1.5/PROMINENT_methylation.egg-info/entry_points.txt
--rw-r--r--   0 laz64    (157829) hpark    (16579)       53 2024-05-17 10:45:16.000000 PROMINENT_methylation-0.1.5/PROMINENT_methylation.egg-info/requires.txt
--rw-r--r--   0 laz64    (157829) hpark    (16579)       22 2024-05-17 10:45:16.000000 PROMINENT_methylation-0.1.5/PROMINENT_methylation.egg-info/top_level.txt
--rw-r--r--   0 laz64    (157829) hpark    (16579)       24 2024-05-17 07:22:16.000000 PROMINENT_methylation-0.1.5/README.md
--rw-r--r--   0 laz64    (157829) hpark    (16579)       38 2024-05-17 10:45:17.662690 PROMINENT_methylation-0.1.5/setup.cfg
--rw-r--r--   0 laz64    (157829) hpark    (16579)      986 2024-05-17 10:43:34.000000 PROMINENT_methylation-0.1.5/setup.py
+drwxr-xr-x   0 laz64    (157829) hpark    (16579)        0 2024-05-17 10:57:45.212641 PROMINENT_methylation-0.1.6/
+-rw-r--r--   0 laz64    (157829) hpark    (16579)      289 2024-05-17 10:57:45.210934 PROMINENT_methylation-0.1.6/PKG-INFO
+drwxr-xr-x   0 laz64    (157829) hpark    (16579)        0 2024-05-17 10:57:45.165104 PROMINENT_methylation-0.1.6/PROMINENT_methylation/
+-rw-r--r--   0 laz64    (157829) hpark    (16579)       37 2024-05-17 10:57:38.000000 PROMINENT_methylation-0.1.6/PROMINENT_methylation/__init__.py
+-rw-r--r--   0 laz64    (157829) hpark    (16579)     1489 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.6/PROMINENT_methylation/dataprep.py
+-rw-r--r--   0 laz64    (157829) hpark    (16579)     2775 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.6/PROMINENT_methylation/interpret.py
+-rwxr-xr-x   0 laz64    (157829) hpark    (16579)     7051 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.6/PROMINENT_methylation/model.py
+-rw-r--r--   0 laz64    (157829) hpark    (16579)     3426 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.6/PROMINENT_methylation/scores.py
+-rwxr-xr-x   0 laz64    (157829) hpark    (16579)    56814 2024-05-17 10:57:01.000000 PROMINENT_methylation-0.1.6/PROMINENT_methylation/train.py
+-rw-r--r--   0 laz64    (157829) hpark    (16579)     3416 2024-05-17 10:57:25.000000 PROMINENT_methylation-0.1.6/PROMINENT_methylation/train_test.py
+-rwxr-xr-x   0 laz64    (157829) hpark    (16579)     1586 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.6/PROMINENT_methylation/utils.py
+drwxr-xr-x   0 laz64    (157829) hpark    (16579)        0 2024-05-17 10:57:45.202555 PROMINENT_methylation-0.1.6/PROMINENT_methylation.egg-info/
+-rw-r--r--   0 laz64    (157829) hpark    (16579)      289 2024-05-17 10:57:45.000000 PROMINENT_methylation-0.1.6/PROMINENT_methylation.egg-info/PKG-INFO
+-rw-r--r--   0 laz64    (157829) hpark    (16579)      554 2024-05-17 10:57:45.000000 PROMINENT_methylation-0.1.6/PROMINENT_methylation.egg-info/SOURCES.txt
+-rw-r--r--   0 laz64    (157829) hpark    (16579)        1 2024-05-17 10:57:45.000000 PROMINENT_methylation-0.1.6/PROMINENT_methylation.egg-info/dependency_links.txt
+-rw-r--r--   0 laz64    (157829) hpark    (16579)      287 2024-05-17 10:57:45.000000 PROMINENT_methylation-0.1.6/PROMINENT_methylation.egg-info/entry_points.txt
+-rw-r--r--   0 laz64    (157829) hpark    (16579)       53 2024-05-17 10:57:45.000000 PROMINENT_methylation-0.1.6/PROMINENT_methylation.egg-info/requires.txt
+-rw-r--r--   0 laz64    (157829) hpark    (16579)       22 2024-05-17 10:57:45.000000 PROMINENT_methylation-0.1.6/PROMINENT_methylation.egg-info/top_level.txt
+-rw-r--r--   0 laz64    (157829) hpark    (16579)       24 2024-05-17 07:22:16.000000 PROMINENT_methylation-0.1.6/README.md
+-rw-r--r--   0 laz64    (157829) hpark    (16579)       38 2024-05-17 10:57:45.214571 PROMINENT_methylation-0.1.6/setup.cfg
+-rw-r--r--   0 laz64    (157829) hpark    (16579)      986 2024-05-17 10:57:33.000000 PROMINENT_methylation-0.1.6/setup.py
```

### Comparing `PROMINENT_methylation-0.1.5/PROMINENT_methylation/dataprep.py` & `PROMINENT_methylation-0.1.6/PROMINENT_methylation/dataprep.py`

 * *Files identical despite different names*

### Comparing `PROMINENT_methylation-0.1.5/PROMINENT_methylation/interpret.py` & `PROMINENT_methylation-0.1.6/PROMINENT_methylation/interpret.py`

 * *Files identical despite different names*

### Comparing `PROMINENT_methylation-0.1.5/PROMINENT_methylation/model.py` & `PROMINENT_methylation-0.1.6/PROMINENT_methylation/model.py`

 * *Files identical despite different names*

### Comparing `PROMINENT_methylation-0.1.5/PROMINENT_methylation/scores.py` & `PROMINENT_methylation-0.1.6/PROMINENT_methylation/scores.py`

 * *Files identical despite different names*

### Comparing `PROMINENT_methylation-0.1.5/PROMINENT_methylation/train.py` & `PROMINENT_methylation-0.1.6/PROMINENT_methylation/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import roc_auc_score, average_precision_score
 from sklearn.metrics import precision_recall_curve
 from statistics import mean 
 from imblearn.over_sampling import SMOTE
 import shap
 import pickle
-from model import *
-from utils import *
+from PROMINENT_methylation.model import *
+from PROMINENT_methylation.utils import *
 import matplotlib.pyplot as plt
 
 class train_kfold:
     def __init__(self, trainArgs):
    
         """
         args:
```

### Comparing `PROMINENT_methylation-0.1.5/PROMINENT_methylation/train_test.py` & `PROMINENT_methylation-0.1.6/PROMINENT_methylation/train_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 import pandas as pd
 from torch import nn
 import torch.nn.functional as F
 from sklearn.preprocessing import MinMaxScaler
 import matplotlib.pyplot as plt
 import argparse
-from train import *
+from PROMINENT_methylation.train import *
 
 def preprocessing1(path_fn, gene_fn, label_fn):
     ### pathway datasets
     if os.path.exists(path_fn):
         pathway = pd.read_csv(path_fn, header=0)       
         print(">> Pathway Data :",path_fn)
         pathway_info = pathway.iloc[:,1:]
```

### Comparing `PROMINENT_methylation-0.1.5/PROMINENT_methylation/utils.py` & `PROMINENT_methylation-0.1.6/PROMINENT_methylation/utils.py`

 * *Files identical despite different names*

### Comparing `PROMINENT_methylation-0.1.5/PROMINENT_methylation.egg-info/SOURCES.txt` & `PROMINENT_methylation-0.1.6/PROMINENT_methylation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PROMINENT_methylation-0.1.5/setup.py` & `PROMINENT_methylation-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='PROMINENT_methylation',
-    version='0.1.5',
+    version='0.1.6',
     packages=['PROMINENT_methylation'],
     description='PROMINENT: AN INTERPRETABLE DEEP LEARNING METHOD TO PREDICT PHENOTYPES USING DNA METHYLATION',
     url='https://github.com/cloudmacchiato/dlmethylation',
     author='Laizhi Zhang',
     author_email='laz64@pitt.edu',
     license='MIT',
     entry_points={
```

