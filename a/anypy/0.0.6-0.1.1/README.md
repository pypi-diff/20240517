# Comparing `tmp/anypy-0.0.6.tar.gz` & `tmp/anypy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anypy-0.0.6.tar", last modified: Thu Oct 12 10:11:55 2023, max compression
+gzip compressed data, was "anypy-0.1.1.tar", last modified: Fri May 17 12:50:32 2024, max compression
```

## Comparing `anypy-0.0.6.tar` & `anypy-0.1.1.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.816382 anypy-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-10-12 10:02:08.000000 anypy-0.0.6/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-10-12 10:02:08.000000 anypy-0.0.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.808381 anypy-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.812381 anypy-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2023-10-12 10:02:08.000000 anypy-0.0.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2023-10-12 10:02:08.000000 anypy-0.0.6/.github/workflows/test_suite.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2023-10-12 10:02:08.000000 anypy-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2023-10-12 10:02:08.000000 anypy-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-10-12 10:02:08.000000 anypy-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2023-10-12 10:11:55.816382 anypy-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2023-10-12 10:02:08.000000 anypy-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.812381 anypy-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2023-10-12 10:02:08.000000 anypy-0.0.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.812381 anypy-0.0.6/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-10-12 10:02:08.000000 anypy-0.0.6/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-10-12 10:11:46.000000 anypy-0.0.6/env.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2023-10-12 10:02:08.000000 anypy-0.0.6/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.808381 anypy-0.0.6/notebooks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.812381 anypy-0.0.6/notebooks/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-10-12 10:11:33.000000 anypy-0.0.6/notebooks/recipes/hydraconf_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2023-10-12 10:11:33.000000 anypy-0.0.6/notebooks/recipes/savefig_pdf.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      961 2023-10-12 10:02:08.000000 anypy-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      756 2023-10-12 10:11:55.816382 anypy-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-10-12 10:02:08.000000 anypy-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.808381 anypy-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.812381 anypy-0.0.6/src/anypy/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-10-12 10:02:08.000000 anypy-0.0.6/src/anypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-12 10:11:55.000000 anypy-0.0.6/src/anypy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.812381 anypy-0.0.6/src/anypy/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 10:02:08.000000 anypy-0.0.6/src/anypy/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2023-10-12 10:02:08.000000 anypy-0.0.6/src/anypy/benchmark/chrono.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.812381 anypy-0.0.6/src/anypy/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2023-10-12 10:02:08.000000 anypy-0.0.6/src/anypy/data/metadata_dataset_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.812381 anypy-0.0.6/src/anypy/latex/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-12 10:02:08.000000 anypy-0.0.6/src/anypy/latex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2023-10-12 10:02:08.000000 anypy-0.0.6/src/anypy/latex/dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.812381 anypy-0.0.6/src/anypy/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2023-10-12 10:02:08.000000 anypy-0.0.6/src/anypy/nn/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    15393 2023-10-12 10:02:08.000000 anypy-0.0.6/src/anypy/nn/dyncnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2023-10-12 10:02:08.000000 anypy-0.0.6/src/anypy/nn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.812381 anypy-0.0.6/src/anypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2023-10-12 10:11:55.000000 anypy-0.0.6/src/anypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2023-10-12 10:11:55.000000 anypy-0.0.6/src/anypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 10:11:55.000000 anypy-0.0.6/src/anypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 10:09:44.000000 anypy-0.0.6/src/anypy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-10-12 10:11:55.000000 anypy-0.0.6/src/anypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-12 10:11:55.000000 anypy-0.0.6/src/anypy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.812381 anypy-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 10:02:08.000000 anypy-0.0.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.812381 anypy-0.0.6/tests/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2023-10-12 10:02:08.000000 anypy-0.0.6/tests/benchmark/test_chrono.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.816382 anypy-0.0.6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-10-12 10:02:08.000000 anypy-0.0.6/tests/data/test_metadata_dataset_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.816382 anypy-0.0.6/tests/latex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 10:02:08.000000 anypy-0.0.6/tests/latex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2023-10-12 10:02:08.000000 anypy-0.0.6/tests/latex/test_dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 10:11:55.816382 anypy-0.0.6/tests/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2023-10-12 10:02:08.000000 anypy-0.0.6/tests/nn/test_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2023-10-12 10:02:08.000000 anypy-0.0.6/tests/nn/test_dyncnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-10-12 10:02:08.000000 anypy-0.0.6/tests/nn/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-12 10:02:08.000000 anypy-0.0.6/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.139304 anypy-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-17 12:45:00.000000 anypy-0.1.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-17 12:45:00.000000 anypy-0.1.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.135304 anypy-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.135304 anypy-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-17 12:45:00.000000 anypy-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-17 12:45:00.000000 anypy-0.1.1/.github/workflows/test_suite.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-17 12:45:00.000000 anypy-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-17 12:45:00.000000 anypy-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-17 12:45:00.000000 anypy-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-17 12:50:32.139304 anypy-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-17 12:45:00.000000 anypy-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.135304 anypy-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-17 12:45:00.000000 anypy-0.1.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.135304 anypy-0.1.1/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-17 12:45:00.000000 anypy-0.1.1/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-17 12:50:26.000000 anypy-0.1.1/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-17 12:45:00.000000 anypy-0.1.1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.135304 anypy-0.1.1/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.135304 anypy-0.1.1/notebooks/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-17 12:50:18.000000 anypy-0.1.1/notebooks/recipes/hydraconf_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-17 12:50:18.000000 anypy-0.1.1/notebooks/recipes/savefig_pdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-17 12:50:18.000000 anypy-0.1.1/notebooks/recipes/savefig_sns_pdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-17 12:45:00.000000 anypy-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-17 12:50:32.139304 anypy-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-17 12:45:00.000000 anypy-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.135304 anypy-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.135304 anypy-0.1.1/src/anypy/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-17 12:45:00.000000 anypy-0.1.1/src/anypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-17 12:50:32.000000 anypy-0.1.1/src/anypy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.139304 anypy-0.1.1/src/anypy/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:45:00.000000 anypy-0.1.1/src/anypy/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-17 12:45:00.000000 anypy-0.1.1/src/anypy/benchmark/chrono.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.139304 anypy-0.1.1/src/anypy/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-17 12:45:00.000000 anypy-0.1.1/src/anypy/data/metadata_dataset_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.139304 anypy-0.1.1/src/anypy/latex/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-17 12:45:00.000000 anypy-0.1.1/src/anypy/latex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-17 12:45:00.000000 anypy-0.1.1/src/anypy/latex/dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.139304 anypy-0.1.1/src/anypy/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-05-17 12:45:00.000000 anypy-0.1.1/src/anypy/nn/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15393 2024-05-17 12:45:00.000000 anypy-0.1.1/src/anypy/nn/dyncnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-17 12:45:00.000000 anypy-0.1.1/src/anypy/nn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.139304 anypy-0.1.1/src/anypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-17 12:50:32.000000 anypy-0.1.1/src/anypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-17 12:50:32.000000 anypy-0.1.1/src/anypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:50:32.000000 anypy-0.1.1/src/anypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:49:13.000000 anypy-0.1.1/src/anypy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 12:50:32.000000 anypy-0.1.1/src/anypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 12:50:32.000000 anypy-0.1.1/src/anypy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.139304 anypy-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:45:00.000000 anypy-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.139304 anypy-0.1.1/tests/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-17 12:45:00.000000 anypy-0.1.1/tests/benchmark/test_chrono.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.139304 anypy-0.1.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-17 12:45:00.000000 anypy-0.1.1/tests/data/test_metadata_dataset_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.139304 anypy-0.1.1/tests/latex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:45:00.000000 anypy-0.1.1/tests/latex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-17 12:45:00.000000 anypy-0.1.1/tests/latex/test_dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:50:32.139304 anypy-0.1.1/tests/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-17 12:45:00.000000 anypy-0.1.1/tests/nn/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-17 12:45:00.000000 anypy-0.1.1/tests/nn/test_dyncnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-17 12:45:00.000000 anypy-0.1.1/tests/nn/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-17 12:45:00.000000 anypy-0.1.1/tests/test_package.py
```

### Comparing `anypy-0.0.6/.github/workflows/publish.yml` & `anypy-0.1.1/.github/workflows/publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
           pytest -v
 
       - name: Build docs website
         shell: bash -l {0}
         run: |
           git config user.name ci-bot
           git config user.email ci-bot@ci.com
-          mike deploy --rebase --push --update-aliases ${RELEASE_TAG_VERSION} latest
+          mike deploy --push --update-aliases ${RELEASE_TAG_VERSION} latest
 
         # Uncomment to publish on PyPI on release
       - name: Check working directory status
         run: git status
 
       - name: Restore working directory (env.yaml Python version)
         run: git checkout .
```

### Comparing `anypy-0.0.6/.github/workflows/test_suite.yml` & `anypy-0.1.1/.github/workflows/test_suite.yml`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/.gitignore` & `anypy-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/.pre-commit-config.yaml` & `anypy-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/LICENSE` & `anypy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/PKG-INFO` & `anypy-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: anypy
-Version: 0.0.6
+Version: 0.1.1
 Summary: A collection of python utilities, without hard dependencies
 Home-page: https://github.com/lucmos/anypy
 Author: Luca Moschella
 Author-email: luca.moschella94@gmail.com
 License: MIT Licence
 Keywords: python
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Provides-Extra: core
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # Generic Python Tools & Utilities
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1 Name: anypy Version: 0.0.6 Summary: A collection of
+Metadata-Version: 2.1 Name: anypy Version: 0.1.1 Summary: A collection of
 python utilities, without hard dependencies Home-page: https://github.com/
 lucmos/anypy Author: Luca Moschella Author-email: luca.moschella94@gmail.com
 License: MIT Licence Keywords: python Platform: UNKNOWN Description-Content-
-Type: text/markdown Provides-Extra: docs Provides-Extra: test Provides-Extra:
-dev License-File: LICENSE # Generic Python Tools & Utilities
+Type: text/markdown Provides-Extra: core Provides-Extra: docs Provides-Extra:
+test Provides-Extra: dev License-File: LICENSE # Generic Python Tools &
+Utilities
                    _[_P_y_P_i_]_[_P_y_P_i_]_[_C_I_]_[_D_o_c_s_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
 A collection of python utilities, without hard dependencies ## Installation
 ```bash pip install anypy ``` ## Quickstart [comment]: <> (> Fill me!) ##
 Development installation Setup the development environment: ```bash git clone
 git@github.com:lucmos/anypy.git cd anypy conda env create -f env.yaml conda
 activate anypy pre-commit install ``` Run the tests: ```bash pre-commit run --
 all-files pytest -v ``` ### Update the dependencies Re-install the project in
```

### Comparing `anypy-0.0.6/README.md` & `anypy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/docs/index.md` & `anypy-0.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/mkdocs.yml` & `anypy-0.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/notebooks/recipes/hydraconf_notebook.ipynb` & `anypy-0.1.1/notebooks/recipes/hydraconf_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/notebooks/recipes/savefig_pdf.ipynb` & `anypy-0.1.1/notebooks/recipes/savefig_pdf.ipynb`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/pyproject.toml` & `anypy-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/setup.cfg` & `anypy-0.1.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -12,39 +12,41 @@
 [options]
 zip_safe = False
 include_package_data = True
 package_dir = 
 	=src
 packages = find:
 install_requires = 
-	pandas
-	hydra-core
-	datasets
-	lightning
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = *.txt, *.md
 
 [options.extras_require]
+core = 
+	pandas
+	hydra-core
+	datasets
+	lightning
 docs = 
 	mkdocs
 	mkdocs-material
 	mike
 test = 
 	pytest
 	pytest-cov
 dev = 
 	black
 	flake8
 	isort
 	pre-commit
 	bandit
+	%(core)s
 	%(test)s
 	%(docs)s
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `anypy-0.0.6/src/anypy/benchmark/chrono.py` & `anypy-0.1.1/src/anypy/benchmark/chrono.py`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/src/anypy/data/metadata_dataset_dict.py` & `anypy-0.1.1/src/anypy/data/metadata_dataset_dict.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         num_shards: Optional[Dict[str, int]] = None,
         num_proc: Optional[int] = None,
         storage_options: Optional[dict] = None,
     ):
         Path(dataset_dict_path).mkdir(exist_ok=True, parents=True)
         self.save_metadata(Path(dataset_dict_path) / f"{CUSTOM_METADATA_KEY}.json")
         super().save_to_disk(
-            dataset_dict_path,
+            str(dataset_dict_path),
             fs=fs,
             max_shard_size=max_shard_size,
             num_shards=num_shards,
             num_proc=num_proc,
             storage_options=storage_options,
         )
 
@@ -61,15 +61,15 @@
         dataset_dict_path: PathLike,
         fs="deprecated",
         keep_in_memory: Optional[bool] = None,
         storage_options: Optional[dict] = None,
     ) -> "MetadataDatasetDict":
         dataset = MetadataDatasetDict(
             DatasetDict.load_from_disk(
-                dataset_dict_path,
+                str(dataset_dict_path),
                 fs=fs,
                 keep_in_memory=keep_in_memory,
                 storage_options=storage_options,
             )
         )
         dataset[CUSTOM_METADATA_KEY] = json.load(open(Path(dataset_dict_path) / f"{CUSTOM_METADATA_KEY}.json"))
```

### Comparing `anypy-0.0.6/src/anypy/nn/blocks.py` & `anypy-0.1.1/src/anypy/nn/blocks.py`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/src/anypy/nn/dyncnn.py` & `anypy-0.1.1/src/anypy/nn/dyncnn.py`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/src/anypy/nn/utils.py` & `anypy-0.1.1/src/anypy/nn/utils.py`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/src/anypy.egg-info/PKG-INFO` & `anypy-0.1.1/src/anypy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: anypy
-Version: 0.0.6
+Version: 0.1.1
 Summary: A collection of python utilities, without hard dependencies
 Home-page: https://github.com/lucmos/anypy
 Author: Luca Moschella
 Author-email: luca.moschella94@gmail.com
 License: MIT Licence
 Keywords: python
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Provides-Extra: core
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # Generic Python Tools & Utilities
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1 Name: anypy Version: 0.0.6 Summary: A collection of
+Metadata-Version: 2.1 Name: anypy Version: 0.1.1 Summary: A collection of
 python utilities, without hard dependencies Home-page: https://github.com/
 lucmos/anypy Author: Luca Moschella Author-email: luca.moschella94@gmail.com
 License: MIT Licence Keywords: python Platform: UNKNOWN Description-Content-
-Type: text/markdown Provides-Extra: docs Provides-Extra: test Provides-Extra:
-dev License-File: LICENSE # Generic Python Tools & Utilities
+Type: text/markdown Provides-Extra: core Provides-Extra: docs Provides-Extra:
+test Provides-Extra: dev License-File: LICENSE # Generic Python Tools &
+Utilities
                    _[_P_y_P_i_]_[_P_y_P_i_]_[_C_I_]_[_D_o_c_s_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
 A collection of python utilities, without hard dependencies ## Installation
 ```bash pip install anypy ``` ## Quickstart [comment]: <> (> Fill me!) ##
 Development installation Setup the development environment: ```bash git clone
 git@github.com:lucmos/anypy.git cd anypy conda env create -f env.yaml conda
 activate anypy pre-commit install ``` Run the tests: ```bash pre-commit run --
 all-files pytest -v ``` ### Update the dependencies Re-install the project in
```

### Comparing `anypy-0.0.6/src/anypy.egg-info/SOURCES.txt` & `anypy-0.1.1/src/anypy.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 setup.py
 .github/workflows/publish.yml
 .github/workflows/test_suite.yml
 docs/index.md
 docs/overrides/main.html
 notebooks/recipes/hydraconf_notebook.ipynb
 notebooks/recipes/savefig_pdf.ipynb
+notebooks/recipes/savefig_sns_pdf.ipynb
 src/anypy/__init__.py
 src/anypy/_version.py
 src/anypy.egg-info/PKG-INFO
 src/anypy.egg-info/SOURCES.txt
 src/anypy.egg-info/dependency_links.txt
 src/anypy.egg-info/not-zip-safe
 src/anypy.egg-info/requires.txt
```

### Comparing `anypy-0.0.6/tests/benchmark/test_chrono.py` & `anypy-0.1.1/tests/benchmark/test_chrono.py`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/tests/data/test_metadata_dataset_dict.py` & `anypy-0.1.1/tests/data/test_metadata_dataset_dict.py`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/tests/latex/test_dataframe.py` & `anypy-0.1.1/tests/latex/test_dataframe.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,27 @@
+from functools import partial
+
 import numpy as np
 import pandas as pd
 
-from anypy.latex import df2table_meanstd
+from anypy.latex import default_meanstd_formatter, df2table_meanstd
 
 
 def test_df2table_meanstd():
     np.random.seed(42)
     df = pd.DataFrame({"model": ["a"] * 100, "score": np.random.randn(100)})
     _, latex_table = df2table_meanstd(
-        df, rows=["model"], metrics=["score"], label_mapping={"a": "My Cool Model"}, caption="Test", precision=3
+        df,
+        rows=["model"],
+        columns=None,
+        metrics=["score"],
+        meanstd_formatter=partial(default_meanstd_formatter, precision=3),
+        label_mapping={"a": "My Cool Model"},
+        caption="Test",
+        label="Test",
     )
     gt_table = r"""\begin{table}
 \caption{Test}
 \label{Test}
 \begin{tabular}{ll}
 \toprule
  & meanstd \\
```

### Comparing `anypy-0.0.6/tests/nn/test_blocks.py` & `anypy-0.1.1/tests/nn/test_blocks.py`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/tests/nn/test_dyncnn.py` & `anypy-0.1.1/tests/nn/test_dyncnn.py`

 * *Files identical despite different names*

### Comparing `anypy-0.0.6/tests/nn/test_utils.py` & `anypy-0.1.1/tests/nn/test_utils.py`

 * *Files identical despite different names*

