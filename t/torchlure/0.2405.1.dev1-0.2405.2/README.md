# Comparing `tmp/torchlure-0.2405.1.dev1.tar.gz` & `tmp/torchlure-0.2405.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlure-0.2405.1.dev1.tar", last modified: Wed May 15 16:22:27 2024, max compression
+gzip compressed data, was "torchlure-0.2405.2.tar", last modified: Fri May 17 00:41:53 2024, max compression
```

## Comparing `torchlure-0.2405.1.dev1.tar` & `torchlure-0.2405.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-15 16:22:27.683635 torchlure-0.2405.1.dev1/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      133 2024-04-19 13:30:09.000000 torchlure-0.2405.1.dev1/.gitignore
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        7 2024-04-19 12:37:01.000000 torchlure-0.2405.1.dev1/.python-version
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1250 2024-05-15 16:22:27.683635 torchlure-0.2405.1.dev1/PKG-INFO
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      786 2024-05-15 16:17:41.000000 torchlure-0.2405.1.dev1/README.md
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1023 2024-05-15 16:22:17.000000 torchlure-0.2405.1.dev1/pyproject.toml
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       38 2024-05-15 16:22:27.683635 torchlure-0.2405.1.dev1/setup.cfg
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      939 2024-05-15 16:17:28.000000 torchlure-0.2405.1.dev1/setup.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-15 16:22:27.683635 torchlure-0.2405.1.dev1/src/
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-15 16:22:27.683635 torchlure-0.2405.1.dev1/src/torchlure/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      179 2024-05-15 16:19:30.000000 torchlure-0.2405.1.dev1/src/torchlure/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-15 16:22:27.683635 torchlure-0.2405.1.dev1/src/torchlure/datasets/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1271 2024-05-15 16:04:19.000000 torchlure-0.2405.1.dev1/src/torchlure/datasets/__init__.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    11373 2024-05-15 14:13:40.000000 torchlure-0.2405.1.dev1/src/torchlure/datasets/minari_ext.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-15 16:22:27.683635 torchlure-0.2405.1.dev1/src/torchlure/functional/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     3567 2024-04-19 13:10:24.000000 torchlure-0.2405.1.dev1/src/torchlure/functional/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-15 16:22:27.683635 torchlure-0.2405.1.dev1/src/torchlure/modules/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1272 2024-04-25 08:19:27.000000 torchlure-0.2405.1.dev1/src/torchlure/modules/__init__.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2894 2024-04-19 13:40:26.000000 torchlure-0.2405.1.dev1/src/torchlure/noise_schedulers.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       31 2024-04-19 12:53:51.000000 torchlure-0.2405.1.dev1/src/torchlure/optim.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1481 2024-04-19 12:49:22.000000 torchlure-0.2405.1.dev1/src/torchlure/utils.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-15 16:22:27.683635 torchlure-0.2405.1.dev1/src/torchlure.egg-info/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1250 2024-05-15 16:22:27.000000 torchlure-0.2405.1.dev1/src/torchlure.egg-info/PKG-INFO
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      493 2024-05-15 16:22:27.000000 torchlure-0.2405.1.dev1/src/torchlure.egg-info/SOURCES.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        1 2024-05-15 16:22:27.000000 torchlure-0.2405.1.dev1/src/torchlure.egg-info/dependency_links.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       73 2024-05-15 16:22:27.000000 torchlure-0.2405.1.dev1/src/torchlure.egg-info/requires.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       10 2024-05-15 16:22:27.000000 torchlure-0.2405.1.dev1/src/torchlure.egg-info/top_level.txt
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 00:41:53.147067 torchlure-0.2405.2/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      133 2024-04-19 13:30:09.000000 torchlure-0.2405.2/.gitignore
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        7 2024-04-19 12:37:01.000000 torchlure-0.2405.2/.python-version
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1245 2024-05-17 00:41:53.147067 torchlure-0.2405.2/PKG-INFO
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      786 2024-05-15 16:17:41.000000 torchlure-0.2405.2/README.md
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1023 2024-05-15 16:22:17.000000 torchlure-0.2405.2/pyproject.toml
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       38 2024-05-17 00:41:53.147067 torchlure-0.2405.2/setup.cfg
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      939 2024-05-15 16:17:28.000000 torchlure-0.2405.2/setup.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 00:41:53.137067 torchlure-0.2405.2/src/
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 00:41:53.137067 torchlure-0.2405.2/src/torchlure/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      173 2024-05-17 00:41:18.000000 torchlure-0.2405.2/src/torchlure/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 00:41:53.147067 torchlure-0.2405.2/src/torchlure/datasets/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1424 2024-05-17 00:41:05.000000 torchlure-0.2405.2/src/torchlure/datasets/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2819 2024-05-17 00:40:11.000000 torchlure-0.2405.2/src/torchlure/datasets/helpers.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    11374 2024-05-15 18:42:40.000000 torchlure-0.2405.2/src/torchlure/datasets/minari_ext.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 00:41:53.147067 torchlure-0.2405.2/src/torchlure/functional/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     3567 2024-04-19 13:10:24.000000 torchlure-0.2405.2/src/torchlure/functional/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 00:41:53.147067 torchlure-0.2405.2/src/torchlure/modules/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1272 2024-04-25 08:19:27.000000 torchlure-0.2405.2/src/torchlure/modules/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2894 2024-04-19 13:40:26.000000 torchlure-0.2405.2/src/torchlure/noise_schedulers.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       31 2024-04-19 12:53:51.000000 torchlure-0.2405.2/src/torchlure/optim.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1481 2024-04-19 12:49:22.000000 torchlure-0.2405.2/src/torchlure/utils.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 00:41:53.147067 torchlure-0.2405.2/src/torchlure.egg-info/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1245 2024-05-17 00:41:53.000000 torchlure-0.2405.2/src/torchlure.egg-info/PKG-INFO
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      527 2024-05-17 00:41:53.000000 torchlure-0.2405.2/src/torchlure.egg-info/SOURCES.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        1 2024-05-17 00:41:53.000000 torchlure-0.2405.2/src/torchlure.egg-info/dependency_links.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       73 2024-05-17 00:41:53.000000 torchlure-0.2405.2/src/torchlure.egg-info/requires.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       10 2024-05-17 00:41:53.000000 torchlure-0.2405.2/src/torchlure.egg-info/top_level.txt
```

### Comparing `torchlure-0.2405.1.dev1/PKG-INFO` & `torchlure-0.2405.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlure
-Version: 0.2405.1.dev1
+Version: 0.2405.2
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
@@ -1,9 +1,8 @@
-Metadata-Version: 2.1 Name: torchlure Version: 0.2405.1.dev1 Author-email:
-fuyutarow
+Metadata-Version: 2.1 Name: torchlure Version: 0.2405.2 Author-email: fuyutarow
 gmail.com> Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure Keywords:
 pytorch Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1 Requires-Dist: numpy>=1.26.4 Requires-Dist: sophia-
 opt>=0.2.2 Requires-Dist: gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28 # Torch
 Lure _[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip install git+https://github.com/Farama-
 Foundation/Minari.git@19565bd8cd33f2e4a3a9a8e4db372044b01ea8d3 ``` ```sh pip
```

### Comparing `torchlure-0.2405.1.dev1/README.md` & `torchlure-0.2405.2/README.md`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.1.dev1/pyproject.toml` & `torchlure-0.2405.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.1.dev1/setup.py` & `torchlure-0.2405.2/setup.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.1.dev1/src/torchlure/datasets/__init__.py` & `torchlure-0.2405.2/src/torchlure/datasets/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 import minari
 from torch.utils.data import DataLoader, Dataset
 
 from .minari_ext import *
+from .helpers import *
 
 
 class D4RLDataset(Dataset):
     def __init__(
         self,
         dataset_name: str,
         env_id: str | None = None,
-        n_episodes: int | None = None,
+        num_episodes: int | None = None,
     ):
 
         try:
             dataset = minari.load_dataset(dataset_name)
             self.dataset = dataset
             return
         except:
             pass
 
         assert (
             env_id is not None
         ), "env_id must be provided if dataset_name is not found"
         assert (
-            n_episodes is not None
-        ), "n_episodes must be provided if dataset_name is not found"
+            num_episodes is not None
+        ), "num_episodes must be provided if dataset_name is not found"
 
         self.dataset_name = dataset_name
         self.env_id = env_id
-        self.n_episodes = n_episodes
+        self.num_episodes = num_episodes
         self.dataset = None
 
-    async def collect_episodes(self):
+    async def collect_episodes(self, num_envs: int = 1, print_every: int = 1000):
         if self.dataset:
             print("Dataset already exists")
             return
 
         await collect_samples_async(
             env_id=self.env_id,
-            n_episodes=self.n_episodes,
+            num_episodes=self.num_episodes,
             dataset_name=self.dataset_name,
+            num_envs=num_envs,
+            print_every=print_every,
         )
         self.dataset = minari.load_dataset(self.dataset_name)
 
     def __len__(self):
         return len(self.dataset)
 
     def __getitem__(self, idx: int):
         return self.dataset[idx]
+
+
+#
```

### Comparing `torchlure-0.2405.1.dev1/src/torchlure/datasets/minari_ext.py` & `torchlure-0.2405.2/src/torchlure/datasets/minari_ext.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
     await asyncio.sleep(0)  # Allow other tasks to run
     env.reset()
     done = False
     while not done:
         action = env.action_space.sample() if policy is None else policy()
         obs, rew, terminated, truncated, info = env.step(action)
         done = terminated or truncated
-    if i % 100 == 0:
+    if i % 1000 == 0:
         print(f"Collected {i} episodes")
 
 
 async def collect_samples_async(env_id, n_episodes, dataset_name, policy=None):
     env = gym.make(env_id)
     env = AsyncDataCollector(env, record_infos=True)
```

### Comparing `torchlure-0.2405.1.dev1/src/torchlure/functional/__init__.py` & `torchlure-0.2405.2/src/torchlure/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.1.dev1/src/torchlure/modules/__init__.py` & `torchlure-0.2405.2/src/torchlure/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.1.dev1/src/torchlure/noise_schedulers.py` & `torchlure-0.2405.2/src/torchlure/noise_schedulers.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.1.dev1/src/torchlure/utils.py` & `torchlure-0.2405.2/src/torchlure/utils.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.1.dev1/src/torchlure.egg-info/PKG-INFO` & `torchlure-0.2405.2/src/torchlure.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlure
-Version: 0.2405.1.dev1
+Version: 0.2405.2
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
@@ -1,9 +1,8 @@
-Metadata-Version: 2.1 Name: torchlure Version: 0.2405.1.dev1 Author-email:
-fuyutarow
+Metadata-Version: 2.1 Name: torchlure Version: 0.2405.2 Author-email: fuyutarow
 gmail.com> Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure Keywords:
 pytorch Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1 Requires-Dist: numpy>=1.26.4 Requires-Dist: sophia-
 opt>=0.2.2 Requires-Dist: gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28 # Torch
 Lure _[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip install git+https://github.com/Farama-
 Foundation/Minari.git@19565bd8cd33f2e4a3a9a8e4db372044b01ea8d3 ``` ```sh pip
```

