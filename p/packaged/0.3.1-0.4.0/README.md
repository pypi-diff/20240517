# Comparing `tmp/packaged-0.3.1.tar.gz` & `tmp/packaged-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaged-0.3.1.tar", last modified: Tue May 14 12:31:39 2024, max compression
+gzip compressed data, was "packaged-0.4.0.tar", last modified: Fri May 17 13:51:48 2024, max compression
```

## Comparing `packaged-0.3.1.tar` & `packaged-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-14 12:31:39.856349 packaged-0.3.1/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)    18089 2024-05-14 12:10:36.000000 packaged-0.3.1/LICENSE
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     4287 2024-05-14 12:31:39.856269 packaged-0.3.1/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3036 2024-05-14 12:26:43.000000 packaged-0.3.1/README.md
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1342 2024-05-14 12:31:39.856662 packaged-0.3.1/setup.cfg
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-09 19:00:34.000000 packaged-0.3.1/setup.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-14 12:31:39.851889 packaged-0.3.1/src/
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-14 12:31:39.854610 packaged-0.3.1/src/packaged/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3778 2024-05-14 12:13:43.000000 packaged-0.3.1/src/packaged/__init__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.3.1/src/packaged/__main__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2377 2024-05-14 12:08:44.000000 packaged-0.3.1/src/packaged/cli.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1457 2024-05-12 06:38:05.000000 packaged-0.3.1/src/packaged/config.py
--rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    19207 2024-05-14 12:16:01.000000 packaged-0.3.1/src/packaged/makeself-header.sh
--rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    21228 2024-05-13 10:09:30.000000 packaged-0.3.1/src/packaged/makeself.sh
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.3.1/src/packaged/py.typed
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-14 12:31:39.855753 packaged-0.3.1/src/packaged.egg-info/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     4287 2024-05-14 12:31:39.000000 packaged-0.3.1/src/packaged.egg-info/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      426 2024-05-14 12:31:39.000000 packaged-0.3.1/src/packaged.egg-info/SOURCES.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-14 12:31:39.000000 packaged-0.3.1/src/packaged.egg-info/dependency_links.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-14 12:31:39.000000 packaged-0.3.1/src/packaged.egg-info/entry_points.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      105 2024-05-14 12:31:39.000000 packaged-0.3.1/src/packaged.egg-info/requires.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-14 12:31:39.000000 packaged-0.3.1/src/packaged.egg-info/top_level.txt
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-17 13:51:48.150334 packaged-0.4.0/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)    18089 2024-05-14 12:10:36.000000 packaged-0.4.0/LICENSE
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     4540 2024-05-17 13:51:48.150263 packaged-0.4.0/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3289 2024-05-17 13:49:45.000000 packaged-0.4.0/README.md
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1342 2024-05-17 13:51:48.150624 packaged-0.4.0/setup.cfg
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-09 19:00:34.000000 packaged-0.4.0/setup.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-17 13:51:48.145815 packaged-0.4.0/src/
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-17 13:51:48.148715 packaged-0.4.0/src/packaged/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     4221 2024-05-17 13:49:45.000000 packaged-0.4.0/src/packaged/__init__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.4.0/src/packaged/__main__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2555 2024-05-17 13:49:45.000000 packaged-0.4.0/src/packaged/cli.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1536 2024-05-17 13:49:45.000000 packaged-0.4.0/src/packaged/config.py
+-rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    19207 2024-05-14 12:16:01.000000 packaged-0.4.0/src/packaged/makeself-header.sh
+-rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    21228 2024-05-13 10:09:30.000000 packaged-0.4.0/src/packaged/makeself.sh
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.4.0/src/packaged/py.typed
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-17 13:51:48.149761 packaged-0.4.0/src/packaged.egg-info/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     4540 2024-05-17 13:51:48.000000 packaged-0.4.0/src/packaged.egg-info/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      426 2024-05-17 13:51:48.000000 packaged-0.4.0/src/packaged.egg-info/SOURCES.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-17 13:51:48.000000 packaged-0.4.0/src/packaged.egg-info/dependency_links.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-17 13:51:48.000000 packaged-0.4.0/src/packaged.egg-info/entry_points.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      105 2024-05-17 13:51:48.000000 packaged-0.4.0/src/packaged.egg-info/requires.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-17 13:51:48.000000 packaged-0.4.0/src/packaged.egg-info/top_level.txt
```

### Comparing `packaged-0.3.1/LICENSE` & `packaged-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `packaged-0.3.1/PKG-INFO` & `packaged-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaged
-Version: 0.3.1
+Version: 0.4.0
 Summary: The easiest way to ship python applications.
 Home-page: https://github.com/tusharsadhwani/packaged
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: GPL-2.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -30,14 +30,19 @@
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 
 # packaged
 
 The easiest way to ship python applications.
 
+![Demo](https://github.com/tusharsadhwani/packaged/blob/main/demo.jpg)
+
+`packaged` can take any Python project, and package it into a self contained
+executable, that can run on other machines without needing Python installed.
+
 ## Installation
 
 ```bash
 pip install packaged
 ```
 
 ## Usage
@@ -62,15 +67,15 @@
 
 ```bash
 packaged ./curve.bin 'pip install -r requirements.txt' 'python bubble_sort_curve.py' ./example/matplotlib
 ```
 
 This produces a `./curve.bin` binary with:
 
-- Python 3.11
+- Python 3.12
 - `matplotlib`
 - `numba`
 - `llvmlite`
 - `pillow`
 
 That outputs an interactive graph GUI.
 
@@ -79,40 +84,40 @@
 You can use a `packaged.toml` file and simply do `packaged path/to/project` to
 create your package. For example, try the `minesweeper` project:
 
 ```bash
 packaged ./example/minesweeper
 ```
 
-[This configuration](tests/end_to_end/test_packages/minesweeper/packaged.toml)
+[This configuration](https://github.com/tusharsadhwani/packaged/blob/main/example/minesweeper/packaged.toml)
 is used for building the package. The equivalent command to build the project
 without `pyproject.toml` would be:
 
 ```bash
 packaged minesweeper.bin 'pip install .' 'python -m minesweeper' ./example/minesweeper
 ```
 
 ### Textual Demo
 
 Since the dependencies themselves contain all the source code needed, you can
 skip the last argument. With this, no other files will be packaged other than
 what is produced in the build step.
 
 ```bash
-packaged './textualdemo.bin' 'pip install textual' 'python -m textual'
+packaged ./textualdemo.bin 'pip install textual' 'python -m textual'
 ```
 
 This will simply package the `textual` library's own demo into a single file.
 
 ### Aliens (pygame)
 
 Pygame ships with various games as well, `pygame.examples.aliens` is one of them:
 
 ```bash
-packaged './aliens' 'pip install pygame' 'python -m pygame.examples.aliens'
+packaged ./aliens 'pip install pygame' 'python -m pygame.examples.aliens'
 ```
 
 Another one that you can try out is `pygame.examples.chimp`.
 
 ## Local Development / Testing
 
 To test and modify the package locally:
```

### Comparing `packaged-0.3.1/README.md` & `packaged-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # packaged
 
 The easiest way to ship python applications.
 
+![Demo](https://github.com/tusharsadhwani/packaged/blob/main/demo.jpg)
+
+`packaged` can take any Python project, and package it into a self contained
+executable, that can run on other machines without needing Python installed.
+
 ## Installation
 
 ```bash
 pip install packaged
 ```
 
 ## Usage
@@ -30,15 +35,15 @@
 
 ```bash
 packaged ./curve.bin 'pip install -r requirements.txt' 'python bubble_sort_curve.py' ./example/matplotlib
 ```
 
 This produces a `./curve.bin` binary with:
 
-- Python 3.11
+- Python 3.12
 - `matplotlib`
 - `numba`
 - `llvmlite`
 - `pillow`
 
 That outputs an interactive graph GUI.
 
@@ -47,40 +52,40 @@
 You can use a `packaged.toml` file and simply do `packaged path/to/project` to
 create your package. For example, try the `minesweeper` project:
 
 ```bash
 packaged ./example/minesweeper
 ```
 
-[This configuration](tests/end_to_end/test_packages/minesweeper/packaged.toml)
+[This configuration](https://github.com/tusharsadhwani/packaged/blob/main/example/minesweeper/packaged.toml)
 is used for building the package. The equivalent command to build the project
 without `pyproject.toml` would be:
 
 ```bash
 packaged minesweeper.bin 'pip install .' 'python -m minesweeper' ./example/minesweeper
 ```
 
 ### Textual Demo
 
 Since the dependencies themselves contain all the source code needed, you can
 skip the last argument. With this, no other files will be packaged other than
 what is produced in the build step.
 
 ```bash
-packaged './textualdemo.bin' 'pip install textual' 'python -m textual'
+packaged ./textualdemo.bin 'pip install textual' 'python -m textual'
 ```
 
 This will simply package the `textual` library's own demo into a single file.
 
 ### Aliens (pygame)
 
 Pygame ships with various games as well, `pygame.examples.aliens` is one of them:
 
 ```bash
-packaged './aliens' 'pip install pygame' 'python -m pygame.examples.aliens'
+packaged ./aliens 'pip install pygame' 'python -m pygame.examples.aliens'
 ```
 
 Another one that you can try out is `pygame.examples.chimp`.
 
 ## Local Development / Testing
 
 To test and modify the package locally:
```

### Comparing `packaged-0.3.1/setup.cfg` & `packaged-0.4.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = packaged
-version = 0.3.1
+version = 0.4.0
 description = The easiest way to ship python applications.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tusharsadhwani/packaged
 author = Tushar Sadhwani
 author_email = tushar.sadhwani000@gmail.com
 license = GPL-2.0-or-later
```

### Comparing `packaged-0.3.1/src/packaged/__init__.py` & `packaged-0.4.0/src/packaged/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,33 +3,43 @@
 from __future__ import annotations
 
 import os.path
 import shutil
 import subprocess
 import tempfile
 
-import yen
+import yen.github
 
 
 MAKESELF_PATH = os.path.join(os.path.dirname(__file__), "makeself.sh")
+DEFAULT_PYTHON_VERSION = "3.12"
 
 
 class SourceDirectoryNotFound(Exception):
     """Raised when provided directory to package does not exist."""
 
     def __init__(self, directory_path: str) -> None:
         super().__init__(directory_path)
         self.directory_path = directory_path
 
 
+class PythonNotAvailable(Exception):
+    """Raised when the Python version asked for is not available for download."""
+
+    def __init__(self, python_version: str) -> None:
+        super().__init__(python_version)
+        self.python_version = python_version
+
+
 def create_package(
     source_directory: str | None,
     output_path: str,
     build_command: str,
     startup_command: str,
+    python_version: str,
 ) -> None:
     """Create the makeself executable, with the startup script in it."""
     if source_directory is None:
         source_directory = tempfile.mkdtemp()
 
     if not os.path.isdir(source_directory):
         raise SourceDirectoryNotFound(source_directory)
@@ -39,15 +49,15 @@
 
     packaged_python_path = os.path.join(source_directory, ".packaged_python")
     if os.path.exists(packaged_python_path):
         shutil.rmtree(packaged_python_path)
 
     try:
         # Use `yen` to ensure a portable Python is present on the system
-        python_version, yen_python_bin_path = ensure_python()
+        python_version, yen_python_bin_path = ensure_python(python_version)
         yen_python_path = os.path.join(yen.PYTHON_INSTALLS_PATH, python_version)
         yen_python_bin_relpath = os.path.relpath(yen_python_bin_path, yen_python_path)
 
         # Put a standalone python interpreter inside the package
         shutil.copytree(yen_python_path, packaged_python_path)
 
         # Get the `python/bin` folder path relative to source directory
@@ -94,13 +104,16 @@
         # Cleanup the packaged python and startup script from source directory
         if os.path.exists(startup_script_path):
             os.remove(startup_script_path)
         if os.path.exists(packaged_python_path):
             shutil.rmtree(packaged_python_path)
 
 
-def ensure_python() -> tuple[str, str]:
+def ensure_python(version: str) -> tuple[str, str]:
     """
     Checks that the version of Python we want to use is available on the
     system, and if not, downloads it.
     """
-    return yen.ensure_python("3.11")
+    try:
+        return yen.ensure_python(version)
+    except yen.github.NotAvailable:
+        raise PythonNotAvailable(version)
```

### Comparing `packaged-0.3.1/src/packaged/cli.py` & `packaged-0.4.0/src/packaged/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 """CLI interface for packaged."""
 
 from __future__ import annotations
 
 import argparse
+import dataclasses
 import os.path
 import platform
 import sys
+import typing
 
-from packaged import SourceDirectoryNotFound, create_package
+from packaged import (
+    DEFAULT_PYTHON_VERSION,
+    PythonNotAvailable,
+    SourceDirectoryNotFound,
+    create_package,
+)
 from packaged.config import (
     Config,
     ConfigValidationError,
     config_file_exists,
     parse_config,
 )
 
@@ -36,21 +43,14 @@
         # Use values from config file instead
         try:
             config = parse_config(argv[0])
         except ConfigValidationError as exc:
             error(f"Expected key {exc.key!r} in config")
             return 3
 
-        source_directory, output_path, build_command, startup_command = (
-            config.source_directory,
-            config.output_path,
-            config.build_command,
-            config.startup_command,
-        )
-
     else:
         parser = argparse.ArgumentParser()
         parser.add_argument("output_path", help="Filename for the generated binary")
         parser.add_argument(
             "build_command", help="Python command to run when building the package"
         )
         parser.add_argument(
@@ -59,22 +59,32 @@
         parser.add_argument(
             "source_directory",
             help="Folder containing your python source to package",
             type=os.path.abspath,
             nargs="?",
             default=None,
         )
-        args = parser.parse_args(argv, namespace=Config)
-
-        source_directory, output_path, build_command, startup_command = (
-            args.source_directory,
-            args.output_path,
-            args.build_command,
-            args.startup_command,
+        parser.add_argument(
+            "--python-version",
+            metavar=DEFAULT_PYTHON_VERSION,
+            help="Version of Python to package your project with.",
+            default=DEFAULT_PYTHON_VERSION,
         )
+        args = parser.parse_args(argv)
+        config = Config(**vars(args))
 
     try:
-        create_package(source_directory, output_path, build_command, startup_command)
+        create_package(
+            config.source_directory,
+            config.output_path,
+            config.build_command,
+            config.startup_command,
+            config.python_version,
+        )
     except SourceDirectoryNotFound as exc:
         error(f"Folder {exc.directory_path!r} does not exist.")
+        return 4
+    except PythonNotAvailable as exc:
+        error(f"Python {exc.python_version!r} is not available for download.")
+        return 5
 
     return 0
```

### Comparing `packaged-0.3.1/src/packaged/config.py` & `packaged-0.4.0/src/packaged/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 @dataclass
 class Config:
     source_directory: str | None
     output_path: str
     build_command: str
     startup_command: str
+    python_version: str
 
 
 CONFIG_NAME = "./packaged.toml"
 
 
 def config_file_exists(source_directory: str) -> bool:
     """Returns true if `packaged.toml` exists in current directory."""
@@ -48,13 +49,14 @@
 
     try:
         config = Config(
             os.path.abspath(source_directory),
             config_data["output_path"],
             config_data["build_command"],
             config_data["startup_command"],
+            config_data.get("python_version", "3.12"),
         )
     except KeyError as exc:
         key = exc.args[0]
         raise ConfigValidationError(key)
 
     return config
```

### Comparing `packaged-0.3.1/src/packaged/makeself-header.sh` & `packaged-0.4.0/src/packaged/makeself-header.sh`

 * *Files identical despite different names*

### Comparing `packaged-0.3.1/src/packaged/makeself.sh` & `packaged-0.4.0/src/packaged/makeself.sh`

 * *Files identical despite different names*

### Comparing `packaged-0.3.1/src/packaged.egg-info/PKG-INFO` & `packaged-0.4.0/src/packaged.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaged
-Version: 0.3.1
+Version: 0.4.0
 Summary: The easiest way to ship python applications.
 Home-page: https://github.com/tusharsadhwani/packaged
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: GPL-2.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -30,14 +30,19 @@
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 
 # packaged
 
 The easiest way to ship python applications.
 
+![Demo](https://github.com/tusharsadhwani/packaged/blob/main/demo.jpg)
+
+`packaged` can take any Python project, and package it into a self contained
+executable, that can run on other machines without needing Python installed.
+
 ## Installation
 
 ```bash
 pip install packaged
 ```
 
 ## Usage
@@ -62,15 +67,15 @@
 
 ```bash
 packaged ./curve.bin 'pip install -r requirements.txt' 'python bubble_sort_curve.py' ./example/matplotlib
 ```
 
 This produces a `./curve.bin` binary with:
 
-- Python 3.11
+- Python 3.12
 - `matplotlib`
 - `numba`
 - `llvmlite`
 - `pillow`
 
 That outputs an interactive graph GUI.
 
@@ -79,40 +84,40 @@
 You can use a `packaged.toml` file and simply do `packaged path/to/project` to
 create your package. For example, try the `minesweeper` project:
 
 ```bash
 packaged ./example/minesweeper
 ```
 
-[This configuration](tests/end_to_end/test_packages/minesweeper/packaged.toml)
+[This configuration](https://github.com/tusharsadhwani/packaged/blob/main/example/minesweeper/packaged.toml)
 is used for building the package. The equivalent command to build the project
 without `pyproject.toml` would be:
 
 ```bash
 packaged minesweeper.bin 'pip install .' 'python -m minesweeper' ./example/minesweeper
 ```
 
 ### Textual Demo
 
 Since the dependencies themselves contain all the source code needed, you can
 skip the last argument. With this, no other files will be packaged other than
 what is produced in the build step.
 
 ```bash
-packaged './textualdemo.bin' 'pip install textual' 'python -m textual'
+packaged ./textualdemo.bin 'pip install textual' 'python -m textual'
 ```
 
 This will simply package the `textual` library's own demo into a single file.
 
 ### Aliens (pygame)
 
 Pygame ships with various games as well, `pygame.examples.aliens` is one of them:
 
 ```bash
-packaged './aliens' 'pip install pygame' 'python -m pygame.examples.aliens'
+packaged ./aliens 'pip install pygame' 'python -m pygame.examples.aliens'
 ```
 
 Another one that you can try out is `pygame.examples.chimp`.
 
 ## Local Development / Testing
 
 To test and modify the package locally:
```

