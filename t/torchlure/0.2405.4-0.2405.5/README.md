# Comparing `tmp/torchlure-0.2405.4.tar.gz` & `tmp/torchlure-0.2405.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlure-0.2405.4.tar", last modified: Fri May 17 11:11:29 2024, max compression
+gzip compressed data, was "torchlure-0.2405.5.tar", last modified: Fri May 17 11:32:04 2024, max compression
```

## Comparing `torchlure-0.2405.4.tar` & `torchlure-0.2405.5.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      133 2024-04-19 13:30:09.000000 torchlure-0.2405.4/.gitignore
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        7 2024-04-19 12:37:01.000000 torchlure-0.2405.4/.python-version
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/.vscode/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      520 2024-05-17 10:31:16.000000 torchlure-0.2405.4/.vscode/extensions.json
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      208 2024-05-17 10:31:16.000000 torchlure-0.2405.4/.vscode/settings.json
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1904 2024-05-17 11:11:29.397067 torchlure-0.2405.4/PKG-INFO
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1417 2024-05-17 11:11:16.000000 torchlure-0.2405.4/README.md
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1044 2024-05-17 10:31:30.000000 torchlure-0.2405.4/pyproject.toml
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       38 2024-05-17 11:11:29.397067 torchlure-0.2405.4/setup.cfg
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      939 2024-05-15 16:17:28.000000 torchlure-0.2405.4/setup.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.387067 torchlure-0.2405.4/src/
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/src/torchlure/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      184 2024-05-17 11:07:37.000000 torchlure-0.2405.4/src/torchlure/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/src/torchlure/datasets/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       46 2024-05-17 10:45:02.000000 torchlure-0.2405.4/src/torchlure/datasets/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/src/torchlure/datasets/d4rl/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     5564 2024-05-17 11:10:50.000000 torchlure-0.2405.4/src/torchlure/datasets/d4rl/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/src/torchlure/datasets/offline_rl/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     4105 2024-05-17 10:47:01.000000 torchlure-0.2405.4/src/torchlure/datasets/offline_rl/__init__.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    11374 2024-05-15 18:42:40.000000 torchlure-0.2405.4/src/torchlure/datasets/offline_rl/minari_ext.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/src/torchlure/functional/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     3567 2024-04-19 13:10:24.000000 torchlure-0.2405.4/src/torchlure/functional/__init__.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/src/torchlure/modules/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1272 2024-04-25 08:19:27.000000 torchlure-0.2405.4/src/torchlure/modules/__init__.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2894 2024-04-19 13:40:26.000000 torchlure-0.2405.4/src/torchlure/noise_schedulers.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       31 2024-04-19 12:53:51.000000 torchlure-0.2405.4/src/torchlure/optim.py
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1481 2024-04-19 12:49:22.000000 torchlure-0.2405.4/src/torchlure/utils.py
-drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:11:29.397067 torchlure-0.2405.4/src/torchlure.egg-info/
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1904 2024-05-17 11:11:29.000000 torchlure-0.2405.4/src/torchlure.egg-info/PKG-INFO
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      636 2024-05-17 11:11:29.000000 torchlure-0.2405.4/src/torchlure.egg-info/SOURCES.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        1 2024-05-17 11:11:29.000000 torchlure-0.2405.4/src/torchlure.egg-info/dependency_links.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       86 2024-05-17 11:11:29.000000 torchlure-0.2405.4/src/torchlure.egg-info/requires.txt
--rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       10 2024-05-17 11:11:29.000000 torchlure-0.2405.4/src/torchlure.egg-info/top_level.txt
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:32:04.567067 torchlure-0.2405.5/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      133 2024-04-19 13:30:09.000000 torchlure-0.2405.5/.gitignore
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        7 2024-04-19 12:37:01.000000 torchlure-0.2405.5/.python-version
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:32:04.567067 torchlure-0.2405.5/.vscode/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      520 2024-05-17 10:31:16.000000 torchlure-0.2405.5/.vscode/extensions.json
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      208 2024-05-17 10:31:16.000000 torchlure-0.2405.5/.vscode/settings.json
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1654 2024-05-17 11:32:04.567067 torchlure-0.2405.5/PKG-INFO
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1167 2024-05-17 11:31:34.000000 torchlure-0.2405.5/README.md
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1044 2024-05-17 10:31:30.000000 torchlure-0.2405.5/pyproject.toml
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       38 2024-05-17 11:32:04.567067 torchlure-0.2405.5/setup.cfg
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      939 2024-05-15 16:17:28.000000 torchlure-0.2405.5/setup.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:32:04.557067 torchlure-0.2405.5/src/
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:32:04.567067 torchlure-0.2405.5/src/torchlure/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      184 2024-05-17 11:31:56.000000 torchlure-0.2405.5/src/torchlure/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:32:04.567067 torchlure-0.2405.5/src/torchlure/datasets/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       46 2024-05-17 10:45:02.000000 torchlure-0.2405.5/src/torchlure/datasets/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:32:04.567067 torchlure-0.2405.5/src/torchlure/datasets/d4rl/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     5216 2024-05-17 11:28:44.000000 torchlure-0.2405.5/src/torchlure/datasets/d4rl/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    22657 2024-05-17 11:28:16.000000 torchlure-0.2405.5/src/torchlure/datasets/d4rl/d4rl_infos.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:32:04.567067 torchlure-0.2405.5/src/torchlure/datasets/offline_rl/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     4105 2024-05-17 10:47:01.000000 torchlure-0.2405.5/src/torchlure/datasets/offline_rl/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)    11374 2024-05-15 18:42:40.000000 torchlure-0.2405.5/src/torchlure/datasets/offline_rl/minari_ext.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:32:04.567067 torchlure-0.2405.5/src/torchlure/functional/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     3567 2024-04-19 13:10:24.000000 torchlure-0.2405.5/src/torchlure/functional/__init__.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:32:04.567067 torchlure-0.2405.5/src/torchlure/modules/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1272 2024-04-25 08:19:27.000000 torchlure-0.2405.5/src/torchlure/modules/__init__.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     2894 2024-04-19 13:40:26.000000 torchlure-0.2405.5/src/torchlure/noise_schedulers.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       31 2024-04-19 12:53:51.000000 torchlure-0.2405.5/src/torchlure/optim.py
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1481 2024-04-19 12:49:22.000000 torchlure-0.2405.5/src/torchlure/utils.py
+drwxr-xr-x   0 fuyutarow  (1000) fuyutarow  (1000)        0 2024-05-17 11:32:04.567067 torchlure-0.2405.5/src/torchlure.egg-info/
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)     1654 2024-05-17 11:32:04.000000 torchlure-0.2405.5/src/torchlure.egg-info/PKG-INFO
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)      678 2024-05-17 11:32:04.000000 torchlure-0.2405.5/src/torchlure.egg-info/SOURCES.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)        1 2024-05-17 11:32:04.000000 torchlure-0.2405.5/src/torchlure.egg-info/dependency_links.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       86 2024-05-17 11:32:04.000000 torchlure-0.2405.5/src/torchlure.egg-info/requires.txt
+-rw-r--r--   0 fuyutarow  (1000) fuyutarow  (1000)       10 2024-05-17 11:32:04.000000 torchlure-0.2405.5/src/torchlure.egg-info/top_level.txt
```

### Comparing `torchlure-0.2405.4/.vscode/extensions.json` & `torchlure-0.2405.5/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.4/PKG-INFO` & `torchlure-0.2405.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlure
-Version: 0.2405.4
+Version: 0.2405.5
 Author-email: fuyutarow <fuyutarow@gmail.com>
 Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure
 Keywords: pytorch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1
@@ -52,37 +52,26 @@
 # Noise Scheduler
 lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02, num_timesteps=1000)
 lure.CosineNoiseScheduler(max_beta=0.999, s=0.008, num_timesteps=1000):
 ```
 
 ### Dataset
 
+
+
 ```py
 from torchlure.datasets import OfflineRLDataset, D4RLDataset
 
-
 # Initial usage with download
 dataset = D4RLDataset(
-    dataset_id="hopper-exppert-2405.1",
-    d4rl_name="d4rl_hopper-expert-v2",
-    env_id="Hopper-v4",
-)
-
-dataset = D4RLDataset(
-    dataset_id="d4rl_halfcheetah-expert-2405",
-    d4rl_name="d4rl_halfcheetah-expert-v2",
-    env_id= "HalfCheetah-v4",
-)
-
-dataset = D4RLDataset(
     dataset_id="d4rl_walker2d-expert-2405",
     d4rl_name="d4rl_walker2d-expert-v2",
     env_id= "Walker2d-v4",
 )
 
 # if you are download it once
 dataset = D4RLDataset(
     dataset_id="d4rl_walker2d-expert-2405",
 )
-
-
 ```
+
+See all datasets [here]()
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchlure Version: 0.2405.4 Author-email: fuyutarow
+Metadata-Version: 2.1 Name: torchlure Version: 0.2405.5 Author-email: fuyutarow
 gmail.com> Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure Keywords:
 pytorch Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1 Requires-Dist: numpy>=1.26.4 Requires-Dist: sophia-
 opt>=0.2.2 Requires-Dist: gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28
 Requires-Dist: gdown>=5.2.0 # Torch Lure _[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip
 install git+https://github.com/Farama-Foundation/
@@ -10,14 +10,11 @@
 torchlure ``` # Usage ```py import torchlure as lure # Optimizers lure.SophiaG
 (lr=1e-3, weight_decay=0.2) # Functions lure.tanh_exp(x) lure.TanhExp()
 lure.quantile_loss(y_pred, y_target, quantile=0.5) lure.QuantileLoss
 (quantile=0.5) lure.RMSNrom(dim=256, eps=1e-6) # Noise Scheduler
 lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02, num_timesteps=1000)
 lure.CosineNoiseScheduler(max_beta=0.999, s=0.008, num_timesteps=1000): ``` ###
 Dataset ```py from torchlure.datasets import OfflineRLDataset, D4RLDataset #
-Initial usage with download dataset = D4RLDataset( dataset_id="hopper-exppert-
-2405.1", d4rl_name="d4rl_hopper-expert-v2", env_id="Hopper-v4", ) dataset =
-D4RLDataset( dataset_id="d4rl_halfcheetah-expert-2405",
-d4rl_name="d4rl_halfcheetah-expert-v2", env_id= "HalfCheetah-v4", ) dataset =
-D4RLDataset( dataset_id="d4rl_walker2d-expert-2405", d4rl_name="d4rl_walker2d-
-expert-v2", env_id= "Walker2d-v4", ) # if you are download it once dataset =
-D4RLDataset( dataset_id="d4rl_walker2d-expert-2405", ) ```
+Initial usage with download dataset = D4RLDataset( dataset_id="d4rl_walker2d-
+expert-2405", d4rl_name="d4rl_walker2d-expert-v2", env_id= "Walker2d-v4", ) #
+if you are download it once dataset = D4RLDataset( dataset_id="d4rl_walker2d-
+expert-2405", ) ``` See all datasets [here]()
```

### Comparing `torchlure-0.2405.4/README.md` & `torchlure-0.2405.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -36,37 +36,26 @@
 # Noise Scheduler
 lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02, num_timesteps=1000)
 lure.CosineNoiseScheduler(max_beta=0.999, s=0.008, num_timesteps=1000):
 ```
 
 ### Dataset
 
+
+
 ```py
 from torchlure.datasets import OfflineRLDataset, D4RLDataset
 
-
 # Initial usage with download
 dataset = D4RLDataset(
-    dataset_id="hopper-exppert-2405.1",
-    d4rl_name="d4rl_hopper-expert-v2",
-    env_id="Hopper-v4",
-)
-
-dataset = D4RLDataset(
-    dataset_id="d4rl_halfcheetah-expert-2405",
-    d4rl_name="d4rl_halfcheetah-expert-v2",
-    env_id= "HalfCheetah-v4",
-)
-
-dataset = D4RLDataset(
     dataset_id="d4rl_walker2d-expert-2405",
     d4rl_name="d4rl_walker2d-expert-v2",
     env_id= "Walker2d-v4",
 )
 
 # if you are download it once
 dataset = D4RLDataset(
     dataset_id="d4rl_walker2d-expert-2405",
 )
+```
 
-
-```
+See all datasets [here]()
```

#### html2text {}

```diff
@@ -4,14 +4,11 @@
 lure.SophiaG(lr=1e-3, weight_decay=0.2) # Functions lure.tanh_exp(x)
 lure.TanhExp() lure.quantile_loss(y_pred, y_target, quantile=0.5)
 lure.QuantileLoss(quantile=0.5) lure.RMSNrom(dim=256, eps=1e-6) # Noise
 Scheduler lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02,
 num_timesteps=1000) lure.CosineNoiseScheduler(max_beta=0.999, s=0.008,
 num_timesteps=1000): ``` ### Dataset ```py from torchlure.datasets import
 OfflineRLDataset, D4RLDataset # Initial usage with download dataset =
-D4RLDataset( dataset_id="hopper-exppert-2405.1", d4rl_name="d4rl_hopper-expert-
-v2", env_id="Hopper-v4", ) dataset = D4RLDataset( dataset_id="d4rl_halfcheetah-
-expert-2405", d4rl_name="d4rl_halfcheetah-expert-v2", env_id= "HalfCheetah-v4",
-) dataset = D4RLDataset( dataset_id="d4rl_walker2d-expert-2405",
-d4rl_name="d4rl_walker2d-expert-v2", env_id= "Walker2d-v4", ) # if you are
-download it once dataset = D4RLDataset( dataset_id="d4rl_walker2d-expert-2405",
-) ```
+D4RLDataset( dataset_id="d4rl_walker2d-expert-2405", d4rl_name="d4rl_walker2d-
+expert-v2", env_id= "Walker2d-v4", ) # if you are download it once dataset =
+D4RLDataset( dataset_id="d4rl_walker2d-expert-2405", ) ``` See all datasets
+[here]()
```

### Comparing `torchlure-0.2405.4/pyproject.toml` & `torchlure-0.2405.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.4/setup.py` & `torchlure-0.2405.5/setup.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.4/src/torchlure/datasets/d4rl/__init__.py` & `torchlure-0.2405.5/src/torchlure/datasets/d4rl/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,37 +5,34 @@
 import gymnasium as gym
 import minari
 from minari.data_collector.episode_buffer import EpisodeBuffer
 from minari.dataset._storages.hdf5_storage import HDF5Storage
 from minari.utils import create_dataset_from_buffers
 from torch.utils.data import DataLoader, Dataset
 
+from .d4rl_infos import D4RL_DATASETS
+
 
 def download_d4rl_dataset(dataset_name):
-    datasets = {
-        "d4rl_halfcheetah-expert-v2": "https://drive.google.com/drive/folders/1YcUMTS7cMrUP8KJ6aQL87D9uYnrvGT02?usp=drive_link",
-        "d4rl_hopper-expert-v2": "https://drive.google.com/drive/folders/1upUt_aCRc3MCWhfVwpDlnW7YoVFEHre9?usp=drive_link",
-        "d4rl_walker2d-expert-v2": "https://drive.google.com/drive/folders/1ncu2DEhADWQBH6EeU_SrywQm8ETMM15M?usp=drive_link",
-    }
     assert (
-        dataset_name in datasets
-    ), f"Dataset {dataset_name} not found in available datasets: {datasets.keys()}"
+        dataset_name in D4RL_DATASETS
+    ), f"Dataset {dataset_name} not found in available datasets: {D4RL_DATASETS.keys()}"
 
     # Create directories if they do not exist
     minari_dir = Path.home() / ".minari"
     datasets_dir = minari_dir / "datasets"
     minari_dir.mkdir(parents=True, exist_ok=True)
     datasets_dir.mkdir(parents=True, exist_ok=True)
 
     # Download dataset if it does not exist already
     target_path = datasets_dir / dataset_name
     if target_path.exists():
         print(f"{dataset_name} already exists at {target_path}, skipping download.")
     else:
-        url = datasets[dataset_name]
+        url = D4RL_DATASETS[dataset_name]
         gdown.download_folder(
             url=url, output=str(target_path), quiet=False, use_cookies=False
         )
 
 
 def collect_all_episodes(storage: HDF5Storage) -> List[Dict[str, Any]]:
     """Collect and return all episodes from the storage."""
```

### Comparing `torchlure-0.2405.4/src/torchlure/datasets/offline_rl/__init__.py` & `torchlure-0.2405.5/src/torchlure/datasets/offline_rl/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.4/src/torchlure/datasets/offline_rl/minari_ext.py` & `torchlure-0.2405.5/src/torchlure/datasets/offline_rl/minari_ext.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.4/src/torchlure/functional/__init__.py` & `torchlure-0.2405.5/src/torchlure/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.4/src/torchlure/modules/__init__.py` & `torchlure-0.2405.5/src/torchlure/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.4/src/torchlure/noise_schedulers.py` & `torchlure-0.2405.5/src/torchlure/noise_schedulers.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.4/src/torchlure/utils.py` & `torchlure-0.2405.5/src/torchlure/utils.py`

 * *Files identical despite different names*

### Comparing `torchlure-0.2405.4/src/torchlure.egg-info/PKG-INFO` & `torchlure-0.2405.5/src/torchlure.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlure
-Version: 0.2405.4
+Version: 0.2405.5
 Author-email: fuyutarow <fuyutarow@gmail.com>
 Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure
 Keywords: pytorch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1
@@ -52,37 +52,26 @@
 # Noise Scheduler
 lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02, num_timesteps=1000)
 lure.CosineNoiseScheduler(max_beta=0.999, s=0.008, num_timesteps=1000):
 ```
 
 ### Dataset
 
+
+
 ```py
 from torchlure.datasets import OfflineRLDataset, D4RLDataset
 
-
 # Initial usage with download
 dataset = D4RLDataset(
-    dataset_id="hopper-exppert-2405.1",
-    d4rl_name="d4rl_hopper-expert-v2",
-    env_id="Hopper-v4",
-)
-
-dataset = D4RLDataset(
-    dataset_id="d4rl_halfcheetah-expert-2405",
-    d4rl_name="d4rl_halfcheetah-expert-v2",
-    env_id= "HalfCheetah-v4",
-)
-
-dataset = D4RLDataset(
     dataset_id="d4rl_walker2d-expert-2405",
     d4rl_name="d4rl_walker2d-expert-v2",
     env_id= "Walker2d-v4",
 )
 
 # if you are download it once
 dataset = D4RLDataset(
     dataset_id="d4rl_walker2d-expert-2405",
 )
-
-
 ```
+
+See all datasets [here]()
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchlure Version: 0.2405.4 Author-email: fuyutarow
+Metadata-Version: 2.1 Name: torchlure Version: 0.2405.5 Author-email: fuyutarow
 gmail.com> Project-URL: Homepage, https://github.com/fuyutarow/torchlure
 Project-URL: Repository, https://github.com/fuyutarow/torchlure Keywords:
 pytorch Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Requires-Dist: torch>=2.1 Requires-Dist: numpy>=1.26.4 Requires-Dist: sophia-
 opt>=0.2.2 Requires-Dist: gymnasium>=0.29.1 Requires-Dist: jax>=0.4.28
 Requires-Dist: gdown>=5.2.0 # Torch Lure _[_C_h_a_n_d_e_l_u_r_e_]# Depndencies ``` pip
 install git+https://github.com/Farama-Foundation/
@@ -10,14 +10,11 @@
 torchlure ``` # Usage ```py import torchlure as lure # Optimizers lure.SophiaG
 (lr=1e-3, weight_decay=0.2) # Functions lure.tanh_exp(x) lure.TanhExp()
 lure.quantile_loss(y_pred, y_target, quantile=0.5) lure.QuantileLoss
 (quantile=0.5) lure.RMSNrom(dim=256, eps=1e-6) # Noise Scheduler
 lure.LinearNoiseScheduler(beta=1e-4, beta_end=0.02, num_timesteps=1000)
 lure.CosineNoiseScheduler(max_beta=0.999, s=0.008, num_timesteps=1000): ``` ###
 Dataset ```py from torchlure.datasets import OfflineRLDataset, D4RLDataset #
-Initial usage with download dataset = D4RLDataset( dataset_id="hopper-exppert-
-2405.1", d4rl_name="d4rl_hopper-expert-v2", env_id="Hopper-v4", ) dataset =
-D4RLDataset( dataset_id="d4rl_halfcheetah-expert-2405",
-d4rl_name="d4rl_halfcheetah-expert-v2", env_id= "HalfCheetah-v4", ) dataset =
-D4RLDataset( dataset_id="d4rl_walker2d-expert-2405", d4rl_name="d4rl_walker2d-
-expert-v2", env_id= "Walker2d-v4", ) # if you are download it once dataset =
-D4RLDataset( dataset_id="d4rl_walker2d-expert-2405", ) ```
+Initial usage with download dataset = D4RLDataset( dataset_id="d4rl_walker2d-
+expert-2405", d4rl_name="d4rl_walker2d-expert-v2", env_id= "Walker2d-v4", ) #
+if you are download it once dataset = D4RLDataset( dataset_id="d4rl_walker2d-
+expert-2405", ) ``` See all datasets [here]()
```

### Comparing `torchlure-0.2405.4/src/torchlure.egg-info/SOURCES.txt` & `torchlure-0.2405.5/src/torchlure.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 src/torchlure.egg-info/PKG-INFO
 src/torchlure.egg-info/SOURCES.txt
 src/torchlure.egg-info/dependency_links.txt
 src/torchlure.egg-info/requires.txt
 src/torchlure.egg-info/top_level.txt
 src/torchlure/datasets/__init__.py
 src/torchlure/datasets/d4rl/__init__.py
+src/torchlure/datasets/d4rl/d4rl_infos.py
 src/torchlure/datasets/offline_rl/__init__.py
 src/torchlure/datasets/offline_rl/minari_ext.py
 src/torchlure/functional/__init__.py
 src/torchlure/modules/__init__.py
```

