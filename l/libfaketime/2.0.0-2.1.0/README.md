# Comparing `tmp/libfaketime-2.0.0.tar.gz` & `tmp/libfaketime-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libfaketime-2.0.0.tar", last modified: Fri Apr 17 16:03:10 2020, max compression
+gzip compressed data, was "libfaketime-2.1.0.tar", last modified: Fri May 17 14:22:40 2024, max compression
```

## Comparing `libfaketime-2.0.0.tar` & `libfaketime-2.1.0.tar`

### file list

```diff
@@ -1,49 +1,38 @@
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2020-04-17 16:03:10.000000 libfaketime-2.0.0/
--rw-rw-r--   0 simon     (1000) simon     (1000)     3134 2020-04-17 16:02:57.000000 libfaketime-2.0.0/CHANGELOG.rst
--rw-------   0 simon     (1000) simon     (1000)    18027 2016-04-02 16:37:49.000000 libfaketime-2.0.0/LICENSE
--rw-------   0 simon     (1000) simon     (1000)      671 2017-07-16 04:08:39.000000 libfaketime-2.0.0/MANIFEST.in
--rw-rw-r--   0 simon     (1000) simon     (1000)    12113 2020-04-17 16:03:10.000000 libfaketime-2.0.0/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)     5725 2020-04-17 16:02:57.000000 libfaketime-2.0.0/README.rst
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2020-04-17 16:03:10.000000 libfaketime-2.0.0/libfaketime/
--rw-rw-r--   0 simon     (1000) simon     (1000)     8752 2020-04-17 15:43:01.000000 libfaketime-2.0.0/libfaketime/__init__.py
--rw-rw-r--   0 simon     (1000) simon     (1000)       22 2020-04-17 16:02:57.000000 libfaketime-2.0.0/libfaketime/_version.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2020-04-17 16:03:10.000000 libfaketime-2.0.0/libfaketime/vendor/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2020-04-17 16:03:10.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime/
--rw-------   0 simon     (1000) simon     (1000)    18092 2016-04-02 16:38:52.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime/COPYING
--rw-------   0 simon     (1000) simon     (1000)      953 2016-04-02 16:38:52.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime/Makefile
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2020-04-17 16:03:10.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime/src/
--rw-rw-r--   0 simon     (1000) simon     (1000)     4075 2018-05-19 23:09:35.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime/src/Makefile
--rw-rw-r--   0 simon     (1000) simon     (1000)     2481 2018-05-19 23:09:35.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime/src/Makefile.OSX
--rw-rw-r--   0 simon     (1000) simon     (1000)    10787 2018-05-19 23:09:35.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime/src/faketime.c
--rw-------   0 simon     (1000) simon     (1000)     1730 2017-07-16 04:12:57.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime/src/faketime_common.h
--rw-rw-r--   0 simon     (1000) simon     (1000)    67475 2018-05-19 23:09:35.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime/src/libfaketime.c
--rw-rw-r--   0 simon     (1000) simon     (1000)      412 2018-05-19 23:09:35.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime/src/libfaketime.map
--rw-------   0 simon     (1000) simon     (1000)      219 2016-04-02 16:38:52.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime/src/sunos_endian.h
--rw-------   0 simon     (1000) simon     (1000)     4823 2016-04-02 16:38:52.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime/src/time_ops.h
--rw-rw-r--   0 simon     (1000) simon     (1000)    77489 2018-05-19 23:09:35.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime/src/uthash.h
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2020-04-17 16:03:10.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime-pre_sierra/
--rw-------   0 simon     (1000) simon     (1000)    18092 2017-07-16 04:12:57.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime-pre_sierra/COPYING
--rw-------   0 simon     (1000) simon     (1000)      953 2017-07-16 04:12:57.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime-pre_sierra/Makefile
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2020-04-17 16:03:10.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime-pre_sierra/src/
--rw-------   0 simon     (1000) simon     (1000)     4033 2017-07-16 04:12:57.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime-pre_sierra/src/Makefile
--rw-------   0 simon     (1000) simon     (1000)     2482 2017-07-16 04:12:57.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime-pre_sierra/src/Makefile.OSX
--rw-rw-r--   0 simon     (1000) simon     (1000)    10984 2018-05-19 23:09:35.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime-pre_sierra/src/faketime.c
--rw-------   0 simon     (1000) simon     (1000)     1463 2017-07-16 04:12:57.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime-pre_sierra/src/faketime_common.h
--rw-rw-r--   0 simon     (1000) simon     (1000)    57253 2018-05-19 23:09:35.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime-pre_sierra/src/libfaketime.c
--rw-------   0 simon     (1000) simon     (1000)      181 2017-07-16 04:12:57.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime-pre_sierra/src/libfaketime.map
--rw-------   0 simon     (1000) simon     (1000)      219 2017-07-16 04:12:57.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime-pre_sierra/src/sunos_endian.h
--rw-------   0 simon     (1000) simon     (1000)     4823 2017-07-16 04:12:57.000000 libfaketime-2.0.0/libfaketime/vendor/libfaketime-pre_sierra/src/time_ops.h
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2020-04-17 16:03:10.000000 libfaketime-2.0.0/libfaketime.egg-info/
--rw-------   0 simon     (1000) simon     (1000)    12113 2020-04-17 16:03:10.000000 libfaketime-2.0.0/libfaketime.egg-info/PKG-INFO
--rw-------   0 simon     (1000) simon     (1000)     1504 2020-04-17 16:03:10.000000 libfaketime-2.0.0/libfaketime.egg-info/SOURCES.txt
--rw-------   0 simon     (1000) simon     (1000)        1 2020-04-17 16:03:10.000000 libfaketime-2.0.0/libfaketime.egg-info/dependency_links.txt
--rw-------   0 simon     (1000) simon     (1000)       57 2020-04-17 16:03:10.000000 libfaketime-2.0.0/libfaketime.egg-info/entry_points.txt
--rw-------   0 simon     (1000) simon     (1000)        1 2016-04-02 16:42:26.000000 libfaketime-2.0.0/libfaketime.egg-info/not-zip-safe
--rw-------   0 simon     (1000) simon     (1000)       32 2020-04-17 16:03:10.000000 libfaketime-2.0.0/libfaketime.egg-info/requires.txt
--rw-------   0 simon     (1000) simon     (1000)       12 2020-04-17 16:03:10.000000 libfaketime-2.0.0/libfaketime.egg-info/top_level.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)      240 2020-04-17 16:03:10.000000 libfaketime-2.0.0/setup.cfg
--rw-rw-r--   0 simon     (1000) simon     (1000)     3702 2020-04-17 15:43:01.000000 libfaketime-2.0.0/setup.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2020-04-17 16:03:10.000000 libfaketime-2.0.0/test/
--rw-rw-r--   0 simon     (1000) simon     (1000)     3926 2019-01-19 22:34:06.000000 libfaketime-2.0.0/test/test_faketime.py
--rw-------   0 simon     (1000) simon     (1000)     1155 2017-09-10 20:17:06.000000 libfaketime-2.0.0/test/test_freezegun.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     2339 2020-04-17 15:43:01.000000 libfaketime-2.0.0/test/test_tz.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 14:22:40.264121 libfaketime-2.1.0/
+-rw-r--r--   0 simon     (1000) simon     (1000)     3532 2024-05-17 14:21:48.000000 libfaketime-2.1.0/CHANGELOG.md
+-rw-r--r--   0 simon     (1000) simon     (1000)    18026 2024-05-17 14:03:34.000000 libfaketime-2.1.0/LICENSE
+-rw-r--r--   0 simon     (1000) simon     (1000)      344 2024-05-17 14:03:34.000000 libfaketime-2.1.0/MANIFEST.in
+-rw-r--r--   0 simon     (1000) simon     (1000)    11440 2024-05-17 14:22:40.264121 libfaketime-2.1.0/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)     6810 2024-05-17 14:03:34.000000 libfaketime-2.1.0/README.md
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 14:22:40.254121 libfaketime-2.1.0/libfaketime/
+-rw-r--r--   0 simon     (1000) simon     (1000)     9740 2024-05-17 14:03:34.000000 libfaketime-2.1.0/libfaketime/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)       22 2024-05-17 14:16:57.000000 libfaketime-2.1.0/libfaketime/_version.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 14:22:40.254121 libfaketime-2.1.0/libfaketime/vendor/
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 14:22:40.264121 libfaketime-2.1.0/libfaketime/vendor/libfaketime/
+-rw-r--r--   0 simon     (1000) simon     (1000)    18092 2022-03-11 18:46:56.000000 libfaketime-2.1.0/libfaketime/vendor/libfaketime/COPYING
+-rw-r--r--   0 simon     (1000) simon     (1000)     1006 2024-05-17 14:06:16.000000 libfaketime-2.1.0/libfaketime/vendor/libfaketime/Makefile
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 14:22:40.264121 libfaketime-2.1.0/libfaketime/vendor/libfaketime/src/
+-rw-r--r--   0 simon     (1000) simon     (1000)     6404 2024-05-17 14:06:16.000000 libfaketime-2.1.0/libfaketime/vendor/libfaketime/src/Makefile
+-rw-r--r--   0 simon     (1000) simon     (1000)     3260 2024-05-17 14:06:16.000000 libfaketime-2.1.0/libfaketime/vendor/libfaketime/src/Makefile.OSX
+-rw-r--r--   0 simon     (1000) simon     (1000)    12653 2024-05-17 14:06:16.000000 libfaketime-2.1.0/libfaketime/vendor/libfaketime/src/faketime.c
+-rw-r--r--   0 simon     (1000) simon     (1000)     3199 2024-05-17 14:06:16.000000 libfaketime-2.1.0/libfaketime/vendor/libfaketime/src/faketime_common.h
+-rw-r--r--   0 simon     (1000) simon     (1000)   111547 2024-05-17 14:06:16.000000 libfaketime-2.1.0/libfaketime/vendor/libfaketime/src/libfaketime.c
+-rw-r--r--   0 simon     (1000) simon     (1000)      412 2024-05-17 14:06:16.000000 libfaketime-2.1.0/libfaketime/vendor/libfaketime/src/libfaketime.map
+-rw-r--r--   0 simon     (1000) simon     (1000)      220 2024-05-17 14:06:16.000000 libfaketime-2.1.0/libfaketime/vendor/libfaketime/src/sunos_endian.h
+-rw-r--r--   0 simon     (1000) simon     (1000)     5017 2024-05-17 14:06:16.000000 libfaketime-2.1.0/libfaketime/vendor/libfaketime/src/time_ops.h
+-rw-r--r--   0 simon     (1000) simon     (1000)    77489 2024-05-17 14:06:16.000000 libfaketime-2.1.0/libfaketime/vendor/libfaketime/src/uthash.h
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 14:22:40.264121 libfaketime-2.1.0/libfaketime.egg-info/
+-rw-r--r--   0 simon     (1000) simon     (1000)    11440 2024-05-17 14:22:40.000000 libfaketime-2.1.0/libfaketime.egg-info/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)      941 2024-05-17 14:22:40.000000 libfaketime-2.1.0/libfaketime.egg-info/SOURCES.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        1 2024-05-17 14:22:40.000000 libfaketime-2.1.0/libfaketime.egg-info/dependency_links.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       56 2024-05-17 14:22:40.000000 libfaketime-2.1.0/libfaketime.egg-info/entry_points.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        1 2024-05-17 14:08:13.000000 libfaketime-2.1.0/libfaketime.egg-info/not-zip-safe
+-rw-r--r--   0 simon     (1000) simon     (1000)       26 2024-05-17 14:22:40.000000 libfaketime-2.1.0/libfaketime.egg-info/requires.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       12 2024-05-17 14:22:40.000000 libfaketime-2.1.0/libfaketime.egg-info/top_level.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)      209 2024-05-17 14:03:34.000000 libfaketime-2.1.0/pyproject.toml
+-rw-r--r--   0 simon     (1000) simon     (1000)      327 2024-05-17 14:22:40.264121 libfaketime-2.1.0/setup.cfg
+-rw-r--r--   0 simon     (1000) simon     (1000)     3585 2024-05-17 14:16:06.000000 libfaketime-2.1.0/setup.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 14:22:40.264121 libfaketime-2.1.0/test/
+-rw-r--r--   0 simon     (1000) simon     (1000)     4733 2024-05-17 14:03:34.000000 libfaketime-2.1.0/test/test_faketime.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1188 2024-05-17 14:03:34.000000 libfaketime-2.1.0/test/test_freezegun.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     2395 2024-05-17 14:03:34.000000 libfaketime-2.1.0/test/test_tz.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `libfaketime-2.0.0/CHANGELOG.rst` & `libfaketime-2.1.0/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,120 +1,128 @@
-.. :changelog:
-
 Changelog
----------
+=========
+
+[Semantic versioning](http://semver.org/) is used.
+
+2.1.0
+-----
+released 2024-05-17
+
+Thanks for @azmeuk for all their contributions to this release!
 
-`Semantic versioning <http://semver.org/>`__ is used.
+- add support for timestamp files, which enables freezing time across subprocesses: [#78](https://github.com/simon-weber/python-libfaketime/pull/78)
+- upgrade underlying libfaketime to 0.9.10 without modifications: [#75](https://github.com/simon-weber/python-libfaketime/pull/75)
+- add a quiet param to rexec_if_needed: [#72](https://github.com/simon-weber/python-libfaketime/pull/72)
 
 2.0.0
-+++++
+-----
 released 2020-04-17
 
 - breaking: drop python 2.7 support
-- set LD_LIBRARY_PATH on linux to support paths containing spaces: `\#57 <https://github.com/simon-weber/python-libfaketime/pull/57>`__
-- fix compatibility with non-pytz tzinfo objects: `\#58 <https://github.com/simon-weber/python-libfaketime/pull/58>`__
+- set LD_LIBRARY_PATH on linux to support paths containing spaces: [#57](https://github.com/simon-weber/python-libfaketime/pull/57)
+- fix compatibility with non-pytz tzinfo objects: [#58](https://github.com/simon-weber/python-libfaketime/pull/58)
 
 1.2.1
-+++++
+-----
 released 2019-01-20
 
 - fix a deadlock on python 3.7+
 
 1.2.0
-+++++
+-----
 released 2018-10-28
 
-- offset-aware datetimes now properly fake the timezone as well: `\#49 <https://github.com/simon-weber/python-libfaketime/pull/49>`__
+- offset-aware datetimes now properly fake the timezone as well: [#49](https://github.com/simon-weber/python-libfaketime/pull/49)
 
 1.1.0
-+++++
+-----
 released 2018-10-07
 
-- decorated classes can access the fake_time object with ``self._faked_time``: `\#47 <https://github.com/simon-weber/python-libfaketime/pull/47>`__
+- decorated classes can access the fake_time object with ``self._faked_time``: [#47](https://github.com/simon-weber/python-libfaketime/pull/47)
 
 1.0.0
-+++++
+-----
 released 2018-06-16
 
-- **backwards incompatible**: the monotonic clock is no longer mocked: `\#45 <https://github.com/simon-weber/python-libfaketime/pull/45>`__
-- ensure TZ is set to a valid timezone: `\#46 <https://github.com/simon-weber/python-libfaketime/pull/46>`__
+- **backwards incompatible**: the monotonic clock is no longer mocked: [#45](https://github.com/simon-weber/python-libfaketime/pull/45)
+- ensure TZ is set to a valid timezone: [#46](https://github.com/simon-weber/python-libfaketime/pull/46)
 
 0.5.2
-+++++
+-----
 released 2018-05-19
 
-- fix a bug causing incorrect times after unpatching under python 3.6+: `\#43 <https://github.com/simon-weber/python-libfaketime/pull/43>`__
-- fix compilation under gcc8: `\#44 <https://github.com/simon-weber/python-libfaketime/pull/44>`__
+- fix a bug causing incorrect times after unpatching under python 3.6+: [#43](https://github.com/simon-weber/python-libfaketime/pull/43)
+- fix compilation under gcc8: [#44](https://github.com/simon-weber/python-libfaketime/pull/44)
 
 0.5.1
-+++++
+-----
 released 2018-01-19
 
-- fix usage as a class decorator : `\#41 <https://github.com/simon-weber/python-libfaketime/pull/41>`__
+- fix usage as a class decorator : [#41](https://github.com/simon-weber/python-libfaketime/pull/41)
 
 0.5.0
-+++++
+-----
 released 2017-09-10
 
-- alias fake_time for freeze_time: `\#31 <https://github.com/simon-weber/python-libfaketime/pull/31>`__
-- add tz_offset parameter: `\#36 <https://github.com/simon-weber/python-libfaketime/pull/36>`__
+- alias fake_time for freeze_time: [#31](https://github.com/simon-weber/python-libfaketime/pull/31)
+- add tz_offset parameter: [#36](https://github.com/simon-weber/python-libfaketime/pull/36)
 
 0.4.4
-+++++
+-----
 released 2017-07-16
 
-- allow contextlib2 as an alternative to contextdecorator: `\#30 <https://github.com/simon-weber/python-libfaketime/pull/30>`__
+- allow contextlib2 as an alternative to contextdecorator: [#30](https://github.com/simon-weber/python-libfaketime/pull/30)
 
 0.4.3
-+++++
+-----
 released 2017-07-07
 
-- add macOS Sierra compatibility: `\#29 <https://github.com/simon-weber/python-libfaketime/pull/29>`__
+- add macOS Sierra compatibility: [#29](https://github.com/simon-weber/python-libfaketime/pull/29)
 
 0.4.2
-+++++
+-----
 released 2016-06-30
 
-- fix only_main_thread=False: `\#24 <https://github.com/simon-weber/python-libfaketime/pull/24>`__
+- fix only_main_thread=False: [#24](https://github.com/simon-weber/python-libfaketime/pull/24)
 
 0.4.1
-+++++
+-----
 released 2016-05-02
 
-- fix deadlocks from uuid.uuid1 when faking time: `\#14 <https://github.com/simon-weber/python-libfaketime/pull/14>`__
-- remove contextdecorator dependency on python3: `\#15 <https://github.com/simon-weber/python-libfaketime/pull/15>`__
+- fix deadlocks from uuid.uuid1 when faking time: [#14](https://github.com/simon-weber/python-libfaketime/pull/14)
+- remove contextdecorator dependency on python3: [#15](https://github.com/simon-weber/python-libfaketime/pull/15)
 
 0.4.0
-+++++
+-----
 released 2016-04-02
 
-- freezegun's tick() is now supported; see `their docs <https://github.com/spulec/freezegun/blob/f1f5148720dd715cfd6dc03bf1861dbedfaad493/README.rst#manual-ticks>`__ for usage.
+- freezegun's tick() is now supported; see [their docs](https://github.com/spulec/freezegun/blob/f1f5148720dd715cfd6dc03bf1861dbedfaad493/README.rst#manual-ticks) for usage.
 
 0.3.0
-+++++
+-----
 released 2016-03-04
 
 - invoking ``libfaketime`` from the command line will now print the necessary environment to avoid a re-exec.
 
 0.2.1
-+++++
+-----
 released 2016-03-01
 
 - python 3 support
 
 0.1.1
-+++++
+-----
 released 2015-09-11
 
 - prevent distribution of test directory: https://github.com/simon-weber/python-libfaketime/pull/4
 
 0.1.0
-+++++
+-----
 released 2015-06-23
 
 - add global start/stop callbacks
 
 0.0.3
-+++++
+-----
 released 2015-03-28
 
 - initial packaged release
```

### Comparing `libfaketime-2.0.0/LICENSE` & `libfaketime-2.1.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -333,8 +333,7 @@
   Ty Coon, President of Vice
 
 This General Public License does not permit incorporating your program into
 proprietary programs.  If your program is a subroutine library, you may
 consider it more useful to permit linking proprietary applications with the
 library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.
-
```

### Comparing `libfaketime-2.0.0/README.rst` & `libfaketime-2.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,163 +1,196 @@
 python-libfaketime: fast date/time mocking
 ==========================================
 
-.. image:: https://img.shields.io/travis/simon-weber/python-libfaketime.svg
-        :target: https://travis-ci.org/simon-weber/python-libfaketime
-.. image:: https://img.shields.io/pypi/v/libfaketime.svg
-        :target: https://pypi.python.org/pypi/libfaketime
-.. image:: https://img.shields.io/badge/dynamic/json.svg?label=release&query=%24.status&maxAge=43200&uri=https%3A%2F%2Fwww.repominder.com%2Fbadge%2FeyJ1c2VyX2lkIjogMiwgInJlcG9faWQiOiA3OX0%3D%2F&link=https%3A%2F%2Fwww.repominder.com%2F
-        :target: https://www.repominder.com
+[![github actions](https://github.com/simon-weber/python-libfaketime/actions/workflows/tests.yaml/badge.svg)](https://github.com/simon-weber/python-libfaketime/actions/workflows/tests.yaml)
+[![pypi](https://img.shields.io/pypi/v/libfaketime.svg)](https://pypi.python.org/pypi/libfaketime)
+[![repominder](https://img.shields.io/badge/dynamic/json.svg?label=release&query=%24.status&maxAge=43200&uri=https%3A%2F%2Fwww.repominder.com%2Fbadge%2FeyJmdWxsX25hbWUiOiAic2ltb24td2ViZXIvcHl0aG9uLWxpYmZha2V0aW1lIn0%3D%2F&link=https%3A%2F%2Fwww.repominder.com%2F)](https://www.repominder.com)
 
-python-libfaketime is a wrapper of `libfaketime <https://github.com/wolfcw/libfaketime>`__ for python.
+python-libfaketime is a wrapper of [libfaketime](https://github.com/wolfcw/libfaketime) for python.
 Some brief details:
 
-* Linux and OS X, Pythons 3.5 through 3.8, pypy and pypy3
-* Mostly compatible with `freezegun <https://github.com/spulec/freezegun>`__.
+* Linux and OS X, Pythons 3.8 through 3.12, pypy and pypy3
+* Mostly compatible with [freezegun](https://github.com/spulec/freezegun).
 * Microsecond resolution.
 * Accepts datetimes and strings that can be parsed by dateutil.
 * Not threadsafe.
-* Will break profiling. A workaround: use ``libfaketime.{begin, end}_callback`` to disable/enable your profiler (`nosetest example <https://gist.github.com/simon-weber/8d43e33448684f85718417ce1a072bc8>`__).
+* Will break profiling. A workaround: use ``libfaketime.{begin, end}_callback`` to disable/enable your profiler ([nosetest example](https://gist.github.com/simon-weber/8d43e33448684f85718417ce1a072bc8)).
 
 
 Installation
 ------------
 
-.. code-block:: sh
-
-    $ pip install libfaketime
+```sh
+$ pip install libfaketime
+```
 
 Usage
 -----
 
-.. code-block:: python
+```python
+import datetime
+from libfaketime import fake_time, reexec_if_needed
 
-    import datetime
-    from libfaketime import fake_time, reexec_if_needed
+# libfaketime needs to be preloaded by the dynamic linker.
+# This will exec the same command, but with the proper environment variables set.
+# You can also skip this and manually manage your env (see "How to avoid re-exec").
+reexec_if_needed()
 
-    # libfaketime needs to be preloaded by the dynamic linker.
-    # This will exec the same command, but with the proper environment variables set.
-    # You can also skip this and manually manage your env (see "How to avoid re-exec").
-    reexec_if_needed()
+def test_datetime_now():
 
-    def test_datetime_now():
+    # fake_time can be used as a context_manager
+    with fake_time('1970-01-01 00:00:01'):
 
-        # fake_time can be used as a context_manager
-        with fake_time('1970-01-01 00:00:01'):
+        # Every calls to a date or datetime function returns the mocked date
+        assert datetime.datetime.utcnow() == datetime.datetime(1970, 1, 1, 0, 0, 1)
+        assert datetime.datetime.now() == datetime.datetime(1970, 1, 1, 0, 0, 1)
+        assert time.time() == 1
 
-            # Every calls to a date or datetime function returns the mocked date
-            assert datetime.datetime.utcnow() == datetime.datetime(1970, 1, 1, 0, 0, 1)
-            assert datetime.datetime.now() == datetime.datetime(1970, 1, 1, 0, 0, 1)
-            assert time.time() == 1
 
+# fake_time can also be used as a decorator
+@fake_time('1970-01-01 00:00:01', tz_offset=12)
+def test_datetime_now_with_offset():
 
-    # fake_time can also be used as a decorator
-    @fake_time('1970-01-01 00:00:01', tz_offset=12)
-    def test_datetime_now_with_offset():
+    # datetime.utcnow returns the mocked datetime without offset
+    assert datetime.datetime.utcnow() == datetime.datetime(1970, 1, 1, 0, 0, 1)
 
-        # datetime.utcnow returns the mocked datetime without offset
-        assert datetime.datetime.utcnow() == datetime.datetime(1970, 1, 1, 0, 0, 1)
+    # datetime.now returns the mocked datetime with the offset passed to fake_time
+    assert datetime.datetime.now() == datetime.datetime(1970, 1, 1, 12, 0, 1)
+```
 
-        # datetime.now returns the mocked datetime with the offset passed to fake_time
-        assert datetime.datetime.now() == datetime.datetime(1970, 1, 1, 12, 0, 1)
+### remove_vars
 
+By default, ``reexec_if_needed`` removes the ``LD_PRELOAD`` variable after the
+re-execution, to keep your environment as clean as possible. You might want it
+to stick around, for example when using parallelized tests that use subprocess
+like ``pytest-xdist``, and simply for tests where subprocess is called. To
+keep them around, pass ``remove_vars=False`` like:
 
-Performance
------------
+```python
+reexec_if_needed(remove_vars=False)
+```
 
-libfaketime tends to be significantly faster than `freezegun <https://github.com/spulec/freezegun>`__.
-Here's the output of a `totally unscientific benchmark <https://github.com/simon-weber/python-libfaketime/blob/master/benchmark.py>`__ on my laptop:
+### quiet
 
-.. code-block:: sh
+To avoid displaying the informative text when re-executing, you can set the
+`quiet` parameter:
 
-    $ python benchmark.py
-    re-exec with libfaketime dependencies
-    timing 1000 executions of <class 'libfaketime.fake_time'>
-    0.021755 seconds
-
-    $ python benchmark.py freezegun
-    timing 1000 executions of <function freeze_time at 0x10aaa1140>
-    6.561472 seconds
+```python
+reexec_if_needed(quiet=True)
+```
 
+### timestamp_file
 
-Use with py.test
-----------------
+A common time can be shared between several execution contexts by using a file
+to store the time to mock, instead of environment variables. This is useful
+to control the time of a running process for instance. Here is a schematized
+use case:
+
+```python
+reexec_if_needed(remove_vars=False)
+
+with fake_time("1970-01-01 00:00:00", timestamp_file="/tmp/timestamp"):
+    subprocess.run("/some/server/process")
 
-The `pytest-libfaketime <https://gitlab.com/yaal/pytest-libfaketime>`__ plugin will automatically configure python-libfaketime for you:
+with fake_time("2000-01-01 00:00:00", timestamp_file="/tmp/timestamp"):
+    assert request_the_server_process_date() == "2000-01-01 00:00:00"
+```
 
-.. code-block:: sh
+Performance
+-----------
 
-    $ pip install pytest-libfaketime
+libfaketime tends to be significantly faster than [freezegun](https://github.com/spulec/freezegun).
+Here's the output of a [totally unscientific benchmark](https://github.com/simon-weber/python-libfaketime/blob/master/benchmark.py) on my laptop:
 
+```sh
+$ python benchmark.py
+re-exec with libfaketime dependencies
+timing 1000 executions of <class 'libfaketime.fake_time'>
+0.021755 seconds
+
+$ python benchmark.py freezegun
+timing 1000 executions of <function freeze_time at 0x10aaa1140>
+6.561472 seconds
+```
 
-Alternatively, you can reexec manually from inside the pytest_configure hook:
+Use with py.test
+----------------
+
+The [pytest-libfaketime](https://github.com/pytest-dev/pytest-libfaketime) plugin will automatically configure python-libfaketime for you:
 
-.. code-block:: python
+```sh
+$ pip install pytest-libfaketime
+```
 
-    # conftest.py
-    import os
-    import libfaketime
-
-    def pytest_configure():
-        libfaketime.reexec_if_needed()
-        _, env_additions = libfaketime.get_reload_information()
-        os.environ.update(env_additions)
+Alternatively, you can reexec manually from inside the pytest_configure hook:
 
+```python
+# conftest.py
+import os
+import libfaketime
+
+def pytest_configure():
+    libfaketime.reexec_if_needed()
+    _, env_additions = libfaketime.get_reload_information()
+    os.environ.update(env_additions)
+```
 
 Use with tox
 ------------
 
 In your tox configuration file, under the ``testenv`` bloc, add the libfaketime environment variables to avoid re-execution:
 
-.. code-block::
-
-    setenv =
-        LD_PRELOAD = {envsitepackagesdir}/libfaketime/vendor/libfaketime/src/libfaketime.so.1
-        DONT_FAKE_MONOTONIC = 1
-        FAKETIME_DID_REEXEC = true
-
+```ini
+setenv =
+    LD_PRELOAD = {envsitepackagesdir}/libfaketime/vendor/libfaketime/src/libfaketime.so.1
+    DONT_FAKE_MONOTONIC = 1
+    FAKETIME_DID_REEXEC = true
+```
 
 Migration from freezegun
 ------------------------
 
 python-libfaketime should have the same behavior as freezegun when running on supported code. To migrate to it, you can run:
 
-.. code-block:: bash
-
-    find . -type f -name "*.py" -exec sed -i 's/freezegun/libfaketime/g' "{}" \;
-
+```bash
+find . -type f -name "*.py" -exec sed -i 's/freezegun/libfaketime/g' "{}" \;
+```
 
 How to avoid re-exec
 --------------------
 
 In some cases - especially when your tests start other processes - re-execing can cause unexpected problems. To avoid this, you can preload the necessary environment variables yourself. The necessary environment for your system can be found by running ``python-libfaketime`` on the command line:
 
-.. code-block:: sh
-
-    $ python-libfaketime
-    export LD_PRELOAD="/home/foo/<snip>/vendor/libfaketime/src/libfaketime.so.1"
-    export DONT_FAKE_MONOTONIC="1"
-    export FAKETIME_DID_REEXEC=true
+```sh
+$ python-libfaketime
+export LD_PRELOAD="/home/foo/<snip>/vendor/libfaketime/src/libfaketime.so.1"
+export DONT_FAKE_MONOTONIC="1"
+export FAKETIME_NO_CACHE="1"
+export FAKETIME_DID_REEXEC=true
+```
 
 You can easily put this in a script like:
 
-.. code-block:: sh
-
-    $ eval $(python-libfaketime)
-    $ pytest  # ...or any other code that imports libfaketime
-
+```sh
+$ eval $(python-libfaketime)
+$ pytest  # ...or any other code that imports libfaketime
+```
 
 Contributing and testing
 ------------------------
 
 Contributions are welcome! You should compile libfaketime before running tests:
 
-.. code-block:: bash
-
-    make -C libfaketime/vendor/libfaketime
+```bash
+git submodule init --update
+# For Linux:
+env FAKETIME_COMPILE_CFLAGS="-UFAKE_STAT -UFAKE_UTIME -UFAKE_SLEEP" make -C libfaketime/vendor/libfaketime
+# For macOS
+env make -C libfaketime/vendor/libfaketime
+```
 
 Then you can install requirements with ``pip install -r requirements.txt`` and use ``pytest`` and ``tox`` to run the tests.
 
 uuid1 deadlock
 --------------
 
 Calling ``uuid.uuid1()`` multiple times while in a fake_time context can result in a deadlock when an OS-level uuid library is available.
```

### Comparing `libfaketime-2.0.0/libfaketime/__init__.py` & `libfaketime-2.1.0/libfaketime/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,121 +1,109 @@
-from __future__ import print_function
-
-from copy import deepcopy
 import datetime
-import dateutil.parser
 import functools
 import inspect
 import os
-import platform
 import sys
 import threading
 import time
 import unittest
 import uuid
+from copy import deepcopy
 
-from pytz import utc, timezone
-
-try:
-    basestring
-except NameError:
-    basestring = (str, bytes)
-
-
-SIERRA_VERSION_TUPLE = (10, 12)
+import dateutil.parser
+from pytz import timezone
+from pytz import utc
 
-# When using reexec_if_needed, remove_vars=True and a test loader that purges sys.modules
-# (like nose), it can be tough to run reexec_if_needed only once.
+# When using reexec_if_needed, remove_vars=True and a test loader that purges
+# sys.modules (like nose), it can be tough to run reexec_if_needed only once.
 # This env var is set by reexec to ensure we don't reload more than once.
 
-_DID_REEXEC_VAR = 'FAKETIME_DID_REEXEC'
+_DID_REEXEC_VAR = "FAKETIME_DID_REEXEC"
+_FAKETIME_FMT = "%Y-%m-%d %T.%f"
 
 
 def _get_lib_path():
-    vendor_dir = 'libfaketime'
-
-    if sys.platform == "darwin":
-        version_tuple = tuple(int(x) for x in platform.mac_ver()[0].split('.'))
-        pre_sierra = version_tuple < SIERRA_VERSION_TUPLE
-        if pre_sierra:
-            vendor_dir = 'libfaketime-pre_sierra'
+    vendor_dir = "libfaketime"
 
     return os.path.join(
-        os.path.dirname(__file__),
-        os.path.join('vendor', vendor_dir, 'src'))
+        os.path.dirname(__file__), os.path.join("vendor", vendor_dir, "src")
+    )
 
 
 def _get_shared_lib(basename):
     return os.path.join(_get_lib_path(), basename)
 
 
 def _setup_ld_preload(soname):
-    if 'LD_PRELOAD' in os.environ:
-        preload = '{}:{}'.format(soname, os.environ['LD_PRELOAD'])
+    if "LD_PRELOAD" in os.environ:
+        preload = "{}:{}".format(soname, os.environ["LD_PRELOAD"])
     else:
         preload = soname
 
     return preload
 
 
 # keys are the first 5 chars since we don't care about the version.
 _lib_addition = {
-    'linux': {
-        'LD_LIBRARY_PATH': _get_lib_path(),
-        'LD_PRELOAD': _setup_ld_preload('libfaketime.so.1')
+    "linux": {
+        "LD_LIBRARY_PATH": _get_lib_path(),
+        "LD_PRELOAD": _setup_ld_preload("libfaketime.so.1"),
     },
-    'darwi': {
-        'DYLD_INSERT_LIBRARIES': _get_shared_lib('libfaketime.1.dylib'),
+    "darwi": {
+        "DYLD_INSERT_LIBRARIES": _get_shared_lib("libfaketime.1.dylib"),
     },
 }
 
 _other_additions = {
-    'linux': {
-        'DONT_FAKE_MONOTONIC': '1',
+    "linux": {
+        "DONT_FAKE_MONOTONIC": "1",
+        "FAKETIME_NO_CACHE": "1",
     },
-    'darwi': {
-        'DONT_FAKE_MONOTONIC': '1',
-        'DYLD_FORCE_FLAT_NAMESPACE': '1',
+    "darwi": {
+        "DONT_FAKE_MONOTONIC": "1",
+        "DYLD_FORCE_FLAT_NAMESPACE": "1",
+        "FAKETIME_NO_CACHE": "1",
     },
 }
 
 _env_additions = deepcopy(_lib_addition)
 for platform_name, d in list(_other_additions.items()):
     # Just doing a .update wouldn't merge the sub dictionaries.
     _env_additions[platform_name].update(d)
 
 
 def get_reload_information():
     try:
         env_additions = _env_additions[sys.platform[:5]]
     except KeyError:
-        raise RuntimeError("libfaketime does not support platform %s" % sys.platform)
+        raise RuntimeError(f"libfaketime does not support platform {sys.platform}")
 
-    needs_reload = os.environ.get(_DID_REEXEC_VAR) != 'true'
+    needs_reload = os.environ.get(_DID_REEXEC_VAR) != "true"
 
     return needs_reload, env_additions
 
 
 def main():  # pragma: nocover
     """Print the necessary environment to stdout."""
 
     _, _env_additions = get_reload_information()
     for key, value in _env_additions.items():
-        print('export %s="%s"' % (key, value))
-    print('export %s=true' % _DID_REEXEC_VAR)
+        print(f'export {key}="{value}"')
+    print(f"export {_DID_REEXEC_VAR}=true")
 
 
-def reexec_if_needed(remove_vars=True):
+def reexec_if_needed(remove_vars=True, quiet=False):
     needs_reload, env_additions = get_reload_information()
     if needs_reload:
         new_environ = os.environ.copy()
         new_environ.update(env_additions)
-        new_environ[_DID_REEXEC_VAR] = 'true'
+        new_environ[_DID_REEXEC_VAR] = "true"
         args = [sys.executable, [sys.executable] + sys.argv, new_environ]
-        print('re-exec with libfaketime dependencies')
+        if not quiet:
+            print("re-exec with libfaketime dependencies")
         os.execve(*args)
 
     if remove_vars:
         for key in env_additions:
             if key in os.environ:
                 del os.environ[key]
 
@@ -127,66 +115,98 @@
 
 def end_callback(instance):
     """Called just after finished faking the time."""
     pass
 
 
 class fake_time:
-    def __init__(self, datetime_spec, only_main_thread=True, tz_offset=None):
+    def __init__(
+        self,
+        datetime_spec=None,
+        only_main_thread=True,
+        tz_offset=None,
+        timestamp_file=None,
+    ):
         self.only_main_thread = only_main_thread
-        self.timezone_str = 'UTC'
+        self.timezone_str = "UTC"
         if tz_offset is not None:
-            self.timezone_str = 'Etc/GMT{0:+}'.format(-tz_offset)
+            self.timezone_str = f"Etc/GMT{-tz_offset:+}"
+
+        if not datetime_spec and not timestamp_file:
+            raise ValueError(
+                "Either 'datetime_spec' or 'timestamp_file' must be passed."
+            )
 
         self.time_to_freeze = datetime_spec
-        if isinstance(datetime_spec, basestring):
-            self.time_to_freeze = utc.localize(dateutil.parser.parse(datetime_spec)) \
-                .astimezone(timezone(self.timezone_str))
+        self.timestamp_file = timestamp_file
+
+        if isinstance(datetime_spec, str):
+            self.time_to_freeze = utc.localize(
+                dateutil.parser.parse(datetime_spec)
+            ).astimezone(timezone(self.timezone_str))
         elif isinstance(datetime_spec, datetime.datetime):
             if datetime_spec.tzinfo:
                 if tz_offset is not None:
-                    raise Exception('Cannot set tz_offset when datetime already has timezone')
+                    raise Exception(
+                        "Cannot set tz_offset when datetime already has timezone"
+                    )
                 self.timezone_str = datetime_spec.tzinfo.tzname(datetime_spec)
 
     def _should_fake(self):
-        return not self.only_main_thread or threading.current_thread().name == 'MainThread'
+        return (
+            not self.only_main_thread or threading.current_thread().name == "MainThread"
+        )
 
     _uuid_func_names = (
         # < 3.7
-        '_uuid_generate_time',
+        "_uuid_generate_time",
         # 3.7+
-        '_generate_time_safe', '_generate_time')
+        "_generate_time_safe",
+        "_generate_time",
+    )
 
     def _should_patch_uuid(self):
         # Return the name of the uuid time generate function, or None if not present.
         # This must be patched to avoid uuid1 deadlocks in OS uuid libraries.
         if self._should_fake() and not self._prev_spec:
             for func_name in self._uuid_func_names:
                 if hasattr(uuid, func_name):
                     return func_name
 
         return None
 
     def _format_datetime(self, _datetime):
-        return _datetime.strftime('%Y-%m-%d %T %f')
+        return _datetime.strftime(_FAKETIME_FMT)
+
+    def _update_time(self, time):
+        if not self.timestamp_file:
+            os.environ["FAKETIME"] = self._format_datetime(time)
+        else:
+            if time:
+                with open(self.timestamp_file, "w") as fd:
+                    fd.write(self._format_datetime(time))
+            os.environ["FAKETIME_TIMESTAMP_FILE"] = self.timestamp_file
 
     def tick(self, delta=datetime.timedelta(seconds=1)):
         self.time_to_freeze += delta
-        os.environ['FAKETIME'] = self._format_datetime(self.time_to_freeze)
+        self._update_time(self.time_to_freeze)
 
     def __enter__(self):
         if self._should_fake():
             begin_callback(self)
-            self._prev_spec = os.environ.get('FAKETIME')
-            self._prev_tz = os.environ.get('TZ')
+            self._prev_spec = os.environ.get("FAKETIME")
+            self._prev_tz = os.environ.get("TZ")
+            self._prev_fmt = os.environ.get("FAKETIME_FMT")
+            self._prev_timestamp_file = os.environ.get("FAKETIME_TIMESTAMP_FILE")
 
-            os.environ['TZ'] = self.timezone_str
+            os.environ["TZ"] = self.timezone_str
 
             time.tzset()
-            os.environ['FAKETIME'] = self._format_datetime(self.time_to_freeze)
+            self._update_time(self.time_to_freeze)
+            os.environ["FAKETIME_FMT"] = _FAKETIME_FMT
 
         func_name = self._should_patch_uuid()
         if func_name:
             self._backup_uuid_generate_time = getattr(uuid, func_name)
             setattr(uuid, func_name, None)
 
         return self
@@ -194,24 +214,37 @@
     def __exit__(self, *exc):
         func_name = self._should_patch_uuid()
         if func_name:
             setattr(uuid, func_name, self._backup_uuid_generate_time)
 
         if self._should_fake():
             if self._prev_tz is not None:
-                os.environ['TZ'] = self._prev_tz
+                os.environ["TZ"] = self._prev_tz
             else:
-                del os.environ['TZ']
+                del os.environ["TZ"]
             time.tzset()
 
-            if self._prev_spec is not None:
-                os.environ['FAKETIME'] = self._prev_spec
+            if self.timestamp_file:
+                if self._prev_timestamp_file is not None:
+                    os.environ["FAKETIME_TIMESTAMP_FILE"] = self._prev_timestamp_file
+                elif "FAKETIME_TIMESTAMP_FILE" in os.environ:
+                    del os.environ["FAKETIME_TIMESTAMP_FILE"]
+
+            else:
+                if self._prev_spec is not None:
+                    os.environ["FAKETIME"] = self._prev_spec
+                else:
+                    del os.environ["FAKETIME"]
+
+            if self._prev_fmt is not None:
+                os.environ["FAKETIME_FMT"] = self._prev_spec
             else:
-                del os.environ['FAKETIME']
-                end_callback(self)
+                del os.environ["FAKETIME_FMT"]
+
+            end_callback(self)
 
         return False
 
     # Freezegun compatibility.
     start = __enter__
     stop = __exit__
 
@@ -224,17 +257,16 @@
         return self.decorate_callable(func)
 
     def decorate_class(self, klass):
         if issubclass(klass, unittest.TestCase):
             # If it's a TestCase, we assume you want to freeze the time for the
             # tests, from setUpClass to tearDownClass
 
-            # Use getattr as in Python 2.6 they are optional
-            orig_setUpClass = getattr(klass, 'setUpClass', None)
-            orig_tearDownClass = getattr(klass, 'tearDownClass', None)
+            orig_setUpClass = getattr(klass, "setUpClass", None)
+            orig_tearDownClass = getattr(klass, "tearDownClass", None)
 
             @classmethod
             def setUpClass(cls):
                 self.start()
                 if orig_setUpClass is not None:
                     orig_setUpClass()
 
@@ -244,44 +276,45 @@
                     orig_tearDownClass()
                 self.stop()
 
             klass.setUpClass = setUpClass
             klass.tearDownClass = tearDownClass
 
         else:
-
             seen = set()
 
-            klasses = klass.mro() if hasattr(klass, 'mro') else [klass] + list(klass.__bases__)
+            klasses = (
+                klass.mro()
+                if hasattr(klass, "mro")
+                else [klass] + list(klass.__bases__)
+            )
             for base_klass in klasses:
-                for (attr, attr_value) in base_klass.__dict__.items():
-                    if attr.startswith('_') or attr in seen:
+                for attr, attr_value in base_klass.__dict__.items():
+                    if attr.startswith("_") or attr in seen:
                         continue
                     seen.add(attr)
 
                     if not callable(attr_value) or inspect.isclass(attr_value):
                         continue
 
                     try:
                         setattr(klass, attr, self(attr_value))
                     except (AttributeError, TypeError):
-                        # Sometimes we can't set this for built-in types and custom callables
+                        # Sometimes we can't set this for built-in types and
+                        # custom callables
                         continue
 
         klass._faked_time = self
         return klass
 
     def decorate_callable(self, func):
         def wrapper(*args, **kwargs):
             with self:
                 result = func(*args, **kwargs)
             return result
-        functools.update_wrapper(wrapper, func)
 
-        # update_wrapper already sets __wrapped__ in Python 3.2+, this is only
-        # needed for Python 2.x support
-        wrapper.__wrapped__ = func
+        functools.update_wrapper(wrapper, func)
 
         return wrapper
 
 
 freeze_time = fake_time
```

### Comparing `libfaketime-2.0.0/libfaketime/vendor/libfaketime/COPYING` & `libfaketime-2.1.0/libfaketime/vendor/libfaketime/COPYING`

 * *Files identical despite different names*

### Comparing `libfaketime-2.0.0/libfaketime/vendor/libfaketime/Makefile` & `libfaketime-2.1.0/libfaketime/vendor/libfaketime/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 INSTALL ?= install
 
 UNAME=$(shell uname)
 SELECTOR:=$(shell if test "${UNAME}" = "Darwin" ; then echo "-f Makefile.OSX" ; fi)
+PREFIX ?= /usr/local
 
 all:
 	$(MAKE) $(SELECTOR) -C src all
 
 test:
+	$(MAKE) $(SELECTOR) -C src all
 	$(MAKE) $(SELECTOR) -C test all
 
 install:
 	$(MAKE) $(SELECTOR) -C src install
 	$(MAKE) $(SELECTOR) -C man install
 	$(INSTALL) -dm0755 "${DESTDIR}${PREFIX}/share/doc/faketime/"
 	$(INSTALL) -m0644 README "${DESTDIR}${PREFIX}/share/doc/faketime/README"
```

### Comparing `libfaketime-2.0.0/libfaketime/vendor/libfaketime/src/Makefile.OSX` & `libfaketime-2.1.0/libfaketime/vendor/libfaketime/src/Makefile.OSX`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 #
 # Notes:
 #
 #   * Compilation Defines:
 #
+#     MACOS_DYLD_INTERPOSE
+#         - Use dlyd interposing instead of name-based function interception
+#           (required since macOS Monterey)
+#
+#     FAKE_SLEEP
+#         - Also intercept sleep(), nanosleep(), usleep(), alarm(), [p]poll()
+#
+#     FAKE_SETTIME
+#         - Intercept clock_settime(), settimeofday(), and adjtime()
+#
+#     FAKE_PID
+#         - Enable faked values for getpid() calls through FAKETIME_FAKEPID
+#
+#     FAKE_RANDOM
+#         - Intercept getentropy(). Dangerous for production use.
+#           See README about FAKE_RANDOM.
+#
 #     FAKE_STAT
 #         - Enables time faking also for files' timestamps.
 #
-#     NO_ATFILE
-#         - Disables support for the fstatat() group of functions
+#     FAKE_FILE_TIMESTAMPS, FAKE_UTIME
+#         - Enables time faking for the utime* functions.  If enabled via
+#           FAKE_FILE_TIMESTAMPS, the faking is opt-in at runtime using
+#           with the FAKE_UTIME environment variable. If enabled via
+#           FAKE_UTIME, the faking is opt-out at runtime. Requires FAKE_STAT.
 #
 #     PTHREAD
 #         - Define this to enable multithreading support.
 #
 #     PTHREAD_SINGLETHREADED_TIME
 #         - Define this if you want to single-thread time() ... there ARE
 #           possible caching side-effects in a multithreaded environment
 #           without this, but the performance impact may require you to
 #           try it unsynchronized.
 #
-# 	  FAKE_SLEEP
-# 	      - Also intercept sleep(), nanosleep(), usleep(), alarm(), [p]poll()
-#
 #   * Compilation addition: second libMT target added for building the pthread-
 #     enabled library as a separate library
 #
 #   * Compilation switch change: previous versions compiled using '-nostartfiles'
 #     This is no longer the case since there is a 'startup' constructor for the library
 #     which is used to activate the start-at times when specified. This also initializes
 #     the dynamic disabling of the FAKE_STAT calls.
@@ -34,16 +51,16 @@
 #
 # default to clang to support thread local variables
 CC ?= clang
 INSTALL ?= install
 
 PREFIX ?= /usr/local
 
-CFLAGS += -DFAKE_SLEEP -DFAKE_INTERNAL_CALLS -DPREFIX='"'${PREFIX}'"'
-LIB_LDFLAGS += -dynamiclib -current_version 0.9.7 -compatibility_version 0.7
+CFLAGS += -DFAKE_SLEEP -DFAKE_INTERNAL_CALLS -DPREFIX='"'${PREFIX}'"' $(FAKETIME_COMPILE_CFLAGS) -DMACOS_DYLD_INTERPOSE -DFAKE_SETTIME
+LIB_LDFLAGS += -dynamiclib -current_version 0.9.10 -compatibility_version 0.7
 
 SONAME = 1
 LIBS = libfaketime.${SONAME}.dylib
 BINS = faketime
 
 all: ${LIBS} ${BINS}
```

### Comparing `libfaketime-2.0.0/libfaketime/vendor/libfaketime/src/faketime.c` & `libfaketime-2.1.0/libfaketime/vendor/libfaketime/src/faketime.c`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  *  libfaketime wrapper command
  *
- *  This file is part of libfaketime, version 0.9.7
+ *  This file is part of libfaketime, version 0.9.10
  *
  *  libfaketime is free software; you can redistribute it and/or modify it
  *  under the terms of the GNU General Public License v2 as published by the
  *  Free Software Foundation.
  *
  *  libfaketime is distributed in the hope that it will be useful, but WITHOUT
  *  ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
@@ -44,17 +44,17 @@
 #include <sys/types.h>
 #include <sys/wait.h>
 #include <sys/mman.h>
 #include <semaphore.h>
 
 #include "faketime_common.h"
 
-const char version[] = "0.9.7";
+const char version[] = "0.9.10";
 
-#ifdef __APPLE__
+#if (defined __APPLE__) || (defined __sun)
 static const char *date_cmd = "gdate";
 #else
 static const char *date_cmd = "date";
 #endif
 
 #define PATH_BUFSIZE 4096
 
@@ -71,14 +71,18 @@
   "The clock will continue to run from this timestamp. Please see the manpage (man faketime)\n"
   "for advanced options, such as stopping the wall clock and make it run faster or slower.\n"
   "\n"
   "The optional switches are:\n"
   "  -m                  : Use the multi-threaded version of libfaketime\n"
   "  -f                  : Use the advanced timestamp specification format (see manpage)\n"
   "  --exclude-monotonic : Prevent monotonic clock from drifting (not the raw monotonic one)\n"
+#ifdef FAKE_PID
+  "  -p PID              : Pretend that the program's process ID is PID\n"
+#endif
+  "  --date-prog PROG    : Use specified GNU-compatible implementation of 'date' program\n"
   "\n"
   "Examples:\n"
   "%s 'last friday 5 pm' /bin/date\n"
   "%s '2008-12-24 08:15:42' /bin/date\n"
   "%s -f '+2,5y x10,0' /bin/bash -c 'date; while true; do echo $SECONDS ; sleep 1 ; done'\n"
   "%s -f '+2,5y x0,50' /bin/bash -c 'date; while true; do echo $SECONDS ; sleep 1 ; done'\n"
   "%s -f '+2,5y i2,0' /bin/bash -c 'date; while true; do date; sleep 1 ; done'\n"
@@ -89,49 +93,81 @@
 }
 
 /** Clean up shared objects */
 static void cleanup_shobjs()
 {
   if (-1 == sem_unlink(sem_name))
   {
-    perror("sem_unlink");
+    perror("faketime: sem_unlink");
   }
   if (-1 == shm_unlink(shm_name))
   {
-    perror("shm_unlink");
+    perror("faketime: shm_unlink");
   }
 }
 
 int main (int argc, char **argv)
 {
   pid_t child_pid;
   int curr_opt = 1;
   bool use_mt = false, use_direct = false;
   long offset;
+  bool fake_pid = false;
+  const char *pid_val;
 
-  while(curr_opt < argc)
+#ifndef SILENT
+  if (getenv("FAKETIME") || getenv("FAKETIME_SHARED") || getenv("FAKETIME_FAKEPID") || getenv("FAKERANDOM_SEED")) {
+    fprintf(stderr, "faketime: You appear to be running faketime within a libfaketime environment. Proceeding, but check for unexpected results...\n");
+  }
+#endif
+
+  while (curr_opt < argc)
   {
     if (0 == strcmp(argv[curr_opt], "-m"))
     {
       use_mt = true;
       curr_opt++;
       continue;
     }
+    if (0 == strcmp(argv[curr_opt], "-p"))
+    {
+      fake_pid = true;
+      pid_val = argv[curr_opt + 1];
+      curr_opt += 2;
+#ifndef FAKE_PID
+      fprintf(stderr, "faketime: -p argument probably won't work (try rebuilding with -DFAKE_PID)\n");
+#endif
+      continue;
+    }
     else if (0 == strcmp(argv[curr_opt], "-f"))
     {
       use_direct = true;
       curr_opt++;
       continue;
     }
     else if (0 == strcmp(argv[curr_opt], "--exclude-monotonic"))
     {
-      setenv("DONT_FAKE_MONOTONIC", "1", true);
+      setenv("FAKETIME_DONT_FAKE_MONOTONIC", "1", true);
       curr_opt++;
       continue;
     }
+    else if (0 == strcmp(argv[curr_opt], "--date-prog"))
+    {
+      curr_opt++;
+      if (curr_opt > argc) {
+        // At best this avoids a segfault reading beyond the argv[]
+        // Realistically there would be other args (e.g. program to call)
+        fprintf(stderr, "faketime: --date-prog requires a further argument\n");
+      } else {
+        date_cmd = argv[curr_opt];
+        curr_opt++;
+        //fprintf(stderr, "faketime: --date-prog assigned: %s\n", date_cmd);
+      }
+      continue;
+    }
     else if ((0 == strcmp(argv[curr_opt], "-v")) ||
              (0 == strcmp(argv[curr_opt], "--version")))
     {
       printf("\n%s: Version %s\n"
          "For usage information please use '%s --help'.\n",
          argv[0], version, argv[0]);
       exit(EXIT_SUCCESS);
@@ -165,17 +201,18 @@
     int ret = EXIT_SUCCESS;
 
     if (0 == (child_pid = fork()))
     {
       close(1);       /* close normal stdout */
       (void) (dup(pfds[1]) + 1);   /* make stdout same as pfds[1] */
       close(pfds[0]); /* we don't need this */
+      // fprintf(stderr, "faketime: using --date-prog: %s\n", date_cmd);
       if (EXIT_SUCCESS != execlp(date_cmd, date_cmd, "-d", argv[curr_opt], "+%s",(char *) NULL))
       {
-        perror("Running (g)date failed");
+        perror("faketime: Running (g)date failed");
         exit(EXIT_FAILURE);
       }
     }
     else
     {
       char buf[256] = {0}; /* e will have way less than 256 digits */
       close(pfds[1]);   /* we won't write to this */
@@ -194,14 +231,16 @@
     }
   }
   else
   {
     /* simply pass format string along */
     setenv("FAKETIME", argv[curr_opt], true);
   }
+  if (fake_pid)
+    setenv("FAKETIME_FAKEPID", pid_val, true);
   int keepalive_fds[2];
   (void) (pipe(keepalive_fds) + 1);
 
   /* we just consumed the timestamp option */
   curr_opt++;
 
   {
@@ -219,49 +258,50 @@
      * the need for crazy #ifdefs.
      */
     snprintf(sem_name, PATH_BUFSIZE -1 ,"/faketime_sem_%ld", (long)getpid());
     snprintf(shm_name, PATH_BUFSIZE -1 ,"/faketime_shm_%ld", (long)getpid());
 
     if (SEM_FAILED == (sem = sem_open(sem_name, O_CREAT|O_EXCL, S_IWUSR|S_IRUSR, 1)))
     {
-      perror("sem_open");
+      perror("faketime: sem_open");
+      fprintf(stderr, "The faketime wrapper only works on platforms that support the sem_open()\nsystem call. However, you may LD_PRELOAD libfaketime without using this wrapper.\n");
       exit(EXIT_FAILURE);
     }
 
     /* create shm */
     if (-1 == (shm_fd = shm_open(shm_name, O_CREAT|O_EXCL|O_RDWR, S_IWUSR|S_IRUSR)))
     {
-      perror("shm_open");
+      perror("faketime: shm_open");
       if (-1 == sem_unlink(argv[2]))
       {
-        perror("sem_unlink");
+        perror("faketime: sem_unlink");
       }
       exit(EXIT_FAILURE);
     }
 
     /* set shm size */
     if (-1 == ftruncate(shm_fd, sizeof(uint64_t)))
     {
-      perror("ftruncate");
+      perror("faketime: ftruncate");
       cleanup_shobjs();
       exit(EXIT_FAILURE);
     }
 
     /* map shm */
     if (MAP_FAILED == (ft_shared = mmap(NULL, sizeof(struct ft_shared_s), PROT_READ|PROT_WRITE,
                         MAP_SHARED, shm_fd, 0)))
     {
-      perror("mmap");
+      perror("faketime: mmap");
       cleanup_shobjs();
       exit(EXIT_FAILURE);
     }
 
     if (sem_wait(sem) == -1)
     {
-      perror("sem_wait");
+      perror("faketime: sem_wait");
       cleanup_shobjs();
       exit(EXIT_FAILURE);
     }
 
     /* init elapsed time ticks to zero */
     ft_shared->ticks = 0;
     ft_shared->file_idx = 0;
@@ -270,22 +310,22 @@
     ft_shared->start_time.mon.tv_sec = 0;
     ft_shared->start_time.mon.tv_nsec = -1;
     ft_shared->start_time.mon_raw.tv_sec = 0;
     ft_shared->start_time.mon_raw.tv_nsec = -1;
 
     if (-1 == munmap(ft_shared, (sizeof(struct ft_shared_s))))
     {
-      perror("munmap");
+      perror("faketime: munmap");
       cleanup_shobjs();
       exit(EXIT_FAILURE);
     }
 
     if (sem_post(sem) == -1)
     {
-      perror("semop");
+      perror("faketime: semop");
       cleanup_shobjs();
       exit(EXIT_FAILURE);
     }
 
     snprintf(shared_objs, sizeof(shared_objs), "%s %s", sem_name, shm_name);
     setenv("FAKETIME_SHARED", shared_objs, true);
     sem_close(sem);
@@ -340,17 +380,18 @@
 #endif
   }
 
   /* run command and clean up shared objects */
   if (0 == (child_pid = fork()))
   {
     close(keepalive_fds[0]); /* only parent needs to read this */
+    // fprintf(stderr, "faketime: Executing: %s\n", argv[curr_opt]);
     if (EXIT_SUCCESS != execvp(argv[curr_opt], &argv[curr_opt]))
     {
-      perror("Running specified command failed");
+      perror("faketime: Running specified command failed");
       exit(EXIT_FAILURE);
     }
   }
   else
   {
     int ret;
     char buf;
```

### Comparing `libfaketime-2.0.0/libfaketime/vendor/libfaketime/src/time_ops.h` & `libfaketime-2.1.0/libfaketime/vendor/libfaketime/src/time_ops.h`

 * *Files 4% similar despite different names*

```diff
@@ -56,17 +56,17 @@
       --(result)->tv_sec;                                           \
       (result)->tv_##prefix##sec += SEC_TO_##prefix##SEC;           \
     }                                                               \
   } while (0)
 #define timermul2(tvp, c, result, prefix)                           \
   do                                                                \
   {                                                                 \
-    long long tmp_time;                                             \
-    tmp_time = (c) * ((tvp)->tv_sec * SEC_TO_##prefix##SEC +        \
-               (tvp)->tv_##prefix##sec);                            \
+    int64_t tmp_time;                                             \
+    tmp_time = (c) * (int64_t) ((int64_t) (tvp)->tv_sec * SEC_TO_##prefix##SEC +        \
+               (int64_t) (tvp)->tv_##prefix##sec);                            \
     (result)->tv_##prefix##sec = tmp_time % SEC_TO_##prefix##SEC;   \
     (result)->tv_sec = (tmp_time - (result)->tv_##prefix##sec) /    \
       SEC_TO_##prefix##SEC;                                         \
     if ((result)->tv_##prefix##sec < 0)                             \
     {                                                               \
       (result)->tv_##prefix##sec +=  SEC_TO_##prefix##SEC;          \
       (result)->tv_sec -= 1;                                        \
@@ -85,20 +85,32 @@
 #endif
 #ifndef timeradd
 #define timeradd(a, b, result) timeradd2(a, b, result, u)
 #endif
 #ifndef timersub
 #define timersub(a, b, result) timersub2(a, b, result, u)
 #endif
-#ifndef timersub
+#ifndef timermul
 #define timermul(a, c, result) timermul2(a, c, result, u)
 #endif
 
 /* ops for nanosecs */
+#ifndef timespecisset
 #define timespecisset(tvp) timerisset2(tvp,n)
+#endif
+#ifndef timespecclear
 #define timespecclear(tvp) timerclear2(tvp, n)
+#endif
+#ifndef timespeccmp
 #define timespeccmp(a, b, CMP) timercmp2(a, b, CMP, n)
+#endif
+#ifndef timespecadd
 #define timespecadd(a, b, result) timeradd2(a, b, result, n)
+#endif
+#ifndef timespecsub
 #define timespecsub(a, b, result) timersub2(a, b, result, n)
+#endif
+#ifndef timespecmul
 #define timespecmul(a, c, result) timermul2(a, c, result, n)
+#endif
 
 #endif
```

### Comparing `libfaketime-2.0.0/libfaketime/vendor/libfaketime/src/uthash.h` & `libfaketime-2.1.0/libfaketime/vendor/libfaketime/src/uthash.h`

 * *Files identical despite different names*

### Comparing `libfaketime-2.0.0/setup.py` & `libfaketime-2.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,112 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 import os
-import platform
 import re
-from setuptools import setup, find_packages
-from setuptools.command.install import install
 import subprocess
 import sys
 
-
-# libfaketime broke compatibility with osx before sierra.
-# We keep a separate submodule for each and choose between them dynamically.
-SIERRA_VERSION_TUPLE = (10, 12)
+from setuptools import find_packages
+from setuptools import setup
+from setuptools.command.install import install
 
 # This hack is from http://stackoverflow.com/a/7071358/1231454;
 # the version is kept in a seperate file and gets parsed - this
 # way, setup.py doesn't have to import the package.
 
-VERSIONFILE = 'libfaketime/_version.py'
+VERSIONFILE = "libfaketime/_version.py"
 
 version_line = open(VERSIONFILE).read()
 version_re = r"^__version__ = ['\"]([^'\"]*)['\"]"
 match = re.search(version_re, version_line, re.M)
 if match:
     version = match.group(1)
 else:
-    raise RuntimeError("Could not find version in '%s'" % VERSIONFILE)
+    raise RuntimeError(f"Could not find version in '{VERSIONFILE}'")
 
 
-_vendor_path = 'libfaketime/vendor/libfaketime'
+_vendor_path = "libfaketime/vendor/libfaketime"
 if sys.platform == "linux" or sys.platform == "linux2":
-    libname = 'libfaketime.so.1'
+    libname = "libfaketime.so.1"
 elif sys.platform == "darwin":
-    libname = 'libfaketime.1.dylib'
-
-    version_tuple = tuple(int(x) for x in platform.mac_ver()[0].split('.'))
-    pre_sierra = version_tuple < SIERRA_VERSION_TUPLE
-    if pre_sierra:
-        _vendor_path = 'libfaketime/vendor/libfaketime-pre_sierra'
-
-    print("OSX version is %s-sierra: %r" % ('pre' if pre_sierra else 'post', version_tuple))
+    libname = "libfaketime.1.dylib"
 
 else:
-    raise RuntimeError("libfaketime does not support platform %s" % sys.platform)
+    raise RuntimeError("libfaketime does not support platform {sys.platform}")
 
-faketime_lib = os.path.join(_vendor_path, 'src', libname)
+faketime_lib = os.path.join(_vendor_path, "src", libname)
 
 
 class CustomInstall(install):
     def run(self):
         self.my_outputs = []
-        subprocess.check_call(['make', '-C', _vendor_path])
+        if sys.platform in ("linux", "linux2"):
+            subprocess.check_call(
+                [
+                    "env",
+                    "FAKETIME_COMPILE_CFLAGS=-UFAKE_STAT -UFAKE_UTIME -UFAKE_SLEEP",
+                    "make",
+                    "-C",
+                    _vendor_path,
+                ]
+            )
+        elif sys.platform == "darwin":
+            subprocess.check_call(["make", "-C", _vendor_path])
 
         dest = os.path.join(self.install_purelib, os.path.dirname(faketime_lib))
         try:
             os.makedirs(dest)
         except OSError as e:
             if e.errno != 17:
                 raise
-        print(faketime_lib, '->', dest)
+        print(faketime_lib, "->", dest)
         self.copy_file(faketime_lib, dest)
         self.my_outputs.append(os.path.join(dest, libname))
 
         install.run(self)
 
     def get_outputs(self):
         outputs = install.get_outputs(self)
         outputs.extend(self.my_outputs)
         return outputs
 
+
 setup(
-    name='libfaketime',
+    name="libfaketime",
     version=version,
-    author='Simon Weber',
-    author_email='simon@simonmweber.com',
-    url='http://pypi.python.org/pypi/libfaketime/',
-    packages=find_packages(exclude=['test']),
+    author="Simon Weber",
+    author_email="simon@simonmweber.com",
+    url="http://pypi.python.org/pypi/libfaketime/",
+    packages=find_packages(exclude=["test"]),
     scripts=[],
-    license='GPLv2',
-    description='A fast alternative to freezegun that wraps libfaketime.',
-    long_description=(open('README.rst').read() + '\n\n' +
-                      open('CHANGELOG.rst').read()),
+    license="GPLv2",
+    description="A fast alternative to freezegun that wraps libfaketime.",
+    long_description=(open("README.md").read() + "\n\n" + open("CHANGELOG.md").read()),
+    long_description_content_type="text/markdown",
     install_requires=[
-        'python-dateutil >= 1.3, != 2.0',         # 2.0 is python3-only
-        'pytz',                                   # for pytz.timezone and pytz.utc
+        "python-dateutil >= 1.3",
+        "pytz",  # for pytz.timezone and pytz.utc
     ],
     classifiers=[
-        'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy',
-        'Topic :: Software Development :: Libraries :: Python Modules',
+        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
+        "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     include_package_data=True,
     zip_safe=False,
-    cmdclass={'install': CustomInstall},
+    cmdclass={"install": CustomInstall},
     entry_points={
-        'console_scripts': [
-            'python-libfaketime = libfaketime:main',
+        "console_scripts": [
+            "python-libfaketime = libfaketime:main",
         ]
     },
 )
```

### Comparing `libfaketime-2.0.0/test/test_faketime.py` & `libfaketime-2.1.0/test/test_faketime.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,110 +1,128 @@
 import datetime
-import time
 import os
+import time
 import uuid
+from unittest.mock import patch
 
-from mock import patch
 import pytest
 
 import libfaketime
-from libfaketime import fake_time, freeze_time
+from libfaketime import fake_time
+from libfaketime import freeze_time
 
 
-class TestReexec():
-    @patch('os.execve')
-    @patch('sys.platform', 'win32')
+class TestReexec:
+    @patch("os.execve")
+    @patch("sys.platform", "win32")
     def test_reexec_windows_fails(self, exec_patch):
         with pytest.raises(RuntimeError):
             libfaketime.reexec_if_needed()
 
 
-class TestFaketime():
+class TestFaketime:
     def _assert_time_not_faked(self):
         # This just makes sure that non-faked time is dynamic;
         # I can't think of a good way to check that the non-faked time is "real".
 
         first = datetime.datetime.now().microsecond
         time.sleep(0.000001)
         second = datetime.datetime.now().microsecond
 
         assert second > first
 
     def test_fake_time_tick(self):
-        with fake_time('2000-01-01 10:00:05') as fake:
+        with fake_time("2000-01-01 10:00:05") as fake:
             assert datetime.datetime(2000, 1, 1, 10, 0, 5) == datetime.datetime.now()
             fake.tick(delta=datetime.timedelta(hours=1))
             assert datetime.datetime(2000, 1, 1, 11, 0, 5) == datetime.datetime.now()
 
     def test_nonfake_time_is_dynamic(self):
         self._assert_time_not_faked()
 
     @fake_time(datetime.datetime.now())
     def test_fake_time_is_static(self):
         first = datetime.datetime.now().microsecond
         second = datetime.datetime.now().microsecond
 
         assert second == first
 
-    @fake_time('2000-01-01 10:00:05')
+    @fake_time("2000-01-01 10:00:05")
     def test_fake_time_parses_easy_strings(self):
         assert datetime.datetime(2000, 1, 1, 10, 0, 5) == datetime.datetime.now()
         assert datetime.datetime(2000, 1, 1, 10, 0, 5) == datetime.datetime.utcnow()
 
     def test_fake_time_parses_easy_strings_with_timezones(self):
-        with fake_time('2000-01-01 10:00:05', tz_offset=3):
+        with fake_time("2000-01-01 10:00:05", tz_offset=3):
             assert datetime.datetime(2000, 1, 1, 13, 0, 5) == datetime.datetime.now()
             assert datetime.datetime(2000, 1, 1, 10, 0, 5) == datetime.datetime.utcnow()
 
-        with fake_time('2000-01-01 10:00:05', tz_offset=-3):
+        with fake_time("2000-01-01 10:00:05", tz_offset=-3):
             assert datetime.datetime(2000, 1, 1, 7, 0, 5) == datetime.datetime.now()
             assert datetime.datetime(2000, 1, 1, 10, 0, 5) == datetime.datetime.utcnow()
 
-    @fake_time('march 1st, 2014 at 1:59pm')
+    @fake_time("march 1st, 2014 at 1:59pm")
     def test_fake_time_parses_tough_strings(self):
         assert datetime.datetime(2014, 3, 1, 13, 59) == datetime.datetime.now()
 
     @fake_time(datetime.datetime(2014, 1, 1, microsecond=123456))
     def test_fake_time_has_microsecond_granularity(self):
-        assert datetime.datetime(2014, 1, 1, microsecond=123456) == datetime.datetime.now()
+        assert (
+            datetime.datetime(2014, 1, 1, microsecond=123456) == datetime.datetime.now()
+        )
 
     def test_nested_fake_time(self):
         self._assert_time_not_faked()
 
-        with fake_time('1/1/2000'):
+        with fake_time("1/1/2000"):
             assert datetime.datetime(2000, 1, 1) == datetime.datetime.now()
 
-            with fake_time('1/1/2001'):
+            with fake_time("1/1/2001"):
                 assert datetime.datetime(2001, 1, 1) == datetime.datetime.now()
 
             assert datetime.datetime(2000, 1, 1) == datetime.datetime.now()
 
         self._assert_time_not_faked()
 
     def test_freeze_time_alias(self):
-        with freeze_time('2000-01-01 10:00:05'):
+        with freeze_time("2000-01-01 10:00:05"):
             assert datetime.datetime(2000, 1, 1, 10, 0, 5) == datetime.datetime.now()
 
     def test_monotonic_not_mocked(self):
-        assert os.environ['DONT_FAKE_MONOTONIC'] == '1'
+        assert os.environ["DONT_FAKE_MONOTONIC"] == "1"
+
+    def test_timestmap_file(self, tmpdir):
+        file_path = str(tmpdir / "faketime.rc")
+
+        with fake_time("2000-01-01 10:00:05", timestamp_file=file_path) as fake:
+            assert datetime.datetime(2000, 1, 1, 10, 0, 5) == datetime.datetime.now()
+            with open(file_path) as fd:
+                assert fd.read() == "2000-01-01 10:00:05.000000"
 
+            fake.tick(delta=datetime.timedelta(hours=1))
+            assert datetime.datetime(2000, 1, 1, 11, 0, 5) == datetime.datetime.now()
+            with open(file_path) as fd:
+                assert fd.read() == "2000-01-01 11:00:05.000000"
 
-class TestUUID1Deadlock():
+        with fake_time(timestamp_file=file_path):
+            assert datetime.datetime(2000, 1, 1, 11, 0, 5) == datetime.datetime.now()
 
+
+class TestUUID1Deadlock:
     @fake_time(datetime.datetime.now())
     def test_uuid1_does_not_deadlock(self):
-        """This test will deadlock if we fail to patch a system level uuid library."""
+        """This test will deadlock if we fail to patch a system level uuid
+        library."""
         for i in range(100):
             uuid.uuid1()
 
 
-@fake_time('2000-01-01')
+@fake_time("2000-01-01")
 class TestClassDecorator:
-
     def test_simple(self):
         assert datetime.datetime(2000, 1, 1) == datetime.datetime.now()
         self._faked_time.tick()
         assert datetime.datetime(2000, 1, 1, 0, 0, 1) == datetime.datetime.now()
 
-    @fake_time('2001-01-01')
+    @fake_time("2001-01-01")
     def test_overwrite_with_func_decorator(self):
         assert datetime.datetime(2001, 1, 1) == datetime.datetime.now()
```

### Comparing `libfaketime-2.0.0/test/test_freezegun.py` & `libfaketime-2.1.0/test/test_freezegun.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-import pytest
-import time
 import datetime
+import time
 
+import pytest
 from freezegun import freeze_time
+
 from libfaketime import fake_time
 
 # TODO
 # - Fix time.localtime
 # - Fix time.strftime
-# - Fix python2 time.time with 1970-01-01
+
+# mark these as being used (via eval)
+assert time
+assert datetime
 
 test_functions = [
     ("datetime.datetime.now", (), {}),
     ("datetime.datetime.utcnow", (), {}),
     ("time.time", (), {}),
-#    ("time.localtime", (), {}),
-#    ("time.strftime", ("%Y-%m-%d %H:%M:%S %Z",), {}),
-    ("datetime.date", (), {"year": 1970, "month":1, "day":1}),
-    ("datetime.datetime", (), {"year": 1970, "month":1, "day":1}),
+    #    ("time.localtime", (), {}),
+    #    ("time.strftime", ("%Y-%m-%d %H:%M:%S %Z",), {}),
+    ("datetime.date", (), {"year": 1970, "month": 1, "day": 1}),
+    ("datetime.datetime", (), {"year": 1970, "month": 1, "day": 1}),
 ]
 
+
 @pytest.mark.parametrize("test_function", test_functions)
 @pytest.mark.parametrize("tz_offset", [0, 12])
-@pytest.mark.parametrize("date_to_freeze", ["1970-01-01 00:00:01"]) 
+@pytest.mark.parametrize("date_to_freeze", ["1970-01-01 00:00:01"])
 def test_compare_against_freezegun_results(test_function, tz_offset, date_to_freeze):
     func_name, args, kwargs = test_function
 
-    with fake_time(date_to_freeze, tz_offset = tz_offset):
+    with fake_time(date_to_freeze, tz_offset=tz_offset):
         libfaketime_result = eval(func_name)(*args, **kwargs)
 
-    with freeze_time(date_to_freeze, tz_offset = tz_offset):
+    with freeze_time(date_to_freeze, tz_offset=tz_offset):
         freezegun_result = eval(func_name)(*args, **kwargs)
 
     assert freezegun_result == libfaketime_result
-
```

### Comparing `libfaketime-2.0.0/test/test_tz.py` & `libfaketime-2.1.0/test/test_tz.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
-import dateutil.tz
 import os
 
+import dateutil.tz
 import pytest
 from pytz import timezone
 
 from libfaketime import fake_time
 
 
 def test_timezone_is_restored_after_context_manager_usage():
@@ -21,46 +21,53 @@
 
     assert abs((now2 - now1).total_seconds()) < 10
     assert abs((utcnow2 - utcnow1).total_seconds()) < 10
 
 
 def test_tzinfo_is_normalized():
     """Ensure utcnow() behaves correctly when faking non-UTC timestamps."""
-    timezone_to_test_with = timezone('Europe/Brussels')
-    time_to_freeze = timezone_to_test_with.localize(datetime.datetime(2017, 1, 2, 15, 2))
+    timezone_to_test_with = timezone("Europe/Brussels")
+    time_to_freeze = timezone_to_test_with.localize(
+        datetime.datetime(2017, 1, 2, 15, 2)
+    )
 
     with fake_time(time_to_freeze):
         # The timeshift of Europe/Brussels is UTC+1 in January
         assert datetime.datetime.now() == datetime.datetime(2017, 1, 2, 15, 2)
         assert datetime.datetime.utcnow() == datetime.datetime(2017, 1, 2, 14, 2)
 
 
 def test_block_setting_of_conflicting_tz_info():
-    """Cannot pass in tz_offset when the timestamp already carries a timezone."""
+    """Cannot pass in tz_offset when the timestamp already carries a
+    timezone."""
     with pytest.raises(Exception) as exc_info:
-        timezone_to_test_with = timezone('America/Havana')
-        time_to_freeze = timezone_to_test_with.localize(datetime.datetime(2012, 10, 2, 21, 38))
+        timezone_to_test_with = timezone("America/Havana")
+        time_to_freeze = timezone_to_test_with.localize(
+            datetime.datetime(2012, 10, 2, 21, 38)
+        )
 
         with fake_time(time_to_freeze, tz_offset=5):
             pass
 
-    assert str(exc_info.value) == 'Cannot set tz_offset when datetime already has timezone'
+    assert (
+        str(exc_info.value) == "Cannot set tz_offset when datetime already has timezone"
+    )
 
 
 @pytest.mark.parametrize("offset", range(-2, 3))
 def test_generated_tz_is_valid(offset):
     """https://github.com/simon-weber/python-libfaketime/issues/46"""
     now = datetime.datetime.now()
 
     with fake_time(now, tz_offset=offset):
-        fake_tz = os.environ['TZ']
+        fake_tz = os.environ["TZ"]
         timezone(fake_tz)  # should not raise pytzdata.exceptions.TimezoneNotFound
 
 
 def test_dateutil_tz_is_valid():
     test_dt = datetime.datetime(2017, 1, 2, 15, 2)
-    dateutil_tzinfo = dateutil.tz.gettz('UTC')
+    dateutil_tzinfo = dateutil.tz.gettz("UTC")
     dt_dateutil_tzinfo = test_dt.replace(tzinfo=dateutil_tzinfo)
 
     # Should be compatible with a dateutil tzinfo object, not just pytz
     with fake_time(dt_dateutil_tzinfo):
         assert datetime.datetime.now(tz=dateutil_tzinfo) == dt_dateutil_tzinfo
```

