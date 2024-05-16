# Comparing `tmp/py_grpcio-1.4.3.tar.gz` & `tmp/py_grpcio-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_grpcio-1.4.3.tar", max compression
+gzip compressed data, was "py_grpcio-1.4.4.tar", max compression
```

## Comparing `py_grpcio-1.4.3.tar` & `py_grpcio-1.4.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1076 2024-05-15 21:28:04.496798 py_grpcio-1.4.3/LICENSE
--rw-r--r--   0        0        0     4581 2024-05-15 21:28:04.496798 py_grpcio-1.4.3/README.md
--rw-r--r--   0        0        0      167 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/__init__.py
--rw-r--r--   0        0        0      796 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/exceptions.py
--rw-r--r--   0        0        0     1961 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/interceptor.py
--rw-r--r--   0        0        0     5102 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/method.py
--rw-r--r--   0        0        0     1148 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/middleware.py
--rw-r--r--   0        0        0     5421 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/models.py
--rw-r--r--   0        0        0      114 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/proto/__init__.py
--rw-r--r--   0        0        0      483 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/proto/enums.py
--rw-r--r--   0        0        0     3882 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/proto/parser.py
--rw-r--r--   0        0        0      686 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/proto/templates/service.proto.template
--rw-r--r--   0        0        0     1921 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/server.py
--rw-r--r--   0        0        0      924 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/service.py
--rw-r--r--   0        0        0     2727 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/service_meta.py
--rw-r--r--   0        0        0      582 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/utils.py
--rw-r--r--   0        0        0      573 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 py_grpcio-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/LICENSE
+-rw-r--r--   0        0        0     4581 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/README.md
+-rw-r--r--   0        0        0      307 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/__meta__.py
+-rw-r--r--   0        0        0      796 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/exceptions.py
+-rw-r--r--   0        0        0     1961 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/interceptor.py
+-rw-r--r--   0        0        0     5102 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/method.py
+-rw-r--r--   0        0        0     1148 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/middleware.py
+-rw-r--r--   0        0        0     5588 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/models.py
+-rw-r--r--   0        0        0      114 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/proto/__init__.py
+-rw-r--r--   0        0        0      483 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/proto/enums.py
+-rw-r--r--   0        0        0     3882 2024-05-16 22:24:26.769816 py_grpcio-1.4.4/py_grpcio/proto/parser.py
+-rw-r--r--   0        0        0      686 2024-05-16 22:24:26.769816 py_grpcio-1.4.4/py_grpcio/proto/templates/service.proto.template
+-rw-r--r--   0        0        0     1921 2024-05-16 22:24:26.769816 py_grpcio-1.4.4/py_grpcio/server.py
+-rw-r--r--   0        0        0      924 2024-05-16 22:24:26.769816 py_grpcio-1.4.4/py_grpcio/service.py
+-rw-r--r--   0        0        0     2727 2024-05-16 22:24:26.769816 py_grpcio-1.4.4/py_grpcio/service_meta.py
+-rw-r--r--   0        0        0      582 2024-05-16 22:24:26.769816 py_grpcio-1.4.4/py_grpcio/utils.py
+-rw-r--r--   0        0        0      573 2024-05-16 22:24:26.769816 py_grpcio-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 py_grpcio-1.4.4/PKG-INFO
```

### Comparing `py_grpcio-1.4.3/LICENSE` & `py_grpcio-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.3/README.md` & `py_grpcio-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.3/py_grpcio/exceptions.py` & `py_grpcio-1.4.4/py_grpcio/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.3/py_grpcio/interceptor.py` & `py_grpcio-1.4.4/py_grpcio/interceptor.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.3/py_grpcio/method.py` & `py_grpcio-1.4.4/py_grpcio/method.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.3/py_grpcio/middleware.py` & `py_grpcio-1.4.4/py_grpcio/middleware.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.3/py_grpcio/models.py` & `py_grpcio-1.4.4/py_grpcio/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,24 +38,26 @@
         ]
 
     @classmethod
     def get_additional_messages(
         cls, model_fields: dict[str, FieldInfo] | None = None
     ) -> dict[str, Type['Message']]:
         messages: dict[str, Type[Message]] = {}
-        for field_name, field_info in (model_fields and model_fields.items()) or cls.model_fields.items():
+        for field_name, field_info in (model_fields is not None and model_fields.items()) or cls.model_fields.items():
             field_type: type | None = field_info.annotation
             if isclass(field_type) and issubclass(field_type, Message):
                 messages[field_type.__name__]: Type[Message] = field_type
                 if additional_messages := cls.get_additional_messages(model_fields=field_type.model_fields):
                     messages.update(**additional_messages)
             elif isinstance(field_type, GenericAlias) and (origin := get_origin(tp=field_type)) is not None:
                 if issubclass(origin, Iterable):
                     if len(args := field_type.__args__) != 1:
-                        raise
+                        raise TypeError(
+                            f'Field `{field_name}`: type `{field_type}` must have only one subtype, not {len(args)}.'
+                        )
                     if isclass(sub_field_type := args[0]) and issubclass(sub_field_type, Message):
                         messages[sub_field_type.__name__]: Type[Message] = sub_field_type
                         if additional_messages := cls.get_additional_messages(model_fields=sub_field_type.model_fields):
                             messages.update(**additional_messages)
         return messages
```

### Comparing `py_grpcio-1.4.3/py_grpcio/proto/parser.py` & `py_grpcio-1.4.4/py_grpcio/proto/parser.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.3/py_grpcio/proto/templates/service.proto.template` & `py_grpcio-1.4.4/py_grpcio/proto/templates/service.proto.template`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.3/py_grpcio/server.py` & `py_grpcio-1.4.4/py_grpcio/server.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.3/py_grpcio/service.py` & `py_grpcio-1.4.4/py_grpcio/service.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.3/py_grpcio/service_meta.py` & `py_grpcio-1.4.4/py_grpcio/service_meta.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.3/py_grpcio/utils.py` & `py_grpcio-1.4.4/py_grpcio/utils.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.3/pyproject.toml` & `py_grpcio-1.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-grpcio"
-version = "1.4.3"
+version = "1.4.4"
 description = "gRPC with autogen by Pydantic models"
 authors = ["Yurii <ykolibroda@lytvynov-production.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "py_grpcio" },
 ]
```

### Comparing `py_grpcio-1.4.3/PKG-INFO` & `py_grpcio-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-grpcio
-Version: 1.4.3
+Version: 1.4.4
 Summary: gRPC with autogen by Pydantic models
 License: MIT
 Author: Yurii
 Author-email: ykolibroda@lytvynov-production.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

