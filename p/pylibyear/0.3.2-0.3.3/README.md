# Comparing `tmp/pylibyear-0.3.2.tar.gz` & `tmp/pylibyear-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibyear-0.3.2.tar", last modified: Wed May 15 18:18:58 2024, max compression
+gzip compressed data, was "pylibyear-0.3.3.tar", last modified: Fri May 17 18:51:32 2024, max compression
```

## Comparing `pylibyear-0.3.2.tar` & `pylibyear-0.3.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-15 18:18:58.667514 pylibyear-0.3.2/
--rw-r--r--   0 sam        (501) staff       (20)     1067 2024-05-15 17:38:45.000000 pylibyear-0.3.2/LICENSE
--rw-r--r--   0 sam        (501) staff       (20)     6569 2024-05-15 18:18:58.666950 pylibyear-0.3.2/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)     5465 2024-05-15 17:39:03.000000 pylibyear-0.3.2/README.md
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-15 18:18:58.658007 pylibyear-0.3.2/libyear/
--rw-r--r--   0 sam        (501) staff       (20)       22 2024-05-15 18:18:40.000000 pylibyear-0.3.2/libyear/__about__.py
--rw-r--r--   0 sam        (501) staff       (20)        0 2024-05-14 19:54:29.000000 pylibyear-0.3.2/libyear/__init__.py
--rw-r--r--   0 sam        (501) staff       (20)     1783 2024-05-15 18:18:40.000000 pylibyear-0.3.2/libyear/main.py
--rw-r--r--   0 sam        (501) staff       (20)     3194 2024-05-15 17:39:03.000000 pylibyear-0.3.2/libyear/pypi.py
--rw-r--r--   0 sam        (501) staff       (20)      988 2024-05-14 19:54:29.000000 pylibyear-0.3.2/libyear/results.py
--rw-r--r--   0 sam        (501) staff       (20)     2470 2024-05-15 18:05:19.000000 pylibyear-0.3.2/libyear/toml.py
--rw-r--r--   0 sam        (501) staff       (20)     1651 2024-05-14 19:54:29.000000 pylibyear-0.3.2/libyear/utils.py
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-15 18:18:58.666162 pylibyear-0.3.2/pylibyear.egg-info/
--rw-r--r--   0 sam        (501) staff       (20)     6569 2024-05-15 18:18:58.000000 pylibyear-0.3.2/pylibyear.egg-info/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)      418 2024-05-15 18:18:58.000000 pylibyear-0.3.2/pylibyear.egg-info/SOURCES.txt
--rw-r--r--   0 sam        (501) staff       (20)        1 2024-05-15 18:18:58.000000 pylibyear-0.3.2/pylibyear.egg-info/dependency_links.txt
--rw-r--r--   0 sam        (501) staff       (20)       45 2024-05-15 18:18:58.000000 pylibyear-0.3.2/pylibyear.egg-info/entry_points.txt
--rw-r--r--   0 sam        (501) staff       (20)      169 2024-05-15 18:18:58.000000 pylibyear-0.3.2/pylibyear.egg-info/requires.txt
--rw-r--r--   0 sam        (501) staff       (20)        8 2024-05-15 18:18:58.000000 pylibyear-0.3.2/pylibyear.egg-info/top_level.txt
--rw-r--r--   0 sam        (501) staff       (20)     1133 2024-05-15 18:18:40.000000 pylibyear-0.3.2/pyproject.toml
--rw-r--r--   0 sam        (501) staff       (20)       38 2024-05-15 18:18:58.667563 pylibyear-0.3.2/setup.cfg
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-15 18:18:58.665639 pylibyear-0.3.2/tests/
--rw-r--r--   0 sam        (501) staff       (20)     4149 2024-05-14 19:54:29.000000 pylibyear-0.3.2/tests/test_libyear.py
--rw-r--r--   0 sam        (501) staff       (20)     1774 2024-05-14 19:54:29.000000 pylibyear-0.3.2/tests/test_toml.py
--rw-r--r--   0 sam        (501) staff       (20)      590 2024-05-14 19:54:29.000000 pylibyear-0.3.2/tests/test_utils.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-17 18:51:32.056223 pylibyear-0.3.3/
+-rw-r--r--   0 sam        (501) staff       (20)     1067 2024-05-15 17:38:45.000000 pylibyear-0.3.3/LICENSE
+-rw-r--r--   0 sam        (501) staff       (20)     6571 2024-05-17 18:51:32.055713 pylibyear-0.3.3/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)     5467 2024-05-15 18:25:53.000000 pylibyear-0.3.3/README.md
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-17 18:51:32.045553 pylibyear-0.3.3/libyear/
+-rw-r--r--   0 sam        (501) staff       (20)       22 2024-05-17 18:50:15.000000 pylibyear-0.3.3/libyear/__about__.py
+-rw-r--r--   0 sam        (501) staff       (20)        0 2024-05-14 19:54:29.000000 pylibyear-0.3.3/libyear/__init__.py
+-rw-r--r--   0 sam        (501) staff       (20)     2140 2024-05-17 18:42:01.000000 pylibyear-0.3.3/libyear/main.py
+-rw-r--r--   0 sam        (501) staff       (20)     3194 2024-05-15 17:39:03.000000 pylibyear-0.3.3/libyear/pypi.py
+-rw-r--r--   0 sam        (501) staff       (20)     2369 2024-05-17 18:37:22.000000 pylibyear-0.3.3/libyear/results.py
+-rw-r--r--   0 sam        (501) staff       (20)     2470 2024-05-15 18:05:19.000000 pylibyear-0.3.3/libyear/toml.py
+-rw-r--r--   0 sam        (501) staff       (20)     1651 2024-05-14 19:54:29.000000 pylibyear-0.3.3/libyear/utils.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-17 18:51:32.054820 pylibyear-0.3.3/pylibyear.egg-info/
+-rw-r--r--   0 sam        (501) staff       (20)     6571 2024-05-17 18:51:32.000000 pylibyear-0.3.3/pylibyear.egg-info/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)      418 2024-05-17 18:51:32.000000 pylibyear-0.3.3/pylibyear.egg-info/SOURCES.txt
+-rw-r--r--   0 sam        (501) staff       (20)        1 2024-05-17 18:51:32.000000 pylibyear-0.3.3/pylibyear.egg-info/dependency_links.txt
+-rw-r--r--   0 sam        (501) staff       (20)       45 2024-05-17 18:51:32.000000 pylibyear-0.3.3/pylibyear.egg-info/entry_points.txt
+-rw-r--r--   0 sam        (501) staff       (20)      169 2024-05-17 18:51:32.000000 pylibyear-0.3.3/pylibyear.egg-info/requires.txt
+-rw-r--r--   0 sam        (501) staff       (20)        8 2024-05-17 18:51:32.000000 pylibyear-0.3.3/pylibyear.egg-info/top_level.txt
+-rw-r--r--   0 sam        (501) staff       (20)     1133 2024-05-17 18:50:14.000000 pylibyear-0.3.3/pyproject.toml
+-rw-r--r--   0 sam        (501) staff       (20)       38 2024-05-17 18:51:32.056289 pylibyear-0.3.3/setup.cfg
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-17 18:51:32.054067 pylibyear-0.3.3/tests/
+-rw-r--r--   0 sam        (501) staff       (20)     4119 2024-05-17 18:44:10.000000 pylibyear-0.3.3/tests/test_libyear.py
+-rw-r--r--   0 sam        (501) staff       (20)     1774 2024-05-14 19:54:29.000000 pylibyear-0.3.3/tests/test_toml.py
+-rw-r--r--   0 sam        (501) staff       (20)      590 2024-05-14 19:54:29.000000 pylibyear-0.3.3/tests/test_utils.py
```

### Comparing `pylibyear-0.3.2/LICENSE` & `pylibyear-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.2/PKG-INFO` & `pylibyear-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibyear
-Version: 0.3.2
+Version: 0.3.3
 Summary: A simple measure of software dependency freshness.
 Author: nasirhjafri
 Author-email: Sam Atkins <samatkins@outlook.com>
 License: MIT License
 Project-URL: Documentation, https://github.com/sam-atkins/pylibyear#readme
 Project-URL: Issues, https://github.com/sam-atkins/pylibyear/issues
 Project-URL: Source, https://github.com/sam-atkins/pylibyear
@@ -25,15 +25,15 @@
 Requires-Dist: pytest-vcr>=1.0.2; extra == "dev"
 Requires-Dist: ruff>=0.4.4; extra == "dev"
 Provides-Extra: build
 Requires-Dist: build==1.2.1; extra == "build"
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/sam-atkins/pylibyear/)
-[![PyPI version fury.io](https://badge.fury.io/py/libyear.svg)](https://pypi.python.org/pypi/pylibyear/)
+[![PyPI version fury.io](https://badge.fury.io/py/pylibyear.svg)](https://pypi.python.org/pypi/pylibyear/)
 
 **This is a fork of [libyear](https://github.com/nasirhjafri/libyear) as it appears to no longer be maintained.**
 
 # [py]libyear
 
 A **simple** measure of software dependency freshness. It is a **single number** telling you how up-to-date your dependencies are.
```

### Comparing `pylibyear-0.3.2/README.md` & `pylibyear-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/sam-atkins/pylibyear/)
-[![PyPI version fury.io](https://badge.fury.io/py/libyear.svg)](https://pypi.python.org/pypi/pylibyear/)
+[![PyPI version fury.io](https://badge.fury.io/py/pylibyear.svg)](https://pypi.python.org/pypi/pylibyear/)
 
 **This is a fork of [libyear](https://github.com/nasirhjafri/libyear) as it appears to no longer be maintained.**
 
 # [py]libyear
 
 A **simple** measure of software dependency freshness. It is a **single number** telling you how up-to-date your dependencies are.
```

### Comparing `pylibyear-0.3.2/libyear/main.py` & `pylibyear-0.3.3/libyear/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 import typer
 from typing_extensions import Annotated
 
 from libyear.__about__ import __version__
-from libyear.results import print_results_table
+from libyear.results import OutputFormat, calculate_results
 from libyear.toml import load_requirements_from_toml
 from libyear.utils import (
     load_requirements,
 )
 
 app = typer.Typer()
 
@@ -32,40 +32,49 @@
 
 
 @app.command()
 def text(
     requirements_file: Annotated[
         str, typer.Argument(help="requirements.txt file path")
     ],
+    json: Annotated[bool, typer.Option(help="Write the output as JSON")] = False,
     sort: Annotated[
         bool, typer.Option(help="Sort by years behind, in descending order")
     ] = False,
 ):
     """
     The text command reads a requirements.txt file and prints a table with the
     libyear calculations.
     """
     loaded_requirements = load_requirements(requirements_file)
     requirements = set()
     requirements.update(loaded_requirements)
-    print_results_table(requirements, sort)
+    if json:
+        calculate_results(requirements, sort, OutputFormat.JSON)
+    else:
+        calculate_results(requirements, sort)
 
 
 @app.command()
 def toml(
     pyproject: Annotated[str, typer.Argument(help="pyproject.toml path")],
+    json: Annotated[bool, typer.Option(help="Write the output as JSON")] = False,
     sort: Annotated[
         bool, typer.Option(help="Sort by years behind, in descending order")
     ] = False,
 ):
     """
     The toml command reads a pyproject.toml file and prints a table with the
     libyear calculations.
     """
     loaded_requirements = load_requirements_from_toml(pyproject)
     requirements = set()
     requirements.update(loaded_requirements)
-    print_results_table(requirements, sort)
+
+    if json:
+        calculate_results(requirements, sort, OutputFormat.JSON)
+    else:
+        calculate_results(requirements, sort)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `pylibyear-0.3.2/libyear/pypi.py` & `pylibyear-0.3.3/libyear/pypi.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.2/libyear/toml.py` & `pylibyear-0.3.3/libyear/toml.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.2/libyear/utils.py` & `pylibyear-0.3.3/libyear/utils.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.2/pylibyear.egg-info/PKG-INFO` & `pylibyear-0.3.3/pylibyear.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibyear
-Version: 0.3.2
+Version: 0.3.3
 Summary: A simple measure of software dependency freshness.
 Author: nasirhjafri
 Author-email: Sam Atkins <samatkins@outlook.com>
 License: MIT License
 Project-URL: Documentation, https://github.com/sam-atkins/pylibyear#readme
 Project-URL: Issues, https://github.com/sam-atkins/pylibyear/issues
 Project-URL: Source, https://github.com/sam-atkins/pylibyear
@@ -25,15 +25,15 @@
 Requires-Dist: pytest-vcr>=1.0.2; extra == "dev"
 Requires-Dist: ruff>=0.4.4; extra == "dev"
 Provides-Extra: build
 Requires-Dist: build==1.2.1; extra == "build"
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/sam-atkins/pylibyear/)
-[![PyPI version fury.io](https://badge.fury.io/py/libyear.svg)](https://pypi.python.org/pypi/pylibyear/)
+[![PyPI version fury.io](https://badge.fury.io/py/pylibyear.svg)](https://pypi.python.org/pypi/pylibyear/)
 
 **This is a fork of [libyear](https://github.com/nasirhjafri/libyear) as it appears to no longer be maintained.**
 
 # [py]libyear
 
 A **simple** measure of software dependency freshness. It is a **single number** telling you how up-to-date your dependencies are.
```

### Comparing `pylibyear-0.3.2/pyproject.toml` & `pylibyear-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pylibyear"
-version = "0.3.2"
+version = "0.3.3"
 description = "A simple measure of software dependency freshness."
 readme = "README.md"
 requires-python = ">=3.11"
 license = {text = "MIT License"}
 keywords = []
 authors = [
   { name = "Sam Atkins", email = "samatkins@outlook.com" },
```

### Comparing `pylibyear-0.3.2/tests/test_libyear.py` & `pylibyear-0.3.3/tests/test_libyear.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 from pathlib import Path
 
 import pytest
 from typer.testing import CliRunner
 
 from libyear.main import app
 
-# runner = CliRunner()
-
 
 @pytest.fixture(scope="module")
 def vcr_config():
     return {"decode_compressed_response": True}
 
 
 @pytest.fixture(scope="module")
 def vcr_cassette_dir(request):
     # Put all cassettes in tests/cassettes/{module}/{test}.yaml
     return os.path.join("tests/cassettes/", request.module.__name__)
 
 
 @pytest.mark.vcr()
-def test_libyear_main_output(capsys):
+def test_libyear_main_output():
     requirements_path = str(Path(__file__).parent / "data" / "requirements.txt")
     runner = CliRunner()
     result = runner.invoke(
         app,
         [
             "text",
             requirements_path,
```

### Comparing `pylibyear-0.3.2/tests/test_toml.py` & `pylibyear-0.3.3/tests/test_toml.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.2/tests/test_utils.py` & `pylibyear-0.3.3/tests/test_utils.py`

 * *Files identical despite different names*

