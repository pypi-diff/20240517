# Comparing `tmp/python_project_cli-1.0.0.tar.gz` & `tmp/python_project_cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_project_cli-1.0.0.tar", max compression
+gzip compressed data, was "python_project_cli-1.1.0.tar", max compression
```

## Comparing `python_project_cli-1.0.0.tar` & `python_project_cli-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2024-05-15 15:39:57.549871 python_project_cli-1.0.0/LICENSE
--rw-r--r--   0        0        0     1328 2024-05-15 15:39:57.549871 python_project_cli-1.0.0/README.md
--rw-r--r--   0        0        0     2455 2024-05-15 15:39:58.405874 python_project_cli-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-15 15:39:57.553871 python_project_cli-1.0.0/src/python_project_cli/__init__.py
--rw-r--r--   0        0        0     1858 2024-05-15 15:39:58.405874 python_project_cli-1.0.0/src/python_project_cli/main.py
--rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 python_project_cli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-17 17:21:46.831250 python_project_cli-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1557 2024-05-17 17:21:46.831250 python_project_cli-1.1.0/README.md
+-rw-r--r--   0        0        0     2387 2024-05-17 17:21:47.899263 python_project_cli-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 17:21:46.831250 python_project_cli-1.1.0/src/python_project_cli/__init__.py
+-rw-r--r--   0        0        0     1858 2024-05-17 17:21:47.899263 python_project_cli-1.1.0/src/python_project_cli/main.py
+-rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 python_project_cli-1.1.0/PKG-INFO
```

### Comparing `python_project_cli-1.0.0/LICENSE` & `python_project_cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_project_cli-1.0.0/README.md` & `python_project_cli-1.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -6,28 +6,39 @@
 ![Deploy](https://github.com/MentorMate/python-project-cli/actions/workflows/main_release.yaml/badge.svg)
 
 ## Overview
 This is a python-cli tool for interactive project setup, following best practices for **Django** and **FastAPI**.
 In order to assure easier distribution, the project is deployed as **pypi** package.
 For optimal maintenance the project utilizes the **tox** framework.
 
-## Installation
-We use `pip` for our package distribution, that's why we recomend that you use virtual environment for the package instalation (`venv` or `poetr`).
+# Installation
+We use `pip` for our package distribution, that's why we recommend that you use a virtual environment for the package installation (`venv` or `poetry`).
 ```bash
-(env) pip install python-project-cli
+pip install python-project-cli
 ```
 
 ## Commands
-- `python-cli generate` - starts interactive project generation, that uses cookiecutter.
-- `python-cli status` - shows the framework repo status. We aim to update the main templates frequently, in order to keep up with the everevolving "best" practices, that's why there's a chance for a repo downtime.
-- `python-cli version` - project version.
+1. **generate**s a new project in interactive mode, usesing `cookiecutter`.
+    ```bash
+    python-cli generate
+    ```
+
+2. Shows the framework repo **status**. We aim to update the main templates frequently, in order to keep up with the everevolving "best" practices, that's why there's a chance for a repo downtime.
+    ```bash
+    python-cli status
+    ```
+
+3. Project's **version**.
+    ```bash
+    python-cli version
+    ```
 
 ### Frameworks
 - Django
 - FastAPI
 
-
+### Project Maintenance (Internal)
+[Confluence link](https://mentormate.atlassian.net/wiki/spaces/MMSDLC/pages/4325900953/Python+CLI+documentation)
 
 ## License
-
 PYTHON-PROJECT-CLI is unlicensed, as found in the
 [LICENSE](https://github.com/MentorMate/python-project-cli/blob/development/LICENSE) file.
```

### Comparing `python_project_cli-1.0.0/pyproject.toml` & `python_project_cli-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python_project_cli"
-version = "1.0.0"
+version = "1.1.0"
 authors = ["alexandermentormate"]
 description = "CLI for building base djang and fastapi based projects"
 readme = "README.md"
 homepage = "https://github.com/MentorMate/python-project-cli/"
 repository = "https://github.com/MentorMate/python-project-cli/"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -28,17 +28,14 @@
 version_toml = ["pyproject.toml:tool.poetry.version"]
 version_variables = [
     "src/python_project_cli/main.py:__version__"
 ]
 upload_to_pypi = true
 build_command = "pip install poetry && poetry build"
 
-[tool.semantic_release.branches.development]
-match = "development"
-
 [tool.semantic_release.branches.main]
 match = "main"
 
 # for development purpose, in order to check for a new potential release
 # when using `semantic-release version`
 [tool.semantic_release.branches.feature]
 match = "feature/*"
```

### Comparing `python_project_cli-1.0.0/src/python_project_cli/main.py` & `python_project_cli-1.1.0/src/python_project_cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from subprocess import run
 from rich.console import Console
 from rich.table import Table
 from rich import print
 import typer
 from typing_extensions import Annotated
 
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 
 app = typer.Typer(add_completion=False)
 console = Console()
 
 
 class Frameworks(StrEnum):
     django = 'Django'
```

### Comparing `python_project_cli-1.0.0/PKG-INFO` & `python_project_cli-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_project_cli
-Version: 1.0.0
+Version: 1.1.0
 Summary: CLI for building base djang and fastapi based projects
 Home-page: https://github.com/MentorMate/python-project-cli/
 Author: alexandermentormate
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -24,29 +24,40 @@
 ![Deploy](https://github.com/MentorMate/python-project-cli/actions/workflows/main_release.yaml/badge.svg)
 
 ## Overview
 This is a python-cli tool for interactive project setup, following best practices for **Django** and **FastAPI**.
 In order to assure easier distribution, the project is deployed as **pypi** package.
 For optimal maintenance the project utilizes the **tox** framework.
 
-## Installation
-We use `pip` for our package distribution, that's why we recomend that you use virtual environment for the package instalation (`venv` or `poetr`).
+# Installation
+We use `pip` for our package distribution, that's why we recommend that you use a virtual environment for the package installation (`venv` or `poetry`).
 ```bash
-(env) pip install python-project-cli
+pip install python-project-cli
 ```
 
 ## Commands
-- `python-cli generate` - starts interactive project generation, that uses cookiecutter.
-- `python-cli status` - shows the framework repo status. We aim to update the main templates frequently, in order to keep up with the everevolving "best" practices, that's why there's a chance for a repo downtime.
-- `python-cli version` - project version.
+1. **generate**s a new project in interactive mode, usesing `cookiecutter`.
+    ```bash
+    python-cli generate
+    ```
+
+2. Shows the framework repo **status**. We aim to update the main templates frequently, in order to keep up with the everevolving "best" practices, that's why there's a chance for a repo downtime.
+    ```bash
+    python-cli status
+    ```
+
+3. Project's **version**.
+    ```bash
+    python-cli version
+    ```
 
 ### Frameworks
 - Django
 - FastAPI
 
-
+### Project Maintenance (Internal)
+[Confluence link](https://mentormate.atlassian.net/wiki/spaces/MMSDLC/pages/4325900953/Python+CLI+documentation)
 
 ## License
-
 PYTHON-PROJECT-CLI is unlicensed, as found in the
 [LICENSE](https://github.com/MentorMate/python-project-cli/blob/development/LICENSE) file.
```

