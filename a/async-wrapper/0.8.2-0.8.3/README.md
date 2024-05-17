# Comparing `tmp/async_wrapper-0.8.2.tar.gz` & `tmp/async_wrapper-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.8.2.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `async_wrapper-0.8.2.tar` & `async_wrapper-0.8.3.tar`

### file list

```diff
@@ -1,17 +1,48 @@
--rw-r--r--   0        0        0     1075 2024-02-26 03:42:07.595076 async_wrapper-0.8.2/LICENSE
--rw-r--r--   0        0        0     1994 2024-02-26 03:42:07.595076 async_wrapper-0.8.2/README.md
--rw-r--r--   0        0        0     5214 2024-02-26 03:42:23.415052 async_wrapper-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      898 2024-02-26 03:42:07.595076 async_wrapper-0.8.2/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0      157 2024-02-26 03:42:07.595076 async_wrapper-0.8.2/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0     1672 2024-02-26 03:42:07.595076 async_wrapper-0.8.2/src/async_wrapper/convert/_async.py
--rw-r--r--   0        0        0     5746 2024-02-26 03:42:07.595076 async_wrapper-0.8.2/src/async_wrapper/convert/_sync.py
--rw-r--r--   0        0        0     1290 2024-02-26 03:42:07.595076 async_wrapper-0.8.2/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0     2101 2024-02-26 03:42:07.595076 async_wrapper-0.8.2/src/async_wrapper/exception.py
--rw-r--r--   0        0        0     8221 2024-02-26 03:42:07.595076 async_wrapper-0.8.2/src/async_wrapper/pipe.py
--rw-r--r--   0        0        0        0 2024-02-26 03:42:07.595076 async_wrapper-0.8.2/src/async_wrapper/py.typed
--rw-r--r--   0        0        0    18141 2024-02-26 03:42:07.595076 async_wrapper-0.8.2/src/async_wrapper/queue.py
--rw-r--r--   0        0        0      207 2024-02-26 03:42:07.595076 async_wrapper-0.8.2/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0     7237 2024-02-26 03:42:07.595076 async_wrapper-0.8.2/src/async_wrapper/task_group/task_group.py
--rw-r--r--   0        0        0     1231 2024-02-26 03:42:07.595076 async_wrapper-0.8.2/src/async_wrapper/task_group/value.py
--rw-r--r--   0        0        0    11470 2024-02-26 03:42:07.595076 async_wrapper-0.8.2/src/async_wrapper/wait.py
--rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 async_wrapper-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/Makefile
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/codecov.yml
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/make.bat
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/.github/workflows/check.yaml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/async_wrapper/exception.py
+-rw-r--r--   0        0        0     8221 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/async_wrapper/pipe.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0    18141 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/async_wrapper/queue.py
+-rw-r--r--   0        0        0    11470 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/async_wrapper/wait.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/async_wrapper/convert/_async.py
+-rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/async_wrapper/convert/_sync.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0     7237 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/async_wrapper/task_group/task_group.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/async_wrapper/task_group/value.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/docs/__init__.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/docs/conf.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/docs/index.rst
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/docs/async_wrapper/convert.rst
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/docs/async_wrapper/exception.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/docs/async_wrapper/index.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/docs/async_wrapper/pipe.rst
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/docs/async_wrapper/queue.rst
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/docs/async_wrapper/task_group.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/src/docs/async_wrapper/wait.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/tests/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/tests/base.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/tests/conftest.py
+-rw-r--r--   0        0        0    12985 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/tests/test_pipe.py
+-rw-r--r--   0        0        0    17184 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/tests/test_queue.py
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/tests/test_wait.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/tests/convert/__init__.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/tests/convert/base.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/tests/convert/test_async.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/tests/convert/test_sync.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/tests/task_group/__init__.py
+-rw-r--r--   0        0        0     8316 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/tests/task_group/test_task_group.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/tests/task_group/test_value.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/LICENSE
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/README.md
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 async_wrapper-0.8.3/PKG-INFO
```

### Comparing `async_wrapper-0.8.2/LICENSE` & `async_wrapper-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.8.2/README.md` & `async_wrapper-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.8.2/pyproject.toml` & `async_wrapper-0.8.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,72 @@
-[tool.poetry]
+[project]
 name = "async-wrapper"
-version = "0.8.2"
+version = "0.8.3"
 description = "async wrapper"
-authors = ["phi <phi.friday@gmail.com>"]
+authors = [{ name = "phi", email = "phi.friday@gmail.com" }]
 readme = "README.md"
-license = "MIT License"
-homepage = "https://async-wrapper.readthedocs.io/"
-repository = "https://github.com/phi-friday/async-wrapper"
-packages = [{ include = "async_wrapper", from = 'src' }]
+license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Framework :: AnyIO",
     "Framework :: AsyncIO",
-    "Framework :: Trio"
+    "Framework :: Trio",
+]
+requires-python = ">= 3.8"
+dependencies = [
+    "typing-extensions>=4.9.0",
+    "anyio>=4.3.0",
+    "sniffio==1.3.0",
+    "exceptiongroup>=1.2.0; python_version < '3.11'",
+]
+
+[project.urls]
+Documentation = "https://async-wrapper.readthedocs.io/"
+Repository = "https://github.com/phi-friday/async-wrapper"
+
+[project.optional-dependencies]
+uvloop = ["uvloop>=0.19.0; platform_system != 'Windows'"]
+docs = [
+    "sphinx>=7.1.0",
+    "readthedocs-sphinx-search>=0.3.2",
+    "sphinx-rtd-theme>=2.0.0",
+    "sphinx-mdinclude>=0.5.3",
 ]
 
-[tool.poetry.dependencies]
-python = ">=3.8"
-typing-extensions = ">=4.9.0"
-anyio = ">=4.3.0"
-sniffio = "1.3.0"
-uvloop = { version = ">=0.19.0", optional = true, markers = "platform_system != 'Windows'" }
-exceptiongroup = { version = ">=1.2.0", markers = "python_version < '3.11'" }
-
-[tool.poetry.extras]
-uvloop = ['uvloop']
-
-[tool.poetry.group.dev.dependencies]
-ruff = "0.2.2"
-ipykernel = ">=6.29.0"
-pytest = ">=8.0.0"
-pre-commit = ">=3.5.0"
-trio = ">=0.24.0"
-pyyaml = ">=6.0.1"
-pytest-cov = ">=4.1.0"
-
-
-[tool.poetry.group.docs.dependencies]
-sphinx = ">=7.1.0"
-readthedocs-sphinx-search = ">=0.3.2"
-sphinx-rtd-theme = ">=2.0.0"
-sphinx-mdinclude = ">=0.5.3"
+[tool.rye]
+managed = true
+dev-dependencies = [
+    "ruff==0.2.2",
+    "ipykernel>=6.29.0",
+    "pytest>=8.0.0",
+    "pre-commit>=3.5.0",
+    "trio>=0.24.0",
+    "pyyaml>=6.0.1",
+    "pytest-cov>=4.1.0",
+]
+
+[tool.rye.scripts]
+html = { cmd = "make html" }
 
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[tool.hatch.metadata]
+allow-direct-references = true
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/async_wrapper"]
 
 [tool.ruff]
 target-version = "py38"
 
 [tool.ruff.lint]
 select = ["ALL"]
 fixable = [
```

### Comparing `async_wrapper-0.8.2/src/async_wrapper/__init__.py` & `async_wrapper-0.8.3/src/async_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.8.2/src/async_wrapper/convert/_async.py` & `async_wrapper-0.8.3/src/async_wrapper/convert/_async.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.8.2/src/async_wrapper/convert/_sync.py` & `async_wrapper-0.8.3/src/async_wrapper/convert/_sync.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.8.2/src/async_wrapper/convert/main.py` & `async_wrapper-0.8.3/src/async_wrapper/convert/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.8.2/src/async_wrapper/exception.py` & `async_wrapper-0.8.3/src/async_wrapper/exception.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.8.2/src/async_wrapper/pipe.py` & `async_wrapper-0.8.3/src/async_wrapper/pipe.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.8.2/src/async_wrapper/queue.py` & `async_wrapper-0.8.3/src/async_wrapper/queue.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.8.2/src/async_wrapper/task_group/task_group.py` & `async_wrapper-0.8.3/src/async_wrapper/task_group/task_group.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.8.2/src/async_wrapper/task_group/value.py` & `async_wrapper-0.8.3/src/async_wrapper/task_group/value.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.8.2/src/async_wrapper/wait.py` & `async_wrapper-0.8.3/src/async_wrapper/wait.py`

 * *Files identical despite different names*

