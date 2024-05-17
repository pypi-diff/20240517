# Comparing `tmp/mlv-1.3.4.tar.gz` & `tmp/mlv-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlv-1.3.4.tar", last modified: Fri May 17 11:45:58 2024, max compression
+gzip compressed data, was "mlv-1.3.5.tar", last modified: Fri May 17 11:50:08 2024, max compression
```

## Comparing `mlv-1.3.4.tar` & `mlv-1.3.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:45:58.267791 mlv-1.3.4/
--rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-01-19 07:04:28.000000 mlv-1.3.4/MANIFEST.in
--rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 11:45:58.267545 mlv-1.3.4/PKG-INFO
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:45:58.266059 mlv-1.3.4/mlv/
--rw-r--r--   0 xiaotan    (501) staff       (20)       40 2024-05-17 07:04:00.000000 mlv-1.3.4/mlv/__init__.py
--rw-r--r--   0 xiaotan    (501) staff       (20)      172 2024-01-24 03:53:24.000000 mlv-1.3.4/mlv/base_model.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     9005 2024-05-17 11:45:31.000000 mlv-1.3.4/mlv/drawing.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     6255 2024-03-11 02:34:04.000000 mlv-1.3.4/mlv/http.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     7392 2024-05-17 06:57:36.000000 mlv-1.3.4/mlv/mps_workaround.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     4485 2024-01-24 08:00:40.000000 mlv-1.3.4/mlv/old_http.py
--rw-r--r--   0 xiaotan    (501) staff       (20)    16126 2024-04-03 16:19:29.000000 mlv-1.3.4/mlv/old_stable_diffusion.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3553 2024-01-21 09:16:52.000000 mlv-1.3.4/mlv/ollama.py
--rw-r--r--   0 xiaotan    (501) staff       (20)      926 2024-01-28 05:59:55.000000 mlv-1.3.4/mlv/rpc.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3050 2024-01-20 05:15:14.000000 mlv-1.3.4/mlv/segment_anything.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3166 2024-01-22 18:45:49.000000 mlv-1.3.4/mlv/stable_diffusion.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     5304 2024-05-17 07:03:15.000000 mlv-1.3.4/mlv/util.py
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:45:58.267263 mlv-1.3.4/mlv.egg-info/
--rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 11:45:58.000000 mlv-1.3.4/mlv.egg-info/PKG-INFO
--rw-r--r--   0 xiaotan    (501) staff       (20)      401 2024-05-17 11:45:58.000000 mlv-1.3.4/mlv.egg-info/SOURCES.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)        1 2024-05-17 11:45:58.000000 mlv-1.3.4/mlv.egg-info/dependency_links.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)      128 2024-05-17 11:45:58.000000 mlv-1.3.4/mlv.egg-info/requires.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)        4 2024-05-17 11:45:58.000000 mlv-1.3.4/mlv.egg-info/top_level.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)       51 2024-01-19 06:35:51.000000 mlv-1.3.4/pyproject.toml
--rw-r--r--   0 xiaotan    (501) staff       (20)       38 2024-05-17 11:45:58.267837 mlv-1.3.4/setup.cfg
--rw-r--r--   0 xiaotan    (501) staff       (20)      400 2024-05-17 11:45:50.000000 mlv-1.3.4/setup.py
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:45:58.267066 mlv-1.3.4/tests/
--rw-r--r--   0 xiaotan    (501) staff       (20)       36 2024-01-19 05:12:11.000000 mlv-1.3.4/tests/test_hello.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:50:08.361299 mlv-1.3.5/
+-rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-01-19 07:04:28.000000 mlv-1.3.5/MANIFEST.in
+-rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 11:50:08.361028 mlv-1.3.5/PKG-INFO
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:50:08.359327 mlv-1.3.5/mlv/
+-rw-r--r--   0 xiaotan    (501) staff       (20)       40 2024-05-17 07:04:00.000000 mlv-1.3.5/mlv/__init__.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)      172 2024-01-24 03:53:24.000000 mlv-1.3.5/mlv/base_model.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     9376 2024-05-17 11:49:36.000000 mlv-1.3.5/mlv/drawing.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     6255 2024-03-11 02:34:04.000000 mlv-1.3.5/mlv/http.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     7392 2024-05-17 06:57:36.000000 mlv-1.3.5/mlv/mps_workaround.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     4485 2024-01-24 08:00:40.000000 mlv-1.3.5/mlv/old_http.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)    16126 2024-04-03 16:19:29.000000 mlv-1.3.5/mlv/old_stable_diffusion.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3553 2024-01-21 09:16:52.000000 mlv-1.3.5/mlv/ollama.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)      926 2024-01-28 05:59:55.000000 mlv-1.3.5/mlv/rpc.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3050 2024-01-20 05:15:14.000000 mlv-1.3.5/mlv/segment_anything.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3166 2024-01-22 18:45:49.000000 mlv-1.3.5/mlv/stable_diffusion.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     5304 2024-05-17 07:03:15.000000 mlv-1.3.5/mlv/util.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:50:08.360753 mlv-1.3.5/mlv.egg-info/
+-rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 11:50:08.000000 mlv-1.3.5/mlv.egg-info/PKG-INFO
+-rw-r--r--   0 xiaotan    (501) staff       (20)      401 2024-05-17 11:50:08.000000 mlv-1.3.5/mlv.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)        1 2024-05-17 11:50:08.000000 mlv-1.3.5/mlv.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)      128 2024-05-17 11:50:08.000000 mlv-1.3.5/mlv.egg-info/requires.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)        4 2024-05-17 11:50:08.000000 mlv-1.3.5/mlv.egg-info/top_level.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)       51 2024-01-19 06:35:51.000000 mlv-1.3.5/pyproject.toml
+-rw-r--r--   0 xiaotan    (501) staff       (20)       38 2024-05-17 11:50:08.361363 mlv-1.3.5/setup.cfg
+-rw-r--r--   0 xiaotan    (501) staff       (20)      400 2024-05-17 11:50:00.000000 mlv-1.3.5/setup.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 11:50:08.360521 mlv-1.3.5/tests/
+-rw-r--r--   0 xiaotan    (501) staff       (20)       36 2024-01-19 05:12:11.000000 mlv-1.3.5/tests/test_hello.py
```

### Comparing `mlv-1.3.4/mlv/drawing.py` & `mlv-1.3.5/mlv/drawing.py`

 * *Files 3% similar despite different names*

```diff
@@ -245,20 +245,29 @@
     name = "drawing_ai"
     model = None
 
     def __init__(self) -> None:
         super().__init__()
 
     def load_model(self, args):
-        with timer("load sd model"):
-            self.model = load_model(
-                args.get("model"),
-                args.get("safety_checker", False),
-                args.get("lora", []),
-            )
+        mode = args.get("mode")
+        if mode == "draw_precision":
+            with timer("load sd model"):
+                self.model = load_model_adapter(
+                    args.get("model"),
+                    args.get("safety_checker", False),
+                    args.get("lora", []),
+                )
+        elif mode == "draw_fast":
+            with timer("load sd model"):
+                self.model = load_model(
+                    args.get("model"),
+                    args.get("safety_checker", False),
+                    args.get("lora", []),
+                )
 
     def run_model(self, args):
         mode = args.get("mode")
         if not mode:
             raise ValueError("model args missing")
         image = args.get("image")
         prompt = args.get("prompt")
```

### Comparing `mlv-1.3.4/mlv/http.py` & `mlv-1.3.5/mlv/http.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.4/mlv/mps_workaround.py` & `mlv-1.3.5/mlv/mps_workaround.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.4/mlv/old_http.py` & `mlv-1.3.5/mlv/old_http.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.4/mlv/old_stable_diffusion.py` & `mlv-1.3.5/mlv/old_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.4/mlv/ollama.py` & `mlv-1.3.5/mlv/ollama.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.4/mlv/rpc.py` & `mlv-1.3.5/mlv/rpc.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.4/mlv/segment_anything.py` & `mlv-1.3.5/mlv/segment_anything.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.4/mlv/stable_diffusion.py` & `mlv-1.3.5/mlv/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.4/mlv/util.py` & `mlv-1.3.5/mlv/util.py`

 * *Files identical despite different names*

