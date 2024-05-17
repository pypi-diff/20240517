# Comparing `tmp/rfc9457-0.0.3.tar.gz` & `tmp/rfc9457-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfc9457-0.0.3.tar", max compression
+gzip compressed data, was "rfc9457-0.0.4.tar", max compression
```

## Comparing `rfc9457-0.0.3.tar` & `rfc9457-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11307 2024-05-16 07:59:06.192672 rfc9457-0.0.3/LICENSE
--rw-r--r--   0        0        0     1789 2024-05-16 07:59:06.192672 rfc9457-0.0.3/README.md
--rw-r--r--   0        0        0     2021 2024-05-16 07:59:06.192672 rfc9457-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2621 2024-05-16 07:59:06.192672 rfc9457-0.0.3/src/rfc9457/__init__.py
--rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 rfc9457-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11307 2024-05-17 08:47:51.051562 rfc9457-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1789 2024-05-17 08:47:51.055562 rfc9457-0.0.4/README.md
+-rw-r--r--   0        0        0     2021 2024-05-17 08:47:51.055562 rfc9457-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2723 2024-05-17 08:47:51.055562 rfc9457-0.0.4/src/rfc9457/__init__.py
+-rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 rfc9457-0.0.4/PKG-INFO
```

### Comparing `rfc9457-0.0.3/LICENSE` & `rfc9457-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rfc9457-0.0.3/README.md` & `rfc9457-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rfc9457-0.0.3/pyproject.toml` & `rfc9457-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rfc9457"
-version = "0.0.3"
+version = "0.0.4"
 description = "Implementation of RFC9457 problems."
 authors = ["Daniel Edgecombe <daniel@nrwl.co>"]
 license = "Apache-2.0"
 repository="https://github.com/NRWLDev/rfc9457/"
 homepage="https://github.com/NRWLDev/rfc9457/"
 readme = "README.md"
 
@@ -19,15 +19,15 @@
 pytest-random-order = "^1.0"
 
 # Style
 ruff = "^0.3"
 pre-commit = "^3.0.2"
 
 [tool.bumpversion]
-current_version = "0.0.3"
+current_version = "0.0.4"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `rfc9457-0.0.3/src/rfc9457/__init__.py` & `rfc9457-0.0.4/src/rfc9457/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         **kwargs,
     ) -> None:
         super().__init__(title)
         self._type = type_
         self.title = title
         self.details = details
         self.status = status
+        self.status_code = status  # work around for sentry integrations that expect status_code attr
         self.extras = kwargs
 
     @property
     def type(self: t.Self) -> str:
         type_ = error_class_to_type(self)
         return self._type if self._type else type_
```

### Comparing `rfc9457-0.0.3/PKG-INFO` & `rfc9457-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfc9457
-Version: 0.0.3
+Version: 0.0.4
 Summary: Implementation of RFC9457 problems.
 Home-page: https://github.com/NRWLDev/rfc9457/
 License: Apache-2.0
 Author: Daniel Edgecombe
 Author-email: daniel@nrwl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

