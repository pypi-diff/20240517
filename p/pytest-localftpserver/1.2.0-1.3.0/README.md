# Comparing `tmp/pytest_localftpserver-1.2.0.tar.gz` & `tmp/pytest_localftpserver-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_localftpserver-1.2.0.tar", last modified: Sat Oct 14 13:31:48 2023, max compression
+gzip compressed data, was "pytest_localftpserver-1.3.0.tar", last modified: Fri May 17 19:59:13 2024, max compression
```

## Comparing `pytest_localftpserver-1.2.0.tar` & `pytest_localftpserver-1.3.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 13:31:48.549912 pytest_localftpserver-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 13:31:48.533911 pytest_localftpserver-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 13:31:48.533911 pytest_localftpserver-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/.github/workflows/CI_CD_actions.yml
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2023-10-14 13:31:48.549912 pytest_localftpserver-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 13:31:48.537911 pytest_localftpserver-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 13:31:48.525911 pytest_localftpserver-1.2.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 13:31:48.537911 pytest_localftpserver-1.2.0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/docs/_templates/autosummary/method.rst
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/docs/api_doc.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     9117 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12836 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 13:31:48.541911 pytest_localftpserver-1.2.0/pytest_localftpserver/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/pytest_localftpserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-14 13:31:48.000000 pytest_localftpserver-1.2.0/pytest_localftpserver/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/pytest_localftpserver/default_keycert.pem
--rw-r--r--   0 runner    (1001) docker     (127)    12605 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/pytest_localftpserver/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/pytest_localftpserver/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    38317 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/pytest_localftpserver/servers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 13:31:48.545911 pytest_localftpserver-1.2.0/pytest_localftpserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2023-10-14 13:31:48.000000 pytest_localftpserver-1.2.0/pytest_localftpserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2023-10-14 13:31:48.000000 pytest_localftpserver-1.2.0/pytest_localftpserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-14 13:31:48.000000 pytest_localftpserver-1.2.0/pytest_localftpserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-14 13:31:48.000000 pytest_localftpserver-1.2.0/pytest_localftpserver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-10-14 13:31:48.000000 pytest_localftpserver-1.2.0/pytest_localftpserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-14 13:31:48.000000 pytest_localftpserver-1.2.0/pytest_localftpserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      249 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-14 13:31:48.549912 pytest_localftpserver-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 13:31:48.549912 pytest_localftpserver-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/tests/not_a_valid_cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/tests/test_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/tests/test_keycert.pem
--rw-r--r--   0 runner    (1001) docker     (127)    27351 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/tests/test_pytest_localftpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/tests/test_pytest_localftpserver_TLS.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/tests/test_pytest_localftpserver_with_env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2023-10-14 13:31:31.000000 pytest_localftpserver-1.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:13.656431 pytest_localftpserver-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:13.652431 pytest_localftpserver-1.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:13.652431 pytest_localftpserver-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/.github/workflows/CI_CD_actions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-05-17 19:59:13.656431 pytest_localftpserver-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:13.652431 pytest_localftpserver-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:13.648431 pytest_localftpserver-1.3.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:13.652431 pytest_localftpserver-1.3.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/docs/_templates/autosummary/method.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/docs/api_doc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9117 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:13.656431 pytest_localftpserver-1.3.0/pytest_localftpserver/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/pytest_localftpserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 19:59:13.000000 pytest_localftpserver-1.3.0/pytest_localftpserver/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/pytest_localftpserver/default_keycert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    12737 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/pytest_localftpserver/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/pytest_localftpserver/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38317 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/pytest_localftpserver/servers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:13.656431 pytest_localftpserver-1.3.0/pytest_localftpserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-05-17 19:59:13.000000 pytest_localftpserver-1.3.0/pytest_localftpserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-17 19:59:13.000000 pytest_localftpserver-1.3.0/pytest_localftpserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:59:13.000000 pytest_localftpserver-1.3.0/pytest_localftpserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-17 19:59:13.000000 pytest_localftpserver-1.3.0/pytest_localftpserver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-17 19:59:13.000000 pytest_localftpserver-1.3.0/pytest_localftpserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 19:59:13.000000 pytest_localftpserver-1.3.0/pytest_localftpserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:59:13.656431 pytest_localftpserver-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:13.656431 pytest_localftpserver-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/tests/not_a_valid_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/tests/test_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/tests/test_keycert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    27491 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/tests/test_pytest_localftpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/tests/test_pytest_localftpserver_TLS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/tests/test_pytest_localftpserver_with_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-17 19:59:09.000000 pytest_localftpserver-1.3.0/tox.ini
```

### Comparing `pytest_localftpserver-1.2.0/.coveragerc` & `pytest_localftpserver-1.3.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/.github/workflows/CI_CD_actions.yml` & `pytest_localftpserver-1.3.0/.github/workflows/CI_CD_actions.yml`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/.gitignore` & `pytest_localftpserver-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/CONTRIBUTING.rst` & `pytest_localftpserver-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/HISTORY.rst` & `pytest_localftpserver-1.3.0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/LICENSE` & `pytest_localftpserver-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/Makefile` & `pytest_localftpserver-1.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/PKG-INFO` & `pytest_localftpserver-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_localftpserver
-Version: 1.2.0
+Version: 1.3.0
 Summary: A PyTest plugin which provides an FTP fixture for your tests
 Author-email: Oz N Tiram <oz.tiram@gmail.com>
 Project-URL: homepage, https://github.com/oz123/pytest-localftpserver
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -23,14 +23,15 @@
 Classifier: Topic :: Software Development :: Testing :: Mocking
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: pyftpdlib>=1.2.0
 Requires-Dist: PyOpenSSL
 Requires-Dist: pytest
+Requires-Dist: wget
 
 PyTest FTP Server
 =================
 
 
 .. image:: https://img.shields.io/pypi/v/pytest_localftpserver.svg
         :target:  https://pypi.org/project/pytest-localftpserver/
```

### Comparing `pytest_localftpserver-1.2.0/README.rst` & `pytest_localftpserver-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/docs/Makefile` & `pytest_localftpserver-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/docs/_templates/autosummary/class.rst` & `pytest_localftpserver-1.3.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/docs/conf.py` & `pytest_localftpserver-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/docs/installation.rst` & `pytest_localftpserver-1.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/docs/make.bat` & `pytest_localftpserver-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/docs/usage.rst` & `pytest_localftpserver-1.3.0/docs/usage.rst`

 * *Files 2% similar despite different names*

```diff
@@ -64,22 +64,24 @@
 
 .. code-block:: python
 
     from ftplib import FTP_TLS
 
     from ssl import SSLContext
     try:
-        from ssl import PROTOCOL_TLS
+        from ssl import PROTOCOL_TLS_CLIENT, TLSVersion
     except Exception:
         from ssl import PROTOCOL_SSLv23 as PROTOCOL_TLS
 
 
     def test_TLS_login(ftpserver_TLS):
         if PYTHON3:
-            ssl_context = SSLContext(PROTOCOL_TLS)
+            ssl_context = SSLContext(PROTOCOL_TLS_CLIENT)
+            ssl_context.minimum_version = TLSVersion.TLSv1_2
+            ssl_context.maximum_version = TLSVersion.TLSv1_3
             ssl_context.load_cert_chain(certfile=DEFAULT_CERTFILE)
             ftp = FTP_TLS(context=ssl_context)
         else:
             ftp = FTP_TLS(certfile=DEFAULT_CERTFILE)
 
         login_dict = ftpserver_TLS.get_login_data()
         ftp.connect(login_dict["host"], login_dict["port"])
```

### Comparing `pytest_localftpserver-1.2.0/pyproject.toml` & `pytest_localftpserver-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=67.0.0", "wheel", "setuptools_scm[toml]>=6.2"]
+requires = ["setuptools>=67.0.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytest_localftpserver"
 dynamic = ["version"]
 description="A PyTest plugin which provides an FTP fixture for your tests"
 authors = [
@@ -29,15 +29,16 @@
   'Topic :: Software Development :: Testing',
   'Topic :: Software Development :: Testing :: Mocking'
 ]
 
 dependencies = [
   'pyftpdlib>=1.2.0',
   'PyOpenSSL',
-  'pytest'
+  'pytest',
+  'wget'
 ]
 
 [tool.setuptools]
 packages = ["pytest_localftpserver"]
 
 [project.entry-points.pytest11]
 localftpserver = "pytest_localftpserver.plugin"
```

### Comparing `pytest_localftpserver-1.2.0/pytest_localftpserver/default_keycert.pem` & `pytest_localftpserver-1.3.0/pytest_localftpserver/default_keycert.pem`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/pytest_localftpserver/helper_functions.py` & `pytest_localftpserver-1.3.0/pytest_localftpserver/helper_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import socket
 import sys
 from traceback import print_tb
 import warnings
 
 from ssl import SSLContext, SSLError
-from ssl import PROTOCOL_TLS
+from ssl import PROTOCOL_TLS_CLIENT, TLSVersion
 
 DEFAULT_CERTFILE = os.path.join(os.path.dirname(__file__),
                                 "default_keycert.pem")
 
 
 class InvalidCertificateError(Exception):
     pass
@@ -77,15 +77,17 @@
 
     InvalidCertificateError
         If the certificate is not valid.
 
     """
     cert_file = os.path.abspath(cert_file)
     try:
-        context = SSLContext(PROTOCOL_TLS)
+        context = SSLContext(PROTOCOL_TLS_CLIENT)
+        context.minimum_version = TLSVersion.TLSv1_2
+        context.maximum_version = TLSVersion.TLSv1_3
         context.load_cert_chain(cert_file)
     except SSLError as e:
         raise InvalidCertificateError("The certificate {}, you tried to use is not valid. "
                                       "Please make sure to use a working certificate or "
                                       "leave it unconfigured to use the default certificate. "
                                       "Details: {}"
                                       "".format(cert_file, e))
```

### Comparing `pytest_localftpserver-1.2.0/pytest_localftpserver/plugin.py` & `pytest_localftpserver-1.3.0/pytest_localftpserver/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/pytest_localftpserver/servers.py` & `pytest_localftpserver-1.3.0/pytest_localftpserver/servers.py`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/pytest_localftpserver.egg-info/PKG-INFO` & `pytest_localftpserver-1.3.0/pytest_localftpserver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pytest-localftpserver
-Version: 1.2.0
+Name: pytest_localftpserver
+Version: 1.3.0
 Summary: A PyTest plugin which provides an FTP fixture for your tests
 Author-email: Oz N Tiram <oz.tiram@gmail.com>
 Project-URL: homepage, https://github.com/oz123/pytest-localftpserver
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -23,14 +23,15 @@
 Classifier: Topic :: Software Development :: Testing :: Mocking
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: pyftpdlib>=1.2.0
 Requires-Dist: PyOpenSSL
 Requires-Dist: pytest
+Requires-Dist: wget
 
 PyTest FTP Server
 =================
 
 
 .. image:: https://img.shields.io/pypi/v/pytest_localftpserver.svg
         :target:  https://pypi.org/project/pytest-localftpserver/
```

### Comparing `pytest_localftpserver-1.2.0/pytest_localftpserver.egg-info/SOURCES.txt` & `pytest_localftpserver-1.3.0/pytest_localftpserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/tests/test_helper_functions.py` & `pytest_localftpserver-1.3.0/tests/test_helper_functions.py`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/tests/test_keycert.pem` & `pytest_localftpserver-1.3.0/tests/test_keycert.pem`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/tests/test_pytest_localftpserver.py` & `pytest_localftpserver-1.3.0/tests/test_pytest_localftpserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import wget
 
 from pytest_localftpserver.plugin import PytestLocalFTPServer
 from pytest_localftpserver.servers import USE_PROCESS
 from pytest_localftpserver.helper_functions import DEFAULT_CERTFILE
 
 
-from ssl import SSLContext, PROTOCOL_TLS
+from ssl import SSLContext, PROTOCOL_TLS_CLIENT, TLSVersion
 
 # HELPER FUNCTIONS
 
 
 FILE_LIST = [
     ("", "testfile1"),
     ("testdir", "testfile2"),
@@ -50,15 +50,17 @@
     Returns
     -------
     ftp: ftplib.FTP
         logged in FTP client
 
     """
     if use_TLS:
-        ssl_context = SSLContext(PROTOCOL_TLS)
+        ssl_context = SSLContext(PROTOCOL_TLS_CLIENT)
+        ssl_context.minimum_version = TLSVersion.TLSv1_2
+        ssl_context.maximum_version = TLSVersion.TLSv1_3
         ssl_context.load_cert_chain(certfile=DEFAULT_CERTFILE)
         ftp = FTP_TLS(context=ssl_context)
     else:
         ftp = FTP()
     login_dict = ftp_fixture.get_login_data()
     ftp.connect(login_dict["host"], login_dict["port"])
     if anon:
```

### Comparing `pytest_localftpserver-1.2.0/tests/test_pytest_localftpserver_TLS.py` & `pytest_localftpserver-1.3.0/tests/test_pytest_localftpserver_TLS.py`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/tests/test_pytest_localftpserver_with_env_var.py` & `pytest_localftpserver-1.3.0/tests/test_pytest_localftpserver_with_env_var.py`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.2.0/tox.ini` & `pytest_localftpserver-1.3.0/tox.ini`

 * *Files identical despite different names*

