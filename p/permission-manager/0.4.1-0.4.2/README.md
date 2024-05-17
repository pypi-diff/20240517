# Comparing `tmp/permission_manager-0.4.1.tar.gz` & `tmp/permission_manager-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permission_manager-0.4.1.tar", max compression
+gzip compressed data, was "permission_manager-0.4.2.tar", max compression
```

## Comparing `permission_manager-0.4.1.tar` & `permission_manager-0.4.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1075 2024-05-15 22:44:43.048700 permission_manager-0.4.1/LICENSE
--rw-r--r--   0        0        0     2602 2024-05-15 22:44:43.048700 permission_manager-0.4.1/README.md
--rw-r--r--   0        0        0      160 2024-05-15 22:44:43.048700 permission_manager-0.4.1/permission_manager/__init__.py
--rw-r--r--   0        0        0     1464 2024-05-15 22:44:43.048700 permission_manager-0.4.1/permission_manager/decorators.py
--rw-r--r--   0        0        0      296 2024-05-15 22:44:43.048700 permission_manager-0.4.1/permission_manager/exceptions.py
--rw-r--r--   0        0        0     4633 2024-05-15 22:44:43.048700 permission_manager-0.4.1/permission_manager/manager.py
--rw-r--r--   0        0        0     1495 2024-05-15 22:44:43.048700 permission_manager-0.4.1/permission_manager/result.py
--rw-r--r--   0        0        0      705 2024-05-15 22:44:43.048700 permission_manager-0.4.1/permission_manager/utils.py
--rw-r--r--   0        0        0     2313 2024-05-15 22:44:43.048700 permission_manager-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 permission_manager-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-17 21:07:59.389009 permission_manager-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2938 2024-05-17 21:07:59.389009 permission_manager-0.4.2/README.md
+-rw-r--r--   0        0        0      327 2024-05-17 21:07:59.389009 permission_manager-0.4.2/permission_manager/__init__.py
+-rw-r--r--   0        0        0     1984 2024-05-17 21:07:59.389009 permission_manager-0.4.2/permission_manager/decorators.py
+-rw-r--r--   0        0        0      552 2024-05-17 21:07:59.389009 permission_manager-0.4.2/permission_manager/exceptions.py
+-rw-r--r--   0        0        0     7756 2024-05-17 21:07:59.389009 permission_manager-0.4.2/permission_manager/manager.py
+-rw-r--r--   0        0        0     1963 2024-05-17 21:07:59.389009 permission_manager-0.4.2/permission_manager/result.py
+-rw-r--r--   0        0        0      418 2024-05-17 21:07:59.389009 permission_manager-0.4.2/permission_manager/types.py
+-rw-r--r--   0        0        0     1146 2024-05-17 21:07:59.389009 permission_manager-0.4.2/permission_manager/utils.py
+-rw-r--r--   0        0        0     2476 2024-05-17 21:07:59.389009 permission_manager-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3647 1970-01-01 00:00:00.000000 permission_manager-0.4.2/PKG-INFO
```

### Comparing `permission_manager-0.4.1/LICENSE` & `permission_manager-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `permission_manager-0.4.1/README.md` & `permission_manager-0.4.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Permission Manager
 
+![example workflow](https://github.com/kindlycat/permission-manager/actions/workflows/tests.yml/badge.svg)
+[![codecov](https://codecov.io/gh/kindlycat/permission-manager/graph/badge.svg?token=XET0GPM9VW)](https://codecov.io/gh/kindlycat/permission-manager)
+
 A simple way to manage object permissions.
 
 Full documentation on [read the docs](https://permission-manager.readthedocs.io/en/latest/).
 
 ## Install
 
 ```bash
@@ -61,17 +64,17 @@
     user=User(name='Ms. Perkins'),
 )
 manager.has_permission('delete')
 # > False
 manager.has_permission('access')
 # > PermissionResult(value=False, message=['Due status'])
 
-manager.resolve()
+manager.resolve(actions=('access', 'create', 'delete'))
 # > {'access': False, 'create': True, 'delete': False}
-manager.resolve(with_messages=True)
+manager.resolve(actions=('access', 'create', 'delete'), with_messages=True)
 # > {'access': {'allow': False, 'messages': ['Due status']},
 #    'create': {'allow': True, 'messages': None},
 #    'delete': {'allow': False, 'messages': None}}
 ```
 
 Also, it's include `PermissionManager`, which add additional functionality to check parent permissions
```

### Comparing `permission_manager-0.4.1/permission_manager/result.py` & `permission_manager-0.4.2/permission_manager/result.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 from dataclasses import dataclass
 
 
 @dataclass
 class PermissionResult:
-    """Class for storing permission values and messages.
+    """Dataclass for storing permission value and messages.
 
     Attributes:
         message (str | list | None): The message associated with the
-            permission result.
+            permission result. It can be a string, a list of strings, or None.
         value (bool): The boolean value indicating the permission result.
         message_if_true (bool): A flag indicating whether to include the
             message when the value is True.
     """
 
     message: str | list | None = None
     value: bool = False
     message_if_true: bool = False
 
     def __post_init__(self) -> None:
-        """Ensure the value is a list."""
+        """Ensure the message attribute is a list.
+
+        If the message attribute is not a list, convert it to a list.
+        """
         if self.message and not isinstance(self.message, list):
             self.message = [self.message]
 
     def __bool__(self) -> bool:
-        """Return the boolean value of the PermissionResult object."""
+        """Return the boolean value of the PermissionResult object.
+
+        Returns:
+            bool: The boolean value indicating the permission result.
+        """
         return self.value
 
     def __repr__(self) -> str:
-        """Return a string representation of the PermissionResult object."""
+        """Return a string representation of the PermissionResult object.
+
+        Returns:
+            str: A string representation of the PermissionResult object.
+        """
         return (
             f'PermissionResult(value={self.value!r}, message={self.message!r})'
         )
 
     @property
     def returned_message(self) -> list | None:
         """Return the message based on the value and message_if_true flag.
 
+        If the value is True and message_if_true is False, return None.
+        Otherwise, return the message.
+
         Returns:
-            list | None: The message associated with the permission result,
-                or None if the value is True and message_if_true is False.
+            list | None: The message associated with the permission
+                result, or None if the value is True and message_if_true is
+                False.
         """
         if self.value and not self.message_if_true:
             return None
         return self.message
```

### Comparing `permission_manager-0.4.1/pyproject.toml` & `permission_manager-0.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "permission-manager"
-version = "0.4.1"
+version = "0.4.2"
 description = "A simple way to manage object permissions."
 authors = ["Grigory Mishchenko <grishkokot@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "permission_manager"}]
 repository = "https://github.com/kindlycat/permission-manager"
 keywords = ["permissions"]
@@ -97,13 +97,22 @@
 indent-style = "space"
 skip-magic-trailing-comma = false
 line-ending = "auto"
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
+[tool.ruff.lint.flake8-self]
+ignore-names = ["_actions", "_aliases"]
+
 [tool.pytest.ini_options]
 testpaths = ["tests"]
-addopts = "-ra -s"
+addopts = "-ra -s -v"
 
-[tool.ruff.lint.flake8-self]
-ignore-names = ["_actions", "_aliases"]
+[tool.coverage.run]
+source = ["permission_manager"]
+omit = ["permission_manager/types.py"]
+
+[tool.coverage.report]
+exclude_also = [
+    "if TYPE_CHECKING:",
+]
```

### Comparing `permission_manager-0.4.1/PKG-INFO` & `permission_manager-0.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permission-manager
-Version: 0.4.1
+Version: 0.4.2
 Summary: A simple way to manage object permissions.
 Home-page: https://github.com/kindlycat/permission-manager
 License: MIT
 Keywords: permissions
 Author: Grigory Mishchenko
 Author-email: grishkokot@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -15,14 +15,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/kindlycat/permission-manager
 Description-Content-Type: text/markdown
 
 # Permission Manager
 
+![example workflow](https://github.com/kindlycat/permission-manager/actions/workflows/tests.yml/badge.svg)
+[![codecov](https://codecov.io/gh/kindlycat/permission-manager/graph/badge.svg?token=XET0GPM9VW)](https://codecov.io/gh/kindlycat/permission-manager)
+
 A simple way to manage object permissions.
 
 Full documentation on [read the docs](https://permission-manager.readthedocs.io/en/latest/).
 
 ## Install
 
 ```bash
@@ -80,17 +83,17 @@
     user=User(name='Ms. Perkins'),
 )
 manager.has_permission('delete')
 # > False
 manager.has_permission('access')
 # > PermissionResult(value=False, message=['Due status'])
 
-manager.resolve()
+manager.resolve(actions=('access', 'create', 'delete'))
 # > {'access': False, 'create': True, 'delete': False}
-manager.resolve(with_messages=True)
+manager.resolve(actions=('access', 'create', 'delete'), with_messages=True)
 # > {'access': {'allow': False, 'messages': ['Due status']},
 #    'create': {'allow': True, 'messages': None},
 #    'delete': {'allow': False, 'messages': None}}
 ```
 
 Also, it's include `PermissionManager`, which add additional functionality to check parent permissions
```

