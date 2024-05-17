# Comparing `tmp/lux_explainer-1.2.0.tar.gz` & `tmp/lux_explainer-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lux_explainer-1.2.0.tar", last modified: Tue Apr 30 10:43:44 2024, max compression
+gzip compressed data, was "lux_explainer-1.2.1.tar", last modified: Fri May 17 18:37:56 2024, max compression
```

## Comparing `lux_explainer-1.2.0.tar` & `lux_explainer-1.2.1.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-04-30 10:43:44.283125 lux_explainer-1.2.0/
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     1063 2024-01-29 09:30:50.000000 lux_explainer-1.2.0/LICENSE
--rw-r--r--   0 sbk       (1000) sbk       (1000)     8662 2024-04-30 10:43:44.283125 lux_explainer-1.2.0/PKG-INFO
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     6383 2024-03-20 13:56:27.000000 lux_explainer-1.2.0/README.md
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     1066 2024-04-30 08:23:51.000000 lux_explainer-1.2.0/pyproject.toml
--rw-rw-r--   0 sbk       (1000) sbk       (1000)       38 2024-04-30 10:43:44.283125 lux_explainer-1.2.0/setup.cfg
-drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-04-30 10:43:44.275125 lux_explainer-1.2.0/src/
-drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-04-30 10:43:44.279125 lux_explainer-1.2.0/src/lux/
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     7114 2024-03-09 15:54:20.000000 lux_explainer-1.2.0/src/lux/UncertainSMOTE.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)       22 2024-03-08 10:52:00.000000 lux_explainer-1.2.0/src/lux/__init__.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)    46500 2024-04-30 07:41:18.000000 lux_explainer-1.2.0/src/lux/lux.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     8830 2024-04-29 12:39:41.000000 lux_explainer-1.2.0/src/lux/metrics.py
-drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-04-30 10:43:44.283125 lux_explainer-1.2.0/src/lux/pyuid3/
--rw-rw-r--   0 sbk       (1000) sbk       (1000)       22 2024-02-22 11:28:53.000000 lux_explainer-1.2.0/src/lux/pyuid3/__init__.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     4344 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/att_stats.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     2085 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/attribute.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)    16634 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/data.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     4453 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/data_scrambler.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     2365 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/entropy_evaluator.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     1097 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/instance.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)      231 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/parse_exception.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     3290 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/reading.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)    24853 2024-04-30 08:17:57.000000 lux_explainer-1.2.0/src/lux/pyuid3/tree.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)      527 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/tree_edge.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     7595 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/tree_evaluator.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     1528 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/tree_node.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)    30251 2024-04-30 07:45:14.000000 lux_explainer-1.2.0/src/lux/pyuid3/uid3.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     1157 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/utils.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)     1395 2024-01-29 10:15:03.000000 lux_explainer-1.2.0/src/lux/pyuid3/value.py
--rw-rw-r--   0 sbk       (1000) sbk       (1000)    12662 2024-04-30 07:37:40.000000 lux_explainer-1.2.0/src/lux/samplers.py
-drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-04-30 10:43:44.283125 lux_explainer-1.2.0/src/lux_explainer.egg-info/
--rw-r--r--   0 sbk       (1000) sbk       (1000)     8662 2024-04-30 10:43:44.000000 lux_explainer-1.2.0/src/lux_explainer.egg-info/PKG-INFO
--rw-rw-r--   0 sbk       (1000) sbk       (1000)      781 2024-04-30 10:43:44.000000 lux_explainer-1.2.0/src/lux_explainer.egg-info/SOURCES.txt
--rw-rw-r--   0 sbk       (1000) sbk       (1000)        1 2024-04-30 10:43:44.000000 lux_explainer-1.2.0/src/lux_explainer.egg-info/dependency_links.txt
--rw-rw-r--   0 sbk       (1000) sbk       (1000)      227 2024-04-30 10:43:44.000000 lux_explainer-1.2.0/src/lux_explainer.egg-info/requires.txt
--rw-rw-r--   0 sbk       (1000) sbk       (1000)        4 2024-04-30 10:43:44.000000 lux_explainer-1.2.0/src/lux_explainer.egg-info/top_level.txt
+drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-05-17 18:37:56.518657 lux_explainer-1.2.1/
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     1063 2024-01-29 09:30:50.000000 lux_explainer-1.2.1/LICENSE
+-rw-r--r--   0 sbk       (1000) sbk       (1000)     9487 2024-05-17 18:37:56.518657 lux_explainer-1.2.1/PKG-INFO
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     7209 2024-05-02 08:07:21.000000 lux_explainer-1.2.1/README.md
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     1066 2024-05-17 18:37:49.000000 lux_explainer-1.2.1/pyproject.toml
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)       38 2024-05-17 18:37:56.518657 lux_explainer-1.2.1/setup.cfg
+drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-05-17 18:37:56.518657 lux_explainer-1.2.1/src/
+drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-05-17 18:37:56.518657 lux_explainer-1.2.1/src/lux/
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)       22 2024-03-08 10:52:00.000000 lux_explainer-1.2.1/src/lux/__init__.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)    47586 2024-05-17 18:34:37.000000 lux_explainer-1.2.1/src/lux/lux.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     8830 2024-04-29 12:39:41.000000 lux_explainer-1.2.1/src/lux/metrics.py
+drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-05-17 18:37:56.518657 lux_explainer-1.2.1/src/lux/pyuid3/
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)       22 2024-02-22 11:28:53.000000 lux_explainer-1.2.1/src/lux/pyuid3/__init__.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     4344 2024-01-29 10:15:03.000000 lux_explainer-1.2.1/src/lux/pyuid3/att_stats.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     2085 2024-01-29 10:15:03.000000 lux_explainer-1.2.1/src/lux/pyuid3/attribute.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)    23527 2024-04-30 12:54:17.000000 lux_explainer-1.2.1/src/lux/pyuid3/data.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     4453 2024-01-29 10:15:03.000000 lux_explainer-1.2.1/src/lux/pyuid3/data_scrambler.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     2365 2024-01-29 10:15:03.000000 lux_explainer-1.2.1/src/lux/pyuid3/entropy_evaluator.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     1097 2024-01-29 10:15:03.000000 lux_explainer-1.2.1/src/lux/pyuid3/instance.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)      231 2024-01-29 10:15:03.000000 lux_explainer-1.2.1/src/lux/pyuid3/parse_exception.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     3290 2024-01-29 10:15:03.000000 lux_explainer-1.2.1/src/lux/pyuid3/reading.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)    24853 2024-04-30 08:17:57.000000 lux_explainer-1.2.1/src/lux/pyuid3/tree.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)      527 2024-01-29 10:15:03.000000 lux_explainer-1.2.1/src/lux/pyuid3/tree_edge.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     7595 2024-01-29 10:15:03.000000 lux_explainer-1.2.1/src/lux/pyuid3/tree_evaluator.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     1528 2024-01-29 10:15:03.000000 lux_explainer-1.2.1/src/lux/pyuid3/tree_node.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)    32135 2024-04-30 12:40:28.000000 lux_explainer-1.2.1/src/lux/pyuid3/uid3.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     1157 2024-01-29 10:15:03.000000 lux_explainer-1.2.1/src/lux/pyuid3/utils.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)     1395 2024-01-29 10:15:03.000000 lux_explainer-1.2.1/src/lux/pyuid3/value.py
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)    17794 2024-04-30 12:38:30.000000 lux_explainer-1.2.1/src/lux/samplers.py
+drwxrwxr-x   0 sbk       (1000) sbk       (1000)        0 2024-05-17 18:37:56.518657 lux_explainer-1.2.1/src/lux_explainer.egg-info/
+-rw-r--r--   0 sbk       (1000) sbk       (1000)     9487 2024-05-17 18:37:56.000000 lux_explainer-1.2.1/src/lux_explainer.egg-info/PKG-INFO
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)      755 2024-05-17 18:37:56.000000 lux_explainer-1.2.1/src/lux_explainer.egg-info/SOURCES.txt
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)        1 2024-05-17 18:37:56.000000 lux_explainer-1.2.1/src/lux_explainer.egg-info/dependency_links.txt
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)      227 2024-05-17 18:37:56.000000 lux_explainer-1.2.1/src/lux_explainer.egg-info/requires.txt
+-rw-rw-r--   0 sbk       (1000) sbk       (1000)        4 2024-05-17 18:37:56.000000 lux_explainer-1.2.1/src/lux_explainer.egg-info/top_level.txt
```

### Comparing `lux_explainer-1.2.0/LICENSE` & `lux_explainer-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lux_explainer-1.2.0/PKG-INFO` & `lux_explainer-1.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lux-explainer
-Version: 1.2.0
+Version: 1.2.1
 Summary: Universal Local Rule-based Explainer
 Author-email: Szymon Bobek <szymon.bobek@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 sbobek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,14 +45,17 @@
 Requires-Dist: shap>=0.41.0
 Requires-Dist: lime>=0.2.0.1
 Requires-Dist: anchor-exp>=0.0.2.0
 Requires-Dist: imbalanced-learn>=0.9.1
 Requires-Dist: gower>=0.1.2
 Requires-Dist: numdifftools>=0.9.41
 
+[![PyPI](https://img.shields.io/pypi/v/lux-explainer)](https://pypi.org/project/lux-explainer/)  ![License](https://img.shields.io/github/license/sbobek/lux)
+ ![PyPI - Downloads](https://img.shields.io/pypi/dm/lux-explainer) [![Documentation Status](https://readthedocs.org/projects/lux-explainer/badge/?version=latest)](https://tsproto.readthedocs.io/en/latest/?badge=latest)
+   
 # LUX (Local Universal Rule-based Explainer)
 ## Main features
   <img align="right"  src="https://raw.githubusercontent.com/sbobek/lux/main/pix/lux-logo.png" width="200">
   
   * Model-agnostic, rule-based and visual local explanations of black-box ML models
   * Integrated counterfactual explanations
   * Rule-based explanations (that are executable at the same time)
@@ -157,15 +160,17 @@
 You can obtain a whole rule-based model for the local uncertain explanation that was generated by LUX for given instance by running following code
 
 ``` python
 #have a look at the entire rule-based model that can be executed with https:://heartdroid.re
 print(lux.to_HMR())
 ```
 
-This will generate model which can later be executed by [HeaRTDroid](https://heartdroid.re)
+This will generate model which can later be executed by [HeaRTDroid](https://heartdroid.re) which is rule-based inference engine for Android mobile devices.
+Additionally, the HMR format below, which is used by  [HeaRTDroid](https://heartdroid.re) allows visualization of explanations in a format of decision tables with [HWEd](https://heartdroid.re/hwed/#/) online editor.
+
 
 ```
 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%% TYPES DEFINITIONS %%%%%%%%%%%%%%%%%%%%%%%%%%
 
 xtype [
  name: petal_length, 
 base:numeric,
@@ -209,17 +214,19 @@
 
 The code should yield something like that (depending on the instance that was selected):
 
 ![](https://raw.githubusercontent.com/sbobek/lux/main/pix/utree.png)
 
 # Cite this work
 
+The software is the direct implementation of a method described in the following paper:
+
 ```
 @misc{bobek2023local,
-      title={Local Universal Rule-based Explanations}, 
+      title={Local Universal Explainer ({LUX}) -- a rule-based explainer with factual, counterfactual and visual explanations}, 
       author={Szymon Bobek and Grzegorz J. Nalepa},
       year={2023},
       eprint={2310.14894},
       archivePrefix={arXiv},
       primaryClass={cs.AI}
 
 }
```

### Comparing `lux_explainer-1.2.0/README.md` & `lux_explainer-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+[![PyPI](https://img.shields.io/pypi/v/lux-explainer)](https://pypi.org/project/lux-explainer/)  ![License](https://img.shields.io/github/license/sbobek/lux)
+ ![PyPI - Downloads](https://img.shields.io/pypi/dm/lux-explainer) [![Documentation Status](https://readthedocs.org/projects/lux-explainer/badge/?version=latest)](https://tsproto.readthedocs.io/en/latest/?badge=latest)
+   
 # LUX (Local Universal Rule-based Explainer)
 ## Main features
   <img align="right"  src="https://raw.githubusercontent.com/sbobek/lux/main/pix/lux-logo.png" width="200">
   
   * Model-agnostic, rule-based and visual local explanations of black-box ML models
   * Integrated counterfactual explanations
   * Rule-based explanations (that are executable at the same time)
@@ -106,15 +109,17 @@
 You can obtain a whole rule-based model for the local uncertain explanation that was generated by LUX for given instance by running following code
 
 ``` python
 #have a look at the entire rule-based model that can be executed with https:://heartdroid.re
 print(lux.to_HMR())
 ```
 
-This will generate model which can later be executed by [HeaRTDroid](https://heartdroid.re)
+This will generate model which can later be executed by [HeaRTDroid](https://heartdroid.re) which is rule-based inference engine for Android mobile devices.
+Additionally, the HMR format below, which is used by  [HeaRTDroid](https://heartdroid.re) allows visualization of explanations in a format of decision tables with [HWEd](https://heartdroid.re/hwed/#/) online editor.
+
 
 ```
 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%% TYPES DEFINITIONS %%%%%%%%%%%%%%%%%%%%%%%%%%
 
 xtype [
  name: petal_length, 
 base:numeric,
@@ -158,18 +163,20 @@
 
 The code should yield something like that (depending on the instance that was selected):
 
 ![](https://raw.githubusercontent.com/sbobek/lux/main/pix/utree.png)
 
 # Cite this work
 
+The software is the direct implementation of a method described in the following paper:
+
 ```
 @misc{bobek2023local,
-      title={Local Universal Rule-based Explanations}, 
+      title={Local Universal Explainer ({LUX}) -- a rule-based explainer with factual, counterfactual and visual explanations}, 
       author={Szymon Bobek and Grzegorz J. Nalepa},
       year={2023},
       eprint={2310.14894},
       archivePrefix={arXiv},
       primaryClass={cs.AI}
 
 }
-```
+```
```

### Comparing `lux_explainer-1.2.0/pyproject.toml` & `lux_explainer-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lux-explainer"
-version = "1.2.0"
+version = "1.2.1"
 description = "Universal Local Rule-based Explainer"
 readme = "README.md"
 authors = [{ name = "Szymon Bobek", email = "szymon.bobek@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `lux_explainer-1.2.0/src/lux/lux.py` & `lux_explainer-1.2.1/src/lux/lux.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from imblearn.over_sampling import SMOTENC, SMOTE
 from sklearn.base import BaseEstimator
 from sklearn.metrics import accuracy_score
 import pandas as pd
 
-from lux.UncertainSMOTE import UncertainSMOTE
+from lux.samplers import UncertainSMOTE
 from lux.pyuid3.data import Data
 from lux.pyuid3.entropy_evaluator import UncertainEntropyEvaluator
 from lux.pyuid3.uid3 import UId3
 from sklearn.neighbors import NearestNeighbors
 from sklearn.cluster import OPTICS
 import shap
 import sklearn
@@ -76,15 +77,15 @@
         :param min_generate_samples: float, optional
             The minimum proportion of the dataset size to generate perturbed instances. This is used by the UncertainSMOTE algotrothm. Default is 0.02.
         :type min_generate_samples: float
         :param uncertainty_sigma: float, optional
             The uncertainty parameter sigma used in the filtering uncertain samples. Every sample that is 2*uncertainty_sigma away from the mean will be removed. Default is 2.
         :type uncertainty_sigma: float
         :param oversampling_strategy: str, optional
-            The strategy for oversampling. It can be 'smote', 'importance', or 'both'. Default is 'smote'.
+            The strategy for oversampling. It can be 'smote', 'importance', or 'both'. Default is 'both'.
         :type oversampling_strategy: str
         """
 
         self.neighborhood_size = neighborhood_size
         self.max_depth = max_depth
         self.node_size_limit = node_size_limit
         self.grow_confidence_threshold = grow_confidence_threshold
@@ -578,17 +579,24 @@
                 instance_to_explain = boundiong_box_points[0]
                 X_train_sample = self.__oversample_smote(X_train_sample, categorical=categorical,
                                                          instance_to_explain=instance_to_explain)
                 isam = ImportanceSampler(classifier=self.classifier, predict_proba=self.predict_proba,
                                          indstance2explain=instance_to_explain,
                                          min_generate_samples=self.min_generate_samples)
                 X_train_sample = isam.fit_transform(X_train_sample)
+                if categorical is not None and sum(categorical) > 0:
+                    sm = SMOTENC(categorical_features=categorical)
+                else:
+                    sm = SMOTE()
+
+                X_train_sample_np, _ = sm.fit_resample(X_train_sample, self.classifier.predict(X_train_sample))
+                X_train_sample = pd.DataFrame(X_train_sample_np, columns=X_train_sample.columns)
 
             cols = X_train_sample.columns
-            X_train_sample_arr = np.concatenate((X_train_sample, np.ones((int(0.3 * X_train_sample.shape[0]), X_train_sample.shape[1])) * instance_to_explain))
+            X_train_sample_arr = np.concatenate((X_train_sample, np.ones((int(self.neighborhood_size * X_train_sample.shape[0]), X_train_sample.shape[1])) * instance_to_explain))
             X_train_sample = pd.DataFrame(X_train_sample_arr, columns=cols)
 
         if X_importances is not None:
             return X_train_sample, X_train_sample_importances
         else:
             return X_train_sample, None
 
@@ -732,15 +740,15 @@
         """
         if categorical is None:
             categorical = [False] * len(features)
         query = []
         if rule == {}:
             return 0, 0
         for i, v in rule.items():
-            op = '' if dict(zip(features, categorical))[i] == False else '=='
+            op = '' #if dict(zip(features, categorical))[i] == False else '=='
             query.append(f'{i}{op}' + f'and {i}{op}'.join(v))
 
         covered = dataset.query(' and '.join(query))
         return covered
 
     def counterfactual(self, instance_to_explain, background, counterfactual_representative='medoid', reduce=True,
                        topn=None, n_jobs=None):
@@ -780,15 +788,22 @@
                         dist = sklearn.metrics.pairwise_distances(rule['covered'].iloc[ids].values.reshape(1, -1),
                                                                   instance_to_explain)
                         representative_sample = rule['covered'].iloc[ids]
                         rule['counterfactual'] = representative_sample
                         rule['distance'] = dist
                 elif counterfactual_representative == self.CF_REPRESENTATIVE_NEAREST:
                     if self.categorical is not None:
-                        ids_dist = gower.gower_topn(instance_to_explain, rule['covered'], n=1,
+                        import inspect
+                        signature = inspect.signature(gower.gower_topn)
+                        has_njobs = 'n_jobs' in signature.parameters
+                        if has_njobs:
+                            ids_dist = gower.gower_topn(instance_to_explain, rule['covered'], n=1,
+                                                        cat_features=self.categorical, n_jobs=n_jobs)
+                        else:
+                            ids_dist = gower.gower_topn(instance_to_explain, rule['covered'], n=1,
                                                     cat_features=self.categorical, n_jobs=n_jobs)
                         representative_sample = rule['covered'].iloc[ids_dist['index'].ravel()[0]]
                         rule['counterfactual'] = representative_sample
                         dist = ids_dist['values']
                         rule['distance'] = dist
                     else:
                         nn_inverse = NearestNeighbors(n_neighbors=1, metric='minkowski')
@@ -804,18 +819,24 @@
         counterfactual_rules = sorted(counterfactual_rules, key=lambda d: d['distance'])
         if topn is None:
             return counterfactual_rules
         else:
             return counterfactual_rules[:topn]
 
     def visualize(self, data, target_column_name='class',instance2explain=None, counterfactual=None, filename='tree.dot'):
-        cfdf = pd.DataFrame(counterfactual['counterfactual']).T
-        cfdf[target_column_name] = np.argmax(self.predict_proba(cfdf.values.reshape(1, -1))[0])
-        i2edf = pd.DataFrame(instance2explain, columns=self.attributes_names)
-        i2edf[target_column_name] = np.argmax(self.predict_proba(i2edf.values.reshape(1, -1))[0])
+        if counterfactual is not None:
+            cfdf = pd.DataFrame(counterfactual['counterfactual']).T
+            cfdf[target_column_name] = np.argmax(self.predict_proba(cfdf.values.reshape(1, -1))[0])
+        else:
+            cfdf=None
+        if instance2explain is not None:
+            i2edf = pd.DataFrame(instance2explain, columns=self.attributes_names)
+            i2edf[target_column_name] = np.argmax(self.predict_proba(i2edf.values.reshape(1, -1))[0])
+        else:
+            i2edf=None
         self.uid3.tree.save_dot(filename, fmt='.2f', visual=True, background_data=data, instance2explain=i2edf,
                                 counterfactual=cfdf)
 
     def to_HMR(self):
         """ Exports to HMR format that can be executed by the HeaRTDroid rule-engine
 
         :return:
```

### Comparing `lux_explainer-1.2.0/src/lux/metrics.py` & `lux_explainer-1.2.1/src/lux/metrics.py`

 * *Files identical despite different names*

### Comparing `lux_explainer-1.2.0/src/lux/pyuid3/att_stats.py` & `lux_explainer-1.2.1/src/lux/pyuid3/att_stats.py`

 * *Files identical despite different names*

### Comparing `lux_explainer-1.2.0/src/lux/pyuid3/attribute.py` & `lux_explainer-1.2.1/src/lux/pyuid3/attribute.py`

 * *Files identical despite different names*

### Comparing `lux_explainer-1.2.0/src/lux/pyuid3/data.py` & `lux_explainer-1.2.1/src/lux/pyuid3/data.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,43 +10,79 @@
 import pandas as pd
 import numpy as np
 from pandas import DataFrame
 from typing import List, Set, Dict
 from typing import Tuple
 from collections import OrderedDict
 
+from .parse_exception import ParseException
 from .reading import Reading
 from .instance import Instance
 from .att_stats import AttStats
 from .attribute import Attribute
 from .value import Value
 
 
 # Cell
 class Data:
     REAL_DOMAIN = '@REAL'
 
     def __init__(self, name: str = None, attributes: List[Attribute] = None, instances: List[Instance] = None):
+        """ Initialize a Data object.
+
+                Parameters:
+                -----------
+                :param name: str, optional
+                    The name of the dataset.
+                :param attributes: List[Attribute], optional
+                    List of attribute objects defining the dataset's attributes.
+                :param instances: List[Instance], optional
+                    List of instance objects containing the dataset's instances.
+        """
         self.name = name
         self.instances = instances
         self.attributes = OrderedDict()
         self.expected_values = dict()
         for at in attributes:
             self.attributes[at.get_name()]=at
             
         if len(attributes) > 0:
             self.class_attribute_name = attributes[-1].get_name()
         else:
             self.class_attribute_name = None
         self.__df__=None
         
     def __len__(self):
+        """
+        Returns the number of instances in the dataset.
+
+        Returns:
+        --------
+        :return: int
+            The number of instances in the dataset.
+        """
         return len(self.instances)
 
     def filter_nominal_attribute_value(self, at: Attribute, value: str, copy : bool =False) -> 'Data':
+        """ Filter the dataset based on the given nominal attribute value.
+
+        Parameters:
+        -----------
+        :param at: Attribute
+            The attribute to filter.
+        :param value: str
+            The value to filter.
+        :param copy: bool, optional
+            Whether to create a copy of the filtered dataset. Defaults to False.
+
+        Returns:
+        --------
+        :return: Data
+            The filtered dataset.
+        """
         new_instances = []
         new_attributes = self.get_attributes().copy()
 
         for i in self.instances:
             reading = i.get_reading_for_attribute(at.get_name())
             instance_val = reading.get_most_probable().get_name()
             if str(instance_val) == str(value):
@@ -55,14 +91,32 @@
                 else:
                     new_instance = i
                 new_instances.append(new_instance)
 
         return Data(self.name, new_attributes, new_instances)
 
     def filter_numeric_attribute_value(self, at: Attribute, value: str, copy : bool = False )-> Tuple['Data','Data']:
+        """ Filter the dataset based on the given numeric attribute value.
+
+       Parameters:
+       -----------
+       :param at: Attribute
+           The attribute to filter.
+       :param value: str
+           The value to filter.
+       :param copy: bool, optional
+           Whether to create a copy of the filtered dataset. Defaults to False.
+
+       Returns:
+       --------
+       :return: Tuple[Data, Data]
+           A tuple containing two filtered datasets:
+           - The first dataset contains instances where the attribute value is less than the given value.
+           - The second dataset contains instances where the attribute value is greater than or equal to the given value.
+       """
         new_instances_less_than = []
         new_instances_greater_equal = []
         new_attributes_lt = self.get_attributes().copy()
         new_attributes_gt = self.get_attributes().copy()
         value = float(value)
         for i in self.instances:
             reading = i.get_reading_for_attribute(at.get_name())
@@ -76,14 +130,32 @@
                 new_instances_less_than.append(new_instance) 
             else:
                 new_instances_greater_equal.append(new_instance)
 
         return (Data(self.name, new_attributes_lt, new_instances_less_than),Data(self.name, new_attributes_gt, new_instances_greater_equal))
     
     def filter_numeric_attribute_value_expr(self, at: Attribute, expr: str, copy : bool = False )-> Tuple['Data','Data']:
+        """ Filter the dataset based on the given expression involving a numeric attribute value.
+
+        Parameters:
+        -----------
+        :param at: Attribute
+            The attribute to filter.
+        :param expr: str
+            The expression to evaluate. It can involve comparisons and arithmetic operations with the attribute value.
+        :param copy: bool, optional
+            Whether to create a copy of the filtered dataset. Defaults to False.
+
+        Returns:
+        --------
+        :return: Tuple[Data, Data]
+            A tuple containing two filtered datasets:
+            - The first dataset contains instances where the attribute value satisfies the expression.
+            - The second dataset contains instances where the attribute value does not satisfy the expression.
+        """
         new_instances_less_than = []
         new_instances_greater_equal = []
         new_attributes_lt = self.get_attributes().copy()
         new_attributes_gt = self.get_attributes().copy()
         
         for i in self.instances:
             reading = i.get_reading_for_attribute(at.get_name())
@@ -103,17 +175,37 @@
             else:
                 new_instances_greater_equal.append(new_instance)
 
         return (Data(self.name, new_attributes_lt, new_instances_less_than),Data(self.name, new_attributes_gt, new_instances_greater_equal))
     
 
     def get_attribute_of_name(self, att_name: str) -> Attribute:
+        """ Get the attribute object corresponding to the given attribute name.
+
+        Parameters:
+        -----------
+        :param att_name: str
+            The name of the attribute to retrieve.
+
+        Returns:
+        --------
+        :return: Attribute
+            The attribute object corresponding to the given attribute name.
+            Returns None if the attribute name is not found in the dataset.
+        """
         return self.attributes.get(att_name, None)
 
     def to_arff_most_probable(self) -> str:
+        """ Convert the dataset to ARFF format using the most probable values for each attribute.
+
+        Returns:
+        --------
+        :return: str
+            The dataset in ARFF format using the most probable values for each attribute.
+        """
         result = '@relation ' + self.name + '\n'
         for at in self.attributes:
             result += at.to_arff() + '\n'
 
         result += '@data\n'
 
         for i in self.instances:
@@ -121,14 +213,27 @@
                 result += r.get_most_probable().get_name()
                 result += ','
             result = result[:-1]  # delete the last coma ','
             result += '\n'
         return result
 
     def to_arff_skip_instance(self, epsilon: float) -> str:
+        """ Convert the dataset to ARFF format skipping instances where the confidence of the most probable value
+        is less than or equal to the given epsilon.
+
+        Parameters:
+        -----------
+        :param epsilon: float
+            The threshold confidence value. Instances with a confidence value less than or equal to epsilon will be skipped.
+
+        Returns:
+        --------
+        :return: str
+            The dataset in ARFF format skipping instances where the confidence of the most probable value is less than or equal to epsilon.
+        """
         result = '@relation ' + self.name + '\n'
         for at in self.attributes:
             result += at.to_arff() + '\n'
 
         result += '@data\n'
 
         for i in self.instances:
@@ -141,14 +246,26 @@
                 partial += ','
             result = result[:-1]  # delete the last coma ','
             result += partial + '\n'
 
         return result
 
     def to_arff_skip_value(self, epsilon: float) -> str:
+        """ Convert the dataset to ARFF format, replacing attribute values with '?' if their confidence is less than or equal to the given epsilon.
+
+        Parameters:
+        -----------
+        :param epsilon: float
+            The threshold confidence value. Attribute values with a confidence value less than or equal to epsilon will be replaced with '?'.
+
+        Returns:
+        --------
+        :return: str
+            The dataset in ARFF format with attribute values replaced with '?' if their confidence is less than or equal to epsilon.
+        """
         result = '@relation ' + self.name + '\n'
         for at in self.attributes:
             result += at.to_arff() + '\n'
 
         result += '@data\n'
 
         for i in self.instances:
@@ -161,104 +278,178 @@
                 partial += ','
             result = result[:-1]  # delete the last coma ','
             result += partial + '\n'
 
         return result
 
     def to_uarff(self) -> str:
+        """
+       Convert the dataset to UARFF (Uncertain ARFF) format.
+
+       Returns:
+       --------
+       :return: str
+           The dataset in UARFF format.
+       """
         result = '@relation ' + self.name + '\n'
         for at in self.attributes:
             result += at.to_arff() + '\n'
 
         result += '@data\n'
 
         for i in self.instances:
             result += i.to_arff() + '\n'
 
         return result
-    
+
     def to_dataframe(self,most_probable=True) -> pd.DataFrame:
+        """ Convert the dataset to a pandas DataFrame.
+
+        Parameters:
+        -----------
+        :param most_probable: bool, optional (default=True)
+            Whether to use the most probable values for each attribute. In current version there is no other option than True.
+
+        Returns:
+        --------
+        :return: pd.DataFrame
+            A pandas DataFrame representing the dataset.
+        """
         if self.__df__ is not None:
             return self.__df__
         columns = [at.get_name() for at in self.get_attributes()]
         values = []
         for i in self.instances:
             row =[]
             for att in columns:
-                ar = i.get_reading_for_attribute(att) 
+                ar = i.get_reading_for_attribute(att)
                 if self.get_attribute_of_name(att).get_type() == Attribute.TYPE_NOMINAL:
                     single_value = int(float(ar.get_most_probable().get_name()))
                 elif self.get_attribute_of_name(att).get_type() == Attribute.TYPE_NUMERICAL:
                     single_value = float(ar.get_most_probable().get_name())
                 row.append(single_value)
             values.append(row)
-    
+
         self.__df__ = pd.DataFrame(values, columns=columns)
         return self.__df__
-    
+
     def to_dataframe_importances(self, average_absolute=False):
+        """ Convert the dataset's importances to a pandas DataFrame.
+
+        Parameters:
+        -----------
+        :param average_absolute: bool, optional (default=False)
+            Whether to calculate the average absolute importances.
+
+        Returns:
+        --------
+        :return: pd.DataFrame
+            A pandas DataFrame representing the importances of each attribute.
+        """
         columns = [at.get_name() for at in self.get_attributes() if at.get_name() != self.class_attribute_name]
         values = []
         for i in self.instances:
             row =[]
             for att in columns:
-                ar = i.get_reading_for_attribute(att) 
+                ar = i.get_reading_for_attribute(att)
                 importances = list(ar.get_most_probable().get_importances().values())
                 row.append(importances)
             values.append(row)
-        
+
         result = np.array([sv for sv in np.moveaxis(np.array(values), 2,0)])
         if average_absolute:
             return np.abs(result).mean(1).mean(0)
         else:
             return result
 
     def calculate_statistics(self, att: Attribute) -> AttStats:
+        """ Calculate statistics for a specific attribute in the dataset.
+
+        Parameters:
+        -----------
+        :param att: Attribute
+            The attribute for which statistics are to be calculated.
+
+        Returns:
+        --------
+        :return: AttStats
+            An object containing statistics for the specified attribute.
+        """
         return AttStats.calculate_statistics(att, self)
-    
+
     def set_importances(self, importances: pd.DataFrame, expected_values: Dict) -> 'Data':
+        """ Set importances for each attribute based on the provided DataFrame of importances and expected values.
+
+        Parameters:
+        -----------
+        :param importances: pd.DataFrame
+            DataFrame containing importances for each attribute.
+        :param expected_values: Dict
+            Dictionary containing expected values.
+
+        Returns:
+        --------
+        :return: Data
+            A new Data object with updated importances.
+        """
         new_instances = []
         if type(importances.columns) is pd.MultiIndex:
             classes = list(importances.columns.get_level_values(0).unique())
         else:
             importances=pd.DataFrame({'__all__':importances})
             warnings.warn("WARNING: SHAP values passed for one class only. This may lead to unexpected behaviour.")
-         
+
         self.expected_values = expected_values
         for (_,r),instance in zip(importances.iterrows(), self.instances):
             new_readings = instance.get_readings().copy()
             for att in r.index.get_level_values(1).unique():
-                reading = instance.get_reading_for_attribute(att) 
+                reading = instance.get_reading_for_attribute(att)
                 importance_dict = {}
                 for cl in classes:
                     importance_dict[cl] = r[cl][att]
                 new_confidence_values = [Value(v.get_name(),v.get_confidence(), importance_dict) for v in reading.values]
                 altered_reading = Reading(reading.get_base_att(), new_confidence_values)
                 #use add_reading, as it will replace the previous one
                 new_instance = Instance(new_readings)
                 new_instance.add_reading(altered_reading)
             new_instances.append(new_instance)
-            
+
         return Data(self.name, self.get_attributes().copy(), new_instances)
-    
+
     def reduce_importance_for_attribute(self, att: Attribute, discount_factor: float, for_class : str = None) -> 'Data':
+        """ Reduce the importance of a specific attribute by a given discount factor.
+
+        Parameters:
+        -----------
+        :param att: Attribute
+            The attribute for which importance needs to be reduced.
+        :param discount_factor: float
+            The discount factor by which to reduce the importance.
+        :param for_class: str, optional (default=None)
+            If provided, reduce the importance only for the specified class.
+
+        Returns:
+        --------
+        :return: Data
+            A new Data object with reduced importance for the specified attribute.
+        """
         new_instances = []
         for i in self.instances:
             new_readings = i.get_readings().copy()
-            reading = i.get_reading_for_attribute(att.get_name()) 
+            reading = i.get_reading_for_attribute(att.get_name())
             if for_class is None:
                 discounted_confidence_values = [Value(v.get_name(),v.get_confidence(), {key: value * (1-discount_factor) for key, value in v.get_importances().items()}) for v in reading.values]
             else:
                 discounted_confidence_values = [Value(v.get_name(),v.get_confidence(), {key: value * (1-discount_factor) for key, value in v.get_importances().items() if key==for_class}) for v in reading.values]
             discounted_reading = Reading(reading.get_base_att(), discounted_confidence_values)
             #use add_reading, as it will replace the previous one
             new_instance = Instance(new_readings)
             new_instance.add_reading(discounted_reading)
             new_instances.append(new_instance)
-            
+
         return Data(self.name, self.get_attributes().copy(), new_instances)
 
     @staticmethod
     def __read_uarff_from_buffer(br: (TextIOWrapper, StringIO)) -> 'Data':
         atts = []
         insts = []
         name = br.readline().split('@relation')[1].strip()
@@ -329,37 +520,37 @@
 
     @staticmethod
     def parse_ucsv(filename: str) -> 'Data':
         df = pd.read_csv(filename)
         name = filename.split('/')[-1].split('.csv')[0]
         out = Data.__read_ucsv_from_dataframe(df, name)
         return out
-    
+
     @staticmethod
     def parse_dataframe(df: pd.DataFrame,name='uarff_data',categorical:List[bool]=None) -> 'Data':
         out = Data.__read_ucsv_from_dataframe(df, name,categorical)
         return out
 
     @staticmethod
     def __parse(temp_data: 'Data', class_id: (int, str)) -> 'Data':
         # if class name is given
         if isinstance(class_id, str):
             class_att_name = class_id
             class_att = temp_data.get_attribute_of_name(class_att_name)
         elif isinstance(class_id, int):
             class_att_name = list(temp_data.attributes.keys())[class_id]
-            class_att = temp_data.attributes[class_att]
+            class_att = temp_data.get_attribute_of_name[class_att_name]
 
         del temp_data.attributes[class_att_name]
         temp_data.attributes.append((class_att_name,class_att))
         # change order of reading for the att
         for i in temp_data.instances:
             class_label = i.get_reading_for_attribute(class_att.get_name())
             readings = i.get_readings()
-            del readings[class_index]
+            del readings[class_id]
             readings.append(class_label)
             i.set_readings(readings)
         return temp_data
 
     @staticmethod
     def parse_uarff_from_string(string: str, class_id: (int, str) = None) -> 'Data':
         try:
@@ -405,15 +596,15 @@
         type = Attribute.TYPE_NOMINAL
         name = att_def[0:name_boundary]
         domain = set()
         untrimmed_domain = re.sub(r'[{}]', '',  att_def[name_boundary:]).split(',')
         for value in untrimmed_domain:
             if value.strip() == Data.REAL_DOMAIN:
                 type = Attribute.TYPE_NUMERICAL
-                break 
+                break
             domain.add(value.replace("'", '').strip())
         return Attribute(name, domain, type)
 
     def get_instances(self) -> List[Instance]:
         return self.instances#.copy()
 
     def get_attributes(self) -> List[Attribute]:
```

### Comparing `lux_explainer-1.2.0/src/lux/pyuid3/data_scrambler.py` & `lux_explainer-1.2.1/src/lux/pyuid3/data_scrambler.py`

 * *Files identical despite different names*

### Comparing `lux_explainer-1.2.0/src/lux/pyuid3/entropy_evaluator.py` & `lux_explainer-1.2.1/src/lux/pyuid3/entropy_evaluator.py`

 * *Files identical despite different names*

### Comparing `lux_explainer-1.2.0/src/lux/pyuid3/instance.py` & `lux_explainer-1.2.1/src/lux/pyuid3/instance.py`

 * *Files identical despite different names*

### Comparing `lux_explainer-1.2.0/src/lux/pyuid3/reading.py` & `lux_explainer-1.2.1/src/lux/pyuid3/reading.py`

 * *Files identical despite different names*

### Comparing `lux_explainer-1.2.0/src/lux/pyuid3/tree.py` & `lux_explainer-1.2.1/src/lux/pyuid3/tree.py`

 * *Files identical despite different names*

### Comparing `lux_explainer-1.2.0/src/lux/pyuid3/tree_edge.py` & `lux_explainer-1.2.1/src/lux/pyuid3/tree_edge.py`

 * *Files identical despite different names*

### Comparing `lux_explainer-1.2.0/src/lux/pyuid3/tree_evaluator.py` & `lux_explainer-1.2.1/src/lux/pyuid3/tree_evaluator.py`

 * *Files identical despite different names*

### Comparing `lux_explainer-1.2.0/src/lux/pyuid3/tree_node.py` & `lux_explainer-1.2.1/src/lux/pyuid3/tree_node.py`

 * *Files identical despite different names*

### Comparing `lux_explainer-1.2.0/src/lux/pyuid3/uid3.py` & `lux_explainer-1.2.1/src/lux/pyuid3/uid3.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,46 @@
 
 # Cell
 class UId3(BaseEstimator):
     
     PARALLEL_ENTRY_FACTOR = 1000
 
     def __init__(self, max_depth=None, node_size_limit = 1, grow_confidence_threshold = 0, min_impurity_decrease=0):
+        """A decision tree classifier with customizable parameters for controlling tree growth.
+
+        Parameters:
+        -----------
+        :param max_depth: int or None, default=None
+            The maximum depth of the tree. If None, then nodes are expanded until all leaves are pure or until all leaves
+            contain less than `node_size_limit` samples.
+        :param node_size_limit: int, default=1
+            The minimum number of samples required to split a node further. If the number of samples at a node is less than
+            `node_size_limit`, the node is not split, and it becomes a leaf.
+        :param grow_confidence_threshold: float, default=0
+            The minimum confidence level required for a split to occur. Splits with a confidence level below this threshold
+            are not performed. Confidence level is typically defined by impurity measures such as Gini impurity or entropy.
+        :param min_impurity_decrease: float, default=0
+            The minimum decrease in impurity required for a split to occur. A split is only considered if it leads to at least
+            this amount of impurity decrease. If a split does not meet this criterion, it is not performed.
+
+        Attributes:
+        -----------
+        TREE_DEPTH_LIMIT: int or None
+            The maximum depth of the tree.
+        NODE_SIZE_LIMIT: int
+            The minimum number of samples required to split a node further.
+        GROW_CONFIDENCE_THRESHOLD: float
+            The minimum confidence level required for a split to occur.
+        tree: object or None
+            The decision tree model constructed after fitting the data.
+        node_size_limit: int
+            The minimum number of samples required to split a node further.
+        min_impurity_decrease: float
+            The minimum decrease in impurity required for a split to occur.
+        """
         self.TREE_DEPTH_LIMIT= max_depth
         self.NODE_SIZE_LIMIT = node_size_limit
         self.GROW_CONFIDENCE_THRESHOLD = grow_confidence_threshold
         self.tree = None
         self.node_size_limit = node_size_limit
         self.min_impurity_decrease=min_impurity_decrease
```

### Comparing `lux_explainer-1.2.0/src/lux/pyuid3/utils.py` & `lux_explainer-1.2.1/src/lux/pyuid3/utils.py`

 * *Files identical despite different names*

### Comparing `lux_explainer-1.2.0/src/lux/pyuid3/value.py` & `lux_explainer-1.2.1/src/lux/pyuid3/value.py`

 * *Files identical despite different names*

### Comparing `lux_explainer-1.2.0/src/lux/samplers.py` & `lux_explainer-1.2.1/src/lux/samplers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,101 @@
 # add smote and importance sampler__all__ = ['UncertainSMOTE']
 
+from sklearn.base import TransformerMixin, BaseEstimator
+import shap
+import pandas as pd
+
 from imblearn.over_sampling._smote.base import BaseSMOTE
 import numpy as np
 import warnings
 from scipy import sparse
-from sklearn.base import TransformerMixin, BaseEstimator
 from sklearn.utils import _safe_indexing, check_array, check_random_state
 from sklearn.metrics import pairwise_distances
-import shap
-import pandas as pd
 
 from sklearn.linear_model import LinearRegression
 import numdifftools as nd
 
 
 class ImportanceSampler(TransformerMixin, BaseEstimator):
+
     def __init__(self, classifier, predict_proba, indstance2explain,min_generate_samples):
+        """
+        A transformer class for generating synthetic data using importance sampling based on SHAP values.
+
+        Parameters:
+        -----------
+        :param classifier: object
+            The classifier used for generating SHAP values.
+        :type classifier: object
+        :param predict_proba: callable
+            A function returning probability estimates for samples.
+        :type predict_proba: callable
+        :param instance2explain: array-like of shape (n_features,)
+            An instance to be used for explaining the synthetic samples creation process.
+        :type instance2explain: array-like of shape (n_features,)
+        :param min_generate_samples: int
+            The minimum number of synthetic samples to generate.
+        :type min_generate_samples: int
+
+        """
         self.classifier = classifier
         self.predict_proba = predict_proba
         self.instance2explain = indstance2explain
         self.min_generate_samples=min_generate_samples
 
     def fit(self, X,y=None):
+        """ Fits the transformer by calculating SHAP values for the given dataset.
+
+            Parameters:
+            -----------
+            :param X: array-like of shape (n_samples, n_features)
+                The input data for which SHAP values are to be calculated.
+            :param y: array-like of shape (n_samples,), default=None
+                The target values. This parameter is not used and is only present to adhere to the scikit-learn transformer interface.
+
+            Returns:
+            --------
+            self: object
+                The fitted transformer instance.
+        """
         self.shap_values =  self.__getshap(X)
         return self
 
     def transform(self,X,y=None):
+        """ Transforms the dataset by generating synthetic samples based on SHAP values.
+
+        Parameters:
+        -----------
+        :param X: array-like of shape (n_samples, n_features)
+            The input data to be transformed.
+        :param y: array-like of shape (n_samples,), default=None
+            The target values. This parameter is not used and is only present to adhere to the scikit-learn transformer interface.
+
+        Returns:
+        --------
+        transformed_data: array-like of shape (n_samples_new, n_features)
+            The transformed dataset containing the original samples along with the generated synthetic samples.
+        """
         return self.__importance_sampler(X,self.instance_to_explain, num=10)
 
     def __getshap(self, X_train_sample):
-        """ Calculates SHAP values
+        """ Calculates SHAP values for the given dataset.
+
+            Parameters:
+            -----------
+            :param X_train_sample: array-like of shape (n_samples, n_features)
+                The input data for which SHAP values are to be calculated.
+
+            Returns:
+            --------
+            shap_values: list or array-like
+                The SHAP values calculated for each feature and sample in the dataset.
+            expected_values: list or array-like
+                The expected values of the SHAP values calculated for each feature and sample in the dataset.
 
-        :param X_train_sample:
-        :return:
         """
         # calculate shap values
         try:
             explainer = shap.Explainer(self.classifier, X_train_sample)
             if hasattr(explainer, "shap_values"):
                 shap_values = explainer.shap_values(X_train_sample, check_additivity=False)
             else:
@@ -96,18 +155,18 @@
 
         for cl in np.unique(indexer):
             gradcl = []
             for dim in range(0, X_train_sample.shape[1]):
                 mask = indexer == cl
                 xs = X_train_sample.iloc[mask, dim]
                 ys = shapclass[mask, dim]
-                svr = LinearRegression()  # SVR()
-                svr.fit(xs.values.reshape(-1, 1), ys)
+                svrc = LinearRegression()  # SVR()
+                svrc.fit(xs.values.reshape(-1, 1), ys)
 
-                F = lambda x, svr=svr: svr.predict(x.reshape(1, -1))
+                F = lambda x, svr=svrc: svr.predict(x.reshape(1, -1))
                 gradient = nd.Gradient(F)
 
                 gradcl.append(gradient)
             gradsf[cl] = gradcl
 
 
         alpha = abs(shapclass).mean()
@@ -153,27 +212,59 @@
             n_jobs=None,
             sigma=1,
             m_neighbors=10,
             min_samples=0.1,
             instance_to_explain=None,
             kind="borderline-1",
     ):
+        """An implementation of Synthetic Minority Over-sampling Technique (SMOTE) with handling of uncertain samples.
+            Parameters:
+            -----------
+            :param predict_proba: callable
+                A function returning probability estimates for samples.
+            :type predict_proba: callable
+            :param sampling_strategy: float, str, dict, or callable, default='all'
+                The sampling strategy to use. Can be a float representing the desired ratio of minority class samples over
+                the majority class samples after resampling, or one of {'all', 'not minority', 'minority'}. Alternatively, it
+                can be a dictionary where the keys represent the class labels and the values represent the desired number of
+                samples for each class, or a callable function returning a dictionary.
+            :type sampling_strategy: float, str, dict, or callable
+            :param random_state: int, RandomState instance or None, default=None
+                Controls the randomness of the algorithm.
+            :type random_state: int, RandomState instance or None
+            :param k_neighbors: int, default=5
+                Number of nearest neighbors to used to construct synthetic samples.
+            :type k_neighbors: int
+            :param n_jobs: int or None, default=None
+                Number of CPU cores used during the computation.
+            :type n_jobs: int or None
+            :param sigma: float, default=1
+                Parameter controlling the thresholding of confidence intervals for identifying uncertain samples.
+            :type sigma: float
+            :param m_neighbors: int, default=10
+                Number of nearest neighbors to consider when estimating if a sample is in danger.
+            :type m_neighbors: int
+            :param min_samples: float, default=0.1
+                Fraction of the maximum class samples to be added as additional synthetic samples.
+            :type min_samples: float
+            :param instance_to_explain: array-like of shape (n_features,) or None, default=None
+                An instance to be used for generating samples around.
+            :type instance_to_explain: array-like of shape (n_features,) or None
+            :param kind: {'borderline-1', 'borderline-2'}, default='borderline-1'
+                The kind of borderline samples to detect. If 'borderline-1', it identifies samples that are
+                borderline to a single class. If 'borderline-2', it identifies samples that are borderline to
+                multiple classes.
+            :type kind: {'borderline-1', 'borderline-2'}
+
+            Attributes:
+            -----------
+            :sampling_strategy_: dict
+                A dictionary containing the actual number of samples for each class after resampling.
         """
 
-        :param predict_proba:
-        :param sampling_strategy:
-        :param random_state:
-        :param k_neighbors:
-        :param n_jobs:
-        :param sigma:
-        :param m_neighbors:
-        :param min_samples:
-        :param instance_to_explain:
-        :param kind:
-        """
         super().__init__(
             sampling_strategy=sampling_strategy,
             random_state=random_state,
             k_neighbors=k_neighbors,
             n_jobs=n_jobs,
         )
         self.m_neighbors = m_neighbors
@@ -285,26 +376,24 @@
     def _in_danger_noise(self, predict_proba, samples, target_class, y, kind="danger"):
         """
         Estimate if a set of sample are in danger or noise.
         :param predict_proba:
            function returning probability estimates for samples
         :param samples: {array-like, sparse matrix} of shape (n_samples, n_features).
            The samples to check if either they are in danger or not.
-        :param target_class: int or str.
+        :param target_class: nt or str.
            The target corresponding class being over-sampled.
         :param y: array-like of shape (n_samples,).
            The true label in order to check the neighbour labels.
-        :param kind:
-           {'danger', 'noise'}, default='danger'
+        :param kind: {'danger', 'noise'}, default='danger'
             The type of classification to use. Can be either:
             - If 'danger', check if samples are in danger,
             - If 'noise', check if samples are noise.
 
-        :return: ndarray of shape (n_samples,).
-           A boolean array where True refer to samples in danger or noise.
+        :return: ndarray of shape (n_samples,). A boolean array where True refer to samples in danger or noise.
         """
 
         c_labels = samples[np.argmax(self.predict_proba(samples), axis=1) == target_class]
         prediction_certainty = np.max(self.predict_proba(c_labels), axis=1)
 
         # shuld this be thresholded like that, or keep n-lowest?
         confidence_threshold = np.mean(prediction_certainty) - self.sigma * np.std(
```

### Comparing `lux_explainer-1.2.0/src/lux_explainer.egg-info/PKG-INFO` & `lux_explainer-1.2.1/src/lux_explainer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lux-explainer
-Version: 1.2.0
+Version: 1.2.1
 Summary: Universal Local Rule-based Explainer
 Author-email: Szymon Bobek <szymon.bobek@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 sbobek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,14 +45,17 @@
 Requires-Dist: shap>=0.41.0
 Requires-Dist: lime>=0.2.0.1
 Requires-Dist: anchor-exp>=0.0.2.0
 Requires-Dist: imbalanced-learn>=0.9.1
 Requires-Dist: gower>=0.1.2
 Requires-Dist: numdifftools>=0.9.41
 
+[![PyPI](https://img.shields.io/pypi/v/lux-explainer)](https://pypi.org/project/lux-explainer/)  ![License](https://img.shields.io/github/license/sbobek/lux)
+ ![PyPI - Downloads](https://img.shields.io/pypi/dm/lux-explainer) [![Documentation Status](https://readthedocs.org/projects/lux-explainer/badge/?version=latest)](https://tsproto.readthedocs.io/en/latest/?badge=latest)
+   
 # LUX (Local Universal Rule-based Explainer)
 ## Main features
   <img align="right"  src="https://raw.githubusercontent.com/sbobek/lux/main/pix/lux-logo.png" width="200">
   
   * Model-agnostic, rule-based and visual local explanations of black-box ML models
   * Integrated counterfactual explanations
   * Rule-based explanations (that are executable at the same time)
@@ -157,15 +160,17 @@
 You can obtain a whole rule-based model for the local uncertain explanation that was generated by LUX for given instance by running following code
 
 ``` python
 #have a look at the entire rule-based model that can be executed with https:://heartdroid.re
 print(lux.to_HMR())
 ```
 
-This will generate model which can later be executed by [HeaRTDroid](https://heartdroid.re)
+This will generate model which can later be executed by [HeaRTDroid](https://heartdroid.re) which is rule-based inference engine for Android mobile devices.
+Additionally, the HMR format below, which is used by  [HeaRTDroid](https://heartdroid.re) allows visualization of explanations in a format of decision tables with [HWEd](https://heartdroid.re/hwed/#/) online editor.
+
 
 ```
 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%% TYPES DEFINITIONS %%%%%%%%%%%%%%%%%%%%%%%%%%
 
 xtype [
  name: petal_length, 
 base:numeric,
@@ -209,17 +214,19 @@
 
 The code should yield something like that (depending on the instance that was selected):
 
 ![](https://raw.githubusercontent.com/sbobek/lux/main/pix/utree.png)
 
 # Cite this work
 
+The software is the direct implementation of a method described in the following paper:
+
 ```
 @misc{bobek2023local,
-      title={Local Universal Rule-based Explanations}, 
+      title={Local Universal Explainer ({LUX}) -- a rule-based explainer with factual, counterfactual and visual explanations}, 
       author={Szymon Bobek and Grzegorz J. Nalepa},
       year={2023},
       eprint={2310.14894},
       archivePrefix={arXiv},
       primaryClass={cs.AI}
 
 }
```

### Comparing `lux_explainer-1.2.0/src/lux_explainer.egg-info/SOURCES.txt` & `lux_explainer-1.2.1/src/lux_explainer.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-src/lux/UncertainSMOTE.py
 src/lux/__init__.py
 src/lux/lux.py
 src/lux/metrics.py
 src/lux/samplers.py
 src/lux/pyuid3/__init__.py
 src/lux/pyuid3/att_stats.py
 src/lux/pyuid3/attribute.py
```

