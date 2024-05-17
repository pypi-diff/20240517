# Comparing `tmp/iam-python-sdk-1.3.2.tar.gz` & `tmp/iam-python-sdk-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam-python-sdk-1.3.2.tar", last modified: Thu Jun 30 08:17:12 2022, max compression
+gzip compressed data, was "iam-python-sdk-1.3.3.tar", last modified: Thu Aug  4 08:09:50 2022, max compression
```

## Comparing `iam-python-sdk-1.3.2.tar` & `iam-python-sdk-1.3.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:17:12.407508 iam-python-sdk-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1624 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11339 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4040 2022-06-30 08:17:12.407508 iam-python-sdk-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:17:12.403509 iam-python-sdk-1.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/docs/asyncio.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/docs/changelog.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     4878 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6934 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/docs/frameworks.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2454 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/docs/iam_python_sdk.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6734 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:17:12.403509 iam-python-sdk-1.3.2/iam_python_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/iam_python_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33296 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/iam_python_sdk/async_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/iam_python_sdk/bloom.py
--rw-r--r--   0 runner    (1001) docker     (121)     3099 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/iam_python_sdk/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/iam_python_sdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    32723 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/iam_python_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2324 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/iam_python_sdk/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2450 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/iam_python_sdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    12037 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/iam_python_sdk/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (121)    14539 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/iam_python_sdk/flask.py
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/iam_python_sdk/http_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/iam_python_sdk/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/iam_python_sdk/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4198 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/iam_python_sdk/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/iam_python_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:17:12.403509 iam-python-sdk-1.3.2/iam_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4040 2022-06-30 08:17:11.000000 iam-python-sdk-1.3.2/iam_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-06-30 08:17:12.000000 iam-python-sdk-1.3.2/iam_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-30 08:17:11.000000 iam-python-sdk-1.3.2/iam_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-06-30 08:17:12.000000 iam-python-sdk-1.3.2/iam_python_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-30 08:17:11.000000 iam-python-sdk-1.3.2/iam_python_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-06-30 08:17:12.000000 iam-python-sdk-1.3.2/iam_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-30 08:17:12.000000 iam-python-sdk-1.3.2/iam_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-06-30 08:17:12.407508 iam-python-sdk-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1935 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:17:12.407508 iam-python-sdk-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2529 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/tests/mock.py
--rw-r--r--   0 runner    (1001) docker     (121)     8093 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/tests/test_async_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/tests/test_bloom.py
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     6691 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5151 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/tests/test_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (121)     4972 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/tests/test_flask.py
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2022-06-30 08:17:02.000000 iam-python-sdk-1.3.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:09:50.903847 iam-python-sdk-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (121)      641 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1755 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11339 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4171 2022-08-04 08:09:50.903847 iam-python-sdk-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:09:50.899847 iam-python-sdk-1.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      989 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/docs/asyncio.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/docs/changelog.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4878 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6934 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/docs/frameworks.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2454 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/docs/iam_python_sdk.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      776 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6734 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:09:50.899847 iam-python-sdk-1.3.3/iam_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/iam_python_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33296 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/iam_python_sdk/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/iam_python_sdk/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3099 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/iam_python_sdk/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/iam_python_sdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32723 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/iam_python_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2324 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/iam_python_sdk/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2450 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/iam_python_sdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13031 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/iam_python_sdk/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15480 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/iam_python_sdk/flask.py
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/iam_python_sdk/http_errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)      773 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/iam_python_sdk/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/iam_python_sdk/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4198 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/iam_python_sdk/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/iam_python_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:09:50.903847 iam-python-sdk-1.3.3/iam_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4171 2022-08-04 08:09:50.000000 iam-python-sdk-1.3.3/iam_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-08-04 08:09:50.000000 iam-python-sdk-1.3.3/iam_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-04 08:09:50.000000 iam-python-sdk-1.3.3/iam_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-04 08:09:50.000000 iam-python-sdk-1.3.3/iam_python_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-04 08:09:50.000000 iam-python-sdk-1.3.3/iam_python_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-08-04 08:09:50.000000 iam-python-sdk-1.3.3/iam_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-04 08:09:50.000000 iam-python-sdk-1.3.3/iam_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      562 2022-08-04 08:09:50.903847 iam-python-sdk-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1935 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 08:09:50.903847 iam-python-sdk-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2529 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7924 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/tests/mock.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8093 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/tests/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/tests/test_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6691 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4882 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/tests/test_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4679 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/tests/test_flask.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1627 2022-08-04 08:09:44.000000 iam-python-sdk-1.3.3/tests/test_utils.py
```

### Comparing `iam-python-sdk-1.3.2/AUTHORS.rst` & `iam-python-sdk-1.3.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/CHANGELOG.rst` & `iam-python-sdk-1.3.3/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 Changelog
 =========
 
+1.3.3 (2022-08-04)
+------------------
+
+* Fixing cookie token issue
+* Refactor getting access token function
+* Fixing CORS handler
+
 1.3.2 (2022-06-30)
 ------------------
 
 * Fixing multiple namespace_role permission validation
 * Disable default verify aud by pyjwt
 * Reformat logging
```

### Comparing `iam-python-sdk-1.3.2/CONTRIBUTING.rst` & `iam-python-sdk-1.3.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/LICENSE` & `iam-python-sdk-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/PKG-INFO` & `iam-python-sdk-1.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-python-sdk
-Version: 1.3.2
+Version: 1.3.3
 Summary: AccelByte IAM Python SDK
 Home-page: https://accelbyte.github.io/iam-python-sdk
 Author: Analytics AccelByte
 Author-email: justice-analytics-team@accelbyte.net
 License: Apache Software License 2.0
 Keywords: iam_python_sdk,accelbyte,iam
 Classifier: Development Status :: 5 - Production/Stable
@@ -66,14 +66,21 @@
 * Flask and FastAPI framework support with CSRF protection and CORS options
 
 
 =========
 Changelog
 =========
 
+1.3.3 (2022-08-04)
+------------------
+
+* Fixing cookie token issue
+* Refactor getting access token function
+* Fixing CORS handler
+
 1.3.2 (2022-06-30)
 ------------------
 
 * Fixing multiple namespace_role permission validation
 * Disable default verify aud by pyjwt
 * Reformat logging
```

### Comparing `iam-python-sdk-1.3.2/README.rst` & `iam-python-sdk-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/docs/Makefile` & `iam-python-sdk-1.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/docs/asyncio.rst` & `iam-python-sdk-1.3.3/docs/asyncio.rst`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/docs/conf.py` & `iam-python-sdk-1.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/docs/frameworks.rst` & `iam-python-sdk-1.3.3/docs/frameworks.rst`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/docs/iam_python_sdk.rst` & `iam-python-sdk-1.3.3/docs/iam_python_sdk.rst`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/docs/installation.rst` & `iam-python-sdk-1.3.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/docs/make.bat` & `iam-python-sdk-1.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/docs/usage.rst` & `iam-python-sdk-1.3.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk/__init__.py` & `iam-python-sdk-1.3.3/iam_python_sdk/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 
 from iam_python_sdk.client import NewDefaultClient
 from iam_python_sdk.async_client import NewAsyncClient
 from iam_python_sdk.config import Config
 
 __author__ = """Analytics AccelByte"""
 __email__ = 'justice-analytics-team@accelbyte.net'
-__version__ = '1.3.2'
+__version__ = '1.3.3'
 __all__ = [
     'NewDefaultClient',
     'NewAsyncClient',
     'Config'
 ]
```

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk/async_client.py` & `iam-python-sdk-1.3.3/iam_python_sdk/async_client.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk/bloom.py` & `iam-python-sdk-1.3.3/iam_python_sdk/bloom.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk/cache.py` & `iam-python-sdk-1.3.3/iam_python_sdk/cache.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk/cli.py` & `iam-python-sdk-1.3.3/iam_python_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk/client.py` & `iam-python-sdk-1.3.3/iam_python_sdk/client.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk/config.py` & `iam-python-sdk-1.3.3/iam_python_sdk/config.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk/errors.py` & `iam-python-sdk-1.3.3/iam_python_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk/fastapi.py` & `iam-python-sdk-1.3.3/iam_python_sdk/fastapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,14 +200,23 @@
             if validate_referer_with_subdomain(referer_header, redirect_uri):
                 return True
 
     return False
 
 
 def validate_referer_with_subdomain(referer_header: str, client_redirect_uri: str) -> bool:
+    """Validate referer header that have subdomain.
+
+    Args:
+        referer_header (str): Referer header string
+        client_redirect_uri (str): Client redirect URI string
+
+    Returns:
+        bool: Referer header status
+    """
     parsed_referer = urlparse(referer_header)
     parsed_redirect_uri = urlparse(client_redirect_uri)
 
     if parsed_referer.scheme == '' or parsed_redirect_uri.scheme == '':
         return False
 
     if parsed_referer.netloc == '' or parsed_redirect_uri.netloc == '':
@@ -215,60 +224,92 @@
 
     if parsed_referer.scheme != parsed_redirect_uri.scheme:
         return False
 
     return parsed_referer.netloc.endswith(parsed_redirect_uri.netloc)
 
 
-def token_required(csrf_protect: Union[bool, None] = None) -> Callable:
-    """Validate token in the FastAPI request. This method support headers and cookies with based token.
-
-    Args:
-        csrf_protect (bool, None): Validate referer for CSRF protection
+def access_token() -> Callable:
+    """Get access token from request.
 
     Raises:
         IAMError: Error IAM init
-        HTTPError: Error if token is not found or invalid
+        HTTPError: Error if token is not found
 
     Returns:
         JWTClaims: JWT claims data
     """
 
     async def _dependency(
         request: Request,
         bearer: Optional[HTTPAuthorizationCredentials] = Security(HTTPBearer(auto_error=False)),
         cookie: Optional[str] = Security(APIKeyCookie(name="access_token", auto_error=False)),
-    ) -> JWTClaims:
+    ) -> tuple:
         try:
             iam = request.app.state.iam
         except AttributeError:
             raise IAMError(
                 "You must initialize a IAM with on fastapi "
                 "startup event before using this method"
             )
 
-        access_token = ""
+        access_token = None
         token_location = iam.config.iam_token_locations
         for location in token_location:
             # Get token from headers
             if location == "headers":
                 if not bearer:
                     continue
 
                 header_parts = bearer.credentials.split()
                 access_token = header_parts[-1], "header"
 
+            # Break loop if access token has been found in request header
+            if access_token:
+                break
+
             # Get token from cookies
             if location == "cookies":
                 if cookie:
                     access_token = cookie, "cookie"
 
         if not access_token:
             raise HTTPError(*UnauthorizedAccess, description=f"Missing access token in {' or '.join(token_location)}")
 
+        return access_token
+
+    return _dependency
+
+
+def token_required(csrf_protect: Union[bool, None] = None) -> Callable:
+    """Validate token in the FastAPI request. This method support headers and cookies with based token.
+
+    Args:
+        csrf_protect (bool, None): Validate referer for CSRF protection
+
+    Raises:
+        IAMError: Error IAM init
+        HTTPError: Error if token is invalid
+
+    Returns:
+        JWTClaims: JWT claims data
+    """
+
+    async def _dependency(
+        request: Request,
+        access_token: tuple = Depends(access_token()),
+    ) -> JWTClaims:
+        try:
+            iam = request.app.state.iam
+        except AttributeError:
+            raise IAMError(
+                "You must initialize a IAM with on fastapi "
+                "startup event before using this method"
+            )
+
         try:
             jwt_claims = await iam.client.ValidateAndParseClaims(access_token[0])
         except (ValidateAndParseClaimsError, UserRevokedError, TokenRevokedError) as e:
             raise HTTPError(*UnauthorizedAccess, description=str(e))
 
         if not jwt_claims:
             raise HTTPError(*UnauthorizedAccess, description=f"Invalid access token")
```

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk/flask.py` & `iam-python-sdk-1.3.3/iam_python_sdk/flask.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,31 +39,14 @@
         self.error_code = error_code
         self.message = message
         self.description = description
 
 
 # ---------- Extensions ---------- #
 
-
-def validate_referer_with_subdomain(referer_header: str, client_redirect_uri: str) -> bool:
-    parsed_referer = urlparse(referer_header)
-    parsed_redirect_uri = urlparse(client_redirect_uri)
-
-    if parsed_referer.scheme == '' or parsed_redirect_uri.scheme == '':
-        return False
-
-    if parsed_referer.netloc == '' or parsed_redirect_uri.netloc == '':
-        return False
-
-    if parsed_referer.scheme != parsed_redirect_uri.scheme:
-        return False
-
-    return parsed_referer.netloc.endswith(parsed_redirect_uri.netloc)
-
-
 class IAM:
     """IAM Flask extensions class.
     """
 
     def __init__(self, app: Union[Flask, None] = None) -> None:
         self.app = app
         if app is not None:
@@ -131,14 +114,18 @@
             else current_app.config.get("IAM_CORS_METHODS")
 
         if isinstance(allowed_methods, list):
             allowed_methods = ", ".join(allowed_methods)
         if isinstance(allowed_headers, list):
             allowed_headers = ", ".join(allowed_headers)
 
+        if "*" not in allowed_origin or allow_credentials == "true":
+            allowed_origin = request.origin
+            response.headers.setdefault("Vary", "Origin")
+
         response.headers.setdefault("Access-Control-Allow-Origin", allowed_origin)
         response.headers.setdefault("Access-Control-Allow-Headers", allowed_headers)
         response.headers.setdefault("Access-Control-Allow-Methods", allowed_methods)
         response.headers.setdefault("Access-Control-Allow-Credentials", allow_credentials)
 
         return response
 
@@ -195,32 +182,53 @@
                 parsed_uri = urlparse(redirect_uri)
                 redirect_uri = f"{parsed_uri.scheme}://{parsed_uri.netloc}"
 
             if not current_app.config.get("IAM_ALLOW_SUBDOMAIN_REFERER"):
                 if referer_header and referer_header.startswith(redirect_uri):
                     return True
             else:
-                if validate_referer_with_subdomain(referer_header, redirect_uri):
+                if self.validate_referer_with_subdomain(referer_header, redirect_uri):
                     return True
 
         return False
 
-    def validate_token_in_request(self, validate_referer: bool) -> JWTClaims:
-        """Validate token in the Flask request. This method support headers and cookies with based token.
+    def validate_referer_with_subdomain(self, referer_header: str, client_redirect_uri: str) -> bool:
+        """Validate referer header that have subdomain.
 
         Args:
-            validate_referer (bool): Validate referer for CSRF protection
+            referer_header (str): Referer header string
+            client_redirect_uri (str): Client redirect URI string
+
+        Returns:
+            bool: Referer header status
+        """
+        parsed_referer = urlparse(referer_header)
+        parsed_redirect_uri = urlparse(client_redirect_uri)
+
+        if parsed_referer.scheme == "" or parsed_redirect_uri.scheme == "":
+            return False
+
+        if parsed_referer.netloc == "" or parsed_redirect_uri.netloc == "":
+            return False
+
+        if parsed_referer.scheme != parsed_redirect_uri.scheme:
+            return False
+
+        return parsed_referer.netloc.endswith(parsed_redirect_uri.netloc)
+
+    def get_token_in_request(self) -> tuple:
+        """Extract access token from request.
 
         Raises:
-            HTTPError: Error if token is not found or invalid
+            HTTPError: Error if token is not found
 
         Returns:
-            JWTClaims: JWT claims data
+            tuple: [0] Access token string, [1] Location of access token
         """
-        access_token = ""
+        access_token = None
         token_location = current_app.config.get("IAM_TOKEN_LOCATIONS", [])
         for location in token_location:
             # Get token from headers
             if location == "headers":
                 auth_name = current_app.config.get("IAM_TOKEN_HEADER_NAME")
                 auth_type = current_app.config.get("IAM_TOKEN_HEADER_TYPE")
 
@@ -230,24 +238,43 @@
 
                 header_parts = auth_header.split()
                 if not auth_type:
                     access_token = header_parts[0], "header"
                 else:
                     access_token = header_parts[1], "header"
 
+            # Break loop if access token has been found in request header
+            if access_token:
+                break
+
             # Get token from cookies
             if location == "cookies":
                 cookie_name = current_app.config.get("IAM_TOKEN_COOKIE_NAME")
                 auth_cookie = request.cookies.get(cookie_name)
                 if auth_cookie:
                     access_token = auth_cookie, "cookie"
 
         if not access_token:
             raise HTTPError(*UnauthorizedAccess, description=f"Missing access token in {' or '.join(token_location)}")
 
+        return access_token
+
+    def validate_token_in_request(self, validate_referer: bool) -> JWTClaims:
+        """Validate token in the Flask request. This method support headers and cookies with based token.
+
+        Args:
+            validate_referer (bool): Validate referer for CSRF protection
+
+        Raises:
+            HTTPError: Error if token is invalid
+
+        Returns:
+            JWTClaims: JWT claims data
+        """
+        access_token = self.get_token_in_request()
         try:
             jwt_claims = self.client.ValidateAndParseClaims(access_token[0])
         except (ValidateAndParseClaimsError, UserRevokedError, TokenRevokedError) as e:
             raise HTTPError(*UnauthorizedAccess, description=str(e))
 
         if not jwt_claims:
             raise HTTPError(*UnauthorizedAccess, description=f"Invalid access token")
```

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk/http_errors.py` & `iam-python-sdk-1.3.3/iam_python_sdk/http_errors.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk/log.py` & `iam-python-sdk-1.3.3/iam_python_sdk/log.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk/models.py` & `iam-python-sdk-1.3.3/iam_python_sdk/models.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk/task.py` & `iam-python-sdk-1.3.3/iam_python_sdk/task.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk/utils.py` & `iam-python-sdk-1.3.3/iam_python_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk.egg-info/PKG-INFO` & `iam-python-sdk-1.3.3/iam_python_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-python-sdk
-Version: 1.3.2
+Version: 1.3.3
 Summary: AccelByte IAM Python SDK
 Home-page: https://accelbyte.github.io/iam-python-sdk
 Author: Analytics AccelByte
 Author-email: justice-analytics-team@accelbyte.net
 License: Apache Software License 2.0
 Keywords: iam_python_sdk,accelbyte,iam
 Classifier: Development Status :: 5 - Production/Stable
@@ -66,14 +66,21 @@
 * Flask and FastAPI framework support with CSRF protection and CORS options
 
 
 =========
 Changelog
 =========
 
+1.3.3 (2022-08-04)
+------------------
+
+* Fixing cookie token issue
+* Refactor getting access token function
+* Fixing CORS handler
+
 1.3.2 (2022-06-30)
 ------------------
 
 * Fixing multiple namespace_role permission validation
 * Disable default verify aud by pyjwt
 * Reformat logging
```

### Comparing `iam-python-sdk-1.3.2/iam_python_sdk.egg-info/SOURCES.txt` & `iam-python-sdk-1.3.3/iam_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/setup.cfg` & `iam-python-sdk-1.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.3.2
+current_version = 1.3.3
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(rc(?P<rc>\d+))?
 serialize = 
 	{major}.{minor}.{patch}rc{rc}
 	{major}.{minor}.{patch}
```

### Comparing `iam-python-sdk-1.3.2/setup.py` & `iam-python-sdk-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,10 +57,10 @@
     include_package_data=True,
     keywords=['iam_python_sdk', 'accelbyte', 'iam'],
     name='iam-python-sdk',
     packages=find_packages(include=['iam_python_sdk', 'iam_python_sdk.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://accelbyte.github.io/iam-python-sdk',
-    version='1.3.2',
+    version='1.3.3',
     zip_safe=False,
 )
```

### Comparing `iam-python-sdk-1.3.2/tests/conftest.py` & `iam-python-sdk-1.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/tests/mock.py` & `iam-python-sdk-1.3.3/tests/mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,14 @@
 @flask_mock.route('/protected_with_csrf')
 @flask_permission_required({"resource": "ADMIN:NAMESPACE:{namespace}:CLIENT", "action": 2}, {"{namespace}": "sdktest"})
 def flask_protected_with_csrf():
     return flask.jsonify({'status': 'protected'})
 
 
 @flask_mock.route('/protected_with_cors', methods=["POST"])
-@flask_permission_required({"resource": "ADMIN:NAMESPACE:{namespace}:CLIENT", "action": 2}, {"{namespace}": "sdktest"})
 @flask_cors_options({"Access-Control-Allow-Headers": ["Device-Id", "Device-Os", "Device-Type"]})
 def flask_protected_with_cors():
     return flask.jsonify({'status': 'protected'})
 
 
 # FastAPI mock
 fastapi_mock = fastapi.APIRouter()
```

### Comparing `iam-python-sdk-1.3.2/tests/test_async_client.py` & `iam-python-sdk-1.3.3/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/tests/test_bloom.py` & `iam-python-sdk-1.3.3/tests/test_bloom.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/tests/test_cache.py` & `iam-python-sdk-1.3.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/tests/test_cli.py` & `iam-python-sdk-1.3.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/tests/test_client.py` & `iam-python-sdk-1.3.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `iam-python-sdk-1.3.2/tests/test_flask.py` & `iam-python-sdk-1.3.3/tests/test_flask.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Tests for `iam_python_sdk.flask` module."""
 
 import json
 
 from flask import Flask, current_app
 
 from iam_python_sdk.client import DefaultClient
-from iam_python_sdk.flask import IAM, validate_referer_with_subdomain
+from iam_python_sdk.flask import IAM
 
 from .mock import iam_mock, client_token
 
 
 def test_init_iam(flask_app: Flask) -> None:
     with flask_app.app_context():
         iam = current_app.extensions.get("flask_iam")
@@ -63,59 +63,57 @@
         c.set_cookie("localhost", "access_token", client_token['access_token'])
         resp = c.get('/protected')
         assert resp.status_code == 200
 
 
 @iam_mock
 def test_protected_with_csrf_endpoint(flask_app: Flask) -> None:
+    # Redirect URI: https://example.com
     with flask_app.test_client() as c:
         c.set_cookie("localhost", "access_token", client_token['access_token'])
         # Valid referer header
         resp = c.get('/protected_with_csrf', headers={"Referer": "https://example.com"})
         assert resp.status_code == 200
         # Invalid referer header
         resp = c.get('/protected_with_csrf', headers={"Referer": "http://foo.bar"})
         assert resp.status_code == 401
 
 
 @iam_mock
 def test_protected_with_csrf_endpoint_with_subdomain(flask_app: Flask) -> None:
     flask_app.config["IAM_ALLOW_SUBDOMAIN_REFERER"] = True
 
+    # Redirect URI: https://example.com
     with flask_app.test_client() as c:
         c.set_cookie("localhost", "access_token", client_token['access_token'])
         # Valid referer header with subdomain
         resp = c.get('/protected_with_csrf', headers={"Referer": "https://test.example.com"})
         assert resp.status_code == 200
         # Invalid referer header
         resp = c.get('/protected_with_csrf', headers={"Referer": "http://test.foo.bar"})
         assert resp.status_code == 401
+        # Invalid scheme
+        resp = c.get('/protected_with_csrf', headers={"Referer": "http://example.com"})
+        assert resp.status_code == 401
+        # Invalid domain
+        resp = c.get('/protected_with_csrf', headers={"Referer": "https://example.net"})
+        assert resp.status_code == 401
 
 
 @iam_mock
 def test_protected_with_cors_endpoint(flask_app: Flask) -> None:
     with flask_app.test_client() as c:
         c.set_cookie("localhost", "access_token", client_token['access_token'])
-        resp = c.options('/protected_with_cors', headers={"Referer": "https://example.com"})
+        resp = c.options(
+            '/protected_with_cors',
+            headers={"Origin": "http://127.0.0.1",
+                     "Access-Control-Request-Method": "POST",
+                     "Access-Control-Request-Headers": "Device-Id"
+                     }
+        )
         assert resp.status_code == 200
         # Preflight options have empty body response
         assert resp.get_json() is None
         # Assert default CORS header
-        assert resp.headers.get("Access-Control-Allow-Origin", "") == "*"
+        assert resp.headers.get("Access-Control-Allow-Origin", "") == "http://127.0.0.1"
         # Assert override CORS header
         assert resp.headers.get("Access-Control-Allow-Headers", "").find("Device-Id") != -1
-
-
-def test_validate_referer_with_subdomain():
-    # Assert wrong URL
-    assert validate_referer_with_subdomain("wrongaddress", "anotherwrong") == False
-    assert validate_referer_with_subdomain("https://example.com", "wrongaddress") == False
-    assert validate_referer_with_subdomain("wrongaddress", "https://example.com") == False
-    # Assert mismatch scheme
-    assert validate_referer_with_subdomain("http://example.com", "https://example.com") == False
-    # Assert mismatch domain
-    assert validate_referer_with_subdomain("https://example.com", "https://example.net") == False
-
-    # Assert exact match
-    assert validate_referer_with_subdomain("https://example.com", "https://example.com") == True
-    # Assert subdomain match
-    assert validate_referer_with_subdomain("https://test.example.com", "https://example.com") == True
```

### Comparing `iam-python-sdk-1.3.2/tests/test_utils.py` & `iam-python-sdk-1.3.3/tests/test_utils.py`

 * *Files identical despite different names*

