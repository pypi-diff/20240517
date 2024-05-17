# Comparing `tmp/litellm_types-0.0.7.tar.gz` & `tmp/litellm_types-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm_types-0.0.7.tar", last modified: Fri May 17 11:27:36 2024, max compression
+gzip compressed data, was "litellm_types-0.0.8.tar", last modified: Fri May 17 12:02:40 2024, max compression
```

## Comparing `litellm_types-0.0.7.tar` & `litellm_types-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-17 11:27:36.693974 litellm_types-0.0.7/
--rw-r--r--   0 salamanderxing   (501) staff       (20)    11357 2024-05-06 12:34:17.000000 litellm_types-0.0.7/LICENSE
--rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-17 11:27:36.693752 litellm_types-0.0.7/PKG-INFO
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-17 11:27:36.692631 litellm_types-0.0.7/litellm_types/
--rw-r--r--   0 salamanderxing   (501) staff       (20)        2 2024-05-05 16:42:41.000000 litellm_types-0.0.7/litellm_types/__init__.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)    11532 2024-05-17 11:24:30.000000 litellm_types-0.0.7/litellm_types/completion.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)      134 2024-05-05 16:26:12.000000 litellm_types-0.0.7/litellm_types/document.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)     3965 2024-05-17 11:27:06.000000 litellm_types-0.0.7/litellm_types/messages.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)      293 2024-05-05 16:23:45.000000 litellm_types-0.0.7/litellm_types/prompt.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)     1324 2024-05-13 11:50:02.000000 litellm_types-0.0.7/litellm_types/test.py
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-17 11:27:36.693552 litellm_types-0.0.7/litellm_types.egg-info/
--rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-17 11:27:36.000000 litellm_types-0.0.7/litellm_types.egg-info/PKG-INFO
--rw-r--r--   0 salamanderxing   (501) staff       (20)      352 2024-05-17 11:27:36.000000 litellm_types-0.0.7/litellm_types.egg-info/SOURCES.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-05-17 11:27:36.000000 litellm_types-0.0.7/litellm_types.egg-info/dependency_links.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       26 2024-05-17 11:27:36.000000 litellm_types-0.0.7/litellm_types.egg-info/requires.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       14 2024-05-17 11:27:36.000000 litellm_types-0.0.7/litellm_types.egg-info/top_level.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-05-17 11:27:36.694018 litellm_types-0.0.7/setup.cfg
--rw-r--r--   0 salamanderxing   (501) staff       (20)      263 2024-05-17 11:27:32.000000 litellm_types-0.0.7/setup.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-17 12:02:40.465127 litellm_types-0.0.8/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)    11357 2024-05-06 12:34:17.000000 litellm_types-0.0.8/LICENSE
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-17 12:02:40.464956 litellm_types-0.0.8/PKG-INFO
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-17 12:02:40.464085 litellm_types-0.0.8/litellm_types/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)        2 2024-05-05 16:42:41.000000 litellm_types-0.0.8/litellm_types/__init__.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)    11607 2024-05-17 12:02:12.000000 litellm_types-0.0.8/litellm_types/completion.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      134 2024-05-05 16:26:12.000000 litellm_types-0.0.8/litellm_types/document.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)     3965 2024-05-17 11:27:06.000000 litellm_types-0.0.8/litellm_types/messages.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      293 2024-05-05 16:23:45.000000 litellm_types-0.0.8/litellm_types/prompt.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)     1324 2024-05-13 11:50:02.000000 litellm_types-0.0.8/litellm_types/test.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-17 12:02:40.464759 litellm_types-0.0.8/litellm_types.egg-info/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-17 12:02:40.000000 litellm_types-0.0.8/litellm_types.egg-info/PKG-INFO
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      352 2024-05-17 12:02:40.000000 litellm_types-0.0.8/litellm_types.egg-info/SOURCES.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-05-17 12:02:40.000000 litellm_types-0.0.8/litellm_types.egg-info/dependency_links.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       26 2024-05-17 12:02:40.000000 litellm_types-0.0.8/litellm_types.egg-info/requires.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       14 2024-05-17 12:02:40.000000 litellm_types-0.0.8/litellm_types.egg-info/top_level.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-05-17 12:02:40.465164 litellm_types-0.0.8/setup.cfg
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      263 2024-05-17 12:02:38.000000 litellm_types-0.0.8/setup.py
```

### Comparing `litellm_types-0.0.7/LICENSE` & `litellm_types-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm_types-0.0.7/litellm_types/completion.py` & `litellm_types-0.0.8/litellm_types/completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,17 +147,18 @@
         model_list: list | None = None,  # pass in a list of api_base,keys, etc.
         # Optional liteLLM function params
         **kwargs,
     ):
         parsed_tools = replace_pydantic_objects_in_tools(tools)
 
         async def wrapper(messages: list[AnyMessage]) -> AssistantMessage:
+            messages_dicts = [m.model_dump_json() for m in messages]
             result = await acompletion(
                 model=model,
-                messages=messages,
+                messages=messages_dicts,
                 # timeout=timeout,
                 temperature=temperature,
                 top_p=top_p,
                 n=n,
                 stream=False,
                 stop=stop,
                 max_tokens=max_tokens,
```

### Comparing `litellm_types-0.0.7/litellm_types/messages.py` & `litellm_types-0.0.8/litellm_types/messages.py`

 * *Files identical despite different names*

### Comparing `litellm_types-0.0.7/litellm_types/test.py` & `litellm_types-0.0.8/litellm_types/test.py`

 * *Files identical despite different names*

