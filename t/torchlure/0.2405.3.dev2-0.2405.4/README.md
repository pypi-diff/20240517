# Comparing `tmp/torchlure-0.2405.3.dev2.tar.gz` & `tmp/torchlure-0.2405.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlure-0.2405.3.dev2.tar", last modified: Fri May 17 10:47:24 2024, max compression
+gzip compressed data, was "torchlure-0.2405.4.tar", last modified: Fri May 17 11:11:29 2024, max compression
```

## Comparing `torchlure-0.2405.3.dev2.tar` & `torchlure-0.2405.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.077067 torchlure-0.2405.3.dev2/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      133 2024-04-19 13:30:09.000000 torchlure-0.2405.3.dev2/.gitignore
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        7 2024-04-19 12:37:01.000000 torchlure-0.2405.3.dev2/.python-version
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/.vscode/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      520 2024-05-17 10:31:16.000000 torchlure-0.2405.3.dev2/.vscode/extensions.json
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      208 2024-05-17 10:31:16.000000 torchlure-0.2405.3.dev2/.vscode/settings.json
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1277 2024-05-17 10:47:24.077067 torchlure-0.2405.3.dev2/PKG-INFO
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      785 2024-05-17 10:38:19.000000 torchlure-0.2405.3.dev2/README.md
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1044 2024-05-17 10:31:30.000000 torchlure-0.2405.3.dev2/pyproject.toml
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       38 2024-05-17 10:47:24.077067 torchlure-0.2405.3.dev2/setup.cfg
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      939 2024-05-15 16:17:28.000000 torchlure-0.2405.3.dev2/setup.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/src/
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/src/torchlure/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      189 2024-05-17 10:47:18.000000 torchlure-0.2405.3.dev2/src/torchlure/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/src/torchlure/datasets/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       46 2024-05-17 10:45:02.000000 torchlure-0.2405.3.dev2/src/torchlure/datasets/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/src/torchlure/datasets/d4rl/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     5509 2024-05-17 10:46:29.000000 torchlure-0.2405.3.dev2/src/torchlure/datasets/d4rl/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/src/torchlure/datasets/offline_rl/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     4105 2024-05-17 10:47:01.000000 torchlure-0.2405.3.dev2/src/torchlure/datasets/offline_rl/__init__.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    11374 2024-05-15 18:42:40.000000 torchlure-0.2405.3.dev2/src/torchlure/datasets/offline_rl/minari_ext.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/src/torchlure/functional/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     3567 2024-04-19 13:10:24.000000 torchlure-0.2405.3.dev2/src/torchlure/functional/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/src/torchlure/modules/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1272 2024-04-25 08:19:27.000000 torchlure-0.2405.3.dev2/src/torchlure/modules/__init__.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2894 2024-04-19 13:40:26.000000 torchlure-0.2405.3.dev2/src/torchlure/noise_schedulers.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       31 2024-04-19 12:53:51.000000 torchlure-0.2405.3.dev2/src/torchlure/optim.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1481 2024-04-19 12:49:22.000000 torchlure-0.2405.3.dev2/src/torchlure/utils.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/src/torchlure.egg-info/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1277 2024-05-17 10:47:24.000000 torchlure-0.2405.3.dev2/src/torchlure.egg-info/PKG-INFO
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      636 2024-05-17 10:47:24.000000 torchlure-0.2405.3.dev2/src/torchlure.egg-info/SOURCES.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        1 2024-05-17 10:47:24.000000 torchlure-0.2405.3.dev2/src/torchlure.egg-info/dependency_links.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       86 2024-05-17 10:47:24.000000 torchlure-0.2405.3.dev2/src/torchlure.egg-info/requires.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       10 2024-05-17 10:47:24.000000 torchlure-0.2405.3.dev2/src/torchlure.egg-info/top_level.txt
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      133 2024-04-19 13:30:09.000000 torchlure-0.2405.4/.gitignore
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        7 2024-04-19 12:37:01.000000 torchlure-0.2405.4/.python-version
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/.vscode/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      520 2024-05-17 10:31:16.000000 torchlure-0.2405.4/.vscode/extensions.json
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      208 2024-05-17 10:31:16.000000 torchlure-0.2405.4/.vscode/settings.json
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1904 2024-05-17 11:11:29.397067 torchlure-0.2405.4/PKG-INFO
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1417 2024-05-17 11:11:16.000000 torchlure-0.2405.4/README.md
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1044 2024-05-17 10:31:30.000000 torchlure-0.2405.4/pyproject.toml
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       38 2024-05-17 11:11:29.397067 torchlure-0.2405.4/setup.cfg
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      939 2024-05-15 16:17:28.000000 torchlure-0.2405.4/setup.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.387067 torchlure-0.2405.4/src/
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/src/torchlure/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      184 2024-05-17 11:07:37.000000 torchlure-0.2405.4/src/torchlure/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/src/torchlure/datasets/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       46 2024-05-17 10:45:02.000000 torchlure-0.2405.4/src/torchlure/datasets/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/src/torchlure/datasets/d4rl/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     5564 2024-05-17 11:10:50.000000 torchlure-0.2405.4/src/torchlure/datasets/d4rl/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/src/torchlure/datasets/offline_rl/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     4105 2024-05-17 10:47:01.000000 torchlure-0.2405.4/src/torchlure/datasets/offline_rl/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    11374 2024-05-15 18:42:40.000000 torchlure-0.2405.4/src/torchlure/datasets/offline_rl/minari_ext.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/src/torchlure/functional/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     3567 2024-04-19 13:10:24.000000 torchlure-0.2405.4/src/torchlure/functional/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/src/torchlure/modules/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1272 2024-04-25 08:19:27.000000 torchlure-0.2405.4/src/torchlure/modules/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2894 2024-04-19 13:40:26.000000 torchlure-0.2405.4/src/torchlure/noise_schedulers.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       31 2024-04-19 12:53:51.000000 torchlure-0.2405.4/src/torchlure/optim.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1481 2024-04-19 12:49:22.000000 torchlure-0.2405.4/src/torchlure/utils.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/src/torchlure.egg-info/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1904 2024-05-17 11:11:29.000000 torchlure-0.2405.4/src/torchlure.egg-info/PKG-INFO
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      636 2024-05-17 11:11:29.000000 torchlure-0.2405.4/src/torchlure.egg-info/SOURCES.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        1 2024-05-17 11:11:29.000000 torchlure-0.2405.4/src/torchlure.egg-info/dependency_links.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       86 2024-05-17 11:11:29.000000 torchlure-0.2405.4/src/torchlure.egg-info/requires.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       10 2024-05-17 11:11:29.000000 torchlure-0.2405.4/src/torchlure.egg-info/top_level.txt
```

### Comparing `torchlure-0.2405.3.dev2/.vscode/extensions.json` & `torchlure-0.2405.4/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev2/pyproject.toml` & `torchlure-0.2405.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev2/setup.py` & `torchlure-0.2405.4/setup.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev2/src/torchlure/datasets/d4rl/__init__.py` & `torchlure-0.2405.4/src/torchlure/datasets/d4rl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,36 +103,39 @@
     print(f"Dataset '{dataset_id}' created successfully.")
 
 
 class D4RLDataset(Dataset):
     def __init__(
         self,
         dataset_id: str,
-        dataset_name: Literal[
-            "d4rl_halfcheetah-expert-v2",
-            "d4rl_hopper-expert-v2",
-            "d4rl_walker2d-expert-v2",
-        ],
+        d4rl_name: (
+            Literal[
+                "d4rl_halfcheetah-expert-v2",
+                "d4rl_hopper-expert-v2",
+                "d4rl_walker2d-expert-v2",
+            ]
+            | None
+        ) = None,
         env_id: str | None = None,
     ):
 
         try:
-            dataset = minari.load_dataset(dataset_name)
+            dataset = minari.load_dataset(dataset_id)
             self.dataset = dataset
             return
         except:
             pass
 
-        download_d4rl_dataset(dataset_name=dataset_name)
+        download_d4rl_dataset(dataset_name=d4rl_name)
 
         # Initialize the environment
         env = gym.make(env_id)
 
         # Get the path to the HDF5 file
-        data_path = Path.home() / ".minari" / "datasets" / dataset_name / "data"
+        data_path = Path.home() / ".minari" / "datasets" / d4rl_name / "data"
         if not data_path.exists():
             raise FileNotFoundError(f"Data path does not exist: {data_path}")
 
         # Initialize HDF5Storage
         storage = HDF5Storage(data_path, env.observation_space, env.action_space)
 
         # Collect all episodes
```

### Comparing `torchlure-0.2405.3.dev2/src/torchlure/datasets/offline_rl/__init__.py` & `torchlure-0.2405.4/src/torchlure/datasets/offline_rl/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev2/src/torchlure/datasets/offline_rl/minari_ext.py` & `torchlure-0.2405.4/src/torchlure/datasets/offline_rl/minari_ext.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev2/src/torchlure/functional/__init__.py` & `torchlure-0.2405.4/src/torchlure/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev2/src/torchlure/modules/__init__.py` & `torchlure-0.2405.4/src/torchlure/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev2/src/torchlure/noise_schedulers.py` & `torchlure-0.2405.4/src/torchlure/noise_schedulers.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev2/src/torchlure/utils.py` & `torchlure-0.2405.4/src/torchlure/utils.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev2/src/torchlure.egg-info/SOURCES.txt` & `torchlure-0.2405.4/src/torchlure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

