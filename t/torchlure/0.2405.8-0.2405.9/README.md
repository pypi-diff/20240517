# Comparing `tmp/torchlure-0.2405.8.tar.gz` & `tmp/torchlure-0.2405.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlure-0.2405.8.tar", last modified: Fri May 17 15:39:33 2024, max compression
+gzip compressed data, was "torchlure-0.2405.9.tar", last modified: Fri May 17 15:44:24 2024, max compression
```

## Comparing `torchlure-0.2405.8.tar` & `torchlure-0.2405.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      133 2024-04-19 13:30:09.000000 torchlure-0.2405.8/.gitignore
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        7 2024-04-19 12:37:01.000000 torchlure-0.2405.8/.python-version
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/.vscode/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      520 2024-05-17 10:31:16.000000 torchlure-0.2405.8/.vscode/extensions.json
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      208 2024-05-17 10:31:16.000000 torchlure-0.2405.8/.vscode/settings.json
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1805 2024-05-17 15:39:33.747067 torchlure-0.2405.8/PKG-INFO
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1290 2024-05-17 11:41:15.000000 torchlure-0.2405.8/README.md
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1064 2024-05-17 15:37:36.000000 torchlure-0.2405.8/pyproject.toml
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       38 2024-05-17 15:39:33.747067 torchlure-0.2405.8/setup.cfg
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      939 2024-05-15 16:17:28.000000 torchlure-0.2405.8/setup.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.737067 torchlure-0.2405.8/src/
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/src/torchlure/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      184 2024-05-17 15:39:20.000000 torchlure-0.2405.8/src/torchlure/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/src/torchlure/datasets/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       46 2024-05-17 10:45:02.000000 torchlure-0.2405.8/src/torchlure/datasets/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/src/torchlure/datasets/d4rl/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     7075 2024-05-17 15:37:12.000000 torchlure-0.2405.8/src/torchlure/datasets/d4rl/__init__.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    22657 2024-05-17 11:28:16.000000 torchlure-0.2405.8/src/torchlure/datasets/d4rl/d4rl_infos.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/src/torchlure/datasets/offline_rl/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     4105 2024-05-17 10:47:01.000000 torchlure-0.2405.8/src/torchlure/datasets/offline_rl/__init__.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    11374 2024-05-15 18:42:40.000000 torchlure-0.2405.8/src/torchlure/datasets/offline_rl/minari_ext.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/src/torchlure/functional/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     3567 2024-04-19 13:10:24.000000 torchlure-0.2405.8/src/torchlure/functional/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/src/torchlure/modules/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1272 2024-04-25 08:19:27.000000 torchlure-0.2405.8/src/torchlure/modules/__init__.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2894 2024-04-19 13:40:26.000000 torchlure-0.2405.8/src/torchlure/noise_schedulers.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       31 2024-04-19 12:53:51.000000 torchlure-0.2405.8/src/torchlure/optim.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1481 2024-04-19 12:49:22.000000 torchlure-0.2405.8/src/torchlure/utils.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/src/torchlure.egg-info/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1805 2024-05-17 15:39:33.000000 torchlure-0.2405.8/src/torchlure.egg-info/PKG-INFO
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      678 2024-05-17 15:39:33.000000 torchlure-0.2405.8/src/torchlure.egg-info/SOURCES.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        1 2024-05-17 15:39:33.000000 torchlure-0.2405.8/src/torchlure.egg-info/dependency_links.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       99 2024-05-17 15:39:33.000000 torchlure-0.2405.8/src/torchlure.egg-info/requires.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       10 2024-05-17 15:39:33.000000 torchlure-0.2405.8/src/torchlure.egg-info/top_level.txt
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:44:24.887067 torchlure-0.2405.9/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      133 2024-04-19 13:30:09.000000 torchlure-0.2405.9/.gitignore
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        7 2024-04-19 12:37:01.000000 torchlure-0.2405.9/.python-version
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:44:24.877067 torchlure-0.2405.9/.vscode/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      520 2024-05-17 10:31:16.000000 torchlure-0.2405.9/.vscode/extensions.json
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      208 2024-05-17 10:31:16.000000 torchlure-0.2405.9/.vscode/settings.json
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1805 2024-05-17 15:44:24.877067 torchlure-0.2405.9/PKG-INFO
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1290 2024-05-17 11:41:15.000000 torchlure-0.2405.9/README.md
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1064 2024-05-17 15:37:36.000000 torchlure-0.2405.9/pyproject.toml
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       38 2024-05-17 15:44:24.887067 torchlure-0.2405.9/setup.cfg
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      939 2024-05-15 16:17:28.000000 torchlure-0.2405.9/setup.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:44:24.877067 torchlure-0.2405.9/src/
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:44:24.877067 torchlure-0.2405.9/src/torchlure/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      184 2024-05-17 15:44:18.000000 torchlure-0.2405.9/src/torchlure/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:44:24.877067 torchlure-0.2405.9/src/torchlure/datasets/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       46 2024-05-17 10:45:02.000000 torchlure-0.2405.9/src/torchlure/datasets/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:44:24.877067 torchlure-0.2405.9/src/torchlure/datasets/d4rl/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     7114 2024-05-17 15:43:30.000000 torchlure-0.2405.9/src/torchlure/datasets/d4rl/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    22657 2024-05-17 11:28:16.000000 torchlure-0.2405.9/src/torchlure/datasets/d4rl/d4rl_infos.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:44:24.877067 torchlure-0.2405.9/src/torchlure/datasets/offline_rl/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     4105 2024-05-17 10:47:01.000000 torchlure-0.2405.9/src/torchlure/datasets/offline_rl/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    11374 2024-05-15 18:42:40.000000 torchlure-0.2405.9/src/torchlure/datasets/offline_rl/minari_ext.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:44:24.877067 torchlure-0.2405.9/src/torchlure/functional/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     3567 2024-04-19 13:10:24.000000 torchlure-0.2405.9/src/torchlure/functional/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:44:24.877067 torchlure-0.2405.9/src/torchlure/modules/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1272 2024-04-25 08:19:27.000000 torchlure-0.2405.9/src/torchlure/modules/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2894 2024-04-19 13:40:26.000000 torchlure-0.2405.9/src/torchlure/noise_schedulers.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       31 2024-04-19 12:53:51.000000 torchlure-0.2405.9/src/torchlure/optim.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1481 2024-04-19 12:49:22.000000 torchlure-0.2405.9/src/torchlure/utils.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:44:24.877067 torchlure-0.2405.9/src/torchlure.egg-info/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1805 2024-05-17 15:44:24.000000 torchlure-0.2405.9/src/torchlure.egg-info/PKG-INFO
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      678 2024-05-17 15:44:24.000000 torchlure-0.2405.9/src/torchlure.egg-info/SOURCES.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        1 2024-05-17 15:44:24.000000 torchlure-0.2405.9/src/torchlure.egg-info/dependency_links.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       99 2024-05-17 15:44:24.000000 torchlure-0.2405.9/src/torchlure.egg-info/requires.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       10 2024-05-17 15:44:24.000000 torchlure-0.2405.9/src/torchlure.egg-info/top_level.txt
```

### Comparing `torchlure-0.2405.8/.vscode/extensions.json` & `torchlure-0.2405.9/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.8/PKG-INFO` & `torchlure-0.2405.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlure
-Version: 0.2405.8
+Version: 0.2405.9
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
-Metadata-Version: 2.1 Name: torchlure Version: 0.2405.8 Author-email: fuyutarow
+Metadata-Version: 2.1 Name: torchlure Version: 0.2405.9 Author-email: fuyutarow
 gmail.com> Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure Keywords:
 pytorch Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1 Requires-Dist: numpy>=1.26.4 Requires-Dist: sophia-
 opt>=0.2.2 Requires-Dist: gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28
 Requires-Dist: gdown>=5.2.0 Requires-Dist: h5py>=3.11.0 # Torch Lure
 _[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip install git+https://github.com/Farama-
```

### Comparing `torchlure-0.2405.8/README.md` & `torchlure-0.2405.9/README.md`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.8/pyproject.toml` & `torchlure-0.2405.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.8/setup.py` & `torchlure-0.2405.9/setup.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.8/src/torchlure/datasets/d4rl/__init__.py` & `torchlure-0.2405.9/src/torchlure/datasets/d4rl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import h5py
 import minari
 import requests
 from minari.data_collector.episode_buffer import EpisodeBuffer
 from minari.utils import create_dataset_from_buffers
 from torch.utils.data import Dataset
 
+from .d4rl_infos import D4RL_DATASETS
+
 
 class D4RLDataset(Dataset):
     def __init__(
         self,
         dataset_id: str,
         d4rl_name: Union[str, None] = None,
         env_id: Union[str, None] = None,
```

### Comparing `torchlure-0.2405.8/src/torchlure/datasets/d4rl/d4rl_infos.py` & `torchlure-0.2405.9/src/torchlure/datasets/d4rl/d4rl_infos.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.8/src/torchlure/datasets/offline_rl/__init__.py` & `torchlure-0.2405.9/src/torchlure/datasets/offline_rl/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.8/src/torchlure/datasets/offline_rl/minari_ext.py` & `torchlure-0.2405.9/src/torchlure/datasets/offline_rl/minari_ext.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.8/src/torchlure/functional/__init__.py` & `torchlure-0.2405.9/src/torchlure/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.8/src/torchlure/modules/__init__.py` & `torchlure-0.2405.9/src/torchlure/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.8/src/torchlure/noise_schedulers.py` & `torchlure-0.2405.9/src/torchlure/noise_schedulers.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.8/src/torchlure/utils.py` & `torchlure-0.2405.9/src/torchlure/utils.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.8/src/torchlure.egg-info/PKG-INFO` & `torchlure-0.2405.9/src/torchlure.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlure
-Version: 0.2405.8
+Version: 0.2405.9
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
-Metadata-Version: 2.1 Name: torchlure Version: 0.2405.8 Author-email: fuyutarow
+Metadata-Version: 2.1 Name: torchlure Version: 0.2405.9 Author-email: fuyutarow
 gmail.com> Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure Keywords:
 pytorch Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1 Requires-Dist: numpy>=1.26.4 Requires-Dist: sophia-
 opt>=0.2.2 Requires-Dist: gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28
 Requires-Dist: gdown>=5.2.0 Requires-Dist: h5py>=3.11.0 # Torch Lure
 _[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip install git+https://github.com/Farama-
```

### Comparing `torchlure-0.2405.8/src/torchlure.egg-info/SOURCES.txt` & `torchlure-0.2405.9/src/torchlure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

