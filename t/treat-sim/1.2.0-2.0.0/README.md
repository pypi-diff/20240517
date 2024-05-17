# Comparing `tmp/treat_sim-1.2.0.tar.gz` & `tmp/treat_sim-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treat_sim-1.2.0.tar", last modified: Wed May  8 10:57:28 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `treat_sim-1.2.0.tar` & `treat_sim-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,9 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:57:28.296830 treat_sim-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-08 10:57:24.000000 treat_sim-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 10:57:24.000000 treat_sim-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-08 10:57:28.296830 treat_sim-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-08 10:57:24.000000 treat_sim-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 10:57:24.000000 treat_sim-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 10:57:28.296830 treat_sim-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-08 10:57:24.000000 treat_sim-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:57:28.296830 treat_sim-1.2.0/treat_sim/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 10:57:24.000000 treat_sim-1.2.0/treat_sim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:57:28.296830 treat_sim-1.2.0/treat_sim/data/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-08 10:57:24.000000 treat_sim-1.2.0/treat_sim/data/ed_arrivals.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-08 10:57:24.000000 treat_sim-1.2.0/treat_sim/distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    38343 2024-05-08 10:57:24.000000 treat_sim-1.2.0/treat_sim/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:57:28.296830 treat_sim-1.2.0/treat_sim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-08 10:57:28.000000 treat_sim-1.2.0/treat_sim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-08 10:57:28.000000 treat_sim-1.2.0/treat_sim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:57:28.000000 treat_sim-1.2.0/treat_sim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 10:57:28.000000 treat_sim-1.2.0/treat_sim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 10:57:28.000000 treat_sim-1.2.0/treat_sim.egg-info/top_level.txt
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 treat_sim-2.0.0/treat_sim/__init__.py
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 treat_sim-2.0.0/treat_sim/distributions.py
+-rw-r--r--   0        0        0    38601 2020-02-02 00:00:00.000000 treat_sim-2.0.0/treat_sim/model.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 treat_sim-2.0.0/treat_sim/data/ed_arrivals.csv
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 treat_sim-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 treat_sim-2.0.0/LICENSE
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 treat_sim-2.0.0/README.md
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 treat_sim-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7933 2020-02-02 00:00:00.000000 treat_sim-2.0.0/PKG-INFO
```

### Comparing `treat_sim-1.2.0/LICENSE` & `treat_sim-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `treat_sim-1.2.0/PKG-INFO` & `treat_sim-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: treat-sim
-Version: 1.2.0
-Summary: A free and open implementation of the Treatment Centre Model from Nelson (2013)
-Home-page: https://github.com/pythonhealthdatascience/stars-treat-sim
-Author: Thomas Monks
-Author-email: forecast-tools@gmail.com
-License: The MIT License (MIT)
+Version: 2.0.0
+Summary: A Python Free and Open Source Software implementation of the Treatment Centre Model from Nelson (2013)
+Project-URL: Homepage, https://github.com/pythonhealthdatascience/stars-treat-sim
+Project-URL: Bug Tracker, https://github.com/pythonhealthdatascience/stars-treat-sim
+Project-URL: Documentation, https://pythonhealthdatascience.github.io/stars-simpy-example-docs/
+Author-email: Thomas Monks <forecast-tools@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8.19
 Requires-Dist: matplotlib>=3.3.4
 Requires-Dist: numpy>=1.19.2
 Requires-Dist: pandas>=1.2.3
 Requires-Dist: scipy>=1.6.1
 Requires-Dist: simpy>=4.0.1
+Description-Content-Type: text/markdown
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pythonhealthdatascience/stars-treat-sim/HEAD)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380+/)
+[![Python](https://img.shields.io/pypi/pyversions/treat_sim)](https://pypi.org/project/treat_sim/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10026326.svg)](https://doi.org/10.5281/zenodo.10026326)
 [![PyPI version fury.io](https://badge.fury.io/py/treat-sim.svg)](https://pypi.org/project/treat-sim/)
 
+
 [<img src="https://img.shields.io/static/v1?label=dockerhub&message=images&color=important?style=for-the-badge&logo=docker">](https://hub.docker.com/r/tommonks01/treat_sim)
 
 
 # Towards Sharing Tools, and Artifacts, for Reusable Simulation: a minimal model example
 
 ## Overview
```

### Comparing `treat_sim-1.2.0/README.md` & `treat_sim-2.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pythonhealthdatascience/stars-treat-sim/HEAD)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380+/)
+[![Python](https://img.shields.io/pypi/pyversions/treat_sim)](https://pypi.org/project/treat_sim/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10026326.svg)](https://doi.org/10.5281/zenodo.10026326)
 [![PyPI version fury.io](https://badge.fury.io/py/treat-sim.svg)](https://pypi.org/project/treat-sim/)
 
+
 [<img src="https://img.shields.io/static/v1?label=dockerhub&message=images&color=important?style=for-the-badge&logo=docker">](https://hub.docker.com/r/tommonks01/treat_sim)
 
 
 # Towards Sharing Tools, and Artifacts, for Reusable Simulation: a minimal model example
 
 ## Overview
```

### Comparing `treat_sim-1.2.0/treat_sim/distributions.py` & `treat_sim-2.0.0/treat_sim/distributions.py`

 * *Files 5% similar despite different names*

```diff
@@ -135,16 +135,18 @@
         return self.rng.lognormal(self.mu, self.sigma)
 
 
 class Normal:
     '''
     Convenience class for the normal distribution.
     packages up distribution parameters, seed and random generator.
+
+    Use the minimum parameter to truncate the distribution
     '''
-    def __init__(self, mean, sigma, random_seed=None):
+    def __init__(self, mean, sigma, minimum=None, random_seed=None):
         '''
         Constructor
         
         Params:
         ------
         mean: float
             The mean of the normal distribution
@@ -155,26 +157,37 @@
         random_seed: int, optional (default=None)
             A random seed to reproduce samples.  If set to none then a unique
             sample is created.
         '''
         self.rng = np.random.default_rng(seed=random_seed)
         self.mean = mean
         self.sigma = sigma
+        self.minimum = minimum
         
     def sample(self, size=None):
         '''
         Generate a sample from the normal distribution
         
         Params:
         -------
         size: int, optional (default=None)
             the number of samples to return.  If size=None then a single
             sample is returned.
         '''
-        return self.rng.normal(self.mean, self.sigma, size=size)
+        samples = self.rng.normal(self.mean, self.sigma, size=size)
+
+        if self.minimum is None:
+            return samples
+        elif size is None:
+            return max(self.minimum, samples)
+        else:
+            # index of samples with negative value
+            neg_idx = np.where(samples < 0)[0]
+            samples[neg_idx] = self.minimum
+            return samples
 
     
 class Uniform():
     '''
     Convenience class for the Uniform distribution.
     packages up distribution parameters, seed and random generator.
     '''
```

### Comparing `treat_sim-1.2.0/treat_sim/model.py` & `treat_sim-2.0.0/treat_sim/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 # registration parameters
 DEFAULT_REG_MEAN = 5.0
 DEFAULT_REG_VAR= 2.0
 
 # examination parameters
 DEFAULT_EXAM_MEAN = 16.0
 DEFAULT_EXAM_VAR = 3.0
+DEFAULT_EXAM_MIN = 0.5
 
 # trauma/stabilisation
 DEFAULT_TRAUMA_MEAN = 90.0
 
 # Trauma treatment
 DEFAULT_TRAUMA_TREAT_MEAN = 30.0
 DEFAULT_TRAUMA_TREAT_VAR = 4.0
@@ -174,14 +175,15 @@
                  n_cubicles_1=DEFAULT_N_CUBICLES_1,
                  n_cubicles_2=DEFAULT_N_CUBICLES_2,
                  triage_mean=DEFAULT_TRIAGE_MEAN,
                  reg_mean=DEFAULT_REG_MEAN,
                  reg_var=DEFAULT_REG_VAR,
                  exam_mean=DEFAULT_EXAM_MEAN,
                  exam_var=DEFAULT_EXAM_VAR,
+                 exam_min=DEFAULT_EXAM_MIN,
                  trauma_mean=DEFAULT_TRAUMA_MEAN,
                  trauma_treat_mean=DEFAULT_TRAUMA_TREAT_MEAN,
                  trauma_treat_var=DEFAULT_TRAUMA_TREAT_VAR,
                  non_trauma_treat_mean=DEFAULT_NON_TRAUMA_TREAT_MEAN,
                  non_trauma_treat_var=DEFAULT_NON_TRAUMA_TREAT_VAR,
                  non_trauma_treat_p=DEFAULT_NON_TRAUMA_TREAT_P,
                  prob_trauma=DEFAULT_PROB_TRAUMA):
@@ -222,14 +224,17 @@
             Variance of the registration distribution (Lognormal)
             
         exam_mean: float
             Mean of the examination distribution (Normal)
             
         exam_var: float
             Variance of the examination distribution (Normal)
+
+        exam_min: float
+            The minimum value that an examination can take (Truncated Normal)
             
         trauma_mean: float
             Mean of the trauma stabilisation distribution (Exponential)
             
         trauma_treat_mean: float
             Mean of the trauma cubicle treatment distribution (Lognormal)
             
@@ -253,14 +258,15 @@
         
         # store parameters for sampling
         self.triage_mean = triage_mean
         self.reg_mean = reg_mean
         self.reg_var = reg_var
         self.exam_mean= exam_mean
         self.exam_var = exam_var
+        self.exam_min = exam_min
         self.trauma_mean = trauma_mean
         self.trauma_treat_mean = trauma_treat_mean
         self.trauma_treat_var = trauma_treat_var
         self.non_trauma_treat_mean = non_trauma_treat_mean
         self.non_trauma_treat_var = non_trauma_treat_var
         self.non_trauma_treat_p = non_trauma_treat_p
         self.prob_trauma = prob_trauma
@@ -318,14 +324,15 @@
         self.reg_dist = Lognormal(self.reg_mean, 
                                   np.sqrt(self.reg_var),
                                   random_seed=self.seeds[1])
         
         # Evaluation (non-trauma only)
         self.exam_dist = Normal(self.exam_mean,
                                 np.sqrt(self.exam_var),
+                                minimum=self.exam_min,
                                 random_seed=self.seeds[2])
         
         # Trauma/stablisation duration (trauma only)
         self.trauma_dist = Exponential(self.trauma_mean, 
                                        random_seed=self.seeds[3])
         
         # Non-trauma treatment
```

