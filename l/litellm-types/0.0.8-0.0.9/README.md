# Comparing `tmp/litellm_types-0.0.8.tar.gz` & `tmp/litellm_types-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm_types-0.0.8.tar", last modified: Fri May 17 12:02:40 2024, max compression
+gzip compressed data, was "litellm_types-0.0.9.tar", last modified: Fri May 17 14:16:03 2024, max compression
```

## Comparing `litellm_types-0.0.8.tar` & `litellm_types-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-17 12:02:40.465127 litellm_types-0.0.8/
--rw-r--r--   0 salamanderxing   (501) staff       (20)    11357 2024-05-06 12:34:17.000000 litellm_types-0.0.8/LICENSE
--rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-17 12:02:40.464956 litellm_types-0.0.8/PKG-INFO
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-17 12:02:40.464085 litellm_types-0.0.8/litellm_types/
--rw-r--r--   0 salamanderxing   (501) staff       (20)        2 2024-05-05 16:42:41.000000 litellm_types-0.0.8/litellm_types/__init__.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)    11607 2024-05-17 12:02:12.000000 litellm_types-0.0.8/litellm_types/completion.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)      134 2024-05-05 16:26:12.000000 litellm_types-0.0.8/litellm_types/document.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)     3965 2024-05-17 11:27:06.000000 litellm_types-0.0.8/litellm_types/messages.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)      293 2024-05-05 16:23:45.000000 litellm_types-0.0.8/litellm_types/prompt.py
--rw-r--r--   0 salamanderxing   (501) staff       (20)     1324 2024-05-13 11:50:02.000000 litellm_types-0.0.8/litellm_types/test.py
-drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-17 12:02:40.464759 litellm_types-0.0.8/litellm_types.egg-info/
--rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-17 12:02:40.000000 litellm_types-0.0.8/litellm_types.egg-info/PKG-INFO
--rw-r--r--   0 salamanderxing   (501) staff       (20)      352 2024-05-17 12:02:40.000000 litellm_types-0.0.8/litellm_types.egg-info/SOURCES.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-05-17 12:02:40.000000 litellm_types-0.0.8/litellm_types.egg-info/dependency_links.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       26 2024-05-17 12:02:40.000000 litellm_types-0.0.8/litellm_types.egg-info/requires.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       14 2024-05-17 12:02:40.000000 litellm_types-0.0.8/litellm_types.egg-info/top_level.txt
--rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-05-17 12:02:40.465164 litellm_types-0.0.8/setup.cfg
--rw-r--r--   0 salamanderxing   (501) staff       (20)      263 2024-05-17 12:02:38.000000 litellm_types-0.0.8/setup.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-17 14:16:03.596449 litellm_types-0.0.9/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)    11357 2024-05-06 12:34:17.000000 litellm_types-0.0.9/LICENSE
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-17 14:16:03.596266 litellm_types-0.0.9/PKG-INFO
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-17 14:16:03.595260 litellm_types-0.0.9/litellm_types/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)        2 2024-05-05 16:42:41.000000 litellm_types-0.0.9/litellm_types/__init__.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)    11632 2024-05-17 12:11:51.000000 litellm_types-0.0.9/litellm_types/completion.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      134 2024-05-05 16:26:12.000000 litellm_types-0.0.9/litellm_types/document.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)     4009 2024-05-17 14:15:22.000000 litellm_types-0.0.9/litellm_types/messages.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      293 2024-05-05 16:23:45.000000 litellm_types-0.0.9/litellm_types/prompt.py
+-rw-r--r--   0 salamanderxing   (501) staff       (20)     1324 2024-05-13 11:50:02.000000 litellm_types-0.0.9/litellm_types/test.py
+drwxr-xr-x   0 salamanderxing   (501) staff       (20)        0 2024-05-17 14:16:03.596083 litellm_types-0.0.9/litellm_types.egg-info/
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      150 2024-05-17 14:16:03.000000 litellm_types-0.0.9/litellm_types.egg-info/PKG-INFO
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      352 2024-05-17 14:16:03.000000 litellm_types-0.0.9/litellm_types.egg-info/SOURCES.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)        1 2024-05-17 14:16:03.000000 litellm_types-0.0.9/litellm_types.egg-info/dependency_links.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       26 2024-05-17 14:16:03.000000 litellm_types-0.0.9/litellm_types.egg-info/requires.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       14 2024-05-17 14:16:03.000000 litellm_types-0.0.9/litellm_types.egg-info/top_level.txt
+-rw-r--r--   0 salamanderxing   (501) staff       (20)       38 2024-05-17 14:16:03.596490 litellm_types-0.0.9/setup.cfg
+-rw-r--r--   0 salamanderxing   (501) staff       (20)      263 2024-05-17 14:15:58.000000 litellm_types-0.0.9/setup.py
```

### Comparing `litellm_types-0.0.8/LICENSE` & `litellm_types-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm_types-0.0.8/litellm_types/completion.py` & `litellm_types-0.0.9/litellm_types/completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,16 @@
         model_list: list | None = None,  # pass in a list of api_base,keys, etc.
         # Optional liteLLM function params
         **kwargs,
     ):
         parsed_tools = replace_pydantic_objects_in_tools(tools)
 
         async def wrapper(messages: list[AnyMessage]) -> AssistantMessage:
-            messages_dicts = [m.model_dump_json() for m in messages]
+            messages_dicts = [m.__dict__ for m in messages]
+            print(messages_dicts)
             result = await acompletion(
                 model=model,
                 messages=messages_dicts,
                 # timeout=timeout,
                 temperature=temperature,
                 top_p=top_p,
                 n=n,
```

### Comparing `litellm_types-0.0.8/litellm_types/messages.py` & `litellm_types-0.0.9/litellm_types/messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,42 +25,42 @@
 
 
 class FunctionMessage(BaseModel):
     content: str
     name: str
     role: Literal["function"] = "function"
 
-    def __init__(self, content: str, name: str):
-        super().__init__(content=content, name=name, role="function")
+    def __init__(self, content: str, name: str, role="function"):
+        super().__init__(content=content, name=name, role=role)
 
 
 class UserMessage(BaseModel):
     content: str
     role: Literal["user"] = "user"
 
-    def __init__(self, content: str):
-        super().__init__(content=content, role="user")
+    def __init__(self, content: str, role="user"):
+        super().__init__(content=content, role=role)
 
 
 class SystemMessage(BaseModel):
     content: str
     role: Literal["system"] = "system"
 
-    def __init__(self, content: str):
-        super().__init__(content=content, role="system")
+    def __init__(self, content: str, role="system"):
+        super().__init__(content=content, role=role)
 
 
 class ToolCall(BaseModel):
     id: str
     function: Function
     type: str
 
     @beartype
-    def __init__(self, id: str, function: Function):
-        super().__init__(id=id, function=function, type="function")
+    def __init__(self, id: str, function: Function, type="function"):
+        super().__init__(id=id, function=function, type=type)
 
 
 class ToolCallDelta(BaseModel):
     id: str | None = None
     function: Function
     type: str | None = None
```

### Comparing `litellm_types-0.0.8/litellm_types/test.py` & `litellm_types-0.0.9/litellm_types/test.py`

 * *Files identical despite different names*

