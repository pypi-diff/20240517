# Comparing `tmp/torchlure-0.2405.3.dev1.tar.gz` & `tmp/torchlure-0.2405.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlure-0.2405.3.dev1.tar", last modified: Fri May 17 10:45:26 2024, max compression
+gzip compressed data, was "torchlure-0.2405.3.dev2.tar", last modified: Fri May 17 10:47:24 2024, max compression
```

## Comparing `torchlure-0.2405.3.dev1.tar` & `torchlure-0.2405.3.dev2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:45:26.687068 torchlure-0.2405.3.dev1/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      133 2024-04-19 13:30:09.000000 torchlure-0.2405.3.dev1/.gitignore
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        7 2024-04-19 12:37:01.000000 torchlure-0.2405.3.dev1/.python-version
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:45:26.687068 torchlure-0.2405.3.dev1/.vscode/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      520 2024-05-17 10:31:16.000000 torchlure-0.2405.3.dev1/.vscode/extensions.json
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      208 2024-05-17 10:31:16.000000 torchlure-0.2405.3.dev1/.vscode/settings.json
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1277 2024-05-17 10:45:26.687068 torchlure-0.2405.3.dev1/PKG-INFO
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      785 2024-05-17 10:38:19.000000 torchlure-0.2405.3.dev1/README.md
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1044 2024-05-17 10:31:30.000000 torchlure-0.2405.3.dev1/pyproject.toml
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       38 2024-05-17 10:45:26.687068 torchlure-0.2405.3.dev1/setup.cfg
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      939 2024-05-15 16:17:28.000000 torchlure-0.2405.3.dev1/setup.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:45:26.687068 torchlure-0.2405.3.dev1/src/
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:45:26.687068 torchlure-0.2405.3.dev1/src/torchlure/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      189 2024-05-17 10:45:17.000000 torchlure-0.2405.3.dev1/src/torchlure/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:45:26.687068 torchlure-0.2405.3.dev1/src/torchlure/datasets/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       46 2024-05-17 10:45:02.000000 torchlure-0.2405.3.dev1/src/torchlure/datasets/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:45:26.687068 torchlure-0.2405.3.dev1/src/torchlure/datasets/d4rl/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     5509 2024-05-17 10:31:22.000000 torchlure-0.2405.3.dev1/src/torchlure/datasets/d4rl/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:45:26.687068 torchlure-0.2405.3.dev1/src/torchlure/datasets/offline_rl/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     4135 2024-05-17 10:44:35.000000 torchlure-0.2405.3.dev1/src/torchlure/datasets/offline_rl/__init__.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    11374 2024-05-15 18:42:40.000000 torchlure-0.2405.3.dev1/src/torchlure/datasets/offline_rl/minari_ext.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:45:26.687068 torchlure-0.2405.3.dev1/src/torchlure/functional/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     3567 2024-04-19 13:10:24.000000 torchlure-0.2405.3.dev1/src/torchlure/functional/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:45:26.687068 torchlure-0.2405.3.dev1/src/torchlure/modules/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1272 2024-04-25 08:19:27.000000 torchlure-0.2405.3.dev1/src/torchlure/modules/__init__.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2894 2024-04-19 13:40:26.000000 torchlure-0.2405.3.dev1/src/torchlure/noise_schedulers.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       31 2024-04-19 12:53:51.000000 torchlure-0.2405.3.dev1/src/torchlure/optim.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1481 2024-04-19 12:49:22.000000 torchlure-0.2405.3.dev1/src/torchlure/utils.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:45:26.687068 torchlure-0.2405.3.dev1/src/torchlure.egg-info/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1277 2024-05-17 10:45:26.000000 torchlure-0.2405.3.dev1/src/torchlure.egg-info/PKG-INFO
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      636 2024-05-17 10:45:26.000000 torchlure-0.2405.3.dev1/src/torchlure.egg-info/SOURCES.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        1 2024-05-17 10:45:26.000000 torchlure-0.2405.3.dev1/src/torchlure.egg-info/dependency_links.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       86 2024-05-17 10:45:26.000000 torchlure-0.2405.3.dev1/src/torchlure.egg-info/requires.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       10 2024-05-17 10:45:26.000000 torchlure-0.2405.3.dev1/src/torchlure.egg-info/top_level.txt
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.077067 torchlure-0.2405.3.dev2/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      133 2024-04-19 13:30:09.000000 torchlure-0.2405.3.dev2/.gitignore
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        7 2024-04-19 12:37:01.000000 torchlure-0.2405.3.dev2/.python-version
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/.vscode/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      520 2024-05-17 10:31:16.000000 torchlure-0.2405.3.dev2/.vscode/extensions.json
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      208 2024-05-17 10:31:16.000000 torchlure-0.2405.3.dev2/.vscode/settings.json
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1277 2024-05-17 10:47:24.077067 torchlure-0.2405.3.dev2/PKG-INFO
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      785 2024-05-17 10:38:19.000000 torchlure-0.2405.3.dev2/README.md
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1044 2024-05-17 10:31:30.000000 torchlure-0.2405.3.dev2/pyproject.toml
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       38 2024-05-17 10:47:24.077067 torchlure-0.2405.3.dev2/setup.cfg
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      939 2024-05-15 16:17:28.000000 torchlure-0.2405.3.dev2/setup.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/src/
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/src/torchlure/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      189 2024-05-17 10:47:18.000000 torchlure-0.2405.3.dev2/src/torchlure/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/src/torchlure/datasets/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       46 2024-05-17 10:45:02.000000 torchlure-0.2405.3.dev2/src/torchlure/datasets/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/src/torchlure/datasets/d4rl/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     5509 2024-05-17 10:46:29.000000 torchlure-0.2405.3.dev2/src/torchlure/datasets/d4rl/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/src/torchlure/datasets/offline_rl/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     4105 2024-05-17 10:47:01.000000 torchlure-0.2405.3.dev2/src/torchlure/datasets/offline_rl/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    11374 2024-05-15 18:42:40.000000 torchlure-0.2405.3.dev2/src/torchlure/datasets/offline_rl/minari_ext.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/src/torchlure/functional/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     3567 2024-04-19 13:10:24.000000 torchlure-0.2405.3.dev2/src/torchlure/functional/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/src/torchlure/modules/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1272 2024-04-25 08:19:27.000000 torchlure-0.2405.3.dev2/src/torchlure/modules/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2894 2024-04-19 13:40:26.000000 torchlure-0.2405.3.dev2/src/torchlure/noise_schedulers.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       31 2024-04-19 12:53:51.000000 torchlure-0.2405.3.dev2/src/torchlure/optim.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1481 2024-04-19 12:49:22.000000 torchlure-0.2405.3.dev2/src/torchlure/utils.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:47:24.067067 torchlure-0.2405.3.dev2/src/torchlure.egg-info/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1277 2024-05-17 10:47:24.000000 torchlure-0.2405.3.dev2/src/torchlure.egg-info/PKG-INFO
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      636 2024-05-17 10:47:24.000000 torchlure-0.2405.3.dev2/src/torchlure.egg-info/SOURCES.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        1 2024-05-17 10:47:24.000000 torchlure-0.2405.3.dev2/src/torchlure.egg-info/dependency_links.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       86 2024-05-17 10:47:24.000000 torchlure-0.2405.3.dev2/src/torchlure.egg-info/requires.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       10 2024-05-17 10:47:24.000000 torchlure-0.2405.3.dev2/src/torchlure.egg-info/top_level.txt
```

### Comparing `torchlure-0.2405.3.dev1/.vscode/extensions.json` & `torchlure-0.2405.3.dev2/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev1/PKG-INFO` & `torchlure-0.2405.3.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlure
-Version: 0.2405.3.dev1
+Version: 0.2405.3.dev2
 Author-email: fuyutarow <fuyutarow@gmail.com>
 Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure
 Keywords: pytorch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchlure Version: 0.2405.3.dev1 Author-email:
+Metadata-Version: 2.1 Name: torchlure Version: 0.2405.3.dev2 Author-email:
 fuyutarow
 gmail.com> Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure Keywords:
 pytorch Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1 Requires-Dist: numpy>=1.26.4 Requires-Dist: sophia-
 opt>=0.2.2 Requires-Dist: gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28
 Requires-Dist: gdown>=5.2.0 # Torch Lure _[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip
```

### Comparing `torchlure-0.2405.3.dev1/README.md` & `torchlure-0.2405.3.dev2/README.md`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev1/pyproject.toml` & `torchlure-0.2405.3.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev1/setup.py` & `torchlure-0.2405.3.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev1/src/torchlure/datasets/d4rl/__init__.py` & `torchlure-0.2405.3.dev2/src/torchlure/datasets/d4rl/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev1/src/torchlure/datasets/offline_rl/__init__.py` & `torchlure-0.2405.3.dev2/src/torchlure/datasets/offline_rl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import time
 
 import gymnasium as gym
 import minari
 from torch.utils.data import DataLoader, Dataset
 
-from .minari_ext import AsyncDataCollector, D4RLDataset
+from .minari_ext import *
 
 
 async def collect_episode(env, policy=None):
     """Collect a single episode using the specified environment and policy."""
     env.reset()
     done = False
     while not done:
```

### Comparing `torchlure-0.2405.3.dev1/src/torchlure/datasets/offline_rl/minari_ext.py` & `torchlure-0.2405.3.dev2/src/torchlure/datasets/offline_rl/minari_ext.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev1/src/torchlure/functional/__init__.py` & `torchlure-0.2405.3.dev2/src/torchlure/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev1/src/torchlure/modules/__init__.py` & `torchlure-0.2405.3.dev2/src/torchlure/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev1/src/torchlure/noise_schedulers.py` & `torchlure-0.2405.3.dev2/src/torchlure/noise_schedulers.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev1/src/torchlure/utils.py` & `torchlure-0.2405.3.dev2/src/torchlure/utils.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.3.dev1/src/torchlure.egg-info/PKG-INFO` & `torchlure-0.2405.3.dev2/src/torchlure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlure
-Version: 0.2405.3.dev1
+Version: 0.2405.3.dev2
 Author-email: fuyutarow <fuyutarow@gmail.com>
 Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure
 Keywords: pytorch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchlure Version: 0.2405.3.dev1 Author-email:
+Metadata-Version: 2.1 Name: torchlure Version: 0.2405.3.dev2 Author-email:
 fuyutarow
 gmail.com> Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure Keywords:
 pytorch Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1 Requires-Dist: numpy>=1.26.4 Requires-Dist: sophia-
 opt>=0.2.2 Requires-Dist: gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28
 Requires-Dist: gdown>=5.2.0 # Torch Lure _[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip
```

### Comparing `torchlure-0.2405.3.dev1/src/torchlure.egg-info/SOURCES.txt` & `torchlure-0.2405.3.dev2/src/torchlure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

