# Comparing `tmp/ouro_py-0.0.1.tar.gz` & `tmp/ouro_py-0.0.2.tar.gz`

## Comparing `ouro_py-0.0.1.tar` & `ouro_py-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 ouro_py-0.0.1/ouro/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ouro_py-0.0.1/ouro/ouro.py
--rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 ouro_py-0.0.1/ouro/air/__init__.py
--rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 ouro_py-0.0.1/ouro/earth/__init__.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 ouro_py-0.0.1/ouro/utils/__init__.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 ouro_py-0.0.1/.gitignore
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 ouro_py-0.0.1/README.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 ouro_py-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 ouro_py-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 ouro_py-0.0.2/ouro/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ouro_py-0.0.2/ouro/ouro.py
+-rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 ouro_py-0.0.2/ouro/air/__init__.py
+-rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 ouro_py-0.0.2/ouro/earth/__init__.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 ouro_py-0.0.2/ouro/utils/__init__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 ouro_py-0.0.2/.gitignore
+-rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 ouro_py-0.0.2/README.md
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 ouro_py-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 ouro_py-0.0.2/PKG-INFO
```

### Comparing `ouro_py-0.0.1/ouro/__init__.py` & `ouro_py-0.0.2/ouro/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 
 import logging
 import os
 
 
 import requests
```

### Comparing `ouro_py-0.0.1/ouro/air/__init__.py` & `ouro_py-0.0.2/ouro/air/__init__.py`

 * *Files identical despite different names*

### Comparing `ouro_py-0.0.1/ouro/earth/__init__.py` & `ouro_py-0.0.2/ouro/earth/__init__.py`

 * *Files identical despite different names*

### Comparing `ouro_py-0.0.1/ouro/utils/__init__.py` & `ouro_py-0.0.2/ouro/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ouro_py-0.0.1/.gitignore` & `ouro_py-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ouro_py-0.0.1/README.md` & `ouro_py-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -78,27 +78,27 @@
 
 ### PyPi installation
 
 Install the package (for > Python 3.7):
 
 ```bash
 # with pip
-pip install ouro
+pip install ouro-py
 ```
 
 ### Local installation
 
 You can also install locally after cloning this repo. Install Development mode with `pip install -e`, which makes it so when you edit the source code the changes will be reflected in your python module.
 
 ## Badges
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?label=license)](https://opensource.org/licenses/MIT)
 [![CI](https://github.com/ourofoundation/ouro-py/actions/workflows/ci.yml/badge.svg)](https://github.com/ourofoundation/ouro-py/actions/workflows/ci.yml)
-[![Python](https://img.shields.io/pypi/pyversions/ouro)](https://pypi.org/project/ouro)
-[![Version](https://img.shields.io/pypi/v/ouro?color=%2334D058)](https://pypi.org/project/ouro)
+[![Python](https://img.shields.io/pypi/pyversions/ouro-py)](https://pypi.org/project/ouro-py)
+[![Version](https://img.shields.io/pypi/v/ouro-py?color=%2334D058)](https://pypi.org/project/ouro-py)
 [![Codecov](https://codecov.io/gh/ourofoundation/ouro-py/branch/develop/graph/badge.svg)](https://codecov.io/gh/ourofoundation/ouro-py)
 [![Last commit](https://img.shields.io/github/last-commit/ourofoundation/ouro-py.svg?style=flat)](https://github.com/ourofoundation/ouro-py/commits)
 [![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ourofoundation/ouro-py)](https://github.com/ourofoundation/ouro-py/commits)
 [![Github Stars](https://img.shields.io/github/stars/ourofoundation/ouro-py?style=flat&logo=github)](https://github.com/ourofoundation/ouro-py/stargazers)
 [![Github Forks](https://img.shields.io/github/forks/ourofoundation/ouro-py?style=flat&logo=github)](https://github.com/ourofoundation/ouro-py/network/members)
 [![Github Watchers](https://img.shields.io/github/watchers/ourofoundation/ouro-py?style=flat&logo=github)](https://github.com/ourofoundation/ouro-py)
 [![GitHub contributors](https://img.shields.io/github/contributors/ourofoundation/ouro-py)](https://github.com/ourofoundation/ouro-py/graphs/contributors)
```

### Comparing `ouro_py-0.0.1/pyproject.toml` & `ouro_py-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 dynamic = ["version"]
 description = "Python wrapper for the Ouro API"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.7"
 authors = [{ name = "Matt Moderwell", email = "matt@ouro.foundation" }]
 keywords = ["ouro"]
-classifiers = []
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
 dependencies = [
     "httpx",
     "numpy",
     "pandas",
     "postgrest",
     "python-dotenv",
     "supabase",
@@ -24,9 +28,16 @@
 [project.urls]
 Homepage = "https://github.com/ourofoundation/ouro-py"
 PyPI = "https://pypi.org/project/ouro-py"
 
 [tool.hatch.version]
 path = "ouro/__init__.py"
 
+
+[tool.hatch.build]
+packages = ["/ouro"]
+
+[tool.hatch.build.targets.wheel]
+include = ["/ouro"]
+
 [tool.hatch.build.targets.sdist]
 include = ["/ouro"]
```

### Comparing `ouro_py-0.0.1/PKG-INFO` & `ouro_py-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.3
 Name: ouro-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for the Ouro API
 Project-URL: Homepage, https://github.com/ourofoundation/ouro-py
 Project-URL: PyPI, https://pypi.org/project/ouro-py
 Author-email: Matt Moderwell <matt@ouro.foundation>
 License-Expression: MIT
 Keywords: ouro
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: httpx
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: postgrest
 Requires-Dist: python-dotenv
 Requires-Dist: supabase
@@ -96,27 +99,27 @@
 
 ### PyPi installation
 
 Install the package (for > Python 3.7):
 
 ```bash
 # with pip
-pip install ouro
+pip install ouro-py
 ```
 
 ### Local installation
 
 You can also install locally after cloning this repo. Install Development mode with `pip install -e`, which makes it so when you edit the source code the changes will be reflected in your python module.
 
 ## Badges
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?label=license)](https://opensource.org/licenses/MIT)
 [![CI](https://github.com/ourofoundation/ouro-py/actions/workflows/ci.yml/badge.svg)](https://github.com/ourofoundation/ouro-py/actions/workflows/ci.yml)
-[![Python](https://img.shields.io/pypi/pyversions/ouro)](https://pypi.org/project/ouro)
-[![Version](https://img.shields.io/pypi/v/ouro?color=%2334D058)](https://pypi.org/project/ouro)
+[![Python](https://img.shields.io/pypi/pyversions/ouro-py)](https://pypi.org/project/ouro-py)
+[![Version](https://img.shields.io/pypi/v/ouro-py?color=%2334D058)](https://pypi.org/project/ouro-py)
 [![Codecov](https://codecov.io/gh/ourofoundation/ouro-py/branch/develop/graph/badge.svg)](https://codecov.io/gh/ourofoundation/ouro-py)
 [![Last commit](https://img.shields.io/github/last-commit/ourofoundation/ouro-py.svg?style=flat)](https://github.com/ourofoundation/ouro-py/commits)
 [![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ourofoundation/ouro-py)](https://github.com/ourofoundation/ouro-py/commits)
 [![Github Stars](https://img.shields.io/github/stars/ourofoundation/ouro-py?style=flat&logo=github)](https://github.com/ourofoundation/ouro-py/stargazers)
 [![Github Forks](https://img.shields.io/github/forks/ourofoundation/ouro-py?style=flat&logo=github)](https://github.com/ourofoundation/ouro-py/network/members)
 [![Github Watchers](https://img.shields.io/github/watchers/ourofoundation/ouro-py?style=flat&logo=github)](https://github.com/ourofoundation/ouro-py)
 [![GitHub contributors](https://img.shields.io/github/contributors/ourofoundation/ouro-py)](https://github.com/ourofoundation/ouro-py/graphs/contributors)
```

