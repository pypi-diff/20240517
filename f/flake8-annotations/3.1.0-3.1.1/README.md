# Comparing `tmp/flake8_annotations-3.1.0.tar.gz` & `tmp/flake8_annotations-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_annotations-3.1.0.tar", max compression
+gzip compressed data, was "flake8_annotations-3.1.1.tar", max compression
```

## Comparing `flake8_annotations-3.1.0.tar` & `flake8_annotations-3.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7572 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1073 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/LICENSE
--rw-r--r--   0        0        0    11348 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/README.md
--rw-r--r--   0        0        0       22 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/flake8_annotations/__init__.py
--rw-r--r--   0        0        0    17308 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/flake8_annotations/ast_walker.py
--rw-r--r--   0        0        0    13831 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/flake8_annotations/checker.py
--rw-r--r--   0        0        0      893 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/flake8_annotations/enums.py
--rw-r--r--   0        0        0     6046 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/flake8_annotations/error_codes.py
--rw-r--r--   0        0        0     2362 2024-05-06 18:47:49.594710 flake8_annotations-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    12716 1970-01-01 00:00:00.000000 flake8_annotations-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7666 2024-05-17 14:07:44.900561 flake8_annotations-3.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1073 2024-05-17 14:07:44.900561 flake8_annotations-3.1.1/LICENSE
+-rw-r--r--   0        0        0    11572 2024-05-17 14:07:44.900561 flake8_annotations-3.1.1/README.md
+-rw-r--r--   0        0        0       22 2024-05-17 14:07:44.900561 flake8_annotations-3.1.1/flake8_annotations/__init__.py
+-rw-r--r--   0        0        0    17308 2024-05-17 14:07:44.900561 flake8_annotations-3.1.1/flake8_annotations/ast_walker.py
+-rw-r--r--   0        0        0    14257 2024-05-17 14:07:44.900561 flake8_annotations-3.1.1/flake8_annotations/checker.py
+-rw-r--r--   0        0        0      893 2024-05-17 14:07:44.900561 flake8_annotations-3.1.1/flake8_annotations/enums.py
+-rw-r--r--   0        0        0     6046 2024-05-17 14:07:44.900561 flake8_annotations-3.1.1/flake8_annotations/error_codes.py
+-rw-r--r--   0        0        0     2362 2024-05-17 14:07:44.900561 flake8_annotations-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12940 1970-01-01 00:00:00.000000 flake8_annotations-3.1.1/PKG-INFO
```

### Comparing `flake8_annotations-3.1.0/CHANGELOG.md` & `flake8_annotations-3.1.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Changelog
 Versions follow [Semantic Versioning](https://semver.org/spec/v2.0.0.html) (`<major>`.`<minor>`.`<patch>`)
 
+## [v3.1.1]
+### Changed
+* #167 Add module-level support for the `--respect-type-ignore` flag
+
 ## [v3.1.0]
 ### Added
 * #164 Add `--respect-type-ignore` to support suppression of errors for functions annotated with `type: ignore`
 
 ## [v3.0.1]
 ### Changed
 * #155 Remove upper bound on Python constraint
```

### Comparing `flake8_annotations-3.1.0/LICENSE` & `flake8_annotations-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_annotations-3.1.0/README.md` & `flake8_annotations-3.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # flake8-annotations
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flake8-annotations/3.1.0?logo=python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flake8-annotations/3.1.1?logo=python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
 [![PyPI](https://img.shields.io/pypi/v/flake8-annotations?logo=Python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
 [![PyPI - License](https://img.shields.io/pypi/l/flake8-annotations?color=magenta)](https://github.com/sco1/flake8-annotations/blob/main/LICENSE)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sco1/flake8-annotations/main.svg)](https://results.pre-commit.ci/latest/github/sco1/flake8-annotations/main)
-[![Open in Visual Studio Code](https://img.shields.io/badge/Open%20in-VSCode.dev-blue)](https://github.dev/sco1/flake8-annotations)
 
 `flake8-annotations` is a plugin for [Flake8](http://flake8.pycqa.org/en/latest/) that detects the absence of [PEP 3107-style](https://www.python.org/dev/peps/pep-3107/) function annotations.
 
 What this won't do: replace [mypy](http://mypy-lang.org/), check type comments (see: [PEP 484](https://peps.python.org/pep-0484/#type-comments)), check variable annotations (see: [PEP 526](https://www.python.org/dev/peps/pep-0526/)), or respect stub files.
 
 ## Installation
 Install from PyPi with your favorite `pip` invocation:
@@ -28,15 +27,15 @@
 ver_str = out.stdout.replace("\n", "")
 cog.out(
     f"```bash\n$ flake8 --version\n{ver_str}\n```"
 )
 ]]] -->
 ```bash
 $ flake8 --version
-7.0.0 (flake8-annotations: 3.1.0, mccabe: 0.7.0, pycodestyle: 2.11.1, pyflakes: 3.2.0) CPython 3.12.3 on Darwin
+7.0.0 (flake8-annotations: 3.1.1, mccabe: 0.7.0, pycodestyle: 2.11.1, pyflakes: 3.2.0) CPython 3.12.3 on Darwin
 ```
 <!-- [[[end]]] -->
 
 ## Table of Warnings
 With the exception of `ANN4xx`-level warnings, all warnings are enabled by default.
 
 ### Function Annotations
@@ -137,17 +136,18 @@
 
 ### `--allow-star-arg-any`
 Suppress `ANN401` for dynamically typed `*args` and `**kwargs`.
 
 Default: `False`
 
 ### `--respect-type-ignore`
-Suppress linting errors for functions annotated with a `# type: ignore` comment.
+Suppress linting errors for functions annotated with a `# type: ignore` comment. Support is also provided for module-level blanket ignores (see: [mypy: Ignoring a whole file](https://mypy.readthedocs.io/en/stable/common_issues.html#ignoring-a-whole-file)). 
 
 **NOTE:** Type ignore tags are not considered, e.g. `# type: ignore[arg-type]` is treated the same as `# type: ignore`.
+**NOTE:** Module-level suppression is only considered for the `# mypy: ignore-errors` or `# type: ignore` tags when provided as the sole contents of the first line of the module.
 
 Default: `False`
 
 
 ## Generic Functions
 Per the Python Glossary, a [generic function](https://docs.python.org/3/glossary.html#term-generic-function) is defined as:
```

### Comparing `flake8_annotations-3.1.0/flake8_annotations/ast_walker.py` & `flake8_annotations-3.1.1/flake8_annotations/ast_walker.py`

 * *Files identical despite different names*

### Comparing `flake8_annotations-3.1.0/flake8_annotations/checker.py` & `flake8_annotations-3.1.1/flake8_annotations/checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         self.lines = lines
 
         self.tree = ast.parse("".join(lines), type_comments=True)  # flake8 doesn't strip newlines
 
         # Type ignores are provided by ast at the module level & we'll need them later when deciding
         # whether or not to emit errors for a given function
         self._type_ignore_lineno = {ti.lineno for ti in self.tree.type_ignores}
+        self._has_mypy_ignore_errors = "# mypy: ignore-errors" in lines[0] if lines else False
 
         # Set by flake8's config parser
         self.suppress_none_returning: bool
         self.suppress_dummy_args: bool
         self.allow_untyped_defs: bool
         self.allow_untyped_nested: bool
         self.mypy_init_return: bool
@@ -110,16 +111,24 @@
 
             # If it's not, and it is overload decorated, store it for the next iteration
             if function.has_decorator(self.overload_decorators):
                 last_overload_decorated_function_name = function.name
 
             # Optionally respect a type: ignore comment
             # These are considered at the function level & tags are not considered
-            if self.respect_type_ignore and (function.lineno in self._type_ignore_lineno):
-                continue
+            if self.respect_type_ignore:
+                if function.lineno in self._type_ignore_lineno:
+                    # function-level ignore
+                    continue
+                elif (1 in self._type_ignore_lineno) or (
+                    self._has_mypy_ignore_errors
+                ):  # pragma: no branch
+                    # module-level ignore
+                    # lineno from ast is 1-indexed
+                    continue
 
             # Yield explicit errors for arguments that are missing annotations
             for arg in function.get_missed_annotations():
                 # Check for type comments here since we're not considering them as typed args
                 if arg.has_type_comment:
                     yield error_codes.ANN402.from_argument(arg).to_flake8()
```

### Comparing `flake8_annotations-3.1.0/flake8_annotations/enums.py` & `flake8_annotations-3.1.1/flake8_annotations/enums.py`

 * *Files identical despite different names*

### Comparing `flake8_annotations-3.1.0/flake8_annotations/error_codes.py` & `flake8_annotations-3.1.1/flake8_annotations/error_codes.py`

 * *Files identical despite different names*

### Comparing `flake8_annotations-3.1.0/pyproject.toml` & `flake8_annotations-3.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flake8-annotations"
-version = "3.1.0"
+version = "3.1.1"
 description = "Flake8 Type Annotation Checks"
 license = "MIT"
 readme = "README.md"
 authors = ["S Co1 <sco1.git@gmail.com>"]
 homepage = "https://github.com/sco1/flake8-annotations"
 repository = "https://github.com/sco1/flake8-annotations"
 classifiers = [
```

### Comparing `flake8_annotations-3.1.0/PKG-INFO` & `flake8_annotations-3.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-annotations
-Version: 3.1.0
+Version: 3.1.1
 Summary: Flake8 Type Annotation Checks
 Home-page: https://github.com/sco1/flake8-annotations
 License: MIT
 Author: S Co1
 Author-email: sco1.git@gmail.com
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,19 +28,18 @@
 Requires-Dist: attrs (>=21.4)
 Requires-Dist: flake8 (>=5.0)
 Project-URL: Issue Tracker, https://github.com/sco1/flake8-annotations/issues
 Project-URL: Repository, https://github.com/sco1/flake8-annotations
 Description-Content-Type: text/markdown
 
 # flake8-annotations
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flake8-annotations/3.1.0?logo=python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flake8-annotations/3.1.1?logo=python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
 [![PyPI](https://img.shields.io/pypi/v/flake8-annotations?logo=Python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
 [![PyPI - License](https://img.shields.io/pypi/l/flake8-annotations?color=magenta)](https://github.com/sco1/flake8-annotations/blob/main/LICENSE)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sco1/flake8-annotations/main.svg)](https://results.pre-commit.ci/latest/github/sco1/flake8-annotations/main)
-[![Open in Visual Studio Code](https://img.shields.io/badge/Open%20in-VSCode.dev-blue)](https://github.dev/sco1/flake8-annotations)
 
 `flake8-annotations` is a plugin for [Flake8](http://flake8.pycqa.org/en/latest/) that detects the absence of [PEP 3107-style](https://www.python.org/dev/peps/pep-3107/) function annotations.
 
 What this won't do: replace [mypy](http://mypy-lang.org/), check type comments (see: [PEP 484](https://peps.python.org/pep-0484/#type-comments)), check variable annotations (see: [PEP 526](https://www.python.org/dev/peps/pep-0526/)), or respect stub files.
 
 ## Installation
 Install from PyPi with your favorite `pip` invocation:
@@ -61,15 +60,15 @@
 ver_str = out.stdout.replace("\n", "")
 cog.out(
     f"```bash\n$ flake8 --version\n{ver_str}\n```"
 )
 ]]] -->
 ```bash
 $ flake8 --version
-7.0.0 (flake8-annotations: 3.1.0, mccabe: 0.7.0, pycodestyle: 2.11.1, pyflakes: 3.2.0) CPython 3.12.3 on Darwin
+7.0.0 (flake8-annotations: 3.1.1, mccabe: 0.7.0, pycodestyle: 2.11.1, pyflakes: 3.2.0) CPython 3.12.3 on Darwin
 ```
 <!-- [[[end]]] -->
 
 ## Table of Warnings
 With the exception of `ANN4xx`-level warnings, all warnings are enabled by default.
 
 ### Function Annotations
@@ -170,17 +169,18 @@
 
 ### `--allow-star-arg-any`
 Suppress `ANN401` for dynamically typed `*args` and `**kwargs`.
 
 Default: `False`
 
 ### `--respect-type-ignore`
-Suppress linting errors for functions annotated with a `# type: ignore` comment.
+Suppress linting errors for functions annotated with a `# type: ignore` comment. Support is also provided for module-level blanket ignores (see: [mypy: Ignoring a whole file](https://mypy.readthedocs.io/en/stable/common_issues.html#ignoring-a-whole-file)). 
 
 **NOTE:** Type ignore tags are not considered, e.g. `# type: ignore[arg-type]` is treated the same as `# type: ignore`.
+**NOTE:** Module-level suppression is only considered for the `# mypy: ignore-errors` or `# type: ignore` tags when provided as the sole contents of the first line of the module.
 
 Default: `False`
 
 
 ## Generic Functions
 Per the Python Glossary, a [generic function](https://docs.python.org/3/glossary.html#term-generic-function) is defined as:
```

