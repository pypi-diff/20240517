# Comparing `tmp/caom2-2.5.tar.gz` & `tmp/caom2-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caom2-2.5.tar", last modified: Fri Jul 15 22:48:57 2022, max compression
+gzip compressed data, was "caom2-2.6.tar", last modified: Thu Dec 22 19:41:25 2022, max compression
```

## Comparing `caom2-2.5.tar` & `caom2-2.6.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 22:48:57.653402 caom2-2.5/
--rw-r--r--   0 runner    (1001) docker     (121)    34520 2022-07-15 22:48:48.000000 caom2-2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-07-15 22:48:48.000000 caom2-2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    16180 2022-07-15 22:48:57.653402 caom2-2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15573 2022-07-15 22:48:48.000000 caom2-2.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 22:48:57.649402 caom2-2.5/caom2/
--rw-r--r--   0 runner    (1001) docker     (121)     4826 2022-07-15 22:48:48.000000 caom2-2.5/caom2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10790 2022-07-15 22:48:48.000000 caom2-2.5/caom2/artifact.py
--rw-r--r--   0 runner    (1001) docker     (121)    15206 2022-07-15 22:48:48.000000 caom2-2.5/caom2/caom_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    19257 2022-07-15 22:48:48.000000 caom2-2.5/caom2/checksum.py
--rw-r--r--   0 runner    (1001) docker     (121)    29512 2022-07-15 22:48:48.000000 caom2-2.5/caom2/chunk.py
--rw-r--r--   0 runner    (1001) docker     (121)    17849 2022-07-15 22:48:48.000000 caom2-2.5/caom2/common.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 22:48:57.649402 caom2-2.5/caom2/data/
--rw-r--r--   0 runner    (1001) docker     (121)    31423 2022-07-15 22:48:48.000000 caom2-2.5/caom2/data/CAOM-2.2.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    33504 2022-07-15 22:48:48.000000 caom2-2.5/caom2/data/CAOM-2.3.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    36574 2022-07-15 22:48:48.000000 caom2-2.5/caom2/data/CAOM-2.4.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    18468 2022-07-15 22:48:48.000000 caom2-2.5/caom2/diff.py
--rw-r--r--   0 runner    (1001) docker     (121)   123816 2022-07-15 22:48:48.000000 caom2-2.5/caom2/obs_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)    38282 2022-07-15 22:48:48.000000 caom2-2.5/caom2/observation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6152 2022-07-15 22:48:48.000000 caom2-2.5/caom2/part.py
--rw-r--r--   0 runner    (1001) docker     (121)    40440 2022-07-15 22:48:48.000000 caom2-2.5/caom2/plane.py
--rw-r--r--   0 runner    (1001) docker     (121)    13519 2022-07-15 22:48:48.000000 caom2-2.5/caom2/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 22:48:57.653402 caom2-2.5/caom2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28238 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/caom_test_instances.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 22:48:57.653402 caom2-2.5/caom2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)     4561 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/CompleteCompositeCircle-CAOM-2.2.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4743 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/CompleteCompositeCircle-CAOM-2.3.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4480 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/CompleteCompositePolygon-CAOM-2.2.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4662 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/CompleteCompositePolygon-CAOM-2.3.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4456 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/CompleteSimpleCircle-CAOM-2.2.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4630 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/CompleteSimpleCircle-CAOM-2.3.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4458 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/CompleteSimplePolygon-CAOM-2.2.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4686 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/CompleteSimplePolygon-CAOM-2.3.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1445 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/MinimalCompositeCircle-CAOM-2.2.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/MinimalCompositeCircle-CAOM-2.3.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1445 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/MinimalCompositePolygon-CAOM-2.2.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/MinimalCompositePolygon-CAOM-2.3.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/MinimalSimpleCircle-CAOM-2.2.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/MinimalSimpleCircle-CAOM-2.3.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/MinimalSimplePolygon-CAOM-2.2.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/MinimalSimplePolygon-CAOM-2.3.xml
--rw-r--r--   0 runner    (1001) docker     (121)   235006 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/SampleComposite-CAOM-2.3.xml
--rw-r--r--   0 runner    (1001) docker     (121)   267135 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/SampleDerived-CAOM-2.4.xml
--rw-r--r--   0 runner    (1001) docker     (121)    28640 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/SampleSimple-CAOM-2.3.xml
--rw-r--r--   0 runner    (1001) docker     (121)    12867 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/diff-actual-CAOM-2.3.xml
--rw-r--r--   0 runner    (1001) docker     (121)    10707 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/diff-actual-CAOM-2.4.xml
--rw-r--r--   0 runner    (1001) docker     (121)    12855 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/diff-expected-CAOM-2.3.xml
--rw-r--r--   0 runner    (1001) docker     (121)    12191 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/data/diff-expected-CAOM-2.4.xml
--rw-r--r--   0 runner    (1001) docker     (121)     9040 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/test_artifact.py
--rw-r--r--   0 runner    (1001) docker     (121)    13698 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/test_caom_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    17874 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/test_checksum.py
--rw-r--r--   0 runner    (1001) docker     (121)    15125 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/test_chunk.py
--rw-r--r--   0 runner    (1001) docker     (121)     8991 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (121)    10047 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/test_diffs.py
--rw-r--r--   0 runner    (1001) docker     (121)    55225 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/test_obs_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)    31776 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4823 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/test_part.py
--rw-r--r--   0 runner    (1001) docker     (121)    27769 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/test_plane.py
--rw-r--r--   0 runner    (1001) docker     (121)    13404 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/test_shape.py
--rw-r--r--   0 runner    (1001) docker     (121)    18214 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/test_wcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4858 2022-07-15 22:48:48.000000 caom2-2.5/caom2/tests/xml_compare.py
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-07-15 22:48:56.000000 caom2-2.5/caom2/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    26991 2022-07-15 22:48:48.000000 caom2-2.5/caom2/wcs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 22:48:57.649402 caom2-2.5/caom2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16180 2022-07-15 22:48:57.000000 caom2-2.5/caom2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2304 2022-07-15 22:48:57.000000 caom2-2.5/caom2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-15 22:48:57.000000 caom2-2.5/caom2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-07-15 22:48:57.000000 caom2-2.5/caom2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-15 22:48:57.000000 caom2-2.5/caom2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-07-15 22:48:57.000000 caom2-2.5/caom2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-07-15 22:48:57.000000 caom2-2.5/caom2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 22:48:57.653402 caom2-2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     4581 2022-07-15 22:48:48.000000 caom2-2.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 22:48:57.649402 caom2-2.5/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 22:48:57.653402 caom2-2.5/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-07-15 22:48:48.000000 caom2-2.5/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-07-15 22:48:48.000000 caom2-2.5/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-07-15 22:48:48.000000 caom2-2.5/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6666 2022-07-15 22:48:48.000000 caom2-2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-15 22:48:48.000000 caom2-2.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4513 2022-07-15 22:48:48.000000 caom2-2.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-07-15 22:48:57.657402 caom2-2.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     3445 2022-07-15 22:48:48.000000 caom2-2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 19:41:25.955135 caom2-2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    34520 2022-12-22 19:41:15.000000 caom2-2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-22 19:41:15.000000 caom2-2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2022-12-22 19:41:25.955135 caom2-2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15407 2022-12-22 19:41:15.000000 caom2-2.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 19:41:25.935135 caom2-2.6/caom2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2022-12-22 19:41:15.000000 caom2-2.6/caom2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2022-12-22 19:41:15.000000 caom2-2.6/caom2/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2022-12-22 19:41:15.000000 caom2-2.6/caom2/caom_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19124 2022-12-22 19:41:15.000000 caom2-2.6/caom2/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29212 2022-12-22 19:41:15.000000 caom2-2.6/caom2/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17482 2022-12-22 19:41:15.000000 caom2-2.6/caom2/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 19:41:25.939135 caom2-2.6/caom2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    31423 2022-12-22 19:41:15.000000 caom2-2.6/caom2/data/CAOM-2.2.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    33504 2022-12-22 19:41:15.000000 caom2-2.6/caom2/data/CAOM-2.3.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    36574 2022-12-22 19:41:15.000000 caom2-2.6/caom2/data/CAOM-2.4.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    18335 2022-12-22 19:41:15.000000 caom2-2.6/caom2/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)   123544 2022-12-22 19:41:15.000000 caom2-2.6/caom2/obs_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38040 2022-12-22 19:41:15.000000 caom2-2.6/caom2/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2022-12-22 19:41:15.000000 caom2-2.6/caom2/part.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40062 2022-12-22 19:41:15.000000 caom2-2.6/caom2/plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13385 2022-12-22 19:41:15.000000 caom2-2.6/caom2/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 19:41:25.947135 caom2-2.6/caom2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28079 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/caom_test_instances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 19:41:25.955135 caom2-2.6/caom2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/CompleteCompositeCircle-CAOM-2.2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/CompleteCompositeCircle-CAOM-2.3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/CompleteCompositePolygon-CAOM-2.2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/CompleteCompositePolygon-CAOM-2.3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/CompleteSimpleCircle-CAOM-2.2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/CompleteSimpleCircle-CAOM-2.3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/CompleteSimplePolygon-CAOM-2.2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/CompleteSimplePolygon-CAOM-2.3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/MinimalCompositeCircle-CAOM-2.2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/MinimalCompositeCircle-CAOM-2.3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/MinimalCompositePolygon-CAOM-2.2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/MinimalCompositePolygon-CAOM-2.3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/MinimalSimpleCircle-CAOM-2.2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/MinimalSimpleCircle-CAOM-2.3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/MinimalSimplePolygon-CAOM-2.2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/MinimalSimplePolygon-CAOM-2.3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   235006 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/SampleComposite-CAOM-2.3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   267135 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/SampleDerived-CAOM-2.4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    28640 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/SampleSimple-CAOM-2.3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/diff-actual-CAOM-2.3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    10707 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/diff-actual-CAOM-2.4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    12863 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/diff-expected-CAOM-2.3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/data/diff-expected-CAOM-2.4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/test_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13564 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/test_caom_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17739 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/test_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/test_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9914 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/test_diffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54995 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/test_obs_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31642 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/test_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27635 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/test_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13270 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/test_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18080 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/test_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2022-12-22 19:41:15.000000 caom2-2.6/caom2/tests/xml_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-22 19:41:24.000000 caom2-2.6/caom2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26857 2022-12-22 19:41:15.000000 caom2-2.6/caom2/wcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 19:41:25.935135 caom2-2.6/caom2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2022-12-22 19:41:25.000000 caom2-2.6/caom2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2022-12-22 19:41:25.000000 caom2-2.6/caom2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 19:41:25.000000 caom2-2.6/caom2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-22 19:41:25.000000 caom2-2.6/caom2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 19:41:25.000000 caom2-2.6/caom2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-22 19:41:25.000000 caom2-2.6/caom2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-22 19:41:25.000000 caom2-2.6/caom2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 19:41:25.955135 caom2-2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2022-12-22 19:41:15.000000 caom2-2.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 19:41:25.927135 caom2-2.6/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 19:41:25.955135 caom2-2.6/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2022-12-22 19:41:15.000000 caom2-2.6/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2022-12-22 19:41:15.000000 caom2-2.6/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2022-12-22 19:41:15.000000 caom2-2.6/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2022-12-22 19:41:15.000000 caom2-2.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 19:41:15.000000 caom2-2.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2022-12-22 19:41:15.000000 caom2-2.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2022-12-22 19:41:25.955135 caom2-2.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3360 2022-12-22 19:41:15.000000 caom2-2.6/setup.py
```

### Comparing `caom2-2.5/LICENSE` & `caom2-2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `caom2-2.5/PKG-INFO` & `caom2-2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: caom2
-Version: 2.5
+Version: 2.6
 Summary: CAOM-2.4 library
 Home-page: http://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca/caom2
 Author: Canadian Astronomy Data Centre
 Author-email: cadc@nrc-cnrc.gc.ca
 License: AGPLv3
-Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4
+Requires-Python: >=3.7, <4
 Provides-Extra: test
 License-File: LICENSE
 
 caom2
 =====
 
 .. image:: https://img.shields.io/pypi/v/caom2.svg   
@@ -33,17 +31,14 @@
 http://www.opencadc.org/caom2/
 
 To create a minimal Simple Observation
 --------------------------------------
 
 .. code:: python
 
-        # make it compatible with Python 2 and 3
-        from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
         import sys
         from caom2 import SimpleObservation, TypedOrderedDict, Plane, Artifact,\
                           Part, Chunk, ObservationWriter, ProductType,\
                           ReleaseType, TypedList
 
         observation = SimpleObservation('collection', 'observationID')
 
@@ -414,9 +409,7 @@
 				</caom2:part>
 			  </caom2:parts>
 			</caom2:artifact>
 		  </caom2:artifacts>
 		</caom2:plane>
 	  </caom2:planes>
 	</caom2:Observation>
-
-
```

### Comparing `caom2-2.5/README.rst` & `caom2-2.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 http://www.opencadc.org/caom2/
 
 To create a minimal Simple Observation
 --------------------------------------
 
 .. code:: python
 
-        # make it compatible with Python 2 and 3
-        from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
         import sys
         from caom2 import SimpleObservation, TypedOrderedDict, Plane, Artifact,\
                           Part, Chunk, ObservationWriter, ProductType,\
                           ReleaseType, TypedList
 
         observation = SimpleObservation('collection', 'observationID')
```

### Comparing `caom2-2.5/caom2/__init__.py` & `caom2-2.6/caom2/__init__.py`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/artifact.py` & `caom2-2.6/caom2/artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -67,20 +66,16 @@
 # ***********************************************************************
 #
 
 """Defines the caom2.Artifact class.
 
 """
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
-
 from builtins import str, int
-from six.moves.urllib.parse import urlparse
+from urllib.parse import urlparse
 
 from . import caom_util
 from .chunk import ProductType
 from .common import AbstractCaomEntity
 from .common import ChecksumURI, OrderedEnum
 from .part import Part
 from datetime import datetime
```

### Comparing `caom2-2.5/caom2/caom_util.py` & `caom2-2.6/caom2/caom_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
 #  (c) 2016.                            (c) 2016.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
@@ -72,24 +71,19 @@
 
 This module contains a number of 'TYPED' objects for use in CAOM2.
 These Typed versions were implemented so that content checking near
 the first point of use could be implemented.  This helps the data
 engineer get the correct meta data more quickly.
 """
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import sys
 import collections
 from datetime import datetime
 
-import six
-from six.moves import collections_abc
-from six.moves.urllib.parse import urlsplit
+from urllib.parse import urlsplit
 from builtins import int, str as newstr
 
 
 __all__ = ['TypedList', 'TypedSet', 'TypedOrderedDict', 'ClassProperty',
            'URISet']
 
 # TODO both these are very bad, implement more sensibly
@@ -263,15 +257,15 @@
 
     @property
     def key_type(self):
         """ Returns the type of the elements of this list"""
         return self._oktypes
 
 
-class TypedSet(collections_abc.MutableSet):
+class TypedSet(collections.abc.MutableSet):
     """
     Class that implements a typed set in Python. Supported types
     are specified when instance is created. Example:
 
        obstype = TypedSet((str), "calibration", "science")
        emptyset = TypedSet((str), )
        multipletypes = TypedSet((str, int, int), 1, 12L, "ABC")
@@ -398,20 +392,20 @@
         super(TypedOrderedDict, self).__init__(self)
         self._oktypes = key_type
         for arg in args:
             self.__setitem__(arg[0], arg[1])
 
     def __str__(self):
         return "\n".join(["{} => {}".format(k, v)
-                          for k, v in six.iteritems(self)])
+                          for k, v in self.items()])
 
     def __repr__(self):
         return "TypedOrderedDict((%r))," % self._oktypes + (
             "(".join(
-                ["(%r,%r)" % (k, v) for k, v in six.iteritems(self)]) + ")")
+                ["(%r,%r)" % (k, v) for k, v in self.items()]) + ")")
 
     def check(self, key, value):
         """
         Check that the value is of the correct type for this typed
         dictionary and that the key attribute of value matches the 'key'
         passed to check
         """
```

### Comparing `caom2-2.5/caom2/checksum.py` & `caom2-2.6/caom2/checksum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2017.                            (c) 2017.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -62,16 +61,14 @@
 #  <http://www.gnu.org/licenses/>.      pas le cas, consultez :
 #                                       <http://www.gnu.org/licenses/>.
 #
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
 
 import hashlib
 import logging
 import struct
 import uuid
 from datetime import datetime
 import argparse
```

### Comparing `caom2-2.5/caom2/chunk.py` & `caom2-2.6/caom2/chunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2019.                            (c) 2019.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -67,16 +66,14 @@
 # ***********************************************************************
 #
 
 """Defines caom2.Chunk class.
 
 """
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
 
 from builtins import str
 
 from caom2.caom_util import int_32
 from . import caom_util
 from . import wcs
 from .common import AbstractCaomEntity
@@ -94,17 +91,14 @@
     AUXILIARY: "auxiliary"
     THUMBNAIL: "thumbnail"
     BIAS: "bias"
     DARK: "dark"
     FLAT: "flat"
     WAVECAL: "wavecal"
     """
-    # __order__ required for Python2.7
-    __order__ = "SCIENCE CALIBRATION PREVIEW INFO NOISE WEIGHT AUXILIARY " \
-                "THUMBNAIL BIAS DARK FLAT WAVECAL"
     SCIENCE = "science"
     CALIBRATION = "calibration"
     PREVIEW = "preview"
     INFO = "info"
     NOISE = "noise"
     WEIGHT = "weight"
     AUXILIARY = "auxiliary"
```

### Comparing `caom2-2.5/caom2/common.py` & `caom2-2.6/caom2/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -63,25 +62,21 @@
 #                                       <http://www.gnu.org/licenses/>.
 #
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import inspect
 import uuid
 from datetime import datetime
 
 from builtins import int, str
-from six.moves.urllib.parse import SplitResult, urlparse, urlsplit
+from urllib.parse import SplitResult, urlparse, urlsplit
 import logging
-import six
 
 from . import caom_util
 import warnings
 with warnings.catch_warnings():
     warnings.simplefilter('ignore')
     from aenum import Enum
 
@@ -106,15 +101,15 @@
                     now.second, int(str(now.microsecond)[:-3] + '000'))
 
 
 class OrderedEnum(Enum):
     """
     Enums are in the order of their definition.
 
-    This is here just for Python2.7 and to work with aenum.
+    TODO: not sure this is required in Python 3
     enum.Enum is supposed to support this.
     """
 
     def __init__(self, *args):
         super(Enum, self).__init__()
         self._order = len(self.__class__.__members__) + 1
 
@@ -144,34 +139,28 @@
     setup all objects with the same generic equality, str and repr methods
     """
 
     def __init__(self):
         pass
 
     def __str__(self):
-        if six.PY3:
-            args = inspect.getfullargspec(self.__init__).args[1:]
-        else:
-            args = inspect.getargspec(self.__init__).args[1:]
+        args = inspect.getfullargspec(self.__init__).args[1:]
         class_name = self.__class__.__name__
         return "\n".join(["{}.{} : {}".
                          format(class_name, arg, getattr(self, arg, None))
                           for arg in args])
 
     def __eq__(self, other):
         if type(other) == type(self):
             return self.__dict__ == other.__dict__
         else:
             return False
 
     def __repr__(self):
-        if six.PY3:
-            args = inspect.getfullargspec(self.__init__).args[1:]
-        else:
-            args = inspect.getargspec(self.__init__).args[1:]
+        args = inspect.getfullargspec(self.__init__).args[1:]
         class_name = ""
         if self.__class__.__module__ != '__main__':
             class_name += self.__class__.__module__ + "."
         class_name += self.__class__.__name__
         pading = " " * (len(class_name) + 1)
         return class_name + "(" + (
             ",\n" + pading).join(
```

### Comparing `caom2-2.5/caom2/data/CAOM-2.2.xsd` & `caom2-2.6/caom2/data/CAOM-2.2.xsd`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/data/CAOM-2.3.xsd` & `caom2-2.6/caom2/data/CAOM-2.3.xsd`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/data/CAOM-2.4.xsd` & `caom2-2.6/caom2/data/CAOM-2.4.xsd`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/diff.py` & `caom2-2.6/caom2/diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2018.                            (c) 2018.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -68,17 +67,14 @@
 #
 
 """
 A difference method for CAOM2 entities.
 
 """
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import math
 
 from caom2.common import CaomObject
 from caom2.caom_util import TypedSet, TypedOrderedDict, TypedList
 from caom2 import Chunk
 from . import caom_util
 
@@ -409,15 +405,15 @@
             if math.isnan(rhs) and math.isnan(lhs):
                 result = True  # the opposite of what python will say
             else:
                 result = rhs == lhs
         else:
             # if only using python 3.5+, use math.isclose, instead of this
             # description of math.isclose from the python documentation
-            result = abs(rhs-lhs) <= max(1e-10 * max(abs(rhs), abs(lhs)), 1e-9)
+            result = abs(rhs-lhs) <= max(1e-12 * max(abs(rhs), abs(lhs)), 1e-11)
     else:
         result = rhs == lhs
     return not result
 
 
 def _get_dict(entity):
     """This removes all the entity attributes that are not considered part of
```

### Comparing `caom2-2.5/caom2/obs_reader_writer.py` & `caom2-2.6/caom2/obs_reader_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -66,22 +66,18 @@
 #
 # ***********************************************************************
 #
 
 
 """ Defines ObservationReader class """
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import os
 import uuid
 from builtins import str, int
-import six
-from six.moves.urllib.parse import urlparse
+from urllib.parse import urlparse
 
 from lxml import etree
 
 from . import artifact
 from . import caom_util
 from . import chunk
 from . import observation
@@ -2035,15 +2031,15 @@
 
     def _add_planes_element(self, planes, parent):
         if planes is None or \
                 (len(planes) == 0 and not self._write_empty_collections):
             return
 
         element = self._get_caom_element("planes", parent)
-        for _plane in six.itervalues(planes):
+        for _plane in planes.values():
             plane_element = self._get_caom_element("plane", element)
             self._add_entity_attributes(_plane, plane_element)
             self._add_element("productID", _plane.product_id, plane_element)
             if _plane.creator_id is not None:
                 if self._output_version >= 23:
                     self._add_element("creatorID", _plane.creator_id,
                                       plane_element)
@@ -2293,15 +2289,15 @@
         self._add_element("transition", transition.transition, element)
 
     def _add_artifacts_element(self, artifacts, parent):
         if artifacts is None:
             return
 
         element = self._get_caom_element("artifacts", parent)
-        for _artifact in six.itervalues(artifacts):
+        for _artifact in artifacts.values():
             artifact_element = self._get_caom_element("artifact", element)
             self._add_entity_attributes(_artifact, artifact_element)
             self._add_element("uri", _artifact.uri, artifact_element)
             self._add_element("productType", _artifact.product_type.value,
                               artifact_element)
             self._add_element("releaseType", _artifact.release_type.value,
                               artifact_element)
@@ -2331,15 +2327,15 @@
             self._add_parts_element(_artifact.parts, artifact_element)
 
     def _add_parts_element(self, parts, parent):
         if parts is None:
             return
 
         element = self._get_caom_element("parts", parent)
-        for _part in six.itervalues(parts):
+        for _part in parts.values():
             part_element = self._get_caom_element("part", element)
             self._add_entity_attributes(_part, part_element)
             self._add_element("name", _part.name, part_element)
             if _part.product_type is not None:
                 self._add_element("productType", _part.product_type.value,
                                   part_element)
             self._add_chunks_element(_part.chunks, part_element)
@@ -2676,16 +2672,14 @@
         if value is None:
             return
         element = self._get_caom_element(name, parent)
         if isinstance(value, str):
             element.text = value
         else:
             if isinstance(value, float):
-                # in Python 2.7 str(float) might alter precision of float
-                # therefore call repr instead
                 element.text = repr(value)
             else:
                 element.text = str(value)
 
     def _add_boolean_element(self, name, value, parent):
         if value is None:
             return
```

### Comparing `caom2-2.5/caom2/observation.py` & `caom2-2.6/caom2/observation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -65,32 +64,28 @@
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
 """definition of the  caom2.Observation object."""
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 from datetime import datetime
 
-import six
 from builtins import str
 import warnings
 from deprecated import deprecated
 
 from . import caom_util
 from .caom_util import int_32
 from .common import AbstractCaomEntity, CaomObject, ObservationURI, \
     VocabularyTerm, OrderedEnum
 from .common import _CAOM_VOCAB_NS
 from .plane import Plane
 from .shape import Point
-from six.moves.urllib.parse import urlsplit
+from urllib.parse import urlsplit
 with warnings.catch_warnings():
     warnings.simplefilter('ignore')
     from aenum import Enum
 
 __all__ = ['ObservationIntentType', 'Status', 'TargetType',
            'Observation', 'ObservationURI', 'Algorithm', 'SimpleObservation',
            'DerivedObservation', 'Environment', 'Instrument', 'Proposal',
@@ -99,16 +94,14 @@
 
 
 class ObservationIntentType(OrderedEnum):
     """
     CALIBRATION: "calibration"
     SCIENCE: "science"
     """
-    # __order__ required for Python2.7
-    __order__ = "SCIENCE CALIBRATION"
     SCIENCE = "science"
     CALIBRATION = "calibration"
 
 
 class Status(Enum):
     """
     FAIL: "fail"
@@ -502,15 +495,15 @@
         Initializes an Algorithm instance
 
         Arguments:
         name : name of the algorithm.  Should be 'exposure' if this is a
                simple observation, otherwise name of algorithm that selected
                composite members or just 'composite' works too.
         """
-        caom_util.type_check(name, six.text_type, 'name', override=False)
+        caom_util.type_check(name, str, 'name', override=False)
         self._name = str(name)
 
     def _key(self):
         return self._name
 
     def __ne__(self, y):
         return not self.__eq__(y)
```

### Comparing `caom2-2.5/caom2/part.py` & `caom2-2.6/caom2/part.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -66,17 +65,14 @@
 #
 # ***********************************************************************
 #
 
 """Defines the caom2.Part class which describes
 the caom2_Observation_Plane_Artifact_Part object."""
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 from builtins import str
 
 from . import caom_util
 from .chunk import Chunk
 from .chunk import ProductType
 from .common import AbstractCaomEntity
```

### Comparing `caom2-2.5/caom2/plane.py` & `caom2-2.6/caom2/plane.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -65,32 +64,30 @@
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
 """defines the caom2.Plane class"""
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 from datetime import datetime
 
 from builtins import str, int
-from six.moves.urllib.parse import SplitResult, urlsplit
+from urllib.parse import SplitResult, urlsplit
 from deprecated import deprecated
 
 from caom2.caom_util import int_32
 from . import caom_util
 from . import shape
 from . import wcs
 from .artifact import Artifact
 from .common import AbstractCaomEntity, CaomObject, ObservationURI,\
     VocabularyTerm, OrderedEnum
 from .common import _CAOM_VOCAB_NS, _OBSCORE_VOCAB_NS
 import warnings
+from enum import Enum
 with warnings.catch_warnings():
     warnings.simplefilter('ignore')
     from aenum import Enum, extend_enum
 
 __all__ = ['CalibrationLevel', 'DataProductType', 'EnergyBand',
            'PolarizationState', 'Quality', 'Plane',
            'PlaneURI', 'DataQuality', 'Metrics', 'Provenance', 'Position',
@@ -149,16 +146,14 @@
     INFRARED: "Infrared"
     OPTICAL: "Optical"
     UV: "UV"
     EUV: "EUV"
     XRAY: "X-ray"
     GAMMARAY: "Gamma-ray"
     """
-    # __order__ required for Python2.7
-    __order__ = "RADIO MILLIMETER INFRARED OPTICAL UV EUV XRAY GAMMARAY"
     RADIO = "Radio"
     MILLIMETER = "Millimeter"
     INFRARED = "Infrared"
     OPTICAL = "Optical"
     UV = "UV"
     EUV = "EUV"
     XRAY = "X-ray"
@@ -182,17 +177,14 @@
     RL: "RL"
     LR: "LR"
     XX: "XX"
     YY: "YY"
     XY: "XY"
     YX: "YX"
     """
-    # __order__ required for Python2.7
-    __order__ = "I Q U V RR LL RL LR XX YY XY YX POLI FPOLI POLA EPOLI " \
-                "CPOLI NPOLI"
     I = "I"  # noqa
     Q = "Q"
     U = "U"
     V = "V"
     RR = "RR"
     LL = "LL"
     RL = "RL"
```

### Comparing `caom2-2.5/caom2/shape.py` & `caom2-2.6/caom2/shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -63,17 +62,14 @@
 #                                       <http://www.gnu.org/licenses/>.
 #
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import math
 from caom2.caom_util import int_32
 from . import caom_util
 from . import common
 import warnings
 with warnings.catch_warnings():
     warnings.simplefilter('ignore')
```

### Comparing `caom2-2.5/caom2/tests/caom_test_instances.py` & `caom2-2.6/caom2/tests/caom_test_instances.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -65,21 +64,17 @@
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
 """ Defines Caom2TestInstances class """
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import collections
 from datetime import datetime
 import uuid
-import six
 from builtins import int
 
 from caom2 import artifact
 from caom2 import caom_util
 from caom2 import chunk
 from caom2 import common
 from caom2 import observation
@@ -357,15 +352,15 @@
                     _plane.custom_axis = self.get_custom()
                     _plane.meta_read_groups.add('ivo://cadc.nrc.ca/groups?A')
                     _plane.meta_read_groups.add('ivo://cadc.nrc.ca/groups?D')
                     _plane.data_read_groups.add('ivo://cadc.nrc.ca/groups?B')
                     _plane.data_read_groups.add('ivo://cadc.nrc.ca/groups?C')
 
             if self.depth > 2:
-                for k, v in six.iteritems(self.get_artifacts()):
+                for k, v in self.get_artifacts().items():
                     _plane.artifacts[k] = v
             planes[prod_id] = _plane
         return planes
 
     def get_poly_position(self):
         position = plane.Position()
 
@@ -518,15 +513,15 @@
             if self.caom_version >= 23:
                 _artifact.max_last_modified = common.get_current_ivoa_time()
                 _artifact.meta_checksum = common.ChecksumURI(
                     "md5:9882dbbf9cadc221019b712fd402bcbd")
                 _artifact.acc_meta_checksum = common.ChecksumURI(
                     "md5:844ce247db0844ad9f721430c80e7a21")
         if self.depth > 3:
-            for k, v in six.iteritems(self.get_parts()):
+            for k, v in self.get_parts().items():
                 _artifact.parts[k] = v
         artifacts["ad:foo/bar1"] = _artifact
         if self.caom_version >= 24:
             _artifact.content_release = \
                 caom_util.str2ivoa("2050-01-11T00:00:00.000")
             _artifact.content_read_groups.add("ivo://cadc.nrc.ca/gms?B")
             _artifact.content_read_groups.add("ivo://cadc.nrc.ca/gms?A")
```

### Comparing `caom2-2.5/caom2/tests/data/CompleteCompositeCircle-CAOM-2.2.xml` & `caom2-2.6/caom2/tests/data/CompleteCompositeCircle-CAOM-2.2.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/CompleteCompositeCircle-CAOM-2.3.xml` & `caom2-2.6/caom2/tests/data/CompleteCompositeCircle-CAOM-2.3.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/CompleteCompositePolygon-CAOM-2.2.xml` & `caom2-2.6/caom2/tests/data/CompleteCompositePolygon-CAOM-2.2.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/CompleteCompositePolygon-CAOM-2.3.xml` & `caom2-2.6/caom2/tests/data/CompleteCompositePolygon-CAOM-2.3.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/CompleteSimpleCircle-CAOM-2.2.xml` & `caom2-2.6/caom2/tests/data/CompleteSimpleCircle-CAOM-2.2.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/CompleteSimpleCircle-CAOM-2.3.xml` & `caom2-2.6/caom2/tests/data/CompleteSimpleCircle-CAOM-2.3.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/CompleteSimplePolygon-CAOM-2.2.xml` & `caom2-2.6/caom2/tests/data/CompleteSimplePolygon-CAOM-2.2.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/CompleteSimplePolygon-CAOM-2.3.xml` & `caom2-2.6/caom2/tests/data/CompleteSimplePolygon-CAOM-2.3.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/MinimalCompositeCircle-CAOM-2.2.xml` & `caom2-2.6/caom2/tests/data/MinimalCompositeCircle-CAOM-2.2.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/MinimalCompositeCircle-CAOM-2.3.xml` & `caom2-2.6/caom2/tests/data/MinimalCompositeCircle-CAOM-2.3.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/MinimalCompositePolygon-CAOM-2.2.xml` & `caom2-2.6/caom2/tests/data/MinimalCompositePolygon-CAOM-2.2.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/MinimalCompositePolygon-CAOM-2.3.xml` & `caom2-2.6/caom2/tests/data/MinimalCompositePolygon-CAOM-2.3.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/MinimalSimpleCircle-CAOM-2.2.xml` & `caom2-2.6/caom2/tests/data/MinimalSimpleCircle-CAOM-2.2.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/MinimalSimpleCircle-CAOM-2.3.xml` & `caom2-2.6/caom2/tests/data/MinimalSimpleCircle-CAOM-2.3.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/MinimalSimplePolygon-CAOM-2.2.xml` & `caom2-2.6/caom2/tests/data/MinimalSimplePolygon-CAOM-2.2.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/MinimalSimplePolygon-CAOM-2.3.xml` & `caom2-2.6/caom2/tests/data/MinimalSimplePolygon-CAOM-2.3.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/SampleComposite-CAOM-2.3.xml` & `caom2-2.6/caom2/tests/data/SampleComposite-CAOM-2.3.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/SampleDerived-CAOM-2.4.xml` & `caom2-2.6/caom2/tests/data/SampleDerived-CAOM-2.4.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/SampleSimple-CAOM-2.3.xml` & `caom2-2.6/caom2/tests/data/SampleSimple-CAOM-2.3.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/diff-actual-CAOM-2.3.xml` & `caom2-2.6/caom2/tests/data/diff-actual-CAOM-2.3.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/diff-actual-CAOM-2.4.xml` & `caom2-2.6/caom2/tests/data/diff-actual-CAOM-2.4.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/data/diff-expected-CAOM-2.3.xml` & `caom2-2.6/caom2/tests/data/diff-expected-CAOM-2.3.xml`

 * *Files 0% similar despite different names*

#### Comparing `caom2-2.5/caom2/tests/data/diff-expected-CAOM-2.3.xml` & `caom2-2.6/caom2/tests/data/diff-expected-CAOM-2.3.xml`

```diff
@@ -115,19 +115,19 @@
         <caom2:sampleSize>1.3000000000000003e-07</caom2:sampleSize>
         <caom2:bandpassName>SDSS r prime</caom2:bandpassName>
         <caom2:emBand>Optical</caom2:emBand>
       </caom2:energy>
       <caom2:time>
         <caom2:bounds>
           <caom2:lower>58979.5015625</caom2:lower>
-          <caom2:upper>58979.5017365</caom2:upper>
+          <caom2:upper>58979.50173611111</caom2:upper>
           <caom2:samples>
             <caom2:sample>
               <caom2:lower>58979.5015625</caom2:lower>
-              <caom2:upper>58979.5017365</caom2:upper>
+              <caom2:upper>58979.50173611111</caom2:upper>
             </caom2:sample>
           </caom2:samples>
         </caom2:bounds>
         <caom2:dimension>1</caom2:dimension>
         <caom2:resolution>15.0</caom2:resolution>
         <caom2:sampleSize>0.00017361110803904012</caom2:sampleSize>
         <caom2:exposure>15.0</caom2:exposure>
```

### Comparing `caom2-2.5/caom2/tests/data/diff-expected-CAOM-2.4.xml` & `caom2-2.6/caom2/tests/data/diff-expected-CAOM-2.4.xml`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/tests/test_artifact.py` & `caom2-2.6/caom2/tests/test_artifact.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -65,20 +64,17 @@
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
 """ Defines TestArtifact class """
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import unittest
 
-from six.moves.urllib.parse import urlparse
+from urllib.parse import urlparse
 
 from .. import artifact
 from .. import common
 from .. import part
 
 
 class TestEnums(unittest.TestCase):
```

### Comparing `caom2-2.5/caom2/tests/test_caom_util.py` & `caom2-2.6/caom2/tests/test_caom_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -63,17 +62,14 @@
 #                                       <http://www.gnu.org/licenses/>.
 #
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import unittest
 import pytest
 
 from builtins import str, int
 
 from .. import artifact
 from .. import caom_util
```

### Comparing `caom2-2.5/caom2/tests/test_checksum.py` & `caom2-2.6/caom2/tests/test_checksum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -65,32 +64,29 @@
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
 """ Defines TestPlane class """
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import hashlib
 import os
 import sys
 from uuid import UUID
 import logging
 
 from builtins import int, str
 
 from caom2 import obs_reader_writer, get_meta_checksum, get_acc_meta_checksum
 from caom2 import update_meta_checksum
 from caom2.caom_util import str2ivoa
 from caom2.checksum import update_checksum, int_32, checksum_diff
 import tempfile
 from mock import patch
-from six import StringIO
+from io import StringIO
 
 THIS_DIR = os.path.dirname(os.path.realpath(__file__))
 TEST_DATA = 'data'
 
 
 def test_primitive_checksum():
     md5 = hashlib.md5()
```

### Comparing `caom2-2.5/caom2/tests/test_chunk.py` & `caom2-2.6/caom2/tests/test_chunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2019.                            (c) 2019.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -65,17 +64,14 @@
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
 """ Defines TestChunk class """
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import unittest
 
 from .. import chunk
 from .. import wcs
 
 
 class TestEnums(unittest.TestCase):
```

### Comparing `caom2-2.5/caom2/tests/test_common.py` & `caom2-2.6/caom2/tests/test_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -65,17 +64,14 @@
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
 """ Defines TestCaom2IdGenerator class """
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import binascii
 import unittest
 
 from .. import artifact
 from .. import chunk
 from .. import common
 from .. import observation
```

### Comparing `caom2-2.5/caom2/tests/test_diffs.py` & `caom2-2.6/caom2/tests/test_diffs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2018.                            (c) 2018.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -62,16 +61,14 @@
 #  <http://www.gnu.org/licenses/>.      pas le cas, consultez :
 #                                       <http://www.gnu.org/licenses/>.
 #
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
 
 import os
 import unittest
 
 from caom2 import Point, shape, Vertex, SegmentType, Position
 
 from .. import diff
```

### Comparing `caom2-2.5/caom2/tests/test_obs_reader_writer.py` & `caom2-2.6/caom2/tests/test_obs_reader_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -65,22 +64,19 @@
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
 """ Defines TestObservationReaderWriter class """
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import os
 import unittest
 
 from lxml import etree
-from six import BytesIO
+from io import BytesIO
 import tempfile
 
 from . import caom_test_instances
 from .xml_compare import xml_compare
 from .. import obs_reader_writer
 from .. import observation
 from .. import plane
@@ -1193,18 +1189,14 @@
         valid_observation = self._create_observation()
         xml = self._write_observation(valid_observation)
         if intent_type is not None:
             xml = xml.replace(b'science', intent_type)
         reader = obs_reader_writer.ObservationReader(True)
         reader.read(BytesIO(xml))
 
-    def runTest(self):
-        # method required to make tests run on Python 2.7
-        pass
-
     def test_schema_validator(self):
         """
         This function is to catch unsupported extensions to our schema.
         This function validates the schema by performing two simple observation
         read-write round trips. One round trip uses a valid observation while
         another uses an observation with an invalid value. The former should
         pass while the latter should fail.
```

### Comparing `caom2-2.5/caom2/tests/test_observation.py` & `caom2-2.6/caom2/tests/test_observation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -65,17 +64,14 @@
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
 """ Defines TestObservation class """
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import unittest
 from datetime import datetime
 from builtins import str
 
 from .. import caom_util
 from .. import observation
 from .. import plane
```

### Comparing `caom2-2.5/caom2/tests/test_part.py` & `caom2-2.6/caom2/tests/test_part.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -65,17 +64,14 @@
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
 """ Defines TestPart class """
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import unittest
 
 from .. import chunk
 from .. import part
 
 
 class TestPart(unittest.TestCase):
```

### Comparing `caom2-2.5/caom2/tests/test_plane.py` & `caom2-2.6/caom2/tests/test_plane.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -65,17 +64,14 @@
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
 """ Defines TestPlane class """
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import unittest
 from datetime import datetime
 
 from .. import artifact
 from .. import chunk
 from .. import observation
 from .. import plane
```

### Comparing `caom2-2.5/caom2/tests/test_shape.py` & `caom2-2.6/caom2/tests/test_shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -63,17 +62,14 @@
 #                                       <http://www.gnu.org/licenses/>.
 #
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import math
 import pytest
 import unittest
 
 from .. import shape
```

### Comparing `caom2-2.5/caom2/tests/test_wcs.py` & `caom2-2.6/caom2/tests/test_wcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -63,17 +62,14 @@
 #                                       <http://www.gnu.org/licenses/>.
 #
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import unittest
 
 from builtins import int
 
 from .. import wcs
```

### Comparing `caom2-2.5/caom2/tests/xml_compare.py` & `caom2-2.6/caom2/tests/xml_compare.py`

 * *Files identical despite different names*

### Comparing `caom2-2.5/caom2/wcs.py` & `caom2-2.6/caom2/wcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2016.                            (c) 2016.
+#  (c) 2022.                            (c) 2022.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -63,17 +62,14 @@
 #                                       <http://www.gnu.org/licenses/>.
 #
 #  $Revision: 4 $
 #
 # ***********************************************************************
 #
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 from builtins import str, int
 
 from . import caom_util
 from . import common
 
 __all__ = ['Axis', 'Coord2D', 'CoordAxis1D', 'CoordAxis2D', 'CoordBounds1D',
            'CoordBounds2D', 'CoordCircle2D', 'CoordError', 'CoordFunction1D',
```

### Comparing `caom2-2.5/caom2.egg-info/PKG-INFO` & `caom2-2.6/caom2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: caom2
-Version: 2.5
+Version: 2.6
 Summary: CAOM-2.4 library
 Home-page: http://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca/caom2
 Author: Canadian Astronomy Data Centre
 Author-email: cadc@nrc-cnrc.gc.ca
 License: AGPLv3
-Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4
+Requires-Python: >=3.7, <4
 Provides-Extra: test
 License-File: LICENSE
 
 caom2
 =====
 
 .. image:: https://img.shields.io/pypi/v/caom2.svg   
@@ -33,17 +31,14 @@
 http://www.opencadc.org/caom2/
 
 To create a minimal Simple Observation
 --------------------------------------
 
 .. code:: python
 
-        # make it compatible with Python 2 and 3
-        from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
         import sys
         from caom2 import SimpleObservation, TypedOrderedDict, Plane, Artifact,\
                           Part, Chunk, ObservationWriter, ProductType,\
                           ReleaseType, TypedList
 
         observation = SimpleObservation('collection', 'observationID')
 
@@ -414,9 +409,7 @@
 				</caom2:part>
 			  </caom2:parts>
 			</caom2:artifact>
 		  </caom2:artifacts>
 		</caom2:plane>
 	  </caom2:planes>
 	</caom2:Observation>
-
-
```

### Comparing `caom2-2.5/caom2.egg-info/SOURCES.txt` & `caom2-2.6/caom2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caom2-2.5/docs/Makefile` & `caom2-2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caom2-2.5/docs/conf.py` & `caom2-2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `caom2-2.5/docs/make.bat` & `caom2-2.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `caom2-2.5/setup.cfg` & `caom2-2.6/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -31,32 +31,29 @@
 long_description = Python library for the CAOM-2.4 data model
 author = Canadian Astronomy Data Centre
 author_email = cadc@nrc-cnrc.gc.ca
 license = AGPLv3
 url = http://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca/caom2
 edit_on_github = False
 github_project = opencadc/caom2tools
-version = 2.5
+version = 2.6
 
 [options]
 install_requires = 
-	future
 	aenum
-	six
 	deprecated
-	lxml<=4.3.0;python_version=="3.4"
-	lxml>=3.7.0;python_version>="3.5"
+	lxml>=3.7.0
 
 [options.extras_require]
 test = 
 	pytest>=4.6
 	pytest-cov>=2.5.1
 	flake8>=3.4.1
-	funcsigs==1.0.2
-	mock==2.0.0
+	funcsigs>=1.0.2
+	mock>=2.0.0
 
 [entry_points]
 caom2-checksum = caom2.checksum:checksum_diff
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `caom2-2.5/setup.py` & `caom2-2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,21 +86,20 @@
       license=LICENSE,
       url=URL,
       long_description=readme(),
       zip_safe=False,
       use_2to3=False,
       setup_requires=['pytest-runner'],
       entry_points=entry_points,
-      python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4',
+      python_requires='>=3.7, <4',
       packages=find_packages(),
       package_data={PACKAGENAME: ['data/*', 'tests/data/*', '*/data/*', '*/tests/data/*']},
       classifiers=[
         'Natural Language :: English',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
       ],
       cmdclass = {
           'coverage': PyTest,
       }
 )
```

