# Comparing `tmp/mlv-1.3.3.tar.gz` & `tmp/mlv-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlv-1.3.3.tar", last modified: Fri May 17 11:44:18 2024, max compression
+gzip compressed data, was "mlv-1.3.4.tar", last modified: Fri May 17 11:45:58 2024, max compression
```

## Comparing `mlv-1.3.3.tar` & `mlv-1.3.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:44:18.406103 mlv-1.3.3/
--rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-01-19 07:04:28.000000 mlv-1.3.3/MANIFEST.in
--rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 11:44:18.405851 mlv-1.3.3/PKG-INFO
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:44:18.404313 mlv-1.3.3/mlv/
--rw-r--r--   0 xiaotan    (501) staff       (20)       40 2024-05-17 07:04:00.000000 mlv-1.3.3/mlv/__init__.py
--rw-r--r--   0 xiaotan    (501) staff       (20)      172 2024-01-24 03:53:24.000000 mlv-1.3.3/mlv/base_model.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     9049 2024-05-17 11:43:41.000000 mlv-1.3.3/mlv/drawing.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     6255 2024-03-11 02:34:04.000000 mlv-1.3.3/mlv/http.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     7392 2024-05-17 06:57:36.000000 mlv-1.3.3/mlv/mps_workaround.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     4485 2024-01-24 08:00:40.000000 mlv-1.3.3/mlv/old_http.py
--rw-r--r--   0 xiaotan    (501) staff       (20)    16126 2024-04-03 16:19:29.000000 mlv-1.3.3/mlv/old_stable_diffusion.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3553 2024-01-21 09:16:52.000000 mlv-1.3.3/mlv/ollama.py
--rw-r--r--   0 xiaotan    (501) staff       (20)      926 2024-01-28 05:59:55.000000 mlv-1.3.3/mlv/rpc.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3050 2024-01-20 05:15:14.000000 mlv-1.3.3/mlv/segment_anything.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3166 2024-01-22 18:45:49.000000 mlv-1.3.3/mlv/stable_diffusion.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     5304 2024-05-17 07:03:15.000000 mlv-1.3.3/mlv/util.py
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:44:18.405584 mlv-1.3.3/mlv.egg-info/
--rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 11:44:18.000000 mlv-1.3.3/mlv.egg-info/PKG-INFO
--rw-r--r--   0 xiaotan    (501) staff       (20)      401 2024-05-17 11:44:18.000000 mlv-1.3.3/mlv.egg-info/SOURCES.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)        1 2024-05-17 11:44:18.000000 mlv-1.3.3/mlv.egg-info/dependency_links.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)      128 2024-05-17 11:44:18.000000 mlv-1.3.3/mlv.egg-info/requires.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)        4 2024-05-17 11:44:18.000000 mlv-1.3.3/mlv.egg-info/top_level.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)       51 2024-01-19 06:35:51.000000 mlv-1.3.3/pyproject.toml
--rw-r--r--   0 xiaotan    (501) staff       (20)       38 2024-05-17 11:44:18.406152 mlv-1.3.3/setup.cfg
--rw-r--r--   0 xiaotan    (501) staff       (20)      400 2024-05-17 11:44:06.000000 mlv-1.3.3/setup.py
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:44:18.405363 mlv-1.3.3/tests/
--rw-r--r--   0 xiaotan    (501) staff       (20)       36 2024-01-19 05:12:11.000000 mlv-1.3.3/tests/test_hello.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:45:58.267791 mlv-1.3.4/
+-rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-01-19 07:04:28.000000 mlv-1.3.4/MANIFEST.in
+-rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 11:45:58.267545 mlv-1.3.4/PKG-INFO
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:45:58.266059 mlv-1.3.4/mlv/
+-rw-r--r--   0 xiaotan    (501) staff       (20)       40 2024-05-17 07:04:00.000000 mlv-1.3.4/mlv/__init__.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)      172 2024-01-24 03:53:24.000000 mlv-1.3.4/mlv/base_model.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     9005 2024-05-17 11:45:31.000000 mlv-1.3.4/mlv/drawing.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     6255 2024-03-11 02:34:04.000000 mlv-1.3.4/mlv/http.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     7392 2024-05-17 06:57:36.000000 mlv-1.3.4/mlv/mps_workaround.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     4485 2024-01-24 08:00:40.000000 mlv-1.3.4/mlv/old_http.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)    16126 2024-04-03 16:19:29.000000 mlv-1.3.4/mlv/old_stable_diffusion.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3553 2024-01-21 09:16:52.000000 mlv-1.3.4/mlv/ollama.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)      926 2024-01-28 05:59:55.000000 mlv-1.3.4/mlv/rpc.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3050 2024-01-20 05:15:14.000000 mlv-1.3.4/mlv/segment_anything.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3166 2024-01-22 18:45:49.000000 mlv-1.3.4/mlv/stable_diffusion.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     5304 2024-05-17 07:03:15.000000 mlv-1.3.4/mlv/util.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:45:58.267263 mlv-1.3.4/mlv.egg-info/
+-rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 11:45:58.000000 mlv-1.3.4/mlv.egg-info/PKG-INFO
+-rw-r--r--   0 xiaotan    (501) staff       (20)      401 2024-05-17 11:45:58.000000 mlv-1.3.4/mlv.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)        1 2024-05-17 11:45:58.000000 mlv-1.3.4/mlv.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)      128 2024-05-17 11:45:58.000000 mlv-1.3.4/mlv.egg-info/requires.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)        4 2024-05-17 11:45:58.000000 mlv-1.3.4/mlv.egg-info/top_level.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)       51 2024-01-19 06:35:51.000000 mlv-1.3.4/pyproject.toml
+-rw-r--r--   0 xiaotan    (501) staff       (20)       38 2024-05-17 11:45:58.267837 mlv-1.3.4/setup.cfg
+-rw-r--r--   0 xiaotan    (501) staff       (20)      400 2024-05-17 11:45:50.000000 mlv-1.3.4/setup.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:45:58.267066 mlv-1.3.4/tests/
+-rw-r--r--   0 xiaotan    (501) staff       (20)       36 2024-01-19 05:12:11.000000 mlv-1.3.4/tests/test_hello.py
```

### Comparing `mlv-1.3.3/mlv/drawing.py` & `mlv-1.3.4/mlv/drawing.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,14 @@
     txt2img_pipe = StableDiffusionPipeline.from_single_file(
         os.path.join(cache_path, model),
         cache_dir=cache_path,
         torch_dtype=torch.float16,
         text_encoder=text_encoder,
         tokenizer=tokenizer,
         variant="fp16",
-        load_safety_checker=safety_checker,
         local_files_only=True,
         use_safetensors=True,
         original_config_file=os.path.join(cache_path, "v1-inference.yaml"),
     )
 
     device = get_device()
     txt2img_pipe.to(device=device)
```

### Comparing `mlv-1.3.3/mlv/http.py` & `mlv-1.3.4/mlv/http.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.3/mlv/mps_workaround.py` & `mlv-1.3.4/mlv/mps_workaround.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.3/mlv/old_http.py` & `mlv-1.3.4/mlv/old_http.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.3/mlv/old_stable_diffusion.py` & `mlv-1.3.4/mlv/old_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.3/mlv/ollama.py` & `mlv-1.3.4/mlv/ollama.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.3/mlv/rpc.py` & `mlv-1.3.4/mlv/rpc.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.3/mlv/segment_anything.py` & `mlv-1.3.4/mlv/segment_anything.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.3/mlv/stable_diffusion.py` & `mlv-1.3.4/mlv/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.3/mlv/util.py` & `mlv-1.3.4/mlv/util.py`

 * *Files identical despite different names*

