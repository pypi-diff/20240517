# Comparing `tmp/phylib-2.4.3.tar.gz` & `tmp/phylib-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phylib-2.4.3.tar", last modified: Thu Dec 22 12:24:24 2022, max compression
+gzip compressed data, was "phylib-2.5.0.tar", last modified: Fri May 17 18:17:42 2024, max compression
```

## Comparing `phylib-2.4.3.tar` & `phylib-2.5.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2022-12-22 12:24:24.011909 phylib-2.4.3/
--rw-rw-rw-   0        0        0     1463 2020-05-12 08:42:14.000000 phylib-2.4.3/LICENSE.md
--rw-rw-rw-   0        0        0      170 2020-05-12 08:42:14.000000 phylib-2.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1158 2022-12-22 12:24:24.011909 phylib-2.4.3/PKG-INFO
--rw-rw-rw-   0        0        0      452 2020-05-12 08:42:14.000000 phylib-2.4.3/README.md
-drwxrwxrwx   0        0        0        0 2022-12-22 12:24:23.961909 phylib-2.4.3/phylib/
--rw-rw-rw-   0        0        0     2540 2022-12-22 12:22:38.000000 phylib-2.4.3/phylib/__init__.py
--rw-rw-rw-   0        0        0     1058 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/conftest.py
-drwxrwxrwx   0        0        0        0 2022-12-22 12:24:23.973911 phylib-2.4.3/phylib/electrode/
--rw-rw-rw-   0        0        0       92 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/electrode/__init__.py
--rw-rw-rw-   0        0        0     5254 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/electrode/mea.py
-drwxrwxrwx   0        0        0        0 2022-12-22 12:24:23.974916 phylib-2.4.3/phylib/electrode/probes/
--rw-rw-rw-   0        0        0     2558 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/electrode/probes/1x32_buzsaki.prb
-drwxrwxrwx   0        0        0        0 2022-12-22 12:24:23.976909 phylib-2.4.3/phylib/electrode/tests/
--rw-rw-rw-   0        0        0        0 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/electrode/tests/__init__.py
--rw-rw-rw-   0        0        0     3081 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/electrode/tests/test_mea.py
-drwxrwxrwx   0        0        0        0 2022-12-22 12:24:23.984909 phylib-2.4.3/phylib/io/
--rw-rw-rw-   0        0        0      227 2021-01-15 17:19:39.000000 phylib-2.4.3/phylib/io/__init__.py
--rw-rw-rw-   0        0        0    13321 2022-11-10 09:44:55.000000 phylib-2.4.3/phylib/io/alf.py
--rw-rw-rw-   0        0        0    14713 2022-06-07 11:28:53.000000 phylib-2.4.3/phylib/io/array.py
--rw-rw-rw-   0        0        0     4203 2022-06-07 11:28:53.000000 phylib-2.4.3/phylib/io/datasets.py
--rw-rw-rw-   0        0        0    12293 2022-06-07 11:28:53.000000 phylib-2.4.3/phylib/io/merge.py
--rw-rw-rw-   0        0        0     1288 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/io/mock.py
--rw-rw-rw-   0        0        0    59158 2022-11-10 09:47:23.000000 phylib-2.4.3/phylib/io/model.py
-drwxrwxrwx   0        0        0        0 2022-12-22 12:24:23.993910 phylib-2.4.3/phylib/io/tests/
--rw-rw-rw-   0        0        0        0 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/io/tests/__init__.py
--rw-rw-rw-   0        0        0     5127 2022-11-10 09:40:50.000000 phylib-2.4.3/phylib/io/tests/conftest.py
--rw-rw-rw-   0        0        0    11278 2022-11-10 09:48:37.000000 phylib-2.4.3/phylib/io/tests/test_alf.py
--rw-rw-rw-   0        0        0    11800 2021-01-15 17:19:39.000000 phylib-2.4.3/phylib/io/tests/test_array.py
--rw-rw-rw-   0        0        0     4732 2022-06-07 11:28:53.000000 phylib-2.4.3/phylib/io/tests/test_datasets.py
--rw-rw-rw-   0        0        0     5419 2022-06-07 11:28:53.000000 phylib-2.4.3/phylib/io/tests/test_merge.py
--rw-rw-rw-   0        0        0     2396 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/io/tests/test_mock.py
--rw-rw-rw-   0        0        0     7137 2022-11-10 09:40:50.000000 phylib-2.4.3/phylib/io/tests/test_model.py
--rw-rw-rw-   0        0        0     8169 2022-06-07 11:28:53.000000 phylib-2.4.3/phylib/io/tests/test_traces.py
--rw-rw-rw-   0        0        0    23633 2022-12-22 12:21:14.000000 phylib-2.4.3/phylib/io/traces.py
-drwxrwxrwx   0        0        0        0 2022-12-22 12:24:23.996909 phylib-2.4.3/phylib/stats/
--rw-rw-rw-   0        0        0      112 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/stats/__init__.py
--rw-rw-rw-   0        0        0     6193 2022-06-07 11:28:53.000000 phylib-2.4.3/phylib/stats/ccg.py
--rw-rw-rw-   0        0        0     2527 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/stats/clusters.py
-drwxrwxrwx   0        0        0        0 2022-12-22 12:24:23.999909 phylib-2.4.3/phylib/stats/tests/
--rw-rw-rw-   0        0        0        0 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/stats/tests/__init__.py
--rw-rw-rw-   0        0        0     5818 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/stats/tests/test_ccg.py
--rw-rw-rw-   0        0        0     3929 2022-06-07 11:28:53.000000 phylib-2.4.3/phylib/stats/tests/test_clusters.py
-drwxrwxrwx   0        0        0        0 2022-12-22 12:24:24.005909 phylib-2.4.3/phylib/utils/
--rw-rw-rw-   0        0        0      423 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/utils/__init__.py
--rw-rw-rw-   0        0        0    11269 2021-01-15 17:19:39.000000 phylib-2.4.3/phylib/utils/_misc.py
--rw-rw-rw-   0        0        0     3109 2022-06-07 11:28:53.000000 phylib-2.4.3/phylib/utils/_types.py
--rw-rw-rw-   0        0        0     9523 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/utils/event.py
--rw-rw-rw-   0        0        0     6770 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/utils/geometry.py
--rw-rw-rw-   0        0        0     2168 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/utils/testing.py
-drwxrwxrwx   0        0        0        0 2022-12-22 12:24:24.010909 phylib-2.4.3/phylib/utils/tests/
--rw-rw-rw-   0        0        0        0 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/utils/tests/__init__.py
--rw-rw-rw-   0        0        0     3344 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/utils/tests/test_event.py
--rw-rw-rw-   0        0        0     4119 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/utils/tests/test_geometry.py
--rw-rw-rw-   0        0        0     4056 2020-05-12 08:42:14.000000 phylib-2.4.3/phylib/utils/tests/test_misc.py
--rw-rw-rw-   0        0        0     1334 2022-11-10 09:40:39.000000 phylib-2.4.3/phylib/utils/tests/test_testing.py
--rw-rw-rw-   0        0        0     2721 2022-06-07 11:28:53.000000 phylib-2.4.3/phylib/utils/tests/test_types.py
-drwxrwxrwx   0        0        0        0 2022-12-22 12:24:23.971909 phylib-2.4.3/phylib.egg-info/
--rw-rw-rw-   0        0        0     1158 2022-12-22 12:24:23.000000 phylib-2.4.3/phylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1334 2022-12-22 12:24:23.000000 phylib-2.4.3/phylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-22 12:24:23.000000 phylib-2.4.3/phylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2022-12-22 12:24:23.000000 phylib-2.4.3/phylib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-12-22 12:24:23.000000 phylib-2.4.3/phylib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      489 2022-12-22 12:24:24.013909 phylib-2.4.3/setup.cfg
--rw-rw-rw-   0        0        0     2151 2020-05-12 08:42:14.000000 phylib-2.4.3/setup.py
+drwxr-xr-x   0 olivier    (501) staff       (20)        0 2024-05-17 18:17:42.178711 phylib-2.5.0/
+-rw-r--r--   0 olivier    (501) staff       (20)     1463 2021-04-12 21:04:56.000000 phylib-2.5.0/LICENSE.md
+-rw-r--r--   0 olivier    (501) staff       (20)      170 2021-04-12 21:04:56.000000 phylib-2.5.0/MANIFEST.in
+-rw-r--r--   0 olivier    (501) staff       (20)     1111 2024-05-17 18:17:42.178812 phylib-2.5.0/PKG-INFO
+-rw-r--r--   0 olivier    (501) staff       (20)      452 2021-04-12 21:04:56.000000 phylib-2.5.0/README.md
+drwxr-xr-x   0 olivier    (501) staff       (20)        0 2024-05-17 18:17:42.160822 phylib-2.5.0/phylib/
+-rw-r--r--   0 olivier    (501) staff       (20)     2505 2024-05-17 18:14:10.000000 phylib-2.5.0/phylib/__init__.py
+-rw-r--r--   0 olivier    (501) staff       (20)     1058 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/conftest.py
+drwxr-xr-x   0 olivier    (501) staff       (20)        0 2024-05-17 18:17:42.162225 phylib-2.5.0/phylib/electrode/
+-rw-r--r--   0 olivier    (501) staff       (20)       92 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/electrode/__init__.py
+-rw-r--r--   0 olivier    (501) staff       (20)     5254 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/electrode/mea.py
+drwxr-xr-x   0 olivier    (501) staff       (20)        0 2024-05-17 18:17:42.162612 phylib-2.5.0/phylib/electrode/probes/
+-rw-r--r--   0 olivier    (501) staff       (20)     2558 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/electrode/probes/1x32_buzsaki.prb
+drwxr-xr-x   0 olivier    (501) staff       (20)        0 2024-05-17 18:17:42.163196 phylib-2.5.0/phylib/electrode/tests/
+-rw-r--r--   0 olivier    (501) staff       (20)        0 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/electrode/tests/__init__.py
+-rw-r--r--   0 olivier    (501) staff       (20)     3081 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/electrode/tests/test_mea.py
+drwxr-xr-x   0 olivier    (501) staff       (20)        0 2024-05-17 18:17:42.166950 phylib-2.5.0/phylib/io/
+-rw-r--r--   0 olivier    (501) staff       (20)      227 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/io/__init__.py
+-rw-r--r--   0 olivier    (501) staff       (20)    13378 2024-05-17 18:14:10.000000 phylib-2.5.0/phylib/io/alf.py
+-rw-r--r--   0 olivier    (501) staff       (20)    14713 2024-05-17 18:14:10.000000 phylib-2.5.0/phylib/io/array.py
+-rw-r--r--   0 olivier    (501) staff       (20)     4203 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/io/datasets.py
+-rw-r--r--   0 olivier    (501) staff       (20)    12293 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/io/merge.py
+-rw-r--r--   0 olivier    (501) staff       (20)     1288 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/io/mock.py
+-rw-r--r--   0 olivier    (501) staff       (20)    59193 2024-05-17 18:14:10.000000 phylib-2.5.0/phylib/io/model.py
+drwxr-xr-x   0 olivier    (501) staff       (20)        0 2024-05-17 18:17:42.171302 phylib-2.5.0/phylib/io/tests/
+-rw-r--r--   0 olivier    (501) staff       (20)        0 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/io/tests/__init__.py
+-rw-r--r--   0 olivier    (501) staff       (20)     5127 2022-11-12 20:32:31.000000 phylib-2.5.0/phylib/io/tests/conftest.py
+-rw-r--r--   0 olivier    (501) staff       (20)    11278 2022-11-12 20:32:31.000000 phylib-2.5.0/phylib/io/tests/test_alf.py
+-rw-r--r--   0 olivier    (501) staff       (20)    11800 2024-05-17 18:14:10.000000 phylib-2.5.0/phylib/io/tests/test_array.py
+-rw-r--r--   0 olivier    (501) staff       (20)     4732 2021-09-10 15:10:44.000000 phylib-2.5.0/phylib/io/tests/test_datasets.py
+-rw-r--r--   0 olivier    (501) staff       (20)     5419 2021-09-10 15:10:44.000000 phylib-2.5.0/phylib/io/tests/test_merge.py
+-rw-r--r--   0 olivier    (501) staff       (20)     2396 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/io/tests/test_mock.py
+-rw-r--r--   0 olivier    (501) staff       (20)     7137 2022-11-12 20:32:31.000000 phylib-2.5.0/phylib/io/tests/test_model.py
+-rw-r--r--   0 olivier    (501) staff       (20)     8169 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/io/tests/test_traces.py
+-rw-r--r--   0 olivier    (501) staff       (20)    23633 2024-05-17 18:14:10.000000 phylib-2.5.0/phylib/io/traces.py
+drwxr-xr-x   0 olivier    (501) staff       (20)        0 2024-05-17 18:17:42.172399 phylib-2.5.0/phylib/stats/
+-rw-r--r--   0 olivier    (501) staff       (20)      112 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/stats/__init__.py
+-rw-r--r--   0 olivier    (501) staff       (20)     6193 2021-08-08 15:43:26.000000 phylib-2.5.0/phylib/stats/ccg.py
+-rw-r--r--   0 olivier    (501) staff       (20)     2527 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/stats/clusters.py
+drwxr-xr-x   0 olivier    (501) staff       (20)        0 2024-05-17 18:17:42.173240 phylib-2.5.0/phylib/stats/tests/
+-rw-r--r--   0 olivier    (501) staff       (20)        0 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/stats/tests/__init__.py
+-rw-r--r--   0 olivier    (501) staff       (20)     5818 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/stats/tests/test_ccg.py
+-rw-r--r--   0 olivier    (501) staff       (20)     3929 2024-05-17 18:14:10.000000 phylib-2.5.0/phylib/stats/tests/test_clusters.py
+drwxr-xr-x   0 olivier    (501) staff       (20)        0 2024-05-17 18:17:42.177173 phylib-2.5.0/phylib/utils/
+-rw-r--r--   0 olivier    (501) staff       (20)      423 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/utils/__init__.py
+-rw-r--r--   0 olivier    (501) staff       (20)    11269 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/utils/_misc.py
+-rw-r--r--   0 olivier    (501) staff       (20)     3109 2021-08-08 15:43:26.000000 phylib-2.5.0/phylib/utils/_types.py
+-rw-r--r--   0 olivier    (501) staff       (20)     9523 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/utils/event.py
+-rw-r--r--   0 olivier    (501) staff       (20)     6770 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/utils/geometry.py
+-rw-r--r--   0 olivier    (501) staff       (20)     2168 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/utils/testing.py
+drwxr-xr-x   0 olivier    (501) staff       (20)        0 2024-05-17 18:17:42.178463 phylib-2.5.0/phylib/utils/tests/
+-rw-r--r--   0 olivier    (501) staff       (20)        0 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/utils/tests/__init__.py
+-rw-r--r--   0 olivier    (501) staff       (20)     3344 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/utils/tests/test_event.py
+-rw-r--r--   0 olivier    (501) staff       (20)     4119 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/utils/tests/test_geometry.py
+-rw-r--r--   0 olivier    (501) staff       (20)     4056 2021-04-12 21:04:56.000000 phylib-2.5.0/phylib/utils/tests/test_misc.py
+-rw-r--r--   0 olivier    (501) staff       (20)     1334 2022-11-12 20:32:31.000000 phylib-2.5.0/phylib/utils/tests/test_testing.py
+-rw-r--r--   0 olivier    (501) staff       (20)     2721 2021-08-08 15:43:26.000000 phylib-2.5.0/phylib/utils/tests/test_types.py
+drwxr-xr-x   0 olivier    (501) staff       (20)        0 2024-05-17 18:17:42.161807 phylib-2.5.0/phylib.egg-info/
+-rw-r--r--   0 olivier    (501) staff       (20)     1111 2024-05-17 18:17:42.000000 phylib-2.5.0/phylib.egg-info/PKG-INFO
+-rw-r--r--   0 olivier    (501) staff       (20)     1334 2024-05-17 18:17:42.000000 phylib-2.5.0/phylib.egg-info/SOURCES.txt
+-rw-r--r--   0 olivier    (501) staff       (20)        1 2024-05-17 18:17:42.000000 phylib-2.5.0/phylib.egg-info/dependency_links.txt
+-rw-r--r--   0 olivier    (501) staff       (20)       52 2024-05-17 18:17:42.000000 phylib-2.5.0/phylib.egg-info/requires.txt
+-rw-r--r--   0 olivier    (501) staff       (20)        7 2024-05-17 18:17:42.000000 phylib-2.5.0/phylib.egg-info/top_level.txt
+-rw-r--r--   0 olivier    (501) staff       (20)      455 2024-05-17 18:17:42.179683 phylib-2.5.0/setup.cfg
+-rw-r--r--   0 olivier    (501) staff       (20)     2151 2021-04-12 21:04:56.000000 phylib-2.5.0/setup.py
```

### Comparing `phylib-2.4.3/LICENSE.md` & `phylib-2.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/PKG-INFO` & `phylib-2.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-Metadata-Version: 2.1
-Name: phylib
-Version: 2.4.3
-Summary: Ephys data analysis for thousands of channels
-Home-page: https://github.com/cortex-lab/phylib
-Author: Cyrille Rossant
-Author-email: cyrille.rossant@gmail.com
-License: BSD
-Keywords: phy,data analysis,electrophysiology,neuroscience
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Framework :: IPython
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# phylib
-[![Build Status](https://img.shields.io/travis/cortex-lab/phylib.svg)](https://travis-ci.org/cortex-lab/phylib)
-[![codecov.io](https://img.shields.io/codecov/c/github/cortex-lab/phylib.svg)](http://codecov.io/github/cortex-lab/phylib?branch=master)
-
-Electrophysiological data analysis library used by [phy](https://github.com/kwikteam/phy/), a spike sorting visualization software, and [ibllib](https://github.com/int-brain-lab/ibllib/).
-
-
+Metadata-Version: 2.1
+Name: phylib
+Version: 2.5.0
+Summary: Ephys data analysis for thousands of channels
+Home-page: https://github.com/cortex-lab/phylib
+Author: Cyrille Rossant
+Author-email: cyrille.rossant@gmail.com
+License: BSD
+Keywords: phy,data analysis,electrophysiology,neuroscience
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Framework :: IPython
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# phylib
+[![Build Status](https://img.shields.io/travis/cortex-lab/phylib.svg)](https://travis-ci.org/cortex-lab/phylib)
+[![codecov.io](https://img.shields.io/codecov/c/github/cortex-lab/phylib.svg)](http://codecov.io/github/cortex-lab/phylib?branch=master)
+
+Electrophysiological data analysis library used by [phy](https://github.com/kwikteam/phy/), a spike sorting visualization software, and [ibllib](https://github.com/int-brain-lab/ibllib/).
```

### Comparing `phylib-2.4.3/phylib/__init__.py` & `phylib-2.5.0/phylib/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,30 +5,28 @@
 
 
 #------------------------------------------------------------------------------
 # Imports
 #------------------------------------------------------------------------------
 
 import atexit
-from io import StringIO
 import logging
 import os.path as op
-import sys
 
 from .utils._misc import _git_version
 from .utils.event import connect, unconnect, emit
 
 
 #------------------------------------------------------------------------------
 # Global variables and functions
 #------------------------------------------------------------------------------
 
 __author__ = 'Cyrille Rossant'
 __email__ = 'cyrille.rossant at gmail.com'
-__version__ = '2.4.3'
+__version__ = '2.5.0'
 __version_git__ = __version__ + _git_version()
 
 
 # Set a null handler on the root logger
 logger = logging.getLogger('phylib')
 logger.setLevel(logging.DEBUG)
 logger.addHandler(logging.NullHandler())
```

### Comparing `phylib-2.4.3/phylib/conftest.py` & `phylib-2.5.0/phylib/conftest.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/electrode/mea.py` & `phylib-2.5.0/phylib/electrode/mea.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/electrode/probes/1x32_buzsaki.prb` & `phylib-2.5.0/phylib/electrode/probes/1x32_buzsaki.prb`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/electrode/tests/test_mea.py` & `phylib-2.5.0/phylib/electrode/tests/test_mea.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/io/alf.py` & `phylib-2.5.0/phylib/io/alf.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 _FILE_RENAMES = [  # file_in, file_out, squeeze (bool to squeeze vector from matlab in npy)
     ('params.py', 'params.py', None),
     ('cluster_KSLabel.tsv', 'cluster_KSLabel.tsv', None),
     ('spike_clusters.npy', 'spikes.clusters.npy', True),
     ('spike_templates.npy', 'spikes.templates.npy', True),
     ('channel_positions.npy', 'channels.localCoordinates.npy', False),
     ('channel_probe.npy', 'channels.probes.npy', True),
+    ('channel_labels.npy', 'channels.labels.npy', True),
     ('cluster_probes.npy', 'clusters.probes.npy', True),
     ('cluster_shanks.npy', 'clusters.shanks.npy', True),
     ('whitening_mat.npy', '_kilosort_whitening.matrix.npy', False),
     ('_phy_spikes_subset.channels.npy', '_phy_spikes_subset.channels.npy', False),
     ('_phy_spikes_subset.spikes.npy', '_phy_spikes_subset.spikes.npy', False),
     ('_phy_spikes_subset.waveforms.npy', '_phy_spikes_subset.waveforms.npy', False),
     ('drift_depths.um.npy', 'drift_depths.um.npy', False),
```

### Comparing `phylib-2.4.3/phylib/io/array.py` & `phylib-2.5.0/phylib/io/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
 # Spike clusters utility functions
 # -----------------------------------------------------------------------------
 
 def _spikes_in_clusters(spike_clusters, clusters):
     """Return the ids of all spikes belonging to the specified clusters."""
     if len(spike_clusters) == 0 or len(clusters) == 0:
         return np.array([], dtype=int)
-    return np.nonzero(np.in1d(spike_clusters, clusters))[0]
+    return np.nonzero(np.isin(spike_clusters, clusters))[0]
 
 
 def _spikes_per_cluster(spike_clusters, spike_ids=None):
     """Return a dictionary {cluster: list_of_spikes}."""
     if spike_clusters is None or not len(spike_clusters):
         return {}
     if spike_ids is None:
```

### Comparing `phylib-2.4.3/phylib/io/datasets.py` & `phylib-2.5.0/phylib/io/datasets.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/io/merge.py` & `phylib-2.5.0/phylib/io/merge.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/io/mock.py` & `phylib-2.5.0/phylib/io/mock.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/io/model.py` & `phylib-2.5.0/phylib/io/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,16 +86,16 @@
     assert data.ndim >= 2
     assert cols.ndim == 2
     assert data.shape[:2] == cols.shape
     n_spikes, n_channels_loc = shape[:2]
     # NOTE: we ensure here that `col` contains integers.
     c = cols.flatten().astype(np.int32)
     # Remove columns that do not belong to the specified channels.
-    c[~np.in1d(c, channel_ids)] = -1
-    assert np.all(np.in1d(c, np.r_[channel_ids, -1]))
+    c[~np.isin(c, channel_ids)] = -1
+    assert np.all(np.isin(c, np.r_[channel_ids, -1]))
     # Convert column indices to relative indices given the specified
     # channel_ids.
     cols_loc = _index_of(c, np.r_[channel_ids, -1]).reshape(cols.shape)
     assert cols_loc.shape == (n_spikes, n_channels_loc)
     n_channels = len(channel_ids)
     # Shape of the output array.
     out_shape = shape
@@ -323,15 +323,15 @@
 
         # Set dat_path.
         if not self.dat_path:  # pragma: no cover
             self.dat_path = []
         elif not isinstance(self.dat_path, (list, tuple)):
             self.dat_path = [self.dat_path]
         assert isinstance(self.dat_path, (list, tuple))
-        self.dat_path = [Path(_).resolve() for _ in self.dat_path]
+        self.dat_path = [Path(p).resolve() if not Path(p).is_symlink() else p for p in self.dat_path]
 
         self.dtype = getattr(self, 'dtype', np.int16)
         if not self.sample_rate:  # pragma: no cover
             logger.warning("No sample rate was given! Defaulting to 1 Hz.")
         self.sample_rate = float(self.sample_rate or 1.)
         assert self.sample_rate > 0
         self.offset = getattr(self, 'offset', 0)
```

### Comparing `phylib-2.4.3/phylib/io/tests/conftest.py` & `phylib-2.5.0/phylib/io/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/io/tests/test_alf.py` & `phylib-2.5.0/phylib/io/tests/test_alf.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/io/tests/test_array.py` & `phylib-2.5.0/phylib/io/tests/test_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,15 +284,15 @@
 
     ae(_spikes_in_clusters(spike_clusters, []), [])
 
     for i in range(n_clusters):
         assert np.all(spike_clusters[_spikes_in_clusters(spike_clusters, [i])] == i)
 
     clusters = [1, 2, 3]
-    assert np.all(np.in1d(
+    assert np.all(np.isin(
         spike_clusters[_spikes_in_clusters(spike_clusters, clusters)], clusters))
 
 
 def test_spikes_per_cluster():
     """Test _spikes_per_cluster()."""
 
     n_spikes = 100
```

### Comparing `phylib-2.4.3/phylib/io/tests/test_datasets.py` & `phylib-2.5.0/phylib/io/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/io/tests/test_merge.py` & `phylib-2.5.0/phylib/io/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/io/tests/test_mock.py` & `phylib-2.5.0/phylib/io/tests/test_mock.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/io/tests/test_model.py` & `phylib-2.5.0/phylib/io/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/io/tests/test_traces.py` & `phylib-2.5.0/phylib/io/tests/test_traces.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/io/traces.py` & `phylib-2.5.0/phylib/io/traces.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/stats/ccg.py` & `phylib-2.5.0/phylib/stats/ccg.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/stats/clusters.py` & `phylib-2.5.0/phylib/stats/clusters.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/stats/tests/test_ccg.py` & `phylib-2.5.0/phylib/stats/tests/test_ccg.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/stats/tests/test_clusters.py` & `phylib-2.5.0/phylib/stats/tests/test_clusters.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 def test_sorted_main_channels(masks):
     masks *= .05
     masks[:, [5, 7]] *= 20
     mean_masks = mean(masks)
     channels = get_sorted_main_channels(mean_masks,
                                         get_unmasked_channels(mean_masks))
-    assert np.all(np.in1d(channels, [5, 7]))
+    assert np.all(np.isin(channels, [5, 7]))
 
 
 def test_waveform_amplitude(masks, waveforms):
     waveforms *= .1
     masks *= .1
 
     waveforms[:, 10, :] *= 10
```

### Comparing `phylib-2.4.3/phylib/utils/_misc.py` & `phylib-2.5.0/phylib/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/utils/_types.py` & `phylib-2.5.0/phylib/utils/_types.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/utils/event.py` & `phylib-2.5.0/phylib/utils/event.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/utils/geometry.py` & `phylib-2.5.0/phylib/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/utils/testing.py` & `phylib-2.5.0/phylib/utils/testing.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/utils/tests/test_event.py` & `phylib-2.5.0/phylib/utils/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/utils/tests/test_geometry.py` & `phylib-2.5.0/phylib/utils/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/utils/tests/test_misc.py` & `phylib-2.5.0/phylib/utils/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/utils/tests/test_testing.py` & `phylib-2.5.0/phylib/utils/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib/utils/tests/test_types.py` & `phylib-2.5.0/phylib/utils/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/phylib.egg-info/PKG-INFO` & `phylib-2.5.0/phylib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-Metadata-Version: 2.1
-Name: phylib
-Version: 2.4.3
-Summary: Ephys data analysis for thousands of channels
-Home-page: https://github.com/cortex-lab/phylib
-Author: Cyrille Rossant
-Author-email: cyrille.rossant@gmail.com
-License: BSD
-Keywords: phy,data analysis,electrophysiology,neuroscience
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Framework :: IPython
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# phylib
-[![Build Status](https://img.shields.io/travis/cortex-lab/phylib.svg)](https://travis-ci.org/cortex-lab/phylib)
-[![codecov.io](https://img.shields.io/codecov/c/github/cortex-lab/phylib.svg)](http://codecov.io/github/cortex-lab/phylib?branch=master)
-
-Electrophysiological data analysis library used by [phy](https://github.com/kwikteam/phy/), a spike sorting visualization software, and [ibllib](https://github.com/int-brain-lab/ibllib/).
-
-
+Metadata-Version: 2.1
+Name: phylib
+Version: 2.5.0
+Summary: Ephys data analysis for thousands of channels
+Home-page: https://github.com/cortex-lab/phylib
+Author: Cyrille Rossant
+Author-email: cyrille.rossant@gmail.com
+License: BSD
+Keywords: phy,data analysis,electrophysiology,neuroscience
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Framework :: IPython
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# phylib
+[![Build Status](https://img.shields.io/travis/cortex-lab/phylib.svg)](https://travis-ci.org/cortex-lab/phylib)
+[![codecov.io](https://img.shields.io/codecov/c/github/cortex-lab/phylib.svg)](http://codecov.io/github/cortex-lab/phylib?branch=master)
+
+Electrophysiological data analysis library used by [phy](https://github.com/kwikteam/phy/), a spike sorting visualization software, and [ibllib](https://github.com/int-brain-lab/ibllib/).
```

### Comparing `phylib-2.4.3/phylib.egg-info/SOURCES.txt` & `phylib-2.5.0/phylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phylib-2.4.3/setup.py` & `phylib-2.5.0/setup.py`

 * *Files identical despite different names*

