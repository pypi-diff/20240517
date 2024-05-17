# Comparing `tmp/torchlure-0.2405.7.tar.gz` & `tmp/torchlure-0.2405.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlure-0.2405.7.tar", last modified: Fri May 17 11:39:14 2024, max compression
+gzip compressed data, was "torchlure-0.2405.8.tar", last modified: Fri May 17 15:39:33 2024, max compression
```

## Comparing `torchlure-0.2405.7.tar` & `torchlure-0.2405.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:39:14.097067 torchlure-0.2405.7/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      133 2024-04-19 13:30:09.000000 torchlure-0.2405.7/.gitignore
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        7 2024-04-19 12:37:01.000000 torchlure-0.2405.7/.python-version
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:39:14.097067 torchlure-0.2405.7/.vscode/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      520 2024-05-17 10:31:16.000000 torchlure-0.2405.7/.vscode/extensions.json
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      208 2024-05-17 10:31:16.000000 torchlure-0.2405.7/.vscode/settings.json
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1765 2024-05-17 11:39:14.097067 torchlure-0.2405.7/PKG-INFO
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1278 2024-05-17 11:35:05.000000 torchlure-0.2405.7/README.md
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1044 2024-05-17 10:31:30.000000 torchlure-0.2405.7/pyproject.toml
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       38 2024-05-17 11:39:14.097067 torchlure-0.2405.7/setup.cfg
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      939 2024-05-15 16:17:28.000000 torchlure-0.2405.7/setup.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:39:14.097067 torchlure-0.2405.7/src/
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:39:14.097067 torchlure-0.2405.7/src/torchlure/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      184 2024-05-17 11:38:57.000000 torchlure-0.2405.7/src/torchlure/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:39:14.097067 torchlure-0.2405.7/src/torchlure/datasets/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       46 2024-05-17 10:45:02.000000 torchlure-0.2405.7/src/torchlure/datasets/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:39:14.097067 torchlure-0.2405.7/src/torchlure/datasets/d4rl/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     5031 2024-05-17 11:36:08.000000 torchlure-0.2405.7/src/torchlure/datasets/d4rl/__init__.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    22657 2024-05-17 11:28:16.000000 torchlure-0.2405.7/src/torchlure/datasets/d4rl/d4rl_infos.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:39:14.097067 torchlure-0.2405.7/src/torchlure/datasets/offline_rl/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     4105 2024-05-17 10:47:01.000000 torchlure-0.2405.7/src/torchlure/datasets/offline_rl/__init__.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    11374 2024-05-15 18:42:40.000000 torchlure-0.2405.7/src/torchlure/datasets/offline_rl/minari_ext.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:39:14.097067 torchlure-0.2405.7/src/torchlure/functional/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     3567 2024-04-19 13:10:24.000000 torchlure-0.2405.7/src/torchlure/functional/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:39:14.097067 torchlure-0.2405.7/src/torchlure/modules/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1272 2024-04-25 08:19:27.000000 torchlure-0.2405.7/src/torchlure/modules/__init__.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2894 2024-04-19 13:40:26.000000 torchlure-0.2405.7/src/torchlure/noise_schedulers.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       31 2024-04-19 12:53:51.000000 torchlure-0.2405.7/src/torchlure/optim.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1481 2024-04-19 12:49:22.000000 torchlure-0.2405.7/src/torchlure/utils.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:39:14.097067 torchlure-0.2405.7/src/torchlure.egg-info/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1765 2024-05-17 11:39:14.000000 torchlure-0.2405.7/src/torchlure.egg-info/PKG-INFO
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      678 2024-05-17 11:39:14.000000 torchlure-0.2405.7/src/torchlure.egg-info/SOURCES.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        1 2024-05-17 11:39:14.000000 torchlure-0.2405.7/src/torchlure.egg-info/dependency_links.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       86 2024-05-17 11:39:14.000000 torchlure-0.2405.7/src/torchlure.egg-info/requires.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       10 2024-05-17 11:39:14.000000 torchlure-0.2405.7/src/torchlure.egg-info/top_level.txt
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      133 2024-04-19 13:30:09.000000 torchlure-0.2405.8/.gitignore
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        7 2024-04-19 12:37:01.000000 torchlure-0.2405.8/.python-version
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/.vscode/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      520 2024-05-17 10:31:16.000000 torchlure-0.2405.8/.vscode/extensions.json
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      208 2024-05-17 10:31:16.000000 torchlure-0.2405.8/.vscode/settings.json
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1805 2024-05-17 15:39:33.747067 torchlure-0.2405.8/PKG-INFO
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1290 2024-05-17 11:41:15.000000 torchlure-0.2405.8/README.md
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1064 2024-05-17 15:37:36.000000 torchlure-0.2405.8/pyproject.toml
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       38 2024-05-17 15:39:33.747067 torchlure-0.2405.8/setup.cfg
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      939 2024-05-15 16:17:28.000000 torchlure-0.2405.8/setup.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.737067 torchlure-0.2405.8/src/
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/src/torchlure/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      184 2024-05-17 15:39:20.000000 torchlure-0.2405.8/src/torchlure/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/src/torchlure/datasets/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       46 2024-05-17 10:45:02.000000 torchlure-0.2405.8/src/torchlure/datasets/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/src/torchlure/datasets/d4rl/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     7075 2024-05-17 15:37:12.000000 torchlure-0.2405.8/src/torchlure/datasets/d4rl/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    22657 2024-05-17 11:28:16.000000 torchlure-0.2405.8/src/torchlure/datasets/d4rl/d4rl_infos.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/src/torchlure/datasets/offline_rl/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     4105 2024-05-17 10:47:01.000000 torchlure-0.2405.8/src/torchlure/datasets/offline_rl/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    11374 2024-05-15 18:42:40.000000 torchlure-0.2405.8/src/torchlure/datasets/offline_rl/minari_ext.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/src/torchlure/functional/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     3567 2024-04-19 13:10:24.000000 torchlure-0.2405.8/src/torchlure/functional/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/src/torchlure/modules/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1272 2024-04-25 08:19:27.000000 torchlure-0.2405.8/src/torchlure/modules/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2894 2024-04-19 13:40:26.000000 torchlure-0.2405.8/src/torchlure/noise_schedulers.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       31 2024-04-19 12:53:51.000000 torchlure-0.2405.8/src/torchlure/optim.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1481 2024-04-19 12:49:22.000000 torchlure-0.2405.8/src/torchlure/utils.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 15:39:33.747067 torchlure-0.2405.8/src/torchlure.egg-info/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1805 2024-05-17 15:39:33.000000 torchlure-0.2405.8/src/torchlure.egg-info/PKG-INFO
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      678 2024-05-17 15:39:33.000000 torchlure-0.2405.8/src/torchlure.egg-info/SOURCES.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        1 2024-05-17 15:39:33.000000 torchlure-0.2405.8/src/torchlure.egg-info/dependency_links.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       99 2024-05-17 15:39:33.000000 torchlure-0.2405.8/src/torchlure.egg-info/requires.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       10 2024-05-17 15:39:33.000000 torchlure-0.2405.8/src/torchlure.egg-info/top_level.txt
```

### Comparing `torchlure-0.2405.7/.vscode/extensions.json` & `torchlure-0.2405.8/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.7/PKG-INFO` & `torchlure-0.2405.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: torchlure
-Version: 0.2405.7
+Version: 0.2405.8
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
 Requires-Dist: gdown>=5.2.0
+Requires-Dist: h5py>=3.11.0
 
 # Torch Lure
 
 
 <a href="https://www.youtube.com/watch?v=wCzCOYCfY9g" target="_blank">
   <img src="http://img.youtube.com/vi/wCzCOYCfY9g/maxresdefault.jpg" alt="Chandelure" style="width: 100%;">
 </a>
@@ -58,20 +59,21 @@
 
 
 
 ```py
 from torchlure.datasets import OfflineRLDataset, D4RLDataset
 
 # Initial usage with download
+# %%
 dataset = D4RLDataset(
-    dataset_id="d4rl_walker2d-expert-2405",
-    d4rl_name="d4rl_walker2d-expert-v2",
-    env_id= "Walker2d-v4",
+    dataset_id= "hopper-medium-expert-v2.2405",
+    d4rl_name= "hopper-medium-expert-v2",
+    env_id= "Hopper-v4",
 )
 
 # if you are download it once
 dataset = D4RLDataset(
-    dataset_id="d4rl_walker2d-expert-2405",
+    dataset_id= "hopper-medium-expert-v2.2405",
 )
 ```
 
 See all datasets [here](https://github.com/pytorch/rl/blob/3a7cf6af2a08089f11e0ed8cad3dd1cea0e253fb/torchrl/data/datasets/d4rl_infos.py)
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: torchlure Version: 0.2405.7 Author-email: fuyutarow
+Metadata-Version: 2.1 Name: torchlure Version: 0.2405.8 Author-email: fuyutarow
 gmail.com> Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure Keywords:
 pytorch Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1 Requires-Dist: numpy>=1.26.4 Requires-Dist: sophia-
 opt>=0.2.2 Requires-Dist: gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28
-Requires-Dist: gdown>=5.2.0 # Torch Lure _[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip
-install git+https://github.com/Farama-Foundation/
-Minari.git@19565bd8cd33f2e4a3a9a8e4db372044b01ea8d3 ``` ```sh pip install
-torchlure ``` # Usage ```py import torchlure as lure # Optimizers lure.SophiaG
-(lr=1e-3, weight_decay=0.2) # Functions lure.tanh_exp(x) lure.TanhExp()
-lure.quantile_loss(y_pred, y_target, quantile=0.5) lure.QuantileLoss
-(quantile=0.5) lure.RMSNrom(dim=256, eps=1e-6) # Noise Scheduler
-lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02, num_timesteps=1000)
-lure.CosineNoiseScheduler(max_beta=0.999, s=0.008, num_timesteps=1000): ``` ###
-Dataset ```py from torchlure.datasets import OfflineRLDataset, D4RLDataset #
-Initial usage with download dataset = D4RLDataset( dataset_id="d4rl_walker2d-
-expert-2405", d4rl_name="d4rl_walker2d-expert-v2", env_id= "Walker2d-v4", ) #
-if you are download it once dataset = D4RLDataset( dataset_id="d4rl_walker2d-
-expert-2405", ) ``` See all datasets [here](https://github.com/pytorch/rl/blob/
+Requires-Dist: gdown>=5.2.0 Requires-Dist: h5py>=3.11.0 # Torch Lure
+_[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip install git+https://github.com/Farama-
+Foundation/Minari.git@19565bd8cd33f2e4a3a9a8e4db372044b01ea8d3 ``` ```sh pip
+install torchlure ``` # Usage ```py import torchlure as lure # Optimizers
+lure.SophiaG(lr=1e-3, weight_decay=0.2) # Functions lure.tanh_exp(x)
+lure.TanhExp() lure.quantile_loss(y_pred, y_target, quantile=0.5)
+lure.QuantileLoss(quantile=0.5) lure.RMSNrom(dim=256, eps=1e-6) # Noise
+Scheduler lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02,
+num_timesteps=1000) lure.CosineNoiseScheduler(max_beta=0.999, s=0.008,
+num_timesteps=1000): ``` ### Dataset ```py from torchlure.datasets import
+OfflineRLDataset, D4RLDataset # Initial usage with download # %% dataset =
+D4RLDataset( dataset_id= "hopper-medium-expert-v2.2405", d4rl_name= "hopper-
+medium-expert-v2", env_id= "Hopper-v4", ) # if you are download it once dataset
+= D4RLDataset( dataset_id= "hopper-medium-expert-v2.2405", ) ``` See all
+datasets [here](https://github.com/pytorch/rl/blob/
 3a7cf6af2a08089f11e0ed8cad3dd1cea0e253fb/torchrl/data/datasets/d4rl_infos.py)
```

### Comparing `torchlure-0.2405.7/README.md` & `torchlure-0.2405.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -42,20 +42,21 @@
 
 
 
 ```py
 from torchlure.datasets import OfflineRLDataset, D4RLDataset
 
 # Initial usage with download
+# %%
 dataset = D4RLDataset(
-    dataset_id="d4rl_walker2d-expert-2405",
-    d4rl_name="d4rl_walker2d-expert-v2",
-    env_id= "Walker2d-v4",
+    dataset_id= "hopper-medium-expert-v2.2405",
+    d4rl_name= "hopper-medium-expert-v2",
+    env_id= "Hopper-v4",
 )
 
 # if you are download it once
 dataset = D4RLDataset(
-    dataset_id="d4rl_walker2d-expert-2405",
+    dataset_id= "hopper-medium-expert-v2.2405",
 )
 ```
 
 See all datasets [here](https://github.com/pytorch/rl/blob/3a7cf6af2a08089f11e0ed8cad3dd1cea0e253fb/torchrl/data/datasets/d4rl_infos.py)
```

#### html2text {}

```diff
@@ -3,13 +3,13 @@
 pip install torchlure ``` # Usage ```py import torchlure as lure # Optimizers
 lure.SophiaG(lr=1e-3, weight_decay=0.2) # Functions lure.tanh_exp(x)
 lure.TanhExp() lure.quantile_loss(y_pred, y_target, quantile=0.5)
 lure.QuantileLoss(quantile=0.5) lure.RMSNrom(dim=256, eps=1e-6) # Noise
 Scheduler lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02,
 num_timesteps=1000) lure.CosineNoiseScheduler(max_beta=0.999, s=0.008,
 num_timesteps=1000): ``` ### Dataset ```py from torchlure.datasets import
-OfflineRLDataset, D4RLDataset # Initial usage with download dataset =
-D4RLDataset( dataset_id="d4rl_walker2d-expert-2405", d4rl_name="d4rl_walker2d-
-expert-v2", env_id= "Walker2d-v4", ) # if you are download it once dataset =
-D4RLDataset( dataset_id="d4rl_walker2d-expert-2405", ) ``` See all datasets
-[here](https://github.com/pytorch/rl/blob/
+OfflineRLDataset, D4RLDataset # Initial usage with download # %% dataset =
+D4RLDataset( dataset_id= "hopper-medium-expert-v2.2405", d4rl_name= "hopper-
+medium-expert-v2", env_id= "Hopper-v4", ) # if you are download it once dataset
+= D4RLDataset( dataset_id= "hopper-medium-expert-v2.2405", ) ``` See all
+datasets [here](https://github.com/pytorch/rl/blob/
 3a7cf6af2a08089f11e0ed8cad3dd1cea0e253fb/torchrl/data/datasets/d4rl_infos.py)
```

### Comparing `torchlure-0.2405.7/pyproject.toml` & `torchlure-0.2405.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     "torch>=2.1",
     "numpy>=1.26.4",
     "sophia-opt>=0.2.2",
     # "minari @ git+https://github.com/Farama-Foundation/Minari@19565bd8cd33f2e4a3a9a8e4db372044b01ea8d3",
     "gymnasium>=0.29.1",
     "jax>=0.4.28",
     "gdown>=5.2.0",
+    "h5py>=3.11.0",
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 keywords = ["pytorch"]
 
 
 [project.urls]
```

### Comparing `torchlure-0.2405.7/setup.py` & `torchlure-0.2405.8/setup.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.7/src/torchlure/datasets/d4rl/d4rl_infos.py` & `torchlure-0.2405.8/src/torchlure/datasets/d4rl/d4rl_infos.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.7/src/torchlure/datasets/offline_rl/__init__.py` & `torchlure-0.2405.8/src/torchlure/datasets/offline_rl/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.7/src/torchlure/datasets/offline_rl/minari_ext.py` & `torchlure-0.2405.8/src/torchlure/datasets/offline_rl/minari_ext.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.7/src/torchlure/functional/__init__.py` & `torchlure-0.2405.8/src/torchlure/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.7/src/torchlure/modules/__init__.py` & `torchlure-0.2405.8/src/torchlure/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.7/src/torchlure/noise_schedulers.py` & `torchlure-0.2405.8/src/torchlure/noise_schedulers.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.7/src/torchlure/utils.py` & `torchlure-0.2405.8/src/torchlure/utils.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.7/src/torchlure.egg-info/PKG-INFO` & `torchlure-0.2405.8/src/torchlure.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: torchlure
-Version: 0.2405.7
+Version: 0.2405.8
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
 Requires-Dist: gdown>=5.2.0
+Requires-Dist: h5py>=3.11.0
 
 # Torch Lure
 
 
 <a href="https://www.youtube.com/watch?v=wCzCOYCfY9g" target="_blank">
   <img src="http://img.youtube.com/vi/wCzCOYCfY9g/maxresdefault.jpg" alt="Chandelure" style="width: 100%;">
 </a>
@@ -58,20 +59,21 @@
 
 
 
 ```py
 from torchlure.datasets import OfflineRLDataset, D4RLDataset
 
 # Initial usage with download
+# %%
 dataset = D4RLDataset(
-    dataset_id="d4rl_walker2d-expert-2405",
-    d4rl_name="d4rl_walker2d-expert-v2",
-    env_id= "Walker2d-v4",
+    dataset_id= "hopper-medium-expert-v2.2405",
+    d4rl_name= "hopper-medium-expert-v2",
+    env_id= "Hopper-v4",
 )
 
 # if you are download it once
 dataset = D4RLDataset(
-    dataset_id="d4rl_walker2d-expert-2405",
+    dataset_id= "hopper-medium-expert-v2.2405",
 )
 ```
 
 See all datasets [here](https://github.com/pytorch/rl/blob/3a7cf6af2a08089f11e0ed8cad3dd1cea0e253fb/torchrl/data/datasets/d4rl_infos.py)
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: torchlure Version: 0.2405.7 Author-email: fuyutarow
+Metadata-Version: 2.1 Name: torchlure Version: 0.2405.8 Author-email: fuyutarow
 gmail.com> Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure Keywords:
 pytorch Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1 Requires-Dist: numpy>=1.26.4 Requires-Dist: sophia-
 opt>=0.2.2 Requires-Dist: gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28
-Requires-Dist: gdown>=5.2.0 # Torch Lure _[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip
-install git+https://github.com/Farama-Foundation/
-Minari.git@19565bd8cd33f2e4a3a9a8e4db372044b01ea8d3 ``` ```sh pip install
-torchlure ``` # Usage ```py import torchlure as lure # Optimizers lure.SophiaG
-(lr=1e-3, weight_decay=0.2) # Functions lure.tanh_exp(x) lure.TanhExp()
-lure.quantile_loss(y_pred, y_target, quantile=0.5) lure.QuantileLoss
-(quantile=0.5) lure.RMSNrom(dim=256, eps=1e-6) # Noise Scheduler
-lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02, num_timesteps=1000)
-lure.CosineNoiseScheduler(max_beta=0.999, s=0.008, num_timesteps=1000): ``` ###
-Dataset ```py from torchlure.datasets import OfflineRLDataset, D4RLDataset #
-Initial usage with download dataset = D4RLDataset( dataset_id="d4rl_walker2d-
-expert-2405", d4rl_name="d4rl_walker2d-expert-v2", env_id= "Walker2d-v4", ) #
-if you are download it once dataset = D4RLDataset( dataset_id="d4rl_walker2d-
-expert-2405", ) ``` See all datasets [here](https://github.com/pytorch/rl/blob/
+Requires-Dist: gdown>=5.2.0 Requires-Dist: h5py>=3.11.0 # Torch Lure
+_[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip install git+https://github.com/Farama-
+Foundation/Minari.git@19565bd8cd33f2e4a3a9a8e4db372044b01ea8d3 ``` ```sh pip
+install torchlure ``` # Usage ```py import torchlure as lure # Optimizers
+lure.SophiaG(lr=1e-3, weight_decay=0.2) # Functions lure.tanh_exp(x)
+lure.TanhExp() lure.quantile_loss(y_pred, y_target, quantile=0.5)
+lure.QuantileLoss(quantile=0.5) lure.RMSNrom(dim=256, eps=1e-6) # Noise
+Scheduler lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02,
+num_timesteps=1000) lure.CosineNoiseScheduler(max_beta=0.999, s=0.008,
+num_timesteps=1000): ``` ### Dataset ```py from torchlure.datasets import
+OfflineRLDataset, D4RLDataset # Initial usage with download # %% dataset =
+D4RLDataset( dataset_id= "hopper-medium-expert-v2.2405", d4rl_name= "hopper-
+medium-expert-v2", env_id= "Hopper-v4", ) # if you are download it once dataset
+= D4RLDataset( dataset_id= "hopper-medium-expert-v2.2405", ) ``` See all
+datasets [here](https://github.com/pytorch/rl/blob/
 3a7cf6af2a08089f11e0ed8cad3dd1cea0e253fb/torchrl/data/datasets/d4rl_infos.py)
```

### Comparing `torchlure-0.2405.7/src/torchlure.egg-info/SOURCES.txt` & `torchlure-0.2405.8/src/torchlure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

