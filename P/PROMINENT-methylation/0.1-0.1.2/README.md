# Comparing `tmp/PROMINENT_methylation-0.1.tar.gz` & `tmp/PROMINENT_methylation-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PROMINENT_methylation-0.1.tar", last modified: Fri May 17 08:13:17 2024, max compression
+gzip compressed data, was "PROMINENT_methylation-0.1.2.tar", last modified: Fri May 17 09:04:43 2024, max compression
```

## Comparing `PROMINENT_methylation-0.1.tar` & `PROMINENT_methylation-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 laz64    (157829) hpark    (16579)        0 2024-05-17 08:13:17.111811 PROMINENT_methylation-0.1/
--rw-r--r--   0 laz64    (157829) hpark    (16579)      287 2024-05-17 08:13:17.110867 PROMINENT_methylation-0.1/PKG-INFO
-drwxr-xr-x   0 laz64    (157829) hpark    (16579)        0 2024-05-17 08:13:17.079010 PROMINENT_methylation-0.1/PROMINENT_methylation/
--rw-r--r--   0 laz64    (157829) hpark    (16579)     1489 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1/PROMINENT_methylation/dataprep.py
--rw-r--r--   0 laz64    (157829) hpark    (16579)     2775 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1/PROMINENT_methylation/interpret.py
--rwxr-xr-x   0 laz64    (157829) hpark    (16579)     7051 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1/PROMINENT_methylation/model.py
--rw-r--r--   0 laz64    (157829) hpark    (16579)     3426 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1/PROMINENT_methylation/scores.py
--rwxr-xr-x   0 laz64    (157829) hpark    (16579)    56770 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1/PROMINENT_methylation/train.py
--rw-r--r--   0 laz64    (157829) hpark    (16579)     3394 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1/PROMINENT_methylation/train_test.py
--rwxr-xr-x   0 laz64    (157829) hpark    (16579)     1586 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1/PROMINENT_methylation/utils.py
-drwxr-xr-x   0 laz64    (157829) hpark    (16579)        0 2024-05-17 08:13:17.105414 PROMINENT_methylation-0.1/PROMINENT_methylation.egg-info/
--rw-r--r--   0 laz64    (157829) hpark    (16579)      287 2024-05-17 08:13:16.000000 PROMINENT_methylation-0.1/PROMINENT_methylation.egg-info/PKG-INFO
--rw-r--r--   0 laz64    (157829) hpark    (16579)      520 2024-05-17 08:13:16.000000 PROMINENT_methylation-0.1/PROMINENT_methylation.egg-info/SOURCES.txt
--rw-r--r--   0 laz64    (157829) hpark    (16579)        1 2024-05-17 08:13:16.000000 PROMINENT_methylation-0.1/PROMINENT_methylation.egg-info/dependency_links.txt
--rw-r--r--   0 laz64    (157829) hpark    (16579)      287 2024-05-17 08:13:16.000000 PROMINENT_methylation-0.1/PROMINENT_methylation.egg-info/entry_points.txt
--rw-r--r--   0 laz64    (157829) hpark    (16579)       72 2024-05-17 08:13:16.000000 PROMINENT_methylation-0.1/PROMINENT_methylation.egg-info/requires.txt
--rw-r--r--   0 laz64    (157829) hpark    (16579)       22 2024-05-17 08:13:16.000000 PROMINENT_methylation-0.1/PROMINENT_methylation.egg-info/top_level.txt
--rw-r--r--   0 laz64    (157829) hpark    (16579)       24 2024-05-17 07:22:16.000000 PROMINENT_methylation-0.1/README.md
--rw-r--r--   0 laz64    (157829) hpark    (16579)       38 2024-05-17 08:13:17.112960 PROMINENT_methylation-0.1/setup.cfg
--rw-r--r--   0 laz64    (157829) hpark    (16579)     1078 2024-05-17 08:00:18.000000 PROMINENT_methylation-0.1/setup.py
+drwxr-xr-x   0 laz64    (157829) hpark    (16579)        0 2024-05-17 09:04:43.702788 PROMINENT_methylation-0.1.2/
+-rw-r--r--   0 laz64    (157829) hpark    (16579)      289 2024-05-17 09:04:43.701033 PROMINENT_methylation-0.1.2/PKG-INFO
+drwxr-xr-x   0 laz64    (157829) hpark    (16579)        0 2024-05-17 09:04:43.618284 PROMINENT_methylation-0.1.2/PROMINENT_methylation/
+-rw-r--r--   0 laz64    (157829) hpark    (16579)     1489 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.2/PROMINENT_methylation/dataprep.py
+-rw-r--r--   0 laz64    (157829) hpark    (16579)     2775 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.2/PROMINENT_methylation/interpret.py
+-rwxr-xr-x   0 laz64    (157829) hpark    (16579)     7051 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.2/PROMINENT_methylation/model.py
+-rw-r--r--   0 laz64    (157829) hpark    (16579)     3426 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.2/PROMINENT_methylation/scores.py
+-rwxr-xr-x   0 laz64    (157829) hpark    (16579)    56770 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.2/PROMINENT_methylation/train.py
+-rw-r--r--   0 laz64    (157829) hpark    (16579)     3394 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.2/PROMINENT_methylation/train_test.py
+-rwxr-xr-x   0 laz64    (157829) hpark    (16579)     1586 2024-05-17 07:21:16.000000 PROMINENT_methylation-0.1.2/PROMINENT_methylation/utils.py
+drwxr-xr-x   0 laz64    (157829) hpark    (16579)        0 2024-05-17 09:04:43.686913 PROMINENT_methylation-0.1.2/PROMINENT_methylation.egg-info/
+-rw-r--r--   0 laz64    (157829) hpark    (16579)      289 2024-05-17 09:04:43.000000 PROMINENT_methylation-0.1.2/PROMINENT_methylation.egg-info/PKG-INFO
+-rw-r--r--   0 laz64    (157829) hpark    (16579)      520 2024-05-17 09:04:43.000000 PROMINENT_methylation-0.1.2/PROMINENT_methylation.egg-info/SOURCES.txt
+-rw-r--r--   0 laz64    (157829) hpark    (16579)        1 2024-05-17 09:04:43.000000 PROMINENT_methylation-0.1.2/PROMINENT_methylation.egg-info/dependency_links.txt
+-rw-r--r--   0 laz64    (157829) hpark    (16579)      287 2024-05-17 09:04:43.000000 PROMINENT_methylation-0.1.2/PROMINENT_methylation.egg-info/entry_points.txt
+-rw-r--r--   0 laz64    (157829) hpark    (16579)       65 2024-05-17 09:04:43.000000 PROMINENT_methylation-0.1.2/PROMINENT_methylation.egg-info/requires.txt
+-rw-r--r--   0 laz64    (157829) hpark    (16579)       22 2024-05-17 09:04:43.000000 PROMINENT_methylation-0.1.2/PROMINENT_methylation.egg-info/top_level.txt
+-rw-r--r--   0 laz64    (157829) hpark    (16579)       24 2024-05-17 07:22:16.000000 PROMINENT_methylation-0.1.2/README.md
+-rw-r--r--   0 laz64    (157829) hpark    (16579)       38 2024-05-17 09:04:43.704727 PROMINENT_methylation-0.1.2/setup.cfg
+-rw-r--r--   0 laz64    (157829) hpark    (16579)     1048 2024-05-17 09:04:34.000000 PROMINENT_methylation-0.1.2/setup.py
```

### Comparing `PROMINENT_methylation-0.1/PROMINENT_methylation/dataprep.py` & `PROMINENT_methylation-0.1.2/PROMINENT_methylation/dataprep.py`

 * *Files identical despite different names*

### Comparing `PROMINENT_methylation-0.1/PROMINENT_methylation/interpret.py` & `PROMINENT_methylation-0.1.2/PROMINENT_methylation/interpret.py`

 * *Files identical despite different names*

### Comparing `PROMINENT_methylation-0.1/PROMINENT_methylation/model.py` & `PROMINENT_methylation-0.1.2/PROMINENT_methylation/model.py`

 * *Files identical despite different names*

### Comparing `PROMINENT_methylation-0.1/PROMINENT_methylation/scores.py` & `PROMINENT_methylation-0.1.2/PROMINENT_methylation/scores.py`

 * *Files identical despite different names*

### Comparing `PROMINENT_methylation-0.1/PROMINENT_methylation/train.py` & `PROMINENT_methylation-0.1.2/PROMINENT_methylation/train.py`

 * *Files identical despite different names*

### Comparing `PROMINENT_methylation-0.1/PROMINENT_methylation/train_test.py` & `PROMINENT_methylation-0.1.2/PROMINENT_methylation/train_test.py`

 * *Files identical despite different names*

### Comparing `PROMINENT_methylation-0.1/PROMINENT_methylation/utils.py` & `PROMINENT_methylation-0.1.2/PROMINENT_methylation/utils.py`

 * *Files identical despite different names*

### Comparing `PROMINENT_methylation-0.1/PROMINENT_methylation.egg-info/SOURCES.txt` & `PROMINENT_methylation-0.1.2/PROMINENT_methylation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PROMINENT_methylation-0.1/setup.py` & `PROMINENT_methylation-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='PROMINENT_methylation',
-    version='0.1',
+    version='0.1.2',
     packages=['PROMINENT_methylation'],
     description='PROMINENT: AN INTERPRETABLE DEEP LEARNING METHOD TO PREDICT PHENOTYPES USING DNA METHYLATION',
     url='https://github.com/cloudmacchiato/dlmethylation',
     author='Laizhi Zhang',
     author_email='laz64@pitt.edu',
     license='MIT',
     entry_points={
@@ -17,14 +17,13 @@
             'PROMINENT-model_interpret = PROMINENT_methylation.interpret:get_feature_importance'
         ]
     },
     install_requires=['numpy',
                       'pandas',
                       'scikit-learn',
                       'shap',
-                      'pickle',
                       'seaborn',
                       'matplotlib',
                       'torch',
                       'imblearn'
     ]
 )
```

