# Comparing `tmp/torchlure-0.2405.2.tar.gz` & `tmp/torchlure-0.2405.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlure-0.2405.2.tar", last modified: Fri May 17 00:41:53 2024, max compression
+gzip compressed data, was "torchlure-0.2405.3.dev0.tar", last modified: Fri May 17 10:35:32 2024, max compression
```

## Comparing `torchlure-0.2405.2.tar` & `torchlure-0.2405.3.dev0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 00:41:53.147067 torchlure-0.2405.2/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      133 2024-04-19 13:30:09.000000 torchlure-0.2405.2/.gitignore
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        7 2024-04-19 12:37:01.000000 torchlure-0.2405.2/.python-version
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1245 2024-05-17 00:41:53.147067 torchlure-0.2405.2/PKG-INFO
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      786 2024-05-15 16:17:41.000000 torchlure-0.2405.2/README.md
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1023 2024-05-15 16:22:17.000000 torchlure-0.2405.2/pyproject.toml
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       38 2024-05-17 00:41:53.147067 torchlure-0.2405.2/setup.cfg
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      939 2024-05-15 16:17:28.000000 torchlure-0.2405.2/setup.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 00:41:53.137067 torchlure-0.2405.2/src/
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 00:41:53.137067 torchlure-0.2405.2/src/torchlure/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      173 2024-05-17 00:41:18.000000 torchlure-0.2405.2/src/torchlure/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 00:41:53.147067 torchlure-0.2405.2/src/torchlure/datasets/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1424 2024-05-17 00:41:05.000000 torchlure-0.2405.2/src/torchlure/datasets/__init__.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2819 2024-05-17 00:40:11.000000 torchlure-0.2405.2/src/torchlure/datasets/helpers.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    11374 2024-05-15 18:42:40.000000 torchlure-0.2405.2/src/torchlure/datasets/minari_ext.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 00:41:53.147067 torchlure-0.2405.2/src/torchlure/functional/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     3567 2024-04-19 13:10:24.000000 torchlure-0.2405.2/src/torchlure/functional/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 00:41:53.147067 torchlure-0.2405.2/src/torchlure/modules/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1272 2024-04-25 08:19:27.000000 torchlure-0.2405.2/src/torchlure/modules/__init__.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2894 2024-04-19 13:40:26.000000 torchlure-0.2405.2/src/torchlure/noise_schedulers.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       31 2024-04-19 12:53:51.000000 torchlure-0.2405.2/src/torchlure/optim.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1481 2024-04-19 12:49:22.000000 torchlure-0.2405.2/src/torchlure/utils.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 00:41:53.147067 torchlure-0.2405.2/src/torchlure.egg-info/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1245 2024-05-17 00:41:53.000000 torchlure-0.2405.2/src/torchlure.egg-info/PKG-INFO
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      527 2024-05-17 00:41:53.000000 torchlure-0.2405.2/src/torchlure.egg-info/SOURCES.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        1 2024-05-17 00:41:53.000000 torchlure-0.2405.2/src/torchlure.egg-info/dependency_links.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       73 2024-05-17 00:41:53.000000 torchlure-0.2405.2/src/torchlure.egg-info/requires.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       10 2024-05-17 00:41:53.000000 torchlure-0.2405.2/src/torchlure.egg-info/top_level.txt
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:35:32.057067 torchlure-0.2405.3.dev0/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      133 2024-04-19 13:30:09.000000 torchlure-0.2405.3.dev0/.gitignore
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        7 2024-04-19 12:37:01.000000 torchlure-0.2405.3.dev0/.python-version
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1278 2024-05-17 10:35:32.057067 torchlure-0.2405.3.dev0/PKG-INFO
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      786 2024-05-15 16:17:41.000000 torchlure-0.2405.3.dev0/README.md
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1044 2024-05-17 10:31:30.000000 torchlure-0.2405.3.dev0/pyproject.toml
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       38 2024-05-17 10:35:32.057067 torchlure-0.2405.3.dev0/setup.cfg
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      939 2024-05-15 16:17:28.000000 torchlure-0.2405.3.dev0/setup.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:35:32.057067 torchlure-0.2405.3.dev0/src/
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:35:32.057067 torchlure-0.2405.3.dev0/src/torchlure/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      177 2024-05-17 10:35:17.000000 torchlure-0.2405.3.dev0/src/torchlure/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:35:32.057067 torchlure-0.2405.3.dev0/src/torchlure/datasets/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1406 2024-05-17 10:32:59.000000 torchlure-0.2405.3.dev0/src/torchlure/datasets/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:35:32.057067 torchlure-0.2405.3.dev0/src/torchlure/datasets/d4rl/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     5509 2024-05-17 10:31:22.000000 torchlure-0.2405.3.dev0/src/torchlure/datasets/d4rl/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2816 2024-05-17 10:34:20.000000 torchlure-0.2405.3.dev0/src/torchlure/datasets/helpers.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    11374 2024-05-15 18:42:40.000000 torchlure-0.2405.3.dev0/src/torchlure/datasets/minari_ext.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:35:32.057067 torchlure-0.2405.3.dev0/src/torchlure/functional/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     3567 2024-04-19 13:10:24.000000 torchlure-0.2405.3.dev0/src/torchlure/functional/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:35:32.057067 torchlure-0.2405.3.dev0/src/torchlure/modules/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1272 2024-04-25 08:19:27.000000 torchlure-0.2405.3.dev0/src/torchlure/modules/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2894 2024-04-19 13:40:26.000000 torchlure-0.2405.3.dev0/src/torchlure/noise_schedulers.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       31 2024-04-19 12:53:51.000000 torchlure-0.2405.3.dev0/src/torchlure/optim.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1481 2024-04-19 12:49:22.000000 torchlure-0.2405.3.dev0/src/torchlure/utils.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 10:35:32.057067 torchlure-0.2405.3.dev0/src/torchlure.egg-info/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1278 2024-05-17 10:35:32.000000 torchlure-0.2405.3.dev0/src/torchlure.egg-info/PKG-INFO
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      567 2024-05-17 10:35:32.000000 torchlure-0.2405.3.dev0/src/torchlure.egg-info/SOURCES.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        1 2024-05-17 10:35:32.000000 torchlure-0.2405.3.dev0/src/torchlure.egg-info/dependency_links.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       86 2024-05-17 10:35:32.000000 torchlure-0.2405.3.dev0/src/torchlure.egg-info/requires.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       10 2024-05-17 10:35:32.000000 torchlure-0.2405.3.dev0/src/torchlure.egg-info/top_level.txt
```

### Comparing `torchlure-0.2405.2/PKG-INFO` & `torchlure-0.2405.3.dev0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: torchlure
-Version: 0.2405.2
+Version: 0.2405.3.dev0
 Author-email: fuyutarow <fuyutarow@gmail.com>
 Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure
 Keywords: pytorch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: sophia-opt>=0.2.2
 Requires-Dist: gymnasium>=0.29.1
 Requires-Dist: jax>=0.4.28
+Requires-Dist: gdown>=5.2.0
 
 # Torch Lure
 
 
 <a href="https://www.youtube.com/watch?v=wCzCOYCfY9g" target="_blank">
   <img src="http://img.youtube.com/vi/wCzCOYCfY9g/maxresdefault.jpg" alt="Chandelure" style="width: 100%;">
 </a>
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: torchlure Version: 0.2405.2 Author-email: fuyutarow
+Metadata-Version: 2.1 Name: torchlure Version: 0.2405.3.dev0 Author-email:
+fuyutarow
 gmail.com> Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure Keywords:
 pytorch Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1 Requires-Dist: numpy>=1.26.4 Requires-Dist: sophia-
-opt>=0.2.2 Requires-Dist: gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28 # Torch
-Lure _[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip install git+https://github.com/Farama-
-Foundation/Minari.git@19565bd8cd33f2e4a3a9a8e4db372044b01ea8d3 ``` ```sh pip
-install torch-lure ``` # Usage ```py import torchlure as lure # Optimizers
-lure.SophiaG(lr=1e-3, weight_decay=0.2) # Functions lure.tanh_exp(x)
-lure.TanhExp() lure.quantile_loss(y_pred, y_target, quantile=0.5)
-lure.QuantileLoss(quantile=0.5) lure.RMSNrom(dim=256, eps=1e-6) # Noise
-Scheduler lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02,
-num_timesteps=1000) lure.CosineNoiseScheduler(max_beta=0.999, s=0.008,
-num_timesteps=1000): ```
+opt>=0.2.2 Requires-Dist: gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28
+Requires-Dist: gdown>=5.2.0 # Torch Lure _[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip
+install git+https://github.com/Farama-Foundation/
+Minari.git@19565bd8cd33f2e4a3a9a8e4db372044b01ea8d3 ``` ```sh pip install
+torch-lure ``` # Usage ```py import torchlure as lure # Optimizers lure.SophiaG
+(lr=1e-3, weight_decay=0.2) # Functions lure.tanh_exp(x) lure.TanhExp()
+lure.quantile_loss(y_pred, y_target, quantile=0.5) lure.QuantileLoss
+(quantile=0.5) lure.RMSNrom(dim=256, eps=1e-6) # Noise Scheduler
+lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02, num_timesteps=1000)
+lure.CosineNoiseScheduler(max_beta=0.999, s=0.008, num_timesteps=1000): ```
```

### Comparing `torchlure-0.2405.2/README.md` & `torchlure-0.2405.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.2/pyproject.toml` & `torchlure-0.2405.3.dev0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 dependencies = [
     "torch>=2.1",
     "numpy>=1.26.4",
     "sophia-opt>=0.2.2",
     # "minari @ git+https://github.com/Farama-Foundation/Minari@19565bd8cd33f2e4a3a9a8e4db372044b01ea8d3",
     "gymnasium>=0.29.1",
     "jax>=0.4.28",
+    "gdown>=5.2.0",
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 keywords = ["pytorch"]
 
 
 [project.urls]
@@ -41,8 +42,8 @@
 write_to = "src/torchlure/_version.py"
 version_scheme = "post-release"
 local_scheme = "dirty-tag"
 
 
 [tool.setuptools.packages.find]
 where = ["src"]
-include = ["torchlure", "torchlure.*"]
+include = ["torchlure", "torchlure.*"]
```

### Comparing `torchlure-0.2405.2/setup.py` & `torchlure-0.2405.3.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.2/src/torchlure/datasets/__init__.py` & `torchlure-0.2405.3.dev0/src/torchlure/datasets/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 import minari
 from torch.utils.data import DataLoader, Dataset
 
-from .minari_ext import *
+from .d4rl import *
 from .helpers import *
+from .minari_ext import *
 
 
-class D4RLDataset(Dataset):
+class MinariRLDataset(Dataset):
     def __init__(
         self,
-        dataset_name: str,
+        dataset_id: str,
         env_id: str | None = None,
         num_episodes: int | None = None,
     ):
 
         try:
-            dataset = minari.load_dataset(dataset_name)
+            dataset = minari.load_dataset(dataset_id)
             self.dataset = dataset
             return
         except:
             pass
 
-        assert (
-            env_id is not None
-        ), "env_id must be provided if dataset_name is not found"
+        assert env_id is not None, "env_id must be provided if dataset_id is not found"
         assert (
             num_episodes is not None
-        ), "num_episodes must be provided if dataset_name is not found"
+        ), "num_episodes must be provided if dataset_id is not found"
 
-        self.dataset_name = dataset_name
+        self.dataset_id = dataset_id
         self.env_id = env_id
         self.num_episodes = num_episodes
         self.dataset = None
 
     async def collect_episodes(self, num_envs: int = 1, print_every: int = 1000):
         if self.dataset:
             print("Dataset already exists")
             return
 
         await collect_samples_async(
             env_id=self.env_id,
             num_episodes=self.num_episodes,
-            dataset_name=self.dataset_name,
+            dataset_id=self.dataset_id,
             num_envs=num_envs,
             print_every=print_every,
         )
-        self.dataset = minari.load_dataset(self.dataset_name)
+        self.dataset = minari.load_dataset(self.dataset_id)
 
     def __len__(self):
         return len(self.dataset)
 
     def __getitem__(self, idx: int):
         return self.dataset[idx]
```

### Comparing `torchlure-0.2405.2/src/torchlure/datasets/helpers.py` & `torchlure-0.2405.3.dev0/src/torchlure/datasets/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import time
 
 import gymnasium as gym
 import minari
+
 from .minari_ext import AsyncDataCollector, D4RLDataset
 
 
 async def collect_episode(env, policy=None):
     """Collect a single episode using the specified environment and policy."""
     env.reset()
     done = False
@@ -38,15 +39,15 @@
             eta_minutes, eta_seconds = divmod(eta, 60)
             print(
                 f"Collected {episodes_done} episodes. ETA: {int(eta_minutes)}m {int(eta_seconds)}s"
             )
 
 
 async def collect_samples_async(
-    env_id, num_episodes, dataset_name, policy=None, num_envs=4, print_every=1000
+    env_id, num_episodes, dataset_id, policy=None, num_envs=4, print_every=1000
 ):
     """Collect samples asynchronously using multiple environments."""
     start_time = time.time()
 
     # Initialize environments
     envs = [
         AsyncDataCollector(gym.make(env_id), record_infos=True) for _ in range(num_envs)
@@ -67,15 +68,15 @@
     tasks = [
         worker(env, queue, policy, start_time, print_every, num_episodes)
         for env in envs
     ]
     await asyncio.gather(*tasks)
 
     # Create the dataset using the first environment
-    dataset = envs[0].create_dataset(dataset_name)
+    dataset = envs[0].create_dataset(dataset_id)
 
     # Add data from other environments to the dataset
     for i, env in enumerate(envs[1:], start=2):
         try:
             env.add_to_dataset(dataset)
         except Exception as e:
             print(f"Error adding data from environment {i}: {e}")
```

### Comparing `torchlure-0.2405.2/src/torchlure/datasets/minari_ext.py` & `torchlure-0.2405.3.dev0/src/torchlure/datasets/minari_ext.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.2/src/torchlure/functional/__init__.py` & `torchlure-0.2405.3.dev0/src/torchlure/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.2/src/torchlure/modules/__init__.py` & `torchlure-0.2405.3.dev0/src/torchlure/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.2/src/torchlure/noise_schedulers.py` & `torchlure-0.2405.3.dev0/src/torchlure/noise_schedulers.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.2/src/torchlure/utils.py` & `torchlure-0.2405.3.dev0/src/torchlure/utils.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.2/src/torchlure.egg-info/PKG-INFO` & `torchlure-0.2405.3.dev0/src/torchlure.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: torchlure
-Version: 0.2405.2
+Version: 0.2405.3.dev0
 Author-email: fuyutarow <fuyutarow@gmail.com>
 Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure
 Keywords: pytorch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: sophia-opt>=0.2.2
 Requires-Dist: gymnasium>=0.29.1
 Requires-Dist: jax>=0.4.28
+Requires-Dist: gdown>=5.2.0
 
 # Torch Lure
 
 
 <a href="https://www.youtube.com/watch?v=wCzCOYCfY9g" target="_blank">
   <img src="http://img.youtube.com/vi/wCzCOYCfY9g/maxresdefault.jpg" alt="Chandelure" style="width: 100%;">
 </a>
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: torchlure Version: 0.2405.2 Author-email: fuyutarow
+Metadata-Version: 2.1 Name: torchlure Version: 0.2405.3.dev0 Author-email:
+fuyutarow
 gmail.com> Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure Keywords:
 pytorch Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1 Requires-Dist: numpy>=1.26.4 Requires-Dist: sophia-
-opt>=0.2.2 Requires-Dist: gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28 # Torch
-Lure _[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip install git+https://github.com/Farama-
-Foundation/Minari.git@19565bd8cd33f2e4a3a9a8e4db372044b01ea8d3 ``` ```sh pip
-install torch-lure ``` # Usage ```py import torchlure as lure # Optimizers
-lure.SophiaG(lr=1e-3, weight_decay=0.2) # Functions lure.tanh_exp(x)
-lure.TanhExp() lure.quantile_loss(y_pred, y_target, quantile=0.5)
-lure.QuantileLoss(quantile=0.5) lure.RMSNrom(dim=256, eps=1e-6) # Noise
-Scheduler lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02,
-num_timesteps=1000) lure.CosineNoiseScheduler(max_beta=0.999, s=0.008,
-num_timesteps=1000): ```
+opt>=0.2.2 Requires-Dist: gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28
+Requires-Dist: gdown>=5.2.0 # Torch Lure _[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip
+install git+https://github.com/Farama-Foundation/
+Minari.git@19565bd8cd33f2e4a3a9a8e4db372044b01ea8d3 ``` ```sh pip install
+torch-lure ``` # Usage ```py import torchlure as lure # Optimizers lure.SophiaG
+(lr=1e-3, weight_decay=0.2) # Functions lure.tanh_exp(x) lure.TanhExp()
+lure.quantile_loss(y_pred, y_target, quantile=0.5) lure.QuantileLoss
+(quantile=0.5) lure.RMSNrom(dim=256, eps=1e-6) # Noise Scheduler
+lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02, num_timesteps=1000)
+lure.CosineNoiseScheduler(max_beta=0.999, s=0.008, num_timesteps=1000): ```
```

### Comparing `torchlure-0.2405.2/src/torchlure.egg-info/SOURCES.txt` & `torchlure-0.2405.3.dev0/src/torchlure.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,9 +11,10 @@
 src/torchlure.egg-info/SOURCES.txt
 src/torchlure.egg-info/dependency_links.txt
 src/torchlure.egg-info/requires.txt
 src/torchlure.egg-info/top_level.txt
 src/torchlure/datasets/__init__.py
 src/torchlure/datasets/helpers.py
 src/torchlure/datasets/minari_ext.py
+src/torchlure/datasets/d4rl/__init__.py
 src/torchlure/functional/__init__.py
 src/torchlure/modules/__init__.py
```

