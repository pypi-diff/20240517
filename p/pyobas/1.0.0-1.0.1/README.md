# Comparing `tmp/pyobas-1.0.0.tar.gz` & `tmp/pyobas-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobas-1.0.0.tar", last modified: Mon May 13 10:07:34 2024, max compression
+gzip compressed data, was "pyobas-1.0.1.tar", last modified: Thu May 16 21:11:15 2024, max compression
```

## Comparing `pyobas-1.0.0.tar` & `pyobas-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 10:07:34.549553 pyobas-1.0.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-13 10:07:24.000000 pyobas-1.0.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2024-05-13 10:07:34.549553 pyobas-1.0.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3159 2024-05-13 10:07:24.000000 pyobas-1.0.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 10:07:34.545553 pyobas-1.0.0/pyobas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/_version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 10:07:34.545553 pyobas-1.0.0/pyobas/apis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      497 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      643 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      532 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/collector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/document.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      890 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/inject.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      722 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/injector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      397 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/me.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/organization.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/team.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/user.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 10:07:34.545553 pyobas-1.0.0/pyobas/backends/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/backends/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4328 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/backends/backend.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/backends/protocol.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16141 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 10:07:34.549553 pyobas-1.0.0/pyobas/contracts/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/contracts/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/contracts/contract_builder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5582 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/contracts/contract_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/contracts/contract_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4208 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/contracts/variable_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14284 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/helpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/mixins.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3865 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 10:07:34.549553 pyobas-1.0.0/pyobas.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2024-05-13 10:07:34.000000 pyobas-1.0.0/pyobas.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2024-05-13 10:07:34.000000 pyobas-1.0.0/pyobas.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-13 10:07:34.000000 pyobas-1.0.0/pyobas.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2024-05-13 10:07:34.000000 pyobas-1.0.0/pyobas.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-13 10:07:34.000000 pyobas-1.0.0/pyobas.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1386 2024-05-13 10:07:34.549553 pyobas-1.0.0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 21:11:15.474918 pyobas-1.0.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-16 21:11:04.000000 pyobas-1.0.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2024-05-16 21:11:15.474918 pyobas-1.0.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3159 2024-05-16 21:11:04.000000 pyobas-1.0.1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 21:11:15.466917 pyobas-1.0.1/pyobas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 21:11:15.470918 pyobas-1.0.1/pyobas/apis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      497 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/apis/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      643 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/apis/attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      532 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/apis/collector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/apis/document.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      890 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/apis/inject.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      722 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/apis/injector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/apis/kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      397 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/apis/me.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/apis/organization.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/apis/team.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/apis/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 21:11:15.470918 pyobas-1.0.1/pyobas/backends/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/backends/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4328 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/backends/backend.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/backends/protocol.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16141 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 21:11:15.470918 pyobas-1.0.1/pyobas/contracts/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/contracts/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/contracts/contract_builder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5582 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/contracts/contract_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/contracts/contract_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4208 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/contracts/variable_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14284 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/mixins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3865 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyobas/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 21:11:15.470918 pyobas-1.0.1/pyobas.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2024-05-16 21:11:15.000000 pyobas-1.0.1/pyobas.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2024-05-16 21:11:15.000000 pyobas-1.0.1/pyobas.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-16 21:11:15.000000 pyobas-1.0.1/pyobas.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2024-05-16 21:11:15.000000 pyobas-1.0.1/pyobas.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-16 21:11:15.000000 pyobas-1.0.1/pyobas.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-16 21:11:04.000000 pyobas-1.0.1/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1386 2024-05-16 21:11:15.474918 pyobas-1.0.1/setup.cfg
```

### Comparing `pyobas-1.0.0/LICENSE` & `pyobas-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/PKG-INFO` & `pyobas-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobas
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python API client for OpenBAS.
 Home-page: https://github.com/OpenBAS-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,20 +30,20 @@
 Requires-Dist: requests-toolbelt~=1.0.0
 Requires-Dist: setuptools~=69.5.1
 Provides-Extra: dev
 Requires-Dist: black~=24.4.0; extra == "dev"
 Requires-Dist: build~=1.2.1; extra == "dev"
 Requires-Dist: isort~=5.13.0; extra == "dev"
 Requires-Dist: types-pytz~=2024.1.0.20240203; extra == "dev"
-Requires-Dist: pre-commit~=3.6.0; extra == "dev"
+Requires-Dist: pre-commit~=3.7.1; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9.0; extra == "dev"
 Requires-Dist: wheel~=0.43.0; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: autoapi~=2.0.1; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints~=2.0.0; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints~=2.1.0; extra == "doc"
 Requires-Dist: sphinx-rtd-theme~=2.0.0; extra == "doc"
 
 # OpenBAS client for Python
 
 [![Website](https://img.shields.io/badge/website-openbas.io-blue.svg)](https://openbas.io)
 [![CircleCI](https://circleci.com/gh/OpenBAS-Platform/client-python.svg?style=shield)](https://circleci.com/gh/OpenBAS-Platform/client-python/tree/main)
 [![readthedocs](https://readthedocs.org/projects/openbas-client-for-python/badge/?style=flat)](https://openbas-client-for-python.readthedocs.io/en/latest/)
```

### Comparing `pyobas-1.0.0/README.md` & `pyobas-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/__init__.py` & `pyobas-1.0.1/pyobas/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 from pyobas._version import (  # noqa: F401
     __author__,
     __copyright__,
     __email__,
     __license__,
     __title__,
```

### Comparing `pyobas-1.0.0/pyobas/apis/attack_pattern.py` & `pyobas-1.0.1/pyobas/apis/attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/apis/collector.py` & `pyobas-1.0.1/pyobas/apis/collector.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/apis/document.py` & `pyobas-1.0.1/pyobas/apis/document.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/apis/inject.py` & `pyobas-1.0.1/pyobas/apis/inject.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/apis/injector.py` & `pyobas-1.0.1/pyobas/apis/injector.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/apis/kill_chain_phase.py` & `pyobas-1.0.1/pyobas/apis/kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/apis/team.py` & `pyobas-1.0.1/pyobas/apis/team.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/apis/user.py` & `pyobas-1.0.1/pyobas/apis/user.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/backends/backend.py` & `pyobas-1.0.1/pyobas/backends/backend.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/backends/protocol.py` & `pyobas-1.0.1/pyobas/backends/protocol.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/base.py` & `pyobas-1.0.1/pyobas/base.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/client.py` & `pyobas-1.0.1/pyobas/client.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/contracts/contract_builder.py` & `pyobas-1.0.1/pyobas/contracts/contract_builder.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/contracts/contract_config.py` & `pyobas-1.0.1/pyobas/contracts/contract_config.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/contracts/variable_helper.py` & `pyobas-1.0.1/pyobas/contracts/variable_helper.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/exceptions.py` & `pyobas-1.0.1/pyobas/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/helpers.py` & `pyobas-1.0.1/pyobas/helpers.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/mixins.py` & `pyobas-1.0.1/pyobas/mixins.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/utils.py` & `pyobas-1.0.1/pyobas/utils.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas.egg-info/PKG-INFO` & `pyobas-1.0.1/pyobas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobas
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python API client for OpenBAS.
 Home-page: https://github.com/OpenBAS-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,20 +30,20 @@
 Requires-Dist: requests-toolbelt~=1.0.0
 Requires-Dist: setuptools~=69.5.1
 Provides-Extra: dev
 Requires-Dist: black~=24.4.0; extra == "dev"
 Requires-Dist: build~=1.2.1; extra == "dev"
 Requires-Dist: isort~=5.13.0; extra == "dev"
 Requires-Dist: types-pytz~=2024.1.0.20240203; extra == "dev"
-Requires-Dist: pre-commit~=3.6.0; extra == "dev"
+Requires-Dist: pre-commit~=3.7.1; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9.0; extra == "dev"
 Requires-Dist: wheel~=0.43.0; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: autoapi~=2.0.1; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints~=2.0.0; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints~=2.1.0; extra == "doc"
 Requires-Dist: sphinx-rtd-theme~=2.0.0; extra == "doc"
 
 # OpenBAS client for Python
 
 [![Website](https://img.shields.io/badge/website-openbas.io-blue.svg)](https://openbas.io)
 [![CircleCI](https://circleci.com/gh/OpenBAS-Platform/client-python.svg?style=shield)](https://circleci.com/gh/OpenBAS-Platform/client-python/tree/main)
 [![readthedocs](https://readthedocs.org/projects/openbas-client-for-python/badge/?style=flat)](https://openbas-client-for-python.readthedocs.io/en/latest/)
```

### Comparing `pyobas-1.0.0/pyobas.egg-info/SOURCES.txt` & `pyobas-1.0.1/pyobas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyproject.toml` & `pyobas-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/setup.cfg` & `pyobas-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -42,19 +42,19 @@
 
 [options.extras_require]
 dev = 
 	black~=24.4.0
 	build~=1.2.1
 	isort~=5.13.0
 	types-pytz~=2024.1.0.20240203
-	pre-commit~=3.6.0
+	pre-commit~=3.7.1
 	types-python-dateutil~=2.9.0
 	wheel~=0.43.0
 doc = 
 	autoapi~=2.0.1
-	sphinx-autodoc-typehints~=2.0.0
+	sphinx-autodoc-typehints~=2.1.0
 	sphinx-rtd-theme~=2.0.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

