# Comparing `tmp/open_api_framework-0.1.0.tar.gz` & `tmp/open_api_framework-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_api_framework-0.1.0.tar", last modified: Tue Jan 30 15:01:01 2024, max compression
+gzip compressed data, was "open_api_framework-0.2.0.tar", last modified: Fri Mar 22 14:57:57 2024, max compression
```

## Comparing `open_api_framework-0.1.0.tar` & `open_api_framework-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:01:01.289497 open_api_framework-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-01-30 15:00:54.000000 open_api_framework-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-30 15:00:54.000000 open_api_framework-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-01-30 15:01:01.289497 open_api_framework-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-01-30 15:00:54.000000 open_api_framework-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:01:01.285497 open_api_framework-0.1.0/open_api_framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:00:54.000000 open_api_framework-0.1.0/open_api_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-01-30 15:00:54.000000 open_api_framework-0.1.0/open_api_framework/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:00:54.000000 open_api_framework-0.1.0/open_api_framework/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:01:01.285497 open_api_framework-0.1.0/open_api_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-01-30 15:01:01.000000 open_api_framework-0.1.0/open_api_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-01-30 15:01:01.000000 open_api_framework-0.1.0/open_api_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 15:01:01.000000 open_api_framework-0.1.0/open_api_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-01-30 15:01:01.000000 open_api_framework-0.1.0/open_api_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-30 15:01:01.000000 open_api_framework-0.1.0/open_api_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-01-30 15:00:54.000000 open_api_framework-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-30 15:01:01.289497 open_api_framework-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:01:01.285497 open_api_framework-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-30 15:00:54.000000 open_api_framework-0.1.0/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:57:57.221083 open_api_framework-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-22 14:57:53.000000 open_api_framework-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-22 14:57:53.000000 open_api_framework-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-03-22 14:57:57.221083 open_api_framework-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-03-22 14:57:53.000000 open_api_framework-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:57:57.217083 open_api_framework-0.2.0/open_api_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:57:53.000000 open_api_framework-0.2.0/open_api_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-22 14:57:53.000000 open_api_framework-0.2.0/open_api_framework/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:57:53.000000 open_api_framework-0.2.0/open_api_framework/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:57:57.221083 open_api_framework-0.2.0/open_api_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-03-22 14:57:57.000000 open_api_framework-0.2.0/open_api_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-22 14:57:57.000000 open_api_framework-0.2.0/open_api_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 14:57:57.000000 open_api_framework-0.2.0/open_api_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-22 14:57:57.000000 open_api_framework-0.2.0/open_api_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-22 14:57:57.000000 open_api_framework-0.2.0/open_api_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-03-22 14:57:53.000000 open_api_framework-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-22 14:57:57.221083 open_api_framework-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:57:57.221083 open_api_framework-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-22 14:57:53.000000 open_api_framework-0.2.0/tests/test_dummy.py
```

### Comparing `open_api_framework-0.1.0/LICENSE` & `open_api_framework-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open_api_framework-0.1.0/PKG-INFO` & `open_api_framework-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_api_framework
-Version: 0.1.0
+Version: 0.2.0
 Summary: TODO
 Author-email: Maykin Media <support@maykinmedia.nl>
 License: Copyright 2024 Maykin Media
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -14,28 +14,27 @@
 Project-URL: Homepage, https://github.com/maykinmedia/open_api_framework
 Project-URL: Documentation, http://open_api_framework.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/maykinmedia/open_api_framework/issues
 Project-URL: Source Code, https://github.com/maykinmedia/open_api_framework
 Keywords: TODO
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: django>=3.2.23
+Requires-Dist: django>=4.2.11
 Requires-Dist: django-axes>=6.3.0
 Requires-Dist: django-cors-headers>=4.3.1
 Requires-Dist: django-markup>=1.8.1
 Requires-Dist: django-jsonform>=2.21.4
 Requires-Dist: django-admin-index>=3.1.0
 Requires-Dist: django-redis>=5.4.0
 Requires-Dist: djangorestframework>=3.12.4
@@ -52,14 +51,15 @@
 Requires-Dist: python-decouple>=3.8
 Requires-Dist: requests>=2.31.0
 Requires-Dist: uwsgi>=2.0.23
 Requires-Dist: sentry-sdk>=1.39.2
 Requires-Dist: elastic-apm>=6.20.0
 Requires-Dist: celery>=5.2.7
 Requires-Dist: flower>=2.0.1
+Requires-Dist: maykin-2fa>=1.0.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-django; extra == "tests"
 Requires-Dist: tox; extra == "tests"
 Requires-Dist: isort; extra == "tests"
 Requires-Dist: black; extra == "tests"
 Requires-Dist: flake8; extra == "tests"
@@ -70,60 +70,52 @@
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Provides-Extra: release
 Requires-Dist: bump-my-version; extra == "release"
 Requires-Dist: twine; extra == "release"
 
 
 
-Welcome to open_api_framework's documentation!
+Welcome to open-api-framework's documentation!
 =================================================
 
-:Version: 0.1.0
-:Source: https://github.com/maykinmedia/open_api_framework
-:Keywords: ``<keywords>``
-:PythonVersion: 3.11
+:Version: 0.2.0
+:Source: https://github.com/maykinmedia/open-api-framework
+:Keywords: metapackage, dependencies
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
 
-<One liner describing the project>
+A metapackage for registration components, that bundles the dependencies shared between these components
 
 .. contents::
 
 .. section-numbering::
 
 Features
 ========
 
-* ...
-* ...
+* Bundling shared dependencies and introducing minimum versions for these dependencies
 
 Installation
 ============
 
 Requirements
 ------------
 
-* Python 3.9/3.11 or above
-* Django 3.2/4.2 or newer
+* Python 3.9 or above
+* Django 4.2 or newer
 
 
 Install
 -------
 
-.. code-block:: bash
-
-    pip install open_api_framework
-
-
-Usage
-=====
-
-<document or refer to docs>
+1. Add open-api-framework to your requirements file
+2. Remove dependencies from your requirements file that occur in ``pyproject.toml``
+3. Recompile the dependencies
 
 Local development
 =================
 
 To install and develop the library locally, use::
 
 .. code-block:: bash
@@ -137,32 +129,32 @@
 
     export PYTHONPATH=. DJANGO_SETTINGS_MODULE=testapp.settings
     django-admin check
     # or other commands like:
     # django-admin makemessages -l nl
 
 
-.. |build-status| image:: https://github.com/maykinmedia/open_api_framework/workflows/Run%20CI/badge.svg
+.. |build-status| image:: https://github.com/maykinmedia/open-api-framework/workflows/Run%20CI/badge.svg
     :alt: Build status
-    :target: https://github.com/maykinmedia/open_api_framework/actions?query=workflow%3A%22Run+CI%22
+    :target: https://github.com/maykinmedia/open-api-framework/actions?query=workflow%3A%22Run+CI%22
 
-.. |code-quality| image:: https://github.com/maykinmedia/open_api_framework/workflows/Code%20quality%20checks/badge.svg
+.. |code-quality| image:: https://github.com/maykinmedia/open-api-framework/workflows/Code%20quality%20checks/badge.svg
      :alt: Code quality checks
-     :target: https://github.com/maykinmedia/open_api_framework/actions?query=workflow%3A%22Code+quality+checks%22
+     :target: https://github.com/maykinmedia/open-api-framework/actions?query=workflow%3A%22Code+quality+checks%22
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
-.. |coverage| image:: https://codecov.io/gh/maykinmedia/open_api_framework/branch/main/graph/badge.svg
-    :target: https://codecov.io/gh/maykinmedia/open_api_framework
+.. |coverage| image:: https://codecov.io/gh/maykinmedia/open-api-framework/branch/main/graph/badge.svg
+    :target: https://codecov.io/gh/maykinmedia/open-api-framework
     :alt: Coverage status
 
-.. |docs| image:: https://readthedocs.org/projects/open_api_framework/badge/?version=latest
-    :target: https://open_api_framework.readthedocs.io/en/latest/?badge=latest
+.. |docs| image:: https://readthedocs.org/projects/open-api-framework/badge/?version=latest
+    :target: https://open-api-framework.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. |python-versions| image:: https://img.shields.io/pypi/pyversions/open_api_framework.svg
+.. |python-versions| image:: https://img.shields.io/pypi/pyversions/open-api-framework.svg
 
-.. |django-versions| image:: https://img.shields.io/pypi/djversions/open_api_framework.svg
+.. |django-versions| image:: https://img.shields.io/pypi/djversions/open-api-framework.svg
 
-.. |pypi-version| image:: https://img.shields.io/pypi/v/open_api_framework.svg
-    :target: https://pypi.org/project/open_api_framework/
+.. |pypi-version| image:: https://img.shields.io/pypi/v/open-api-framework.svg
+    :target: https://pypi.org/project/open-api-framework/
```

### Comparing `open_api_framework-0.1.0/open_api_framework.egg-info/PKG-INFO` & `open_api_framework-0.2.0/open_api_framework.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_api_framework
-Version: 0.1.0
+Version: 0.2.0
 Summary: TODO
 Author-email: Maykin Media <support@maykinmedia.nl>
 License: Copyright 2024 Maykin Media
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -14,28 +14,27 @@
 Project-URL: Homepage, https://github.com/maykinmedia/open_api_framework
 Project-URL: Documentation, http://open_api_framework.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/maykinmedia/open_api_framework/issues
 Project-URL: Source Code, https://github.com/maykinmedia/open_api_framework
 Keywords: TODO
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: django>=3.2.23
+Requires-Dist: django>=4.2.11
 Requires-Dist: django-axes>=6.3.0
 Requires-Dist: django-cors-headers>=4.3.1
 Requires-Dist: django-markup>=1.8.1
 Requires-Dist: django-jsonform>=2.21.4
 Requires-Dist: django-admin-index>=3.1.0
 Requires-Dist: django-redis>=5.4.0
 Requires-Dist: djangorestframework>=3.12.4
@@ -52,14 +51,15 @@
 Requires-Dist: python-decouple>=3.8
 Requires-Dist: requests>=2.31.0
 Requires-Dist: uwsgi>=2.0.23
 Requires-Dist: sentry-sdk>=1.39.2
 Requires-Dist: elastic-apm>=6.20.0
 Requires-Dist: celery>=5.2.7
 Requires-Dist: flower>=2.0.1
+Requires-Dist: maykin-2fa>=1.0.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-django; extra == "tests"
 Requires-Dist: tox; extra == "tests"
 Requires-Dist: isort; extra == "tests"
 Requires-Dist: black; extra == "tests"
 Requires-Dist: flake8; extra == "tests"
@@ -70,60 +70,52 @@
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Provides-Extra: release
 Requires-Dist: bump-my-version; extra == "release"
 Requires-Dist: twine; extra == "release"
 
 
 
-Welcome to open_api_framework's documentation!
+Welcome to open-api-framework's documentation!
 =================================================
 
-:Version: 0.1.0
-:Source: https://github.com/maykinmedia/open_api_framework
-:Keywords: ``<keywords>``
-:PythonVersion: 3.11
+:Version: 0.2.0
+:Source: https://github.com/maykinmedia/open-api-framework
+:Keywords: metapackage, dependencies
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
 
-<One liner describing the project>
+A metapackage for registration components, that bundles the dependencies shared between these components
 
 .. contents::
 
 .. section-numbering::
 
 Features
 ========
 
-* ...
-* ...
+* Bundling shared dependencies and introducing minimum versions for these dependencies
 
 Installation
 ============
 
 Requirements
 ------------
 
-* Python 3.9/3.11 or above
-* Django 3.2/4.2 or newer
+* Python 3.9 or above
+* Django 4.2 or newer
 
 
 Install
 -------
 
-.. code-block:: bash
-
-    pip install open_api_framework
-
-
-Usage
-=====
-
-<document or refer to docs>
+1. Add open-api-framework to your requirements file
+2. Remove dependencies from your requirements file that occur in ``pyproject.toml``
+3. Recompile the dependencies
 
 Local development
 =================
 
 To install and develop the library locally, use::
 
 .. code-block:: bash
@@ -137,32 +129,32 @@
 
     export PYTHONPATH=. DJANGO_SETTINGS_MODULE=testapp.settings
     django-admin check
     # or other commands like:
     # django-admin makemessages -l nl
 
 
-.. |build-status| image:: https://github.com/maykinmedia/open_api_framework/workflows/Run%20CI/badge.svg
+.. |build-status| image:: https://github.com/maykinmedia/open-api-framework/workflows/Run%20CI/badge.svg
     :alt: Build status
-    :target: https://github.com/maykinmedia/open_api_framework/actions?query=workflow%3A%22Run+CI%22
+    :target: https://github.com/maykinmedia/open-api-framework/actions?query=workflow%3A%22Run+CI%22
 
-.. |code-quality| image:: https://github.com/maykinmedia/open_api_framework/workflows/Code%20quality%20checks/badge.svg
+.. |code-quality| image:: https://github.com/maykinmedia/open-api-framework/workflows/Code%20quality%20checks/badge.svg
      :alt: Code quality checks
-     :target: https://github.com/maykinmedia/open_api_framework/actions?query=workflow%3A%22Code+quality+checks%22
+     :target: https://github.com/maykinmedia/open-api-framework/actions?query=workflow%3A%22Code+quality+checks%22
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
-.. |coverage| image:: https://codecov.io/gh/maykinmedia/open_api_framework/branch/main/graph/badge.svg
-    :target: https://codecov.io/gh/maykinmedia/open_api_framework
+.. |coverage| image:: https://codecov.io/gh/maykinmedia/open-api-framework/branch/main/graph/badge.svg
+    :target: https://codecov.io/gh/maykinmedia/open-api-framework
     :alt: Coverage status
 
-.. |docs| image:: https://readthedocs.org/projects/open_api_framework/badge/?version=latest
-    :target: https://open_api_framework.readthedocs.io/en/latest/?badge=latest
+.. |docs| image:: https://readthedocs.org/projects/open-api-framework/badge/?version=latest
+    :target: https://open-api-framework.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. |python-versions| image:: https://img.shields.io/pypi/pyversions/open_api_framework.svg
+.. |python-versions| image:: https://img.shields.io/pypi/pyversions/open-api-framework.svg
 
-.. |django-versions| image:: https://img.shields.io/pypi/djversions/open_api_framework.svg
+.. |django-versions| image:: https://img.shields.io/pypi/djversions/open-api-framework.svg
 
-.. |pypi-version| image:: https://img.shields.io/pypi/v/open_api_framework.svg
-    :target: https://pypi.org/project/open_api_framework/
+.. |pypi-version| image:: https://img.shields.io/pypi/v/open-api-framework.svg
+    :target: https://pypi.org/project/open-api-framework/
```

### Comparing `open_api_framework-0.1.0/open_api_framework.egg-info/requires.txt` & `open_api_framework-0.2.0/open_api_framework.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-django>=3.2.23
+django>=4.2.11
 django-axes>=6.3.0
 django-cors-headers>=4.3.1
 django-markup>=1.8.1
 django-jsonform>=2.21.4
 django-admin-index>=3.1.0
 django-redis>=5.4.0
 djangorestframework>=3.12.4
@@ -19,14 +19,15 @@
 python-decouple>=3.8
 requests>=2.31.0
 uwsgi>=2.0.23
 sentry-sdk>=1.39.2
 elastic-apm>=6.20.0
 celery>=5.2.7
 flower>=2.0.1
+maykin-2fa>=1.0.0
 
 [coverage]
 pytest-cov
 
 [docs]
 sphinx
 sphinx-rtd-theme
```

### Comparing `open_api_framework-0.1.0/pyproject.toml` & `open_api_framework-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "open_api_framework"
-version = "0.1.0"
+version = "0.2.0"
 description = "TODO"
 authors = [
     {name = "Maykin Media", email = "support@maykinmedia.nl"}
 ]
 readme = "README.rst"
 license = {file = "LICENSE"}
 keywords = ["TODO"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: Django",
-    "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 requires-python = ">=3.9"
 dependencies = [
-    "django>=3.2.23",
+    "django>=4.2.11",
     "django-axes>=6.3.0",
     "django-cors-headers>=4.3.1",
     "django-markup>=1.8.1",
     "django-jsonform>=2.21.4",
     "django-admin-index>=3.1.0",
     "django-redis>=5.4.0",
     "djangorestframework>=3.12.4",
@@ -49,14 +48,15 @@
     "python-decouple>=3.8",
     "requests>=2.31.0",
     "uwsgi>=2.0.23",
     "sentry-sdk>=1.39.2",
     "elastic-apm>=6.20.0",
     "celery>=5.2.7",
     "flower>=2.0.1",
+    "maykin-2fa>=1.0.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/maykinmedia/open_api_framework"
 Documentation = "http://open_api_framework.readthedocs.io/en/latest/"
 "Bug Tracker" = "https://github.com/maykinmedia/open_api_framework/issues"
 "Source Code" = "https://github.com/maykinmedia/open_api_framework"
@@ -94,15 +94,15 @@
 sections=["FUTURE", "STDLIB", "DJANGO", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 DJANGO_SETTINGS_MODULE = "testapp.settings"
 
 [tool.bumpversion]
-current_version = "0.1.0"
+current_version = "0.2.0"
 files = [
     {filename = "pyproject.toml"},
     {filename = "README.rst"},
     {filename = "docs/conf.py"},
 ]
 
 [tool.coverage.report]
```

