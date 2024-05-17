# Comparing `tmp/allen1989-0.1.0.tar.gz` & `tmp/allen1989-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allen1989-0.1.0.tar", last modified: Sat Oct 30 12:40:18 2021, max compression
+gzip compressed data, was "allen1989-0.2.0.tar", last modified: Fri May 17 07:59:23 2024, max compression
```

## Comparing `allen1989-0.1.0.tar` & `allen1989-0.2.0.tar`

### file list

```diff
@@ -1,57 +1,53 @@
-drwxrwxrwx   0        0        0        0 2021-10-30 12:40:18.070190 allen1989-0.1.0/
--rw-rw-rw-   0        0        0      316 2021-10-30 12:35:23.000000 allen1989-0.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3312 2021-10-30 12:35:23.000000 allen1989-0.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2021-10-30 12:35:23.000000 allen1989-0.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2021-10-30 12:35:23.000000 allen1989-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      437 2021-10-30 12:35:23.000000 allen1989-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2674 2021-10-30 12:40:18.070190 allen1989-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1467 2021-10-30 12:35:23.000000 allen1989-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2021-10-30 12:40:18.000100 allen1989-0.1.0/doc/
--rw-rw-rw-   0        0        0     6967 2021-10-30 12:35:23.000000 allen1989-0.1.0/doc/Makefile
-drwxrwxrwx   0        0        0        0 2021-10-30 12:40:18.014893 allen1989-0.1.0/doc/_dvlpt/
--rw-rw-rw-   0        0        0      134 2021-10-30 12:39:08.000000 allen1989-0.1.0/doc/_dvlpt/allen1989.raw.rst
--rw-rw-rw-   0        0        0      284 2021-10-30 12:39:08.000000 allen1989-0.1.0/doc/_dvlpt/allen1989.rst
--rw-rw-rw-   0        0        0      149 2021-10-30 12:39:08.000000 allen1989-0.1.0/doc/_dvlpt/allen1989.transfer.rst
--rw-rw-rw-   0        0        0      146 2021-10-30 12:39:08.000000 allen1989-0.1.0/doc/_dvlpt/allen1989.version.rst
--rw-rw-rw-   0        0        0       59 2021-10-30 12:39:08.000000 allen1989-0.1.0/doc/_dvlpt/modules.rst
-drwxrwxrwx   0        0        0        0 2021-10-30 12:40:18.019902 allen1989-0.1.0/doc/_gallery/
--rw-rw-rw-   0        0        0      924 2021-10-30 12:39:10.000000 allen1989-0.1.0/doc/_gallery/index.rst
--rw-rw-rw-   0        0        0     2189 2021-10-30 12:39:10.000000 allen1989-0.1.0/doc/_gallery/plot_heat_conductance.rst
--rw-rw-rw-   0        0        0      468 2021-10-30 12:39:10.000000 allen1989-0.1.0/doc/_gallery/sg_execution_times.rst
--rw-rw-rw-   0        0        0       29 2021-10-30 12:35:23.000000 allen1989-0.1.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2021-10-30 12:40:18.024947 allen1989-0.1.0/doc/badges/
--rw-rw-rw-   0        0        0      227 2021-10-30 12:35:23.000000 allen1989-0.1.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2021-10-30 12:40:18.029962 allen1989-0.1.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2021-10-30 12:35:23.000000 allen1989-0.1.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5086 2021-10-30 12:35:23.000000 allen1989-0.1.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2021-10-30 12:35:23.000000 allen1989-0.1.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2021-10-30 12:35:23.000000 allen1989-0.1.0/doc/history.rst
--rw-rw-rw-   0        0        0      593 2021-10-30 12:35:23.000000 allen1989-0.1.0/doc/index.rst
--rw-rw-rw-   0        0        0      164 2021-10-30 12:35:23.000000 allen1989-0.1.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2021-10-30 12:35:23.000000 allen1989-0.1.0/doc/make.bat
--rw-rw-rw-   0        0        0      128 2021-10-30 12:35:23.000000 allen1989-0.1.0/doc/management.rst
--rw-rw-rw-   0        0        0     1387 2021-10-30 12:35:23.000000 allen1989-0.1.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2021-10-30 12:35:23.000000 allen1989-0.1.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2021-10-30 12:40:18.035003 allen1989-0.1.0/doc/user/
--rw-rw-rw-   0        0        0       83 2021-10-30 12:35:23.000000 allen1989-0.1.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2021-10-30 12:35:23.000000 allen1989-0.1.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      310 2021-10-30 12:35:23.000000 allen1989-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       29 2021-10-30 12:35:23.000000 allen1989-0.1.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2021-10-30 12:40:18.075224 allen1989-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1857 2021-10-30 12:35:23.000000 allen1989-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-10-30 12:40:17.925278 allen1989-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2021-10-30 12:40:18.045079 allen1989-0.1.0/src/allen1989/
--rw-rw-rw-   0        0        0      182 2021-10-30 12:35:23.000000 allen1989-0.1.0/src/allen1989/__init__.py
--rw-rw-rw-   0        0        0      665 2021-10-25 08:22:34.000000 allen1989-0.1.0/src/allen1989/raw.py
--rw-rw-rw-   0        0        0      779 2021-10-25 08:08:52.000000 allen1989-0.1.0/src/allen1989/transfer.py
--rw-rw-rw-   0        0        0      367 2021-10-30 12:35:23.000000 allen1989-0.1.0/src/allen1989/version.py
-drwxrwxrwx   0        0        0        0 2021-10-30 12:40:18.055122 allen1989-0.1.0/src/allen1989.egg-info/
--rw-rw-rw-   0        0        0     2674 2021-10-30 12:40:17.000000 allen1989-0.1.0/src/allen1989.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      978 2021-10-30 12:40:17.000000 allen1989-0.1.0/src/allen1989.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-30 12:40:17.000000 allen1989-0.1.0/src/allen1989.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-10-25 07:49:56.000000 allen1989-0.1.0/src/allen1989.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2021-10-30 12:40:17.000000 allen1989-0.1.0/src/allen1989.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-10-30 12:40:18.070190 allen1989-0.1.0/test/
--rw-rw-rw-   0        0        0      973 2021-10-30 12:35:23.000000 allen1989-0.1.0/test/conftest.py
--rw-rw-rw-   0        0        0       84 2021-10-30 12:35:23.000000 allen1989-0.1.0/test/test_packaging.py
--rw-rw-rw-   0        0        0      446 2021-10-25 08:12:31.000000 allen1989-0.1.0/test/test_transfer.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:59:23.349912 allen1989-0.2.0/
+-rw-rw-rw-   0        0        0      316 2024-05-17 07:51:44.000000 allen1989-0.2.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3319 2024-05-17 07:51:44.000000 allen1989-0.2.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-17 07:51:44.000000 allen1989-0.2.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-17 07:51:44.000000 allen1989-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2785 2024-05-17 07:59:23.348914 allen1989-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1123 2024-05-17 07:51:44.000000 allen1989-0.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:59:23.318915 allen1989-0.2.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-17 07:51:44.000000 allen1989-0.2.0/doc/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-17 07:59:23.322914 allen1989-0.2.0/doc/_gallery/
+-rw-rw-rw-   0        0        0      924 2021-10-30 12:39:10.000000 allen1989-0.2.0/doc/_gallery/index.rst
+-rw-rw-rw-   0        0        0     2189 2021-10-30 12:39:10.000000 allen1989-0.2.0/doc/_gallery/plot_heat_conductance.rst
+-rw-rw-rw-   0        0        0      468 2021-10-30 12:39:10.000000 allen1989-0.2.0/doc/_gallery/sg_execution_times.rst
+-rw-rw-rw-   0        0        0       29 2024-05-17 07:51:44.000000 allen1989-0.2.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:59:23.323914 allen1989-0.2.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-17 07:51:44.000000 allen1989-0.2.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:59:23.324913 allen1989-0.2.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-17 07:51:44.000000 allen1989-0.2.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5086 2024-05-17 07:51:44.000000 allen1989-0.2.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-17 07:51:44.000000 allen1989-0.2.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-17 07:51:44.000000 allen1989-0.2.0/doc/history.rst
+-rw-rw-rw-   0        0        0      593 2024-05-17 07:51:44.000000 allen1989-0.2.0/doc/index.rst
+-rw-rw-rw-   0        0        0      219 2024-05-17 07:51:44.000000 allen1989-0.2.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-17 07:51:44.000000 allen1989-0.2.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-17 07:51:44.000000 allen1989-0.2.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1051 2024-05-17 07:51:44.000000 allen1989-0.2.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-17 07:51:44.000000 allen1989-0.2.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:59:23.327915 allen1989-0.2.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-17 07:51:44.000000 allen1989-0.2.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-17 07:51:44.000000 allen1989-0.2.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2243 2024-05-17 07:51:44.000000 allen1989-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      310 2024-05-17 07:51:44.000000 allen1989-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-17 07:51:44.000000 allen1989-0.2.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 07:59:23.350915 allen1989-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 07:59:23.289548 allen1989-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 07:59:23.333914 allen1989-0.2.0/src/allen1989/
+-rw-rw-rw-   0        0        0      247 2024-05-17 07:51:44.000000 allen1989-0.2.0/src/allen1989/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:59:23.341914 allen1989-0.2.0/src/allen1989/clean/
+-rw-rw-rw-   0        0        0      134 2024-05-17 07:51:44.000000 allen1989-0.2.0/src/allen1989/clean/readme.rst
+-rw-rw-rw-   0        0        0      379 2024-05-17 07:51:44.000000 allen1989-0.2.0/src/allen1989/info.py
+-rw-rw-rw-   0        0        0      665 2021-10-25 08:22:34.000000 allen1989-0.2.0/src/allen1989/raw.py
+-rw-rw-rw-   0        0        0      779 2021-10-25 08:08:52.000000 allen1989-0.2.0/src/allen1989/transfer.py
+-rw-rw-rw-   0        0        0      367 2024-05-17 07:51:44.000000 allen1989-0.2.0/src/allen1989/version.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:59:23.347914 allen1989-0.2.0/src/allen1989.egg-info/
+-rw-rw-rw-   0        0        0     2785 2024-05-17 07:59:23.000000 allen1989-0.2.0/src/allen1989.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      871 2024-05-17 07:59:23.000000 allen1989-0.2.0/src/allen1989.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 07:59:23.000000 allen1989-0.2.0/src/allen1989.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2024-05-17 07:59:23.000000 allen1989-0.2.0/src/allen1989.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-17 07:59:23.000000 allen1989-0.2.0/src/allen1989.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 07:59:23.345914 allen1989-0.2.0/test/
+-rw-rw-rw-   0        0        0      985 2024-05-17 07:51:44.000000 allen1989-0.2.0/test/conftest.py
+-rw-rw-rw-   0        0        0      377 2024-05-17 07:51:44.000000 allen1989-0.2.0/test/test_packaging.py
+-rw-rw-rw-   0        0        0      452 2024-05-17 07:02:57.000000 allen1989-0.2.0/test/test_transfer.py
```

### Comparing `allen1989-0.1.0/CONTRIBUTING.rst` & `allen1989-0.2.0/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
   1. The pull request should include tests.
   2. If the pull request adds functionality, the docs should be updated. Put
      your new functionality into a function with a docstring, and add the
      feature to the list in README.rst.
-  3. The pull request should work for Python 39.
+  3. The pull request should work for Python 3.9, 3.12.
      
 
 Tips
 ----
 
 
 To run a subset of tests::
```

### Comparing `allen1989-0.1.0/LICENSE` & `allen1989-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `allen1989-0.1.0/PKG-INFO` & `allen1989-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,76 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: allen1989
-Version: 0.1.0
+Version: 0.2.0
 Summary: Formalisms from Allen at al. 1989 paper
-Home-page: https://gitlab.com/b326/allen1989
-Author: revesansparole
-Author-email: revesansparole@gmail.com
+Author-email: revesansparole <revesansparole@gmail.com>
+Maintainer-email: revesansparole <revesansparole@gmail.com>, Jerome Chopard <revesansparole@gmail.com>
 License: cc_by_nc
-Description: ========================
-        allen1989
-        ========================
-        
-        .. {# pkglts, doc
-        
-        .. image:: https://b326.gitlab.io/allen1989/_images/badge_doc.svg
-            :alt: Documentation status
-            :target: https://b326.gitlab.io/allen1989/
-        
-        .. image:: https://b326.gitlab.io/allen1989/_images/badge_pkging_pip.svg
-            :alt: PyPI version
-            :target: https://pypi.org/project/allen1989/0.1.0/
-        
-        .. image:: https://b326.gitlab.io/allen1989/_images/badge_pkging_conda.svg
-            :alt: Conda version
-            :target: https://anaconda.org/revesansparole/allen1989
-        
-        .. image:: https://badge.fury.io/py/allen1989.svg
-            :alt: PyPI version
-            :target: https://badge.fury.io/py/allen1989
-        
-        .. #}
-        .. {# pkglts, glabpkg, after doc
-        
-        main: |main_build|_ |main_coverage|_
-        
-        .. |main_build| image:: https://gitlab.com/b326/allen1989/badges/main/pipeline.svg
-        .. _main_build: https://gitlab.com/b326/allen1989/commits/main
-        
-        .. |main_coverage| image:: https://gitlab.com/b326/allen1989/badges/main/coverage.svg
-        .. _main_coverage: https://gitlab.com/b326/allen1989/commits/main
-        
-        
-        prod: |prod_build|_ |prod_coverage|_
-        
-        .. |prod_build| image:: https://gitlab.com/b326/allen1989/badges/prod/pipeline.svg
-        .. _prod_build: https://gitlab.com/b326/allen1989/commits/prod
-        
-        .. |prod_coverage| image:: https://gitlab.com/b326/allen1989/badges/prod/coverage.svg
-        .. _prod_coverage: https://gitlab.com/b326/allen1989/commits/prod
-        .. #}
-        
-        Formalisms from Allen at al. 1989 paper
-        
-        
-        
-        =======
-        History
-        =======
-        
-        creation (2021-10-25)
-        ------------------------
-        
-        * First release on PyPI.
-        
-Platform: UNKNOWN
+Project-URL: repository, https://gitlab.com/b326/allen1989
+Project-URL: pip, https://pypi.org/project/allen1989/0.2.0/
+Project-URL: conda, https://anaconda.org/revesansparole/allen1989
+Project-URL: doc, https://b326.gitlab.io/allen1989/
+Project-URL: pypi, https://badge.fury.io/py/allen1989
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS.rst
+Provides-Extra: doc
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx-gallery; extra == "doc"
+Requires-Dist: sphinx_rtd_theme; extra == "doc"
+Provides-Extra: dvlpt
+Requires-Dist: twine; extra == "dvlpt"
+Provides-Extra: example
+Requires-Dist: matplotlib; extra == "example"
+Requires-Dist: numpy; extra == "example"
+Provides-Extra: test
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
+
+========================
+allen1989
+========================
+
+.. {# pkglts, doc
+
+.. image:: https://b326.gitlab.io/allen1989/_images/badge_pkging_pip.svg
+    :alt: PyPI version
+    :target: https://pypi.org/project/allen1989/0.2.0/
+
+.. image:: https://b326.gitlab.io/allen1989/_images/badge_pkging_conda.svg
+    :alt: Conda version
+    :target: https://anaconda.org/revesansparole/allen1989
+
+.. image:: https://b326.gitlab.io/allen1989/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/allen1989/
+
+.. image:: https://badge.fury.io/py/allen1989.svg
+    :alt: PyPI version
+    :target: https://badge.fury.io/py/allen1989
+
+.. #}
+.. {# pkglts, glabpkg_dev, after doc
+
+main: |main_build|_ |main_coverage|_
+
+.. |main_build| image:: https://gitlab.com/b326/allen1989/badges/main/pipeline.svg
+.. _main_build: https://gitlab.com/b326/allen1989/commits/main
+
+.. |main_coverage| image:: https://gitlab.com/b326/allen1989/badges/main/coverage.svg
+.. _main_coverage: https://gitlab.com/b326/allen1989/commits/main
+.. #}
+
+Formalisms from Allen at al. 1989 paper
+
```

### Comparing `allen1989-0.1.0/README.rst` & `allen1989-0.2.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,36 @@
 ========================
 allen1989
 ========================
 
 .. {# pkglts, doc
 
-.. image:: https://b326.gitlab.io/allen1989/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/allen1989/
-
 .. image:: https://b326.gitlab.io/allen1989/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/allen1989/0.1.0/
+    :target: https://pypi.org/project/allen1989/0.2.0/
 
 .. image:: https://b326.gitlab.io/allen1989/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/allen1989
 
+.. image:: https://b326.gitlab.io/allen1989/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/allen1989/
+
 .. image:: https://badge.fury.io/py/allen1989.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/allen1989
 
 .. #}
-.. {# pkglts, glabpkg, after doc
+.. {# pkglts, glabpkg_dev, after doc
 
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/allen1989/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/allen1989/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/allen1989/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/allen1989/commits/main
-
-
-prod: |prod_build|_ |prod_coverage|_
-
-.. |prod_build| image:: https://gitlab.com/b326/allen1989/badges/prod/pipeline.svg
-.. _prod_build: https://gitlab.com/b326/allen1989/commits/prod
-
-.. |prod_coverage| image:: https://gitlab.com/b326/allen1989/badges/prod/coverage.svg
-.. _prod_coverage: https://gitlab.com/b326/allen1989/commits/prod
 .. #}
 
 Formalisms from Allen at al. 1989 paper
```

### Comparing `allen1989-0.1.0/doc/Makefile` & `allen1989-0.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `allen1989-0.1.0/doc/_gallery/index.rst` & `allen1989-0.2.0/doc/_gallery/index.rst`

 * *Files identical despite different names*

### Comparing `allen1989-0.1.0/doc/_gallery/plot_heat_conductance.rst` & `allen1989-0.2.0/doc/_gallery/plot_heat_conductance.rst`

 * *Files identical despite different names*

### Comparing `allen1989-0.1.0/doc/biblio/biblio.rst` & `allen1989-0.2.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `allen1989-0.1.0/doc/conf.py` & `allen1989-0.2.0/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,17 +85,17 @@
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
 # The short X.Y version.
-version = "0.1.0"
+version = "0.2.0"
 # The full version, including alpha/beta/rc tags.
-release = "0.1.0"
+release = "0.2.0"
 
 
 exclude_patterns = ['build', 'dist']
 
 pygments_style = 'sphinx'
 
 # -- Options for HTML output -------------------------------------------
```

### Comparing `allen1989-0.1.0/doc/index.rst` & `allen1989-0.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `allen1989-0.1.0/doc/make.bat` & `allen1989-0.2.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `allen1989-0.1.0/doc/readme.rst` & `allen1989-0.2.0/doc/readme.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 Overview
 ========
 
-.. {# pkglts, glabpkg
-
-.. image:: https://b326.gitlab.io/allen1989/_images/badge_doc.svg
-    :alt: Documentation status
-    :target: https://b326.gitlab.io/allen1989/
+.. {# pkglts, glabpkg_dev
 
 .. image:: https://b326.gitlab.io/allen1989/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/allen1989/0.1.0/
+    :target: https://pypi.org/project/allen1989/0.2.0/
+
 
 .. image:: https://b326.gitlab.io/allen1989/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/allen1989
 
+
+.. image:: https://b326.gitlab.io/allen1989/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/allen1989/
+
+
 .. image:: https://badge.fury.io/py/allen1989.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/allen1989
 
 
+
+
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/allen1989/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/allen1989/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/allen1989/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/allen1989/commits/main
-
-
-prod: |prod_build|_ |prod_coverage|_
-
-.. |prod_build| image:: https://gitlab.com/b326/allen1989/badges/prod/pipeline.svg
-.. _prod_build: https://gitlab.com/b326/allen1989/commits/prod
-
-.. |prod_coverage| image:: https://gitlab.com/b326/allen1989/badges/prod/coverage.svg
-.. _prod_coverage: https://gitlab.com/b326/allen1989/commits/prod
-
 .. #}
 
 Formalisms from Allen at al. 1989 paper
```

### Comparing `allen1989-0.1.0/src/allen1989/raw.py` & `allen1989-0.2.0/src/allen1989/raw.py`

 * *Files identical despite different names*

### Comparing `allen1989-0.1.0/src/allen1989/transfer.py` & `allen1989-0.2.0/src/allen1989/transfer.py`

 * *Files identical despite different names*

### Comparing `allen1989-0.1.0/src/allen1989.egg-info/PKG-INFO` & `allen1989-0.2.0/src/allen1989.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,76 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: allen1989
-Version: 0.1.0
+Version: 0.2.0
 Summary: Formalisms from Allen at al. 1989 paper
-Home-page: https://gitlab.com/b326/allen1989
-Author: revesansparole
-Author-email: revesansparole@gmail.com
+Author-email: revesansparole <revesansparole@gmail.com>
+Maintainer-email: revesansparole <revesansparole@gmail.com>, Jerome Chopard <revesansparole@gmail.com>
 License: cc_by_nc
-Description: ========================
-        allen1989
-        ========================
-        
-        .. {# pkglts, doc
-        
-        .. image:: https://b326.gitlab.io/allen1989/_images/badge_doc.svg
-            :alt: Documentation status
-            :target: https://b326.gitlab.io/allen1989/
-        
-        .. image:: https://b326.gitlab.io/allen1989/_images/badge_pkging_pip.svg
-            :alt: PyPI version
-            :target: https://pypi.org/project/allen1989/0.1.0/
-        
-        .. image:: https://b326.gitlab.io/allen1989/_images/badge_pkging_conda.svg
-            :alt: Conda version
-            :target: https://anaconda.org/revesansparole/allen1989
-        
-        .. image:: https://badge.fury.io/py/allen1989.svg
-            :alt: PyPI version
-            :target: https://badge.fury.io/py/allen1989
-        
-        .. #}
-        .. {# pkglts, glabpkg, after doc
-        
-        main: |main_build|_ |main_coverage|_
-        
-        .. |main_build| image:: https://gitlab.com/b326/allen1989/badges/main/pipeline.svg
-        .. _main_build: https://gitlab.com/b326/allen1989/commits/main
-        
-        .. |main_coverage| image:: https://gitlab.com/b326/allen1989/badges/main/coverage.svg
-        .. _main_coverage: https://gitlab.com/b326/allen1989/commits/main
-        
-        
-        prod: |prod_build|_ |prod_coverage|_
-        
-        .. |prod_build| image:: https://gitlab.com/b326/allen1989/badges/prod/pipeline.svg
-        .. _prod_build: https://gitlab.com/b326/allen1989/commits/prod
-        
-        .. |prod_coverage| image:: https://gitlab.com/b326/allen1989/badges/prod/coverage.svg
-        .. _prod_coverage: https://gitlab.com/b326/allen1989/commits/prod
-        .. #}
-        
-        Formalisms from Allen at al. 1989 paper
-        
-        
-        
-        =======
-        History
-        =======
-        
-        creation (2021-10-25)
-        ------------------------
-        
-        * First release on PyPI.
-        
-Platform: UNKNOWN
+Project-URL: repository, https://gitlab.com/b326/allen1989
+Project-URL: pip, https://pypi.org/project/allen1989/0.2.0/
+Project-URL: conda, https://anaconda.org/revesansparole/allen1989
+Project-URL: doc, https://b326.gitlab.io/allen1989/
+Project-URL: pypi, https://badge.fury.io/py/allen1989
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS.rst
+Provides-Extra: doc
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx-gallery; extra == "doc"
+Requires-Dist: sphinx_rtd_theme; extra == "doc"
+Provides-Extra: dvlpt
+Requires-Dist: twine; extra == "dvlpt"
+Provides-Extra: example
+Requires-Dist: matplotlib; extra == "example"
+Requires-Dist: numpy; extra == "example"
+Provides-Extra: test
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
+
+========================
+allen1989
+========================
+
+.. {# pkglts, doc
+
+.. image:: https://b326.gitlab.io/allen1989/_images/badge_pkging_pip.svg
+    :alt: PyPI version
+    :target: https://pypi.org/project/allen1989/0.2.0/
+
+.. image:: https://b326.gitlab.io/allen1989/_images/badge_pkging_conda.svg
+    :alt: Conda version
+    :target: https://anaconda.org/revesansparole/allen1989
+
+.. image:: https://b326.gitlab.io/allen1989/_images/badge_doc.svg
+    :alt: Documentation status
+    :target: https://b326.gitlab.io/allen1989/
+
+.. image:: https://badge.fury.io/py/allen1989.svg
+    :alt: PyPI version
+    :target: https://badge.fury.io/py/allen1989
+
+.. #}
+.. {# pkglts, glabpkg_dev, after doc
+
+main: |main_build|_ |main_coverage|_
+
+.. |main_build| image:: https://gitlab.com/b326/allen1989/badges/main/pipeline.svg
+.. _main_build: https://gitlab.com/b326/allen1989/commits/main
+
+.. |main_coverage| image:: https://gitlab.com/b326/allen1989/badges/main/coverage.svg
+.. _main_coverage: https://gitlab.com/b326/allen1989/commits/main
+.. #}
+
+Formalisms from Allen at al. 1989 paper
+
```

### Comparing `allen1989-0.1.0/test/conftest.py` & `allen1989-0.2.0/test/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=allen1989")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=allen1989")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

