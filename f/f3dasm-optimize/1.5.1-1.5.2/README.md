# Comparing `tmp/f3dasm_optimize-1.5.1.tar.gz` & `tmp/f3dasm_optimize-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f3dasm_optimize-1.5.1.tar", last modified: Tue Apr 23 11:21:07 2024, max compression
+gzip compressed data, was "f3dasm_optimize-1.5.2.tar", last modified: Fri May 17 14:01:58 2024, max compression
```

## Comparing `f3dasm_optimize-1.5.1.tar` & `f3dasm_optimize-1.5.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-23 11:21:07.161931 f3dasm_optimize-1.5.1/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1511 2023-06-14 13:02:10.000000 f3dasm_optimize-1.5.1/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-06-14 13:00:50.000000 f3dasm_optimize-1.5.1/MANIFEST.in
--rw-r--r--   0 martin    (1000) martin    (1000)     4187 2024-04-23 11:21:07.161931 f3dasm_optimize-1.5.1/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     2912 2023-11-17 22:45:34.000000 f3dasm_optimize-1.5.1/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)        5 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.1/VERSION
--rw-rw-r--   0 martin    (1000) martin    (1000)      100 2023-06-14 13:00:50.000000 f3dasm_optimize-1.5.1/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-11-17 22:45:34.000000 f3dasm_optimize-1.5.1/requirements.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       74 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.1/requirements_all.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     1185 2024-04-23 11:21:07.161931 f3dasm_optimize-1.5.1/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-23 11:21:07.157931 f3dasm_optimize-1.5.1/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-23 11:21:07.157931 f3dasm_optimize-1.5.1/src/f3dasm_optimize/
--rw-rw-r--   0 martin    (1000) martin    (1000)      716 2023-11-17 22:45:34.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-23 11:21:07.157931 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2572 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4197 2023-11-17 22:45:34.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/_imports.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1331 2023-11-30 15:22:34.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/_protocol.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-23 11:21:07.157931 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-02 02:36:58.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2495 2023-11-30 15:22:34.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/evosax_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1631 2023-11-30 15:22:34.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/nevergrad_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1648 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/optax_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3893 2024-02-07 15:48:24.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/optuna_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4509 2023-11-30 15:22:34.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/pygmo_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4056 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/tensorflow_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2661 2024-02-23 19:54:12.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/evosax_optimizers.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3024 2024-02-23 19:54:30.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/nevergrad_optimizers.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2263 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/optax_optimizers.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5783 2024-02-23 20:03:23.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/optimizer.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      932 2024-02-23 19:59:00.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/optuna_optimizers.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     9380 2024-02-23 20:03:07.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/pygmo_optimizers.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     6548 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/tensorflow_optimizers.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-23 11:21:07.161931 f3dasm_optimize-1.5.1/src/f3dasm_optimize.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)     4187 2024-04-23 11:21:07.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     1188 2024-04-23 11:21:07.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2024-04-23 11:21:07.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      102 2024-04-23 11:21:07.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       16 2024-04-23 11:21:07.000000 f3dasm_optimize-1.5.1/src/f3dasm_optimize.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 14:01:58.228110 f3dasm_optimize-1.5.2/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1511 2023-06-14 13:02:10.000000 f3dasm_optimize-1.5.2/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-06-14 13:00:50.000000 f3dasm_optimize-1.5.2/MANIFEST.in
+-rw-r--r--   0 martin    (1000) martin    (1000)     4194 2024-05-17 14:01:58.228110 f3dasm_optimize-1.5.2/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2912 2023-11-17 22:45:34.000000 f3dasm_optimize-1.5.2/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)        5 2024-05-17 13:55:26.000000 f3dasm_optimize-1.5.2/VERSION
+-rw-rw-r--   0 martin    (1000) martin    (1000)      100 2023-06-14 13:00:50.000000 f3dasm_optimize-1.5.2/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-11-17 22:45:34.000000 f3dasm_optimize-1.5.2/requirements.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       81 2024-05-17 13:55:26.000000 f3dasm_optimize-1.5.2/requirements_all.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1185 2024-05-17 14:01:58.228110 f3dasm_optimize-1.5.2/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 14:01:58.220111 f3dasm_optimize-1.5.2/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 14:01:58.220111 f3dasm_optimize-1.5.2/src/f3dasm_optimize/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      716 2023-11-17 22:45:34.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 14:01:58.224110 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2572 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4197 2023-11-17 22:45:34.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/_imports.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1330 2024-05-17 13:55:26.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/_protocol.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 14:01:58.224110 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/adapters/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-02 02:36:58.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/adapters/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2495 2023-11-30 15:22:34.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/adapters/evosax_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1631 2023-11-30 15:22:34.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/adapters/nevergrad_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1648 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/adapters/optax_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3893 2024-02-07 15:48:24.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/adapters/optuna_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4459 2024-05-17 13:55:26.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/adapters/pygmo_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4056 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/adapters/tensorflow_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2661 2024-02-23 19:54:12.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/evosax_optimizers.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3024 2024-02-23 19:54:30.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/nevergrad_optimizers.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2263 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/optax_optimizers.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5783 2024-02-23 20:03:23.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/optimizer.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      932 2024-02-23 19:59:00.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/optuna_optimizers.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9380 2024-02-23 20:03:07.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/pygmo_optimizers.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6548 2024-04-23 11:19:25.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/tensorflow_optimizers.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 14:01:58.224110 f3dasm_optimize-1.5.2/src/f3dasm_optimize.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)     4194 2024-05-17 14:01:58.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1188 2024-05-17 14:01:58.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2024-05-17 14:01:58.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      109 2024-05-17 14:01:58.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       16 2024-05-17 14:01:58.000000 f3dasm_optimize-1.5.2/src/f3dasm_optimize.egg-info/top_level.txt
```

### Comparing `f3dasm_optimize-1.5.1/LICENSE` & `f3dasm_optimize-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/PKG-INFO` & `f3dasm_optimize-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f3dasm_optimize
-Version: 1.5.1
+Version: 1.5.2
 Summary: f3dasm_optimize: Your one line description of the package
 Home-page: https://github.com/bessagroup/f3dasm_optimize
 Author: Martin van der Schelling
 Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD-3-Clause License
 Keywords: keyword1,keyword2,keyword3
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,15 +23,15 @@
 Requires-Dist: f3dasm>=1.4.5
 Provides-Extra: all
 Requires-Dist: tensorflow; extra == "all"
 Requires-Dist: pygmo; platform_system == "Linux" and extra == "all"
 Requires-Dist: nevergrad; extra == "all"
 Requires-Dist: evosax; extra == "all"
 Requires-Dist: optuna; extra == "all"
-Requires-Dist: optax; extra == "all"
+Requires-Dist: optax==0.1.7; extra == "all"
 
 f3dasm_optimize
 ---------------
 *Optimization extension package for the framework for data-driven design \& analysis of structures and materials*
 
 ***
```

### Comparing `f3dasm_optimize-1.5.1/README.md` & `f3dasm_optimize-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/setup.cfg` & `f3dasm_optimize-1.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/__init__.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/__init__.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/_imports.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/_imports.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/_protocol.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/_protocol.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 #
 # =============================================================================
 
 
 class Domain(Protocol):
     """Protocol class for the domain"""
 
-    def get_continuous_parameters(self):
+    @property
+    def continuous(self):
         ...
 
 
 class ExperimentSample(Protocol):
     def to_numpy(self) -> Tuple[np.ndarray, np.ndarray]:
         ...
```

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/evosax_implementations.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/adapters/evosax_implementations.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/nevergrad_implementations.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/adapters/nevergrad_implementations.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/optax_implementations.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/adapters/optax_implementations.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/optuna_implementations.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/adapters/optuna_implementations.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/pygmo_implementations.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/adapters/pygmo_implementations.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,19 +84,17 @@
 
         Returns
         -------
             box constraints
         """
         return (
             [parameter.lower_bound
-             for parameter in self.domain.get_continuous_parameters(
-             ).values()],
+             for parameter in self.domain.continuous.space.values()],
             [parameter.upper_bound
-             for parameter in self.domain.get_continuous_parameters(
-             ).values()],
+             for parameter in self.domain.continuous.space.values()],
         )
 
 
 class PygmoAlgorithm(Optimizer):
     """Wrapper around the pygmo algorithm class
 
     Parameters
```

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/adapters/tensorflow_implementations.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/adapters/tensorflow_implementations.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/evosax_optimizers.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/evosax_optimizers.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/nevergrad_optimizers.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/nevergrad_optimizers.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/optax_optimizers.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/optax_optimizers.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/optimizer.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/optimizer.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/optuna_optimizers.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/optuna_optimizers.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/pygmo_optimizers.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/pygmo_optimizers.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize/_src/tensorflow_optimizers.py` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize/_src/tensorflow_optimizers.py`

 * *Files identical despite different names*

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize.egg-info/PKG-INFO` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f3dasm_optimize
-Version: 1.5.1
+Version: 1.5.2
 Summary: f3dasm_optimize: Your one line description of the package
 Home-page: https://github.com/bessagroup/f3dasm_optimize
 Author: Martin van der Schelling
 Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD-3-Clause License
 Keywords: keyword1,keyword2,keyword3
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,15 +23,15 @@
 Requires-Dist: f3dasm>=1.4.5
 Provides-Extra: all
 Requires-Dist: tensorflow; extra == "all"
 Requires-Dist: pygmo; platform_system == "Linux" and extra == "all"
 Requires-Dist: nevergrad; extra == "all"
 Requires-Dist: evosax; extra == "all"
 Requires-Dist: optuna; extra == "all"
-Requires-Dist: optax; extra == "all"
+Requires-Dist: optax==0.1.7; extra == "all"
 
 f3dasm_optimize
 ---------------
 *Optimization extension package for the framework for data-driven design \& analysis of structures and materials*
 
 ***
```

### Comparing `f3dasm_optimize-1.5.1/src/f3dasm_optimize.egg-info/SOURCES.txt` & `f3dasm_optimize-1.5.2/src/f3dasm_optimize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

