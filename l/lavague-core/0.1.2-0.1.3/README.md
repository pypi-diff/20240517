# Comparing `tmp/lavague_core-0.1.2.tar.gz` & `tmp/lavague_core-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_core-0.1.2.tar", max compression
+gzip compressed data, was "lavague_core-0.1.3.tar", max compression
```

## Comparing `lavague_core-0.1.2.tar` & `lavague_core-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-05-16 06:03:22.535020 lavague_core-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2024-05-16 06:03:22.535047 lavague_core-0.1.2/README.md
--rw-r--r--   0        0        0      956 2024-05-16 06:03:22.535306 lavague_core-0.1.2/lavague/core/__init__.py
--rw-r--r--   0        0        0     4084 2024-05-16 06:03:22.535479 lavague_core-0.1.2/lavague/core/action_engine.py
--rw-r--r--   0        0        0     5873 2024-05-16 16:15:46.747778 lavague_core-0.1.2/lavague/core/agents.py
--rw-r--r--   0        0        0     2778 2024-05-16 06:03:22.535653 lavague_core-0.1.2/lavague/core/base_driver.py
--rw-r--r--   0        0        0     1896 2024-05-16 06:03:22.535742 lavague_core-0.1.2/lavague/core/context.py
--rw-r--r--   0        0        0     1296 2024-05-16 06:03:22.535814 lavague_core-0.1.2/lavague/core/extractors.py
--rw-r--r--   0        0        0      613 2024-05-16 06:03:22.535883 lavague_core-0.1.2/lavague/core/prompt_templates.py
--rw-r--r--   0        0        0    12117 2024-05-16 06:03:22.536134 lavague_core-0.1.2/lavague/core/retrievers.py
--rw-r--r--   0        0        0     3793 2024-05-16 06:03:22.536249 lavague_core-0.1.2/lavague/core/utilities/format_utils.py
--rw-r--r--   0        0        0     3584 2024-05-16 13:44:40.529386 lavague_core-0.1.2/lavague/core/utilities/telemetry.py
--rw-r--r--   0        0        0     1361 2024-05-16 06:03:22.536457 lavague_core-0.1.2/lavague/core/utilities/version_checker.py
--rw-r--r--   0        0        0      491 2024-05-16 06:03:22.536523 lavague_core-0.1.2/lavague/core/utilities/web_utils.py
--rw-r--r--   0        0        0     3445 2024-05-16 06:03:22.536696 lavague_core-0.1.2/lavague/core/world_model.py
--rw-r--r--   0        0        0     1080 2024-05-16 16:15:57.691336 lavague_core-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 lavague_core-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-16 06:03:22.535020 lavague_core-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-16 06:03:22.535047 lavague_core-0.1.3/README.md
+-rw-r--r--   0        0        0      956 2024-05-16 06:03:22.535306 lavague_core-0.1.3/lavague/core/__init__.py
+-rw-r--r--   0        0        0     4084 2024-05-16 06:03:22.535479 lavague_core-0.1.3/lavague/core/action_engine.py
+-rw-r--r--   0        0        0     5873 2024-05-17 07:27:00.823259 lavague_core-0.1.3/lavague/core/agents.py
+-rw-r--r--   0        0        0     2778 2024-05-16 06:03:22.535653 lavague_core-0.1.3/lavague/core/base_driver.py
+-rw-r--r--   0        0        0     1896 2024-05-16 06:03:22.535742 lavague_core-0.1.3/lavague/core/context.py
+-rw-r--r--   0        0        0     1296 2024-05-16 06:03:22.535814 lavague_core-0.1.3/lavague/core/extractors.py
+-rw-r--r--   0        0        0      613 2024-05-16 06:03:22.535883 lavague_core-0.1.3/lavague/core/prompt_templates.py
+-rw-r--r--   0        0        0    12117 2024-05-16 06:03:22.536134 lavague_core-0.1.3/lavague/core/retrievers.py
+-rw-r--r--   0        0        0     3793 2024-05-16 06:03:22.536249 lavague_core-0.1.3/lavague/core/utilities/format_utils.py
+-rw-r--r--   0        0        0     3563 2024-05-17 07:27:58.340843 lavague_core-0.1.3/lavague/core/utilities/telemetry.py
+-rw-r--r--   0        0        0     1361 2024-05-16 06:03:22.536457 lavague_core-0.1.3/lavague/core/utilities/version_checker.py
+-rw-r--r--   0        0        0      491 2024-05-16 06:03:22.536523 lavague_core-0.1.3/lavague/core/utilities/web_utils.py
+-rw-r--r--   0        0        0     3445 2024-05-16 06:03:22.536696 lavague_core-0.1.3/lavague/core/world_model.py
+-rw-r--r--   0        0        0     1080 2024-05-17 17:57:46.869711 lavague_core-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 lavague_core-0.1.3/PKG-INFO
```

### Comparing `lavague_core-0.1.2/LICENSE` & `lavague_core-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.2/lavague/core/__init__.py` & `lavague_core-0.1.3/lavague/core/__init__.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.2/lavague/core/action_engine.py` & `lavague_core-0.1.3/lavague/core/action_engine.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.2/lavague/core/agents.py` & `lavague_core-0.1.3/lavague/core/agents.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,15 +115,15 @@
                         screenshot_after_action = None
                         image = None
                         error = repr(e)
                         pass
                     finally:
                         action_id = str(uuid.uuid4())
                         send_telemetry(
-                            model_name=action_engine.llm.metadata.model_name, 
+                            model_name=action_engine.llm.metadata.model_name,
                             code=action,
                             instruction=instruction,
                             url=url,
                             origin="Agent",
                             success=success,
                             test=False,
                             error=error,
@@ -131,15 +131,15 @@
                             bounding_box=bounding_box,
                             viewport_size=viewport_size,
                             main_objective=objective,
                             objectives=output,
                             action_id=action_id,
                             multi_modal_model=world_model.mm_llm.metadata.model_name,
                             step_id=step_id,
-                            run_id=run_id
+                            run_id=run_id,
                         )
                         send_telemetry_scr(
                             action_id,
                             screenshot_before_action,
                             image,
                             screenshot_after_action,
                         )
```

### Comparing `lavague_core-0.1.2/lavague/core/base_driver.py` & `lavague_core-0.1.3/lavague/core/base_driver.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.2/lavague/core/context.py` & `lavague_core-0.1.3/lavague/core/context.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.2/lavague/core/extractors.py` & `lavague_core-0.1.3/lavague/core/extractors.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.2/lavague/core/prompt_templates.py` & `lavague_core-0.1.3/lavague/core/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.2/lavague/core/retrievers.py` & `lavague_core-0.1.3/lavague/core/retrievers.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.2/lavague/core/utilities/format_utils.py` & `lavague_core-0.1.3/lavague/core/utilities/format_utils.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.2/lavague/core/utilities/telemetry.py` & `lavague_core-0.1.3/lavague/core/utilities/telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     return buffer.getvalue()
 
 
 def send_telemetry_scr(
     action_id: str, before: Image, image: Image, after: Image, test: bool = False
 ):
     try:
-        if TELEMETRY_VAR is None:
+        if TELEMETRY_VAR == "HIGH":
             if before is not None:
                 before = compress_img(before)
             if image is not None:
                 image = compress_img(image)
             if after is not None:
                 after = compress_img(after)
             dict_img = {
@@ -39,15 +39,15 @@
             }
             pack = msgpack.packb(dict_img)
             r = requests.post(
                 "https://telemetrylavague.mithrilsecurity.io/telemetry_scrs", data=pack
             )
             if r.status_code != 200:
                 raise ValueError(r.content)
-        elif TELEMETRY_VAR == "NONE":
+        else:
             pass
     except Exception as e:
         if not test:
             print("Telemetry (screenshot) failed with ", e)
         else:
             raise ValueError("Telemetry failed with ", e)
 
@@ -107,8 +107,8 @@
                 raise ValueError(r.content)
         elif TELEMETRY_VAR == "NONE":
             pass
     except Exception as e:
         if not test:
             print("Telemetry failed with ", e)
         else:
-            raise ValueError("Telemetry failed with ", e)
+            raise ValueError("Telemetry failed with ", e)
```

### Comparing `lavague_core-0.1.2/lavague/core/utilities/version_checker.py` & `lavague_core-0.1.3/lavague/core/utilities/version_checker.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.2/lavague/core/world_model.py` & `lavague_core-0.1.3/lavague/core/world_model.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.2/pyproject.toml` & `lavague_core-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poetry]
 name = "lavague-core"
-version = "0.1.2"
+version = "0.1.3"
 description = "automation code generation from text instructions"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_core-0.1.2/PKG-INFO` & `lavague_core-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-core
-Version: 0.1.2
+Version: 0.1.3
 Summary: automation code generation from text instructions
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

