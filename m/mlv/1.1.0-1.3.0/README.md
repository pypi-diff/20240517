# Comparing `tmp/mlv-1.1.0.tar.gz` & `tmp/mlv-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlv-1.1.0.tar", last modified: Sun Jan 28 06:18:10 2024, max compression
+gzip compressed data, was "mlv-1.3.0.tar", last modified: Fri May 17 07:11:04 2024, max compression
```

## Comparing `mlv-1.1.0.tar` & `mlv-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-01-28 06:18:10.735422 mlv-1.1.0/
--rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-01-19 07:04:28.000000 mlv-1.1.0/MANIFEST.in
--rw-r--r--   0 xiaotan    (501) staff       (20)      169 2024-01-28 06:18:10.735215 mlv-1.1.0/PKG-INFO
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-01-28 06:18:10.733345 mlv-1.1.0/mlv/
--rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-01-19 00:35:11.000000 mlv-1.1.0/mlv/__init__.py
--rw-r--r--   0 xiaotan    (501) staff       (20)      172 2024-01-24 03:53:24.000000 mlv-1.1.0/mlv/base_model.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     1513 2024-01-27 04:03:50.000000 mlv-1.1.0/mlv/downloader.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     5731 2024-01-28 06:04:18.000000 mlv-1.1.0/mlv/http.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     7352 2024-01-19 05:12:11.000000 mlv-1.1.0/mlv/mps_workaround.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     4485 2024-01-24 08:00:40.000000 mlv-1.1.0/mlv/old_http.py
--rw-r--r--   0 xiaotan    (501) staff       (20)    15962 2024-01-22 02:15:32.000000 mlv-1.1.0/mlv/old_stable_diffusion.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3553 2024-01-21 09:16:52.000000 mlv-1.1.0/mlv/ollama.py
--rw-r--r--   0 xiaotan    (501) staff       (20)      926 2024-01-28 05:59:55.000000 mlv-1.1.0/mlv/rpc.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3050 2024-01-20 05:15:14.000000 mlv-1.1.0/mlv/segment_anything.py
--rw-r--r--   0 xiaotan    (501) staff       (20)      587 2024-01-27 03:36:06.000000 mlv-1.1.0/mlv/setting.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3166 2024-01-22 18:45:49.000000 mlv-1.1.0/mlv/stable_diffusion.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     2425 2024-01-27 10:17:41.000000 mlv-1.1.0/mlv/util.py
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-01-28 06:18:10.734970 mlv-1.1.0/mlv.egg-info/
--rw-r--r--   0 xiaotan    (501) staff       (20)      169 2024-01-28 06:18:10.000000 mlv-1.1.0/mlv.egg-info/PKG-INFO
--rw-r--r--   0 xiaotan    (501) staff       (20)      419 2024-01-28 06:18:10.000000 mlv-1.1.0/mlv.egg-info/SOURCES.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)        1 2024-01-28 06:18:10.000000 mlv-1.1.0/mlv.egg-info/dependency_links.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)       53 2024-01-28 06:18:10.000000 mlv-1.1.0/mlv.egg-info/requires.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)        1 2024-01-28 06:18:10.000000 mlv-1.1.0/mlv.egg-info/top_level.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)       51 2024-01-19 06:35:51.000000 mlv-1.1.0/pyproject.toml
--rw-r--r--   0 xiaotan    (501) staff       (20)       38 2024-01-28 06:18:10.735489 mlv-1.1.0/setup.cfg
--rw-r--r--   0 xiaotan    (501) staff       (20)      241 2024-01-28 06:17:51.000000 mlv-1.1.0/setup.py
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-01-28 06:18:10.734666 mlv-1.1.0/tests/
--rw-r--r--   0 xiaotan    (501) staff       (20)       36 2024-01-19 05:12:11.000000 mlv-1.1.0/tests/test_hello.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 07:11:04.156573 mlv-1.3.0/
+-rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-01-19 07:04:28.000000 mlv-1.3.0/MANIFEST.in
+-rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 07:11:04.156317 mlv-1.3.0/PKG-INFO
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 07:11:04.154609 mlv-1.3.0/mlv/
+-rw-r--r--   0 xiaotan    (501) staff       (20)       40 2024-05-17 07:04:00.000000 mlv-1.3.0/mlv/__init__.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)      172 2024-01-24 03:53:24.000000 mlv-1.3.0/mlv/base_model.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     8893 2024-05-17 07:10:17.000000 mlv-1.3.0/mlv/drawing.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     6255 2024-03-11 02:34:04.000000 mlv-1.3.0/mlv/http.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     7392 2024-05-17 06:57:36.000000 mlv-1.3.0/mlv/mps_workaround.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     4485 2024-01-24 08:00:40.000000 mlv-1.3.0/mlv/old_http.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)    16126 2024-04-03 16:19:29.000000 mlv-1.3.0/mlv/old_stable_diffusion.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3553 2024-01-21 09:16:52.000000 mlv-1.3.0/mlv/ollama.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)      926 2024-01-28 05:59:55.000000 mlv-1.3.0/mlv/rpc.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3050 2024-01-20 05:15:14.000000 mlv-1.3.0/mlv/segment_anything.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3166 2024-01-22 18:45:49.000000 mlv-1.3.0/mlv/stable_diffusion.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     5304 2024-05-17 07:03:15.000000 mlv-1.3.0/mlv/util.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 07:11:04.156032 mlv-1.3.0/mlv.egg-info/
+-rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 07:11:04.000000 mlv-1.3.0/mlv.egg-info/PKG-INFO
+-rw-r--r--   0 xiaotan    (501) staff       (20)      401 2024-05-17 07:11:04.000000 mlv-1.3.0/mlv.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)        1 2024-05-17 07:11:04.000000 mlv-1.3.0/mlv.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)      128 2024-05-17 07:11:04.000000 mlv-1.3.0/mlv.egg-info/requires.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)        4 2024-05-17 07:11:04.000000 mlv-1.3.0/mlv.egg-info/top_level.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)       51 2024-01-19 06:35:51.000000 mlv-1.3.0/pyproject.toml
+-rw-r--r--   0 xiaotan    (501) staff       (20)       38 2024-05-17 07:11:04.156623 mlv-1.3.0/setup.cfg
+-rw-r--r--   0 xiaotan    (501) staff       (20)      400 2024-05-17 07:02:42.000000 mlv-1.3.0/setup.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 07:11:04.155669 mlv-1.3.0/tests/
+-rw-r--r--   0 xiaotan    (501) staff       (20)       36 2024-01-19 05:12:11.000000 mlv-1.3.0/tests/test_hello.py
```

### Comparing `mlv-1.1.0/mlv/http.py` & `mlv-1.3.0/mlv/http.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,41 @@
+from .util import (
+    check_model_files_exist,
+    load_aiapps_json,
+    find_free_port,
+    cache_path,
+    aiapps_path,
+    output_path,
+    DownloadManager,
+    rpc_code,
+)
+
+
+### SPLIT
+
+
 import time
-import json
 import xmlrpc.client
 import subprocess
 import atexit
 import os
 from flask import Flask, request, abort
 from os import path
 import threading
-from mlv.old_http import find_free_port
-from .setting import cache_path, aiapps_path, output_path
-from .util import check_model_files_exist, load_aiapps_json
-from .downloader import DownloadManager
+from flask_cors import CORS
 
 
 lock = threading.Lock()
 
 if not path.exists(cache_path):
     os.makedirs(cache_path, exist_ok=True)
 
 infer = {"pipe": None}
 app = Flask(__name__)
+CORS(app)
 context = {"app": {}}
 aiapps = load_aiapps_json()
 print("Load aiapps", [app["name"] for app in aiapps])
 
 
 def get_frameworks_port():
     result = {}
@@ -47,24 +59,28 @@
         self.process = process
         self.proxy = xmlrpc.client.ServerProxy(
             "http://localhost:" + port, allow_none=True
         )
 
         # wait for the app process finish setup
         max_retries = 5
+        success = False
         while max_retries:
             time.sleep(1)
             try:
                 self.proxy.test_connection()
+                print("App is connected, ", app_name)
+                success = True
                 break
             except Exception:
                 print("test connection fail, retry")
             finally:
                 max_retries -= 1
-        print("App is connected, ", app_name)
+        if not success:
+            raise Exception("App can not connect, " + app_name)
 
 
 @app.route("/download_file", methods=["POST"])
 def download_file():
     data = request.get_json()
     dl = DownloadManager(os.path.join(cache_path, data.get("app_name")))
     if data.get("from_huggingface"):
@@ -129,33 +145,46 @@
         if not app["info"].get("framework"):
             abort(500, "App config error, no framework found")
         need_framework = app["info"]["framework"]
         if not all(running_frameworks.get(f) for f in need_framework):
             abort(500, "Needed framework not start")
 
     model_process = subprocess.Popen(
-        f"venv/bin/python3 -c 'from main import Model;from mlv.rpc import start_server;start_server(Model, {app_port}, {running_frameworks_json})'",
+        f"venv/bin/python3 -c '{rpc_code}\nfrom main import Model;start_server(Model, {app_port}, {running_frameworks_json})'",
         cwd=app_source_path,
         shell=True,
         # set env OLLAMA_MODELS=models path
         env={
             "APP_SOURCE_PATH": app_source_path,
             "APP_MODEL_PATH": app_model_path,
             "APP_OUTPUT_PATH": app_output_path,
-            "OLLAMA_MODELS": os.path.join(cache_path, "ollama"),
             **os.environ,
         },
     )
-    context["app"][app["name"]] = AppRunner(
-        app["name"],
-        model_process,
-        str(app_port),
-        app["info"].get("is_framework", None),
+
+    try:
+        context["app"][app["name"]] = AppRunner(
+            app["name"],
+            model_process,
+            str(app_port),
+            app["info"].get("is_framework", None),
+        )
+        return {"success": True}
+    except Exception:
+        return {"success": False}
+
+
+@app.route("/test_connection", methods={"POST"})
+def tecn():
+    data = request.get_json()
+    client = xmlrpc.client.ServerProxy(
+        "http://localhost:" + data.get("port"), allow_none=True
     )
-    return {"success": True}
+    result = client.test_connection()
+    return {"result": result}
 
 
 @app.route("/stop_app", methods=["POST"])
 def stop_app():
     data = request.get_json()
     with lock:
         global context
@@ -171,14 +200,19 @@
 def is_app_running():
     data = request.get_json()
     if data and data.get("model"):
         return "yes" if context["app"][data["model"]] else "no"
     abort(404)
 
 
+@app.route("/hello", methods=["GET"])
+def hello():
+    return "success"
+
+
 def run_app():
     port = os.getenv("PORT") or find_free_port()
     print(f"###PORT:{port}")
     app.run(host="localhost", port=port)
 
 
 def onexit():
```

### Comparing `mlv-1.1.0/mlv/mps_workaround.py` & `mlv-1.3.0/mlv/mps_workaround.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,17 +87,19 @@
 
 
 if has_mps:
     if platform.mac_ver()[0].startswith("13.2."):
         # MPS workaround for https://github.com/pytorch/pytorch/issues/95188, thanks to danieldk (https://github.com/explosion/curated-transformers/pull/124)
         CondFunc(
             "torch.nn.functional.linear",
-            lambda _, input, weight, bias: (torch.matmul(input, weight.t()) + bias)
-            if bias is not None
-            else torch.matmul(input, weight.t()),
+            lambda _, input, weight, bias: (
+                (torch.matmul(input, weight.t()) + bias)
+                if bias is not None
+                else torch.matmul(input, weight.t())
+            ),
             lambda _, input, weight, bias: input.numel() > 10485760,
         )
 
     if version.parse(torch.__version__) < version.parse("1.13"):
         # PyTorch 1.13 doesn't need these fixes but unfortunately is slower and has regressions that prevent training from working
 
         # MPS workaround for https://github.com/pytorch/pytorch/issues/79383
```

### Comparing `mlv-1.1.0/mlv/old_http.py` & `mlv-1.3.0/mlv/old_http.py`

 * *Files identical despite different names*

### Comparing `mlv-1.1.0/mlv/old_stable_diffusion.py` & `mlv-1.3.0/mlv/old_stable_diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 is_mac = platform == "darwin"
 
 
 def get_device():
     return (
         "cuda"
         if torch.cuda.is_available()
-        else "mps"
-        if torch.backends.mps.is_available()
-        else "cpu"
+        else "mps" if torch.backends.mps.is_available() else "cpu"
     )
 
 
 def resize(img: Image.Image):
     maxs = max(img.size[0], img.size[1])
     if maxs < 900:
         return img
@@ -430,14 +428,19 @@
             txt2img_pipe.load_lora_weights(
                 os.path.join(cache_path, "lora", lora_weights[i] + ".safetensors")
             )
             txt2img_pipe.fuse_lora()
     generator = torch.Generator()
 
     img2img_pipe = StableDiffusionImg2ImgPipeline(**txt2img_pipe.components)
+    img2img_pipe.disable_lora()
+    img2img_pipe.load_lora_weights(
+        os.path.join(cache_path, "lora", "pytorch_lora_weights.safetensors")
+    )
+    img2img_pipe.fuse_lora()
 
     def infer(
         prompt,
         image,
         num_inference_steps=5,
         guidance_scale=2,
         strength=0.9,
```

### Comparing `mlv-1.1.0/mlv/ollama.py` & `mlv-1.3.0/mlv/ollama.py`

 * *Files identical despite different names*

### Comparing `mlv-1.1.0/mlv/rpc.py` & `mlv-1.3.0/mlv/rpc.py`

 * *Files identical despite different names*

### Comparing `mlv-1.1.0/mlv/segment_anything.py` & `mlv-1.3.0/mlv/segment_anything.py`

 * *Files identical despite different names*

### Comparing `mlv-1.1.0/mlv/stable_diffusion.py` & `mlv-1.3.0/mlv/stable_diffusion.py`

 * *Files identical despite different names*

