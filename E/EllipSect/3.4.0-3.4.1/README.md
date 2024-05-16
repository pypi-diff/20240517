# Comparing `tmp/EllipSect-3.4.0.tar.gz` & `tmp/ellipsect-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EllipSect-3.4.0.tar", last modified: Sat Apr 13 01:31:39 2024, max compression
+gzip compressed data, was "ellipsect-3.4.1.tar", last modified: Thu May 16 23:41:50 2024, max compression
```

## Comparing `EllipSect-3.4.0.tar` & `ellipsect-3.4.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.437674 EllipSect-3.4.0/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      206 2022-05-19 20:23:00.000000 EllipSect-3.4.0/AUTHORS.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1126 2022-08-31 20:39:25.000000 EllipSect-3.4.0/CHANGELOG.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    13841 2022-05-19 05:38:00.000000 EllipSect-3.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    35147 2020-07-24 13:17:31.000000 EllipSect-3.4.0/LICENSE.txt
--rw-r--r--   0 canorve   (1000) canorve   (1000)     7164 2024-04-13 01:31:39.437674 EllipSect-3.4.0/PKG-INFO
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     5874 2023-08-08 07:01:01.000000 EllipSect-3.4.0/README.rst
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.421674 EllipSect-3.4.0/docs/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1154 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/Makefile
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.421674 EllipSect-3.4.0/docs/_static/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       18 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/_static/.gitignore
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     7461 2022-06-03 20:18:01.000000 EllipSect-3.4.0/docs/api.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       41 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/authors.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       43 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/changelog.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     9758 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/conf.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       33 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/contributing.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    18141 2024-04-11 23:03:41.000000 EllipSect-3.4.0/docs/howto.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2321 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/index.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       67 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/license.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       39 2022-05-19 05:38:00.000000 EllipSect-3.4.0/docs/readme.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      307 2022-05-27 21:03:59.000000 EllipSect-3.4.0/docs/requirements.txt
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.421674 EllipSect-3.4.0/example/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      341 2020-09-18 22:51:02.000000 EllipSect-3.4.0/example/README
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    69120 2020-08-14 03:16:26.000000 EllipSect-3.4.0/example/gal.fits
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2646 2020-08-14 03:16:26.000000 EllipSect-3.4.0/example/galfit.feedme
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    25920 2020-08-14 03:16:26.000000 EllipSect-3.4.0/example/psf.fits
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.429674 EllipSect-3.4.0/img/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   251092 2021-05-21 15:14:44.000000 EllipSect-3.4.0/img/A2029.ring.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   149798 2021-10-21 21:59:56.000000 EllipSect-3.4.0/img/A85.comp.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   573061 2022-03-30 17:48:47.000000 EllipSect-3.4.0/img/A85.con-cub.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   670362 2022-03-30 17:49:48.000000 EllipSect-3.4.0/img/A85.cub.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    98164 2021-10-21 22:00:51.000000 EllipSect-3.4.0/img/A85.def.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   610346 2022-03-30 17:44:31.000000 EllipSect-3.4.0/img/A85.ell-cub.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   503397 2021-10-21 22:01:09.000000 EllipSect-3.4.0/img/A85.grid.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    95479 2021-10-21 22:01:39.000000 EllipSect-3.4.0/img/A85.log.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   102981 2021-10-21 22:02:04.000000 EllipSect-3.4.0/img/A85.pix.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   327227 2020-08-14 03:16:26.000000 EllipSect-3.4.0/img/A85.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    95328 2021-10-21 22:02:35.000000 EllipSect-3.4.0/img/A85.ranx1.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    89311 2021-10-21 22:03:30.000000 EllipSect-3.4.0/img/A85.ranx2.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    91257 2021-10-21 22:04:08.000000 EllipSect-3.4.0/img/A85.rany1.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      355 2022-05-19 05:38:00.000000 EllipSect-3.4.0/pyproject.toml
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1760 2024-04-13 01:31:39.441674 EllipSect-3.4.0/setup.cfg
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      706 2022-05-19 05:38:00.000000 EllipSect-3.4.0/setup.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.417674 EllipSect-3.4.0/src/
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.437674 EllipSect-3.4.0/src/EllipSect.egg-info/
--rw-r--r--   0 canorve   (1000) canorve   (1000)     7164 2024-04-13 01:31:39.000000 EllipSect-3.4.0/src/EllipSect.egg-info/PKG-INFO
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1610 2024-04-13 01:31:39.000000 EllipSect-3.4.0/src/EllipSect.egg-info/SOURCES.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        1 2024-04-13 01:31:39.000000 EllipSect-3.4.0/src/EllipSect.egg-info/dependency_links.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       57 2024-04-13 01:31:39.000000 EllipSect-3.4.0/src/EllipSect.egg-info/entry_points.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        1 2022-05-23 00:05:26.000000 EllipSect-3.4.0/src/EllipSect.egg-info/not-zip-safe
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      146 2024-04-13 01:31:39.000000 EllipSect-3.4.0/src/EllipSect.egg-info/requires.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       10 2024-04-13 01:31:39.000000 EllipSect-3.4.0/src/EllipSect.egg-info/top_level.txt
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.433674 EllipSect-3.4.0/src/ellipsect/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      675 2022-05-29 17:51:45.000000 EllipSect-3.4.0/src/ellipsect/__init__.py
--rwxrwxr-x   0 canorve   (1000) canorve   (1000)     2080 2024-02-09 20:55:40.000000 EllipSect-3.4.0/src/ellipsect/ellipsectors.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.433674 EllipSect-3.4.0/src/ellipsect/inout/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:15:19.000000 EllipSect-3.4.0/src/ellipsect/inout/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    22988 2023-11-15 21:56:50.000000 EllipSect-3.4.0/src/ellipsect/inout/galfit.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     3380 2023-02-10 20:37:56.000000 EllipSect-3.4.0/src/ellipsect/inout/gfits.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    25023 2024-04-11 22:10:54.000000 EllipSect-3.4.0/src/ellipsect/inout/plots.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    20165 2023-06-10 20:46:21.000000 EllipSect-3.4.0/src/ellipsect/inout/prt.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    21218 2024-04-11 22:20:26.000000 EllipSect-3.4.0/src/ellipsect/inout/read.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.433674 EllipSect-3.4.0/src/ellipsect/lib/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 06:03:15.000000 EllipSect-3.4.0/src/ellipsect/lib/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     8144 2024-04-11 21:55:45.000000 EllipSect-3.4.0/src/ellipsect/lib/clas.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1506 2023-07-02 05:45:35.000000 EllipSect-3.4.0/src/ellipsect/lib/libs.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.433674 EllipSect-3.4.0/src/ellipsect/phot/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:10:40.000000 EllipSect-3.4.0/src/ellipsect/phot/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     5878 2023-10-24 22:42:37.000000 EllipSect-3.4.0/src/ellipsect/phot/ned.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    15252 2023-03-14 00:35:39.000000 EllipSect-3.4.0/src/ellipsect/phot/phot.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    12315 2023-10-27 21:26:58.000000 EllipSect-3.4.0/src/ellipsect/phot/tidal.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.433674 EllipSect-3.4.0/src/ellipsect/sectors/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:15:40.000000 EllipSect-3.4.0/src/ellipsect/sectors/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     3065 2023-02-09 23:00:21.000000 EllipSect-3.4.0/src/ellipsect/sectors/comp.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     6814 2023-02-09 23:00:25.000000 EllipSect-3.4.0/src/ellipsect/sectors/ellip.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2981 2023-02-09 23:00:28.000000 EllipSect-3.4.0/src/ellipsect/sectors/num.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    20510 2024-04-11 22:00:26.000000 EllipSect-3.4.0/src/ellipsect/sectors/sect.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.437674 EllipSect-3.4.0/src/ellipsect/sky/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 07:02:06.000000 EllipSect-3.4.0/src/ellipsect/sky/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    24185 2023-02-09 23:00:47.000000 EllipSect-3.4.0/src/ellipsect/sky/sky.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-04-13 01:31:39.437674 EllipSect-3.4.0/tests/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      277 2022-05-19 05:38:00.000000 EllipSect-3.4.0/tests/conftest.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    69120 2020-08-14 03:16:26.000000 EllipSect-3.4.0/tests/gal.fits
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2879 2022-05-27 20:24:55.000000 EllipSect-3.4.0/tests/galfit.01
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   192960 2024-04-13 01:28:00.000000 EllipSect-3.4.0/tests/imgblock.fits
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    25920 2020-08-14 03:16:26.000000 EllipSect-3.4.0/tests/psf.fits
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    15557 2024-04-12 06:43:05.000000 EllipSect-3.4.0/tests/test_ellipsect.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2575 2022-05-19 05:38:00.000000 EllipSect-3.4.0/tox.ini
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-16 23:41:50.946574 ellipsect-3.4.1/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      206 2022-05-19 20:23:00.000000 ellipsect-3.4.1/AUTHORS.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1126 2022-08-31 20:39:25.000000 ellipsect-3.4.1/CHANGELOG.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    13841 2022-05-19 05:38:00.000000 ellipsect-3.4.1/CONTRIBUTING.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    35147 2020-07-24 13:17:31.000000 ellipsect-3.4.1/LICENSE.txt
+-rw-r--r--   0 canorve   (1000) canorve   (1000)     7164 2024-05-16 23:41:50.946574 ellipsect-3.4.1/PKG-INFO
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     5874 2023-08-08 07:01:01.000000 ellipsect-3.4.1/README.rst
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-16 23:41:50.926574 ellipsect-3.4.1/docs/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1154 2022-05-19 05:38:00.000000 ellipsect-3.4.1/docs/Makefile
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-16 23:41:50.926574 ellipsect-3.4.1/docs/_static/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       18 2022-05-19 05:38:00.000000 ellipsect-3.4.1/docs/_static/.gitignore
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     7461 2022-06-03 20:18:01.000000 ellipsect-3.4.1/docs/api.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       41 2022-05-19 05:38:00.000000 ellipsect-3.4.1/docs/authors.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       43 2022-05-19 05:38:00.000000 ellipsect-3.4.1/docs/changelog.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     9758 2022-05-19 05:38:00.000000 ellipsect-3.4.1/docs/conf.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       33 2022-05-19 05:38:00.000000 ellipsect-3.4.1/docs/contributing.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    18141 2024-04-11 23:03:41.000000 ellipsect-3.4.1/docs/howto.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2321 2022-05-19 05:38:00.000000 ellipsect-3.4.1/docs/index.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       67 2022-05-19 05:38:00.000000 ellipsect-3.4.1/docs/license.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       39 2022-05-19 05:38:00.000000 ellipsect-3.4.1/docs/readme.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      307 2022-05-27 21:03:59.000000 ellipsect-3.4.1/docs/requirements.txt
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-16 23:41:50.930574 ellipsect-3.4.1/example/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      341 2020-09-18 22:51:02.000000 ellipsect-3.4.1/example/README
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    69120 2020-08-14 03:16:26.000000 ellipsect-3.4.1/example/gal.fits
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2646 2020-08-14 03:16:26.000000 ellipsect-3.4.1/example/galfit.feedme
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    25920 2020-08-14 03:16:26.000000 ellipsect-3.4.1/example/psf.fits
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-16 23:41:50.934574 ellipsect-3.4.1/img/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   251092 2021-05-21 15:14:44.000000 ellipsect-3.4.1/img/A2029.ring.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   149798 2021-10-21 21:59:56.000000 ellipsect-3.4.1/img/A85.comp.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   573061 2022-03-30 17:48:47.000000 ellipsect-3.4.1/img/A85.con-cub.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   670362 2022-03-30 17:49:48.000000 ellipsect-3.4.1/img/A85.cub.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    98164 2021-10-21 22:00:51.000000 ellipsect-3.4.1/img/A85.def.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   610346 2022-03-30 17:44:31.000000 ellipsect-3.4.1/img/A85.ell-cub.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   503397 2021-10-21 22:01:09.000000 ellipsect-3.4.1/img/A85.grid.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    95479 2021-10-21 22:01:39.000000 ellipsect-3.4.1/img/A85.log.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   102981 2021-10-21 22:02:04.000000 ellipsect-3.4.1/img/A85.pix.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   327227 2020-08-14 03:16:26.000000 ellipsect-3.4.1/img/A85.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    95328 2021-10-21 22:02:35.000000 ellipsect-3.4.1/img/A85.ranx1.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    89311 2021-10-21 22:03:30.000000 ellipsect-3.4.1/img/A85.ranx2.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    91257 2021-10-21 22:04:08.000000 ellipsect-3.4.1/img/A85.rany1.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      355 2022-05-19 05:38:00.000000 ellipsect-3.4.1/pyproject.toml
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1760 2024-05-16 23:41:50.946574 ellipsect-3.4.1/setup.cfg
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      706 2022-05-19 05:38:00.000000 ellipsect-3.4.1/setup.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-16 23:41:50.918574 ellipsect-3.4.1/src/
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-16 23:41:50.946574 ellipsect-3.4.1/src/EllipSect.egg-info/
+-rw-r--r--   0 canorve   (1000) canorve   (1000)     7164 2024-05-16 23:41:50.000000 ellipsect-3.4.1/src/EllipSect.egg-info/PKG-INFO
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1610 2024-05-16 23:41:50.000000 ellipsect-3.4.1/src/EllipSect.egg-info/SOURCES.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        1 2024-05-16 23:41:50.000000 ellipsect-3.4.1/src/EllipSect.egg-info/dependency_links.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       57 2024-05-16 23:41:50.000000 ellipsect-3.4.1/src/EllipSect.egg-info/entry_points.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        1 2022-05-23 00:05:26.000000 ellipsect-3.4.1/src/EllipSect.egg-info/not-zip-safe
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      146 2024-05-16 23:41:50.000000 ellipsect-3.4.1/src/EllipSect.egg-info/requires.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       10 2024-05-16 23:41:50.000000 ellipsect-3.4.1/src/EllipSect.egg-info/top_level.txt
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-16 23:41:50.938574 ellipsect-3.4.1/src/ellipsect/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      675 2022-05-29 17:51:45.000000 ellipsect-3.4.1/src/ellipsect/__init__.py
+-rwxrwxr-x   0 canorve   (1000) canorve   (1000)     2080 2024-02-09 20:55:40.000000 ellipsect-3.4.1/src/ellipsect/ellipsectors.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-16 23:41:50.938574 ellipsect-3.4.1/src/ellipsect/inout/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:15:19.000000 ellipsect-3.4.1/src/ellipsect/inout/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    22988 2023-11-15 21:56:50.000000 ellipsect-3.4.1/src/ellipsect/inout/galfit.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     3380 2023-02-10 20:37:56.000000 ellipsect-3.4.1/src/ellipsect/inout/gfits.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    25023 2024-04-11 22:10:54.000000 ellipsect-3.4.1/src/ellipsect/inout/plots.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    20165 2023-06-10 20:46:21.000000 ellipsect-3.4.1/src/ellipsect/inout/prt.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    21218 2024-04-11 22:20:26.000000 ellipsect-3.4.1/src/ellipsect/inout/read.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-16 23:41:50.942574 ellipsect-3.4.1/src/ellipsect/lib/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 06:03:15.000000 ellipsect-3.4.1/src/ellipsect/lib/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     8144 2024-04-11 21:55:45.000000 ellipsect-3.4.1/src/ellipsect/lib/clas.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1506 2023-07-02 05:45:35.000000 ellipsect-3.4.1/src/ellipsect/lib/libs.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-16 23:41:50.942574 ellipsect-3.4.1/src/ellipsect/phot/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:10:40.000000 ellipsect-3.4.1/src/ellipsect/phot/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     5878 2023-10-24 22:42:37.000000 ellipsect-3.4.1/src/ellipsect/phot/ned.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    15252 2023-03-14 00:35:39.000000 ellipsect-3.4.1/src/ellipsect/phot/phot.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    12315 2023-10-27 21:26:58.000000 ellipsect-3.4.1/src/ellipsect/phot/tidal.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-16 23:41:50.942574 ellipsect-3.4.1/src/ellipsect/sectors/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 02:15:40.000000 ellipsect-3.4.1/src/ellipsect/sectors/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     3065 2023-02-09 23:00:21.000000 ellipsect-3.4.1/src/ellipsect/sectors/comp.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     6814 2023-02-09 23:00:25.000000 ellipsect-3.4.1/src/ellipsect/sectors/ellip.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2981 2023-02-09 23:00:28.000000 ellipsect-3.4.1/src/ellipsect/sectors/num.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    20510 2024-04-11 22:00:26.000000 ellipsect-3.4.1/src/ellipsect/sectors/sect.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-16 23:41:50.942574 ellipsect-3.4.1/src/ellipsect/sky/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2021-08-21 07:02:06.000000 ellipsect-3.4.1/src/ellipsect/sky/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    24277 2024-05-16 23:05:36.000000 ellipsect-3.4.1/src/ellipsect/sky/sky.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-16 23:41:50.946574 ellipsect-3.4.1/tests/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      277 2022-05-19 05:38:00.000000 ellipsect-3.4.1/tests/conftest.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    69120 2020-08-14 03:16:26.000000 ellipsect-3.4.1/tests/gal.fits
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2879 2022-05-27 20:24:55.000000 ellipsect-3.4.1/tests/galfit.01
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   192960 2024-05-16 23:37:51.000000 ellipsect-3.4.1/tests/imgblock.fits
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    25920 2020-08-14 03:16:26.000000 ellipsect-3.4.1/tests/psf.fits
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    15557 2024-04-12 06:43:05.000000 ellipsect-3.4.1/tests/test_ellipsect.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2575 2024-04-13 13:45:38.000000 ellipsect-3.4.1/tox.ini
```

### Comparing `EllipSect-3.4.0/CHANGELOG.rst` & `ellipsect-3.4.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/CONTRIBUTING.rst` & `ellipsect-3.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/LICENSE.txt` & `ellipsect-3.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/PKG-INFO` & `ellipsect-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EllipSect
-Version: 3.4.0
+Version: 3.4.1
 Summary: A surface brightness analysis tool for GALFIT output.
 Home-page: https://github.com/canorve/EllipSect
 Author: Christopher Añorve
 Author-email: canorve@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Documentation, https://github.com/canorve/EllipSect/blob/master/README.rst
 Project-URL: Source, https://github.com/canorve/EllipSect
```

### Comparing `EllipSect-3.4.0/README.rst` & `ellipsect-3.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/docs/Makefile` & `ellipsect-3.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/docs/api.rst` & `ellipsect-3.4.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/docs/conf.py` & `ellipsect-3.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/docs/howto.rst` & `ellipsect-3.4.1/docs/howto.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/docs/index.rst` & `ellipsect-3.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/example/gal.fits` & `ellipsect-3.4.1/example/gal.fits`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/example/galfit.feedme` & `ellipsect-3.4.1/example/galfit.feedme`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/example/psf.fits` & `ellipsect-3.4.1/example/psf.fits`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/img/A2029.ring.png` & `ellipsect-3.4.1/img/A2029.ring.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/img/A85.comp.png` & `ellipsect-3.4.1/img/A85.comp.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/img/A85.con-cub.png` & `ellipsect-3.4.1/img/A85.con-cub.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/img/A85.cub.png` & `ellipsect-3.4.1/img/A85.cub.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/img/A85.def.png` & `ellipsect-3.4.1/img/A85.def.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/img/A85.ell-cub.png` & `ellipsect-3.4.1/img/A85.ell-cub.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/img/A85.grid.png` & `ellipsect-3.4.1/img/A85.grid.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/img/A85.log.png` & `ellipsect-3.4.1/img/A85.log.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/img/A85.pix.png` & `ellipsect-3.4.1/img/A85.pix.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/img/A85.png` & `ellipsect-3.4.1/img/A85.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/img/A85.ranx1.png` & `ellipsect-3.4.1/img/A85.ranx1.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/img/A85.ranx2.png` & `ellipsect-3.4.1/img/A85.ranx2.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/img/A85.rany1.png` & `ellipsect-3.4.1/img/A85.rany1.png`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/setup.cfg` & `ellipsect-3.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/setup.py` & `ellipsect-3.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/EllipSect.egg-info/PKG-INFO` & `ellipsect-3.4.1/src/EllipSect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EllipSect
-Version: 3.4.0
+Version: 3.4.1
 Summary: A surface brightness analysis tool for GALFIT output.
 Home-page: https://github.com/canorve/EllipSect
 Author: Christopher Añorve
 Author-email: canorve@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Documentation, https://github.com/canorve/EllipSect/blob/master/README.rst
 Project-URL: Source, https://github.com/canorve/EllipSect
```

### Comparing `EllipSect-3.4.0/src/EllipSect.egg-info/SOURCES.txt` & `ellipsect-3.4.1/src/EllipSect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/__init__.py` & `ellipsect-3.4.1/src/ellipsect/__init__.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/ellipsectors.py` & `ellipsect-3.4.1/src/ellipsect/ellipsectors.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/inout/galfit.py` & `ellipsect-3.4.1/src/ellipsect/inout/galfit.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/inout/gfits.py` & `ellipsect-3.4.1/src/ellipsect/inout/gfits.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/inout/plots.py` & `ellipsect-3.4.1/src/ellipsect/inout/plots.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/inout/prt.py` & `ellipsect-3.4.1/src/ellipsect/inout/prt.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/inout/read.py` & `ellipsect-3.4.1/src/ellipsect/inout/read.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/lib/clas.py` & `ellipsect-3.4.1/src/ellipsect/lib/clas.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/lib/libs.py` & `ellipsect-3.4.1/src/ellipsect/lib/libs.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/phot/ned.py` & `ellipsect-3.4.1/src/ellipsect/phot/ned.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/phot/phot.py` & `ellipsect-3.4.1/src/ellipsect/phot/phot.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/phot/tidal.py` & `ellipsect-3.4.1/src/ellipsect/phot/tidal.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/sectors/comp.py` & `ellipsect-3.4.1/src/ellipsect/sectors/comp.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/sectors/ellip.py` & `ellipsect-3.4.1/src/ellipsect/sectors/ellip.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/sectors/num.py` & `ellipsect-3.4.1/src/ellipsect/sectors/num.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/sectors/sect.py` & `ellipsect-3.4.1/src/ellipsect/sectors/sect.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/src/ellipsect/sky/sky.py` & `ellipsect-3.4.1/src/ellipsect/sky/sky.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,14 +255,17 @@
 
 
     def GetXYRBorder(self):
         "this subroutine get the coordinates of the border"
 
         q =  self.q
 
+        if self.thetadeg > 360:
+            self.thetadeg = self.thetadeg - 360 #quick fix
+
         theta = self.thetadeg * (np.pi / 180)  # rads!!
 
         thetax=np.sqrt((np.cos(theta))**2 + (q**2)*(np.sin(theta))**2 )
         thetay=np.sqrt((q**2)*(np.cos(theta))**2 + (np.sin(theta))**2 )
 
 
         if (self.thetadeg >-45 and self.thetadeg <= 45):
```

### Comparing `EllipSect-3.4.0/tests/gal.fits` & `ellipsect-3.4.1/tests/gal.fits`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/tests/galfit.01` & `ellipsect-3.4.1/tests/galfit.01`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/tests/imgblock.fits` & `ellipsect-3.4.1/tests/imgblock.fits`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/tests/psf.fits` & `ellipsect-3.4.1/tests/psf.fits`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/tests/test_ellipsect.py` & `ellipsect-3.4.1/tests/test_ellipsect.py`

 * *Files identical despite different names*

### Comparing `EllipSect-3.4.0/tox.ini` & `ellipsect-3.4.1/tox.ini`

 * *Files identical despite different names*

