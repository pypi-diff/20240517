# Comparing `tmp/e2e_sae-0.0.2.tar.gz` & `tmp/e2e_sae-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2e_sae-0.0.2.tar", last modified: Mon May 13 10:23:42 2024, max compression
+gzip compressed data, was "e2e_sae-0.0.3.tar", last modified: Fri May 17 20:17:18 2024, max compression
```

## Comparing `e2e_sae-0.0.2.tar` & `e2e_sae-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-13 10:23:42.564823 e2e_sae-0.0.2/
--rw-r--r--   0 dan        (501) staff       (20)     1071 2024-04-21 12:55:51.000000 e2e_sae-0.0.2/LICENSE
--rw-r--r--   0 dan        (501) staff       (20)     4560 2024-05-13 10:23:42.564607 e2e_sae-0.0.2/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     3597 2024-05-13 10:20:50.000000 e2e_sae-0.0.2/README.md
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-13 10:23:42.559827 e2e_sae-0.0.2/e2e_sae/
--rw-r--r--   0 dan        (501) staff       (20)       56 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/e2e_sae/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     3027 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/e2e_sae/data.py
--rw-r--r--   0 dan        (501) staff       (20)     1605 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/e2e_sae/hooks.py
--rw-r--r--   0 dan        (501) staff       (20)     2577 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/e2e_sae/loader.py
--rw-r--r--   0 dan        (501) staff       (20)     1948 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/e2e_sae/log.py
--rw-r--r--   0 dan        (501) staff       (20)    11196 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/e2e_sae/losses.py
--rw-r--r--   0 dan        (501) staff       (20)    11914 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/e2e_sae/metrics.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-13 10:23:42.561633 e2e_sae-0.0.2/e2e_sae/models/
--rw-r--r--   0 dan        (501) staff       (20)        0 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/e2e_sae/models/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     5364 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/e2e_sae/models/mlp.py
--rw-r--r--   0 dan        (501) staff       (20)     3132 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/e2e_sae/models/sparsifiers.py
--rw-r--r--   0 dan        (501) staff       (20)    20645 2024-05-13 08:36:37.000000 e2e_sae-0.0.2/e2e_sae/models/transformers.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-13 10:23:42.562671 e2e_sae-0.0.2/e2e_sae/scripts/
--rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-10 16:49:48.000000 e2e_sae-0.0.2/e2e_sae/scripts/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    25338 2024-05-13 09:54:46.000000 e2e_sae-0.0.2/e2e_sae/scripts/autointerp.py
--rw-r--r--   0 dan        (501) staff       (20)    13657 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/e2e_sae/scripts/upload_hf_dataset.py
--rw-r--r--   0 dan        (501) staff       (20)      151 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/e2e_sae/settings.py
--rw-r--r--   0 dan        (501) staff       (20)     1692 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/e2e_sae/types.py
--rw-r--r--   0 dan        (501) staff       (20)    12862 2024-05-13 08:33:52.000000 e2e_sae-0.0.2/e2e_sae/utils.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-13 10:23:42.564134 e2e_sae-0.0.2/e2e_sae.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)     4560 2024-05-13 10:23:42.000000 e2e_sae-0.0.2/e2e_sae.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      681 2024-05-13 10:23:42.000000 e2e_sae-0.0.2/e2e_sae.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-13 10:23:42.000000 e2e_sae-0.0.2/e2e_sae.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)      339 2024-05-13 10:23:42.000000 e2e_sae-0.0.2/e2e_sae.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)        8 2024-05-13 10:23:42.000000 e2e_sae-0.0.2/e2e_sae.egg-info/top_level.txt
--rw-r--r--   0 dan        (501) staff       (20)     2319 2024-05-13 10:18:39.000000 e2e_sae-0.0.2/pyproject.toml
--rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-13 10:23:42.564880 e2e_sae-0.0.2/setup.cfg
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-13 10:23:42.563898 e2e_sae-0.0.2/tests/
--rw-r--r--   0 dan        (501) staff       (20)     1900 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/tests/test_mlp.py
--rw-r--r--   0 dan        (501) staff       (20)     8053 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/tests/test_sae.py
--rw-r--r--   0 dan        (501) staff       (20)     2534 2024-05-13 09:31:13.000000 e2e_sae-0.0.2/tests/test_train_tlens_saes.py
--rw-r--r--   0 dan        (501) staff       (20)     1064 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/tests/test_transformer.py
--rw-r--r--   0 dan        (501) staff       (20)     2103 2024-04-22 15:36:40.000000 e2e_sae-0.0.2/tests/test_utils.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-17 20:17:18.002145 e2e_sae-0.0.3/
+-rw-r--r--   0 dan        (501) staff       (20)     1071 2024-04-21 12:55:51.000000 e2e_sae-0.0.3/LICENSE
+-rw-r--r--   0 dan        (501) staff       (20)     4769 2024-05-17 20:17:18.001778 e2e_sae-0.0.3/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     3724 2024-05-17 12:29:31.000000 e2e_sae-0.0.3/README.md
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-17 20:17:17.998436 e2e_sae-0.0.3/e2e_sae/
+-rw-r--r--   0 dan        (501) staff       (20)       56 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     3027 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/data.py
+-rw-r--r--   0 dan        (501) staff       (20)     1605 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/hooks.py
+-rw-r--r--   0 dan        (501) staff       (20)     2577 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/loader.py
+-rw-r--r--   0 dan        (501) staff       (20)     1948 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/log.py
+-rw-r--r--   0 dan        (501) staff       (20)    11196 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/losses.py
+-rw-r--r--   0 dan        (501) staff       (20)    11914 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/metrics.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-17 20:17:17.999876 e2e_sae-0.0.3/e2e_sae/models/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/models/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     5364 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/models/mlp.py
+-rw-r--r--   0 dan        (501) staff       (20)     3132 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/models/sparsifiers.py
+-rw-r--r--   0 dan        (501) staff       (20)    20943 2024-05-17 10:10:13.000000 e2e_sae-0.0.3/e2e_sae/models/transformers.py
+-rw-r--r--   0 dan        (501) staff       (20)    11142 2024-05-17 16:32:10.000000 e2e_sae-0.0.3/e2e_sae/plotting.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-17 20:17:18.000205 e2e_sae-0.0.3/e2e_sae/scripts/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-10 16:49:48.000000 e2e_sae-0.0.3/e2e_sae/scripts/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)    13657 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/scripts/upload_hf_dataset.py
+-rw-r--r--   0 dan        (501) staff       (20)      151 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/settings.py
+-rw-r--r--   0 dan        (501) staff       (20)     1692 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/e2e_sae/types.py
+-rw-r--r--   0 dan        (501) staff       (20)    12944 2024-05-17 10:10:13.000000 e2e_sae-0.0.3/e2e_sae/utils.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-17 20:17:18.001227 e2e_sae-0.0.3/e2e_sae.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)     4769 2024-05-17 20:17:17.000000 e2e_sae-0.0.3/e2e_sae.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      671 2024-05-17 20:17:17.000000 e2e_sae-0.0.3/e2e_sae.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-17 20:17:17.000000 e2e_sae-0.0.3/e2e_sae.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)      391 2024-05-17 20:17:17.000000 e2e_sae-0.0.3/e2e_sae.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)        8 2024-05-17 20:17:17.000000 e2e_sae-0.0.3/e2e_sae.egg-info/top_level.txt
+-rw-r--r--   0 dan        (501) staff       (20)     2289 2024-05-17 20:16:02.000000 e2e_sae-0.0.3/pyproject.toml
+-rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-17 20:17:18.002203 e2e_sae-0.0.3/setup.cfg
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-17 20:17:18.001012 e2e_sae-0.0.3/tests/
+-rw-r--r--   0 dan        (501) staff       (20)     1900 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/tests/test_mlp.py
+-rw-r--r--   0 dan        (501) staff       (20)     8053 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/tests/test_sae.py
+-rw-r--r--   0 dan        (501) staff       (20)     2534 2024-05-14 08:17:02.000000 e2e_sae-0.0.3/tests/test_train_tlens_saes.py
+-rw-r--r--   0 dan        (501) staff       (20)     1064 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/tests/test_transformer.py
+-rw-r--r--   0 dan        (501) staff       (20)     2103 2024-04-22 15:36:40.000000 e2e_sae-0.0.3/tests/test_utils.py
```

### Comparing `e2e_sae-0.0.2/LICENSE` & `e2e_sae-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.2/PKG-INFO` & `e2e_sae-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2e_sae
-Version: 0.0.2
+Version: 0.0.3
 Summary: Repo for training sparse autoencoders end-to-end
 Project-URL: repository, https://github.com/ApolloResearch/e2e_sae
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch~=2.2.0
 Requires-Dist: torchvision~=0.17.0
@@ -17,32 +17,34 @@
 Requires-Dist: ipykernel~=6.29.0
 Requires-Dist: transformer-lens~=1.14.0
 Requires-Dist: jaxtyping~=0.2.25
 Requires-Dist: python-dotenv~=1.0.1
 Requires-Dist: zstandard~=0.22.0
 Requires-Dist: matplotlib~=3.5.3
 Requires-Dist: seaborn~=0.13.2
+Requires-Dist: umap-learn~=0.5.6
 Requires-Dist: tenacity~=8.2.3
 Requires-Dist: statsmodels~=0.14.2
+Requires-Dist: automated-interpretability~=0.0.3
 Provides-Extra: dev
 Requires-Dist: ruff~=0.1.14; extra == "dev"
-Requires-Dist: pyright~=1.1.360; extra == "dev"
+Requires-Dist: pyright~=1.1.362; extra == "dev"
 Requires-Dist: pre-commit~=3.6.0; extra == "dev"
 
 # e2e_sae
 
 This library is used to train and evaluate Sparse Autoencoders (SAEs). It handles the following
 training types:
-- End-to-end (e2e): Loss function includes sparsity and final model kl_divergence.
-- e2e + future reconstruction: Loss function includes sparsity, final model kl_divergence, and MSE
-    at future layers.
-- Local (i.e. vanilla SAEs): Loss function includes sparsity and MSE at the SAE layer
+- e2e (end-to-end): Loss function includes sparsity and final model kl_divergence.
+- e2e + downstream reconstruction: Loss function includes sparsity, final model kl_divergence, and MSE
+    at downstream layers.
+- local (i.e. vanilla SAEs): Loss function includes sparsity and MSE at the SAE layer
 - Any combination of the above.
 
-See [TODO: add paper] which argues for training SAEs e2e rather than locally. All SAEs presented in the paper can be found at https://wandb.ai/sparsify/gpt2 and can be loaded using this library.
+See our [paper](https://publications.apolloresearch.ai/end_to_end_sparse_dictionary_learning) which argues for training SAEs e2e rather than locally. All SAEs presented in the paper can be found at https://wandb.ai/sparsify/gpt2 and can be loaded using this library.
 
 ## Usage
 ### Installation
 ```bash
 pip install e2e_sae
 ```
 
@@ -67,28 +69,30 @@
 from Weights and Biases or locally by running
 ```python
 from e2e_sae import SAETransformer
 model = SAETransformer.from_wandb("<entity/project/run_id>")
 # or, if stored locally
 model = SAETransformer.from_local_path("/path/to/checkpoint/dir") 
 ```
-Note that all runs in the [TODO: Add e2e paper]() can be loaded this way (e.g.
-[sparsify/gpt2/tvj2owza](https://wandb.ai/sparsify/gpt2/runs/tvj2owza)).
+All runs in our
+[paper](https://publications.apolloresearch.ai/end_to_end_sparse_dictionary_learning)
+can be loaded this way (e.g.[sparsify/gpt2/tvj2owza](https://wandb.ai/sparsify/gpt2/runs/tvj2owza)).
 
 
 This will instantiate a `SAETransformer` class, which contains a TransformerLens model with SAEs
 attached. To do a forward pass without SAEs, use the `forward_raw` method, to do a forward pass with
 SAEs, use the `forward` method (or simply call the SAETansformer instance).
 
+The dictionary elements of an SAE can be accessed via `SAE.dict_elements`. This is will normalize
+the decoder elements to have norm 1.
 
-### Autointerpretability
-To run autointerpretability on SAEs uploaded to Neuronpedia, use the script
-`e2e_sae/scripts/autointerp.py`. Note that this will require you to first install Johnny Lin's fork
-of OpenAI's `neuron_explainer` package with `pip install
-git+https://github.com/hijohnnylin/automated-interpretability.git`.
+### Analysis
+To reproduce all of the analysis in our
+[paper](https://publications.apolloresearch.ai/end_to_end_sparse_dictionary_learning) use the
+scripts in `e2e_sae/scripts/analysis/`.
 
 ## Contributing
 Developer dependencies are installed with `make install-dev`, which will also install pre-commit
 hooks.
 
 Suggested extensions and settings for VSCode are provided in `.vscode/`. To use the suggested
 settings, copy `.vscode/settings-example.json` to `.vscode/settings.json`.
```

### Comparing `e2e_sae-0.0.2/README.md` & `e2e_sae-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # e2e_sae
 
 This library is used to train and evaluate Sparse Autoencoders (SAEs). It handles the following
 training types:
-- End-to-end (e2e): Loss function includes sparsity and final model kl_divergence.
-- e2e + future reconstruction: Loss function includes sparsity, final model kl_divergence, and MSE
-    at future layers.
-- Local (i.e. vanilla SAEs): Loss function includes sparsity and MSE at the SAE layer
+- e2e (end-to-end): Loss function includes sparsity and final model kl_divergence.
+- e2e + downstream reconstruction: Loss function includes sparsity, final model kl_divergence, and MSE
+    at downstream layers.
+- local (i.e. vanilla SAEs): Loss function includes sparsity and MSE at the SAE layer
 - Any combination of the above.
 
-See [TODO: add paper] which argues for training SAEs e2e rather than locally. All SAEs presented in the paper can be found at https://wandb.ai/sparsify/gpt2 and can be loaded using this library.
+See our [paper](https://publications.apolloresearch.ai/end_to_end_sparse_dictionary_learning) which argues for training SAEs e2e rather than locally. All SAEs presented in the paper can be found at https://wandb.ai/sparsify/gpt2 and can be loaded using this library.
 
 ## Usage
 ### Installation
 ```bash
 pip install e2e_sae
 ```
 
@@ -37,28 +37,30 @@
 from Weights and Biases or locally by running
 ```python
 from e2e_sae import SAETransformer
 model = SAETransformer.from_wandb("<entity/project/run_id>")
 # or, if stored locally
 model = SAETransformer.from_local_path("/path/to/checkpoint/dir") 
 ```
-Note that all runs in the [TODO: Add e2e paper]() can be loaded this way (e.g.
-[sparsify/gpt2/tvj2owza](https://wandb.ai/sparsify/gpt2/runs/tvj2owza)).
+All runs in our
+[paper](https://publications.apolloresearch.ai/end_to_end_sparse_dictionary_learning)
+can be loaded this way (e.g.[sparsify/gpt2/tvj2owza](https://wandb.ai/sparsify/gpt2/runs/tvj2owza)).
 
 
 This will instantiate a `SAETransformer` class, which contains a TransformerLens model with SAEs
 attached. To do a forward pass without SAEs, use the `forward_raw` method, to do a forward pass with
 SAEs, use the `forward` method (or simply call the SAETansformer instance).
 
+The dictionary elements of an SAE can be accessed via `SAE.dict_elements`. This is will normalize
+the decoder elements to have norm 1.
 
-### Autointerpretability
-To run autointerpretability on SAEs uploaded to Neuronpedia, use the script
-`e2e_sae/scripts/autointerp.py`. Note that this will require you to first install Johnny Lin's fork
-of OpenAI's `neuron_explainer` package with `pip install
-git+https://github.com/hijohnnylin/automated-interpretability.git`.
+### Analysis
+To reproduce all of the analysis in our
+[paper](https://publications.apolloresearch.ai/end_to_end_sparse_dictionary_learning) use the
+scripts in `e2e_sae/scripts/analysis/`.
 
 ## Contributing
 Developer dependencies are installed with `make install-dev`, which will also install pre-commit
 hooks.
 
 Suggested extensions and settings for VSCode are provided in `.vscode/`. To use the suggested
 settings, copy `.vscode/settings-example.json` to `.vscode/settings.json`.
```

### Comparing `e2e_sae-0.0.2/e2e_sae/data.py` & `e2e_sae-0.0.3/e2e_sae/data.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.2/e2e_sae/hooks.py` & `e2e_sae-0.0.3/e2e_sae/hooks.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.2/e2e_sae/loader.py` & `e2e_sae-0.0.3/e2e_sae/loader.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.2/e2e_sae/log.py` & `e2e_sae-0.0.3/e2e_sae/log.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.2/e2e_sae/losses.py` & `e2e_sae-0.0.3/e2e_sae/losses.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.2/e2e_sae/metrics.py` & `e2e_sae-0.0.3/e2e_sae/metrics.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.2/e2e_sae/models/mlp.py` & `e2e_sae-0.0.3/e2e_sae/models/mlp.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.2/e2e_sae/models/sparsifiers.py` & `e2e_sae-0.0.3/e2e_sae/models/sparsifiers.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.2/e2e_sae/models/transformers.py` & `e2e_sae-0.0.3/e2e_sae/models/transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from functools import partial
 from pathlib import Path
 from typing import Any, Literal, cast
 
 import torch
 import tqdm
 import wandb
@@ -56,15 +57,15 @@
                 init_decoder_orthogonal=init_decoder_orthogonal,
             )
 
     def forward_raw(
         self,
         tokens: Int[Tensor, "batch pos"],
         run_entire_model: bool,
-        final_layer: int | None,
+        final_layer: int | None = None,
         cache_positions: list[str] | None = None,
     ) -> tuple[
         Float[torch.Tensor, "batch pos d_vocab"], dict[str, Float[torch.Tensor, "batch pos dim"]]
     ]:
         """Forward pass through the original transformer without the SAEs.
 
         Args:
@@ -73,14 +74,17 @@
             final_layer: The layer to stop at if `run_entire_model` is False.
             cache_positions: Hooks to cache activations at in addition to the SAE positions.
 
         Returns:
             - The logits of the original model.
             - The activations of the original model.
         """
+        assert (
+            not run_entire_model or final_layer is None
+        ), "Can't specify both run_entire_model and final_layer"
         all_hook_names = self.raw_sae_positions + (cache_positions or [])
         orig_logits, orig_acts = self.tlens_model.run_with_cache(
             tokens,
             names_filter=all_hook_names,
             return_cache_object=False,
             stop_at_layer=None if run_entire_model else final_layer,
         )
@@ -368,28 +372,31 @@
 
         Returns:
             An instance of the SAETransformer class loaded from the specified wandb run.
         """
         api = wandb.Api()
         run: Run = api.run(wandb_project_run_id)
 
+        cache_dir = Path(os.environ.get("SAE_CACHE_DIR", "/tmp/"))
+        model_cache_dir = cache_dir / wandb_project_run_id
+
         train_config_file_remote = [
             file for file in run.files() if file.name.endswith("final_config.yaml")
         ][0]
 
         train_config_file = train_config_file_remote.download(
-            exist_ok=True, replace=True, root="/tmp/"
+            exist_ok=True, replace=True, root=model_cache_dir
         ).name
 
         checkpoints = [file for file in run.files() if file.name.endswith(".pt")]
         latest_checkpoint_remote = sorted(
             checkpoints, key=lambda x: int(x.name.split(".pt")[0].split("_")[-1])
         )[-1]
         latest_checkpoint_file = latest_checkpoint_remote.download(
-            exist_ok=True, replace=True, root="/tmp/"
+            exist_ok=True, replace=True, root=model_cache_dir
         ).name
         assert latest_checkpoint_file is not None, "Failed to download the latest checkpoint."
 
         return cls.from_local_path(
             checkpoint_file=latest_checkpoint_file, config_file=train_config_file
         )
```

### Comparing `e2e_sae-0.0.2/e2e_sae/scripts/upload_hf_dataset.py` & `e2e_sae-0.0.3/e2e_sae/scripts/upload_hf_dataset.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.2/e2e_sae/types.py` & `e2e_sae-0.0.3/e2e_sae/types.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.2/e2e_sae/utils.py` & `e2e_sae-0.0.3/e2e_sae/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,27 +138,29 @@
         >>> bar2 = replace_pydantic_model(bar, {"foo": {"a": 3}})
         >>> bar2
         Bar(foo=Foo(a=3, b=2))
     """
     return model.__class__(**deep_update(model.model_dump(), *updates))
 
 
-def filter_names(all_names: list[str], filter_names: list[str]) -> list[str]:
+def filter_names(all_names: list[str], filter_names: list[str] | str) -> list[str]:
     """Use filter_names to filter `all_names` by partial match.
 
     The filtering is done by checking if any of the filter_names are in the all_names. Partial
     matches are allowed. E.g. "hook_resid_pre" matches ["blocks.0.hook_resid_pre",
     "blocks.1.hook_resid_pre", ...].
 
     Args:
         all_names: The names to filter.
         filter_names: The names to use to filter all_names by partial match.
     Returns:
         The filtered names.
     """
+    if isinstance(filter_names, str):
+        filter_names = [filter_names]
     return [name for name in all_names if any(filter_name in name for filter_name in filter_names)]
 
 
 def get_hook_shapes(tlens_model: HookedTransformer, hook_names: list[str]) -> dict[str, list[int]]:
     """Get the shapes of activations at the hook points labelled by hook_names"""
     # Sadly I can't see any way to easily get the shapes of activations at hook_points without
     # actually running the model.
```

### Comparing `e2e_sae-0.0.2/e2e_sae.egg-info/PKG-INFO` & `e2e_sae-0.0.3/e2e_sae.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2e_sae
-Version: 0.0.2
+Version: 0.0.3
 Summary: Repo for training sparse autoencoders end-to-end
 Project-URL: repository, https://github.com/ApolloResearch/e2e_sae
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch~=2.2.0
 Requires-Dist: torchvision~=0.17.0
@@ -17,32 +17,34 @@
 Requires-Dist: ipykernel~=6.29.0
 Requires-Dist: transformer-lens~=1.14.0
 Requires-Dist: jaxtyping~=0.2.25
 Requires-Dist: python-dotenv~=1.0.1
 Requires-Dist: zstandard~=0.22.0
 Requires-Dist: matplotlib~=3.5.3
 Requires-Dist: seaborn~=0.13.2
+Requires-Dist: umap-learn~=0.5.6
 Requires-Dist: tenacity~=8.2.3
 Requires-Dist: statsmodels~=0.14.2
+Requires-Dist: automated-interpretability~=0.0.3
 Provides-Extra: dev
 Requires-Dist: ruff~=0.1.14; extra == "dev"
-Requires-Dist: pyright~=1.1.360; extra == "dev"
+Requires-Dist: pyright~=1.1.362; extra == "dev"
 Requires-Dist: pre-commit~=3.6.0; extra == "dev"
 
 # e2e_sae
 
 This library is used to train and evaluate Sparse Autoencoders (SAEs). It handles the following
 training types:
-- End-to-end (e2e): Loss function includes sparsity and final model kl_divergence.
-- e2e + future reconstruction: Loss function includes sparsity, final model kl_divergence, and MSE
-    at future layers.
-- Local (i.e. vanilla SAEs): Loss function includes sparsity and MSE at the SAE layer
+- e2e (end-to-end): Loss function includes sparsity and final model kl_divergence.
+- e2e + downstream reconstruction: Loss function includes sparsity, final model kl_divergence, and MSE
+    at downstream layers.
+- local (i.e. vanilla SAEs): Loss function includes sparsity and MSE at the SAE layer
 - Any combination of the above.
 
-See [TODO: add paper] which argues for training SAEs e2e rather than locally. All SAEs presented in the paper can be found at https://wandb.ai/sparsify/gpt2 and can be loaded using this library.
+See our [paper](https://publications.apolloresearch.ai/end_to_end_sparse_dictionary_learning) which argues for training SAEs e2e rather than locally. All SAEs presented in the paper can be found at https://wandb.ai/sparsify/gpt2 and can be loaded using this library.
 
 ## Usage
 ### Installation
 ```bash
 pip install e2e_sae
 ```
 
@@ -67,28 +69,30 @@
 from Weights and Biases or locally by running
 ```python
 from e2e_sae import SAETransformer
 model = SAETransformer.from_wandb("<entity/project/run_id>")
 # or, if stored locally
 model = SAETransformer.from_local_path("/path/to/checkpoint/dir") 
 ```
-Note that all runs in the [TODO: Add e2e paper]() can be loaded this way (e.g.
-[sparsify/gpt2/tvj2owza](https://wandb.ai/sparsify/gpt2/runs/tvj2owza)).
+All runs in our
+[paper](https://publications.apolloresearch.ai/end_to_end_sparse_dictionary_learning)
+can be loaded this way (e.g.[sparsify/gpt2/tvj2owza](https://wandb.ai/sparsify/gpt2/runs/tvj2owza)).
 
 
 This will instantiate a `SAETransformer` class, which contains a TransformerLens model with SAEs
 attached. To do a forward pass without SAEs, use the `forward_raw` method, to do a forward pass with
 SAEs, use the `forward` method (or simply call the SAETansformer instance).
 
+The dictionary elements of an SAE can be accessed via `SAE.dict_elements`. This is will normalize
+the decoder elements to have norm 1.
 
-### Autointerpretability
-To run autointerpretability on SAEs uploaded to Neuronpedia, use the script
-`e2e_sae/scripts/autointerp.py`. Note that this will require you to first install Johnny Lin's fork
-of OpenAI's `neuron_explainer` package with `pip install
-git+https://github.com/hijohnnylin/automated-interpretability.git`.
+### Analysis
+To reproduce all of the analysis in our
+[paper](https://publications.apolloresearch.ai/end_to_end_sparse_dictionary_learning) use the
+scripts in `e2e_sae/scripts/analysis/`.
 
 ## Contributing
 Developer dependencies are installed with `make install-dev`, which will also install pre-commit
 hooks.
 
 Suggested extensions and settings for VSCode are provided in `.vscode/`. To use the suggested
 settings, copy `.vscode/settings-example.json` to `.vscode/settings.json`.
```

### Comparing `e2e_sae-0.0.2/e2e_sae.egg-info/SOURCES.txt` & `e2e_sae-0.0.3/e2e_sae.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 e2e_sae/__init__.py
 e2e_sae/data.py
 e2e_sae/hooks.py
 e2e_sae/loader.py
 e2e_sae/log.py
 e2e_sae/losses.py
 e2e_sae/metrics.py
+e2e_sae/plotting.py
 e2e_sae/settings.py
 e2e_sae/types.py
 e2e_sae/utils.py
 e2e_sae.egg-info/PKG-INFO
 e2e_sae.egg-info/SOURCES.txt
 e2e_sae.egg-info/dependency_links.txt
 e2e_sae.egg-info/requires.txt
 e2e_sae.egg-info/top_level.txt
 e2e_sae/models/__init__.py
 e2e_sae/models/mlp.py
 e2e_sae/models/sparsifiers.py
 e2e_sae/models/transformers.py
 e2e_sae/scripts/__init__.py
-e2e_sae/scripts/autointerp.py
 e2e_sae/scripts/upload_hf_dataset.py
 tests/test_mlp.py
 tests/test_sae.py
 tests/test_train_tlens_saes.py
 tests/test_transformer.py
 tests/test_utils.py
```

### Comparing `e2e_sae-0.0.2/pyproject.toml` & `e2e_sae-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "e2e_sae"
-version = "0.0.2"
+version = "0.0.3"
 description = "Repo for training sparse autoencoders end-to-end"
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = [
     "torch~=2.2.0",
     "torchvision~=0.17.0",
     "einops~=0.7.0",
@@ -16,25 +16,27 @@
     "ipykernel~=6.29.0",
     "transformer-lens~=1.14.0",
     "jaxtyping~=0.2.25",
     "python-dotenv~=1.0.1",
     "zstandard~=0.22.0",
     "matplotlib~=3.5.3",
     "seaborn~=0.13.2",
+    "umap-learn~=0.5.6",
     "tenacity~=8.2.3",
     "statsmodels~=0.14.2",
+    "automated-interpretability~=0.0.3"
 ]
 
 [project.urls]
 repository = "https://github.com/ApolloResearch/e2e_sae"
 
 [project.optional-dependencies]
 dev = [
     "ruff~=0.1.14",
-    "pyright~=1.1.360",
+    "pyright~=1.1.362",
     "pre-commit~=3.6.0",
 ]
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
@@ -69,17 +71,14 @@
 docstring-code-format = true
 
 [tool.ruff.isort]
 known-third-party = ["wandb"]
 
 [tool.pyright]
 include = ["e2e_sae", "tests"]
-exclude = [
-    "e2e_sae/scripts/autointerp.py",  # neuron_explainer package not yet on pypi
-]
 
 strictListInference = true
 strictDictionaryInference = true
 strictSetInference = true
 reportFunctionMemberAccess = true
 reportUnknownParameterType = true
 reportIncompatibleMethodOverride = true
```

### Comparing `e2e_sae-0.0.2/tests/test_mlp.py` & `e2e_sae-0.0.3/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.2/tests/test_sae.py` & `e2e_sae-0.0.3/tests/test_sae.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.2/tests/test_train_tlens_saes.py` & `e2e_sae-0.0.3/tests/test_train_tlens_saes.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.2/tests/test_transformer.py` & `e2e_sae-0.0.3/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `e2e_sae-0.0.2/tests/test_utils.py` & `e2e_sae-0.0.3/tests/test_utils.py`

 * *Files identical despite different names*

