# Comparing `tmp/denoising_diffusion_pytorch-2.0.0.tar.gz` & `tmp/denoising_diffusion_pytorch-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising_diffusion_pytorch-2.0.0.tar", last modified: Fri May  3 16:35:25 2024, max compression
+gzip compressed data, was "denoising_diffusion_pytorch-2.0.1.tar", last modified: Fri May 17 13:08:54 2024, max compression
```

## Comparing `denoising_diffusion_pytorch-2.0.0.tar` & `denoising_diffusion_pytorch-2.0.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:35:25.127220 denoising_diffusion_pytorch-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-03 16:35:25.127220 denoising_diffusion_pytorch-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:35:25.123220 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (127)    27964 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    38426 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/fid_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    35678 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    18413 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/karras_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    18224 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/karras_unet_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)    23187 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/karras_unet_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    21071 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:35:25.127220 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-03 16:35:25.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-03 16:35:25.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:35:25.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 16:35:25.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 16:35:25.000000 denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:35:25.127220 denoising_diffusion_pytorch-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-03 16:35:21.000000 denoising_diffusion_pytorch-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:08:54.599446 denoising_diffusion_pytorch-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-17 13:08:54.599446 denoising_diffusion_pytorch-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:08:54.599446 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27964 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38426 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/fid_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35678 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18413 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/karras_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18224 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/karras_unet_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23187 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/karras_unet_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39839 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/repaint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21071 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:08:54.599446 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-17 13:08:54.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-17 13:08:54.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:08:54.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-17 13:08:54.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 13:08:54.000000 denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 13:08:54.599446 denoising_diffusion_pytorch-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-17 13:08:50.000000 denoising_diffusion_pytorch-2.0.1/setup.py
```

### Comparing `denoising_diffusion_pytorch-2.0.0/LICENSE` & `denoising_diffusion_pytorch-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/PKG-INFO` & `denoising_diffusion_pytorch-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 2.0.0
+Version: 2.0.1
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising_diffusion_pytorch-2.0.0/README.md` & `denoising_diffusion_pytorch-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/__init__.py` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/attend.py` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/attend.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             self.cuda_config = AttentionConfig(False, True, True)
 
     def flash_attn(self, q, k, v):
         _, heads, q_len, _, k_len, is_cuda, device = *q.shape, k.shape[-2], q.is_cuda, q.device
 
         if exists(self.scale):
             default_scale = q.shape[-1]
-            q = q * (scale / default_scale)
+            q = q * (self.scale / default_scale)
 
         q, k, v = map(lambda t: t.contiguous(), (q, k, v))
 
         # Check if there is a compatible device for flash attention
 
         config = self.cuda_config if is_cuda else self.cpu_config
```

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/fid_evaluation.py` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/fid_evaluation.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/karras_unet.py` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/karras_unet.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/karras_unet_1d.py` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/karras_unet_1d.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/karras_unet_3d.py` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/karras_unet_3d.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 2.0.0
+Version: 2.0.1
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising_diffusion_pytorch-2.0.0/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising_diffusion_pytorch-2.0.1/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 denoising_diffusion_pytorch/elucidated_diffusion.py
 denoising_diffusion_pytorch/fid_evaluation.py
 denoising_diffusion_pytorch/guided_diffusion.py
 denoising_diffusion_pytorch/karras_unet.py
 denoising_diffusion_pytorch/karras_unet_1d.py
 denoising_diffusion_pytorch/karras_unet_3d.py
 denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+denoising_diffusion_pytorch/repaint.py
 denoising_diffusion_pytorch/simple_diffusion.py
 denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
 denoising_diffusion_pytorch/version.py
 denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
 denoising_diffusion_pytorch.egg-info/PKG-INFO
 denoising_diffusion_pytorch.egg-info/SOURCES.txt
 denoising_diffusion_pytorch.egg-info/dependency_links.txt
```

### Comparing `denoising_diffusion_pytorch-2.0.0/setup.py` & `denoising_diffusion_pytorch-2.0.1/setup.py`

 * *Files identical despite different names*

