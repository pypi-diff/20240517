# Comparing `tmp/precommend-0.3.2.tar.gz` & `tmp/precommend-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precommend-0.3.2.tar", last modified: Tue May 14 08:50:55 2024, max compression
+gzip compressed data, was "precommend-0.3.3.tar", last modified: Fri May 17 12:33:09 2024, max compression
```

## Comparing `precommend-0.3.2.tar` & `precommend-0.3.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:55.821545 precommend-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:55.817545 precommend-0.3.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 08:50:49.000000 precommend-0.3.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:55.817545 precommend-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-14 08:50:49.000000 precommend-0.3.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-14 08:50:49.000000 precommend-0.3.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-14 08:50:49.000000 precommend-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-14 08:50:49.000000 precommend-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 08:50:49.000000 precommend-0.3.2/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-14 08:50:49.000000 precommend-0.3.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 08:50:49.000000 precommend-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-14 08:50:55.821545 precommend-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-14 08:50:49.000000 precommend-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-14 08:50:49.000000 precommend-0.3.2/bump_identify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:55.817545 precommend-0.3.2/precommend/
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-14 08:50:49.000000 precommend-0.3.2/precommend/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 08:50:49.000000 precommend-0.3.2/precommend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-14 08:50:49.000000 precommend-0.3.2/precommend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 08:50:55.000000 precommend-0.3.2/precommend/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-14 08:50:49.000000 precommend-0.3.2/precommend/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-14 08:50:49.000000 precommend-0.3.2/precommend/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:55.821545 precommend-0.3.2/precommend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-14 08:50:55.000000 precommend-0.3.2/precommend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-14 08:50:55.000000 precommend-0.3.2/precommend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:50:55.000000 precommend-0.3.2/precommend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 08:50:55.000000 precommend-0.3.2/precommend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 08:50:55.000000 precommend-0.3.2/precommend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 08:50:55.000000 precommend-0.3.2/precommend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-14 08:50:49.000000 precommend-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:50:55.821545 precommend-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 08:50:49.000000 precommend-0.3.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-14 08:50:49.000000 precommend-0.3.2/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:55.817545 precommend-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:49.000000 precommend-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-14 08:50:49.000000 precommend-0.3.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:55.813545 precommend-0.3.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:55.817545 precommend-0.3.2/tests/data/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 08:50:49.000000 precommend-0.3.2/tests/data/cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:49.000000 precommend-0.3.2/tests/data/cpp/test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:55.817545 precommend-0.3.2/tests/data/generic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:55.817545 precommend-0.3.2/tests/data/generic/.github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:49.000000 precommend-0.3.2/tests/data/generic/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:55.817545 precommend-0.3.2/tests/data/generic/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:49.000000 precommend-0.3.2/tests/data/generic/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:49.000000 precommend-0.3.2/tests/data/generic/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:55.821545 precommend-0.3.2/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:49.000000 precommend-0.3.2/tests/data/python/foo.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:50:49.000000 precommend-0.3.2/tests/data/python/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-14 08:50:49.000000 precommend-0.3.2/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:33:09.066347 precommend-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:33:09.062348 precommend-0.3.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-17 12:32:09.000000 precommend-0.3.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:33:09.062348 precommend-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-17 12:32:09.000000 precommend-0.3.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-17 12:32:09.000000 precommend-0.3.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-17 12:32:09.000000 precommend-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-17 12:32:09.000000 precommend-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-17 12:32:09.000000 precommend-0.3.3/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-17 12:32:09.000000 precommend-0.3.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 12:32:09.000000 precommend-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-17 12:33:09.066347 precommend-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-17 12:32:09.000000 precommend-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-17 12:32:09.000000 precommend-0.3.3/bump_identify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:33:09.062348 precommend-0.3.3/precommend/
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-17 12:32:09.000000 precommend-0.3.3/precommend/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-17 12:32:09.000000 precommend-0.3.3/precommend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-17 12:32:09.000000 precommend-0.3.3/precommend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 12:33:08.000000 precommend-0.3.3/precommend/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-17 12:32:09.000000 precommend-0.3.3/precommend/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-17 12:32:09.000000 precommend-0.3.3/precommend/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:33:09.066347 precommend-0.3.3/precommend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-17 12:33:09.000000 precommend-0.3.3/precommend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-17 12:33:09.000000 precommend-0.3.3/precommend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:33:09.000000 precommend-0.3.3/precommend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-17 12:33:09.000000 precommend-0.3.3/precommend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-17 12:33:09.000000 precommend-0.3.3/precommend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 12:33:09.000000 precommend-0.3.3/precommend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-17 12:32:09.000000 precommend-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 12:33:09.066347 precommend-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-17 12:32:09.000000 precommend-0.3.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-17 12:32:09.000000 precommend-0.3.3/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:33:09.062348 precommend-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:32:09.000000 precommend-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-17 12:32:09.000000 precommend-0.3.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:33:09.058347 precommend-0.3.3/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:33:09.062348 precommend-0.3.3/tests/data/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 12:32:09.000000 precommend-0.3.3/tests/data/cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:32:09.000000 precommend-0.3.3/tests/data/cpp/test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:33:09.062348 precommend-0.3.3/tests/data/generic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:33:09.062348 precommend-0.3.3/tests/data/generic/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:32:09.000000 precommend-0.3.3/tests/data/generic/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:33:09.062348 precommend-0.3.3/tests/data/generic/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:32:09.000000 precommend-0.3.3/tests/data/generic/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:32:09.000000 precommend-0.3.3/tests/data/generic/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:33:09.062348 precommend-0.3.3/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:32:09.000000 precommend-0.3.3/tests/data/python/foo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:32:09.000000 precommend-0.3.3/tests/data/python/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-17 12:32:09.000000 precommend-0.3.3/tests/test_core.py
```

### Comparing `precommend-0.3.2/.github/workflows/ci.yml` & `precommend-0.3.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `precommend-0.3.2/.github/workflows/pypi.yml` & `precommend-0.3.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `precommend-0.3.2/.gitignore` & `precommend-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `precommend-0.3.2/.pre-commit-config.yaml` & `precommend-0.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `precommend-0.3.2/LICENSE.md` & `precommend-0.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `precommend-0.3.2/PKG-INFO` & `precommend-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: precommend
-Version: 0.3.2
+Version: 0.3.3
 Summary: Opinionated initialization of pre-commit configurations
 Maintainer-email: Dominic Kempf <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: COPYING.md
 Requires-Dist: click
 Requires-Dist: identify>=2.5.36
-Requires-Dist: pre-commit>=3.7.0
+Requires-Dist: pre-commit>=3.7.1
 Requires-Dist: ruamel.yaml
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 
 # Welcome to precommend
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `precommend-0.3.2/README.md` & `precommend-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `precommend-0.3.2/bump_identify.py` & `precommend-0.3.3/bump_identify.py`

 * *Files identical despite different names*

### Comparing `precommend-0.3.2/precommend/.pre-commit-config.yaml` & `precommend-0.3.3/precommend/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `precommend-0.3.2/precommend/__main__.py` & `precommend-0.3.3/precommend/__main__.py`

 * *Files identical despite different names*

### Comparing `precommend-0.3.2/precommend/core.py` & `precommend-0.3.3/precommend/core.py`

 * *Files identical despite different names*

### Comparing `precommend-0.3.2/precommend/rules.py` & `precommend-0.3.3/precommend/rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 
 @rule
 def actionlint(ctx):
     if ctx.directory_exists(".github/workflows"):
         return "actionlint"
 
+    if ctx.filename_exists("action.yml"):
+        return "actionlint"
+
 
 @rule
 def shell_fmt_go(ctx):
     if ctx.tag_exists("shell") or ctx.tag_exists("bash"):
         return "shell-fmt-go"
```

### Comparing `precommend-0.3.2/precommend.egg-info/PKG-INFO` & `precommend-0.3.3/precommend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: precommend
-Version: 0.3.2
+Version: 0.3.3
 Summary: Opinionated initialization of pre-commit configurations
 Maintainer-email: Dominic Kempf <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: COPYING.md
 Requires-Dist: click
 Requires-Dist: identify>=2.5.36
-Requires-Dist: pre-commit>=3.7.0
+Requires-Dist: pre-commit>=3.7.1
 Requires-Dist: ruamel.yaml
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 
 # Welcome to precommend
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `precommend-0.3.2/precommend.egg-info/SOURCES.txt` & `precommend-0.3.3/precommend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `precommend-0.3.2/pyproject.toml` & `precommend-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
     "click",
     "identify >= 2.5.36",
-    "pre-commit >= 3.7.0",
+    "pre-commit >= 3.7.1",
     "ruamel.yaml",
 ]
 
 [project.optional-dependencies]
 tests = [
     "pytest",
 ]
```

### Comparing `precommend-0.3.2/tests/test_core.py` & `precommend-0.3.3/tests/test_core.py`

 * *Files identical despite different names*

