# Comparing `tmp/some_aiohttp_middleware-0.1.5.tar.gz` & `tmp/some_aiohttp_middleware-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "some_aiohttp_middleware-0.1.5.tar", max compression
+gzip compressed data, was "some_aiohttp_middleware-0.1.6.tar", max compression
```

## Comparing `some_aiohttp_middleware-0.1.5.tar` & `some_aiohttp_middleware-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1065 2024-05-06 07:49:13.003096 some_aiohttp_middleware-0.1.5/LICENSE
--rw-r--r--   0        0        0      563 2024-05-06 07:49:13.003096 some_aiohttp_middleware-0.1.5/README.md
--rw-r--r--   0        0        0     1435 2024-05-06 07:49:32.158970 some_aiohttp_middleware-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      153 2024-05-06 07:49:13.003096 some_aiohttp_middleware-0.1.5/src/some_aiohttp_middleware/__init__.py
--rw-r--r--   0        0        0     1762 2024-05-06 07:49:13.003096 some_aiohttp_middleware-0.1.5/src/some_aiohttp_middleware/admin_auth_handler.py
--rw-r--r--   0        0        0     4854 2024-05-06 07:49:13.003096 some_aiohttp_middleware-0.1.5/src/some_aiohttp_middleware/base.py
--rw-r--r--   0        0        0     2760 2024-05-06 07:49:13.003096 some_aiohttp_middleware-0.1.5/src/some_aiohttp_middleware/db.py
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 some_aiohttp_middleware-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-17 12:08:49.595529 some_aiohttp_middleware-0.1.6/LICENSE
+-rw-r--r--   0        0        0      563 2024-05-17 12:08:49.595529 some_aiohttp_middleware-0.1.6/README.md
+-rw-r--r--   0        0        0     1547 2024-05-17 12:09:09.971817 some_aiohttp_middleware-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      196 2024-05-17 12:08:49.595529 some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/__init__.py
+-rw-r--r--   0        0        0     1762 2024-05-17 12:08:49.595529 some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/admin_auth_handler.py
+-rw-r--r--   0        0        0     4854 2024-05-17 12:08:49.595529 some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/base.py
+-rw-r--r--   0        0        0     2760 2024-05-17 12:08:49.595529 some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/db.py
+-rw-r--r--   0        0        0     2441 2024-05-17 12:08:49.595529 some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/s3.py
+-rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 some_aiohttp_middleware-0.1.6/PKG-INFO
```

### Comparing `some_aiohttp_middleware-0.1.5/LICENSE` & `some_aiohttp_middleware-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `some_aiohttp_middleware-0.1.5/README.md` & `some_aiohttp_middleware-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `some_aiohttp_middleware-0.1.5/pyproject.toml` & `some_aiohttp_middleware-0.1.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "some-aiohttp-middleware"
-version = "0.1.5"
+version = "0.1.6"
 license = "MIT"
 description = "Middleware framework for aiohttp"
 authors = ["tommmlij <tommmlij@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/tommmlij/some-aiohttp-middleware"
 packages = [{ include = "some_aiohttp_middleware", from = "src" }]
 
@@ -15,35 +15,39 @@
 [tool.poetry.dependencies]
 python = ">=3.8.1 <3.13"
 aiohttp = "^3.9.3"
 sqlalchemy = "^2.0.27"
 asyncpg = "^0.29.0"
 pydantic = "^2.6.4"
 aiohttp-pydantic = "^2.0.0"
+pydantic-settings = "^2.2.1"
+aioboto3 = "^12.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 flake8 = "^7.0.0"
 pytest-asyncio = "^0.23.5"
 pytest-aiohttp = "^1.0.5"
 colorlog = "^6.8.2"
 coverage = "^7.4.3"
 mypy = "^1.8.0"
 black = "^24.2.0"
 isort = "^5.13.2"
+aiohttp-middlewares = "^2.3.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 flake8 = "^7.0.0"
 pytest-asyncio = "^0.23.5"
 pytest-aiohttp = "^1.0.5"
 coverage = "^7.4.3"
 mypy = "^1.8.0"
 black = "^24.2.0"
 isort = "^5.13.2"
+aiohttp-middlewares = "^2.3.0"
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `some_aiohttp_middleware-0.1.5/src/some_aiohttp_middleware/admin_auth_handler.py` & `some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/admin_auth_handler.py`

 * *Files identical despite different names*

### Comparing `some_aiohttp_middleware-0.1.5/src/some_aiohttp_middleware/base.py` & `some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/base.py`

 * *Files identical despite different names*

### Comparing `some_aiohttp_middleware-0.1.5/src/some_aiohttp_middleware/db.py` & `some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/db.py`

 * *Files identical despite different names*

### Comparing `some_aiohttp_middleware-0.1.5/PKG-INFO` & `some_aiohttp_middleware-0.1.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: some-aiohttp-middleware
-Version: 0.1.5
+Version: 0.1.6
 Summary: Middleware framework for aiohttp
 Home-page: https://github.com/tommmlij/some-aiohttp-middleware
 License: MIT
 Author: tommmlij
 Author-email: tommmlij@gmail.com
 Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aioboto3 (>=12.4.0,<13.0.0)
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: aiohttp-pydantic (>=2.0.0,<3.0.0)
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0)
 Project-URL: GitHub: issues, https://github.com/tommmlij/some-aiohttp-middleware/issues
 Project-URL: GitHub: repo, https://github.com/tommmlij/some-aiohttp-middleware
 Description-Content-Type: text/markdown
 
 ![Static Badge](https://img.shields.io/badge/Python-3.8%2B-brightgreen?logo=python)
 ![PyPI - Version](https://img.shields.io/pypi/v/some-aiohttp-middleware?logo=pypi&logoColor=yellow&color=brightgreen)
```

