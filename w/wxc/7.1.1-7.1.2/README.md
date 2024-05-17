# Comparing `tmp/wxc-7.1.1.tar.gz` & `tmp/wxc-7.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxc-7.1.1.tar", last modified: Fri Sep  8 17:08:54 2023, max compression
+gzip compressed data, was "wxc-7.1.2.tar", last modified: Fri May 17 07:48:05 2024, max compression
```

## Comparing `wxc-7.1.1.tar` & `wxc-7.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:08:54.812105 wxc-7.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-09-08 17:08:45.000000 wxc-7.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2023-09-08 17:08:54.812105 wxc-7.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2023-09-08 17:08:45.000000 wxc-7.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2023-09-08 17:08:45.000000 wxc-7.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-08 17:08:54.812105 wxc-7.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:08:54.808104 wxc-7.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:08:54.812105 wxc-7.1.1/src/wxc/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-08 17:08:45.000000 wxc-7.1.1/src/wxc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      108 2023-09-08 17:08:45.000000 wxc-7.1.1/src/wxc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2023-09-08 17:08:45.000000 wxc-7.1.1/src/wxc/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2023-09-08 17:08:45.000000 wxc-7.1.1/src/wxc/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-09-08 17:08:45.000000 wxc-7.1.1/src/wxc/levenshtein.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:08:54.812105 wxc-7.1.1/src/wxc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2023-09-08 17:08:54.000000 wxc-7.1.1/src/wxc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-09-08 17:08:54.000000 wxc-7.1.1/src/wxc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 17:08:54.000000 wxc-7.1.1/src/wxc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-09-08 17:08:54.000000 wxc-7.1.1/src/wxc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-08 17:08:54.000000 wxc-7.1.1/src/wxc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-09-08 17:08:54.000000 wxc-7.1.1/src/wxc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:08:54.812105 wxc-7.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2023-09-08 17:08:45.000000 wxc-7.1.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-09-08 17:08:45.000000 wxc-7.1.1/tests/test_builtin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2023-09-08 17:08:45.000000 wxc-7.1.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2023-09-08 17:08:45.000000 wxc-7.1.1/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2023-09-08 17:08:45.000000 wxc-7.1.1/tests/test_stdlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:48:05.158438 wxc-7.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-17 07:47:58.000000 wxc-7.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-17 07:48:05.158438 wxc-7.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-17 07:47:58.000000 wxc-7.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-17 07:47:58.000000 wxc-7.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 07:48:05.158438 wxc-7.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:48:05.154438 wxc-7.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:48:05.158438 wxc-7.1.2/src/wxc/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 07:47:58.000000 wxc-7.1.2/src/wxc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-05-17 07:47:58.000000 wxc-7.1.2/src/wxc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-05-17 07:47:58.000000 wxc-7.1.2/src/wxc/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-17 07:47:58.000000 wxc-7.1.2/src/wxc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-17 07:47:58.000000 wxc-7.1.2/src/wxc/levenshtein.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:48:05.158438 wxc-7.1.2/src/wxc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-17 07:48:05.000000 wxc-7.1.2/src/wxc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-17 07:48:05.000000 wxc-7.1.2/src/wxc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 07:48:05.000000 wxc-7.1.2/src/wxc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-17 07:48:05.000000 wxc-7.1.2/src/wxc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 07:48:05.000000 wxc-7.1.2/src/wxc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 07:48:05.000000 wxc-7.1.2/src/wxc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:48:05.158438 wxc-7.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-17 07:47:58.000000 wxc-7.1.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-17 07:47:58.000000 wxc-7.1.2/tests/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-17 07:47:58.000000 wxc-7.1.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-17 07:47:58.000000 wxc-7.1.2/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-17 07:47:58.000000 wxc-7.1.2/tests/test_stdlib.py
```

### Comparing `wxc-7.1.1/LICENSE` & `wxc-7.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wxc-7.1.1/PKG-INFO` & `wxc-7.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxc
-Version: 7.1.1
+Version: 7.1.2
 Summary: A CLI facility to inspect Python environments.
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/wxc
 Project-URL: Changelog, https://github.com/neutrinoceros/wxc/blob/main/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -18,15 +18,14 @@
 
 # wxc
 
 [![PyPI](https://img.shields.io/pypi/v/wxc.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/wxc/)
 [![](https://img.shields.io/badge/contributions-welcome-brightgreen)](https://github.com/neutrinoceros/wxc/pulls)
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/wxc/main.svg)](https://results.pre-commit.ci/latest/github/neutrinoceros/wxc/main)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 
 `wxc` (pronounced "which") allows you to inspect source code in your Python
 environment from the command line. It is based on the `inspect` module from the
 standard library.
```

### Comparing `wxc-7.1.1/README.md` & `wxc-7.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # wxc
 
 [![PyPI](https://img.shields.io/pypi/v/wxc.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/wxc/)
 [![](https://img.shields.io/badge/contributions-welcome-brightgreen)](https://github.com/neutrinoceros/wxc/pulls)
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/wxc/main.svg)](https://results.pre-commit.ci/latest/github/neutrinoceros/wxc/main)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 
 `wxc` (pronounced "which") allows you to inspect source code in your Python
 environment from the command line. It is based on the `inspect` module from the
 standard library.
```

### Comparing `wxc-7.1.1/pyproject.toml` & `wxc-7.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -46,29 +46,29 @@
 [tool.setuptools.dynamic]
 version = {attr = "wxc.__version__"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
 namespaces = false
 
-[tool.ruff]
+[tool.ruff.lint]
 exclude = ["*__init__.py"]
 ignore = ["E501"]
 select = [
     "E",
     "F",
     "W",
     "C4",  # flake8-comprehensions
     "B",   # flake8-bugbear
     "YTT", # flake8-2020
     "I",   # isort
     "UP",  # pyupgrade
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 combine-as-imports = true
 known-first-party = ["wxc"]
 
 [tool.coverage.paths]
 source = [
   "/home/runner/work/wxc",
   "/Users/runner/work/wxc",
```

### Comparing `wxc-7.1.1/src/wxc/api.py` & `wxc-7.1.2/src/wxc/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 from types import BuiltinFunctionType
 
 from wxc.levenshtein import levenshtein_distance
 
 if False:
     # typecheck only
     from collections.abc import Iterable  # type: ignore [unreachable]
-    from typing import Any
+    from typing import Any, TypedDict
+
+    class FullDataDict(TypedDict):
+        source: str | None
+        version: str
+        in_stdlib: bool
 
 
 # sorted by decreasing order of priority
 VERSION_ATTR_LOOKUP_TABLE = ("__version__", "VERSION", "version")
 
 
 def is_builtin(name: str) -> bool:
@@ -107,17 +112,20 @@
         file = inspect.getfile(obj)
     except OSError:
         file = obj.__file__
     except TypeError:
         # this happens for instance with `math.sqrt`
         # because inspect.getfile doesn't work on compiled code
         # the second condition is met for os.fspath
-        if inspect.ismodule(obj) or is_builtin_func(obj):
-            raise
-        if isinstance(obj, property):
+        if (
+            inspect.ismodule(obj)
+            or is_builtin_func(obj)
+            or inspect.getmodule(obj) is builtins
+            or isinstance(obj, property)
+        ):
             raise
         return get_sourcefile(inspect.getmodule(obj))
     return file
 
 
 def get_sourceline(obj):
     import inspect
@@ -149,45 +157,51 @@
         from platform import python_version
 
         return f"Python {python_version()}"
 
     raise LookupError(f"Could not determine version metadata from {package_name!r}")
 
 
-def get_full_data(name: str) -> dict:
-    data = defaultdict(str)
+def get_full_data(name: str) -> FullDataDict:
     package_name, _, _ = name.partition(".")
 
     objects = get_objects(name)
+    _d_source: str | None = None
 
     for obj in reversed(objects):
         try:
             source = get_sourcefile(obj)
         except RecursionError:
             pass
-        except TypeError:
-            # as of Python 3.11, inspect.getfile doesn't have support for properties
-            # but we're not making this a hard failure in case it is added in the future
-            # and we fallback to finding out the sourcefile of the class itself
-            if isinstance(obj, property):
+        except TypeError as exc:
+            if "built-in module" in str(exc):
+                # see https://github.com/neutrinoceros/wxc/issues/233
+                _d_source = "built-in"
+                break
+            elif isinstance(obj, property):
+                # as of Python 3.11, inspect.getfile doesn't have support for properties
+                # but we're not making this a hard failure in case it is added in the future
+                # and we fallback to finding out the sourcefile of the class itself
                 continue
             else:
                 raise
         else:
             try:
                 lineno = get_sourceline(obj)
             except (OSError, TypeError):
                 pass
             else:
                 source += f":{lineno}" if lineno else ""
                 break
             finally:
-                data["source"] = source
+                _d_source = source
 
     try:
-        data["version"] = get_version(package_name)
+        _d_version = get_version(package_name)
     except LookupError:
-        pass
-
-    data["in_stdlib"] = package_name in sys.stdlib_module_names
+        _d_version = "unknown"
 
-    return data
+    return {
+        "source": _d_source,
+        "version": _d_version,
+        "in_stdlib": package_name in sys.stdlib_module_names,
+    }
```

### Comparing `wxc-7.1.1/src/wxc/cli.py` & `wxc-7.1.2/src/wxc/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,28 +120,28 @@
             msg += f" {args.name!r} is a C-compiled function."
         print_err(msg)
         return 1
 
     if args.full:
         from rich import print
 
-        data["name"] = args.name
-        ver = f"version = {data.pop('version', 'unknown')}"
-        print("\n".join(f"{k} = {v}" for k, v in data.items()))
+        all_data = {**data, "name": args.name}
+        ver = f"version = {all_data['version']}"
+        print("\n".join(f"{k} = {v}" for k, v in all_data.items()))
         builtin_print(ver)
         return 0
 
     if args.version:
         if not data["version"]:
             print_err(f"did not find version metadata for {args.name!r}")
             return 1
         builtin_print(data["version"])
         return 0
 
-    if "source" not in data:
+    if data["source"] == "":
         print_err(f"did not resolve source file for {args.name!r}")
         return 1
 
     if args.source:
         import inspect
 
         from rich.syntax import Syntax
```

### Comparing `wxc-7.1.1/src/wxc/levenshtein.py` & `wxc-7.1.2/src/wxc/levenshtein.py`

 * *Files identical despite different names*

### Comparing `wxc-7.1.1/src/wxc.egg-info/PKG-INFO` & `wxc-7.1.2/src/wxc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxc
-Version: 7.1.1
+Version: 7.1.2
 Summary: A CLI facility to inspect Python environments.
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/wxc
 Project-URL: Changelog, https://github.com/neutrinoceros/wxc/blob/main/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -18,15 +18,14 @@
 
 # wxc
 
 [![PyPI](https://img.shields.io/pypi/v/wxc.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/wxc/)
 [![](https://img.shields.io/badge/contributions-welcome-brightgreen)](https://github.com/neutrinoceros/wxc/pulls)
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/wxc/main.svg)](https://results.pre-commit.ci/latest/github/neutrinoceros/wxc/main)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 
 `wxc` (pronounced "which") allows you to inspect source code in your Python
 environment from the command line. It is based on the `inspect` module from the
 standard library.
```

### Comparing `wxc-7.1.1/tests/test_api.py` & `wxc-7.1.2/tests/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 )
 def test_finder(package_name):
     pytest.importorskip(package_name)
     imp = get_full_data(package_name)
     assert "source" in imp
 
     filename, _, line = imp["source"].partition(":")
+    if filename == "built-in":
+        return
     p = Path(filename)
     assert p.exists()
     if not imp["in_stdlib"]:
         assert package_name in p.parts
 
 
 def test_get_obj():
```

### Comparing `wxc-7.1.1/tests/test_builtin.py` & `wxc-7.1.2/tests/test_builtin.py`

 * *Files identical despite different names*

### Comparing `wxc-7.1.1/tests/test_cli.py` & `wxc-7.1.2/tests/test_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 from importlib import import_module
 from importlib.util import find_spec
 
 import pytest
 
 from wxc.cli import main
 
@@ -22,23 +21,14 @@
         import_module(package_name)
     except ImportError:
         pytest.skip()
 
     ret = main([package_name, "--version"])
 
     out, err = capsys.readouterr()
-
-    if package_name == "math" and sys.platform.startswith("win"):
-        # rich may output an unspecified amount of newlines
-        # that don't actually affect the result visually
-        assert out.strip() == ""
-        assert err == "ERROR failed to locate source data.\n"
-        assert ret != 0
-        return
-
     assert out != "unknown"
     assert err == ""
     assert ret == 0
 
 
 @pytest.mark.parametrize("arg", valid_queries)
 def test_falty_queries(capsys, arg):
@@ -68,18 +58,15 @@
     ret = main(["pathlib.nothing"])
     assert ret != 0
     out, err = capsys.readouterr()
     # rich may output an unspecified amount of newlines
     # that don't actually affect the result visually
     assert out.strip() == ""
 
-    assert err.startswith(
-        "ERROR module 'pathlib' has no attribute 'nothing'."
-        " Here are the closest matches:"
-    )
+    assert err.startswith("ERROR module 'pathlib' has no attribute 'nothing'.")
 
 
 def test_compiled_source(capsys):
     pytest.importorskip("numpy")
     ret = main(["numpy.abs.at"])
     out, err = capsys.readouterr()
     assert (
```

### Comparing `wxc-7.1.1/tests/test_schema.py` & `wxc-7.1.2/tests/test_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """Check for robustness of get_full_data
     with an empty module (in particular, no version data)
     """
     syspath, name = fake_module
     data = get_full_data(name)
     filename, _, _ = data["source"].partition(":")
     assert Path(syspath, name) in Path(filename).parents
-    assert "version" not in data
+    assert data["version"] == "unknown"
 
     template.validate(data)
 
 
 def test_field_member():
     d1 = get_full_data("os.path")
     d2 = get_full_data("os.path.expanduser")
```

### Comparing `wxc-7.1.1/tests/test_stdlib.py` & `wxc-7.1.2/tests/test_stdlib.py`

 * *Files identical despite different names*

