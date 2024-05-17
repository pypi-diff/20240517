# Comparing `tmp/CluSex-2.3.6.tar.gz` & `tmp/clusex-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CluSex-2.3.6.tar", last modified: Wed Oct  5 00:27:20 2022, max compression
+gzip compressed data, was "clusex-2.3.8.tar", last modified: Fri May 17 00:07:06 2024, max compression
```

## Comparing `CluSex-2.3.6.tar` & `clusex-2.3.8.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2022-10-05 00:27:20.565642 CluSex-2.3.6/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      120 2022-09-08 03:54:53.000000 CluSex-2.3.6/AUTHORS.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      128 2022-05-11 23:56:49.000000 CluSex-2.3.6/CHANGELOG.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    13802 2022-05-11 23:56:49.000000 CluSex-2.3.6/CONTRIBUTING.rst
--rwxrwxrwx   0 canorve   (1000) canorve   (1000)    35148 2018-04-30 20:18:27.000000 CluSex-2.3.6/LICENSE.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    11821 2022-10-05 00:27:20.565642 CluSex-2.3.6/PKG-INFO
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    10996 2022-09-08 03:54:41.000000 CluSex-2.3.6/README.rst
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2022-10-05 00:27:20.549642 CluSex-2.3.6/docs/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1154 2022-05-11 23:56:49.000000 CluSex-2.3.6/docs/Makefile
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2022-10-05 00:27:20.549642 CluSex-2.3.6/docs/_static/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       18 2022-05-11 23:56:49.000000 CluSex-2.3.6/docs/_static/.gitignore
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     3977 2022-08-31 03:34:53.000000 CluSex-2.3.6/docs/api.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       41 2022-05-11 23:56:49.000000 CluSex-2.3.6/docs/authors.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       43 2022-05-11 23:56:49.000000 CluSex-2.3.6/docs/changelog.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     9743 2022-05-11 23:56:49.000000 CluSex-2.3.6/docs/conf.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     5926 2022-09-08 04:00:18.000000 CluSex-2.3.6/docs/config.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       33 2022-05-11 23:56:49.000000 CluSex-2.3.6/docs/contributing.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     5694 2022-09-08 03:57:51.000000 CluSex-2.3.6/docs/howto.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2309 2022-05-11 23:56:49.000000 CluSex-2.3.6/docs/index.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       67 2022-05-11 23:56:49.000000 CluSex-2.3.6/docs/license.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)       39 2022-05-20 21:06:40.000000 CluSex-2.3.6/docs/readme.rst
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      341 2022-10-04 22:38:17.000000 CluSex-2.3.6/docs/requirements.txt
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2022-10-05 00:27:20.561642 CluSex-2.3.6/img/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)  1435524 2022-08-15 20:48:46.000000 CluSex-2.3.6/img/Comagood.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)  1381688 2022-08-24 01:11:10.000000 CluSex-2.3.6/img/Comaimproved.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   948143 2022-08-15 20:40:43.000000 CluSex-2.3.6/img/Comarun1.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   979901 2022-08-15 20:40:55.000000 CluSex-2.3.6/img/Comarun2.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)  1118810 2022-08-15 20:27:00.000000 CluSex-2.3.6/img/SatRegion.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   889911 2022-08-24 01:11:10.000000 CluSex-2.3.6/img/mask.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)   889506 2022-08-24 01:11:10.000000 CluSex-2.3.6/img/mask2.png
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      355 2022-05-11 23:56:49.000000 CluSex-2.3.6/pyproject.toml
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1981 2022-10-05 00:27:20.569642 CluSex-2.3.6/setup.cfg
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      703 2022-05-11 23:56:49.000000 CluSex-2.3.6/setup.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2022-10-05 00:27:20.545642 CluSex-2.3.6/src/
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2022-10-05 00:27:20.565642 CluSex-2.3.6/src/CluSex.egg-info/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    11821 2022-10-05 00:27:20.000000 CluSex-2.3.6/src/CluSex.egg-info/PKG-INFO
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1237 2022-10-05 00:27:20.000000 CluSex-2.3.6/src/CluSex.egg-info/SOURCES.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        1 2022-10-05 00:27:20.000000 CluSex-2.3.6/src/CluSex.egg-info/dependency_links.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      363 2022-10-05 00:27:20.000000 CluSex-2.3.6/src/CluSex.egg-info/entry_points.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        1 2022-08-17 19:57:55.000000 CluSex-2.3.6/src/CluSex.egg-info/not-zip-safe
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      185 2022-10-05 00:27:20.000000 CluSex-2.3.6/src/CluSex.egg-info/requires.txt
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        7 2022-10-05 00:27:20.000000 CluSex-2.3.6/src/CluSex.egg-info/top_level.txt
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2022-10-05 00:27:20.565642 CluSex-2.3.6/src/clusex/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      806 2022-09-04 19:56:22.000000 CluSex-2.3.6/src/clusex/__init__.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2022-10-05 00:27:20.565642 CluSex-2.3.6/src/clusex/config/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2022-05-22 19:27:45.000000 CluSex-2.3.6/src/clusex/config/__init__.py
--rwxrwxrwx   0 canorve   (1000) canorve   (1000)       88 2010-03-31 15:31:30.000000 CluSex-2.3.6/src/clusex/config/default.conv
--rwxrwxrwx   0 canorve   (1000) canorve   (1000)     2187 2010-03-31 15:31:31.000000 CluSex-2.3.6/src/clusex/config/default.nnw
--rw-r--r--   0 canorve   (1000) canorve   (1000)     6944 2019-10-17 20:41:58.000000 CluSex-2.3.6/src/clusex/config/default.sex
--rwxr-xr-x   0 canorve   (1000) canorve   (1000)     1583 2022-08-16 06:44:51.000000 CluSex-2.3.6/src/clusex/config/sex.param
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2022-10-05 00:27:20.565642 CluSex-2.3.6/src/clusex/lib/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2022-05-26 03:17:44.000000 CluSex-2.3.6/src/clusex/lib/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     8719 2022-09-30 05:37:07.000000 CluSex-2.3.6/src/clusex/lib/cgpng.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     3075 2022-09-06 03:05:25.000000 CluSex-2.3.6/src/clusex/lib/check.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1680 2022-08-09 19:11:52.000000 CluSex-2.3.6/src/clusex/lib/ds9.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     1558 2022-08-09 20:22:18.000000 CluSex-2.3.6/src/clusex/lib/init.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     5538 2022-08-17 18:08:48.000000 CluSex-2.3.6/src/clusex/lib/join.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    15324 2022-09-28 04:11:16.000000 CluSex-2.3.6/src/clusex/lib/make.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     4648 2022-07-28 23:12:10.000000 CluSex-2.3.6/src/clusex/lib/radcor.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     7174 2022-09-02 23:32:59.000000 CluSex-2.3.6/src/clusex/lib/read.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    21469 2022-08-03 00:40:53.000000 CluSex-2.3.6/src/clusex/lib/satbox.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    21137 2022-08-05 22:10:55.000000 CluSex-2.3.6/src/clusex/lib/sky.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     4975 2022-07-29 23:37:15.000000 CluSex-2.3.6/src/clusex/lib/writesex.py
--rwxrwxrwx   0 canorve   (1000) canorve   (1000)     7591 2022-09-03 18:50:07.000000 CluSex-2.3.6/src/clusex/pysex.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2022-10-05 00:27:20.565642 CluSex-2.3.6/src/clusex/run/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2022-05-26 03:17:44.000000 CluSex-2.3.6/src/clusex/run/__init__.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)    18158 2022-09-30 05:47:42.000000 CluSex-2.3.6/src/clusex/run/console.py
-drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2022-10-05 00:27:20.565642 CluSex-2.3.6/tests/
--rw-rw-r--   0 canorve   (1000) canorve   (1000)      274 2022-05-11 23:56:49.000000 CluSex-2.3.6/tests/conftest.py
--rw-rw-r--   0 canorve   (1000) canorve   (1000)     2575 2022-05-11 23:56:49.000000 CluSex-2.3.6/tox.ini
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-17 00:07:05.995710 clusex-2.3.8/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      120 2022-09-08 03:54:53.000000 clusex-2.3.8/AUTHORS.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      128 2022-05-11 23:56:49.000000 clusex-2.3.8/CHANGELOG.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    13802 2022-05-11 23:56:49.000000 clusex-2.3.8/CONTRIBUTING.rst
+-rwxrwxrwx   0 canorve   (1000) canorve   (1000)    35148 2018-04-30 20:18:27.000000 clusex-2.3.8/LICENSE.txt
+-rw-r--r--   0 canorve   (1000) canorve   (1000)    12217 2024-05-17 00:07:05.995710 clusex-2.3.8/PKG-INFO
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    10996 2022-09-08 03:54:41.000000 clusex-2.3.8/README.rst
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-17 00:07:05.927710 clusex-2.3.8/docs/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1154 2022-05-11 23:56:49.000000 clusex-2.3.8/docs/Makefile
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-17 00:07:05.931710 clusex-2.3.8/docs/_static/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       18 2022-05-11 23:56:49.000000 clusex-2.3.8/docs/_static/.gitignore
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     3977 2022-08-31 03:34:53.000000 clusex-2.3.8/docs/api.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       41 2022-05-11 23:56:49.000000 clusex-2.3.8/docs/authors.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       43 2022-05-11 23:56:49.000000 clusex-2.3.8/docs/changelog.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     9743 2022-05-11 23:56:49.000000 clusex-2.3.8/docs/conf.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     5926 2022-09-08 04:00:18.000000 clusex-2.3.8/docs/config.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       33 2022-05-11 23:56:49.000000 clusex-2.3.8/docs/contributing.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     5694 2022-09-08 03:57:51.000000 clusex-2.3.8/docs/howto.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2309 2022-05-11 23:56:49.000000 clusex-2.3.8/docs/index.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       67 2022-05-11 23:56:49.000000 clusex-2.3.8/docs/license.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)       39 2022-05-20 21:06:40.000000 clusex-2.3.8/docs/readme.rst
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      373 2022-10-16 09:05:30.000000 clusex-2.3.8/docs/requirements.txt
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-17 00:07:05.979710 clusex-2.3.8/img/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)  1435524 2022-08-15 20:48:46.000000 clusex-2.3.8/img/Comagood.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)  1381688 2022-08-24 01:11:10.000000 clusex-2.3.8/img/Comaimproved.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   948143 2022-08-15 20:40:43.000000 clusex-2.3.8/img/Comarun1.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   979901 2022-08-15 20:40:55.000000 clusex-2.3.8/img/Comarun2.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)  1118810 2022-08-15 20:27:00.000000 clusex-2.3.8/img/SatRegion.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   889911 2022-08-24 01:11:10.000000 clusex-2.3.8/img/mask.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)   889506 2022-08-24 01:11:10.000000 clusex-2.3.8/img/mask2.png
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      355 2022-05-11 23:56:49.000000 clusex-2.3.8/pyproject.toml
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1981 2024-05-17 00:07:05.995710 clusex-2.3.8/setup.cfg
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      703 2022-05-11 23:56:49.000000 clusex-2.3.8/setup.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-17 00:07:05.903710 clusex-2.3.8/src/
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-17 00:07:05.995710 clusex-2.3.8/src/CluSex.egg-info/
+-rw-r--r--   0 canorve   (1000) canorve   (1000)    12217 2024-05-17 00:07:05.000000 clusex-2.3.8/src/CluSex.egg-info/PKG-INFO
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1258 2024-05-17 00:07:05.000000 clusex-2.3.8/src/CluSex.egg-info/SOURCES.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        1 2024-05-17 00:07:05.000000 clusex-2.3.8/src/CluSex.egg-info/dependency_links.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      363 2024-05-17 00:07:05.000000 clusex-2.3.8/src/CluSex.egg-info/entry_points.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        1 2022-08-17 19:57:55.000000 clusex-2.3.8/src/CluSex.egg-info/not-zip-safe
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      185 2024-05-17 00:07:05.000000 clusex-2.3.8/src/CluSex.egg-info/requires.txt
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        7 2024-05-17 00:07:05.000000 clusex-2.3.8/src/CluSex.egg-info/top_level.txt
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-17 00:07:05.987710 clusex-2.3.8/src/clusex/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      806 2022-09-04 19:56:22.000000 clusex-2.3.8/src/clusex/__init__.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-17 00:07:05.991711 clusex-2.3.8/src/clusex/config/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2022-05-22 19:27:45.000000 clusex-2.3.8/src/clusex/config/__init__.py
+-rwxrwxrwx   0 canorve   (1000) canorve   (1000)       88 2010-03-31 15:31:30.000000 clusex-2.3.8/src/clusex/config/default.conv
+-rwxrwxrwx   0 canorve   (1000) canorve   (1000)     2187 2010-03-31 15:31:31.000000 clusex-2.3.8/src/clusex/config/default.nnw
+-rw-r--r--   0 canorve   (1000) canorve   (1000)     6944 2019-10-17 20:41:58.000000 clusex-2.3.8/src/clusex/config/default.sex
+-rwxr-xr-x   0 canorve   (1000) canorve   (1000)     1583 2022-08-16 06:44:51.000000 clusex-2.3.8/src/clusex/config/sex.param
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-17 00:07:05.991711 clusex-2.3.8/src/clusex/lib/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2022-05-26 03:17:44.000000 clusex-2.3.8/src/clusex/lib/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     8719 2022-09-30 05:37:07.000000 clusex-2.3.8/src/clusex/lib/cgpng.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     3075 2022-09-06 03:05:25.000000 clusex-2.3.8/src/clusex/lib/check.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1680 2022-08-09 19:11:52.000000 clusex-2.3.8/src/clusex/lib/ds9.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     1558 2022-08-09 20:22:18.000000 clusex-2.3.8/src/clusex/lib/init.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     5538 2022-08-17 18:08:48.000000 clusex-2.3.8/src/clusex/lib/join.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    16484 2023-10-25 21:34:55.000000 clusex-2.3.8/src/clusex/lib/make.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     4648 2022-07-28 23:12:10.000000 clusex-2.3.8/src/clusex/lib/radcor.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     7174 2022-09-02 23:32:59.000000 clusex-2.3.8/src/clusex/lib/read.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    21469 2022-08-03 00:40:53.000000 clusex-2.3.8/src/clusex/lib/satbox.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    21365 2024-05-16 23:06:05.000000 clusex-2.3.8/src/clusex/lib/sky.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     4975 2022-07-29 23:37:15.000000 clusex-2.3.8/src/clusex/lib/writesex.py
+-rwxrwxrwx   0 canorve   (1000) canorve   (1000)     7578 2022-10-16 09:04:08.000000 clusex-2.3.8/src/clusex/pysex.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-17 00:07:05.995710 clusex-2.3.8/src/clusex/run/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)        0 2022-05-26 03:17:44.000000 clusex-2.3.8/src/clusex/run/__init__.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)    18158 2022-09-30 05:47:42.000000 clusex-2.3.8/src/clusex/run/console.py
+drwxrwxr-x   0 canorve   (1000) canorve   (1000)        0 2024-05-17 00:07:05.995710 clusex-2.3.8/tests/
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      274 2022-05-11 23:56:49.000000 clusex-2.3.8/tests/conftest.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)      629 2022-10-22 00:53:34.000000 clusex-2.3.8/tests/test_clusex.py
+-rw-rw-r--   0 canorve   (1000) canorve   (1000)     2616 2022-10-16 08:40:50.000000 clusex-2.3.8/tox.ini
```

### Comparing `CluSex-2.3.6/CONTRIBUTING.rst` & `clusex-2.3.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/LICENSE.txt` & `clusex-2.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/PKG-INFO` & `clusex-2.3.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CluSex
-Version: 2.3.6
+Version: 2.3.8
 Summary: Sextractor on Cluster Galaxies
 Home-page: https://github.com/canorve/CluSex
 Author: Christopher Añorve, Omar López-Cruz
 Author-email: canorve@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Documentation, https://github.com/canorve/CluSex/blob/master/README.rst
 Platform: any
@@ -12,16 +12,27 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: testing
 License-File: LICENSE.txt
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: sphinx>=3.2.1
+Requires-Dist: numpy>=1.20.3
+Requires-Dist: astropy>=4.0.2
+Requires-Dist: matplotlib>=3.5.2
+Requires-Dist: pandas>=1.3.4
+Requires-Dist: Pillow>=8.4.0
+Requires-Dist: tk>=0.1.0
+Provides-Extra: testing
+Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
 
 .. contents::
    :depth: 3
 ..
 
 
 --------------
```

### Comparing `CluSex-2.3.6/README.rst` & `clusex-2.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/docs/Makefile` & `clusex-2.3.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/docs/api.rst` & `clusex-2.3.8/docs/api.rst`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/docs/conf.py` & `clusex-2.3.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/docs/config.rst` & `clusex-2.3.8/docs/config.rst`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/docs/howto.rst` & `clusex-2.3.8/docs/howto.rst`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/docs/index.rst` & `clusex-2.3.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/img/Comagood.png` & `clusex-2.3.8/img/Comagood.png`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/img/Comaimproved.png` & `clusex-2.3.8/img/Comaimproved.png`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/img/Comarun1.png` & `clusex-2.3.8/img/Comarun1.png`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/img/Comarun2.png` & `clusex-2.3.8/img/Comarun2.png`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/img/SatRegion.png` & `clusex-2.3.8/img/SatRegion.png`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/img/mask.png` & `clusex-2.3.8/img/mask.png`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/img/mask2.png` & `clusex-2.3.8/img/mask2.png`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/setup.cfg` & `clusex-2.3.8/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	sphinx>=3.2.1
 	numpy>=1.20.3
 	astropy>=4.0.2
 	matplotlib>=3.5.2
 	pandas>=1.3.4
-	tkinter>=8.6
-	PIL>=8.4.0
+	Pillow>=8.4.0
+	tk>=0.1.0
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `CluSex-2.3.6/setup.py` & `clusex-2.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/src/CluSex.egg-info/PKG-INFO` & `clusex-2.3.8/src/CluSex.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CluSex
-Version: 2.3.6
+Version: 2.3.8
 Summary: Sextractor on Cluster Galaxies
 Home-page: https://github.com/canorve/CluSex
 Author: Christopher Añorve, Omar López-Cruz
 Author-email: canorve@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Documentation, https://github.com/canorve/CluSex/blob/master/README.rst
 Platform: any
@@ -12,16 +12,27 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: testing
 License-File: LICENSE.txt
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: sphinx>=3.2.1
+Requires-Dist: numpy>=1.20.3
+Requires-Dist: astropy>=4.0.2
+Requires-Dist: matplotlib>=3.5.2
+Requires-Dist: pandas>=1.3.4
+Requires-Dist: Pillow>=8.4.0
+Requires-Dist: tk>=0.1.0
+Provides-Extra: testing
+Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
 
 .. contents::
    :depth: 3
 ..
 
 
 --------------
```

### Comparing `CluSex-2.3.6/src/CluSex.egg-info/SOURCES.txt` & `clusex-2.3.8/src/CluSex.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -51,8 +51,9 @@
 src/clusex/lib/radcor.py
 src/clusex/lib/read.py
 src/clusex/lib/satbox.py
 src/clusex/lib/sky.py
 src/clusex/lib/writesex.py
 src/clusex/run/__init__.py
 src/clusex/run/console.py
-tests/conftest.py
+tests/conftest.py
+tests/test_clusex.py
```

### Comparing `CluSex-2.3.6/src/clusex/__init__.py` & `clusex-2.3.8/src/clusex/__init__.py`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/src/clusex/config/default.nnw` & `clusex-2.3.8/src/clusex/config/default.nnw`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/src/clusex/config/default.sex` & `clusex-2.3.8/src/clusex/config/default.sex`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/src/clusex/config/sex.param` & `clusex-2.3.8/src/clusex/config/sex.param`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/src/clusex/lib/cgpng.py` & `clusex-2.3.8/src/clusex/lib/cgpng.py`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/src/clusex/lib/check.py` & `clusex-2.3.8/src/clusex/lib/check.py`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/src/clusex/lib/ds9.py` & `clusex-2.3.8/src/clusex/lib/ds9.py`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/src/clusex/lib/init.py` & `clusex-2.3.8/src/clusex/lib/init.py`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/src/clusex/lib/join.py` & `clusex-2.3.8/src/clusex/lib/join.py`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/src/clusex/lib/make.py` & `clusex-2.3.8/src/clusex/lib/make.py`

 * *Files 4% similar despite different names*

```diff
@@ -439,19 +439,26 @@
             imgstmp = "obj-" + str(round(N[idx])) + ".png"
 
             yy = int(X[idx]) - xmin[idx]  #interchange because numpy arrays 
 
             xx = int(Y[idx]) - ymin[idx] 
 
             #quick routine:
+            #ShowImg(stamp[ymin[idx]-1:ymax[idx]-1,xmin[idx]-1:xmax[idx]-1], 
+            #            xx, yy, wcs, imgstmp, dpival = dpi, sky = Bkgd[idx], 
+            #            cmap = cmap, bri = bright, con = contrast, 
+            #            frac = frac, fracmax = fracmax)
+
             ShowImg(stamp[ymin[idx]-1:ymax[idx]-1,xmin[idx]-1:xmax[idx]-1], 
-                        xx, yy, wcs, imgstmp, dpival = dpi, sky = Bkgd[idx], 
+                        wcs, imgstmp, dpival = dpi, sky = Bkgd[idx], 
                         cmap = cmap, bri = bright, con = contrast, 
                         frac = frac, fracmax = fracmax)
 
+
+
             #slow routine
 
             #GetPng(stamp[ymin[idx]-1:ymax[idx]-1,xmin[idx]-1:xmax[idx]-1], 
             #        counts, wcs, dpi=dpi, cmap = cmap, namepng = imgstmp, 
             #        bri = bright, con = contrast)
 
 
@@ -477,70 +484,100 @@
 
     objimg[zero_pix]  = 0
 
     return objimg
 
 
 def ShowImg(img: np.array ,xc: int, yc: int, wcs, namepng="obj.png", 
-            dpival=100, sky=1, cmap='viridis', bri = 33, con = 0.98, 
+            dpival=100, sky=1, cmap='viridis', bri = 0, con = 1, 
             frac = 1, fracmax = 1):
     """This routine shows the image"""
 
         
     #hdu = fits.open(cubeimg)
     #data = (hdu[1].data.copy()).astype(float)
     #hdu.close()
 
-    data=img
+    data =  (img.copy()).astype(float)
 
     root_ext = os.path.splitext(namepng)
 
     objname = root_ext[0]
 
+    #flatten image
+
+    flatdatimg = data.flatten()  
+
+    flatdatimg.sort()
+
+    datimgpatch = flatdatimg#[modbot:modtop]
+
+    datmin = np.min(datimgpatch)
+    datmax = np.max(datimgpatch)
+
+
+    data = data.clip(datmax/1e4, datmax)
 
-    mask=data < 0 
+    datmin = datmax/1e4
+
+
+    middle = (datmax -datmin)/2
+
+   #brightness auto-adjust according to the contrast value 
+
+    Autobri = middle*(con -1) + modmin*(1-con) 
+
+    #user can re-adjust according to the contrast value
+    newdata = con*(data - middle) + middle + Autobri + bri*(datmax-middle)
+
+    mask = data < 0 
     data[mask] = 1 # avoids problems in log
      
-    fig, ax1 = plt.subplots(figsize=(7, 7)) 
+    fig, ax1 = plt.subplots(figsize=(8, 8)) 
+    #fig, ax1 = plt.subplots(figsize=(700/dpival, 700/dpival),dpi=dpival) 
+    #plt.figure(figsize = (800 / my_dpi, 800 / my_dpi), dpi = my_dpi)
+
+
     fig.subplots_adjust(left=0.08, right=0.94, bottom=0.04, top=0.94)
 
-    ax1=fig.add_subplot(projection=wcs)
+    ax1 = fig.add_subplot(projection=wcs)
 
-    flatdata=data.flatten()  
+    #flatdata = data.flatten()  
 
-    flatdata.sort()
+    #flatdata.sort()
 
-    tot=len(flatdata)
+    #tot=len(flatdata)
 
-    top=round(.9*tot)
-    bot=round(.1*tot)
+    #top=round(.9*tot)
+    #bot=round(.1*tot)
 
-    imgpatch=flatdata#[bot:top]
+    #imgpatch=flatdata#[bot:top]
 
 
+    #galmin = np.min(imgpatch)
+    #galmin = sky 
+    #galmax = np.max(imgpatch)
 
-    galmin = np.min(imgpatch)
-    galmin = sky 
-    galmax = np.max(imgpatch)
+    #median=np.median(imgpatch)
 
- 
-    median=np.median(imgpatch)
+    #galmin = (frac)*galmin 
+    #galmax = fracmax*galmax
 
-    galmin = (frac)*galmin 
-    galmax = fracmax*galmax
 
+    #if (galmin > galmax): #to prevent from failing
+    #    galmin, galmax = galmax, galmin
 
-    if (galmin > galmax): #to prevent from failing
-        galmin, galmax = galmax, galmin
+    #my old routine
+    #ax1.imshow(con*data+bri, origin = 'lower', norm
+    #            = colors.LogNorm(vmin = galmin, vmax = galmax), 
+    #            cmap = cmap, interpolation='nearest')
 
-    #my routine
-    ax1.imshow(con*data+bri, origin = 'lower', norm
-                = colors.LogNorm(vmin = galmin, vmax = galmax), 
-                cmap = cmap, interpolation='nearest')
 
+    im = ax1.imshow(newdata, origin ='lower', interpolation='nearest', norm 
+                    = colors.LogNorm(vmin=datmin, vmax=datmax), cmap = cmap)
 
 
     ax1.set_xlabel('Right Ascension')
     ax1.set_ylabel('Declination')
     ax1.grid(color='black', ls='solid', alpha=0.1)
 
     ax1.set_title(objname)
```

### Comparing `CluSex-2.3.6/src/clusex/lib/radcor.py` & `clusex-2.3.8/src/clusex/lib/radcor.py`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/src/clusex/lib/read.py` & `clusex-2.3.8/src/clusex/lib/read.py`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/src/clusex/lib/satbox.py` & `clusex-2.3.8/src/clusex/lib/satbox.py`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/src/clusex/lib/sky.py` & `clusex-2.3.8/src/clusex/lib/sky.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,17 @@
 
 
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
@@ -359,22 +362,27 @@
             #skystd=np.append(skystd,std)
             skymed=np.append(skymed,median)
 
 
 
         totmean = np.mean(sky)
         # to compute standard deviation:
-        for idx, item in enumerate(range(cont)):
+        #for idx, item in enumerate(range(cont)):
 
-            bimg=boximg[idx]
+        #    bimg=boximg[idx]
 
             # not quite the var of the box, but it is needed to compute the TOTAL std:
-            skyvar =  ((bimg-totmean)**2).sum() 
+        #    skyvar =  ((bimg-totmean)**2).sum() 
+
+        #    skystd=np.append(skystd,skyvar)
 
-            skystd=np.append(skystd,skyvar)
+        # new way to compute sky
+        sky = np.mean(boximg) 
+        skystd = np.std(boximg)
+        skymed = np.median(boximg)
 
 
         return sky,skystd,skymed,N
 
     def MakeCoord(self,xmino,xmaxo,ymino,ymaxo,xmaxf,ymaxf):
         ''' creates (x,y) coordinates between the inner and outer box'''
```

### Comparing `CluSex-2.3.6/src/clusex/lib/writesex.py` & `clusex-2.3.8/src/clusex/lib/writesex.py`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/src/clusex/pysex.py` & `clusex-2.3.8/src/clusex/pysex.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 import numpy as np
 import sys
 import os
 import subprocess as sp
 from astropy.io import fits
 import os.path
-import scipy
 
 from pathlib import Path
 import shutil
 import argparse
 
 
 from clusex.lib.init import Params
```

### Comparing `CluSex-2.3.6/src/clusex/run/console.py` & `clusex-2.3.8/src/clusex/run/console.py`

 * *Files identical despite different names*

### Comparing `CluSex-2.3.6/tox.ini` & `clusex-2.3.8/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Read more under https://tox.wiki/
 # THIS SCRIPT IS SUPPOSED TO BE AN EXAMPLE. MODIFY IT ACCORDING TO YOUR NEEDS!
 
 [tox]
 minversion = 3.24
 envlist = default
 isolated_build = True
-
+tox_pip_extensions_ext_venv_update = true
 
 [testenv]
 description = Invoke pytest to run automated tests
 setenv =
     TOXINIDIR = {toxinidir}
 passenv =
     HOME
```

