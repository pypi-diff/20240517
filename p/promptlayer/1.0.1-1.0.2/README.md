# Comparing `tmp/promptlayer-1.0.1.tar.gz` & `tmp/promptlayer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptlayer-1.0.1.tar", max compression
+gzip compressed data, was "promptlayer-1.0.2.tar", max compression
```

## Comparing `promptlayer-1.0.1.tar` & `promptlayer-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-05-14 15:09:50.781215 promptlayer-1.0.1/LICENSE
--rw-r--r--   0        0        0     3870 2024-05-14 15:09:50.781215 promptlayer-1.0.1/README.md
--rw-r--r--   0        0        0     1565 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/__init__.py
--rw-r--r--   0        0        0      224 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/groups/__init__.py
--rw-r--r--   0        0        0      165 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/groups/groups.py
--rw-r--r--   0        0        0     4035 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/promptlayer.py
--rw-r--r--   0        0        0      717 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/templates.py
--rw-r--r--   0        0        0      945 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/track/__init__.py
--rw-r--r--   0        0        0     1610 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/track/track.py
--rw-r--r--   0        0        0       61 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/types/__init__.py
--rw-r--r--   0        0        0     3813 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/types/prompt_template.py
--rw-r--r--   0        0        0    21130 2024-05-14 15:09:50.785215 promptlayer-1.0.1/promptlayer/utils.py
--rw-r--r--   0        0        0      571 2024-05-14 15:09:50.785215 promptlayer-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4628 1970-01-01 00:00:00.000000 promptlayer-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-16 22:40:18.073473 promptlayer-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3870 2024-05-16 22:40:18.073473 promptlayer-1.0.2/README.md
+-rw-r--r--   0        0        0     1602 2024-05-16 22:40:18.073473 promptlayer-1.0.2/promptlayer/__init__.py
+-rw-r--r--   0        0        0      224 2024-05-16 22:40:18.073473 promptlayer-1.0.2/promptlayer/groups/__init__.py
+-rw-r--r--   0        0        0      165 2024-05-16 22:40:18.073473 promptlayer-1.0.2/promptlayer/groups/groups.py
+-rw-r--r--   0        0        0     4035 2024-05-16 22:40:18.073473 promptlayer-1.0.2/promptlayer/promptlayer.py
+-rw-r--r--   0        0        0      717 2024-05-16 22:40:18.073473 promptlayer-1.0.2/promptlayer/templates.py
+-rw-r--r--   0        0        0      945 2024-05-16 22:40:18.073473 promptlayer-1.0.2/promptlayer/track/__init__.py
+-rw-r--r--   0        0        0     1610 2024-05-16 22:40:18.073473 promptlayer-1.0.2/promptlayer/track/track.py
+-rw-r--r--   0        0        0       61 2024-05-16 22:40:18.073473 promptlayer-1.0.2/promptlayer/types/__init__.py
+-rw-r--r--   0        0        0     3813 2024-05-16 22:40:18.073473 promptlayer-1.0.2/promptlayer/types/prompt_template.py
+-rw-r--r--   0        0        0    21130 2024-05-16 22:40:18.073473 promptlayer-1.0.2/promptlayer/utils.py
+-rw-r--r--   0        0        0      571 2024-05-16 22:40:18.073473 promptlayer-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4628 1970-01-01 00:00:00.000000 promptlayer-1.0.2/PKG-INFO
```

### Comparing `promptlayer-1.0.1/LICENSE` & `promptlayer-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.1/README.md` & `promptlayer-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.1/promptlayer/__init__.py` & `promptlayer-1.0.2/promptlayer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,8 +41,9 @@
                 api_key=self.api_key,
             )
             return anthropic
         else:
             raise AttributeError(f"module {__name__} has no attribute {name}")
 
 
-__all__ = ["PromptLayer"]
+__version__ = "1.0.2"
+__all__ = ["PromptLayer", "__version__"]
```

### Comparing `promptlayer-1.0.1/promptlayer/promptlayer.py` & `promptlayer-1.0.2/promptlayer/promptlayer.py`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.1/promptlayer/templates.py` & `promptlayer-1.0.2/promptlayer/templates.py`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.1/promptlayer/track/__init__.py` & `promptlayer-1.0.2/promptlayer/track/__init__.py`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.1/promptlayer/track/track.py` & `promptlayer-1.0.2/promptlayer/track/track.py`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.1/promptlayer/types/prompt_template.py` & `promptlayer-1.0.2/promptlayer/types/prompt_template.py`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.1/promptlayer/utils.py` & `promptlayer-1.0.2/promptlayer/utils.py`

 * *Files identical despite different names*

### Comparing `promptlayer-1.0.1/pyproject.toml` & `promptlayer-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promptlayer"
-version = "1.0.1"
+version = "1.0.2"
 description = "PromptLayer is a platform for prompt engineering and tracks your LLM requests."
 authors = ["Magniv <hello@magniv.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `promptlayer-1.0.1/PKG-INFO` & `promptlayer-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 1.0.1
+Version: 1.0.2
 Summary: PromptLayer is a platform for prompt engineering and tracks your LLM requests.
 License: Apache-2.0
 Author: Magniv
 Author-email: hello@magniv.io
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 1.0.1 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 1.0.2 Summary: PromptLayer is
 a platform for prompt engineering and tracks your LLM requests. License:
 Apache-2.0 Author: Magniv Author-email: hello@magniv.io Requires-Python:
 >=3.8.1,<4.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: anthropic (>=0.25.8,<0.26.0)
```

