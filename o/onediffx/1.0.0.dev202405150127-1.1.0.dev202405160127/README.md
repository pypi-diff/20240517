# Comparing `tmp/onediffx-1.0.0.dev202405150127.tar.gz` & `tmp/onediffx-1.1.0.dev202405160127.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediffx-1.0.0.dev202405150127.tar", last modified: Wed May 15 01:28:14 2024, max compression
+gzip compressed data, was "onediffx-1.1.0.dev202405160127.tar", last modified: Thu May 16 01:28:08 2024, max compression
```

## Comparing `onediffx-1.0.0.dev202405150127.tar` & `onediffx-1.1.0.dev202405160127.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:28:14.236531 onediffx-1.0.0.dev202405150127/
--rw-r--r--   0 runner    (1001) docker     (127)    22296 2024-05-15 01:28:14.236531 onediffx-1.0.0.dev202405150127/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21242 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:28:14.228531 onediffx-1.0.0.dev202405150127/onediffx/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:28:14.232531 onediffx-1.0.0.dev202405150127/onediffx/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/compilers/diffusion_pipeline_compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:28:14.232531 onediffx-1.0.0.dev202405150127/onediffx/deep_cache/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/deep_cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:28:14.232531 onediffx-1.0.0.dev202405150127/onediffx/deep_cache/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/deep_cache/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24987 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/deep_cache/models/fast_unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/deep_cache/models/pipeline_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25684 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/deep_cache/models/unet_2d_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/deep_cache/models/unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/deep_cache/models/unet_3d_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/deep_cache/models/unet_spatio_temporal_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    79951 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/deep_cache/pipeline_stable_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    91202 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/deep_cache/pipeline_stable_diffusion_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/deep_cache/pipeline_stable_video_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:28:14.236531 onediffx-1.0.0.dev202405150127/onediffx/lora/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/lora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/lora/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/lora/state_dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/lora/text_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11130 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/lora/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    13887 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/lora/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:28:14.236531 onediffx-1.0.0.dev202405150127/onediffx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/onediffx/utils/patch_image_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:28:14.236531 onediffx-1.0.0.dev202405150127/onediffx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22296 2024-05-15 01:28:14.000000 onediffx-1.0.0.dev202405150127/onediffx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-15 01:28:14.000000 onediffx-1.0.0.dev202405150127/onediffx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 01:28:14.000000 onediffx-1.0.0.dev202405150127/onediffx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 01:28:14.000000 onediffx-1.0.0.dev202405150127/onediffx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 01:28:14.000000 onediffx-1.0.0.dev202405150127/onediffx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 01:28:14.236531 onediffx-1.0.0.dev202405150127/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:28:14.236531 onediffx-1.0.0.dev202405150127/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-05-15 01:27:53.000000 onediffx-1.0.0.dev202405150127/tests/test_lora.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:28:08.004719 onediffx-1.1.0.dev202405160127/
+-rw-r--r--   0 runner    (1001) docker     (127)    22332 2024-05-16 01:28:08.004719 onediffx-1.1.0.dev202405160127/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21275 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:28:07.996719 onediffx-1.1.0.dev202405160127/onediffx/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:28:08.000719 onediffx-1.1.0.dev202405160127/onediffx/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/compilers/diffusion_pipeline_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:28:08.000719 onediffx-1.1.0.dev202405160127/onediffx/deep_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/deep_cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:28:08.000719 onediffx-1.1.0.dev202405160127/onediffx/deep_cache/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/deep_cache/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24987 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/deep_cache/models/fast_unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/deep_cache/models/pipeline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25684 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/deep_cache/models/unet_2d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/deep_cache/models/unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/deep_cache/models/unet_3d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/deep_cache/models/unet_spatio_temporal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79951 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/deep_cache/pipeline_stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91202 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/deep_cache/pipeline_stable_diffusion_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/deep_cache/pipeline_stable_video_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:28:08.004719 onediffx-1.1.0.dev202405160127/onediffx/lora/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/lora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/lora/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/lora/state_dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/lora/text_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/lora/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13887 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/lora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:28:08.004719 onediffx-1.1.0.dev202405160127/onediffx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/onediffx/utils/patch_image_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:28:08.004719 onediffx-1.1.0.dev202405160127/onediffx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22332 2024-05-16 01:28:07.000000 onediffx-1.1.0.dev202405160127/onediffx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-16 01:28:07.000000 onediffx-1.1.0.dev202405160127/onediffx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:28:07.000000 onediffx-1.1.0.dev202405160127/onediffx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 01:28:07.000000 onediffx-1.1.0.dev202405160127/onediffx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 01:28:07.000000 onediffx-1.1.0.dev202405160127/onediffx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:28:08.004719 onediffx-1.1.0.dev202405160127/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:28:08.004719 onediffx-1.1.0.dev202405160127/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-05-16 01:27:46.000000 onediffx-1.1.0.dev202405160127/tests/test_lora.py
```

### Comparing `onediffx-1.0.0.dev202405150127/PKG-INFO` & `onediffx-1.1.0.dev202405160127/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: onediffx
-Version: 1.0.0.dev202405150127
+Version: 1.1.0.dev202405160127
 Summary: onediff extensions for diffusers
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
-Author-email: caishenghang@oneflow.org
-License: Apache
+Author-email: contact@siliconflow.com
+License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -221,27 +221,27 @@
 
 ### Run Stable Video Diffusion with OneDiffX
 
 ```python
 import torch
 
 from diffusers.utils import load_image, export_to_video
-from onediffx import compile_pipe, compiler_config
+from onediffx import compile_pipe, compile_options
 from onediffx.deep_cache import StableVideoDiffusionPipeline
 
 pipe = StableVideoDiffusionPipeline.from_pretrained(
     "stabilityai/stable-video-diffusion-img2vid-xt",
     torch_dtype=torch.float16,
     variant="fp16",
     use_safetensors=True
 )
 pipe.to("cuda")
 
-compiler_config.attention_allow_half_precision_score_accumulation_max_m = 0
-pipe = compile_pipe(pipe)
+compile_options.oneflow.attention_allow_half_precision_score_accumulation_max_m = 0
+pipe = compile_pipe(pipe, options=compile_options)
 
 input_image = load_image("https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/diffusers/svd/rocket.png?download=true")
 input_image = input_image.resize((1024, 576))
 
 # Warmup
 for i in range(1):
     deepcache_output = pipe(
```

### Comparing `onediffx-1.0.0.dev202405150127/README.md` & `onediffx-1.1.0.dev202405160127/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -193,27 +193,27 @@
 
 ### Run Stable Video Diffusion with OneDiffX
 
 ```python
 import torch
 
 from diffusers.utils import load_image, export_to_video
-from onediffx import compile_pipe, compiler_config
+from onediffx import compile_pipe, compile_options
 from onediffx.deep_cache import StableVideoDiffusionPipeline
 
 pipe = StableVideoDiffusionPipeline.from_pretrained(
     "stabilityai/stable-video-diffusion-img2vid-xt",
     torch_dtype=torch.float16,
     variant="fp16",
     use_safetensors=True
 )
 pipe.to("cuda")
 
-compiler_config.attention_allow_half_precision_score_accumulation_max_m = 0
-pipe = compile_pipe(pipe)
+compile_options.oneflow.attention_allow_half_precision_score_accumulation_max_m = 0
+pipe = compile_pipe(pipe, options=compile_options)
 
 input_image = load_image("https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/diffusers/svd/rocket.png?download=true")
 input_image = input_image.resize((1024, 576))
 
 # Warmup
 for i in range(1):
     deepcache_output = pipe(
```

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/compilers/diffusion_pipeline_compiler.py` & `onediffx-1.1.0.dev202405160127/onediffx/compilers/diffusion_pipeline_compiler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import torch
-from onediff.infer_compiler import oneflow_compile
-from onediff.infer_compiler.deployable_module import DeployableModule
+from onediff.infer_compiler import compile, DeployableModule
 from onediff.infer_compiler.utils.log_utils import logger
 
 
 def _recursive_getattr(obj, attr, default=None):
     attrs = attr.split(".")
     for attr in attrs:
         if not hasattr(obj, attr):
@@ -30,14 +29,15 @@
     "fast_unet",  # for deepcache
     "prior",  # for StableCascadePriorPipeline
     "decoder",  # for StableCascadeDecoderPipeline
     "vqgan.down_blocks",  # for StableCascadeDecoderPipeline
     "vqgan.up_blocks",  # for StableCascadeDecoderPipeline
     "vae.decoder",
     "vae.encoder",
+    "transformer",  # for Transformer-based DiffusionPipeline such as DiTPipeline and PixArtAlphaPipeline
 ]
 
 
 def _filter_parts(ignores=()):
     filtered_parts = []
     for part in _PARTS:
         skip = False
@@ -48,30 +48,32 @@
         if not skip:
             filtered_parts.append(part)
 
     return filtered_parts
 
 
 def compile_pipe(
-    pipe, *, ignores=(),
+    pipe, *, backend="oneflow", options=None, ignores=(),
 ):
     # To fix the bug of graph load of vae. Please refer to: https://github.com/siliconflow/onediff/issues/452
     if (
         hasattr(pipe, "upcast_vae")
         and pipe.vae.dtype == torch.float16
         and pipe.vae.config.force_upcast
     ):
         pipe.upcast_vae()
 
     filtered_parts = _filter_parts(ignores=ignores)
     for part in filtered_parts:
         obj = _recursive_getattr(pipe, part, None)
         if obj is not None:
             logger.info(f"Compiling {part}")
-            _recursive_setattr(pipe, part, oneflow_compile(obj))
+            _recursive_setattr(
+                pipe, part, compile(obj, backend=backend, options=options)
+            )
 
     if hasattr(pipe, "image_processor") and "image_processor" not in ignores:
         logger.info("Patching image_processor")
 
         from onediffx.utils.patch_image_processor import (
             patch_image_prcessor as patch_image_prcessor_,
         )
```

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/deep_cache/__init__.py` & `onediffx-1.1.0.dev202405160127/onediffx/deep_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/deep_cache/models/fast_unet_2d_condition.py` & `onediffx-1.1.0.dev202405160127/onediffx/deep_cache/models/fast_unet_2d_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py` & `onediffx-1.1.0.dev202405160127/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/deep_cache/models/pipeline_utils.py` & `onediffx-1.1.0.dev202405160127/onediffx/deep_cache/models/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/deep_cache/models/unet_2d_blocks.py` & `onediffx-1.1.0.dev202405160127/onediffx/deep_cache/models/unet_2d_blocks.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/deep_cache/models/unet_2d_condition.py` & `onediffx-1.1.0.dev202405160127/onediffx/deep_cache/models/unet_2d_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/deep_cache/models/unet_3d_blocks.py` & `onediffx-1.1.0.dev202405160127/onediffx/deep_cache/models/unet_3d_blocks.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/deep_cache/models/unet_spatio_temporal_condition.py` & `onediffx-1.1.0.dev202405160127/onediffx/deep_cache/models/unet_spatio_temporal_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/deep_cache/pipeline_stable_diffusion.py` & `onediffx-1.1.0.dev202405160127/onediffx/deep_cache/pipeline_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/deep_cache/pipeline_stable_diffusion_xl.py` & `onediffx-1.1.0.dev202405160127/onediffx/deep_cache/pipeline_stable_diffusion_xl.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/deep_cache/pipeline_stable_video_diffusion.py` & `onediffx-1.1.0.dev202405160127/onediffx/deep_cache/pipeline_stable_video_diffusion.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/lora/lora.py` & `onediffx-1.1.0.dev202405160127/onediffx/lora/lora.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/lora/state_dict_utils.py` & `onediffx-1.1.0.dev202405160127/onediffx/lora/state_dict_utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/lora/text_encoder.py` & `onediffx-1.1.0.dev202405160127/onediffx/lora/text_encoder.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/lora/unet.py` & `onediffx-1.1.0.dev202405160127/onediffx/lora/unet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from packaging import version
 from typing import Union, Dict
 from collections import defaultdict
 
 import torch
-from onediff.infer_compiler.deployable_module import DeployableModule
+from onediff.infer_compiler import DeployableModule
 from onediff.infer_compiler.utils.log_utils import logger
 from diffusers.models.lora import (
     LoRACompatibleConv,
     LoRACompatibleLinear,
 )
 from .utils import fuse_lora, get_adapter_names, is_peft_available
 from diffusers.utils import is_accelerate_available
```

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/lora/utils.py` & `onediffx-1.1.0.dev202405160127/onediffx/lora/utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/onediffx/utils/patch_image_processor.py` & `onediffx-1.1.0.dev202405160127/onediffx/utils/patch_image_processor.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/onediffx.egg-info/PKG-INFO` & `onediffx-1.1.0.dev202405160127/onediffx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: onediffx
-Version: 1.0.0.dev202405150127
+Version: 1.1.0.dev202405160127
 Summary: onediff extensions for diffusers
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
-Author-email: caishenghang@oneflow.org
-License: Apache
+Author-email: contact@siliconflow.com
+License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -221,27 +221,27 @@
 
 ### Run Stable Video Diffusion with OneDiffX
 
 ```python
 import torch
 
 from diffusers.utils import load_image, export_to_video
-from onediffx import compile_pipe, compiler_config
+from onediffx import compile_pipe, compile_options
 from onediffx.deep_cache import StableVideoDiffusionPipeline
 
 pipe = StableVideoDiffusionPipeline.from_pretrained(
     "stabilityai/stable-video-diffusion-img2vid-xt",
     torch_dtype=torch.float16,
     variant="fp16",
     use_safetensors=True
 )
 pipe.to("cuda")
 
-compiler_config.attention_allow_half_precision_score_accumulation_max_m = 0
-pipe = compile_pipe(pipe)
+compile_options.oneflow.attention_allow_half_precision_score_accumulation_max_m = 0
+pipe = compile_pipe(pipe, options=compile_options)
 
 input_image = load_image("https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/diffusers/svd/rocket.png?download=true")
 input_image = input_image.resize((1024, 576))
 
 # Warmup
 for i in range(1):
     deepcache_output = pipe(
```

### Comparing `onediffx-1.0.0.dev202405150127/onediffx.egg-info/SOURCES.txt` & `onediffx-1.1.0.dev202405160127/onediffx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202405150127/setup.py` & `onediffx-1.1.0.dev202405160127/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 setup(
     name="onediffx",
     version=get_version(),
     description="onediff extensions for diffusers",
     url="https://github.com/siliconflow/onediff",
     author="OneDiff contributors",
-    license="Apache",
-    author_email="caishenghang@oneflow.org",
+    license="Apache-2.0",
+    author_email="contact@siliconflow.com",
     packages=find_packages(),
     python_requires=">=3.7.0",
     install_requires=[
         "transformers>=4.27.1",
         "diffusers>=0.19.3,<=0.27.0",
         "accelerate",
         "torch",
```

### Comparing `onediffx-1.0.0.dev202405150127/tests/test_lora.py` & `onediffx-1.1.0.dev202405160127/tests/test_lora.py`

 * *Files identical despite different names*

