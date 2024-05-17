# Comparing `tmp/nias-0.0.1.tar.gz` & `tmp/nias-0.0.1.dev0.tar.gz`

## Comparing `nias-0.0.1.tar` & `nias-0.0.1.dev0.tar`

### file list

```diff
@@ -1,26 +1,7 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 nias-0.0.1/docs/.gitignore
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 nias-0.0.1/docs/conf.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nias-0.0.1/docs/index.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 nias-0.0.1/docs/notebook1.ipynb
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nias-0.0.1/docs/notebook2.md
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 nias-0.0.1/src/nias/__init__.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 nias-0.0.1/src/nias/exceptions.py
--rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 nias-0.0.1/src/nias/interfaces.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 nias-0.0.1/src/nias/base/__init__.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 nias-0.0.1/src/nias/base/linear_solvers.py
--rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 nias-0.0.1/src/nias/base/operators.py
--rw-r--r--   0        0        0    12886 2020-02-02 00:00:00.000000 nias-0.0.1/src/nias/base/vectorarrays.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 nias-0.0.1/src/nias/bindings/__init__.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 nias-0.0.1/src/nias/bindings/numpy/__init__.py
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 nias-0.0.1/src/nias/bindings/numpy/linear_solvers.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 nias-0.0.1/src/nias/bindings/numpy/operators.py
--rw-r--r--   0        0        0    10573 2020-02-02 00:00:00.000000 nias-0.0.1/src/nias/bindings/numpy/vectorarrays.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 nias-0.0.1/src/nias/linalg/__init__.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 nias-0.0.1/src/nias/linalg/eigs.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 nias-0.0.1/src/nias/linalg/gram_schmidt.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 nias-0.0.1/src/nias/linalg/svd.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 nias-0.0.1/.gitignore
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 nias-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 nias-0.0.1/README.md
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 nias-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 nias-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nias-0.0.1.dev0/src/nias/__init__.py
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 nias-0.0.1.dev0/src/nias/interfaces.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 nias-0.0.1.dev0/.gitignore
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 nias-0.0.1.dev0/LICENSE.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 nias-0.0.1.dev0/README.md
+-rw-r--r--   0        0        0     5080 2020-02-02 00:00:00.000000 nias-0.0.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 nias-0.0.1.dev0/PKG-INFO
```

### Comparing `nias-0.0.1/.gitignore` & `nias-0.0.1.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `nias-0.0.1/LICENSE.txt` & `nias-0.0.1.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nias-0.0.1/pyproject.toml` & `nias-0.0.1.dev0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -23,33 +23,16 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering :: Mathematics",
 ]
 dependencies = [
   "numpy>=1.20.3,!=1.25.0,<2", # 1.25.0 crashes CI, >=2 breaks API
   "scipy>=1.5.4",
-  "typer",
 ]
 
-[project.optional-dependencies]
-tests = [
-  "pytest-cov",
-  "pytest>=7.2.1",
-]
-docs = [
-  "sphinx",
-  "myst-nb",
-]
-
-[tool.coverage.run]
-relative_files = true
-source = [
-  "src/nias",
-  "demos",
-]
 
 [tool.hatch.build.targets.sdist]
 include = [
   "/src",
   "/docs",
   "CITATION.cff",
 ]
@@ -58,19 +41,14 @@
 packages = [
   "/src/nias",
 ]
 
 [tool.hatch.version]
 path = "src/nias/__init__.py"
 
-[tool.pytest.ini_options]
-pythonpath = "src"
-testpaths = "tests"
-python_files = "*.py"
-
 [tool.ruff]
 src = ["src"] # this makes isort behave nicely
 line-length = 120
 select = [
   "F", # Pyflakes
   "W", # pycodestyle warning
   "E", # pycodestyle error
@@ -146,14 +124,20 @@
 "scipy.linalg" = "spla"
 
 [tool.ruff.flake8-quotes]
 inline-quotes = "single"
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"] # module imported but unused
+"docs/source/try_on_binder.py" = ["N801"] # class name CapWords convention
+"src/pymor/algorithms/genericsolvers.py" = ["TD001"] # invalid TODO tag (XXX)
+"src/pymor/algorithms/rules.py" = ["N801", "N805"] # class name CapWords convention, first argument should be `self`
+"src/pymor/analyticalproblems/expressions.py" = ["N801"] # class name CapWords convention
+"src/pymor/basic.py" = ["F401"] # ununsed imports
+"src/pymordemos/*" = ["F403", "F405"] # undefined import due to pymor.basic functionality
 
 [tool.ruff.pycodestyle]
 max-doc-length = 100
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
```

### Comparing `nias-0.0.1/PKG-INFO` & `nias-0.0.1.dev0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nias
-Version: 0.0.1
+Version: 0.0.1.dev0
 Summary: Numerics In Abstract Spaces
 Author-email: NIAS developers <main.developers@pymor.org>
 Maintainer-email: Stephan Rave <stephan.rave@uni-muenster.de>
 License: Copyright NIAS developers and contributors. All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the
         following conditions are met:
@@ -28,21 +28,12 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Requires-Dist: numpy!=1.25.0,<2,>=1.20.3
 Requires-Dist: scipy>=1.5.4
-Requires-Dist: typer
-Provides-Extra: docs
-Requires-Dist: myst-nb; extra == 'docs'
-Requires-Dist: sphinx; extra == 'docs'
-Provides-Extra: tests
-Requires-Dist: pytest-cov; extra == 'tests'
-Requires-Dist: pytest>=7.2.1; extra == 'tests'
 Description-Content-Type: text/markdown
 
-# Numerics In Abstract Spaces
+# Numerics In Abstract Spaces - Base Libary
 
-[![PyPI](https://img.shields.io/pypi/v/nias.svg)](https://pypi.python.org/pypi/nias)
-[![Documentation Status](https://readthedocs.org/projects/nias/badge/?version=latest)](https://nias.readthedocs.io/en/latest/?badge=latest)
-[![Tests](https://github.com/nias-project/nias/actions/workflows/tests.yml/badge.svg)](https://github.com/nias-project/nias/actions/workflows/tests.yml)
+This library contains the core interfaces and backend bindings.
```

