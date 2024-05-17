# Comparing `tmp/sqlalchemy_mate-2.0.0.0.tar.gz` & `tmp/sqlalchemy_mate-2.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_mate-2.0.0.0.tar", last modified: Wed May 15 06:24:51 2024, max compression
+gzip compressed data, was "sqlalchemy_mate-2.0.0.1.tar", last modified: Fri May 17 06:10:33 2024, max compression
```

## Comparing `sqlalchemy_mate-2.0.0.0.tar` & `sqlalchemy_mate-2.0.0.1.tar`

### file list

```diff
@@ -1,57 +1,73 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.073165 sqlalchemy_mate-2.0.0.0/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.0/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.0/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      356 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.0/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)    11668 2024-05-15 06:24:51.072941 sqlalchemy_mate-2.0.0.0/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     9672 2024-05-15 06:12:00.000000 sqlalchemy_mate-2.0.0.0/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     6707 2024-05-15 06:13:01.000000 sqlalchemy_mate-2.0.0.0/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.0/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      390 2024-05-14 20:30:28.000000 sqlalchemy_mate-2.0.0.0/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      871 2024-05-14 20:26:57.000000 sqlalchemy_mate-2.0.0.0/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      128 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.0/requirements-furo-sphinx-search.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      214 2024-05-14 20:27:06.000000 sqlalchemy_mate-2.0.0.0/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       51 2024-05-14 20:57:38.000000 sqlalchemy_mate-2.0.0.0/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2024-05-15 06:24:51.073209 sqlalchemy_mate-2.0.0.0/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7479 2024-05-15 05:55:50.000000 sqlalchemy_mate-2.0.0.0/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.065862 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/
--rw-r--r--   0 sanhehu    (501) staff       (20)      803 2024-05-15 05:36:41.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      100 2024-05-15 06:02:49.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/_version.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.067817 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/
--rw-r--r--   0 sanhehu    (501) staff       (20)       85 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      343 2024-05-15 05:07:50.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/deleting.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3332 2024-05-15 04:37:22.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/inserting.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6145 2024-05-15 05:01:17.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/selecting.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3686 2024-05-15 05:07:15.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/updating.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.068067 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    14141 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/engine_creator.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2173 2024-05-14 21:20:06.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/io.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.068518 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/orm/
--rw-r--r--   0 sanhehu    (501) staff       (20)       50 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/orm/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    20444 2024-05-15 05:18:28.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/orm/extended_declarative_base.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5917 2024-05-15 04:01:42.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/pt.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.069299 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/types/
--rw-r--r--   0 sanhehu    (501) staff       (20)      192 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/types/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1931 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/types/compressed.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2565 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/types/compressed_json.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2453 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/types/json_serializable.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3476 2024-05-15 05:11:24.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.069674 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.070054 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/vendor/timeout_decorator/
--rw-r--r--   0 sanhehu    (501) staff       (20)      162 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/vendor/timeout_decorator/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6411 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/vendor/timeout_decorator/timeout_decorator.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.071708 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)    11668 2024-05-15 06:24:51.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1331 2024-05-15 06:24:51.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2024-05-15 06:24:51.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      291 2024-05-15 06:24:51.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       16 2024-05-15 06:24:51.000000 sqlalchemy_mate-2.0.0.0/sqlalchemy_mate.egg-info/top_level.txt
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-15 06:24:51.071420 sqlalchemy_mate-2.0.0.0/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3190 2024-05-15 04:08:44.000000 sqlalchemy_mate-2.0.0.0/tests/test_engine_creator.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1051 2024-05-15 05:38:39.000000 sqlalchemy_mate-2.0.0.0/tests/test_import.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1308 2024-05-14 21:00:03.000000 sqlalchemy_mate-2.0.0.0/tests/test_io.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6352 2024-05-15 03:57:04.000000 sqlalchemy_mate-2.0.0.0/tests/test_pt.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1527 2024-05-15 04:08:55.000000 sqlalchemy_mate-2.0.0.0/tests/test_utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.674117 sqlalchemy_mate-2.0.0.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      356 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)    11696 2024-05-17 06:10:33.673886 sqlalchemy_mate-2.0.0.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     9700 2024-05-17 05:49:58.000000 sqlalchemy_mate-2.0.0.1/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8742 2024-05-17 06:07:09.000000 sqlalchemy_mate-2.0.0.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      390 2024-05-14 20:30:28.000000 sqlalchemy_mate-2.0.0.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      871 2024-05-14 20:26:57.000000 sqlalchemy_mate-2.0.0.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      128 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.1/requirements-furo-sphinx-search.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      214 2024-05-14 20:27:06.000000 sqlalchemy_mate-2.0.0.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       51 2024-05-14 20:57:38.000000 sqlalchemy_mate-2.0.0.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2024-05-17 06:10:33.674164 sqlalchemy_mate-2.0.0.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7479 2024-05-15 05:55:50.000000 sqlalchemy_mate-2.0.0.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.663241 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      258 2024-05-16 13:04:55.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      100 2024-05-17 06:07:22.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      578 2024-05-17 04:57:05.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.666418 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       85 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      343 2024-05-15 05:07:50.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/deleting.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2024-05-16 12:56:47.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/deleting_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3332 2024-05-15 04:37:22.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/inserting.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       61 2024-05-16 12:57:04.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/inserting_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6145 2024-05-15 05:01:17.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/selecting.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      403 2024-05-16 12:57:55.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/selecting_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3686 2024-05-15 05:07:15.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/updating.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       91 2024-05-16 12:57:34.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/updating_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.666847 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    14141 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/engine_creator.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2173 2024-05-14 21:20:06.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/io.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       80 2024-05-16 13:00:32.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/io_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.667611 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/orm/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       50 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/orm/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       77 2024-05-16 12:59:27.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/orm/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    20444 2024-05-15 05:18:28.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/orm/extended_declarative_base.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.668084 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/patterns/
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2024-05-15 18:33:49.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/patterns/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       75 2024-05-17 04:56:43.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/patterns/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.669360 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/patterns/status_tracker/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      357 2024-05-16 06:33:00.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/patterns/status_tracker/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      145 2024-05-16 14:11:16.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/patterns/status_tracker/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    15137 2024-05-17 06:04:38.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/patterns/status_tracker/impl.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5917 2024-05-15 04:01:42.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/pt.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      261 2024-05-16 13:21:05.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/pt_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.670457 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       24 2024-05-16 13:02:00.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      192 2024-05-16 13:02:02.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1931 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/compressed.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2565 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/compressed_json.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2453 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/json_serializable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3487 2024-05-16 13:02:42.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.670842 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.671242 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/vendor/timeout_decorator/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      162 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/vendor/timeout_decorator/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6411 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/vendor/timeout_decorator/timeout_decorator.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.672763 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)    11696 2024-05-17 06:10:33.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1825 2024-05-17 06:10:33.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2024-05-17 06:10:33.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      291 2024-05-17 06:10:33.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       16 2024-05-17 06:10:33.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.672495 sqlalchemy_mate-2.0.0.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1276 2024-05-17 06:05:50.000000 sqlalchemy_mate-2.0.0.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3197 2024-05-16 12:45:12.000000 sqlalchemy_mate-2.0.0.1/tests/test_engine_creator.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1353 2024-05-16 12:45:55.000000 sqlalchemy_mate-2.0.0.1/tests/test_io.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6071 2024-05-16 13:20:05.000000 sqlalchemy_mate-2.0.0.1/tests/test_pt.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1603 2024-05-16 13:20:23.000000 sqlalchemy_mate-2.0.0.1/tests/test_utils.py
```

### Comparing `sqlalchemy_mate-2.0.0.0/AUTHORS.rst` & `sqlalchemy_mate-2.0.0.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/LICENSE.txt` & `sqlalchemy_mate-2.0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/PKG-INFO` & `sqlalchemy_mate-2.0.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_mate
-Version: 2.0.0.0
+Version: 2.0.0.1
 Summary: A library extend sqlalchemy module, makes CRUD easier.
 Home-page: https://github.com/MacHu-GWU/sqlalchemy_mate-project
-Download-URL: https://pypi.python.org/pypi/sqlalchemy_mate/2.0.0.0#downloads
+Download-URL: https://pypi.python.org/pypi/sqlalchemy_mate/2.0.0.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -162,15 +162,15 @@
         }
     }
 
 code:
 
 .. code-block:: python
 
-    from sqlalchemy_mate import EngineCreator
+    from sqlalchemy_mate.api import EngineCreator
 
     ec = EngineCreator.from_json(
         json_file="path-to-json-file",
         json_path="credentials.db1", # dot notation json path
     )
     engine = ec.create_postgresql_pg8000()
 
@@ -196,15 +196,15 @@
 From ``$HOME/.db.json``
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 You can put lots of database connection info in a ``.db.json`` file in your ``$HOME`` directory.
 
 .. code-block:: python
 
-    from sqlalchemy_mate import EngineCreator
+    from sqlalchemy_mate.api import EngineCreator
 
     ec = EngineCreator.from_home_db_json(identifier="db1")
     engine = ec.create_postgresql_psycopg2()
 
 ``$HOME/.db.json`` **assumes flat json schema**, but you can use dot notation json path for ``identifier`` to adapt any json schema:
 
 .. code-block:: python
@@ -226,15 +226,15 @@
 From json file on AWS S3
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 This is similar to ``from_json``, but the json file is stored on AWS S3.
 
 .. code-block:: python
 
-    from sqlalchemy_mate import EngineCreator
+    from sqlalchemy_mate.api import EngineCreator
     ec = EngineCreator.from_s3_json(
         bucket_name="my-bucket", key="db.json",
         json_path="identifier1",
         aws_profile="my-profile",
     )
     engine = ec.create_redshift()
 
@@ -250,15 +250,15 @@
     export DB_DEV_PORT="..."
     export DB_DEV_DATABASE="..."
     export DB_DEV_USERNAME="..."
     export DB_DEV_PASSWORD="..."
 
 .. code-block:: python
 
-    from sqlalchemy_mate import EngineCreator
+    from sqlalchemy_mate.api import EngineCreator
     # read from DB_DEV_USERNAME, DB_DEV_PASSWORD, ...
     ec = EngineCreator.from_env(prefix="DB_DEV")
     engine = ec.create_redshift()
 
 If you want to read database credential safely from cloud, for example, AWS EC2, AWS Lambda, you can use AWS KMS to decrypt your credentials
 
 .. code-block:: python
@@ -286,15 +286,15 @@
 
 ``sqlalchemy_mate`` uses ``smart_insert`` strategy to try with smaller bulk insert, which has higher probabily to work. As a result, total number of commits are greatly reduced.
 
 With sql expression:
 
 .. code-block:: python
 
-    from sqlalchemy_mate import inserting
+    from sqlalchemy_mate.api import inserting
     engine = create_engine(...)
     t_users = Table(
         "users", metadata,
         Column("id", Integer),
         ...
     )
     # lots of data
@@ -303,15 +303,15 @@
     inserting.smart_insert(engine, t_users, data)
 
 
 With ORM:
 
 .. code-block:: python
 
-    from sqlalchemy_mate import ExtendedBase
+    from sqlalchemy_mate.api import ExtendedBase
     Base = declarative_base()
     class User(Base, ExtendedBase): # inherit from ExtendedBase
         ...
     # lots of users
     data = [User(id=1, name="Alice"), User(id=2, name="Bob"), ...]
     # the magic method
     User.smart_insert(engine_or_session, data) # That's it
@@ -321,15 +321,15 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Automatically update value by primary key.
 
 .. code-block:: python
 
     # in SQL expression
-    from sqlalchemy_mate import updating
+    from sqlalchemy_mate.api import updating
 
     data = [{"id": 1, "name": "Alice}, {"id": 2, "name": "Bob"}, ...]
     updating.update_all(engine, table, data)
     updating.upsert_all(engine, table, data)
 
     # in ORM
     data = [User(id=1, name="Alice"), User(id=2, name="Bob"), ...]
```

### Comparing `sqlalchemy_mate-2.0.0.0/README.rst` & `sqlalchemy_mate-2.0.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         }
     }
 
 code:
 
 .. code-block:: python
 
-    from sqlalchemy_mate import EngineCreator
+    from sqlalchemy_mate.api import EngineCreator
 
     ec = EngineCreator.from_json(
         json_file="path-to-json-file",
         json_path="credentials.db1", # dot notation json path
     )
     engine = ec.create_postgresql_pg8000()
 
@@ -145,15 +145,15 @@
 From ``$HOME/.db.json``
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 You can put lots of database connection info in a ``.db.json`` file in your ``$HOME`` directory.
 
 .. code-block:: python
 
-    from sqlalchemy_mate import EngineCreator
+    from sqlalchemy_mate.api import EngineCreator
 
     ec = EngineCreator.from_home_db_json(identifier="db1")
     engine = ec.create_postgresql_psycopg2()
 
 ``$HOME/.db.json`` **assumes flat json schema**, but you can use dot notation json path for ``identifier`` to adapt any json schema:
 
 .. code-block:: python
@@ -175,15 +175,15 @@
 From json file on AWS S3
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 This is similar to ``from_json``, but the json file is stored on AWS S3.
 
 .. code-block:: python
 
-    from sqlalchemy_mate import EngineCreator
+    from sqlalchemy_mate.api import EngineCreator
     ec = EngineCreator.from_s3_json(
         bucket_name="my-bucket", key="db.json",
         json_path="identifier1",
         aws_profile="my-profile",
     )
     engine = ec.create_redshift()
 
@@ -199,15 +199,15 @@
     export DB_DEV_PORT="..."
     export DB_DEV_DATABASE="..."
     export DB_DEV_USERNAME="..."
     export DB_DEV_PASSWORD="..."
 
 .. code-block:: python
 
-    from sqlalchemy_mate import EngineCreator
+    from sqlalchemy_mate.api import EngineCreator
     # read from DB_DEV_USERNAME, DB_DEV_PASSWORD, ...
     ec = EngineCreator.from_env(prefix="DB_DEV")
     engine = ec.create_redshift()
 
 If you want to read database credential safely from cloud, for example, AWS EC2, AWS Lambda, you can use AWS KMS to decrypt your credentials
 
 .. code-block:: python
@@ -235,15 +235,15 @@
 
 ``sqlalchemy_mate`` uses ``smart_insert`` strategy to try with smaller bulk insert, which has higher probabily to work. As a result, total number of commits are greatly reduced.
 
 With sql expression:
 
 .. code-block:: python
 
-    from sqlalchemy_mate import inserting
+    from sqlalchemy_mate.api import inserting
     engine = create_engine(...)
     t_users = Table(
         "users", metadata,
         Column("id", Integer),
         ...
     )
     # lots of data
@@ -252,15 +252,15 @@
     inserting.smart_insert(engine, t_users, data)
 
 
 With ORM:
 
 .. code-block:: python
 
-    from sqlalchemy_mate import ExtendedBase
+    from sqlalchemy_mate.api import ExtendedBase
     Base = declarative_base()
     class User(Base, ExtendedBase): # inherit from ExtendedBase
         ...
     # lots of users
     data = [User(id=1, name="Alice"), User(id=2, name="Bob"), ...]
     # the magic method
     User.smart_insert(engine_or_session, data) # That's it
@@ -270,15 +270,15 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Automatically update value by primary key.
 
 .. code-block:: python
 
     # in SQL expression
-    from sqlalchemy_mate import updating
+    from sqlalchemy_mate.api import updating
 
     data = [{"id": 1, "name": "Alice}, {"id": 2, "name": "Bob"}, ...]
     updating.update_all(engine, table, data)
     updating.upsert_all(engine, table, data)
 
     # in ORM
     data = [User(id=1, name="Alice"), User(id=2, name="Bob"), ...]
```

### Comparing `sqlalchemy_mate-2.0.0.0/requirements-doc.txt` & `sqlalchemy_mate-2.0.0.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/setup.py` & `sqlalchemy_mate-2.0.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/inserting.py` & `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/inserting.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/selecting.py` & `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/selecting.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/crud/updating.py` & `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/updating.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/engine_creator.py` & `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/engine_creator.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/io.py` & `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/io.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/orm/extended_declarative_base.py` & `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/orm/extended_declarative_base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/paths.py` & `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/paths.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/pt.py` & `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/pt.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/types/compressed.py` & `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/compressed.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/types/compressed_json.py` & `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/compressed_json.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/types/json_serializable.py` & `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/json_serializable.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/utils.py` & `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     if auto_close:
         session.close()
 
 
 from .vendor import timeout_decorator
 
 
-def test_connection(engine, timeout=3):
+def test_connection(engine: sa.Engine, timeout=3):
     @timeout_decorator.timeout(timeout)
     def _test_connection(engine):
         with engine.connect() as connection:
             v = connection.execute(sa.text("SELECT 1;")).fetchall()[0][0]
             assert v == 1
 
     try:
```

### Comparing `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/vendor/pytest_cov_helper.py` & `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate/vendor/timeout_decorator/timeout_decorator.py` & `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/vendor/timeout_decorator/timeout_decorator.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.0/sqlalchemy_mate.egg-info/PKG-INFO` & `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_mate
-Version: 2.0.0.0
+Version: 2.0.0.1
 Summary: A library extend sqlalchemy module, makes CRUD easier.
 Home-page: https://github.com/MacHu-GWU/sqlalchemy_mate-project
-Download-URL: https://pypi.python.org/pypi/sqlalchemy_mate/2.0.0.0#downloads
+Download-URL: https://pypi.python.org/pypi/sqlalchemy_mate/2.0.0.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -162,15 +162,15 @@
         }
     }
 
 code:
 
 .. code-block:: python
 
-    from sqlalchemy_mate import EngineCreator
+    from sqlalchemy_mate.api import EngineCreator
 
     ec = EngineCreator.from_json(
         json_file="path-to-json-file",
         json_path="credentials.db1", # dot notation json path
     )
     engine = ec.create_postgresql_pg8000()
 
@@ -196,15 +196,15 @@
 From ``$HOME/.db.json``
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 You can put lots of database connection info in a ``.db.json`` file in your ``$HOME`` directory.
 
 .. code-block:: python
 
-    from sqlalchemy_mate import EngineCreator
+    from sqlalchemy_mate.api import EngineCreator
 
     ec = EngineCreator.from_home_db_json(identifier="db1")
     engine = ec.create_postgresql_psycopg2()
 
 ``$HOME/.db.json`` **assumes flat json schema**, but you can use dot notation json path for ``identifier`` to adapt any json schema:
 
 .. code-block:: python
@@ -226,15 +226,15 @@
 From json file on AWS S3
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 This is similar to ``from_json``, but the json file is stored on AWS S3.
 
 .. code-block:: python
 
-    from sqlalchemy_mate import EngineCreator
+    from sqlalchemy_mate.api import EngineCreator
     ec = EngineCreator.from_s3_json(
         bucket_name="my-bucket", key="db.json",
         json_path="identifier1",
         aws_profile="my-profile",
     )
     engine = ec.create_redshift()
 
@@ -250,15 +250,15 @@
     export DB_DEV_PORT="..."
     export DB_DEV_DATABASE="..."
     export DB_DEV_USERNAME="..."
     export DB_DEV_PASSWORD="..."
 
 .. code-block:: python
 
-    from sqlalchemy_mate import EngineCreator
+    from sqlalchemy_mate.api import EngineCreator
     # read from DB_DEV_USERNAME, DB_DEV_PASSWORD, ...
     ec = EngineCreator.from_env(prefix="DB_DEV")
     engine = ec.create_redshift()
 
 If you want to read database credential safely from cloud, for example, AWS EC2, AWS Lambda, you can use AWS KMS to decrypt your credentials
 
 .. code-block:: python
@@ -286,15 +286,15 @@
 
 ``sqlalchemy_mate`` uses ``smart_insert`` strategy to try with smaller bulk insert, which has higher probabily to work. As a result, total number of commits are greatly reduced.
 
 With sql expression:
 
 .. code-block:: python
 
-    from sqlalchemy_mate import inserting
+    from sqlalchemy_mate.api import inserting
     engine = create_engine(...)
     t_users = Table(
         "users", metadata,
         Column("id", Integer),
         ...
     )
     # lots of data
@@ -303,15 +303,15 @@
     inserting.smart_insert(engine, t_users, data)
 
 
 With ORM:
 
 .. code-block:: python
 
-    from sqlalchemy_mate import ExtendedBase
+    from sqlalchemy_mate.api import ExtendedBase
     Base = declarative_base()
     class User(Base, ExtendedBase): # inherit from ExtendedBase
         ...
     # lots of users
     data = [User(id=1, name="Alice"), User(id=2, name="Bob"), ...]
     # the magic method
     User.smart_insert(engine_or_session, data) # That's it
@@ -321,15 +321,15 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Automatically update value by primary key.
 
 .. code-block:: python
 
     # in SQL expression
-    from sqlalchemy_mate import updating
+    from sqlalchemy_mate.api import updating
 
     data = [{"id": 1, "name": "Alice}, {"id": 2, "name": "Bob"}, ...]
     updating.update_all(engine, table, data)
     updating.upsert_all(engine, table, data)
 
     # in ORM
     data = [User(id=1, name="Alice"), User(id=2, name="Bob"), ...]
```

### Comparing `sqlalchemy_mate-2.0.0.0/tests/test_engine_creator.py` & `sqlalchemy_mate-2.0.0.1/tests/test_engine_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,10 +98,10 @@
                 password="pass",
             ),
         )
         assert new_data == dict(host=1, port=2, database=3, username=4, password=5)
 
 
 if __name__ == "__main__":
-    from sqlalchemy_mate.tests import run_cov_test
+    from sqlalchemy_mate.tests.helper import run_cov_test
 
     run_cov_test(__file__, "sqlalchemy_mate.engine_creator", preview=False)
```

### Comparing `sqlalchemy_mate-2.0.0.0/tests/test_io.py` & `sqlalchemy_mate-2.0.0.1/tests/test_io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # -*- coding: utf-8 -*-
 
 import pytest
 
 from sqlalchemy_mate import io
-from sqlalchemy_mate.tests import (
-    IS_WINDOWS, engine_sqlite, engine_psql, t_user, BaseTest,
+from sqlalchemy_mate.tests.api import (
+    IS_WINDOWS,
+    engine_sqlite,
+    engine_psql,
+    t_user,
+    BaseCrudTest,
 )
 
 
 def teardown_module(module):
     import os
 
     try:
         filepath = __file__.replace("test_io.py", "t_user.csv")
         os.remove(filepath)
     except:
         pass
 
 
-class DataIOTestBase(BaseTest):
+class DataIOTestBase(BaseCrudTest):
     @classmethod
     def class_level_data_setup(cls):
         with cls.engine.connect() as connection:
             connection.execute(t_user.delete())
             data = [
                 {"user_id": 1, "name": "Alice"},
                 {"user_id": 2, "name": "Bob"},
@@ -44,11 +48,10 @@
     reason="no psql service container for windows",
 )
 class TestDataIOPostgres(DataIOTestBase):
     engine = engine_psql
 
 
 if __name__ == "__main__":
-    import os
+    from sqlalchemy_mate.tests.helper import run_cov_test
 
-    basename = os.path.basename(__file__)
-    pytest.main([basename, "-s", "--tb=native"])
+    run_cov_test(__file__, "sqlalchemy_mate.io", preview=False)
```

### Comparing `sqlalchemy_mate-2.0.0.0/tests/test_pt.py` & `sqlalchemy_mate-2.0.0.1/tests/test_pt.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import pytest
 
 import sqlalchemy as sa
 import sqlalchemy.orm as orm
 
 from prettytable import PrettyTable
 
-from sqlalchemy_mate import pt, selecting
-from sqlalchemy_mate.tests import (
+from sqlalchemy_mate.api import pt, selecting
+from sqlalchemy_mate.tests.api import (
     IS_WINDOWS,
     engine_sqlite,
     engine_psql,
     t_user,
     t_inv,
     User,
     Association,
-    BaseTest,
+    BaseCrudTest,
 )
 
 
-class PrettyTableTestBase(BaseTest):
+class PrettyTableTestBase(BaseCrudTest):
     @classmethod
     def class_level_data_setup(cls):
         cls.delete_all_data_in_core_table()
         cls.delete_all_data_in_orm_table()
 
         t_user_data = [
             {"user_id": 1, "name": "Alice"},
@@ -42,15 +42,15 @@
             {"store_id": 3, "item_id": 2},
         ]
 
         with cls.engine.connect() as connection:
             connection.execute(sa.insert(t_user), t_user_data)
             connection.execute(t_inv.insert(), t_inv_data)
             connection.commit()
-        
+
         with orm.Session(cls.engine) as ses:
             ses.add_all(
                 [
                     User(id=1, name="X"),
                     User(id=2, name="Y"),
                     User(id=3, name="Z"),
                 ]
@@ -61,52 +61,52 @@
                     Association(x_id=1, y_id=2, flag=2),
                     Association(x_id=2, y_id=1, flag=3),
                     Association(x_id=2, y_id=2, flag=4),
                 ]
             )
             ses.commit()
 
-    def _test_get_headers(self):
+    def test_get_headers(self):
         with orm.Session(self.eng) as ses:
             user = ses.get(User, 1)
             keys, values = pt.get_keys_values(user)
             assert keys == ["id", "name"]
             assert values == [1, "X"]
 
         with self.eng.connect() as connection:
             row = connection.execute(sa.select(t_user).limit(1)).fetchone()
             keys, values = pt.get_keys_values(row)
             assert keys == ["user_id", "name"]
             assert values == [1, "Alice"]
 
-    def _test_from_result(self):
+    def test_from_result(self):
         with orm.Session(self.eng) as ses:
             res = ses.scalars(sa.select(User))
             ptable = pt.from_result(res)
             assert len(ptable._rows) == 3
 
         with self.eng.connect() as connection:
             res = connection.execute(sa.select(t_user))
             ptable = pt.from_result(res)
             assert len(ptable._rows) == 4
 
-    def _test_from_text_clause(self):
+    def test_from_text_clause(self):
         stmt = sa.text(f"SELECT * FROM {t_user.name} LIMIT 2")
         tb = pt.from_text_clause(stmt, self.eng)
         assert isinstance(tb, PrettyTable)
         assert len(tb._rows) == 2
         stmt = sa.text(
             f"SELECT * FROM {t_user.name} WHERE {t_user.name}.user_id = :user_id;"
         )
         stmt = stmt.bindparams(user_id=1)
         tb = pt.from_text_clause(stmt, self.eng)
         assert isinstance(tb, PrettyTable)
         assert len(tb._rows) == 1
 
-    def _test_from_stmt(self):
+    def test_from_stmt(self):
         stmt = sa.select(t_inv)
         tb = pt.from_stmt(stmt, self.eng)
         assert isinstance(tb, PrettyTable)
         assert len(tb._rows) == 6
 
         stmt = sa.select(t_inv).limit(3)
         tb = pt.from_stmt(stmt, self.eng)
@@ -120,41 +120,41 @@
         assert len(tb._rows) == 2
 
         query = sa.select(User).limit(2)
         tb = pt.from_stmt(query, self.eng)
         assert isinstance(tb, PrettyTable)
         assert len(tb._rows) == 2
 
-    def _test_from_table(self):
+    def test_from_table(self):
         tb = pt.from_table(t_inv, self.eng, limit=10)
         assert isinstance(tb, PrettyTable)
         assert len(tb._rows) == 6
 
         tb = pt.from_table(t_inv, self.eng, limit=3)
         assert isinstance(tb, PrettyTable)
         assert len(tb._rows) == 3
 
-    def _test_from_model(self):
+    def test_from_model(self):
         tb = pt.from_model(Association, self.eng, limit=2)
         assert isinstance(tb, PrettyTable)
         assert len(tb._rows) == 2
 
         with orm.Session(self.eng) as ses:
             tb = pt.from_model(User, ses, limit=2)
             assert isinstance(tb, PrettyTable)
             assert len(tb._rows) == 2
 
-    def _test_from_data(self):
+    def test_from_data(self):
         with self.eng.connect() as connection:
             rows = [row._asdict() for row in connection.execute(sa.select(t_user))]
             tb = pt.from_dict_list(rows)
             assert isinstance(tb, PrettyTable)
             assert len(tb._rows) == 4
 
-    def _test_from_everything(self):
+    def test_from_everything(self):
         t = sa.text(f"SELECT * FROM {t_user.name} LIMIT 2")
         stmt = sa.select(t_user)
         table = t_inv
         query = sa.select(Association)
         orm_class = User
         result = selecting.select_all(self.engine, t_user)
         data = [row._asdict() for row in selecting.select_all(self.engine, t_user)]
@@ -172,34 +172,24 @@
         for thing in everything:
             tb = pt.from_everything(thing, self.engine, limit=10)
             assert isinstance(tb, PrettyTable)
 
         with pytest.raises(Exception):
             pt.from_everything(None)
 
-    def test(self):
-        self._test_get_headers()
-        self._test_from_result()
-        self._test_from_text_clause()
-        self._test_from_stmt()
-        self._test_from_table()
-        self._test_from_model()
-        self._test_from_data()
-        self._test_from_everything()
-
 
 class TestPrettyTableSqlite(PrettyTableTestBase):
     engine = engine_sqlite
 
 
 @pytest.mark.skipif(
     IS_WINDOWS,
     reason="no psql service container for windows",
 )
 class TestPrettyTablePostgres(PrettyTableTestBase):
     engine = engine_psql
 
 
 if __name__ == "__main__":
-    from sqlalchemy_mate.tests import run_cov_test
+    from sqlalchemy_mate.tests.helper import run_cov_test
 
     run_cov_test(__file__, "sqlalchemy_mate.pt", preview=False)
```

### Comparing `sqlalchemy_mate-2.0.0.0/tests/test_utils.py` & `sqlalchemy_mate-2.0.0.1/tests/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # -*- coding: utf-8 -*-
 
 
 import pytest
 from sqlalchemy_mate import utils
-from sqlalchemy_mate import EngineCreator, TimeoutError
-from sqlalchemy_mate.tests import (
+from sqlalchemy_mate.api import EngineCreator, TimeoutError
+from sqlalchemy_mate.tests.api import (
     IS_WINDOWS,
-    engine_sqlite, engine_psql, User, BaseTest,
+    engine_sqlite,
+    engine_psql,
+    BaseCrudTest,
 )
 
 
 def test_ensure_list():
-    assert utils.ensure_list(1) == [1, ]
+    assert utils.ensure_list(1) == [
+        1,
+    ]
     assert utils.ensure_list([1, 2, 3]) == [1, 2, 3]
     assert utils.ensure_list((1, 2, 3)) == (1, 2, 3)
 
 
-class UtilityTestBase(BaseTest):
+class UtilityTestBase(BaseCrudTest):
     def test_timeout_good_case(self):
         utils.test_connection(self.engine, timeout=3)
 
 
 @pytest.mark.skipif(
     IS_WINDOWS,
     reason="windows doesn't have such signal",
@@ -39,18 +43,21 @@
     reason="no psql service container for windows",
 )
 class TestUtilityPostgres(UtilityTestBase):
     engine = engine_psql
 
     def test_timeout_bad_case(self):
         engine = EngineCreator(
-            host="stampy.db.elephantsql.com", port=5432,
-            database="diyvavwx", username="diyvavwx", password="wrongpassword"
+            host="stampy.db.elephantsql.com",
+            port=5432,
+            database="diyvavwx",
+            username="diyvavwx",
+            password="wrongpassword",
         ).create_postgresql_pg8000()
         with pytest.raises(Exception):
             utils.test_connection(engine, timeout=10)
 
 
 if __name__ == "__main__":
-    from sqlalchemy_mate.tests import run_cov_test
+    from sqlalchemy_mate.tests.helper import run_cov_test
 
-    run_cov_test(__file__, "sqlalchemy_mate.utils", preview=False)
+    run_cov_test(__file__, "sqlalchemy_mate.utils", preview=False)
```

