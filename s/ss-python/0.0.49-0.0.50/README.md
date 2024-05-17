# Comparing `tmp/ss_python-0.0.49.tar.gz` & `tmp/ss_python-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ss_python-0.0.49.tar", last modified: Sun Feb 18 10:16:19 2024, max compression
+gzip compressed data, was "ss_python-0.0.50.tar", last modified: Mon Mar 25 06:05:08 2024, max compression
```

## Comparing `ss_python-0.0.49.tar` & `ss_python-0.0.50.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1078 2024-02-18 10:16:02.789392 ss_python-0.0.49/LICENSE
--rw-r--r--   0        0        0     7446 2024-02-18 10:16:02.789392 ss_python-0.0.49/README.md
--rw-r--r--   0        0        0     2601 2024-02-18 10:16:19.945410 ss_python-0.0.49/pyproject.toml
--rw-r--r--   0        0        0       28 2024-02-18 10:16:02.793392 ss_python-0.0.49/src/ss_python/__init__.py
--rw-r--r--   0        0        0      883 2024-02-18 10:16:02.793392 ss_python-0.0.49/src/ss_python/cli.py
--rw-r--r--   0        0        0        0 2024-02-18 10:16:02.793392 ss_python-0.0.49/src/ss_python/py.typed
--rw-r--r--   0        0        0     1054 2024-02-18 10:16:02.793392 ss_python-0.0.49/src/ss_python/settings.py
--rw-r--r--   0        0        0       25 2024-02-18 10:16:02.797392 ss_python-0.0.49/tests/__init__.py
--rw-r--r--   0        0        0      437 2024-02-18 10:16:02.797392 ss_python-0.0.49/tests/cli_test.py
--rw-r--r--   0        0        0      136 2024-02-18 10:16:02.797392 ss_python-0.0.49/tests/pkg_test.py
--rw-r--r--   0        0        0      337 2024-02-18 10:16:02.797392 ss_python-0.0.49/tests/settings_test.py
--rw-r--r--   0        0        0     8487 1970-01-01 00:00:00.000000 ss_python-0.0.49/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-03-25 06:04:52.725015 ss_python-0.0.50/LICENSE
+-rw-r--r--   0        0        0     7974 2024-03-25 06:04:52.729015 ss_python-0.0.50/README.md
+-rw-r--r--   0        0        0     2601 2024-03-25 06:05:08.821105 ss_python-0.0.50/pyproject.toml
+-rw-r--r--   0        0        0       28 2024-03-25 06:04:52.729015 ss_python-0.0.50/src/ss_python/__init__.py
+-rw-r--r--   0        0        0      884 2024-03-25 06:04:52.729015 ss_python-0.0.50/src/ss_python/cli.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:04:52.733015 ss_python-0.0.50/src/ss_python/py.typed
+-rw-r--r--   0        0        0     1055 2024-03-25 06:04:52.733015 ss_python-0.0.50/src/ss_python/settings.py
+-rw-r--r--   0        0        0       25 2024-03-25 06:04:52.733015 ss_python-0.0.50/tests/__init__.py
+-rw-r--r--   0        0        0      438 2024-03-25 06:04:52.733015 ss_python-0.0.50/tests/cli_test.py
+-rw-r--r--   0        0        0      136 2024-03-25 06:04:52.733015 ss_python-0.0.50/tests/pkg_test.py
+-rw-r--r--   0        0        0      338 2024-03-25 06:04:52.737015 ss_python-0.0.50/tests/settings_test.py
+-rw-r--r--   0        0        0     9015 1970-01-01 00:00:00.000000 ss_python-0.0.50/PKG-INFO
```

### Comparing `ss_python-0.0.49/LICENSE` & `ss_python-0.0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `ss_python-0.0.49/README.md` & `ss_python-0.0.50/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Serious Scaffold Python
 
 A Python project template covering the entire development lifecycle with various integrations, configurations and modules.
 
 [![CI](https://github.com/serious-scaffold/ss-python/actions/workflows/ci.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/ci.yml)
-[![Release](https://github.com/serious-scaffold/ss-python/actions/workflows/release.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/release.yml)
-[![DevContainer](https://github.com/serious-scaffold/ss-python/actions/workflows/devcontainer.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/devcontainer.yml)
 [![CommitLint](https://github.com/serious-scaffold/ss-python/actions/workflows/commitlint.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/commitlint.yml)
+[![DevContainer](https://github.com/serious-scaffold/ss-python/actions/workflows/devcontainer.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/devcontainer.yml)
+[![Release](https://github.com/serious-scaffold/ss-python/actions/workflows/release.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/release.yml)
+[![Renovate](https://github.com/serious-scaffold/ss-python/actions/workflows/renovate.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/renovate.yml)
 [![Coverage](https://img.shields.io/endpoint?url=https://serious-scaffold.github.io/ss-python/_static/badges/coverage.json)](https://serious-scaffold.github.io/ss-python/reports/coverage)
 [![PyPI](https://img.shields.io/pypi/v/ss-python)](https://pypi.org/project/ss-python/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ss-python)](https://pypi.org/project/ss-python/)
 [![GitHub](https://img.shields.io/github/license/serious-scaffold/ss-python)](https://github.com/serious-scaffold/ss-python/blob/main/LICENSE)
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
@@ -31,21 +32,23 @@
 If you find this helpful, please consider [sponsorship](https://github.com/sponsors/huxuan).
 
 ## 🛠️ Features
 
 - Project setup and template update with [`copier`](https://copier.readthedocs.io/).
 - Manage dependencies and virtual environments with [`pdm`](https://pdm-project.org/).
 - Version the package using [dynamic SCM tag](https://backend.pdm-project.org/metadata/#read-from-scm-tag-supporting-git-and-hg) with [`pdm-backend`](https://backend.pdm-project.org/).
-- Containerization for development and deployment with [dev container](https://containers.dev/) integration.
+- Containerization for development and deployment with [dev container](https://containers.dev/).
+- Automate dependency updates with [Renovate](https://github.com/renovatebot/renovate).
 - Automate Git hooks with [pre-commit hooks](https://github.com/pre-commit/pre-commit-hooks) and [local](https://pre-commit.com/#repository-local-hooks) linters.
-- Lint with [`mypy`](http://www.mypy-lang.org/), [`ruff`](https://github.com/charliermarsh/ruff), and [`toml-sort`](https://github.com/pappasam/toml-sort).
+- Lint with [`mypy`](http://www.mypy-lang.org/), [`ruff`](https://github.com/charliermarsh/ruff), [`toml-sort`](https://github.com/pappasam/toml-sort) and [`commitlint`](https://commitlint.js.org/).
 - Test with [`pytest`](https://pytest.org/) and [`coverage`](https://coverage.readthedocs.io) for threshold and reports.
-- Document with [`sphinx`](https://www.sphinx-doc.org/), the [`furo`](https://pradyunsg.me/furo) theme, and [mypy](https://mypy.readthedocs.io/en/stable/command_line.html?report-generation)/[coverage](https://coverage.readthedocs.io/en/7.3.0/cmd.html#html-reporting-coverage-html) reports.
+- Documentation with [`sphinx`](https://www.sphinx-doc.org/), the [`furo`](https://pradyunsg.me/furo) theme, and [mypy](https://mypy.readthedocs.io/en/stable/command_line.html?report-generation)/[coverage](https://coverage.readthedocs.io/en/7.3.0/cmd.html#html-reporting-coverage-html) reports.
 - Continuous Integration with [GitHub Actions](https://docs.github.com/actions) and [GitLab CI/CD](https://docs.gitlab.com/ee/ci/).
-- [Versioned documentation](https://docs.readthedocs.io/en/stable/versions.html) with [Read the Docs](https://readthedocs.org/) integration.
+- Latest stable documentation published to [GitHub](https://docs.github.com/en/pages)/[GitLab](https://docs.gitlab.com/ee/user/project/pages/) Pages.
+- [Versioned documentation](https://docs.readthedocs.io/en/stable/versions.html) and [pull request previews](https://docs.readthedocs.io/en/stable/pull-requests.html) with [Read the Docs](https://readthedocs.org/).
 - Develop Command Line Interfaces with [`typer`](https://typer.tiangolo.com/).
 - Manage configurations with [`pydantic-settings`](https://docs.pydantic.dev/latest/usage/pydantic_settings/).
 - Centralize common actions with a unified Makefile.
 - VSCode settings with recommended extensions.
 
 ## 🔧 Prerequisites
```

### Comparing `ss_python-0.0.49/pyproject.toml` & `ss_python-0.0.50/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "full-development-lifecycle",
     "project-template",
     "serious-scaffold",
 ]
 name = "ss-python"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.0.49"
+version = "0.0.50"
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
 ss-python-cli = "ss_python.cli:app"
```

### Comparing `ss_python-0.0.49/src/ss_python/cli.py` & `ss_python-0.0.50/src/ss_python/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Command Line Interface."""
+
 import typer
 
 app = typer.Typer()
 
 
 @app.command()
 def run() -> None:
```

### Comparing `ss_python-0.0.49/src/ss_python/settings.py` & `ss_python-0.0.50/src/ss_python/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Settings Module."""
+
 import logging
 from logging import getLevelName
 from typing import Optional
 
 from pydantic_settings import BaseSettings, SettingsConfigDict
```

### Comparing `ss_python-0.0.49/PKG-INFO` & `ss_python-0.0.50/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ss-python
-Version: 0.0.49
+Version: 0.0.50
 Summary: A Python project template covering the entire development lifecycle with various integrations, configurations and modules.
 Keywords: copier-template full-development-lifecycle project-template serious-scaffold
 Home-page: https://github.com/serious-scaffold/ss-python/
 Author-Email: huxuan <i@huxuan.org>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -22,17 +22,18 @@
 Description-Content-Type: text/markdown
 
 # Serious Scaffold Python
 
 A Python project template covering the entire development lifecycle with various integrations, configurations and modules.
 
 [![CI](https://github.com/serious-scaffold/ss-python/actions/workflows/ci.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/ci.yml)
-[![Release](https://github.com/serious-scaffold/ss-python/actions/workflows/release.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/release.yml)
-[![DevContainer](https://github.com/serious-scaffold/ss-python/actions/workflows/devcontainer.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/devcontainer.yml)
 [![CommitLint](https://github.com/serious-scaffold/ss-python/actions/workflows/commitlint.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/commitlint.yml)
+[![DevContainer](https://github.com/serious-scaffold/ss-python/actions/workflows/devcontainer.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/devcontainer.yml)
+[![Release](https://github.com/serious-scaffold/ss-python/actions/workflows/release.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/release.yml)
+[![Renovate](https://github.com/serious-scaffold/ss-python/actions/workflows/renovate.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/renovate.yml)
 [![Coverage](https://img.shields.io/endpoint?url=https://serious-scaffold.github.io/ss-python/_static/badges/coverage.json)](https://serious-scaffold.github.io/ss-python/reports/coverage)
 [![PyPI](https://img.shields.io/pypi/v/ss-python)](https://pypi.org/project/ss-python/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ss-python)](https://pypi.org/project/ss-python/)
 [![GitHub](https://img.shields.io/github/license/serious-scaffold/ss-python)](https://github.com/serious-scaffold/ss-python/blob/main/LICENSE)
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
@@ -54,21 +55,23 @@
 If you find this helpful, please consider [sponsorship](https://github.com/sponsors/huxuan).
 
 ## 🛠️ Features
 
 - Project setup and template update with [`copier`](https://copier.readthedocs.io/).
 - Manage dependencies and virtual environments with [`pdm`](https://pdm-project.org/).
 - Version the package using [dynamic SCM tag](https://backend.pdm-project.org/metadata/#read-from-scm-tag-supporting-git-and-hg) with [`pdm-backend`](https://backend.pdm-project.org/).
-- Containerization for development and deployment with [dev container](https://containers.dev/) integration.
+- Containerization for development and deployment with [dev container](https://containers.dev/).
+- Automate dependency updates with [Renovate](https://github.com/renovatebot/renovate).
 - Automate Git hooks with [pre-commit hooks](https://github.com/pre-commit/pre-commit-hooks) and [local](https://pre-commit.com/#repository-local-hooks) linters.
-- Lint with [`mypy`](http://www.mypy-lang.org/), [`ruff`](https://github.com/charliermarsh/ruff), and [`toml-sort`](https://github.com/pappasam/toml-sort).
+- Lint with [`mypy`](http://www.mypy-lang.org/), [`ruff`](https://github.com/charliermarsh/ruff), [`toml-sort`](https://github.com/pappasam/toml-sort) and [`commitlint`](https://commitlint.js.org/).
 - Test with [`pytest`](https://pytest.org/) and [`coverage`](https://coverage.readthedocs.io) for threshold and reports.
-- Document with [`sphinx`](https://www.sphinx-doc.org/), the [`furo`](https://pradyunsg.me/furo) theme, and [mypy](https://mypy.readthedocs.io/en/stable/command_line.html?report-generation)/[coverage](https://coverage.readthedocs.io/en/7.3.0/cmd.html#html-reporting-coverage-html) reports.
+- Documentation with [`sphinx`](https://www.sphinx-doc.org/), the [`furo`](https://pradyunsg.me/furo) theme, and [mypy](https://mypy.readthedocs.io/en/stable/command_line.html?report-generation)/[coverage](https://coverage.readthedocs.io/en/7.3.0/cmd.html#html-reporting-coverage-html) reports.
 - Continuous Integration with [GitHub Actions](https://docs.github.com/actions) and [GitLab CI/CD](https://docs.gitlab.com/ee/ci/).
-- [Versioned documentation](https://docs.readthedocs.io/en/stable/versions.html) with [Read the Docs](https://readthedocs.org/) integration.
+- Latest stable documentation published to [GitHub](https://docs.github.com/en/pages)/[GitLab](https://docs.gitlab.com/ee/user/project/pages/) Pages.
+- [Versioned documentation](https://docs.readthedocs.io/en/stable/versions.html) and [pull request previews](https://docs.readthedocs.io/en/stable/pull-requests.html) with [Read the Docs](https://readthedocs.org/).
 - Develop Command Line Interfaces with [`typer`](https://typer.tiangolo.com/).
 - Manage configurations with [`pydantic-settings`](https://docs.pydantic.dev/latest/usage/pydantic_settings/).
 - Centralize common actions with a unified Makefile.
 - VSCode settings with recommended extensions.
 
 ## 🔧 Prerequisites
```

