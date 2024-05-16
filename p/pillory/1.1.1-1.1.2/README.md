# Comparing `tmp/pillory-1.1.1.tar.gz` & `tmp/pillory-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillory-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pillory-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pillory-1.1.1.tar` & `pillory-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      797 2024-05-16 16:46:40.421772 pillory-1.1.1/.circleci/config.yml
--rw-r--r--   0        0        0       50 2024-05-16 16:46:40.421772 pillory-1.1.1/.gitignore
--rw-r--r--   0        0        0      359 2024-05-16 16:46:40.421772 pillory-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     9161 2024-05-16 16:46:40.421772 pillory-1.1.1/LICENSE
--rw-r--r--   0        0        0      354 2024-05-16 16:46:40.421772 pillory-1.1.1/Makefile
--rw-r--r--   0        0        0     4793 2024-05-16 16:46:40.421772 pillory-1.1.1/README.md
--rw-r--r--   0        0        0     1372 2024-05-16 16:46:40.421772 pillory-1.1.1/dev-requirements.txt
--rw-r--r--   0        0        0       41 2024-05-16 16:46:40.421772 pillory-1.1.1/example/__init__.py
--rw-r--r--   0        0        0      311 2024-05-16 16:46:40.421772 pillory-1.1.1/example/definition.py
--rw-r--r--   0        0        0      180 2024-05-16 16:46:40.421772 pillory-1.1.1/example/empty/README.txt
--rw-r--r--   0        0        0      649 2024-05-16 16:46:40.421772 pillory-1.1.1/example/test_use.py
--rw-r--r--   0        0        0      222 2024-05-16 16:46:40.421772 pillory-1.1.1/example/use.py
--rwxr-xr-x   0        0        0     8702 2024-05-16 16:46:40.421772 pillory-1.1.1/pillory.py
--rw-r--r--   0        0        0     1093 2024-05-16 16:46:40.421772 pillory-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1245 2024-05-16 16:46:40.421772 pillory-1.1.1/test_example.py
--rw-r--r--   0        0        0     2797 2024-05-16 16:46:40.421772 pillory-1.1.1/test_pillory.py
--rw-r--r--   0        0        0     5376 1970-01-01 00:00:00.000000 pillory-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      797 2024-05-16 18:23:23.574022 pillory-1.1.2/.circleci/config.yml
+-rw-r--r--   0        0        0       50 2024-05-16 18:23:23.574022 pillory-1.1.2/.gitignore
+-rw-r--r--   0        0        0      359 2024-05-16 18:23:23.574022 pillory-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9161 2024-05-16 18:23:23.574022 pillory-1.1.2/LICENSE
+-rw-r--r--   0        0        0      354 2024-05-16 18:23:23.574022 pillory-1.1.2/Makefile
+-rw-r--r--   0        0        0     4793 2024-05-16 18:23:23.574022 pillory-1.1.2/README.md
+-rw-r--r--   0        0        0     1372 2024-05-16 18:23:23.574022 pillory-1.1.2/dev-requirements.txt
+-rw-r--r--   0        0        0       41 2024-05-16 18:23:23.574022 pillory-1.1.2/example/__init__.py
+-rw-r--r--   0        0        0      311 2024-05-16 18:23:23.574022 pillory-1.1.2/example/definition.py
+-rw-r--r--   0        0        0      180 2024-05-16 18:23:23.574022 pillory-1.1.2/example/empty/README.txt
+-rw-r--r--   0        0        0      649 2024-05-16 18:23:23.574022 pillory-1.1.2/example/test_use.py
+-rw-r--r--   0        0        0      222 2024-05-16 18:23:23.574022 pillory-1.1.2/example/use.py
+-rwxr-xr-x   0        0        0     9834 2024-05-16 18:23:23.574022 pillory-1.1.2/pillory.py
+-rw-r--r--   0        0        0     1093 2024-05-16 18:23:23.574022 pillory-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1245 2024-05-16 18:23:23.574022 pillory-1.1.2/test_example.py
+-rw-r--r--   0        0        0     2827 2024-05-16 18:23:23.574022 pillory-1.1.2/test_pillory.py
+-rw-r--r--   0        0        0     5376 1970-01-01 00:00:00.000000 pillory-1.1.2/PKG-INFO
```

### Comparing `pillory-1.1.1/.circleci/config.yml` & `pillory-1.1.2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `pillory-1.1.1/LICENSE` & `pillory-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pillory-1.1.1/README.md` & `pillory-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pillory-1.1.1/dev-requirements.txt` & `pillory-1.1.2/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `pillory-1.1.1/example/test_use.py` & `pillory-1.1.2/example/test_use.py`

 * *Files identical despite different names*

### Comparing `pillory-1.1.1/pillory.py` & `pillory-1.1.2/pillory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """A linter to scrutinize how you are using mocks in Python."""
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 # pyright: strict
 
 import ast
+import logging
 import pathlib
 import sys
 from collections.abc import Iterator
 
 # Excludes taken from ruff.
 EXCLUDE = [
     ".bzr",
@@ -171,42 +172,79 @@
     for item in path.iterdir():
         if item.is_file() and item.suffix == ".py" and item.name != "__init__.py":
             yield item.stem
         elif item.is_dir() and item.name != "__pycache__":
             yield item.name
 
 
-def find_errors(patches: list[ast.Call]) -> Iterator[tuple[str, int, int, str]]:
+def find_errors(
+    patches: list[ast.Call], file: str
+) -> Iterator[tuple[str, int, int, str]]:
     """
     Decide whether each patch call has errors or not.
 
     The return value is a tuple that matches the input args for format_message.
 
     It is assumed that all the patches are in the same file.
 
     This function won't import any modules, but it will search the file system and
     ast.parse files to decide whether the right thing was patched or not.
+
+    file is just used for logging.
     """
+    logger = logging.getLogger(__name__)
     for node in patches:
         args = node.args
         if len(args) == 0:
+            logger.debug(
+                "%s:%s:%s: patch call with no args", file, node.lineno, node.col_offset
+            )
             continue
         first_arg = args[0]
         if not isinstance(first_arg, ast.Constant):
+            logger.debug(
+                "%s:%s:%s: patch arg not a constant", file, node.lineno, node.col_offset
+            )
             continue
         name = first_arg.value
         if not isinstance(name, str):
+            logger.debug(
+                "%s:%s:%s: patch arg not a str (%s)",
+                file,
+                node.lineno,
+                node.col_offset,
+                repr(name),
+            )
+            continue
+        if "." not in name:
+            logger.debug(
+                "%s:%s:%s: patch arg not an import name (%s)",
+                file,
+                node.lineno,
+                node.col_offset,
+                repr(name),
+            )
             continue
         if name.split(".", 1)[0] == "builtins":
             yield ("PM103", node.lineno, node.col_offset, name)
             # builtins isn't a normal module found in path, so even though it could be
             # possible for there to be more errors on the same line, we don't check for
             # them because it would need special handling.
             continue
-        source_path, remaining = find_importable(name, sys.path)
+        try:
+            source_path, remaining = find_importable(name, sys.path)
+        except (LookupError, ValueError):
+            logger.debug(
+                "%s:%s:%s: could not find %s in sys.path",
+                file,
+                node.lineno,
+                node.col_offset,
+                name,
+            )
+            continue
         if "." in remaining:
             yield ("PM102", node.lineno, node.col_offset, name)
         source_path = pathlib.Path(source_path)
         if source_path.is_dir():
             definitions = find_package_definitions(str(source_path))
         else:
             definitions = find_module_definitions(source_path.read_text())
@@ -245,14 +283,14 @@
         visitor = MockImportVisitor()
         try:
             parsed_module = ast.parse(source)
         except SyntaxError:
             continue
         visitor = MockImportVisitor()
         visitor.visit(parsed_module)
-        errors = find_errors(visitor.patches)
+        errors = find_errors(visitor.patches, str(file))
         for rule_code, lineno, col_offset, arg in errors:
             print(format_message(str(file), lineno, col_offset, rule_code, arg))
 
 
 if __name__ == "__main__":
     main(sys.argv)
```

### Comparing `pillory-1.1.1/pyproject.toml` & `pillory-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pillory-1.1.1/test_example.py` & `pillory-1.1.2/test_example.py`

 * *Files identical despite different names*

### Comparing `pillory-1.1.1/test_pillory.py` & `pillory-1.1.2/test_pillory.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
                         ast.Call(
                             func=ast.Name(id="patch", ctx=ast.Load()),
                             args=[ast.Constant(value="builtins.open")],
                             lineno=1,
                             col_offset=0,
                         )
                     ],
+                    "hey.py",
                 )
             ),
             [("PM103", 1, 0, "builtins.open")],
         )
 
     def test_find_importable(self):
         self.assertEqual(
```

### Comparing `pillory-1.1.1/PKG-INFO` & `pillory-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillory
-Version: 1.1.1
+Version: 1.1.2
 Summary: A linter to scrutinize how you are using mocks in Python.
 Author-email: Fergal Armstrong <patio.algebra0i@icloud.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: coverage~=7.5 ; extra == "dev"
 Requires-Dist: flit~=3.9 ; extra == "dev"
 Requires-Dist: pip-tools~=7.4 ; extra == "dev"
```

