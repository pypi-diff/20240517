# Comparing `tmp/alsina2011-1.0.0.tar.gz` & `tmp/alsina2011-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alsina2011-1.0.0.tar", last modified: Thu Mar  9 14:33:06 2023, max compression
+gzip compressed data, was "alsina2011-1.1.0.tar", last modified: Fri May 17 09:40:13 2024, max compression
```

## Comparing `alsina2011-1.0.0.tar` & `alsina2011-1.1.0.tar`

### file list

```diff
@@ -1,69 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 14:33:06.188534 alsina2011-1.0.0/
--rw-rw-rw-   0        0        0      316 2023-03-09 14:22:10.000000 alsina2011-1.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3322 2023-03-09 14:22:10.000000 alsina2011-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2023-03-09 14:22:10.000000 alsina2011-1.0.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2023-03-09 14:22:10.000000 alsina2011-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      438 2023-03-09 14:22:10.000000 alsina2011-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2285 2023-03-09 14:33:06.188534 alsina2011-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1492 2023-03-09 14:22:10.000000 alsina2011-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-09 14:33:05.976119 alsina2011-1.0.0/doc/
--rw-rw-rw-   0        0        0     6967 2023-03-09 14:22:10.000000 alsina2011-1.0.0/doc/Makefile
-drwxrwxrwx   0        0        0        0 2023-03-09 14:33:06.020132 alsina2011-1.0.0/doc/_gallery/
--rw-rw-rw-   0        0        0     3934 2023-03-09 14:18:21.000000 alsina2011-1.0.0/doc/_gallery/index.rst
--rw-rw-rw-   0        0        0     2292 2023-03-09 14:18:20.000000 alsina2011-1.0.0/doc/_gallery/plot_an.rst
--rw-rw-rw-   0        0        0     2383 2023-03-09 14:18:19.000000 alsina2011-1.0.0/doc/_gallery/plot_diff_t_air_leaf.rst
--rw-rw-rw-   0        0        0     2271 2023-03-09 14:18:21.000000 alsina2011-1.0.0/doc/_gallery/plot_ec.rst
--rw-rw-rw-   0        0        0     2349 2023-03-09 14:18:20.000000 alsina2011-1.0.0/doc/_gallery/plot_gs.rst
--rw-rw-rw-   0        0        0     2221 2023-03-09 14:18:18.000000 alsina2011-1.0.0/doc/_gallery/plot_t_air.rst
--rw-rw-rw-   0        0        0     2335 2023-03-09 14:18:19.000000 alsina2011-1.0.0/doc/_gallery/plot_t_leaf.rst
--rw-rw-rw-   0        0        0     2168 2023-03-09 14:18:21.000000 alsina2011-1.0.0/doc/_gallery/plot_vpd.rst
--rw-rw-rw-   0        0        0     2356 2023-03-09 14:18:21.000000 alsina2011-1.0.0/doc/_gallery/plot_vpd_leaf.rst
--rw-rw-rw-   0        0        0     2353 2023-03-09 14:18:20.000000 alsina2011-1.0.0/doc/_gallery/plot_wp_leaf.rst
--rw-rw-rw-   0        0        0     2127 2023-03-09 14:18:21.000000 alsina2011-1.0.0/doc/_gallery/sg_execution_times.rst
--rw-rw-rw-   0        0        0       29 2023-03-09 14:22:10.000000 alsina2011-1.0.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2023-03-09 14:33:06.032122 alsina2011-1.0.0/doc/badges/
--rw-rw-rw-   0        0        0      282 2023-03-09 14:22:10.000000 alsina2011-1.0.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2023-03-09 14:33:06.036119 alsina2011-1.0.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2023-03-09 14:22:10.000000 alsina2011-1.0.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     5102 2023-03-09 14:22:10.000000 alsina2011-1.0.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2023-03-09 14:22:10.000000 alsina2011-1.0.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-03-09 14:22:10.000000 alsina2011-1.0.0/doc/history.rst
--rw-rw-rw-   0        0        0      595 2023-03-09 14:22:10.000000 alsina2011-1.0.0/doc/index.rst
--rw-rw-rw-   0        0        0      220 2023-03-09 14:22:10.000000 alsina2011-1.0.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2023-03-09 14:22:10.000000 alsina2011-1.0.0/doc/make.bat
--rw-rw-rw-   0        0        0      133 2023-03-09 14:22:10.000000 alsina2011-1.0.0/doc/management.rst
--rw-rw-rw-   0        0        0     1411 2023-03-09 14:22:10.000000 alsina2011-1.0.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2023-03-09 14:22:10.000000 alsina2011-1.0.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2023-03-09 14:33:06.040128 alsina2011-1.0.0/doc/user/
--rw-rw-rw-   0        0        0       86 2023-03-09 14:22:10.000000 alsina2011-1.0.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2023-03-09 14:22:10.000000 alsina2011-1.0.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0      345 2023-03-09 14:22:10.000000 alsina2011-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       29 2023-03-09 14:22:10.000000 alsina2011-1.0.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0      187 2023-03-09 14:33:06.204535 alsina2011-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1867 2023-03-09 14:22:10.000000 alsina2011-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-09 14:33:05.904116 alsina2011-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-09 14:33:06.052121 alsina2011-1.0.0/src/alsina2011/
--rw-rw-rw-   0        0        0      261 2023-03-09 14:22:10.000000 alsina2011-1.0.0/src/alsina2011/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-09 14:33:06.180542 alsina2011-1.0.0/src/alsina2011/clean/
--rw-rw-rw-   0        0        0     2218 2023-03-09 14:01:18.000000 alsina2011-1.0.0/src/alsina2011/clean/an.csv
--rw-rw-rw-   0        0        0     2271 2023-03-09 14:04:04.000000 alsina2011-1.0.0/src/alsina2011/clean/diff_t_air_leaf.csv
--rw-rw-rw-   0        0        0     2090 2023-03-09 14:04:33.000000 alsina2011-1.0.0/src/alsina2011/clean/ec.csv
--rw-rw-rw-   0        0        0     2264 2023-03-09 14:04:56.000000 alsina2011-1.0.0/src/alsina2011/clean/gs.csv
--rw-rw-rw-   0        0        0     1396 2023-03-09 14:00:10.000000 alsina2011-1.0.0/src/alsina2011/clean/info.json
--rw-rw-rw-   0        0        0      134 2023-03-09 14:22:10.000000 alsina2011-1.0.0/src/alsina2011/clean/readme.rst
--rw-rw-rw-   0        0        0     2773 2023-03-09 14:05:16.000000 alsina2011-1.0.0/src/alsina2011/clean/t_air.csv
--rw-rw-rw-   0        0        0     2205 2023-03-09 14:05:37.000000 alsina2011-1.0.0/src/alsina2011/clean/t_leaf.csv
--rw-rw-rw-   0        0        0     2795 2023-03-09 14:05:57.000000 alsina2011-1.0.0/src/alsina2011/clean/vpd.csv
--rw-rw-rw-   0        0        0     2244 2023-03-09 14:06:16.000000 alsina2011-1.0.0/src/alsina2011/clean/vpd_leaf.csv
--rw-rw-rw-   0        0        0     1994 2023-03-09 14:06:39.000000 alsina2011-1.0.0/src/alsina2011/clean/wp_leaf.csv
--rw-rw-rw-   0        0        0      152 2023-03-09 14:22:10.000000 alsina2011-1.0.0/src/alsina2011/info.py
--rw-rw-rw-   0        0        0      367 2023-03-09 14:22:10.000000 alsina2011-1.0.0/src/alsina2011/version.py
-drwxrwxrwx   0        0        0        0 2023-03-09 14:33:06.136549 alsina2011-1.0.0/src/alsina2011.egg-info/
--rw-rw-rw-   0        0        0     2285 2023-03-09 14:33:05.000000 alsina2011-1.0.0/src/alsina2011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1360 2023-03-09 14:33:05.000000 alsina2011-1.0.0/src/alsina2011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 14:33:05.000000 alsina2011-1.0.0/src/alsina2011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 13:59:28.000000 alsina2011-1.0.0/src/alsina2011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-03-09 14:33:05.000000 alsina2011-1.0.0/src/alsina2011.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-09 14:33:06.188534 alsina2011-1.0.0/test/
--rw-rw-rw-   0        0        0      974 2023-03-09 14:22:10.000000 alsina2011-1.0.0/test/conftest.py
--rw-rw-rw-   0        0        0       86 2023-03-09 14:22:10.000000 alsina2011-1.0.0/test/test_packaging.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:40:13.032187 alsina2011-1.1.0/
+-rw-rw-rw-   0        0        0      316 2024-05-17 09:35:25.000000 alsina2011-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3323 2024-05-17 09:35:25.000000 alsina2011-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-17 09:35:25.000000 alsina2011-1.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-17 09:35:25.000000 alsina2011-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3281 2024-05-17 09:40:13.028668 alsina2011-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1492 2024-05-17 09:35:25.000000 alsina2011-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:40:12.982036 alsina2011-1.1.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-17 09:35:25.000000 alsina2011-1.1.0/doc/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-17 09:40:12.991968 alsina2011-1.1.0/doc/_gallery/
+-rw-rw-rw-   0        0        0     3995 2024-05-17 08:48:35.000000 alsina2011-1.1.0/doc/_gallery/index.rst
+-rw-rw-rw-   0        0        0     2292 2023-03-09 14:18:20.000000 alsina2011-1.1.0/doc/_gallery/plot_an.rst
+-rw-rw-rw-   0        0        0     2378 2024-05-17 08:48:35.000000 alsina2011-1.1.0/doc/_gallery/plot_diff_t_air_leaf.rst
+-rw-rw-rw-   0        0        0     2271 2023-03-09 14:18:21.000000 alsina2011-1.1.0/doc/_gallery/plot_ec.rst
+-rw-rw-rw-   0        0        0     2349 2023-03-09 14:18:20.000000 alsina2011-1.1.0/doc/_gallery/plot_gs.rst
+-rw-rw-rw-   0        0        0     2216 2024-05-17 08:48:35.000000 alsina2011-1.1.0/doc/_gallery/plot_t_air.rst
+-rw-rw-rw-   0        0        0     2330 2024-05-17 08:48:35.000000 alsina2011-1.1.0/doc/_gallery/plot_t_leaf.rst
+-rw-rw-rw-   0        0        0     2168 2023-03-09 14:18:21.000000 alsina2011-1.1.0/doc/_gallery/plot_vpd.rst
+-rw-rw-rw-   0        0        0     2356 2023-03-09 14:18:21.000000 alsina2011-1.1.0/doc/_gallery/plot_vpd_leaf.rst
+-rw-rw-rw-   0        0        0     2353 2023-03-09 14:18:20.000000 alsina2011-1.1.0/doc/_gallery/plot_wp_leaf.rst
+-rw-rw-rw-   0        0        0     1921 2024-05-17 08:48:35.000000 alsina2011-1.1.0/doc/_gallery/sg_execution_times.rst
+-rw-rw-rw-   0        0        0       29 2024-05-17 09:35:25.000000 alsina2011-1.1.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:40:12.991968 alsina2011-1.1.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-17 09:35:25.000000 alsina2011-1.1.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:40:12.991968 alsina2011-1.1.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-17 09:35:25.000000 alsina2011-1.1.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     5102 2024-05-17 09:35:25.000000 alsina2011-1.1.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-17 09:35:25.000000 alsina2011-1.1.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-17 09:35:25.000000 alsina2011-1.1.0/doc/history.rst
+-rw-rw-rw-   0        0        0      595 2024-05-17 09:35:25.000000 alsina2011-1.1.0/doc/index.rst
+-rw-rw-rw-   0        0        0      220 2024-05-17 09:35:25.000000 alsina2011-1.1.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-17 09:35:25.000000 alsina2011-1.1.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-17 09:35:25.000000 alsina2011-1.1.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1419 2024-05-17 09:35:25.000000 alsina2011-1.1.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-17 09:35:25.000000 alsina2011-1.1.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:40:12.991968 alsina2011-1.1.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-17 09:35:25.000000 alsina2011-1.1.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-17 09:35:25.000000 alsina2011-1.1.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2308 2024-05-17 09:35:25.000000 alsina2011-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      345 2024-05-17 09:35:25.000000 alsina2011-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       29 2024-05-17 09:35:25.000000 alsina2011-1.1.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 09:40:13.032187 alsina2011-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 09:40:12.941969 alsina2011-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:40:13.002056 alsina2011-1.1.0/src/alsina2011/
+-rw-rw-rw-   0        0        0      253 2024-05-17 09:35:25.000000 alsina2011-1.1.0/src/alsina2011/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:40:13.022391 alsina2011-1.1.0/src/alsina2011/clean/
+-rw-rw-rw-   0        0        0     1898 2024-05-17 08:43:39.000000 alsina2011-1.1.0/src/alsina2011/clean/an.csv
+-rw-rw-rw-   0        0        0     1951 2024-05-17 08:45:25.000000 alsina2011-1.1.0/src/alsina2011/clean/diff_t_air_leaf.csv
+-rw-rw-rw-   0        0        0     1790 2024-05-17 08:45:38.000000 alsina2011-1.1.0/src/alsina2011/clean/ec.csv
+-rw-rw-rw-   0        0        0     1944 2024-05-17 08:45:50.000000 alsina2011-1.1.0/src/alsina2011/clean/gs.csv
+-rw-rw-rw-   0        0        0     1396 2024-05-17 08:46:00.000000 alsina2011-1.1.0/src/alsina2011/clean/info.json
+-rw-rw-rw-   0        0        0      134 2024-05-17 09:35:25.000000 alsina2011-1.1.0/src/alsina2011/clean/readme.rst
+-rw-rw-rw-   0        0        0     2773 2024-05-17 08:46:07.000000 alsina2011-1.1.0/src/alsina2011/clean/t_air.csv
+-rw-rw-rw-   0        0        0     1885 2024-05-17 08:47:09.000000 alsina2011-1.1.0/src/alsina2011/clean/t_leaf.csv
+-rw-rw-rw-   0        0        0     2795 2024-05-17 08:47:46.000000 alsina2011-1.1.0/src/alsina2011/clean/vpd.csv
+-rw-rw-rw-   0        0        0     1924 2024-05-17 08:47:52.000000 alsina2011-1.1.0/src/alsina2011/clean/vpd_leaf.csv
+-rw-rw-rw-   0        0        0     1714 2024-05-17 08:48:09.000000 alsina2011-1.1.0/src/alsina2011/clean/wp_leaf.csv
+-rw-rw-rw-   0        0        0      379 2024-05-17 09:35:25.000000 alsina2011-1.1.0/src/alsina2011/info.py
+-rw-rw-rw-   0        0        0      367 2024-05-17 09:35:25.000000 alsina2011-1.1.0/src/alsina2011/version.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:40:13.028668 alsina2011-1.1.0/src/alsina2011.egg-info/
+-rw-rw-rw-   0        0        0     3281 2024-05-17 09:40:12.000000 alsina2011-1.1.0/src/alsina2011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1344 2024-05-17 09:40:12.000000 alsina2011-1.1.0/src/alsina2011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 09:40:12.000000 alsina2011-1.1.0/src/alsina2011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2024-05-17 09:40:12.000000 alsina2011-1.1.0/src/alsina2011.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-17 09:40:12.000000 alsina2011-1.1.0/src/alsina2011.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 09:40:13.022391 alsina2011-1.1.0/test/
+-rw-rw-rw-   0        0        0      986 2024-05-17 09:35:25.000000 alsina2011-1.1.0/test/conftest.py
+-rw-rw-rw-   0        0        0      381 2024-05-17 09:35:25.000000 alsina2011-1.1.0/test/test_packaging.py
```

### Comparing `alsina2011-1.0.0/CONTRIBUTING.rst` & `alsina2011-1.1.0/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
   1. The pull request should include tests.
   2. If the pull request adds functionality, the docs should be updated. Put
      your new functionality into a function with a docstring, and add the
      feature to the list in README.rst.
-  3. The pull request should work for Python 39.
+  3. The pull request should work for Python 3.9.
      
 
 Tips
 ----
 
 
 To run a subset of tests::
```

### Comparing `alsina2011-1.0.0/LICENSE` & `alsina2011-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alsina2011-1.0.0/README.rst` & `alsina2011-1.1.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 alsina2011
 ========================
 
 .. {# pkglts, doc
 
 .. image:: https://b326.gitlab.io/alsina2011/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/alsina2011/1.0.0/
+    :target: https://pypi.org/project/alsina2011/1.1.0/
 
 .. image:: https://b326.gitlab.io/alsina2011/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/alsina2011
 
 .. image:: https://b326.gitlab.io/alsina2011/_images/badge_doc.svg
     :alt: Documentation status
```

### Comparing `alsina2011-1.0.0/doc/Makefile` & `alsina2011-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `alsina2011-1.0.0/doc/_gallery/index.rst` & `alsina2011-1.1.0/doc/_gallery/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 
 
 .. raw:: html
 
     <div class="sphx-glr-thumbnails">
 
+.. thumbnail-parent-div-open
 
 .. raw:: html
 
     <div class="sphx-glr-thumbcontainer" tooltip="plot extracted t_air to compare to article figure 4">
 
 .. only:: html
 
@@ -165,14 +166,16 @@
 
 .. raw:: html
 
       <div class="sphx-glr-thumbnail-title">VPD leaf</div>
     </div>
 
 
+.. thumbnail-parent-div-close
+
 .. raw:: html
 
     </div>
 
 
 .. toctree::
    :hidden:
@@ -184,12 +187,13 @@
    /_gallery/plot_an
    /_gallery/plot_gs
    /_gallery/plot_ec
    /_gallery/plot_vpd
    /_gallery/plot_vpd_leaf
 
 
+
 .. only:: html
 
  .. rst-class:: sphx-glr-signature
 
     `Gallery generated by Sphinx-Gallery <https://sphinx-gallery.github.io>`_
```

### Comparing `alsina2011-1.0.0/doc/_gallery/plot_an.rst` & `alsina2011-1.1.0/doc/_gallery/plot_an.rst`

 * *Files identical despite different names*

### Comparing `alsina2011-1.0.0/doc/_gallery/plot_diff_t_air_leaf.rst` & `alsina2011-1.1.0/doc/_gallery/plot_diff_t_air_leaf.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 .. only:: html
 
     .. note::
         :class: sphx-glr-download-link-note
 
         :ref:`Go to the end <sphx_glr_download__gallery_plot_diff_t_air_leaf.py>`
-        to download the full example code
+        to download the full example code.
 
 .. rst-class:: sphx-glr-example-title
 
 .. _sphx_glr__gallery_plot_diff_t_air_leaf.py:
 
 
 Debug leaf temperature
@@ -32,15 +32,15 @@
    :srcset: /_gallery/images/sphx_glr_plot_diff_t_air_leaf_001.png
    :class: sphx-glr-single-img
 
 
 
 
 
-.. code-block:: default
+.. code-block:: Python
 
     import matplotlib.pyplot as plt
     import pandas as pd
 
     from alsina2011 import pth_clean
 
     # read data
@@ -65,33 +65,30 @@
 
     fig.tight_layout()
     plt.show()
 
 
 .. rst-class:: sphx-glr-timing
 
-   **Total running time of the script:** ( 0 minutes  0.330 seconds)
+   **Total running time of the script:** (0 minutes 0.121 seconds)
 
 
 .. _sphx_glr_download__gallery_plot_diff_t_air_leaf.py:
 
 .. only:: html
 
   .. container:: sphx-glr-footer sphx-glr-footer-example
 
+    .. container:: sphx-glr-download sphx-glr-download-jupyter
 
-
+      :download:`Download Jupyter notebook: plot_diff_t_air_leaf.ipynb <plot_diff_t_air_leaf.ipynb>`
 
     .. container:: sphx-glr-download sphx-glr-download-python
 
       :download:`Download Python source code: plot_diff_t_air_leaf.py <plot_diff_t_air_leaf.py>`
 
-    .. container:: sphx-glr-download sphx-glr-download-jupyter
-
-      :download:`Download Jupyter notebook: plot_diff_t_air_leaf.ipynb <plot_diff_t_air_leaf.ipynb>`
-
 
 .. only:: html
 
  .. rst-class:: sphx-glr-signature
 
     `Gallery generated by Sphinx-Gallery <https://sphinx-gallery.github.io>`_
```

### Comparing `alsina2011-1.0.0/doc/_gallery/plot_ec.rst` & `alsina2011-1.1.0/doc/_gallery/plot_ec.rst`

 * *Files identical despite different names*

### Comparing `alsina2011-1.0.0/doc/_gallery/plot_gs.rst` & `alsina2011-1.1.0/doc/_gallery/plot_gs.rst`

 * *Files identical despite different names*

### Comparing `alsina2011-1.0.0/doc/_gallery/plot_t_air.rst` & `alsina2011-1.1.0/doc/_gallery/plot_t_air.rst`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 .. only:: html
 
     .. note::
         :class: sphx-glr-download-link-note
 
         :ref:`Go to the end <sphx_glr_download__gallery_plot_t_air.py>`
-        to download the full example code
+        to download the full example code.
 
 .. rst-class:: sphx-glr-example-title
 
 .. _sphx_glr__gallery_plot_t_air.py:
 
 
 Air temperature
@@ -33,15 +33,15 @@
    :srcset: /_gallery/images/sphx_glr_plot_t_air_001.png
    :class: sphx-glr-single-img
 
 
 
 
 
-.. code-block:: default
+.. code-block:: Python
 
     import matplotlib.pyplot as plt
     import pandas as pd
 
     from alsina2011 import pth_clean
 
     # read data
@@ -64,33 +64,30 @@
 
     fig.tight_layout()
     plt.show()
 
 
 .. rst-class:: sphx-glr-timing
 
-   **Total running time of the script:** ( 0 minutes  0.790 seconds)
+   **Total running time of the script:** (0 minutes 0.438 seconds)
 
 
 .. _sphx_glr_download__gallery_plot_t_air.py:
 
 .. only:: html
 
   .. container:: sphx-glr-footer sphx-glr-footer-example
 
+    .. container:: sphx-glr-download sphx-glr-download-jupyter
 
-
+      :download:`Download Jupyter notebook: plot_t_air.ipynb <plot_t_air.ipynb>`
 
     .. container:: sphx-glr-download sphx-glr-download-python
 
       :download:`Download Python source code: plot_t_air.py <plot_t_air.py>`
 
-    .. container:: sphx-glr-download sphx-glr-download-jupyter
-
-      :download:`Download Jupyter notebook: plot_t_air.ipynb <plot_t_air.ipynb>`
-
 
 .. only:: html
 
  .. rst-class:: sphx-glr-signature
 
     `Gallery generated by Sphinx-Gallery <https://sphinx-gallery.github.io>`_
```

### Comparing `alsina2011-1.0.0/doc/_gallery/plot_t_leaf.rst` & `alsina2011-1.1.0/doc/_gallery/plot_t_leaf.rst`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 .. only:: html
 
     .. note::
         :class: sphx-glr-download-link-note
 
         :ref:`Go to the end <sphx_glr_download__gallery_plot_t_leaf.py>`
-        to download the full example code
+        to download the full example code.
 
 .. rst-class:: sphx-glr-example-title
 
 .. _sphx_glr__gallery_plot_t_leaf.py:
 
 
 Leaf temperature
@@ -33,15 +33,15 @@
    :srcset: /_gallery/images/sphx_glr_plot_t_leaf_001.png
    :class: sphx-glr-single-img
 
 
 
 
 
-.. code-block:: default
+.. code-block:: Python
 
     import matplotlib.pyplot as plt
     import pandas as pd
 
     from alsina2011 import pth_clean
 
     # read data
@@ -68,33 +68,30 @@
 
     fig.tight_layout()
     plt.show()
 
 
 .. rst-class:: sphx-glr-timing
 
-   **Total running time of the script:** ( 0 minutes  0.212 seconds)
+   **Total running time of the script:** (0 minutes 0.107 seconds)
 
 
 .. _sphx_glr_download__gallery_plot_t_leaf.py:
 
 .. only:: html
 
   .. container:: sphx-glr-footer sphx-glr-footer-example
 
+    .. container:: sphx-glr-download sphx-glr-download-jupyter
 
-
+      :download:`Download Jupyter notebook: plot_t_leaf.ipynb <plot_t_leaf.ipynb>`
 
     .. container:: sphx-glr-download sphx-glr-download-python
 
       :download:`Download Python source code: plot_t_leaf.py <plot_t_leaf.py>`
 
-    .. container:: sphx-glr-download sphx-glr-download-jupyter
-
-      :download:`Download Jupyter notebook: plot_t_leaf.ipynb <plot_t_leaf.ipynb>`
-
 
 .. only:: html
 
  .. rst-class:: sphx-glr-signature
 
     `Gallery generated by Sphinx-Gallery <https://sphinx-gallery.github.io>`_
```

### Comparing `alsina2011-1.0.0/doc/_gallery/plot_vpd.rst` & `alsina2011-1.1.0/doc/_gallery/plot_vpd.rst`

 * *Files identical despite different names*

### Comparing `alsina2011-1.0.0/doc/_gallery/plot_vpd_leaf.rst` & `alsina2011-1.1.0/doc/_gallery/plot_vpd_leaf.rst`

 * *Files identical despite different names*

### Comparing `alsina2011-1.0.0/doc/_gallery/plot_wp_leaf.rst` & `alsina2011-1.1.0/doc/_gallery/plot_wp_leaf.rst`

 * *Files identical despite different names*

### Comparing `alsina2011-1.0.0/doc/biblio/biblio.rst` & `alsina2011-1.1.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `alsina2011-1.0.0/doc/conf.py` & `alsina2011-1.1.0/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,17 +85,17 @@
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
 # The short X.Y version.
-version = "1.0.0"
+version = "1.1.0"
 # The full version, including alpha/beta/rc tags.
-release = "1.0.0"
+release = "1.1.0"
 
 
 exclude_patterns = ['build', 'dist']
 
 pygments_style = 'sphinx'
 
 # -- Options for HTML output -------------------------------------------
```

### Comparing `alsina2011-1.0.0/doc/index.rst` & `alsina2011-1.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `alsina2011-1.0.0/doc/make.bat` & `alsina2011-1.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `alsina2011-1.0.0/doc/readme.rst` & `alsina2011-1.1.0/doc/readme.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Overview
 ========
 
 .. {# pkglts, glabpkg_dev
 
 .. image:: https://b326.gitlab.io/alsina2011/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/alsina2011/1.0.0/
+    :target: https://pypi.org/project/alsina2011/1.1.0/
+
 
 .. image:: https://b326.gitlab.io/alsina2011/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/alsina2011
 
+
 .. image:: https://b326.gitlab.io/alsina2011/_images/badge_doc.svg
     :alt: Documentation status
     :target: https://b326.gitlab.io/alsina2011/
 
+
 .. image:: https://badge.fury.io/py/alsina2011.svg
     :alt: PyPI version
     :target: https://badge.fury.io/py/alsina2011
 
 
 
+
 main: |main_build|_ |main_coverage|_
 
 .. |main_build| image:: https://gitlab.com/b326/alsina2011/badges/main/pipeline.svg
 .. _main_build: https://gitlab.com/b326/alsina2011/commits/main
 
 .. |main_coverage| image:: https://gitlab.com/b326/alsina2011/badges/main/coverage.svg
 .. _main_coverage: https://gitlab.com/b326/alsina2011/commits/main
```

### Comparing `alsina2011-1.0.0/src/alsina2011/clean/an.csv` & `alsina2011-1.1.0/src/alsina2011/clean/t_leaf.csv`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-# This file has been generated by fmt_an.py
+# This file has been generated by fmt_t_leaf.py
 #
-# an: [mumol CO2 m-2 s-1] photosynthetic rate
+# t_leaf: [°C] leaf temperature
 #
-when;rootstock;date;an
-fall;berlandieri;2006-09-19 05:01:17.774799432;-0.18528317365825941
-fall;berlandieri;2006-09-19 08:01:05.152053934;2.061867423906101
-fall;berlandieri;2006-09-19 09:48:06.232937885;12.134250825876975
-fall;berlandieri;2006-09-19 10:51:04.532656460;6.980981783548842
-fall;berlandieri;2006-09-19 14:01:09.544094491;6.770909016506014
-fall;berlandieri;2006-09-19 15:15:56.874491874;7.053122433460118
-fall;berlandieri;2006-09-19 17:01:13.909518646;5.76602793624215
-fall;riparia;2006-09-19 05:01:17.774799432;-0.7804813850510897
-fall;riparia;2006-09-19 08:03:18.008663694;1.5372664796659983
-fall;riparia;2006-09-19 09:45:41.391596733;8.435471574759067
-fall;riparia;2006-09-19 10:53:05.413444086;7.991210317598991
-fall;riparia;2006-09-19 14:01:59.353963850;6.02112117835186
-fall;riparia;2006-09-19 15:14:37.526874632;5.452957153335449
-fall;riparia;2006-09-19 17:03:23.077696354;5.02491831885607
-spring;berlandieri;2006-06-21 04:33:53.705213316;-1.2024569301218833
-spring;berlandieri;2006-06-21 08:28:29.221640051;11.894548049646684
-spring;berlandieri;2006-06-21 09:43:32.223419025;15.637849483683713
-spring;berlandieri;2006-06-21 11:53:29.367427035;7.546077416652423
-spring;berlandieri;2006-06-21 13:15:29.425741829;8.61689107341734
-spring;berlandieri;2006-06-21 14:34:50.765658071;9.76558676395534
-spring;berlandieri;2006-06-21 16:14:02.446344391;9.759377220656775
-spring;berlandieri;2006-06-21 17:51:54.779413468;9.732620843176898
-spring;berlandieri;2006-06-21 20:30:37.471718911;-1.9323417451882854
-spring;riparia;2006-06-21 04:33:53.705213316;-1.9483466243944427
-spring;riparia;2006-06-21 08:27:39.409988841;13.668005815789611
-spring;riparia;2006-06-21 09:45:41.391596733;15.329649910740661
-spring;riparia;2006-06-21 11:53:58.905174919;7.049382302575236
-spring;riparia;2006-06-21 13:16:19.235611187;5.7950824841439275
-spring;riparia;2006-06-21 14:33:31.418040829;6.1687457392071
-spring;riparia;2006-06-21 16:16:11.616303951;6.983920090343451
-spring;riparia;2006-06-21 17:49:45.611235759;8.646281490805144
-spring;riparia;2006-06-21 20:26:19.133581643;-1.739059512670135
+when;rootstock;date;t_leaf
+fall;berlandieri;2006-09-19 05:13:42;18.76517135209111
+fall;berlandieri;2006-09-19 08:08:52;18.813555406649364
+fall;berlandieri;2006-09-19 09:43:17;25.43808430069422
+fall;berlandieri;2006-09-19 10:56:11;28.548871154101178
+fall;berlandieri;2006-09-19 12:16:26;33.432779679723794
+fall;berlandieri;2006-09-19 14:01:59;33.95515728551189
+fall;berlandieri;2006-09-19 15:16:48;32.78618371800262
+fall;berlandieri;2006-09-19 17:05:43;30.551724915734706
+fall;riparia;2006-09-19 05:11:25;18.55722709883513
+fall;riparia;2006-09-19 08:12:28;19.011044423089412
+fall;riparia;2006-09-19 09:42:08;25.363247143613286
+fall;riparia;2006-09-19 10:58:16;29.15887612037756
+fall;riparia;2006-09-19 12:16:15;34.0327665348419
+fall;riparia;2006-09-19 14:05:46;34.13430258040254
+fall;riparia;2006-09-19 15:20:12;32.48984518984827
+fall;riparia;2006-09-19 17:05:43;31.082905703362027
+spring;berlandieri;2006-06-21 04:32:12;17.43283101476544
+spring;berlandieri;2006-06-21 08:27:00;27.695832100190454
+spring;berlandieri;2006-06-21 11:53:19;40.0938482341718
+spring;berlandieri;2006-06-21 13:11:52;41.783468016518995
+spring;berlandieri;2006-06-21 14:29:16;42.22623897317472
+spring;berlandieri;2006-06-21 16:11:04;41.593921931068714
+spring;berlandieri;2006-06-21 17:46:17;38.47084422420501
+spring;berlandieri;2006-06-21 20:25:40;28.06469148612223
+spring;riparia;2006-06-21 04:31:39;17.58017814037256
+spring;riparia;2006-06-21 08:27:11;27.62685336028682
+spring;riparia;2006-06-21 11:48:55;41.17370728059228
+spring;riparia;2006-06-21 13:12:14;43.10405418491427
+spring;riparia;2006-06-21 14:32:23;44.24738356570866
+spring;riparia;2006-06-21 16:08:09;43.37187065280673
+spring;riparia;2006-06-21 17:49:34;38.44097345239434
+spring;riparia;2006-06-21 20:27:19;28.06293364984756
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alsina2011-1.0.0/src/alsina2011/clean/diff_t_air_leaf.csv` & `alsina2011-1.1.0/src/alsina2011/clean/t_air.csv`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,53 @@
-# This file has been generated by fmt_diff_t_air_leaf.py
+# This file has been generated by fmt_t_air.py
 #
-# diff_t_air_leaf: [°C] difference t_leaf - t_air
+# t_air: [°C] temperature of atmosphere
 #
-when;rootstock;date;diff_t_air_leaf
-fall;berlandieri;2006-09-19 05:07:39.254239200;1.23179614601487
-fall;berlandieri;2006-09-19 08:08:33.791902248;1.2791264756887393
-fall;berlandieri;2006-09-19 09:38:19.078946537;-0.8698369690214012
-fall;berlandieri;2006-09-19 10:59:36.693855191;0.19374745850756003
-fall;berlandieri;2006-09-19 12:11:20.889366287;-0.5202744257520999
-fall;berlandieri;2006-09-19 14:08:26.289999813;-1.221466332494801
-fall;berlandieri;2006-09-19 15:18:31.138475644;-0.9185143700782961
-fall;berlandieri;2006-09-19 17:07:35.008099220;0.23504748008593923
-fall;riparia;2006-09-19 05:07:39.254239200;1.2299847383359923
-fall;riparia;2006-09-19 08:10:47.473817957;1.2582157236238016
-fall;riparia;2006-09-19 09:41:51.937275841;-0.9493516656234764
-fall;riparia;2006-09-19 11:01:38.291327339;-0.21517589562362094
-fall;riparia;2006-09-19 12:13:33.262432768;-0.4455374133718193
-fall;riparia;2006-09-19 14:02:59.436281550;-1.0670553122467128
-fall;riparia;2006-09-19 15:20:55.344973504;-0.9119533919303979
-fall;riparia;2006-09-19 17:08:29.943907929;0.11704670968336206
-spring;berlandieri;2006-06-21 04:27:06.989913650;1.874458100160671
-spring;berlandieri;2006-06-21 08:26:11.521323740;0.9865565332658264
-spring;berlandieri;2006-06-21 11:50:48.231612794;2.8035876892467275
-spring;berlandieri;2006-06-21 13:16:06.356354755;2.4291970125064086
-spring;berlandieri;2006-06-21 14:33:04.822617558;3.289541482577406
-spring;berlandieri;2006-06-21 16:09:17.918408941;2.957710376973248
-spring;berlandieri;2006-06-21 17:49:59.708749321;1.884481291272993
-spring;berlandieri;2006-06-21 20:29:42.335323205;1.4936918393490721
-spring;riparia;2006-06-21 04:32:52.666678089;1.9488919024472162
-spring;riparia;2006-06-21 08:25:23.212995910;0.47936054610426293
-spring;riparia;2006-06-21 11:51:16.888216566;1.114717006094823
-spring;riparia;2006-06-21 13:11:08.970634308;1.4573476898573552
-spring;riparia;2006-06-21 14:31:47.857685956;1.5474690138497889
-spring;riparia;2006-06-21 16:11:23.208952212;1.4595846208450314
-spring;riparia;2006-06-21 17:47:54.418206051;1.5437862957445647
-spring;riparia;2006-06-21 20:25:31.754236663;1.3744909213728436
+when;date;t_air
+fall;2006-09-19 00:59:51.247232765;12.756542750403192
+fall;2006-09-19 02:00:59.520760103;12.008359077152932
+fall;2006-09-19 02:59:33.443663445;11.327270977081017
+fall;2006-09-19 04:02:18.111726244;10.548889971554814
+fall;2006-09-19 04:59:56.112712424;10.317581329822406
+fall;2006-09-19 06:01:10.245091359;9.988816553812605
+fall;2006-09-19 07:02:24.374732513;10.80751142427113
+fall;2006-09-19 08:01:50.441415070;15.015199663972272
+fall;2006-09-19 09:01:16.510835409;18.323660317142796
+fall;2006-09-19 09:58:54.511821588;20.949901231609527
+fall;2006-09-19 11:00:53.910673565;25.275186093359363
+fall;2006-09-19 12:00:37.507368635;28.90720525395771
+fall;2006-09-19 12:59:00.769352295;31.537329552663877
+fall;2006-09-19 14:07:09.760442158;32.639189156582106
+fall;2006-09-19 14:59:21.423394370;33.504637147232216
+fall;2006-09-19 16:00:36.264858615;33.649517223439176
+fall;2006-09-19 17:00:01.614242518;33.6527113922449
+fall;2006-09-19 17:57:38.897930045;31.14997171978416
+fall;2006-09-19 19:00:41.085054233;28.45810429154711
+fall;2006-09-19 20:00:07.869035444;24.084697380117518
+fall;2006-09-19 21:01:22.718713032;19.46865325938125
+fall;2006-09-19 22:06:13.688832251;17.30375546905861
+fall;2006-09-19 22:58:26.069083116;16.247261783960603
+fall;2006-09-19 23:59:40.193248707;15.142368316558454
+spring;2006-06-21 01:04:03.228695697;14.359755778703615
+spring;2006-06-21 02:02:38.170056957;13.67979688080542
+spring;2006-06-21 03:06:18.757302769;13.339815604668
+spring;2006-06-21 04:03:56.761030017;13.243655555941857
+spring;2006-06-21 05:01:34.762019484;12.330128393353004
+spring;2006-06-21 06:02:48.894401912;12.137807077775172
+spring;2006-06-21 07:04:03.024046559;17.18625653373117
+spring;2006-06-21 08:03:29.090732506;20.98461439311741
+spring;2006-06-21 09:02:55.157418453;24.975293568081476
+spring;2006-06-21 10:00:33.161145701;28.96597274304554
+spring;2006-06-21 10:59:59.227831649;31.99504241661915
+spring;2006-06-21 12:04:49.483393693;34.399066291907864
+spring;2006-06-21 13:00:39.421424461;35.93764120178248
+spring;2006-06-21 14:00:05.488110409;37.13965313942684
+spring;2006-06-21 15:03:07.680713754;38.00510149577817
+spring;2006-06-21 16:00:45.681703221;37.95702074053977
+spring;2006-06-21 17:03:47.874306567;36.995411482774415
+spring;2006-06-21 18:05:02.001213432;35.264514161008975
+spring;2006-06-21 19:08:04.191078997;32.3796861440878
+spring;2006-06-21 20:03:54.129109765;27.427397345920713
+spring;2006-06-21 21:01:32.132837013;22.90783363952345
+spring;2006-06-21 22:02:46.262481659;21.128856293394943
+spring;2006-06-21 23:02:12.326429826;19.6864421631218
+spring;2006-06-22 00:03:26.455253138;18.2921086662745
```

### Comparing `alsina2011-1.0.0/src/alsina2011/clean/gs.csv` & `alsina2011-1.1.0/src/alsina2011/clean/vpd.csv`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,53 @@
-# This file has been generated by fmt_gs.py
+# This file has been generated by fmt_vpd.py
 #
-# gs: [mmol H2O m-2 s-1] stomatal conductance
+# vpd: [kPa] vapor pressure deficit
 #
-when;rootstock;date;gs
-fall;berlandieri;2006-09-19 05:02:09.722890270;0.03779293724398841
-fall;berlandieri;2006-09-19 08:02:02.105364884;0.07483009245672984
-fall;berlandieri;2006-09-19 09:45:11.855630700;0.1352988497520563
-fall;berlandieri;2006-09-19 10:52:39.001063264;0.1526836355072579
-fall;berlandieri;2006-09-19 14:01:46.877441519;0.09221482729580355
-fall;berlandieri;2006-09-19 15:15:50.798379171;0.12622853191474664
-fall;berlandieri;2006-09-19 17:01:39.258134282;0.09826169453931488
-fall;riparia;2006-09-19 04:59:31.009837272;0.03930465405486616
-fall;riparia;2006-09-19 07:58:04.039349090;0.07785354305052816
-fall;riparia;2006-09-19 09:43:52.499104202;0.09901757840281772
-fall;riparia;2006-09-19 10:51:19.644536765;0.13756639951030908
-fall;riparia;2006-09-19 14:00:27.524478722;0.1043085448107835
-fall;riparia;2006-09-19 15:18:29.511432168;0.10128514513311315
-fall;riparia;2006-09-19 17:00:19.905171486;0.105064445646329
-spring;berlandieri;2006-06-21 04:31:44.538817458;0.022675752163167417
-spring;berlandieri;2006-06-21 08:28:29.221640051;0.3189727732285443
-spring;berlandieri;2006-06-21 09:47:50.568683698;0.3537423107948624
-spring;berlandieri;2006-06-21 11:53:29.365645184;0.2653067161241041
-spring;berlandieri;2006-06-21 13:15:29.423959978;0.24943364717978023
-spring;berlandieri;2006-06-21 14:34:50.769221774;0.28949420207019205
-spring;berlandieri;2006-06-21 16:14:02.451689945;0.2622832655303058
-spring;berlandieri;2006-06-21 17:51:54.777631617;0.23582817890983715
-spring;berlandieri;2006-06-21 20:30:37.469937060;0.027966735543175858
-spring;riparia;2006-06-21 04:31:44.538817458;0.022675752163167417
-spring;riparia;2006-06-21 08:29:48.578166549;0.33408997528140794
-spring;riparia;2006-06-21 09:47:50.568683698;0.36508021233451005
-spring;riparia;2006-06-21 11:56:08.076916330;0.16402152007486298
-spring;riparia;2006-06-21 13:14:10.070997181;0.16704491975253338
-spring;riparia;2006-06-21 14:33:31.416258977;0.15721876896784875
-spring;riparia;2006-06-21 16:14:02.451689945;0.16250978629194257
-spring;riparia;2006-06-21 17:51:54.777631617;0.1836738555883174
-spring;riparia;2006-06-21 20:30:37.469937060;0.018896417705866253
+when;date;vpd
+fall;2006-09-19 00:57:50.651923423;0.08480544297070747
+fall;2006-09-19 01:59:00.182099271;0.12063828620861194
+fall;2006-09-19 03:02:40.766610934;0.03652512781793682
+fall;2006-09-19 03:57:44.184268003;0.09204998417165555
+fall;2006-09-19 05:03:05.946218938;0.07442665238561919
+fall;2006-09-19 06:06:51.138416235;0.02859997873589748
+fall;2006-09-19 07:05:34.208252997;-0.019359323116239224
+fall;2006-09-19 07:59:49.339664357;0.2014916461885372
+fall;2006-09-19 09:01:51.758295987;0.5168624879367947
+fall;2006-09-19 09:59:27.993419915;0.8159407323185732
+fall;2006-09-19 11:01:30.412051544;1.363606902011055
+fall;2006-09-19 12:01:13.255863618;2.149012196915278
+fall;2006-09-19 12:57:01.430766526;3.0644656072308925
+fall;2006-09-19 13:59:02.083529330;3.464765143152179
+fall;2006-09-19 14:56:56.872595945;3.745579734396591
+fall;2006-09-19 15:59:40.519473542;3.7295243799275926
+fall;2006-09-19 17:02:44.469735966;3.6865554920159807
+fall;2006-09-19 18:01:27.539572728;3.1353142658306536
+fall;2006-09-19 19:01:53.380237377;2.552023506548819
+fall;2006-09-19 20:00:16.141213751;1.5102551992463074
+fall;2006-09-19 21:00:30.499624360;0.7788822406884774
+fall;2006-09-19 22:01:44.621059156;0.5878047221268448
+fall;2006-09-19 23:01:07.161486403;0.4556209943256464
+fall;2006-09-19 23:57:12.116249829;0.31816676528177723
+spring;2006-06-21 01:04:03.228695697;0.14498392431498708
+spring;2006-06-21 02:02:38.170056957;0.1687811135050481
+spring;2006-06-21 03:06:18.757302769;0.15688273206626047
+spring;2006-06-21 04:03:56.761030017;0.12815737055687393
+spring;2006-06-21 05:01:34.762019484;0.15867686815673476
+spring;2006-06-21 06:07:54.537548683;0.13692150261056923
+spring;2006-06-21 07:04:03.024046559;0.3778198165601321
+spring;2006-06-21 08:06:01.913674782;0.9116001361784578
+spring;2006-06-21 09:02:55.157418453;1.4195427219002852
+spring;2006-06-21 10:03:05.984087978;2.2963368374744704
+spring;2006-06-21 10:59:59.227831649;3.3856112767900655
+spring;2006-06-21 12:02:16.660451417;4.532088325258528
+spring;2006-06-21 13:00:39.421424461;5.122576944704094
+spring;2006-06-21 14:00:05.488110409;5.5589835921329085
+spring;2006-06-21 15:00:34.857771478;5.972191422574726
+spring;2006-06-21 16:03:18.504645498;5.583028085195152
+spring;2006-06-21 17:03:47.874306567;4.986415295070981
+spring;2006-06-21 17:59:56.352591099;4.302780808290278
+spring;2006-06-21 19:05:31.368136720;3.298239172587005
+spring;2006-06-21 20:03:54.129109765;1.9676134623072041
+spring;2006-06-21 20:58:59.309894737;1.2362407166829064
+spring;2006-06-21 22:00:13.436801602;0.9368410325968402
+spring;2006-06-21 23:04:45.149372102;0.6963357787578675
+spring;2006-06-22 00:05:59.279290526;0.6070243790634047
```

### Comparing `alsina2011-1.0.0/src/alsina2011/clean/info.json` & `alsina2011-1.1.0/src/alsina2011/clean/info.json`

 * *Files identical despite different names*

### Comparing `alsina2011-1.0.0/src/alsina2011/clean/t_leaf.csv` & `alsina2011-1.1.0/src/alsina2011/clean/ec.csv`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-# This file has been generated by fmt_t_leaf.py
+# This file has been generated by fmt_ec.py
 #
-# t_leaf: [°C] leaf temperature
+# ec: [mmol vine-1 s-1] whole plant transpiration
 #
-when;rootstock;date;t_leaf
-fall;berlandieri;2006-09-19 05:13:42.121443241;18.76517135209111
-fall;berlandieri;2006-09-19 08:08:52.601398802;18.813555406649364
-fall;berlandieri;2006-09-19 09:43:17.582153540;25.43808430069422
-fall;berlandieri;2006-09-19 10:56:11.693461269;28.548871154101178
-fall;berlandieri;2006-09-19 12:16:26.932304328;33.432779679723794
-fall;berlandieri;2006-09-19 14:01:59.543972916;33.95515728551189
-fall;berlandieri;2006-09-19 15:16:48.112290302;32.78618371800262
-fall;berlandieri;2006-09-19 17:05:43.284149942;30.551724915734706
-fall;riparia;2006-09-19 05:11:25.979428229;18.55722709883513
-fall;riparia;2006-09-19 08:12:28.637143636;19.011044423089412
-fall;riparia;2006-09-19 09:42:08.907589020;25.363247143613286
-fall;riparia;2006-09-19 10:58:16.515867613;29.15887612037756
-fall;riparia;2006-09-19 12:16:15.722107184;34.0327665348419
-fall;riparia;2006-09-19 14:05:46.901120051;34.13430258040254
-fall;riparia;2006-09-19 15:20:12.939631624;32.48984518984827
-fall;riparia;2006-09-19 17:05:43.284149942;31.082905703362027
-spring;berlandieri;2006-06-21 04:32:12.024789981;17.43283101476544
-spring;berlandieri;2006-06-21 08:27:00.931119147;27.695832100190454
-spring;berlandieri;2006-06-21 11:53:19.646825388;40.0938482341718
-spring;berlandieri;2006-06-21 13:11:52.512640571;41.783468016518995
-spring;berlandieri;2006-06-21 14:29:16.954776331;42.22623897317472
-spring;berlandieri;2006-06-21 16:11:04.948465033;41.593921931068714
-spring;berlandieri;2006-06-21 17:46:17.238384663;38.47084422420501
-spring;berlandieri;2006-06-21 20:25:40.386547611;28.06469148612223
-spring;riparia;2006-06-21 04:31:39.481546230;17.58017814037256
-spring;riparia;2006-06-21 08:27:11.743690166;27.62685336028682
-spring;riparia;2006-06-21 11:48:55.846042684;41.17370728059228
-spring;riparia;2006-06-21 13:12:14.127402542;43.10405418491427
-spring;riparia;2006-06-21 14:32:23.704312945;44.24738356570866
-spring;riparia;2006-06-21 16:08:09.117030132;43.37187065280673
-spring;riparia;2006-06-21 17:49:34.800492296;38.44097345239434
-spring;riparia;2006-06-21 20:27:19.168466434;28.06293364984756
+when;rootstock;date;ec
+fall;berlandieri;2006-09-19 05:02:10;3.1584387999794927
+fall;berlandieri;2006-09-19 08:00:53;5.705223612508284
+fall;berlandieri;2006-09-19 09:44:38;13.66518898680767
+fall;berlandieri;2006-09-19 10:53:28;16.512585917623824
+fall;berlandieri;2006-09-19 14:02:05;13.283540167149571
+fall;berlandieri;2006-09-19 15:16:53;18.086097628459704
+fall;berlandieri;2006-09-19 17:02:10;14.153386114421053
+fall;riparia;2006-09-19 05:00:43;1.8705876924534763
+fall;riparia;2006-09-19 08:00:40;3.5598015844038144
+fall;riparia;2006-09-19 09:46:11;6.334750650592788
+fall;riparia;2006-09-19 10:53:14;9.96551038607048
+fall;riparia;2006-09-19 14:02:15;8.84372050721666
+fall;riparia;2006-09-19 15:16:28;8.988951859605095
+fall;riparia;2006-09-19 17:03:28;8.943029551621557
+spring;berlandieri;2006-06-21 04:29:17;1.1858725988482348
+spring;berlandieri;2006-06-21 08:26:21;18.198153271302985
+spring;berlandieri;2006-06-21 11:49:48;30.00209536815686
+spring;berlandieri;2006-06-21 13:10:18;29.561881019666657
+spring;berlandieri;2006-06-21 14:29:39;34.77947118149106
+spring;berlandieri;2006-06-21 16:08:51;31.69175817375067
+spring;berlandieri;2006-06-21 17:46:43;23.91506852102616
+spring;berlandieri;2006-06-21 20:23:56;2.1536581914922763
+spring;riparia;2006-06-21 04:29:58;0.4543869345703371
+spring;riparia;2006-06-21 08:24:00;8.162462190279353
+spring;riparia;2006-06-21 11:50:17;9.87525608562903
+spring;riparia;2006-06-21 13:11:08;10.319560221508418
+spring;riparia;2006-06-21 14:29:50;10.968026600501144
+spring;riparia;2006-06-21 16:09:30;10.60746680916705
+spring;riparia;2006-06-21 17:49:04;8.588978300052247
+spring;riparia;2006-06-21 20:25:38;0.5947991919153637
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `alsina2011-1.0.0/src/alsina2011/clean/vpd_leaf.csv` & `alsina2011-1.1.0/src/alsina2011/clean/diff_t_air_leaf.csv`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-# This file has been generated by fmt_vpd_leaf.py
+# This file has been generated by fmt_diff_t_air_leaf.py
 #
-# vpd: [kPa] vapor pressure deficit between leaf and atmosphere
+# diff_t_air_leaf: [°C] difference t_leaf - t_air
 #
-when;rootstock;date;vpd
-fall;berlandieri;2006-09-19 05:08:31.794376349;1.4392281512885443
-fall;berlandieri;2006-09-19 08:09:51.141384727;1.3136958752803087
-fall;berlandieri;2006-09-19 09:43:16.619828497;1.8060607570003135
-fall;berlandieri;2006-09-19 10:59:16.423436158;1.9980085872558329
-fall;berlandieri;2006-09-19 12:15:31.912798277;2.552680440742508
-fall;berlandieri;2006-09-19 14:03:06.344431096;2.4780734377273603
-fall;berlandieri;2006-09-19 15:16:43.869060797;2.6429421163787223
-fall;berlandieri;2006-09-19 17:02:59.620935017;2.4631770323029185
-fall;riparia;2006-09-19 05:08:31.794376349;1.4621544981730459
-fall;riparia;2006-09-19 08:08:20.626108495;1.3329051507026772
-fall;riparia;2006-09-19 09:41:51.725933627;1.8405286275984096
-fall;riparia;2006-09-19 11:00:30.079908434;2.1111571943026206
-fall;riparia;2006-09-19 12:15:37.534179640;2.6927070362734575
-fall;riparia;2006-09-19 14:04:36.863267419;2.4503987279256627
-fall;riparia;2006-09-19 15:19:33.665750759;2.697258802497518
-fall;riparia;2006-09-19 17:04:24.516609931;2.4696870746341455
-spring;berlandieri;2006-06-21 04:28:57.293146112;1.7601772999345862
-spring;berlandieri;2006-06-21 08:27:03.770168604;2.769427814247188
-spring;berlandieri;2006-06-21 11:53:22.484089065;5.439658657189007
-spring;berlandieri;2006-06-21 13:16:51.686988090;5.8379308714774805
-spring;berlandieri;2006-06-21 14:30:58.566996183;5.79655447772026
-spring;berlandieri;2006-06-21 16:12:46.560657367;5.630248095623502
-spring;berlandieri;2006-06-21 17:46:20.070362895;4.763496055801376
-spring;berlandieri;2006-06-21 20:27:22.005591171;3.265549423241512
-spring;riparia;2006-06-21 04:31:42.312009250;1.7143277305629105
-spring;riparia;2006-06-21 08:25:35.800821197;2.7313248275321413
-spring;riparia;2006-06-21 11:50:37.465225927;6.333810459848347
-spring;riparia;2006-06-21 13:13:55.744833254;6.67321398145571
-spring;riparia;2006-06-21 14:32:26.541533623;7.220375985467586
-spring;riparia;2006-06-21 16:11:29.516331669;6.783205745514323
-spring;riparia;2006-06-21 17:46:20.070362895;5.047062751822855
-spring;riparia;2006-06-21 20:27:22.005591171;3.3064468228551878
+when;rootstock;date;diff_t_air_leaf
+fall;berlandieri;2006-09-19 05:07:39;1.23179614601487
+fall;berlandieri;2006-09-19 08:08:33;1.2791264756887393
+fall;berlandieri;2006-09-19 09:38:19;-0.8698369690214012
+fall;berlandieri;2006-09-19 10:59:36;0.19374745850756003
+fall;berlandieri;2006-09-19 12:11:20;-0.5202744257520999
+fall;berlandieri;2006-09-19 14:08:26;-1.221466332494801
+fall;berlandieri;2006-09-19 15:18:31;-0.9185143700782961
+fall;berlandieri;2006-09-19 17:07:35;0.23504748008593923
+fall;riparia;2006-09-19 05:07:39;1.2299847383359923
+fall;riparia;2006-09-19 08:10:47;1.2582157236238016
+fall;riparia;2006-09-19 09:41:51;-0.9493516656234764
+fall;riparia;2006-09-19 11:01:38;-0.21517589562362094
+fall;riparia;2006-09-19 12:13:33;-0.4455374133718193
+fall;riparia;2006-09-19 14:02:59;-1.0670553122467128
+fall;riparia;2006-09-19 15:20:55;-0.9119533919303979
+fall;riparia;2006-09-19 17:08:29;0.11704670968336206
+spring;berlandieri;2006-06-21 04:27:06;1.874458100160671
+spring;berlandieri;2006-06-21 08:26:11;0.9865565332658264
+spring;berlandieri;2006-06-21 11:50:48;2.8035876892467275
+spring;berlandieri;2006-06-21 13:16:06;2.4291970125064086
+spring;berlandieri;2006-06-21 14:33:04;3.289541482577406
+spring;berlandieri;2006-06-21 16:09:17;2.957710376973248
+spring;berlandieri;2006-06-21 17:49:59;1.884481291272993
+spring;berlandieri;2006-06-21 20:29:42;1.4936918393490721
+spring;riparia;2006-06-21 04:32:52;1.9488919024472162
+spring;riparia;2006-06-21 08:25:23;0.47936054610426293
+spring;riparia;2006-06-21 11:51:16;1.114717006094823
+spring;riparia;2006-06-21 13:11:08;1.4573476898573552
+spring;riparia;2006-06-21 14:31:47;1.5474690138497889
+spring;riparia;2006-06-21 16:11:23;1.4595846208450314
+spring;riparia;2006-06-21 17:47:54;1.5437862957445647
+spring;riparia;2006-06-21 20:25:31;1.3744909213728436
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alsina2011-1.0.0/src/alsina2011.egg-info/SOURCES.txt` & `alsina2011-1.1.0/src/alsina2011.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
-MANIFEST.in
 README.rst
+pyproject.toml
 requirements.txt
 requirements_minimal.txt
-setup.cfg
-setup.py
 doc/Makefile
 doc/authors.rst
 doc/conf.py
 doc/contributing.rst
 doc/history.rst
 doc/index.rst
 doc/installation.rst
@@ -36,15 +34,15 @@
 doc/user/overview.rst
 src/alsina2011/__init__.py
 src/alsina2011/info.py
 src/alsina2011/version.py
 src/alsina2011.egg-info/PKG-INFO
 src/alsina2011.egg-info/SOURCES.txt
 src/alsina2011.egg-info/dependency_links.txt
-src/alsina2011.egg-info/not-zip-safe
+src/alsina2011.egg-info/requires.txt
 src/alsina2011.egg-info/top_level.txt
 src/alsina2011/clean/an.csv
 src/alsina2011/clean/diff_t_air_leaf.csv
 src/alsina2011/clean/ec.csv
 src/alsina2011/clean/gs.csv
 src/alsina2011/clean/info.json
 src/alsina2011/clean/readme.rst
```

### Comparing `alsina2011-1.0.0/test/conftest.py` & `alsina2011-1.1.0/test/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 
 import pytest
 # #}
 
 
 # {# pkglts, test.pytest_cmdline_preparse
-def pytest_cmdline_preparse(args):
-    if 'PYCHARM_HOSTED' not in os.environ:
-        args.append("--cov=alsina2011")
+# def pytest_cmdline_preparse(args):
+#
+#     if 'PYCHARM_HOSTED' not in os.environ:
+#         args.append("--cov=alsina2011")
+#
 # #}
 
 
 # {# pkglts, test.pytest_addoption
 def pytest_addoption(parser):
     parser.addoption("--runslow", action="store_true",
                      default=False, help="run slow tests")
```

