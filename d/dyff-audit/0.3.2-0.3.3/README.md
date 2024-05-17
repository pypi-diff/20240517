# Comparing `tmp/dyff_audit-0.3.2.tar.gz` & `tmp/dyff_audit-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_audit-0.3.2.tar", last modified: Wed Apr 24 05:55:32 2024, max compression
+gzip compressed data, was "dyff_audit-0.3.3.tar", last modified: Fri May 17 04:20:30 2024, max compression
```

## Comparing `dyff_audit-0.3.2.tar` & `dyff_audit-0.3.3.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.046439 dyff_audit-0.3.2/
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1839 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1800 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3690 2024-04-24 05:55:32.046439 dyff_audit-0.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2309 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.029439 dyff_audit-0.3.2/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.036439 dyff_audit-0.3.2/dyff/audit/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.038439 dyff_audit-0.3.2/dyff/audit/analysis/
--rw-rw-rw-   0 root         (0) root         (0)      296 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/analysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6108 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/analysis/context.py
--rw-rw-rw-   0 root         (0) root         (0)     1689 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/analysis/jupyter.py
--rw-rw-rw-   0 root         (0) root         (0)     1179 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/analysis/legacy.py
--rw-rw-rw-   0 root         (0) root         (0)     2814 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/analysis/python.py
--rw-rw-rw-   0 root         (0) root         (0)     3409 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/analysis/runners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.038439 dyff_audit-0.3.2/dyff/audit/data/
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2368 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/data/text.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/dynamic_import.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.039439 dyff_audit-0.3.2/dyff/audit/local/
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24096 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/local/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.039439 dyff_audit-0.3.2/dyff/audit/metrics/
--rw-rw-rw-   0 root         (0) root         (0)      233 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/metrics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1071 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/metrics/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4359 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/metrics/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.041439 dyff_audit-0.3.2/dyff/audit/scoring/
--rw-rw-rw-   0 root         (0) root         (0)      261 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/scoring/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/scoring/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3949 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/scoring/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1787 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/scoring/example.py
--rw-rw-rw-   0 root         (0) root         (0)    11999 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/scoring/text.py
--rw-rw-rw-   0 root         (0) root         (0)     5994 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/dyff/audit/workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.045439 dyff_audit-0.3.2/dyff_audit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3690 2024-04-24 05:55:32.000000 dyff_audit-0.3.2/dyff_audit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1412 2024-04-24 05:55:32.000000 dyff_audit-0.3.2/dyff_audit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 05:55:32.000000 dyff_audit-0.3.2/dyff_audit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      136 2024-04-24 05:55:32.000000 dyff_audit-0.3.2/dyff_audit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-24 05:55:32.000000 dyff_audit-0.3.2/dyff_audit.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1911 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 05:55:32.046439 dyff_audit-0.3.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.043439 dyff_audit-0.3.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)      193 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.032439 dyff_audit-0.3.2/tests/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.043439 dyff_audit-0.3.2/tests/data/dataset/
--rw-rw-rw-   0 root         (0) root         (0)     1196 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/tests/data/dataset/part-0.parquet
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.043439 dyff_audit-0.3.2/tests/data/evaluation/
--rw-rw-rw-   0 root         (0) root         (0)     2990 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/tests/data/evaluation/part-0.parquet
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.044438 dyff_audit-0.3.2/tests/data/module_jupyter_notebook/
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/tests/data/module_jupyter_notebook/notebook_dependency.py
--rw-rw-rw-   0 root         (0) root         (0)     5740 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/tests/data/module_jupyter_notebook/test-notebook.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.032439 dyff_audit-0.3.2/tests/data/module_python_function/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.032439 dyff_audit-0.3.2/tests/data/module_python_function/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.044438 dyff_audit-0.3.2/tests/data/module_python_function/dyff/fake/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/tests/data/module_python_function/dyff/fake/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/tests/data/module_python_function/dyff/fake/method.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.032439 dyff_audit-0.3.2/tests/data/module_python_rubric/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.032439 dyff_audit-0.3.2/tests/data/module_python_rubric/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:55:32.045439 dyff_audit-0.3.2/tests/data/module_python_rubric/dyff/fake/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/tests/data/module_python_rubric/dyff/fake/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1726 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/tests/data/module_python_rubric/dyff/fake/rubric.py
--rw-rw-rw-   0 root         (0) root         (0)      948 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/tests/test_import.py
--rw-rw-rw-   0 root         (0) root         (0)    10808 2024-04-24 05:55:26.000000 dyff_audit-0.3.2/tests/test_local_platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.184360 dyff_audit-0.3.3/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1840 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1800 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-05-17 04:20:30.184360 dyff_audit-0.3.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.169360 dyff_audit-0.3.3/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.175360 dyff_audit-0.3.3/dyff/audit/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      604 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/_internal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.177360 dyff_audit-0.3.3/dyff/audit/analysis/
+-rw-rw-rw-   0 root         (0) root         (0)      296 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/analysis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6108 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/analysis/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1689 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/analysis/jupyter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/analysis/legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2814 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/analysis/python.py
+-rw-rw-rw-   0 root         (0) root         (0)     2920 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/analysis/runners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.177360 dyff_audit-0.3.3/dyff/audit/data/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2368 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/data/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/dynamic_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.178360 dyff_audit-0.3.3/dyff/audit/local/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5580 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/local/mocks.py
+-rw-rw-rw-   0 root         (0) root         (0)    33208 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/local/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.178360 dyff_audit-0.3.3/dyff/audit/metrics/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/metrics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/metrics/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4359 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/metrics/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.179360 dyff_audit-0.3.3/dyff/audit/scoring/
+-rw-rw-rw-   0 root         (0) root         (0)      261 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/scoring/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/scoring/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3949 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/scoring/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1787 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/scoring/example.py
+-rw-rw-rw-   0 root         (0) root         (0)    11999 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/scoring/text.py
+-rw-rw-rw-   0 root         (0) root         (0)     5994 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/dyff/audit/workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.183360 dyff_audit-0.3.3/dyff_audit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-05-17 04:20:30.000000 dyff_audit-0.3.3/dyff_audit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1457 2024-05-17 04:20:30.000000 dyff_audit-0.3.3/dyff_audit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 04:20:30.000000 dyff_audit-0.3.3/dyff_audit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2024-05-17 04:20:30.000000 dyff_audit-0.3.3/dyff_audit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-17 04:20:30.000000 dyff_audit-0.3.3/dyff_audit.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 04:20:30.184360 dyff_audit-0.3.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.181360 dyff_audit-0.3.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.171360 dyff_audit-0.3.3/tests/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.181360 dyff_audit-0.3.3/tests/data/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/tests/data/dataset/part-0.parquet
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.182360 dyff_audit-0.3.3/tests/data/evaluation/
+-rw-rw-rw-   0 root         (0) root         (0)     2990 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/tests/data/evaluation/part-0.parquet
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.182360 dyff_audit-0.3.3/tests/data/module_jupyter_notebook/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/tests/data/module_jupyter_notebook/notebook_dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)     5740 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/tests/data/module_jupyter_notebook/test-notebook.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.171360 dyff_audit-0.3.3/tests/data/module_python_function/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.171360 dyff_audit-0.3.3/tests/data/module_python_function/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.182360 dyff_audit-0.3.3/tests/data/module_python_function/dyff/fake/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/tests/data/module_python_function/dyff/fake/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/tests/data/module_python_function/dyff/fake/method.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.172360 dyff_audit-0.3.3/tests/data/module_python_rubric/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.172360 dyff_audit-0.3.3/tests/data/module_python_rubric/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 04:20:30.183360 dyff_audit-0.3.3/tests/data/module_python_rubric/dyff/fake/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/tests/data/module_python_rubric/dyff/fake/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/tests/data/module_python_rubric/dyff/fake/rubric.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/tests/test_import.py
+-rw-rw-rw-   0 root         (0) root         (0)    20502 2024-05-17 04:20:23.000000 dyff_audit-0.3.3/tests/test_workflows.py
```

### Comparing `dyff_audit-0.3.2/.gitlab-ci.yml` & `dyff_audit-0.3.3/.gitlab-ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     file:
       - detect-secrets.yml
   - project: buildgarden/pipelines/prettier
     ref: 0.3.2
     file:
       - prettier.yml
   - project: buildgarden/pipelines/python
-    ref: 0.9.1
+    ref: 0.10.0
     file:
       - python-autoflake.yml
       - python-black.yml
       - python-build-sdist.yml
       - python-build-wheel.yml
       - python-import-linter.yml
       - python-isort.yml
```

### Comparing `dyff_audit-0.3.2/.pre-commit-config.yaml` & `dyff_audit-0.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/.secrets.baseline` & `dyff_audit-0.3.3/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/CODE_OF_CONDUCT.md` & `dyff_audit-0.3.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/LICENSE` & `dyff_audit-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/PKG-INFO` & `dyff_audit-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-audit
-Version: 0.3.2
+Version: 0.3.3
 Summary: Audit tools for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-audit
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-audit/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_audit-0.3.2/README.md` & `dyff_audit-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/dyff/audit/analysis/context.py` & `dyff_audit-0.3.3/dyff/audit/analysis/context.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/dyff/audit/analysis/jupyter.py` & `dyff_audit-0.3.3/dyff/audit/analysis/jupyter.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/dyff/audit/analysis/legacy.py` & `dyff_audit-0.3.3/dyff/audit/analysis/legacy.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/dyff/audit/analysis/python.py` & `dyff_audit-0.3.3/dyff/audit/analysis/python.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/dyff/audit/analysis/runners.py` & `dyff_audit-0.3.3/dyff/audit/analysis/runners.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,52 +4,37 @@
 import os
 import subprocess
 from pathlib import Path
 from typing import Optional
 
 from dyff.schema.platform import MethodBase, MethodImplementationKind, Report
 
+from .._internal import fqn
 from . import jupyter, legacy, python
 
 
-def _fqn(obj) -> tuple[str, str]:
-    """See: https://stackoverflow.com/a/70693158"""
-    try:
-        module = obj.__module__
-    except AttributeError:
-        module = obj.__class__.__module__
-    try:
-        name = obj.__qualname__
-    except AttributeError:
-        name = obj.__class__.__qualname__
-    # if obj is a method of builtin class, then module will be None
-    if module == "builtins" or module is None:
-        raise AssertionError("should not be called on a builtin")
-    return module, name
-
-
 def run_analysis(method: MethodBase, *, storage_root: Path, config_file: Path):
     pythonpath = os.pathsep.join(
         str(storage_root / module) for module in method.modules
     )
     env = os.environ.copy()
     env.update(
         {
             "DYFF_AUDIT_LOCAL_STORAGE_ROOT": str(storage_root),
             "DYFF_AUDIT_ANALYSIS_CONFIG_FILE": str(config_file),
             "PYTHONPATH": pythonpath,
         }
     )
 
     if method.implementation.kind == MethodImplementationKind.JupyterNotebook:
-        impl_module, impl_name = _fqn(jupyter.run_jupyter_notebook)
+        impl_module, impl_name = fqn(jupyter.run_jupyter_notebook)
     elif method.implementation.kind == MethodImplementationKind.PythonFunction:
-        impl_module, impl_name = _fqn(python.run_python_function)
+        impl_module, impl_name = fqn(python.run_python_function)
     elif method.implementation.kind == MethodImplementationKind.PythonRubric:
-        impl_module, impl_name = _fqn(python.run_python_rubric)
+        impl_module, impl_name = fqn(python.run_python_rubric)
     else:
         raise NotImplementedError(
             f"method.implementation.kind = {method.implementation.kind}"
         )
 
     cmd = f"from {impl_module} import {impl_name}; {impl_name}()"
     subprocess.run(
@@ -88,15 +73,15 @@
         quote(rubric),
         quote(dataset_path),
         quote(evaluation_path),
         quote(output_path),
         ", ".join(quote(module) for module in modules),
     ]
 
-    impl_module, impl_name = _fqn(legacy.run_python_rubric)
+    impl_module, impl_name = fqn(legacy.run_python_rubric)
     cmd = (
         f"from {impl_module} import {impl_name}; {impl_name}"
         "(rubric={}, dataset_path={}, evaluation_path={}, output_path={}, modules=[{}])".format(
             *args
         )
     )
```

### Comparing `dyff_audit-0.3.2/dyff/audit/data/text.py` & `dyff_audit-0.3.3/dyff/audit/data/text.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/dyff/audit/local/platform.py` & `dyff_audit-0.3.3/dyff/audit/local/platform.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,58 +3,58 @@
 
 # mypy: disable-error-code="import-untyped"
 from __future__ import annotations
 
 import json
 from datetime import datetime
 from pathlib import Path
-from typing import Any, Iterable, Optional, TypeVar
+from typing import Any, Optional, Type
 
-import pyarrow
 import ruamel.yaml
 
-from dyff.client import Client
+from dyff.client import Client, HttpResponseError
 from dyff.schema import ids
+from dyff.schema.adapters import Adapter, create_pipeline
 from dyff.schema.dataset import arrow, binary
 from dyff.schema.platform import (
     Analysis,
     Artifact,
     DataSchema,
     Dataset,
     Digest,
     EntityStatus,
     Evaluation,
     ForeignInferenceService,
     ForeignMethod,
     InferenceInterface,
+    InferenceService,
+    InferenceSession,
+    InferenceSessionAndToken,
     InferenceSessionSpec,
     Measurement,
     Method,
-    MethodInputKind,
     Module,
     Report,
     SafetyCase,
 )
 from dyff.schema.requests import (
     AnalysisCreateRequest,
     DatasetCreateRequest,
     EvaluationCreateRequest,
+    InferenceSessionCreateRequest,
     MethodCreateRequest,
     ModuleCreateRequest,
     ReportCreateRequest,
 )
 
+from .. import dynamic_import
+from .._internal import fqn
 from ..analysis import run_analysis, run_report
 from ..workflows import local_evaluation
-
-T = TypeVar("T")
-
-
-def _once(x: T) -> Iterable[T]:
-    yield x
+from . import mocks
 
 
 class _Datasets:
     def __init__(self, platform: DyffLocalPlatform):
         self._platform = platform
 
     def create(self, dataset_request: DatasetCreateRequest) -> Dataset:
@@ -68,17 +68,20 @@
 
         cache_dir = self._platform.entity_path(id)
         cache_dir.mkdir()
         with open(cache_dir / ".dataset.json", "w") as fout:
             fout.write(dataset.json())
         return dataset
 
-    def get(self, id: str) -> Dataset:
-        file = self._platform.entity_path(id) / ".dataset.json"
-        return Dataset.parse_file(file)
+    def get(self, id: str) -> Optional[Dataset]:
+        try:
+            file = self._platform.entity_path(id) / ".dataset.json"
+            return Dataset.parse_file(file)
+        except FileNotFoundError:
+            return None
 
     def create_arrow_dataset(
         self, dataset_directory: str, *, account: str, name: str
     ) -> Dataset:
         """Create a Dataset resource describing an existing Arrow dataset.
 
         Internally, constructs a ``DatasetCreateRequest`` using information
@@ -152,14 +155,83 @@
                     fout.write(fin.read())
 
 
 class _Evaluations:
     def __init__(self, platform: DyffLocalPlatform):
         self._platform = platform
 
+    def create(
+        self, evaluation_request: EvaluationCreateRequest, *, id: Optional[str] = None
+    ) -> Evaluation:
+        id = id or ids.generate_entity_id()
+        dataset = self._platform.datasets.get(evaluation_request.dataset)
+        if dataset is None:
+            raise HttpResponseError(status_code=404)
+
+        evaluation_dict: dict[str, Any] = {}
+        evaluation_dict["id"] = id
+        evaluation_dict["account"] = evaluation_request.account
+        evaluation_dict["dataset"] = evaluation_request.dataset
+        evaluation_dict["replications"] = evaluation_request.replications
+
+        if evaluation_request.inferenceSessionReference is not None:
+            session = self._platform.inferencesessions.get(
+                evaluation_request.inferenceSessionReference
+            )
+            if session is None:
+                raise HttpResponseError(status_code=404)
+            token = self._platform.inferencesessions.token(session.id)
+            evaluation_dict["inferenceSessionReference"] = (
+                evaluation_request.inferenceSessionReference
+            )
+        elif evaluation_request.inferenceSession is not None:
+            service_id = evaluation_request.inferenceSession.inferenceService
+            session_request = InferenceSessionCreateRequest(
+                account=evaluation_request.account, inferenceService=service_id
+            )
+            session_and_token = self._platform.inferencesessions.create(session_request)
+            session = session_and_token.inferencesession
+            token = session_and_token.token
+        else:
+            raise ValueError(
+                "must specify one of {inferenceSession, inferenceSessionReference}"
+            )
+
+        evaluation_dict["inferenceSession"] = session.dict()
+        evaluation = Evaluation.parse_obj(evaluation_dict)
+        # TODO: Actually check success / failure
+        evaluation.status = EntityStatus.complete
+
+        cache_dir = self._platform.entity_path(evaluation.id)
+        cache_dir.mkdir()
+        with open(cache_dir / ".evaluation.json", "w") as fout:
+            fout.write(evaluation.json())
+
+        inference_client = self._platform.inferencesessions.client(
+            session.id, token, interface=session.inferenceService.interface
+        )
+        session.inferenceService.interface.outputSchema.arrowSchema
+
+        input_dataset = arrow.open_dataset(str(self._platform.entity_path(dataset.id)))
+
+        output_generator = inference_client.run_evaluation(
+            input_dataset,
+            replications=evaluation_request.replications,
+            id=evaluation.id,
+        )
+        arrow.write_dataset(
+            output_generator,
+            output_path=str(self._platform.entity_path(evaluation.id)),
+            feature_schema=arrow.decode_schema(
+                session.inferenceService.interface.outputSchema.arrowSchema
+            ),
+        )
+
+        return evaluation
+
     def import_data(
         self,
         dataset_directory: Path | str,
         *,
         id: Optional[str] = None,
         evaluation_request: Optional[EvaluationCreateRequest] = None,
     ) -> Evaluation:
@@ -186,30 +258,33 @@
             evaluation_request and evaluation_request.account
         ) or ids.null_id()
         evaluation_dict["dataset"] = (
             evaluation_request and evaluation_request.dataset
         ) or ids.null_id()
         evaluation_dict["replications"] = len(replications)
 
-        service_id = (
-            evaluation_request and evaluation_request.inferenceSession.inferenceService
-        ) or ids.null_id()
+        if evaluation_request and evaluation_request.inferenceSession:
+            service_id = evaluation_request.inferenceSession.inferenceService
+        else:
+            service_id = ids.null_id()
         session_spec = InferenceSessionSpec(
             inferenceService=ForeignInferenceService(
                 id=service_id,
                 name="",
                 account=ids.null_id(),
                 interface=InferenceInterface(
                     endpoint="",
                     outputSchema=DataSchema(arrowSchema=arrow.encode_schema(ds.schema)),
                 ),
             )
         )
         evaluation_dict["inferenceSession"] = session_spec.dict()
         evaluation = Evaluation.parse_obj(evaluation_dict)
+        # TODO: actually check success / failure
+        evaluation.status = EntityStatus.complete
 
         cache_dir = self._platform.entity_path(evaluation.id)
         cache_dir.mkdir()
         with open(cache_dir / ".evaluation.json", "w") as fout:
             fout.write(evaluation.json())
 
         artifact_paths = [
@@ -229,14 +304,15 @@
             assert artifact.digest.md5 is not None
             file_path = Path(dataset_directory) / artifact.path
             cache_path = self._platform.entity_path(evaluation.id) / artifact.path
             cache_path.parent.mkdir(parents=True, exist_ok=True)
             with open(file_path, "rb") as fin:
                 with open(cache_path, "wb") as fout:
                     fout.write(fin.read())
+
         return evaluation
 
     def local_evaluation(self, *, dataset: str, inferencesession: str) -> str:
         client = self._platform._require_client()
         session = client.inferencesessions.get(inferencesession)
         id = ids.generate_entity_id()
         return local_evaluation(
@@ -244,28 +320,170 @@
             session,
             input_dataset_path=self._platform.entity_path(dataset),
             # workflows.local_evaluation() creates an /id subdirectory for the output
             output_dataset_path=self._platform.storage_root,
             id=id,
         )
 
-    def get(self, id: str) -> Evaluation:
-        file = self._platform.entity_path(id) / ".evaluation.json"
-        return Evaluation.parse_file(file)
+    def get(self, id: str) -> Optional[Evaluation]:
+        try:
+            file = self._platform.entity_path(id) / ".evaluation.json"
+            return Evaluation.parse_file(file)
+        except FileNotFoundError:
+            return None
+
+
+class _InferenceServices:
+    def __init__(self, platform: DyffLocalPlatform):
+        self._platform = platform
+
+    def create_mock(
+        self,
+        mock_type: Type[mocks.InferenceServiceMock],
+        *,
+        account: str,
+        id: Optional[str] = None,
+    ) -> InferenceService:
+        id = id or ids.generate_entity_id()
+
+        mock = mock_type()
+        service = InferenceService(
+            account=account,
+            id=id,
+            name=".".join(fqn(mock_type)),
+            interface=mock.interface,
+            status=EntityStatus.ready,
+        )
+
+        cache_dir = self._platform.entity_path(id)
+        cache_dir.mkdir()
+        with open(cache_dir / ".inferenceservice.json", "w") as fout:
+            fout.write(service.json())
+
+        return service
+
+    def get(self, id: str) -> Optional[InferenceService]:
+        try:
+            file = self._platform.entity_path(id) / ".inferenceservice.json"
+            return InferenceService.parse_file(file)
+        except FileNotFoundError:
+            return None
+
+
+class _InferenceSessions:
+    def __init__(self, platform: DyffLocalPlatform):
+        self._platform = platform
+
+    def create(
+        self, session_request: InferenceSessionCreateRequest
+    ) -> InferenceSessionAndToken:
+        id = ids.generate_entity_id()
+
+        service = self._platform.inferenceservices.get(session_request.inferenceService)
+        if service is None:
+            raise HttpResponseError(status_code=404)
+
+        session = InferenceSession(
+            account=session_request.account,
+            id=id,
+            inferenceService=ForeignInferenceService.parse_obj(service.dict()),
+            status=EntityStatus.admitted,
+        )
+
+        cache_dir = self._platform.entity_path(id)
+        cache_dir.mkdir()
+        with open(cache_dir / ".inferencesession.json", "w") as fout:
+            fout.write(session.json())
+
+        return InferenceSessionAndToken(inferencesession=session, token="dummy-token")
+
+    def get(self, id: str) -> Optional[InferenceSession]:
+        try:
+            file = self._platform.entity_path(id) / ".inferencesession.json"
+            return InferenceSession.parse_file(file)
+        except FileNotFoundError:
+            return None
+
+    def delete(self, id: str) -> None:
+        session = self.get(id)
+        if session is None:
+            raise HttpResponseError(status_code=404)
+        session.status = EntityStatus.deleted
+        with open(
+            self._platform.entity_path(id) / ".inferencesession.json", "w"
+        ) as fout:
+            fout.write(session.json())
+
+    def ready(self, id: str) -> bool:
+        try:
+            session = self.get(id)
+            if session is None:
+                raise HttpResponseError(status_code=404)
+            return session.status == EntityStatus.admitted
+        except:
+            return False
+
+    def token(self, id: str) -> str:
+        return "dummy-token"
+
+    def infer(
+        self, id: str, endpoint: str, request: dict[str, Any]
+    ) -> list[dict[str, Any]]:
+        session = self.get(id)
+        if session is None:
+            raise HttpResponseError(status_code=404)
+        mock: mocks.InferenceServiceMock = dynamic_import.instantiate(
+            session.inferenceService.name
+        )
+        return mock.infer(endpoint, request)
+
+    def client(
+        self,
+        session_id: str,
+        token: str,
+        *,
+        interface: Optional[InferenceInterface] = None,
+        endpoint: Optional[str] = None,
+        input_adapter: Optional[Adapter] = None,
+        output_adapter: Optional[Adapter] = None,
+    ) -> mocks.InferenceSessionClientMock:
+        if interface is not None:
+            inference_endpoint = endpoint or interface.endpoint
+            if input_adapter is None:
+                if interface.inputPipeline is not None:
+                    input_adapter = create_pipeline(interface.inputPipeline)
+            if output_adapter is None:
+                if interface.outputPipeline is not None:
+                    output_adapter = create_pipeline(interface.outputPipeline)
+
+        session = self.get(session_id)
+        if session is None:
+            raise HttpResponseError(status_code=404)
+        service: mocks.InferenceServiceMock = dynamic_import.instantiate(
+            session.inferenceService.name
+        )
+        return mocks.InferenceSessionClientMock(
+            service,
+            inference_endpoint=inference_endpoint,
+            input_adapter=input_adapter,
+            output_adapter=output_adapter,
+        )
 
 
 class _Measurements:
     def __init__(self, platform: DyffLocalPlatform):
         self._platform = platform
 
     def create(self, analysis_request: AnalysisCreateRequest) -> Measurement:
         id = ids.generate_entity_id()
 
         method_id = analysis_request.method
         method = self._platform.methods.get(method_id)
+        if method is None:
+            raise HttpResponseError(status_code=404)
 
         # Create an entity representing the output of the Analysis
         measurement_spec = method.output.measurement
         if measurement_spec is None:
             raise ValueError("Method spec violates constraints")
 
         measurement = Measurement(
@@ -302,17 +520,20 @@
             method,
             storage_root=self._platform.storage_root,
             config_file=config_file,
         )
 
         return measurement
 
-    def get(self, id: str) -> Measurement:
-        file = self._platform.entity_path(id) / ".measurement.json"
-        return Measurement.parse_file(file)
+    def get(self, id: str) -> Optional[Measurement]:
+        try:
+            file = self._platform.entity_path(id) / ".measurement.json"
+            return Measurement.parse_file(file)
+        except FileNotFoundError:
+            return None
 
 
 class _Methods:
     def __init__(self, platform: DyffLocalPlatform):
         self._platform = platform
 
     def create(self, method_request: MethodCreateRequest) -> Method:
@@ -326,17 +547,20 @@
 
         cache_dir = self._platform.entity_path(id)
         cache_dir.mkdir()
         with open(cache_dir / ".method.json", "w") as fout:
             fout.write(method.json())
         return method
 
-    def get(self, id: str) -> Method:
-        file = self._platform.entity_path(id) / ".method.json"
-        return Method.parse_file(file)
+    def get(self, id: str) -> Optional[Method]:
+        try:
+            file = self._platform.entity_path(id) / ".method.json"
+            return Method.parse_file(file)
+        except FileNotFoundError:
+            return None
 
 
 class _Modules:
     def __init__(self, platform: DyffLocalPlatform):
         self._platform = platform
 
     def create(self, module_request: ModuleCreateRequest) -> Module:
@@ -350,17 +574,20 @@
 
         cache_dir = self._platform.entity_path(id)
         cache_dir.mkdir()
         with open(cache_dir / ".module.json", "w") as fout:
             fout.write(module.json())
         return module
 
-    def get(self, id: str) -> Module:
-        file = self._platform.entity_path(id) / ".module.json"
-        return Module.parse_file(file)
+    def get(self, id: str) -> Optional[Module]:
+        try:
+            file = self._platform.entity_path(id) / ".module.json"
+            return Module.parse_file(file)
+        except FileNotFoundError:
+            return None
 
     def create_package(
         self, package_directory: str, *, account: str, name: str
     ) -> Module:
         """Create a Module resource describing a package structured as a directory tree.
 
         Internally, constructs a ``ModuleCreateRequest`` using information
@@ -443,14 +670,16 @@
         report_dict = report_request.dict()
         report_dict["id"] = id
         report_dict["account"] = self._platform.account
         report_dict["status"] = EntityStatus.ready
         report_dict["creationTime"] = datetime.now()
 
         evaluation = self._platform.evaluations.get(report_request.evaluation)
+        if evaluation is None:
+            raise HttpResponseError(status_code=404)
         report_dict["dataset"] = evaluation.dataset
         report_dict["inferenceService"] = (
             evaluation.inferenceSession.inferenceService.id
         )
 
         report = Report.parse_obj(report_dict)
 
@@ -459,28 +688,33 @@
         with open(cache_dir / ".report.json", "w") as fout:
             fout.write(report.json())
 
         run_report(report, storage_root=self._platform.storage_root)
 
         return report
 
-    def get(self, id: str) -> Module:
-        file = self._platform.entity_path(id) / ".module.json"
-        return Module.parse_file(file)
+    def get(self, id: str) -> Optional[Report]:
+        try:
+            file = self._platform.entity_path(id) / ".report.json"
+            return Report.parse_file(file)
+        except FileNotFoundError:
+            return None
 
 
 class _SafetyCases:
     def __init__(self, platform: DyffLocalPlatform):
         self._platform = platform
 
     def create(self, analysis_request: AnalysisCreateRequest) -> SafetyCase:
         id = ids.generate_entity_id()
 
         method_id = analysis_request.method
         method = self._platform.methods.get(method_id)
+        if method is None:
+            raise HttpResponseError(status_code=404)
 
         # Create an entity representing the output of the Analysis
         safetycase_spec = method.output.safetyCase
         if safetycase_spec is None:
             raise ValueError("Method spec violates constraints")
 
         safetycase = SafetyCase(
@@ -518,17 +752,20 @@
             method,
             storage_root=self._platform.storage_root,
             config_file=config_file,
         )
 
         return safetycase
 
-    def get(self, id: str) -> SafetyCase:
-        file = self._platform.entity_path(id) / ".safetycase.json"
-        return SafetyCase.parse_file(file)
+    def get(self, id: str) -> Optional[SafetyCase]:
+        try:
+            file = self._platform.entity_path(id) / ".safetycase.json"
+            return SafetyCase.parse_file(file)
+        except FileNotFoundError:
+            return None
 
 
 class DyffLocalPlatform:
     """Emulates a subset of Dyff Platform operations locally.
 
     This class is intended to aid in local development and debugging of code
     and data that will run on the Dyff Platform. The inferface mirrors that of
@@ -539,23 +776,25 @@
     calls like ``get`` and ``data`` will forward to a remote Dyff Platform
     instance if the requested entity is not available locally. API calls that
     modify the platform state are **never** forwarded to a remote instance.
     """
 
     def __init__(
         self,
-        storage_root: Path,
+        storage_root: Path | str,
         *,
         remote_client: Optional[Client] = None,
     ):
-        self._storage_root = storage_root
+        self._storage_root = Path(storage_root)
         self._client = remote_client
 
         self._datasets = _Datasets(self)
         self._evaluations = _Evaluations(self)
+        self._inferenceservices = _InferenceServices(self)
+        self._inferencesessions = _InferenceSessions(self)
         self._measurements = _Measurements(self)
         self._methods = _Methods(self)
         self._modules = _Modules(self)
         self._reports = _Reports(self)
         self._safetycases = _SafetyCases(self)
 
         self._storage_root.mkdir(exist_ok=True)
@@ -574,14 +813,22 @@
         return self._datasets
 
     @property
     def evaluations(self) -> _Evaluations:
         return self._evaluations
 
     @property
+    def inferenceservices(self) -> _InferenceServices:
+        return self._inferenceservices
+
+    @property
+    def inferencesessions(self) -> _InferenceSessions:
+        return self._inferencesessions
+
+    @property
     def measurements(self) -> _Measurements:
         return self._measurements
 
     @property
     def methods(self) -> _Methods:
         return self._methods
 
@@ -632,34 +879,34 @@
             target = cache_path.resolve()
             if target != package:
                 raise ValueError(f"{id} -> {target}: conflict")
         else:
             raise ValueError(f"{cache_path} exists and is not a symlink")
         return id
 
-    def _download_data(self, kind: MethodInputKind, id: str, path: Path):
-        assert self._client is not None
-        if kind == MethodInputKind.Dataset:
-            dataset = self._client.datasets.get(id)
-            dataset_data = self._client.datasets.data(dataset)
-            arrow.write_dataset(
-                dataset_data.to_batches(),
-                output_path=str(path),
-                feature_schema=dataset_data.dataset_schema,
-                existing_data_behavior="error",
-            )
-        elif kind == MethodInputKind.Evaluation:
-            raise NotImplementedError()
-        elif kind == MethodInputKind.Measurement:
-            raise NotImplementedError()
-        elif kind == MethodInputKind.Report:
-            report = self._client.reports.get(id)
-            report_data = self._client.reports.data(report)
-            record_batch = pyarrow.RecordBatch.from_pandas(report_data)
-            arrow.write_dataset(
-                _once(record_batch),
-                output_path=str(path),
-                feature_schema=record_batch.schema,
-                existing_data_behavior="error",
-            )
-        else:
-            raise ValueError(f"MethodInputKind {kind}")
+    # def _download_data(self, kind: MethodInputKind, id: str, path: Path):
+    #     assert self._client is not None
+    #     if kind == MethodInputKind.Dataset:
+    #         dataset = self._client.datasets.get(id)
+    #         dataset_data = self._client.datasets.data(dataset)
+    #         arrow.write_dataset(
+    #             dataset_data.to_batches(),
+    #             output_path=str(path),
+    #             feature_schema=dataset_data.dataset_schema,
+    #             existing_data_behavior="error",
+    #         )
+    #     elif kind == MethodInputKind.Evaluation:
+    #         raise NotImplementedError()
+    #     elif kind == MethodInputKind.Measurement:
+    #         raise NotImplementedError()
+    #     elif kind == MethodInputKind.Report:
+    #         report = self._client.reports.get(id)
+    #         report_data = self._client.reports.data(report)
+    #         record_batch = pyarrow.RecordBatch.from_pandas(report_data)
+    #         arrow.write_dataset(
+    #             _once(record_batch),
+    #             output_path=str(path),
+    #             feature_schema=record_batch.schema,
+    #             existing_data_behavior="error",
+    #         )
+    #     else:
+    #         raise ValueError(f"MethodInputKind {kind}")
```

### Comparing `dyff_audit-0.3.2/dyff/audit/metrics/base.py` & `dyff_audit-0.3.3/dyff/audit/metrics/base.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/dyff/audit/metrics/text.py` & `dyff_audit-0.3.3/dyff/audit/metrics/text.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/dyff/audit/scoring/base.py` & `dyff_audit-0.3.3/dyff/audit/scoring/base.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/dyff/audit/scoring/classification.py` & `dyff_audit-0.3.3/dyff/audit/scoring/classification.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/dyff/audit/scoring/example.py` & `dyff_audit-0.3.3/dyff/audit/scoring/example.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/dyff/audit/scoring/text.py` & `dyff_audit-0.3.3/dyff/audit/scoring/text.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/dyff/audit/workflows.py` & `dyff_audit-0.3.3/dyff/audit/workflows.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/dyff_audit.egg-info/PKG-INFO` & `dyff_audit-0.3.3/dyff_audit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-audit
-Version: 0.3.2
+Version: 0.3.3
 Summary: Audit tools for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-audit
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-audit/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_audit-0.3.2/dyff_audit.egg-info/SOURCES.txt` & `dyff_audit-0.3.3/dyff_audit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 CODE_OF_CONDUCT.md
 LICENSE
 NOTICE
 README.md
 makefile
 pyproject.toml
 dyff/audit/__init__.py
+dyff/audit/_internal.py
 dyff/audit/dynamic_import.py
 dyff/audit/workflows.py
 dyff/audit/analysis/__init__.py
 dyff/audit/analysis/context.py
 dyff/audit/analysis/jupyter.py
 dyff/audit/analysis/legacy.py
 dyff/audit/analysis/python.py
 dyff/audit/analysis/runners.py
 dyff/audit/data/__init__.py
 dyff/audit/data/text.py
 dyff/audit/local/__init__.py
+dyff/audit/local/mocks.py
 dyff/audit/local/platform.py
 dyff/audit/metrics/__init__.py
 dyff/audit/metrics/base.py
 dyff/audit/metrics/text.py
 dyff/audit/scoring/__init__.py
 dyff/audit/scoring/base.py
 dyff/audit/scoring/classification.py
@@ -34,15 +36,15 @@
 dyff_audit.egg-info/PKG-INFO
 dyff_audit.egg-info/SOURCES.txt
 dyff_audit.egg-info/dependency_links.txt
 dyff_audit.egg-info/requires.txt
 dyff_audit.egg-info/top_level.txt
 tests/conftest.py
 tests/test_import.py
-tests/test_local_platform.py
+tests/test_workflows.py
 tests/data/dataset/part-0.parquet
 tests/data/evaluation/part-0.parquet
 tests/data/module_jupyter_notebook/notebook_dependency.py
 tests/data/module_jupyter_notebook/test-notebook.ipynb
 tests/data/module_python_function/dyff/fake/__init__.py
 tests/data/module_python_function/dyff/fake/method.py
 tests/data/module_python_rubric/dyff/fake/__init__.py
```

### Comparing `dyff_audit-0.3.2/makefile` & `dyff_audit-0.3.3/makefile`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/pyproject.toml` & `dyff_audit-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/tests/data/dataset/part-0.parquet` & `dyff_audit-0.3.3/tests/data/dataset/part-0.parquet`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/tests/data/evaluation/part-0.parquet` & `dyff_audit-0.3.3/tests/data/evaluation/part-0.parquet`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/tests/data/module_jupyter_notebook/test-notebook.ipynb` & `dyff_audit-0.3.3/tests/data/module_jupyter_notebook/test-notebook.ipynb`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/tests/data/module_python_function/dyff/fake/method.py` & `dyff_audit-0.3.3/tests/data/module_python_function/dyff/fake/method.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/tests/data/module_python_rubric/dyff/fake/rubric.py` & `dyff_audit-0.3.3/tests/data/module_python_rubric/dyff/fake/rubric.py`

 * *Files identical despite different names*

### Comparing `dyff_audit-0.3.2/tests/test_import.py` & `dyff_audit-0.3.3/tests/test_import.py`

 * *Files identical despite different names*

