# Comparing `tmp/adspower-1.0.0.tar.gz` & `tmp/adspower-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adspower-1.0.0.tar", max compression
+gzip compressed data, was "adspower-2.0.0.tar", max compression
```

## Comparing `adspower-1.0.0.tar` & `adspower-2.0.0.tar`

### file list

```diff
@@ -1,9 +1,53 @@
--rw-r--r--   0        0        0     1062 2023-11-11 14:57:15.312160 adspower-1.0.0/LICENSE
--rw-r--r--   0        0        0     2326 2023-12-13 15:56:26.866471 adspower-1.0.0/README.md
--rw-r--r--   0        0        0      621 2023-12-13 15:50:21.118932 adspower-1.0.0/adspower/__init__.py
--rw-r--r--   0        0        0    19184 2023-12-13 15:05:12.500606 adspower-1.0.0/adspower/adspower.py
--rw-r--r--   0        0        0     3453 2023-12-13 15:05:12.502745 adspower-1.0.0/adspower/exceptions.py
--rw-r--r--   0        0        0     1467 2023-11-11 15:18:28.397354 adspower-1.0.0/adspower/types.py
--rw-r--r--   0        0        0      300 2023-12-13 15:01:31.016403 adspower-1.0.0/adspower/utils.py
--rw-r--r--   0        0        0     1065 2023-12-13 16:01:44.502359 adspower-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3307 1970-01-01 00:00:00.000000 adspower-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-17 16:56:11.595785 adspower-2.0.0/LICENSE
+-rw-r--r--   0        0        0     5360 2024-05-17 16:56:40.340081 adspower-2.0.0/README.md
+-rw-r--r--   0        0        0     6148 2024-03-28 21:36:21.497542 adspower-2.0.0/adspower/.DS_Store
+-rw-r--r--   0        0        0      574 2024-05-17 16:56:11.597097 adspower-2.0.0/adspower/__init__.py
+-rw-r--r--   0        0        0      575 2024-05-17 16:56:11.597303 adspower-2.0.0/adspower/_api_entity.py
+-rw-r--r--   0        0        0     2185 2024-05-17 16:56:11.598716 adspower-2.0.0/adspower/_base_category.py
+-rw-r--r--   0        0        0     3656 2024-05-17 16:56:11.599073 adspower-2.0.0/adspower/_base_group.py
+-rw-r--r--   0        0        0     4676 2024-05-17 16:56:11.599344 adspower-2.0.0/adspower/_base_http_client.py
+-rw-r--r--   0        0        0    17092 2024-05-17 16:56:11.599574 adspower-2.0.0/adspower/_base_profile_api.py
+-rw-r--r--   0        0        0      127 2024-05-17 16:56:11.602307 adspower-2.0.0/adspower/async_api/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-13 16:52:30.576253 adspower-2.0.0/adspower/async_api/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3041 2024-04-13 16:52:30.689713 adspower-2.0.0/adspower/async_api/__pycache__/category.cpython-311.pyc
+-rw-r--r--   0        0        0     4830 2024-04-13 16:52:56.419550 adspower-2.0.0/adspower/async_api/__pycache__/group.cpython-311.pyc
+-rw-r--r--   0        0        0     6844 2024-04-13 16:52:30.584548 adspower-2.0.0/adspower/async_api/__pycache__/http_client.cpython-311.pyc
+-rw-r--r--   0        0        0    20853 2024-04-13 16:52:30.692386 adspower-2.0.0/adspower/async_api/__pycache__/profile_api.cpython-311.pyc
+-rw-r--r--   0        0        0     1390 2024-05-17 16:56:11.602431 adspower-2.0.0/adspower/async_api/_base_profile.py
+-rw-r--r--   0        0        0     1513 2024-05-17 16:56:11.602639 adspower-2.0.0/adspower/async_api/category.py
+-rw-r--r--   0        0        0     2277 2024-05-17 16:56:11.602830 adspower-2.0.0/adspower/async_api/group.py
+-rw-r--r--   0        0        0     4603 2024-05-17 16:56:11.603111 adspower-2.0.0/adspower/async_api/http_client.py
+-rw-r--r--   0        0        0       46 2024-05-17 16:56:11.603899 adspower-2.0.0/adspower/async_api/playwright/__init__.py
+-rw-r--r--   0        0        0      265 2024-04-05 10:13:09.343021 adspower-2.0.0/adspower/async_api/playwright/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7181 2024-04-13 17:16:03.126815 adspower-2.0.0/adspower/async_api/playwright/__pycache__/profile.cpython-311.pyc
+-rw-r--r--   0        0        0     5678 2024-05-17 16:56:11.604117 adspower-2.0.0/adspower/async_api/playwright/profile.py
+-rw-r--r--   0        0        0    14258 2024-05-17 16:56:11.604433 adspower-2.0.0/adspower/async_api/profile_api.py
+-rw-r--r--   0        0        0       46 2024-05-17 16:56:11.604858 adspower-2.0.0/adspower/async_api/selenium/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-13 17:16:03.089580 adspower-2.0.0/adspower/async_api/selenium/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7358 2024-04-13 17:16:03.091952 adspower-2.0.0/adspower/async_api/selenium/__pycache__/profile.cpython-311.pyc
+-rw-r--r--   0        0        0     6004 2024-05-17 16:56:11.605079 adspower-2.0.0/adspower/async_api/selenium/profile.py
+-rw-r--r--   0        0        0     2233 2024-05-17 16:56:11.605255 adspower-2.0.0/adspower/exceptions.py
+-rw-r--r--   0        0        0      128 2024-05-17 16:56:11.606512 adspower-2.0.0/adspower/sync_api/__init__.py
+-rw-r--r--   0        0        0      408 2024-04-13 15:55:54.872311 adspower-2.0.0/adspower/sync_api/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3061 2024-04-20 07:57:35.369143 adspower-2.0.0/adspower/sync_api/__pycache__/_base_profile.cpython-311.pyc
+-rw-r--r--   0        0        0     2839 2024-04-14 10:02:14.342060 adspower-2.0.0/adspower/sync_api/__pycache__/category.cpython-311.pyc
+-rw-r--r--   0        0        0     4269 2024-04-13 15:55:54.874173 adspower-2.0.0/adspower/sync_api/__pycache__/group.cpython-311.pyc
+-rw-r--r--   0        0        0     6470 2024-04-13 15:55:54.880057 adspower-2.0.0/adspower/sync_api/__pycache__/http_client.cpython-311.pyc
+-rw-r--r--   0        0        0    17873 2024-04-19 11:54:56.936014 adspower-2.0.0/adspower/sync_api/__pycache__/profile_api.cpython-311.pyc
+-rw-r--r--   0        0        0     1301 2024-05-17 16:56:11.606817 adspower-2.0.0/adspower/sync_api/_base_profile.py
+-rw-r--r--   0        0        0     1494 2024-05-17 16:56:11.606918 adspower-2.0.0/adspower/sync_api/category.py
+-rw-r--r--   0        0        0     2217 2024-05-17 16:56:11.607017 adspower-2.0.0/adspower/sync_api/group.py
+-rw-r--r--   0        0        0     4469 2024-05-17 16:56:11.607432 adspower-2.0.0/adspower/sync_api/http_client.py
+-rw-r--r--   0        0        0       45 2024-05-17 16:56:11.607653 adspower-2.0.0/adspower/sync_api/playwright/__init__.py
+-rw-r--r--   0        0        0      289 2024-04-14 16:29:04.004792 adspower-2.0.0/adspower/sync_api/playwright/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7317 2024-04-19 12:17:34.250343 adspower-2.0.0/adspower/sync_api/playwright/__pycache__/profile.cpython-311.pyc
+-rw-r--r--   0        0        0     5570 2024-05-17 16:56:11.607914 adspower-2.0.0/adspower/sync_api/playwright/profile.py
+-rw-r--r--   0        0        0    13893 2024-05-17 16:56:11.608160 adspower-2.0.0/adspower/sync_api/profile_api.py
+-rw-r--r--   0        0        0       46 2024-05-17 16:56:11.608254 adspower-2.0.0/adspower/sync_api/selenium/__init__.py
+-rw-r--r--   0        0        0      262 2024-04-01 16:08:48.029121 adspower-2.0.0/adspower/sync_api/selenium/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4729 2024-04-04 22:46:36.298311 adspower-2.0.0/adspower/sync_api/selenium/__pycache__/profile.cpython-311.pyc
+-rw-r--r--   0        0        0     5947 2024-05-17 16:56:11.609776 adspower-2.0.0/adspower/sync_api/selenium/profile.py
+-rw-r--r--   0        0        0     3676 2024-05-17 16:56:11.610012 adspower-2.0.0/adspower/types.py
+-rw-r--r--   0        0        0     1099 2024-05-17 16:56:11.610275 adspower-2.0.0/adspower/utils.py
+-rw-r--r--   0        0        0     1259 2024-05-17 16:56:11.610398 adspower-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6478 1970-01-01 00:00:00.000000 adspower-2.0.0/PKG-INFO
```

### Comparing `adspower-1.0.0/LICENSE` & `adspower-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adspower-1.0.0/pyproject.toml` & `adspower-2.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = 'adspower'
-version = '1.0.0'
+version = '2.0.0'
 description = 'The package for interacting with API of anti-detect browser AdsPower.'
-authors = ['Alexey <abelenkov2006@gmail.com>']
+authors = ['Alexey <axbelenkov@gmail.com>']
 license = 'MIT'
 readme = 'README.md'
 repository = 'https://github.com/blnkoff/adspower'
 homepage = 'https://github.com/blnkoff/adspower'
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
@@ -17,20 +17,27 @@
     'Operating System :: Microsoft :: Windows',
     'Operating System :: MacOS'
 ]
 packages = [{ include = 'adspower' }]
 
 [tool.poetry.dependencies]
 python = '^3.11'
-requests = "^2.31.0"
-selenium = "^4.16.0"
+httpx = "^0.27.0"
+selenium = {version = "^4.16.0", optional = true}
+playwright = {version = "^1.42.0", optional = true}
+
+[tool.poetry.extras]
+selenium = ["selenium"]
+playwright = ["playwright"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 twine = "^4.0.2"
 build = "^1.0.3"
 sphinx-rtd-theme = "^2.0.0"
 sphinx = "^7.2.6"
+faker = "^24.9.0"
+pytest-asyncio = "^0.23.6"
 
 [build-system]
 requires = ['poetry-core']
 build-backend = 'poetry.core.masonry.api'
```

