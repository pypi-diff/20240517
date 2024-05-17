# Comparing `tmp/python_cmethods-2.2.2.tar.gz` & `tmp/python_cmethods-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_cmethods-2.2.2.tar", last modified: Tue May  7 05:38:03 2024, max compression
+gzip compressed data, was "python_cmethods-2.2.3.tar", last modified: Fri May 17 14:33:04 2024, max compression
```

## Comparing `python_cmethods-2.2.2.tar` & `python_cmethods-2.2.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:38:03.277833 python_cmethods-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:38:03.269832 python_cmethods-2.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:38:03.273833 python_cmethods-2.2.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.github/dependabot.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:38:03.273833 python_cmethods-2.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.github/workflows/_build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.github/workflows/_build_doc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.github/workflows/_codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.github/workflows/_codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.github/workflows/_pre_commit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.github/workflows/_pypi_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.github/workflows/_pypi_test_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.github/workflows/_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.github/workflows/cicd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.github/workflows/scorecard.yml
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13733 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    32891 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    53917 2024-05-07 05:38:03.277833 python_cmethods-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13794 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:38:03.273833 python_cmethods-2.2.2/cmethods/
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/cmethods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 05:38:03.000000 python_cmethods-2.2.2/cmethods/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/cmethods/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9253 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/cmethods/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/cmethods/scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/cmethods/static.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/cmethods/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/cmethods/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:38:03.277833 python_cmethods-2.2.2/python_cmethods.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    53917 2024-05-07 05:38:03.000000 python_cmethods-2.2.2/python_cmethods.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-07 05:38:03.000000 python_cmethods-2.2.2/python_cmethods.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 05:38:03.000000 python_cmethods-2.2.2/python_cmethods.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 05:38:03.000000 python_cmethods-2.2.2/python_cmethods.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-07 05:38:03.000000 python_cmethods-2.2.2/python_cmethods.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 05:38:03.000000 python_cmethods-2.2.2/python_cmethods.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 05:38:03.277833 python_cmethods-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 05:37:56.000000 python_cmethods-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:04.589160 python_cmethods-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:04.581160 python_cmethods-2.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:04.581160 python_cmethods-2.2.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/dependabot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:04.585160 python_cmethods-2.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/_build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/_build_doc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/_codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/_codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/_pre_commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/_pypi_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/_pypi_test_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/cicd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.github/workflows/scorecard.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13733 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32891 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    54246 2024-05-17 14:33:04.589160 python_cmethods-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14083 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:04.585160 python_cmethods-2.2.3/cmethods/
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/cmethods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 14:33:04.000000 python_cmethods-2.2.3/cmethods/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/cmethods/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9253 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/cmethods/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/cmethods/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/cmethods/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/cmethods/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/cmethods/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:04.585160 python_cmethods-2.2.3/python_cmethods.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    54246 2024-05-17 14:33:04.000000 python_cmethods-2.2.3/python_cmethods.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-17 14:33:04.000000 python_cmethods-2.2.3/python_cmethods.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:33:04.000000 python_cmethods-2.2.3/python_cmethods.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-17 14:33:04.000000 python_cmethods-2.2.3/python_cmethods.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-17 14:33:04.000000 python_cmethods-2.2.3/python_cmethods.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 14:33:04.000000 python_cmethods-2.2.3/python_cmethods.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:33:04.589160 python_cmethods-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-17 14:32:55.000000 python_cmethods-2.2.3/setup.py
```

### Comparing `python_cmethods-2.2.2/.gitattributes` & `python_cmethods-2.2.3/.gitattributes`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/.github/ISSUE_TEMPLATE/bug_report.md` & `python_cmethods-2.2.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/.github/ISSUE_TEMPLATE/feature_request.md` & `python_cmethods-2.2.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/.github/codecov.yml` & `python_cmethods-2.2.3/.github/codecov.yml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/.github/workflows/_build.yaml` & `python_cmethods-2.2.3/.github/workflows/_build.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 permissions: read-all
 
 jobs:
   Build:
     runs-on: ${{ inputs.os }}
     steps:
       - name: Checkout repository
-        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
+        uses: actions/checkout@44c2b7a8a4ea60a981eaca3cf939b5f4305c123b # v4.1.5
         with:
           fetch-depth: 0 # IMPORTANT: otherwise the current tag does not get fetched and the build version gets worse
 
       - name: Set up Python ${{ inputs.python-version }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d # v5.1.0
         with:
           python-version: ${{ inputs.python-version }}
```

### Comparing `python_cmethods-2.2.2/.github/workflows/_build_doc.yaml` & `python_cmethods-2.2.3/.github/workflows/_build_doc.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -20,22 +20,23 @@
 permissions: read-all
 
 jobs:
   Build:
     runs-on: ${{ inputs.os }}
     steps:
       - name: Checkout repository
-        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
+        uses: actions/checkout@44c2b7a8a4ea60a981eaca3cf939b5f4305c123b # v4.1.5
 
       - name: Set up Python ${{ inputs.python-version }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d # v5.1.0
         with:
           python-version: ${{ inputs.python-version }}
 
       - name: Install dependencies
         run: |
-          python -m pip install --upgrade pip
-          python -m pip install .
-          python -m pip install -r doc/requirements.txt
+          python -m pip install --user --upgrade pip
+          python -m pip install --user .
+          python -m pip install --user -r doc/requirements.txt
+          DEBIAN_FRONTEND=noninteractive sudo apt-get install -y pandoc
 
       - name: Build the documentation
         run: cd doc && make html
```

### Comparing `python_cmethods-2.2.2/.github/workflows/_codecov.yaml` & `python_cmethods-2.2.3/.github/workflows/_codecov.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     runs-on: ${{ inputs.os }}
     env:
       OS: ${{ inputs.os }}
       PYTHON: ${{ inputs.python-version }}
 
     steps:
       - name: Checkout repository
-        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
+        uses: actions/checkout@44c2b7a8a4ea60a981eaca3cf939b5f4305c123b # v4.1.5
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d # v5.1.0
         with:
           python-version: ${{ inputs.python-version }}
 
       - name: Install dependencies
```

### Comparing `python_cmethods-2.2.2/.github/workflows/_codeql.yaml` & `python_cmethods-2.2.3/.github/workflows/_codeql.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     #   matrix:
     #     language: ["python"]
     # CodeQL supports [ 'cpp', 'csharp', 'go', 'java', 'javascript', 'python', 'ruby' ]
     # Learn more about CodeQL language support at https://aka.ms/codeql-docs/language-support
 
     steps:
       - name: Checkout repository
-        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
+        uses: actions/checkout@44c2b7a8a4ea60a981eaca3cf939b5f4305c123b # v4.1.5
 
       # Initializes the CodeQL tools for scanning.
       - name: Initialize CodeQL
         uses: github/codeql-action/init@v3
         with:
           languages: python
           # If you wish to specify custom queries, you can do so here or in a config file.
```

### Comparing `python_cmethods-2.2.2/.github/workflows/_pypi_publish.yaml` & `python_cmethods-2.2.3/.github/workflows/_pypi_publish.yaml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/.github/workflows/_pypi_test_publish.yaml` & `python_cmethods-2.2.3/.github/workflows/_pypi_test_publish.yaml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/.github/workflows/_test.yaml` & `python_cmethods-2.2.3/.github/workflows/_test.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 jobs:
   Test:
     name: Test ${{ inputs.os }} ${{ inputs.python-version }}
     runs-on: ${{ inputs.os }}
     steps:
       - name: Checkout repository
-        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
+        uses: actions/checkout@44c2b7a8a4ea60a981eaca3cf939b5f4305c123b # v4.1.5
 
       - name: Set up Python ${{ inputs.python-version }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d # v5.1.0
         with:
           python-version: ${{ inputs.python-version }}
 
       - name: Install dependencies
```

### Comparing `python_cmethods-2.2.2/.github/workflows/cicd.yaml` & `python_cmethods-2.2.3/.github/workflows/cicd.yaml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/.github/workflows/scorecard.yml` & `python_cmethods-2.2.3/.github/workflows/scorecard.yml`

 * *Files 4% similar despite different names*

```diff
@@ -28,20 +28,20 @@
       id-token: write
       # Uncomment the permissions below if installing in a private repository.
       # contents: read
       # actions: read
 
     steps:
       - name: "Checkout code"
-        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
+        uses: actions/checkout@44c2b7a8a4ea60a981eaca3cf939b5f4305c123b # v4.1.5
         with:
           persist-credentials: false
 
       - name: "Run analysis"
-        uses: ossf/scorecard-action@0864cf19026789058feabb7e87baa5f140aac736 # v2.3.1
+        uses: ossf/scorecard-action@dc50aa9510b46c811795eb24b2f1ba02a914e534 # v2.3.3
         with:
           results_file: results.sarif
           results_format: sarif
           # (Optional) "write" PAT token. Uncomment the `repo_token` line below if:
           # - you want to enable the Branch-Protection check on a *public* repository, or
           # - you are installing Scorecard on a *private* repository
           # To create the PAT, follow the steps in https://github.com/ossf/scorecard-action#authentication-with-pat.
```

### Comparing `python_cmethods-2.2.2/.gitignore` & `python_cmethods-2.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/.pre-commit-config.yaml` & `python_cmethods-2.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/CHANGELOG.md` & `python_cmethods-2.2.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/LICENSE` & `python_cmethods-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/Makefile` & `python_cmethods-2.2.3/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 	$(PYTHON) -m build .
 
 ## dev		Installs the package in edit mode
 ##
 .PHONY: dev
 dev:
 	@git lfs install
-	$(PYTHON) -m pip install -e ".[dev,test]"
+	$(PYTHON) -m pip install -e ".[dev,test,jupyter,examples]"
 
 ## install		Install the package
 ##
 .PHONY: install
 install:
 	$(PYTHON) -m pip install .
```

### Comparing `python_cmethods-2.2.2/PKG-INFO` & `python_cmethods-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cmethods
-Version: 2.2.2
+Version: 2.2.3
 Summary: A collection of bias correction techniques written in Python - for climate sciences.
 Author-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 Maintainer-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -664,14 +664,15 @@
 Provides-Extra: jupyter
 Requires-Dist: venv-kernel; extra == "jupyter"
 Provides-Extra: dev
 Requires-Dist: setuptools_scm; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
+Requires-Dist: nbsphinx; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: ruff==0.3.5; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
@@ -686,15 +687,15 @@
 # python-cmethods
 
 <div align="center">
 
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/btschwertfeger/python-cmethods)
 [![Generic badge](https://img.shields.io/badge/python-3.8_|_3.9_|_3.10_|_3.11|_3.12-blue.svg)](https://shields.io/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-orange.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![Downloads](https://pepy.tech/badge/python-cmethods)](https://pepy.tech/project/python-cmethods)
+[![PyPI Downloads](https://pepy.tech/badge/python-cmethods)](https://pepy.tech/project/python-cmethods)
 
 [![CI/CD](https://github.com/btschwertfeger/python-cmethods/actions/workflows/cicd.yaml/badge.svg?branch=master)](https://github.com/btschwertfeger/python-cmethods/actions/workflows/cicd.yaml)
 [![codecov](https://codecov.io/github/btschwertfeger/python-cmethods/branch/master/graph/badge.svg?token=OSO4PAABPD)](https://codecov.io/github/btschwertfeger/python-cmethods)
 
 [![OpenSSF ScoreCard](https://img.shields.io/ossf-scorecard/github.com/btschwertfeger/python-cmethods?label=openssf%20scorecard&style=flat)](https://securityscorecards.dev/viewer/?uri=github.com/btschwertfeger/python-cmethods)
 [![OpenSSF Best Practices](https://www.bestpractices.dev/projects/8666/badge)](https://www.bestpractices.dev/projects/8666)
 
@@ -789,14 +790,18 @@
 - Detrended Quantile Mapping
 - Quantile Delta Mapping
 
 Please refer to the official documentation for more information about these
 methods as well as sample scripts:
 https://python-cmethods.readthedocs.io/en/stable/
 
+## Best Practices and important Notes
+
+- The training data should have the same temporal resolution.
+
 - Except for the variance scaling, all methods can be applied on stochastic and
   non-stochastic climate variables. Variance scaling can only be applied on
   non-stochastic climate variables.
 
   - Non-stochastic climate variables are those that can be predicted with
     relative certainty based on factors such as location, elevation, and season.
     Examples of non-stochastic climate variables include air temperature, air
@@ -825,14 +830,18 @@
 > For optimal compatibility on macOS, ensure that 'hdf5' and 'netcdf' are
 > pre-installed using Homebrew (`brew install hdf5 netcdf`).
 
 ```bash
 python3 -m pip install python-cmethods
 ```
 
+The package is also available via conda-forge. See
+[conda-forge/python_cmethods-feedstock](https://github.com/conda-forge/python_cmethods-feedstock/tree/main) for more
+information.
+
 <a name="examples"></a>
 
 ## 4. CLI Usage
 
 The python-cmethods package provides a command-line interface for applying
 various bias correction methods out of the box.
```

### Comparing `python_cmethods-2.2.2/README.md` & `python_cmethods-2.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # python-cmethods
 
 <div align="center">
 
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/btschwertfeger/python-cmethods)
 [![Generic badge](https://img.shields.io/badge/python-3.8_|_3.9_|_3.10_|_3.11|_3.12-blue.svg)](https://shields.io/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-orange.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![Downloads](https://pepy.tech/badge/python-cmethods)](https://pepy.tech/project/python-cmethods)
+[![PyPI Downloads](https://pepy.tech/badge/python-cmethods)](https://pepy.tech/project/python-cmethods)
 
 [![CI/CD](https://github.com/btschwertfeger/python-cmethods/actions/workflows/cicd.yaml/badge.svg?branch=master)](https://github.com/btschwertfeger/python-cmethods/actions/workflows/cicd.yaml)
 [![codecov](https://codecov.io/github/btschwertfeger/python-cmethods/branch/master/graph/badge.svg?token=OSO4PAABPD)](https://codecov.io/github/btschwertfeger/python-cmethods)
 
 [![OpenSSF ScoreCard](https://img.shields.io/ossf-scorecard/github.com/btschwertfeger/python-cmethods?label=openssf%20scorecard&style=flat)](https://securityscorecards.dev/viewer/?uri=github.com/btschwertfeger/python-cmethods)
 [![OpenSSF Best Practices](https://www.bestpractices.dev/projects/8666/badge)](https://www.bestpractices.dev/projects/8666)
 
@@ -104,14 +104,18 @@
 - Detrended Quantile Mapping
 - Quantile Delta Mapping
 
 Please refer to the official documentation for more information about these
 methods as well as sample scripts:
 https://python-cmethods.readthedocs.io/en/stable/
 
+## Best Practices and important Notes
+
+- The training data should have the same temporal resolution.
+
 - Except for the variance scaling, all methods can be applied on stochastic and
   non-stochastic climate variables. Variance scaling can only be applied on
   non-stochastic climate variables.
 
   - Non-stochastic climate variables are those that can be predicted with
     relative certainty based on factors such as location, elevation, and season.
     Examples of non-stochastic climate variables include air temperature, air
@@ -140,14 +144,18 @@
 > For optimal compatibility on macOS, ensure that 'hdf5' and 'netcdf' are
 > pre-installed using Homebrew (`brew install hdf5 netcdf`).
 
 ```bash
 python3 -m pip install python-cmethods
 ```
 
+The package is also available via conda-forge. See
+[conda-forge/python_cmethods-feedstock](https://github.com/conda-forge/python_cmethods-feedstock/tree/main) for more
+information.
+
 <a name="examples"></a>
 
 ## 4. CLI Usage
 
 The python-cmethods package provides a command-line interface for applying
 various bias correction methods out of the box.
```

### Comparing `python_cmethods-2.2.2/SECURITY.md` & `python_cmethods-2.2.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/cmethods/__init__.py` & `python_cmethods-2.2.3/cmethods/__init__.py`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/cmethods/core.py` & `python_cmethods-2.2.3/cmethods/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,46 +56,46 @@
         if not len(kwargs["input_core_dims"]) == 3 or any(
             not isinstance(value, str) for value in kwargs["input_core_dims"].values()
         ):
             raise ValueError(
                 'input_core_dims must have three key-value pairs like: {"obs": "time", "simh": "time", "simp": "time"}',
             )
 
-        input_core_dims = kwargs["input_core_dims"]
+        input_core_dims = kwargs.pop("input_core_dims")
     else:
         input_core_dims = {"obs": "time", "simh": "time", "simp": "time"}
 
     result: XRData = xr.apply_ufunc(
         __METHODS_FUNC__[method],
         obs,
         simh,
-        # Need to spoof a fake time axis since 'time' coord on full dataset is different
-        # than 'time' coord on training dataset.
+        # Need to spoof a fake time axis since 'time' coord on full dataset is
+        # different than 'time' coord on training dataset.
         simp.rename({input_core_dims["simp"]: "__t_simp__"}),
         dask="parallelized",
         vectorize=True,
-        # This will vectorize over the time dimension, so will submit each grid cell
-        # independently
+        # This will vectorize over the time dimension, so will submit each grid
+        # cell independently
         input_core_dims=[
             [input_core_dims["obs"]],
             [input_core_dims["simh"]],
             ["__t_simp__"],
         ],
         # Need to denote that the final output dataset will be labeled with the
         # spoofed time coordinate
         output_core_dims=[["__t_simp__"]],
         kwargs=dict(kwargs),
     )
 
     # Rename to proper coordinate name.
     result = result.rename({"__t_simp__": input_core_dims["simp"]})
 
-    # ufunc will put the core dimension to the end (time), so want to preserve original
-    # order where time is commonly first.
-    return result.transpose(*obs.dims)
+    # ufunc will put the core dimension to the end (time), so want to preserve
+    # original order where time is commonly first.
+    return result.transpose(*obs.rename({input_core_dims["obs"]: input_core_dims["simp"]}).dims)
 
 
 def adjust(
     method: str,
     obs: XRData,
     simh: XRData,
     simp: XRData,
```

### Comparing `python_cmethods-2.2.2/cmethods/distribution.py` & `python_cmethods-2.2.3/cmethods/distribution.py`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/cmethods/scaling.py` & `python_cmethods-2.2.3/cmethods/scaling.py`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/cmethods/static.py` & `python_cmethods-2.2.3/cmethods/static.py`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/cmethods/utils.py` & `python_cmethods-2.2.3/cmethods/utils.py`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.2/pyproject.toml` & `python_cmethods-2.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 dev = [
   # building
   "setuptools_scm",
   "build",
   # documentation
   "sphinx",
   "sphinx-rtd-theme",
+  "nbsphinx",
   # linting
   "pylint",
   "flake8",
   "ruff==0.3.5",
   # typing
   "mypy",
 ]
```

### Comparing `python_cmethods-2.2.2/python_cmethods.egg-info/PKG-INFO` & `python_cmethods-2.2.3/python_cmethods.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cmethods
-Version: 2.2.2
+Version: 2.2.3
 Summary: A collection of bias correction techniques written in Python - for climate sciences.
 Author-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 Maintainer-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -664,14 +664,15 @@
 Provides-Extra: jupyter
 Requires-Dist: venv-kernel; extra == "jupyter"
 Provides-Extra: dev
 Requires-Dist: setuptools_scm; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
+Requires-Dist: nbsphinx; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: ruff==0.3.5; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
@@ -686,15 +687,15 @@
 # python-cmethods
 
 <div align="center">
 
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/btschwertfeger/python-cmethods)
 [![Generic badge](https://img.shields.io/badge/python-3.8_|_3.9_|_3.10_|_3.11|_3.12-blue.svg)](https://shields.io/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-orange.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![Downloads](https://pepy.tech/badge/python-cmethods)](https://pepy.tech/project/python-cmethods)
+[![PyPI Downloads](https://pepy.tech/badge/python-cmethods)](https://pepy.tech/project/python-cmethods)
 
 [![CI/CD](https://github.com/btschwertfeger/python-cmethods/actions/workflows/cicd.yaml/badge.svg?branch=master)](https://github.com/btschwertfeger/python-cmethods/actions/workflows/cicd.yaml)
 [![codecov](https://codecov.io/github/btschwertfeger/python-cmethods/branch/master/graph/badge.svg?token=OSO4PAABPD)](https://codecov.io/github/btschwertfeger/python-cmethods)
 
 [![OpenSSF ScoreCard](https://img.shields.io/ossf-scorecard/github.com/btschwertfeger/python-cmethods?label=openssf%20scorecard&style=flat)](https://securityscorecards.dev/viewer/?uri=github.com/btschwertfeger/python-cmethods)
 [![OpenSSF Best Practices](https://www.bestpractices.dev/projects/8666/badge)](https://www.bestpractices.dev/projects/8666)
 
@@ -789,14 +790,18 @@
 - Detrended Quantile Mapping
 - Quantile Delta Mapping
 
 Please refer to the official documentation for more information about these
 methods as well as sample scripts:
 https://python-cmethods.readthedocs.io/en/stable/
 
+## Best Practices and important Notes
+
+- The training data should have the same temporal resolution.
+
 - Except for the variance scaling, all methods can be applied on stochastic and
   non-stochastic climate variables. Variance scaling can only be applied on
   non-stochastic climate variables.
 
   - Non-stochastic climate variables are those that can be predicted with
     relative certainty based on factors such as location, elevation, and season.
     Examples of non-stochastic climate variables include air temperature, air
@@ -825,14 +830,18 @@
 > For optimal compatibility on macOS, ensure that 'hdf5' and 'netcdf' are
 > pre-installed using Homebrew (`brew install hdf5 netcdf`).
 
 ```bash
 python3 -m pip install python-cmethods
 ```
 
+The package is also available via conda-forge. See
+[conda-forge/python_cmethods-feedstock](https://github.com/conda-forge/python_cmethods-feedstock/tree/main) for more
+information.
+
 <a name="examples"></a>
 
 ## 4. CLI Usage
 
 The python-cmethods package provides a command-line interface for applying
 various bias correction methods out of the box.
```

### Comparing `python_cmethods-2.2.2/python_cmethods.egg-info/SOURCES.txt` & `python_cmethods-2.2.3/python_cmethods.egg-info/SOURCES.txt`

 * *Files identical despite different names*

