# Comparing `tmp/mlv-1.3.0.tar.gz` & `tmp/mlv-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlv-1.3.0.tar", last modified: Fri May 17 07:11:04 2024, max compression
+gzip compressed data, was "mlv-1.3.1.tar", last modified: Fri May 17 11:37:44 2024, max compression
```

## Comparing `mlv-1.3.0.tar` & `mlv-1.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 07:11:04.156573 mlv-1.3.0/
--rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-01-19 07:04:28.000000 mlv-1.3.0/MANIFEST.in
--rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 07:11:04.156317 mlv-1.3.0/PKG-INFO
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 07:11:04.154609 mlv-1.3.0/mlv/
--rw-r--r--   0 xiaotan    (501) staff       (20)       40 2024-05-17 07:04:00.000000 mlv-1.3.0/mlv/__init__.py
--rw-r--r--   0 xiaotan    (501) staff       (20)      172 2024-01-24 03:53:24.000000 mlv-1.3.0/mlv/base_model.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     8893 2024-05-17 07:10:17.000000 mlv-1.3.0/mlv/drawing.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     6255 2024-03-11 02:34:04.000000 mlv-1.3.0/mlv/http.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     7392 2024-05-17 06:57:36.000000 mlv-1.3.0/mlv/mps_workaround.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     4485 2024-01-24 08:00:40.000000 mlv-1.3.0/mlv/old_http.py
--rw-r--r--   0 xiaotan    (501) staff       (20)    16126 2024-04-03 16:19:29.000000 mlv-1.3.0/mlv/old_stable_diffusion.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3553 2024-01-21 09:16:52.000000 mlv-1.3.0/mlv/ollama.py
--rw-r--r--   0 xiaotan    (501) staff       (20)      926 2024-01-28 05:59:55.000000 mlv-1.3.0/mlv/rpc.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3050 2024-01-20 05:15:14.000000 mlv-1.3.0/mlv/segment_anything.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3166 2024-01-22 18:45:49.000000 mlv-1.3.0/mlv/stable_diffusion.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     5304 2024-05-17 07:03:15.000000 mlv-1.3.0/mlv/util.py
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 07:11:04.156032 mlv-1.3.0/mlv.egg-info/
--rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 07:11:04.000000 mlv-1.3.0/mlv.egg-info/PKG-INFO
--rw-r--r--   0 xiaotan    (501) staff       (20)      401 2024-05-17 07:11:04.000000 mlv-1.3.0/mlv.egg-info/SOURCES.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)        1 2024-05-17 07:11:04.000000 mlv-1.3.0/mlv.egg-info/dependency_links.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)      128 2024-05-17 07:11:04.000000 mlv-1.3.0/mlv.egg-info/requires.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)        4 2024-05-17 07:11:04.000000 mlv-1.3.0/mlv.egg-info/top_level.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)       51 2024-01-19 06:35:51.000000 mlv-1.3.0/pyproject.toml
--rw-r--r--   0 xiaotan    (501) staff       (20)       38 2024-05-17 07:11:04.156623 mlv-1.3.0/setup.cfg
--rw-r--r--   0 xiaotan    (501) staff       (20)      400 2024-05-17 07:02:42.000000 mlv-1.3.0/setup.py
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 07:11:04.155669 mlv-1.3.0/tests/
--rw-r--r--   0 xiaotan    (501) staff       (20)       36 2024-01-19 05:12:11.000000 mlv-1.3.0/tests/test_hello.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:37:44.771746 mlv-1.3.1/
+-rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-01-19 07:04:28.000000 mlv-1.3.1/MANIFEST.in
+-rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 11:37:44.771449 mlv-1.3.1/PKG-INFO
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:37:44.769357 mlv-1.3.1/mlv/
+-rw-r--r--   0 xiaotan    (501) staff       (20)       40 2024-05-17 07:04:00.000000 mlv-1.3.1/mlv/__init__.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)      172 2024-01-24 03:53:24.000000 mlv-1.3.1/mlv/base_model.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     8985 2024-05-17 11:37:24.000000 mlv-1.3.1/mlv/drawing.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     6255 2024-03-11 02:34:04.000000 mlv-1.3.1/mlv/http.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     7392 2024-05-17 06:57:36.000000 mlv-1.3.1/mlv/mps_workaround.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     4485 2024-01-24 08:00:40.000000 mlv-1.3.1/mlv/old_http.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)    16126 2024-04-03 16:19:29.000000 mlv-1.3.1/mlv/old_stable_diffusion.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3553 2024-01-21 09:16:52.000000 mlv-1.3.1/mlv/ollama.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)      926 2024-01-28 05:59:55.000000 mlv-1.3.1/mlv/rpc.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3050 2024-01-20 05:15:14.000000 mlv-1.3.1/mlv/segment_anything.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3166 2024-01-22 18:45:49.000000 mlv-1.3.1/mlv/stable_diffusion.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     5304 2024-05-17 07:03:15.000000 mlv-1.3.1/mlv/util.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:37:44.771119 mlv-1.3.1/mlv.egg-info/
+-rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 11:37:44.000000 mlv-1.3.1/mlv.egg-info/PKG-INFO
+-rw-r--r--   0 xiaotan    (501) staff       (20)      401 2024-05-17 11:37:44.000000 mlv-1.3.1/mlv.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)        1 2024-05-17 11:37:44.000000 mlv-1.3.1/mlv.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)      128 2024-05-17 11:37:44.000000 mlv-1.3.1/mlv.egg-info/requires.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)        4 2024-05-17 11:37:44.000000 mlv-1.3.1/mlv.egg-info/top_level.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)       51 2024-01-19 06:35:51.000000 mlv-1.3.1/pyproject.toml
+-rw-r--r--   0 xiaotan    (501) staff       (20)       38 2024-05-17 11:37:44.771803 mlv-1.3.1/setup.cfg
+-rw-r--r--   0 xiaotan    (501) staff       (20)      400 2024-05-17 11:37:31.000000 mlv-1.3.1/setup.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:37:44.770698 mlv-1.3.1/tests/
+-rw-r--r--   0 xiaotan    (501) staff       (20)       36 2024-01-19 05:12:11.000000 mlv-1.3.1/tests/test_hello.py
```

### Comparing `mlv-1.3.0/mlv/drawing.py` & `mlv-1.3.1/mlv/drawing.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 from io import BytesIO
 import time
 import platform
 import torch
 import os
 import random
 from PIL import Image, ImageOps
-import mps_workaround
+from mps_workaround import has_mps
 
 is_mac = platform == "darwin"
 cache_path = os.getenv("APP_MODEL_PATH", "")
 output_path = os.getenv("APP_OUTPUT_PATH", "")
 model_path = os.getenv("APP_MODEL_PATH", "")
 
+# This is for load mps_workaround file to packaging
+print("has mps", has_mps)
+
 
 def dataurl_to_image(data_url):
     _, encoded = data_url.split("base64,")
     data = b64decode(encoded)
     o = BytesIO(data)
     m = Image.open(o)
     return m
```

### Comparing `mlv-1.3.0/mlv/http.py` & `mlv-1.3.1/mlv/http.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.0/mlv/mps_workaround.py` & `mlv-1.3.1/mlv/mps_workaround.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.0/mlv/old_http.py` & `mlv-1.3.1/mlv/old_http.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.0/mlv/old_stable_diffusion.py` & `mlv-1.3.1/mlv/old_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.0/mlv/ollama.py` & `mlv-1.3.1/mlv/ollama.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.0/mlv/rpc.py` & `mlv-1.3.1/mlv/rpc.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.0/mlv/segment_anything.py` & `mlv-1.3.1/mlv/segment_anything.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.0/mlv/stable_diffusion.py` & `mlv-1.3.1/mlv/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.0/mlv/util.py` & `mlv-1.3.1/mlv/util.py`

 * *Files identical despite different names*

