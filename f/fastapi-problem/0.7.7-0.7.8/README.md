# Comparing `tmp/fastapi_problem-0.7.7.tar.gz` & `tmp/fastapi_problem-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_problem-0.7.7.tar", max compression
+gzip compressed data, was "fastapi_problem-0.7.8.tar", max compression
```

## Comparing `fastapi_problem-0.7.7.tar` & `fastapi_problem-0.7.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11307 2024-05-16 07:03:50.656904 fastapi_problem-0.7.7/LICENSE
--rw-r--r--   0        0        0     1891 2024-05-16 07:03:50.656904 fastapi_problem-0.7.7/README.md
--rw-r--r--   0        0        0     2196 2024-05-16 07:03:50.660904 fastapi_problem-0.7.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 07:03:50.660904 fastapi_problem-0.7.7/src/fastapi_problem/__init__.py
--rw-r--r--   0        0        0      220 2024-05-16 07:03:50.660904 fastapi_problem-0.7.7/src/fastapi_problem/cors.py
--rw-r--r--   0        0        0     1789 2024-05-16 07:03:50.660904 fastapi_problem-0.7.7/src/fastapi_problem/error.py
--rw-r--r--   0        0        0        0 2024-05-16 07:03:50.660904 fastapi_problem-0.7.7/src/fastapi_problem/handler/__init__.py
--rw-r--r--   0        0        0     5959 2024-05-16 07:03:50.660904 fastapi_problem-0.7.7/src/fastapi_problem/handler/base.py
--rw-r--r--   0        0        0     3004 2024-05-16 07:03:50.660904 fastapi_problem-0.7.7/src/fastapi_problem/handler/fastapi.py
--rw-r--r--   0        0        0      299 2024-05-16 07:03:50.660904 fastapi_problem-0.7.7/src/fastapi_problem/handler/util.py
--rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 fastapi_problem-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0    11307 2024-05-17 09:02:55.954609 fastapi_problem-0.7.8/LICENSE
+-rw-r--r--   0        0        0     1891 2024-05-17 09:02:55.954609 fastapi_problem-0.7.8/README.md
+-rw-r--r--   0        0        0     2194 2024-05-17 09:02:55.958609 fastapi_problem-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 09:02:55.958609 fastapi_problem-0.7.8/src/fastapi_problem/__init__.py
+-rw-r--r--   0        0        0      220 2024-05-17 09:02:55.958609 fastapi_problem-0.7.8/src/fastapi_problem/cors.py
+-rw-r--r--   0        0        0     1789 2024-05-17 09:02:55.958609 fastapi_problem-0.7.8/src/fastapi_problem/error.py
+-rw-r--r--   0        0        0        0 2024-05-17 09:02:55.958609 fastapi_problem-0.7.8/src/fastapi_problem/handler/__init__.py
+-rw-r--r--   0        0        0     5945 2024-05-17 09:02:55.958609 fastapi_problem-0.7.8/src/fastapi_problem/handler/base.py
+-rw-r--r--   0        0        0     2990 2024-05-17 09:02:55.958609 fastapi_problem-0.7.8/src/fastapi_problem/handler/fastapi.py
+-rw-r--r--   0        0        0      299 2024-05-17 09:02:55.958609 fastapi_problem-0.7.8/src/fastapi_problem/handler/util.py
+-rw-r--r--   0        0        0     2624 1970-01-01 00:00:00.000000 fastapi_problem-0.7.8/PKG-INFO
```

### Comparing `fastapi_problem-0.7.7/LICENSE` & `fastapi_problem-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_problem-0.7.7/README.md` & `fastapi_problem-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_problem-0.7.7/pyproject.toml` & `fastapi_problem-0.7.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "fastapi-problem"
-version = "0.7.7"
+version = "0.7.8"
 description = "FastAPI support for RFC9457 problems."
 authors = ["Daniel Edgecombe <edgy.edgemond@gmail.com>"]
 license = "Apache-2.0"
 repository="https://github.com/NRWLDev/fastapi-problem/"
 homepage="https://github.com/NRWLDev/fastapi-problem/"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-rfc9457 = "^0.0.2"
+rfc9457 = "^0.0"
 
 [tool.poetry.dev-dependencies]
 
 fastapi = "*"
 
 changelog-gen = { version="^0.9", extras=["bump-my-version"]}
 pytest = "~7.4.3"
@@ -24,15 +24,15 @@
 pytest-random-order = "^1.0"
 
 # Style
 ruff = "^0.3.0"
 pre-commit = "^3.0.2"
 
 [tool.bumpversion]
-current_version = "0.7.7"
+current_version = "0.7.8"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `fastapi_problem-0.7.7/src/fastapi_problem/error.py` & `fastapi_problem-0.7.8/src/fastapi_problem/error.py`

 * *Files identical despite different names*

### Comparing `fastapi_problem-0.7.7/src/fastapi_problem/handler/base.py` & `fastapi_problem-0.7.8/src/fastapi_problem/handler/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import http
 import logging
 import typing as t
 
+from rfc9457 import Problem, StatusProblem
 from starlette.middleware.cors import CORSMiddleware
 from starlette.requests import Request
 from starlette.responses import JSONResponse
 
-from fastapi_problem.error import Problem, StatusProblem
 from fastapi_problem.handler.util import convert_status_code
 
 if t.TYPE_CHECKING:
     from starlette.exceptions import HTTPException
 
     from fastapi_problem.cors import CorsConfiguration
```

### Comparing `fastapi_problem-0.7.7/src/fastapi_problem/handler/fastapi.py` & `fastapi_problem-0.7.8/src/fastapi_problem/handler/fastapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import json
 import logging
 import typing as t
 
 from fastapi.exceptions import RequestValidationError
+from rfc9457 import Problem, StatusProblem
 from starlette.exceptions import HTTPException
 
-from fastapi_problem.error import Problem, StatusProblem
 from fastapi_problem.handler.base import CorsPostHook, ExceptionHandler, http_exception_handler
 
 if t.TYPE_CHECKING:
     from fastapi import FastAPI
     from starlette.requests import Request
 
     from fastapi_problem.cors import CorsConfiguration
```

### Comparing `fastapi_problem-0.7.7/PKG-INFO` & `fastapi_problem-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: fastapi-problem
-Version: 0.7.7
+Version: 0.7.8
 Summary: FastAPI support for RFC9457 problems.
 Home-page: https://github.com/NRWLDev/fastapi-problem/
 License: Apache-2.0
 Author: Daniel Edgecombe
 Author-email: edgy.edgemond@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: rfc9457 (>=0.0.2,<0.0.3)
+Requires-Dist: rfc9457 (>=0.0,<0.1)
 Project-URL: Repository, https://github.com/NRWLDev/fastapi-problem/
 Description-Content-Type: text/markdown
 
 # FastAPI Problems
 [![image](https://img.shields.io/pypi/v/fastapi_problem.svg)](https://pypi.org/project/fastapi-problem/)
 [![image](https://img.shields.io/pypi/l/fastapi_problem.svg)](https://pypi.org/project/fastapi-problem/)
 [![image](https://img.shields.io/pypi/pyversions/fastapi_problem.svg)](https://pypi.org/project/fastapi-problem/)
```

