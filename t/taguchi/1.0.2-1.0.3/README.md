# Comparing `tmp/taguchi-1.0.2.tar.gz` & `tmp/taguchi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taguchi-1.0.2.tar", last modified: Thu May  9 03:48:17 2024, max compression
+gzip compressed data, was "taguchi-1.0.3.tar", last modified: Fri May 17 20:50:28 2024, max compression
```

## Comparing `taguchi-1.0.2.tar` & `taguchi-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-09 03:48:17.894682 taguchi-1.0.2/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       29 2024-05-09 03:46:44.000000 taguchi-1.0.2/MANIFEST.in
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4216 2024-05-09 03:48:17.894682 taguchi-1.0.2/PKG-INFO
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     3786 2024-05-09 03:35:22.000000 taguchi-1.0.2/README.md
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      103 2024-05-04 04:45:54.000000 taguchi-1.0.2/pyproject.toml
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      757 2024-05-09 03:48:17.895682 taguchi-1.0.2/setup.cfg
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-09 03:48:17.888682 taguchi-1.0.2/taguchi/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       17 2024-05-09 03:47:23.000000 taguchi-1.0.2/taguchi/__init__.py
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     2721 2024-05-09 03:20:06.000000 taguchi-1.0.2/taguchi/__main__.py
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)   126954 2024-05-09 02:16:59.000000 taguchi-1.0.2/taguchi/database.json
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-09 03:48:17.893682 taguchi-1.0.2/taguchi.egg-info/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4216 2024-05-09 03:48:17.000000 taguchi-1.0.2/taguchi.egg-info/PKG-INFO
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      296 2024-05-09 03:48:17.000000 taguchi-1.0.2/taguchi.egg-info/SOURCES.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-09 03:48:17.000000 taguchi-1.0.2/taguchi.egg-info/dependency_links.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       54 2024-05-09 03:48:17.000000 taguchi-1.0.2/taguchi.egg-info/entry_points.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-04 04:46:44.000000 taguchi-1.0.2/taguchi.egg-info/not-zip-safe
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        8 2024-05-09 03:48:17.000000 taguchi-1.0.2/taguchi.egg-info/top_level.txt
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-17 20:50:28.461237 taguchi-1.0.3/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       29 2024-05-09 03:46:44.000000 taguchi-1.0.3/MANIFEST.in
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4216 2024-05-17 20:50:28.461237 taguchi-1.0.3/PKG-INFO
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     3786 2024-05-09 03:35:22.000000 taguchi-1.0.3/README.md
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      103 2024-05-04 04:45:54.000000 taguchi-1.0.3/pyproject.toml
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      757 2024-05-17 20:50:28.462237 taguchi-1.0.3/setup.cfg
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-17 20:50:28.458237 taguchi-1.0.3/taguchi/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       17 2024-05-17 20:34:26.000000 taguchi-1.0.3/taguchi/__init__.py
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     3329 2024-05-17 20:49:51.000000 taguchi-1.0.3/taguchi/__main__.py
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)   126984 2024-05-17 20:49:28.000000 taguchi-1.0.3/taguchi/database.json
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-17 20:50:28.460237 taguchi-1.0.3/taguchi.egg-info/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4216 2024-05-17 20:50:28.000000 taguchi-1.0.3/taguchi.egg-info/PKG-INFO
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      296 2024-05-17 20:50:28.000000 taguchi-1.0.3/taguchi.egg-info/SOURCES.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-17 20:50:28.000000 taguchi-1.0.3/taguchi.egg-info/dependency_links.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       54 2024-05-17 20:50:28.000000 taguchi-1.0.3/taguchi.egg-info/entry_points.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-04 04:46:44.000000 taguchi-1.0.3/taguchi.egg-info/not-zip-safe
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        8 2024-05-17 20:50:28.000000 taguchi-1.0.3/taguchi.egg-info/top_level.txt
```

### Comparing `taguchi-1.0.2/PKG-INFO` & `taguchi-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taguchi
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool for optimising systems parameterised by environment variables, based on Taguchi/orthogonal array systems of experiments.
 Home-page: https://github.com/jcranney/taguchi
 Author: Jesse Cranney
 Author-email: jesse.cranney@anu.edu.au
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `taguchi-1.0.2/README.md` & `taguchi-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `taguchi-1.0.2/setup.cfg` & `taguchi-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `taguchi-1.0.2/taguchi/__main__.py` & `taguchi-1.0.3/taguchi/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,28 +18,35 @@
 
 with open("./taguchi.yaml","r") as f:
     a : dict = yaml.full_load(f)
 
 command = a.pop("command")
 
 params = []
+static_params = []
 for param in list(a.keys()):
     if len(a[param])==0:
         if verbose: 
             print(f"empty param: {param}, skipping it.")
         continue
     if len(a[param])==1:
         os.environ[param] = str(a[param][0])
         if verbose:
             print(f"param {param} has only one value, setting to {str(a[param][0])}")
+        static_params.append(param)
         continue
     params.append(param)
 
 n_params = len(params)
-n_states = len(a[params[0]])
+if n_params > 0:
+    n_states = len(a[params[0]])
+else:
+    n_states = 0 # to get here, we must have static parameters only (if anything)
+                 # I realise that n_states makes more sense as "1" but let's have
+                 # n_states = 0 => all static params
 for param in params:
     if len(a[param]) != n_states:
         raise ValueError("All parameters must have the same number of states (for now)")
 
 filename = resources.files("taguchi")/"database.json"
 
 with open(filename,"r") as f:
@@ -52,14 +59,15 @@
 
 if verbose:
     print(f"Doing {len(array)} experiments in total!\n")
 if verbose > 1:
     print("Experiments:")
     print(array)
 
+
 results = []
 for experiment in array:
     for param,state in zip(params,experiment):
         os.environ[param] = str(a[param][state])
         if verbose:
             print(param,state)
     proc = subprocess.Popen(command, stdout=subprocess.PIPE, shell=True)
@@ -81,17 +89,26 @@
         except ValueError:
             pass
     if result is None:
         raise ValueError("No number found in output of command")
     
     results.append(result)
 
+if len(params) > 0:
+    print("\n`````` VARIABLE PARAMS ``````")
 for j,param in enumerate(params):
     print(f"{param:12s}")
     for i,state in enumerate(a[param]):
         res = 0.0
         n_experiment = 0
         for k,experiment in enumerate(array):
             if experiment[j]==i:
                 res += results[k]
                 n_experiment += 1
-        print(f"{state:12} : {res/n_experiment:12f}")
+        print(f"{state:12} : {res/n_experiment:12f}")
+
+if len(static_params) > 0:
+    print("\n``````  STATIC PARAMS  ``````")
+for j,param in enumerate(static_params):
+    print(f"{param:12s}")
+    for i,state in enumerate(a[param]):
+        print(f"{state:12} : {sum(results)/len(results):12f}")
```

### Comparing `taguchi-1.0.2/taguchi/database.json` & `taguchi-1.0.3/taguchi/database.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9743589743589743%*

 * *Differences: {"'0,0'": '[[]]', "'1,2'": '[[0], [1]]'}*

```diff
@@ -1,8 +1,19 @@
 {
+    "0,0": [
+        []
+    ],
+    "1,2": [
+        [
+            0
+        ],
+        [
+            1
+        ]
+    ],
     "10,2": [
         [
             1,
             0,
             0,
             0,
             1,
```

### Comparing `taguchi-1.0.2/taguchi.egg-info/PKG-INFO` & `taguchi-1.0.3/taguchi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taguchi
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool for optimising systems parameterised by environment variables, based on Taguchi/orthogonal array systems of experiments.
 Home-page: https://github.com/jcranney/taguchi
 Author: Jesse Cranney
 Author-email: jesse.cranney@anu.edu.au
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

