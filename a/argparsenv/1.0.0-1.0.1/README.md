# Comparing `tmp/argparsenv-1.0.0.tar.gz` & `tmp/argparsenv-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparsenv-1.0.0.tar", max compression
+gzip compressed data, was "argparsenv-1.0.1.tar", max compression
```

## Comparing `argparsenv-1.0.0.tar` & `argparsenv-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2024-05-14 09:01:37.639314 argparsenv-1.0.0/LICENSE
--rw-r--r--   0        0        0     1859 2024-05-14 09:01:37.639314 argparsenv-1.0.0/README.md
--rw-r--r--   0        0        0      142 2024-05-14 09:01:37.639314 argparsenv-1.0.0/argparsenv/__init__.py
--rw-r--r--   0        0        0     3272 2024-05-14 09:01:37.639314 argparsenv-1.0.0/argparsenv/argparsenv.py
--rw-r--r--   0        0        0      526 2024-05-14 09:01:37.639314 argparsenv-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2397 1970-01-01 00:00:00.000000 argparsenv-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-17 19:49:29.016646 argparsenv-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1889 2024-05-17 19:49:29.016646 argparsenv-1.0.1/README.md
+-rw-r--r--   0        0        0      142 2024-05-17 19:49:29.016646 argparsenv-1.0.1/argparsenv/__init__.py
+-rw-r--r--   0        0        0     3272 2024-05-17 19:49:29.016646 argparsenv-1.0.1/argparsenv/argparsenv.py
+-rw-r--r--   0        0        0     1099 2024-05-17 19:49:29.016646 argparsenv-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 argparsenv-1.0.1/PKG-INFO
```

### Comparing `argparsenv-1.0.0/LICENSE` & `argparsenv-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argparsenv-1.0.0/README.md` & `argparsenv-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 ## Usage
 
 This module builds on top of python's standard library
 [argparse](https://docs.python.org/3/library/argparse.html).
 
 ```python
+import argparsenv
+
 env_arg_parser = ArgumentParser()
 env_arg_parser.add_argument(
     "--port",
     dest="port",
     env_var="MY_APP_DB_PORT",
     default="3306",
 )
@@ -65,11 +67,12 @@
 For feature requests, bug reports or questions, please open an issue.
 For code contributions, please open a pull request.
 
 Please make sure to install `pre-commit` before making changes to the code (this enables
 checks for code formatting, linting, etc. before committing changes):
 
 ```bash
-pip install pre-commit
+pip install poetry
+poetry install
 cd path/to/argparsenv
 pre-commit install
 ```
```

### Comparing `argparsenv-1.0.0/argparsenv/argparsenv.py` & `argparsenv-1.0.1/argparsenv/argparsenv.py`

 * *Files identical despite different names*

### Comparing `argparsenv-1.0.0/PKG-INFO` & `argparsenv-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 Metadata-Version: 2.1
 Name: argparsenv
-Version: 1.0.0
+Version: 1.0.1
 Summary: Extends python's argparser with environment variables
+Home-page: https://github.com/snaeil/argparsenv
 License: MIT
+Keywords: cli,environment,arguments
 Author: snaeil
 Author-email: schnegel@posteo.de
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Typing :: Typed
 Requires-Dist: overrides (>=7.7.0,<8.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Project-URL: Repository, https://github.com/snaeil/argparsenv
 Description-Content-Type: text/markdown
 
 # argparsenv
 
 This project extends python's argparse module to allow for environment variable overrides of command line arguments.
 
 The rule for environment variable overrides is as follows:
@@ -41,14 +52,16 @@
 
 ## Usage
 
 This module builds on top of python's standard library
 [argparse](https://docs.python.org/3/library/argparse.html).
 
 ```python
+import argparsenv
+
 env_arg_parser = ArgumentParser()
 env_arg_parser.add_argument(
     "--port",
     dest="port",
     env_var="MY_APP_DB_PORT",
     default="3306",
 )
@@ -81,12 +94,13 @@
 For feature requests, bug reports or questions, please open an issue.
 For code contributions, please open a pull request.
 
 Please make sure to install `pre-commit` before making changes to the code (this enables
 checks for code formatting, linting, etc. before committing changes):
 
 ```bash
-pip install pre-commit
+pip install poetry
+poetry install
 cd path/to/argparsenv
 pre-commit install
 ```
```

