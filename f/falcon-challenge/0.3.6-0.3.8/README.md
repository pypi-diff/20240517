# Comparing `tmp/falcon_challenge-0.3.6.tar.gz` & `tmp/falcon_challenge-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_challenge-0.3.6.tar", last modified: Wed May 15 19:06:22 2024, max compression
+gzip compressed data, was "falcon_challenge-0.3.8.tar", last modified: Fri May 17 03:52:31 2024, max compression
```

## Comparing `falcon_challenge-0.3.6.tar` & `falcon_challenge-0.3.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:06:22.154477 falcon_challenge-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-15 19:06:22.154477 falcon_challenge-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:06:22.150477 falcon_challenge-0.3.6/decoder_demos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/decoder_demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/decoder_demos/decoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/decoder_demos/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/decoder_demos/ndt2_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/decoder_demos/random_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/decoder_demos/rnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13812 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/decoder_demos/sklearn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/decoder_demos/sklearn_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:06:22.154477 falcon_challenge-0.3.6/falcon_challenge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/falcon_challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/falcon_challenge/challenge_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/falcon_challenge/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/falcon_challenge/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    28367 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/falcon_challenge/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/falcon_challenge/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:06:22.154477 falcon_challenge-0.3.6/falcon_challenge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-15 19:06:22.000000 falcon_challenge-0.3.6/falcon_challenge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-15 19:06:22.000000 falcon_challenge-0.3.6/falcon_challenge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:06:22.000000 falcon_challenge-0.3.6/falcon_challenge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 19:06:22.000000 falcon_challenge-0.3.6/falcon_challenge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 19:06:22.000000 falcon_challenge-0.3.6/falcon_challenge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:06:22.154477 falcon_challenge-0.3.6/preproc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/assemble_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/h2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/m1_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    24166 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/m1_reachgrasp_preprocv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/m2_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/m2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/merge_answers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/nwb_create_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/wrapper_convert_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/zip_data.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:06:22.154477 falcon_challenge-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:52:31.678625 falcon_challenge-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-17 03:52:31.678625 falcon_challenge-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:52:31.674625 falcon_challenge-0.3.8/decoder_demos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/decoder_demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/decoder_demos/decoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/decoder_demos/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/decoder_demos/ndt2_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/decoder_demos/random_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/decoder_demos/rnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13812 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/decoder_demos/sklearn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/decoder_demos/sklearn_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:52:31.674625 falcon_challenge-0.3.8/falcon_challenge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/falcon_challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/falcon_challenge/challenge_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/falcon_challenge/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/falcon_challenge/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28438 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/falcon_challenge/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/falcon_challenge/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:52:31.678625 falcon_challenge-0.3.8/falcon_challenge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-17 03:52:31.000000 falcon_challenge-0.3.8/falcon_challenge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-17 03:52:31.000000 falcon_challenge-0.3.8/falcon_challenge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:52:31.000000 falcon_challenge-0.3.8/falcon_challenge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-17 03:52:31.000000 falcon_challenge-0.3.8/falcon_challenge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-17 03:52:31.000000 falcon_challenge-0.3.8/falcon_challenge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:52:31.678625 falcon_challenge-0.3.8/preproc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/assemble_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/h2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/m1_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24166 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/m1_reachgrasp_preprocv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/m2_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/m2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/merge_answers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/nwb_create_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/wrapper_convert_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/preproc/zip_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:52:31.678625 falcon_challenge-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-17 03:52:24.000000 falcon_challenge-0.3.8/setup.py
```

### Comparing `falcon_challenge-0.3.6/LICENSE` & `falcon_challenge-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/PKG-INFO` & `falcon_challenge-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.3.6
+Version: 0.3.8
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.3.6/README.md` & `falcon_challenge-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/decoder_demos/decoding_utils.py` & `falcon_challenge-0.3.8/decoder_demos/decoding_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/decoder_demos/filtering.py` & `falcon_challenge-0.3.8/decoder_demos/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/decoder_demos/ndt2_sample.py` & `falcon_challenge-0.3.8/decoder_demos/ndt2_sample.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,33 +34,36 @@
     parser.add_argument(
         '--phase', choices=['minival', 'test'], default='minival'
     )
     parser.add_argument(
         '--batch-size', type=int, default=1
     )
     parser.add_argument(
-        '--continual', action='store_true', default=False
+        '--continual', action='store_true', default=False # deprecated
     )
     
     args = parser.parse_args()
 
+
     evaluator = FalconEvaluator(
         eval_remote=args.evaluation == "remote",
         split=args.split,
-        continual=args.continual
+        # continual=args.continual
     )
 
     task = getattr(FalconTask, args.split)
     config = FalconConfig(task=task)
+    max_bins = 50 if task in [FalconTask.m1, FalconTask.m2] else 200 # h1
 
     decoder = NDT2Decoder(
         task_config=config,
         model_ckpt_path=args.model_path,
         model_cfg_stem=args.config_stem,
         zscore_path=args.zscore_path,
+        max_bins=max_bins,
         dataset_handles=[x.stem for x in evaluator.get_eval_files(phase=args.phase)],
         batch_size=args.batch_size
     )
 
 
     evaluator.evaluate(decoder, phase=args.phase)
```

### Comparing `falcon_challenge-0.3.6/decoder_demos/random_decoder.py` & `falcon_challenge-0.3.8/decoder_demos/random_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/decoder_demos/rnn_decoder.py` & `falcon_challenge-0.3.8/decoder_demos/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/decoder_demos/sklearn_decoder.py` & `falcon_challenge-0.3.8/decoder_demos/sklearn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/decoder_demos/sklearn_sample.py` & `falcon_challenge-0.3.8/decoder_demos/sklearn_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/falcon_challenge/config.py` & `falcon_challenge-0.3.8/falcon_challenge/config.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/falcon_challenge/dataloaders.py` & `falcon_challenge-0.3.8/falcon_challenge/dataloaders.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/falcon_challenge/evaluator.py` & `falcon_challenge-0.3.8/falcon_challenge/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,18 +292,21 @@
     trial_change = pad_sequence([torch.tensor(t) for t in trial_change], batch_first=False).numpy()
     eval_mask = pad_sequence([torch.tensor(t) for t in eval_mask], batch_first=False).numpy() # Serves as a mask for padding as well
     datafile_idx = np.array(datafile_idx)
     return data, targets, trial_change, eval_mask, datafile_idx
 
 class FalconEvaluator:
 
-    def __init__(self, eval_remote=False, split='h1', continual=False):
+    def __init__(self, eval_remote=False, split='h1'):
         self.eval_remote = eval_remote
         assert split in ['h1', 'h2', 'm1', 'm2'], "Split must be h1, h2, m1, or m2."
-        self.continual = continual
+        if split in ['h1', 'm1', 'm2']:
+            self.continual = True
+        else:
+            self.continual = False
         self.dataset: FalconTask = getattr(FalconTask, split)
         self.cfg = FalconConfig(self.dataset)
 
     @staticmethod
     def get_eval_handles(is_remote: bool, dataset: FalconTask, phase: str = 'minival'):
         if is_remote: # i.e. definitely docker
             data_dir = os.environ.get("EVAL_DATA_PATH")
```

### Comparing `falcon_challenge-0.3.6/falcon_challenge/interface.py` & `falcon_challenge-0.3.8/falcon_challenge/interface.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/falcon_challenge.egg-info/PKG-INFO` & `falcon_challenge-0.3.8/falcon_challenge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.3.6
+Version: 0.3.8
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.3.6/falcon_challenge.egg-info/SOURCES.txt` & `falcon_challenge-0.3.8/falcon_challenge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/preproc/assemble_data.py` & `falcon_challenge-0.3.8/preproc/assemble_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/preproc/filtering.py` & `falcon_challenge-0.3.8/preproc/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/preproc/h2_preproc.py` & `falcon_challenge-0.3.8/preproc/h2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/preproc/m1_fewshot_trial_counts.py` & `falcon_challenge-0.3.8/preproc/m1_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/preproc/m1_reachgrasp_preprocv2.py` & `falcon_challenge-0.3.8/preproc/m1_reachgrasp_preprocv2.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/preproc/m2_fewshot_trial_counts.py` & `falcon_challenge-0.3.8/preproc/m2_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/preproc/m2_preproc.py` & `falcon_challenge-0.3.8/preproc/m2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/preproc/merge_answers.py` & `falcon_challenge-0.3.8/preproc/merge_answers.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/preproc/nwb_create_utils.py` & `falcon_challenge-0.3.8/preproc/nwb_create_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/preproc/wrapper_convert_batch.py` & `falcon_challenge-0.3.8/preproc/wrapper_convert_batch.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/preproc/zip_data.py` & `falcon_challenge-0.3.8/preproc/zip_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.6/setup.py` & `falcon_challenge-0.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='falcon_challenge',
-    version='0.3.6',
+    version='0.3.8',
 
     url='https://github.com/snel-repo/stability-benchmark',
     author='Joel Ye',
     author_email='joelye9@gmail.com',
 
     packages=find_packages(exclude=['data_demos', 'data']),
     install_requires=[
```

