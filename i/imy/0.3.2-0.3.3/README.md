# Comparing `tmp/imy-0.3.2.tar.gz` & `tmp/imy-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imy-0.3.2.tar", max compression
+gzip compressed data, was "imy-0.3.3.tar", max compression
```

## Comparing `imy-0.3.2.tar` & `imy-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.3.2/LICENSE
--rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.3.2/README.md
--rw-r--r--   0        0        0        0 2024-04-22 13:27:52.000000 imy-0.3.2/imy/__init__.py
--rw-r--r--   0        0        0     6727 2024-04-26 06:20:02.579623 imy-0.3.2/imy/assets.py
--rw-r--r--   0        0        0     6395 2024-04-29 15:43:18.799268 imy-0.3.2/imy/async_utils.py
--rw-r--r--   0        0        0     9840 2024-04-22 13:49:54.000000 imy-0.3.2/imy/config.py
--rw-r--r--   0        0        0     1112 2024-04-29 16:01:49.458562 imy-0.3.2/imy/docstrings/__init__.py
--rw-r--r--   0        0        0     6538 2024-05-16 08:25:56.236283 imy-0.3.2/imy/docstrings/data_models.py
--rw-r--r--   0        0        0    18612 2024-05-16 08:25:56.236283 imy-0.3.2/imy/docstrings/parsers.py
--rw-r--r--   0        0        0     8578 2024-04-25 19:05:06.904544 imy-0.3.2/imy/inject.py
--rw-r--r--   0        0        0    14594 2024-04-29 15:43:49.552681 imy-0.3.2/imy/logs.py
--rw-r--r--   0        0        0     3185 2024-04-22 13:27:52.000000 imy-0.3.2/imy/package_metadata.py
--rw-r--r--   0        0        0      753 2024-05-16 08:25:59.966294 imy-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 imy-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.3.3/LICENSE
+-rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 13:27:52.000000 imy-0.3.3/imy/__init__.py
+-rw-r--r--   0        0        0     6727 2024-04-26 06:20:02.579623 imy-0.3.3/imy/assets.py
+-rw-r--r--   0        0        0     6395 2024-04-29 15:43:18.799268 imy-0.3.3/imy/async_utils.py
+-rw-r--r--   0        0        0     9840 2024-04-22 13:49:54.000000 imy-0.3.3/imy/config.py
+-rw-r--r--   0        0        0     1112 2024-04-29 16:01:49.458562 imy-0.3.3/imy/docstrings/__init__.py
+-rw-r--r--   0        0        0     6585 2024-05-16 18:35:39.095175 imy-0.3.3/imy/docstrings/data_models.py
+-rw-r--r--   0        0        0    19129 2024-05-16 18:35:39.095175 imy-0.3.3/imy/docstrings/parsers.py
+-rw-r--r--   0        0        0     8578 2024-04-25 19:05:06.904544 imy-0.3.3/imy/inject.py
+-rw-r--r--   0        0        0    14594 2024-04-29 15:43:49.552681 imy-0.3.3/imy/logs.py
+-rw-r--r--   0        0        0     3185 2024-04-22 13:27:52.000000 imy-0.3.3/imy/package_metadata.py
+-rw-r--r--   0        0        0      753 2024-05-16 18:35:52.798465 imy-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 imy-0.3.3/PKG-INFO
```

### Comparing `imy-0.3.2/LICENSE` & `imy-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `imy-0.3.2/imy/assets.py` & `imy-0.3.3/imy/assets.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.2/imy/async_utils.py` & `imy-0.3.3/imy/async_utils.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.2/imy/config.py` & `imy-0.3.3/imy/config.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.2/imy/docstrings/__init__.py` & `imy-0.3.3/imy/docstrings/__init__.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.2/imy/docstrings/data_models.py` & `imy-0.3.3/imy/docstrings/data_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,16 @@
 
     object: Callable
 
     name: str
     parameters: list[FunctionParameter]
     return_type: introspection.types.TypeAnnotation | Unset
     synchronous: bool
+    class_method: bool
+    static_method: bool
 
     summary: str | None
     details: str | None
 
     raises: list[tuple[str, str]]  # type, description
 
     metadata: FunctionMetadata
```

### Comparing `imy-0.3.2/imy/docstrings/parsers.py` & `imy-0.3.3/imy/docstrings/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,15 +231,17 @@
     return data_models.Docstring(
         summary=summary,
         details=details,
         key_sections=key_value_sections,
     )
 
 
-def parse_function(func: Callable[..., Any]) -> data_models.FunctionDocs:
+def parse_function(
+    func: Callable[..., Any] | classmethod | staticmethod,
+) -> data_models.FunctionDocs:
     """
     Given a function, parse its signature and docstring into a `FunctionDocs`
     object.
     """
 
     def parse_annotation(
         annotation: object,
@@ -269,14 +271,23 @@
             func.__module__,
             extra_globals=extra_globals,
             mode="ast",
             treat_name_errors_as_imports=True,
             strict=True,
         )
 
+    is_class_method = is_static_method = False
+
+    if isinstance(func, staticmethod):
+        is_static_method = True
+        func = func.__func__
+    elif isinstance(func, classmethod):
+        is_class_method = True
+        func = func.__func__
+
     # Parse the parameters
     signature = inspect.signature(func)
     parameters: dict[str, data_models.FunctionParameter] = {}
 
     for param_name, param in signature.parameters.items():
         if param.default == inspect.Parameter.empty:
             param_default = data_models.UNSET
@@ -369,14 +380,16 @@
     # Build the result
     return data_models.FunctionDocs(
         object=func,
         name=func.__name__,
         parameters=list(parameters.values()),
         return_type=parse_annotation(signature.return_annotation),
         synchronous=not inspect.iscoroutinefunction(func),
+        class_method=is_class_method,
+        static_method=is_static_method,
         summary=parsed.summary,
         details=parsed.details,
         raises=raises,
         metadata=metadata,
     )
 
 
@@ -446,17 +459,22 @@
     def add_functions(cls: type) -> None:
         # Chain to the base classes
         for base in cls.__bases__:
             add_functions(base)
 
         # Then process this class. This way locals functions override inherited
         # ones.
-        for name, func in inspect.getmembers(cls, inspect.isfunction):
-            func_docs = parse_function(func)
-            functions_by_name[name] = func_docs
+        for name, func in vars(cls).items():
+            if (
+                inspect.isfunction(func)
+                or isinstance(func, classmethod)
+                or isinstance(func, staticmethod)
+            ):
+                func_docs = parse_function(func)
+                functions_by_name[name] = func_docs
 
     add_functions(cls)
 
     # Do the same for fields
     fields_by_name: dict[str, data_models.ClassField] = {}
 
     def add_fields(cls: type) -> None:
```

### Comparing `imy-0.3.2/imy/inject.py` & `imy-0.3.3/imy/inject.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.2/imy/logs.py` & `imy-0.3.3/imy/logs.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.2/imy/package_metadata.py` & `imy-0.3.3/imy/package_metadata.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.2/pyproject.toml` & `imy-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "imy"
-version = "0.3.2"
+version = "0.3.3"
 description = "Random utilities I can't go without"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/i-miss-you"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `imy-0.3.2/PKG-INFO` & `imy-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imy
-Version: 0.3.2
+Version: 0.3.3
 Summary: Random utilities I can't go without
 Home-page: https://gitlab.com/Vivern/i-miss-you
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

