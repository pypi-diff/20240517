# Comparing `tmp/mlv-1.3.2.tar.gz` & `tmp/mlv-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlv-1.3.2.tar", last modified: Fri May 17 11:39:50 2024, max compression
+gzip compressed data, was "mlv-1.3.3.tar", last modified: Fri May 17 11:44:18 2024, max compression
```

## Comparing `mlv-1.3.2.tar` & `mlv-1.3.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:39:50.640634 mlv-1.3.2/
--rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-01-19 07:04:28.000000 mlv-1.3.2/MANIFEST.in
--rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 11:39:50.640365 mlv-1.3.2/PKG-INFO
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:39:50.638563 mlv-1.3.2/mlv/
--rw-r--r--   0 xiaotan    (501) staff       (20)       40 2024-05-17 07:04:00.000000 mlv-1.3.2/mlv/__init__.py
--rw-r--r--   0 xiaotan    (501) staff       (20)      172 2024-01-24 03:53:24.000000 mlv-1.3.2/mlv/base_model.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     8986 2024-05-17 11:39:15.000000 mlv-1.3.2/mlv/drawing.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     6255 2024-03-11 02:34:04.000000 mlv-1.3.2/mlv/http.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     7392 2024-05-17 06:57:36.000000 mlv-1.3.2/mlv/mps_workaround.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     4485 2024-01-24 08:00:40.000000 mlv-1.3.2/mlv/old_http.py
--rw-r--r--   0 xiaotan    (501) staff       (20)    16126 2024-04-03 16:19:29.000000 mlv-1.3.2/mlv/old_stable_diffusion.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3553 2024-01-21 09:16:52.000000 mlv-1.3.2/mlv/ollama.py
--rw-r--r--   0 xiaotan    (501) staff       (20)      926 2024-01-28 05:59:55.000000 mlv-1.3.2/mlv/rpc.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3050 2024-01-20 05:15:14.000000 mlv-1.3.2/mlv/segment_anything.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3166 2024-01-22 18:45:49.000000 mlv-1.3.2/mlv/stable_diffusion.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     5304 2024-05-17 07:03:15.000000 mlv-1.3.2/mlv/util.py
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:39:50.640098 mlv-1.3.2/mlv.egg-info/
--rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 11:39:50.000000 mlv-1.3.2/mlv.egg-info/PKG-INFO
--rw-r--r--   0 xiaotan    (501) staff       (20)      401 2024-05-17 11:39:50.000000 mlv-1.3.2/mlv.egg-info/SOURCES.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)        1 2024-05-17 11:39:50.000000 mlv-1.3.2/mlv.egg-info/dependency_links.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)      128 2024-05-17 11:39:50.000000 mlv-1.3.2/mlv.egg-info/requires.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)        4 2024-05-17 11:39:50.000000 mlv-1.3.2/mlv.egg-info/top_level.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)       51 2024-01-19 06:35:51.000000 mlv-1.3.2/pyproject.toml
--rw-r--r--   0 xiaotan    (501) staff       (20)       38 2024-05-17 11:39:50.640682 mlv-1.3.2/setup.cfg
--rw-r--r--   0 xiaotan    (501) staff       (20)      400 2024-05-17 11:39:33.000000 mlv-1.3.2/setup.py
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:39:50.639753 mlv-1.3.2/tests/
--rw-r--r--   0 xiaotan    (501) staff       (20)       36 2024-01-19 05:12:11.000000 mlv-1.3.2/tests/test_hello.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:44:18.406103 mlv-1.3.3/
+-rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-01-19 07:04:28.000000 mlv-1.3.3/MANIFEST.in
+-rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 11:44:18.405851 mlv-1.3.3/PKG-INFO
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:44:18.404313 mlv-1.3.3/mlv/
+-rw-r--r--   0 xiaotan    (501) staff       (20)       40 2024-05-17 07:04:00.000000 mlv-1.3.3/mlv/__init__.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)      172 2024-01-24 03:53:24.000000 mlv-1.3.3/mlv/base_model.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     9049 2024-05-17 11:43:41.000000 mlv-1.3.3/mlv/drawing.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     6255 2024-03-11 02:34:04.000000 mlv-1.3.3/mlv/http.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     7392 2024-05-17 06:57:36.000000 mlv-1.3.3/mlv/mps_workaround.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     4485 2024-01-24 08:00:40.000000 mlv-1.3.3/mlv/old_http.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)    16126 2024-04-03 16:19:29.000000 mlv-1.3.3/mlv/old_stable_diffusion.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3553 2024-01-21 09:16:52.000000 mlv-1.3.3/mlv/ollama.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)      926 2024-01-28 05:59:55.000000 mlv-1.3.3/mlv/rpc.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3050 2024-01-20 05:15:14.000000 mlv-1.3.3/mlv/segment_anything.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3166 2024-01-22 18:45:49.000000 mlv-1.3.3/mlv/stable_diffusion.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     5304 2024-05-17 07:03:15.000000 mlv-1.3.3/mlv/util.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:44:18.405584 mlv-1.3.3/mlv.egg-info/
+-rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 11:44:18.000000 mlv-1.3.3/mlv.egg-info/PKG-INFO
+-rw-r--r--   0 xiaotan    (501) staff       (20)      401 2024-05-17 11:44:18.000000 mlv-1.3.3/mlv.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)        1 2024-05-17 11:44:18.000000 mlv-1.3.3/mlv.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)      128 2024-05-17 11:44:18.000000 mlv-1.3.3/mlv.egg-info/requires.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)        4 2024-05-17 11:44:18.000000 mlv-1.3.3/mlv.egg-info/top_level.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)       51 2024-01-19 06:35:51.000000 mlv-1.3.3/pyproject.toml
+-rw-r--r--   0 xiaotan    (501) staff       (20)       38 2024-05-17 11:44:18.406152 mlv-1.3.3/setup.cfg
+-rw-r--r--   0 xiaotan    (501) staff       (20)      400 2024-05-17 11:44:06.000000 mlv-1.3.3/setup.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:44:18.405363 mlv-1.3.3/tests/
+-rw-r--r--   0 xiaotan    (501) staff       (20)       36 2024-01-19 05:12:11.000000 mlv-1.3.3/tests/test_hello.py
```

### Comparing `mlv-1.3.2/mlv/drawing.py` & `mlv-1.3.3/mlv/drawing.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,29 +151,33 @@
 def load_model(model, safety_checker, lora_weights=[]):
     from diffusers import (
         StableDiffusionImg2ImgPipeline,
         StableDiffusionPipeline,
         LCMScheduler,
     )
     from diffusers.loaders.single_file_utils import (
-        create_text_encoder_from_ldm_clip_checkpoint,
-        load_single_file_model_checkpoint,
+        create_diffusers_clip_model_from_ldm,
+        load_single_file_checkpoint,
     )
     from diffusers.utils import load_image
-    from transformers import CLIPTextConfig, CLIPTokenizer
+    from transformers import CLIPTextConfig, CLIPTokenizer, CLIPTextModel
 
     # if not check_safetensors_exist(model_id):
     #     raise ValueError("safetensors file not exist")
 
     config_name = os.path.join(cache_path, "clip")
-    checkpoint = load_single_file_model_checkpoint(
+    checkpoint = load_single_file_checkpoint(
         os.path.join(cache_path, model), local_files_only=True
     )
-    text_encoder = create_text_encoder_from_ldm_clip_checkpoint(
-        config_name, checkpoint, local_files_only=True, torch_dtype=torch.float16
+    text_encoder = create_diffusers_clip_model_from_ldm(
+        CLIPTextModel,
+        checkpoint,
+        config=os.path.join(cache_path, "clip"),
+        local_files_only=True,
+        torch_dtype=torch.float16,
     )
     tokenizer = CLIPTokenizer.from_pretrained(config_name, local_files_only=True)
     txt2img_pipe = StableDiffusionPipeline.from_single_file(
         os.path.join(cache_path, model),
         cache_dir=cache_path,
         torch_dtype=torch.float16,
         text_encoder=text_encoder,
```

### Comparing `mlv-1.3.2/mlv/http.py` & `mlv-1.3.3/mlv/http.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.2/mlv/mps_workaround.py` & `mlv-1.3.3/mlv/mps_workaround.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.2/mlv/old_http.py` & `mlv-1.3.3/mlv/old_http.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.2/mlv/old_stable_diffusion.py` & `mlv-1.3.3/mlv/old_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.2/mlv/ollama.py` & `mlv-1.3.3/mlv/ollama.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.2/mlv/rpc.py` & `mlv-1.3.3/mlv/rpc.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.2/mlv/segment_anything.py` & `mlv-1.3.3/mlv/segment_anything.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.2/mlv/stable_diffusion.py` & `mlv-1.3.3/mlv/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.2/mlv/util.py` & `mlv-1.3.3/mlv/util.py`

 * *Files identical despite different names*

