# Comparing `tmp/llm_jupyter-0.1.0.tar.gz` & `tmp/llm_jupyter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_jupyter-0.1.0.tar", last modified: Mon May 13 09:56:39 2024, max compression
+gzip compressed data, was "llm_jupyter-0.2.0.tar", last modified: Fri May 17 15:42:34 2024, max compression
```

## Comparing `llm_jupyter-0.1.0.tar` & `llm_jupyter-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:56:39.702075 llm_jupyter-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 09:56:32.000000 llm_jupyter-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-13 09:56:39.702075 llm_jupyter-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-13 09:56:32.000000 llm_jupyter-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:56:39.702075 llm_jupyter-0.1.0/llm_jupyter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-13 09:56:39.000000 llm_jupyter-0.1.0/llm_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-13 09:56:39.000000 llm_jupyter-0.1.0/llm_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:56:39.000000 llm_jupyter-0.1.0/llm_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-13 09:56:39.000000 llm_jupyter-0.1.0/llm_jupyter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-13 09:56:39.000000 llm_jupyter-0.1.0/llm_jupyter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 09:56:39.000000 llm_jupyter-0.1.0/llm_jupyter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-13 09:56:32.000000 llm_jupyter-0.1.0/llm_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-13 09:56:32.000000 llm_jupyter-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:56:39.702075 llm_jupyter-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:56:39.702075 llm_jupyter-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-13 09:56:32.000000 llm_jupyter-0.1.0/tests/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:42:34.943824 llm_jupyter-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 15:42:26.000000 llm_jupyter-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-17 15:42:34.943824 llm_jupyter-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-17 15:42:26.000000 llm_jupyter-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:42:34.943824 llm_jupyter-0.2.0/llm_jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-17 15:42:26.000000 llm_jupyter-0.2.0/llm_jupyter/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-17 15:42:26.000000 llm_jupyter-0.2.0/llm_jupyter/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:42:34.943824 llm_jupyter-0.2.0/llm_jupyter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-17 15:42:34.000000 llm_jupyter-0.2.0/llm_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-17 15:42:34.000000 llm_jupyter-0.2.0/llm_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:42:34.000000 llm_jupyter-0.2.0/llm_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-17 15:42:34.000000 llm_jupyter-0.2.0/llm_jupyter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-17 15:42:34.000000 llm_jupyter-0.2.0/llm_jupyter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 15:42:34.000000 llm_jupyter-0.2.0/llm_jupyter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-17 15:42:26.000000 llm_jupyter-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 15:42:34.943824 llm_jupyter-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:42:34.943824 llm_jupyter-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-17 15:42:26.000000 llm_jupyter-0.2.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-17 15:42:26.000000 llm_jupyter-0.2.0/tests/test_magic_functions.py
```

### Comparing `llm_jupyter-0.1.0/LICENSE` & `llm_jupyter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_jupyter-0.1.0/PKG-INFO` & `llm_jupyter-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-jupyter
-Version: 0.1.0
+Version: 0.2.0
 Summary: Run a IPython interpreter in the LLM virtual environment
 Author: Simon Willison
 Author-email: Lucas Rangel Cezimbra <lucas@cezimbra.tec.br>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/lucasrcezimbra/llm-jupyter
 Project-URL: Changelog, https://github.com/lucasrcezimbra/llm-jupyter/releases
 Project-URL: Issues, https://github.com/lucasrcezimbra/llm-jupyter/issues
@@ -13,28 +13,30 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ipython
 Requires-Dist: jupyter
 Requires-Dist: llm
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
 
 # llm-jupyter
 
 [![PyPI](https://img.shields.io/pypi/v/llm-jupyter.svg)](https://pypi.org/project/llm-jupyter/)
 [![Changelog](https://img.shields.io/github/v/release/lucasrcezimbra/llm-jupyter?include_prereleases&label=changelog)](https://github.com/lucasrcezimbra/llm-jupyter/releases)
 [![Tests](https://github.com/lucasrcezimbra/llm-jupyter/workflows/Test/badge.svg)](https://github.com/lucasrcezimbra/llm-jupyter/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/lucasrcezimbra/llm-jupyter/blob/main/LICENSE)
 
-Run a IPython interpreter in the LLM virtual environment
+Run a IPython interpreter in the [LLM](https://github.com/simonw/llm) virtual environment
 
 ## Installation
 
 Install this plugin in the same environment as [LLM](https://llm.datasette.io/).
 ```bash
+pipx install llm
 llm install llm-jupyter
 ```
 ## Usage
 
 ### IPython
 This plugin adds a new `ipython` command to LLM. This executes IPython in the same virtual environment as LLM itself.
 
@@ -47,31 +49,41 @@
 
 Or to start a IPython shell. In that shell you can import `llm` and use it to interact with models:
 ```bash
 llm ipython
 ```
 
 ```python
-In [1]: !llm 'Who are you?'
-# Output: I am an AI digital assistant here to help you with any questions or tasks you may have. How can I assist you today?
+In [1]: %llm 'Who are you?'
+
+# LLM output will be set as the next input
+In [2]: print("I am a Python programmer using Jupyter Notebook.")
 ```
 
+https://github.com/lucasrcezimbra/llm-jupyter/assets/7042915/b7f8a9ec-d269-4b24-bac3-a01ad6802032
+
 
 ### Notebook
 This plugin also adds a new `notebook` command to LLM. This executes a Jupyter Notebook in the same virtual environment as LLM itself.
 
 ```bash
 llm notebook
 ```
 
 ```python
-!llm 'Who are you?'
-# Output: I am an AI digital assistant here to help you with any questions or tasks you may have. How can I assist you today?
+%load_ext llm_jupyter.magic
+
+%llm 'Who are you?'
+
+# LLM output will be set as the next input
+print("I am a Python programmer using Jupyter Notebook.")
 ```
 
+https://github.com/lucasrcezimbra/llm-jupyter/assets/7042915/58c63b2e-3a7b-43f1-b0aa-ab3daf2e9810
+
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 git clone git@github.com:lucasrcezimbra/llm-jupyter.git
 cd llm-jupyter
 python -m venv .venv
```

### Comparing `llm_jupyter-0.1.0/README.md` & `llm_jupyter-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # llm-jupyter
 
 [![PyPI](https://img.shields.io/pypi/v/llm-jupyter.svg)](https://pypi.org/project/llm-jupyter/)
 [![Changelog](https://img.shields.io/github/v/release/lucasrcezimbra/llm-jupyter?include_prereleases&label=changelog)](https://github.com/lucasrcezimbra/llm-jupyter/releases)
 [![Tests](https://github.com/lucasrcezimbra/llm-jupyter/workflows/Test/badge.svg)](https://github.com/lucasrcezimbra/llm-jupyter/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/lucasrcezimbra/llm-jupyter/blob/main/LICENSE)
 
-Run a IPython interpreter in the LLM virtual environment
+Run a IPython interpreter in the [LLM](https://github.com/simonw/llm) virtual environment
 
 ## Installation
 
 Install this plugin in the same environment as [LLM](https://llm.datasette.io/).
 ```bash
+pipx install llm
 llm install llm-jupyter
 ```
 ## Usage
 
 ### IPython
 This plugin adds a new `ipython` command to LLM. This executes IPython in the same virtual environment as LLM itself.
 
@@ -27,31 +28,41 @@
 
 Or to start a IPython shell. In that shell you can import `llm` and use it to interact with models:
 ```bash
 llm ipython
 ```
 
 ```python
-In [1]: !llm 'Who are you?'
-# Output: I am an AI digital assistant here to help you with any questions or tasks you may have. How can I assist you today?
+In [1]: %llm 'Who are you?'
+
+# LLM output will be set as the next input
+In [2]: print("I am a Python programmer using Jupyter Notebook.")
 ```
 
+https://github.com/lucasrcezimbra/llm-jupyter/assets/7042915/b7f8a9ec-d269-4b24-bac3-a01ad6802032
+
 
 ### Notebook
 This plugin also adds a new `notebook` command to LLM. This executes a Jupyter Notebook in the same virtual environment as LLM itself.
 
 ```bash
 llm notebook
 ```
 
 ```python
-!llm 'Who are you?'
-# Output: I am an AI digital assistant here to help you with any questions or tasks you may have. How can I assist you today?
+%load_ext llm_jupyter.magic
+
+%llm 'Who are you?'
+
+# LLM output will be set as the next input
+print("I am a Python programmer using Jupyter Notebook.")
 ```
 
+https://github.com/lucasrcezimbra/llm-jupyter/assets/7042915/58c63b2e-3a7b-43f1-b0aa-ab3daf2e9810
+
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 git clone git@github.com:lucasrcezimbra/llm-jupyter.git
 cd llm-jupyter
 python -m venv .venv
```

### Comparing `llm_jupyter-0.1.0/llm_jupyter.egg-info/PKG-INFO` & `llm_jupyter-0.2.0/llm_jupyter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-jupyter
-Version: 0.1.0
+Version: 0.2.0
 Summary: Run a IPython interpreter in the LLM virtual environment
 Author: Simon Willison
 Author-email: Lucas Rangel Cezimbra <lucas@cezimbra.tec.br>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/lucasrcezimbra/llm-jupyter
 Project-URL: Changelog, https://github.com/lucasrcezimbra/llm-jupyter/releases
 Project-URL: Issues, https://github.com/lucasrcezimbra/llm-jupyter/issues
@@ -13,28 +13,30 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ipython
 Requires-Dist: jupyter
 Requires-Dist: llm
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
 
 # llm-jupyter
 
 [![PyPI](https://img.shields.io/pypi/v/llm-jupyter.svg)](https://pypi.org/project/llm-jupyter/)
 [![Changelog](https://img.shields.io/github/v/release/lucasrcezimbra/llm-jupyter?include_prereleases&label=changelog)](https://github.com/lucasrcezimbra/llm-jupyter/releases)
 [![Tests](https://github.com/lucasrcezimbra/llm-jupyter/workflows/Test/badge.svg)](https://github.com/lucasrcezimbra/llm-jupyter/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/lucasrcezimbra/llm-jupyter/blob/main/LICENSE)
 
-Run a IPython interpreter in the LLM virtual environment
+Run a IPython interpreter in the [LLM](https://github.com/simonw/llm) virtual environment
 
 ## Installation
 
 Install this plugin in the same environment as [LLM](https://llm.datasette.io/).
 ```bash
+pipx install llm
 llm install llm-jupyter
 ```
 ## Usage
 
 ### IPython
 This plugin adds a new `ipython` command to LLM. This executes IPython in the same virtual environment as LLM itself.
 
@@ -47,31 +49,41 @@
 
 Or to start a IPython shell. In that shell you can import `llm` and use it to interact with models:
 ```bash
 llm ipython
 ```
 
 ```python
-In [1]: !llm 'Who are you?'
-# Output: I am an AI digital assistant here to help you with any questions or tasks you may have. How can I assist you today?
+In [1]: %llm 'Who are you?'
+
+# LLM output will be set as the next input
+In [2]: print("I am a Python programmer using Jupyter Notebook.")
 ```
 
+https://github.com/lucasrcezimbra/llm-jupyter/assets/7042915/b7f8a9ec-d269-4b24-bac3-a01ad6802032
+
 
 ### Notebook
 This plugin also adds a new `notebook` command to LLM. This executes a Jupyter Notebook in the same virtual environment as LLM itself.
 
 ```bash
 llm notebook
 ```
 
 ```python
-!llm 'Who are you?'
-# Output: I am an AI digital assistant here to help you with any questions or tasks you may have. How can I assist you today?
+%load_ext llm_jupyter.magic
+
+%llm 'Who are you?'
+
+# LLM output will be set as the next input
+print("I am a Python programmer using Jupyter Notebook.")
 ```
 
+https://github.com/lucasrcezimbra/llm-jupyter/assets/7042915/58c63b2e-3a7b-43f1-b0aa-ab3daf2e9810
+
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 git clone git@github.com:lucasrcezimbra/llm-jupyter.git
 cd llm-jupyter
 python -m venv .venv
```

### Comparing `llm_jupyter-0.1.0/pyproject.toml` & `llm_jupyter-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-jupyter"
-version = "0.1.0"
+version = "0.2.0"
 description = "Run a IPython interpreter in the LLM virtual environment"
 readme = "README.md"
 authors = [
   {name = "Lucas Rangel Cezimbra", email="lucas@cezimbra.tec.br"},
   {name = "Simon Willison"},
 ]
 license = {text = "Apache-2.0"}
@@ -20,11 +20,17 @@
 [project.urls]
 Homepage = "https://github.com/lucasrcezimbra/llm-jupyter"
 Changelog = "https://github.com/lucasrcezimbra/llm-jupyter/releases"
 Issues = "https://github.com/lucasrcezimbra/llm-jupyter/issues"
 CI = "https://github.com/lucasrcezimbra/llm-jupyter/actions"
 
 [project.entry-points.llm]
-python = "llm_jupyter"
+ipython = "llm_jupyter.commands"
 
 [project.optional-dependencies]
-test = ["pytest"]
+test = ["pytest", "pytest-mock"]
+
+
+[tool.ruff]
+select = ["A", "B", "BLE", "E", "F", "I", "RUF", "SIM", "W"]
+ignore = ["E501"]
+line-length = 88
```

### Comparing `llm_jupyter-0.1.0/tests/test_commands.py` & `llm_jupyter-0.2.0/tests/test_commands.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from llm.cli import cli
+import re
+
 from click.testing import CliRunner
+from llm.cli import cli
 
 
 def test_ipython_execute(tmpdir):
     runner = CliRunner()
 
     # tmpdir should be empty
     assert len(tmpdir.listdir()) == 0
@@ -24,14 +26,26 @@
 
     runner.invoke(cli, ["ipython", "help"])
 
     captured = capfd.readouterr()
     assert captured.out.startswith("=========\n IPython\n========")
 
 
+def test_ipython_auto_load_extension(capfd):
+    runner = CliRunner()
+
+    runner.invoke(cli, ["ipython", "-c", "%llm --help"])
+
+    captured = capfd.readouterr()
+    assert re.match(
+        r"^usage: .* \[-h\] \[--print\] \[--model MODEL\] \[--system SYSTEM\]",
+        captured.out,
+    )
+
+
 def test_jupyter(capfd):
     runner = CliRunner()
 
     runner.invoke(cli, ["notebook", "--help-all"])
 
     captured = capfd.readouterr()
     assert captured.out.startswith(
```

