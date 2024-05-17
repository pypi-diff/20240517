# Comparing `tmp/pypeman-0.5.5.tar.gz` & `tmp/pypeman-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypeman-0.5.5.tar", last modified: Thu Oct 19 15:35:07 2023, max compression
+gzip compressed data, was "pypeman-0.5.6.tar", last modified: Fri May 17 13:34:40 2024, max compression
```

## Comparing `pypeman-0.5.5.tar` & `pypeman-0.5.6.tar`

### file list

```diff
@@ -1,61 +1,106 @@
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-10-19 15:35:07.297024 pypeman-0.5.5/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    11358 2023-10-19 15:24:17.000000 pypeman-0.5.5/LICENSE
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       41 2023-10-19 15:24:17.000000 pypeman-0.5.5/MANIFEST.in
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3077 2023-10-19 15:35:07.297024 pypeman-0.5.5/PKG-INFO
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1928 2023-10-19 15:24:17.000000 pypeman-0.5.5/README.rst
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-10-19 15:35:07.293023 pypeman-0.5.5/pypeman/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       68 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    34192 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/channels.py
--rwxrwxr-x   0 quentin   (1000) quentin   (1000)    12351 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/commands.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2443 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/conf.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-10-19 15:35:07.293023 pypeman-0.5.5/pypeman/contrib/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/contrib/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3606 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/contrib/csv.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2178 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/contrib/ctx.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8624 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/contrib/ftp.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6750 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/contrib/hl7.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    12527 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/contrib/http.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      803 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/contrib/time.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      971 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/contrib/xml.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2126 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/debug.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1451 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/default_settings.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3433 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/endpoints.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      189 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/errors.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1395 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/events.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2577 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/graph.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-10-19 15:35:07.297024 pypeman-0.5.5/pypeman/helpers/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/helpers/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      421 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/helpers/aio_compat.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3247 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/helpers/cli.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      235 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/helpers/itertools.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1894 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/helpers/lazyload.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      663 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/helpers/logging.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3005 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/helpers/reloader.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1216 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/helpers/sleeper.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      315 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/helpers/tempfile.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1335 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/map_item.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6369 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/message.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    17864 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/msgstore.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    27982 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/nodes.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3713 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/persistence.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3946 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/pjt_templates.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2998 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/plugin_mgr.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-10-19 15:35:07.297024 pypeman-0.5.5/pypeman/plugins/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/plugins/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4262 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/plugins/base.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-10-19 15:35:07.297024 pypeman-0.5.5/pypeman/plugins/remoteadmin/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/plugins/remoteadmin/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      712 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/plugins/remoteadmin/plugin.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1033 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/plugins/remoteadmin/urls.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8801 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/plugins/remoteadmin/views.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    18518 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/remoteadmin.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3790 2023-10-19 15:24:17.000000 pypeman-0.5.5/pypeman/test.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-10-19 15:35:07.293023 pypeman-0.5.5/pypeman.egg-info/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3077 2023-10-19 15:35:07.000000 pypeman-0.5.5/pypeman.egg-info/PKG-INFO
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1259 2023-10-19 15:35:07.000000 pypeman-0.5.5/pypeman.egg-info/SOURCES.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        1 2023-10-19 15:35:07.000000 pypeman-0.5.5/pypeman.egg-info/dependency_links.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       49 2023-10-19 15:35:07.000000 pypeman-0.5.5/pypeman.egg-info/entry_points.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      175 2023-10-19 15:35:07.000000 pypeman-0.5.5/pypeman.egg-info/requires.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        8 2023-10-19 15:35:07.000000 pypeman-0.5.5/pypeman.egg-info/top_level.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      279 2023-10-19 15:35:07.297024 pypeman-0.5.5/setup.cfg
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2312 2023-10-19 15:24:17.000000 pypeman-0.5.5/setup.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:34:40.857996 pypeman-0.5.6/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    11358 2024-05-17 13:22:31.000000 pypeman-0.5.6/LICENSE
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       41 2024-05-17 13:22:31.000000 pypeman-0.5.6/MANIFEST.in
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3077 2024-05-17 13:34:40.857996 pypeman-0.5.6/PKG-INFO
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1928 2024-05-17 13:22:31.000000 pypeman-0.5.6/README.rst
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:34:40.849996 pypeman-0.5.6/pypeman/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       68 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    34582 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/channels.py
+-rwxrwxr-x   0 quentin   (1000) quentin   (1000)    12351 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/commands.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2443 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/conf.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:34:40.853996 pypeman-0.5.6/pypeman/contrib/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/contrib/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3606 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/contrib/csv.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2178 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/contrib/ctx.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8624 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/contrib/ftp.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6750 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/contrib/hl7.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    13244 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/contrib/http.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      803 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/contrib/time.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      971 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/contrib/xml.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2126 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/debug.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1451 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/default_settings.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3433 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/endpoints.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      189 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/errors.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1395 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/events.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2577 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/graph.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:34:40.853996 pypeman-0.5.6/pypeman/helpers/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/helpers/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      421 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/helpers/aio_compat.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3247 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/helpers/cli.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      235 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/helpers/itertools.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1894 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/helpers/lazyload.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      663 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/helpers/logging.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3005 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/helpers/reloader.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1216 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/helpers/sleeper.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      315 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/helpers/tempfile.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1335 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/map_item.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6369 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/message.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    21658 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/msgstore.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    27982 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/nodes.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3906 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/persistence.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3946 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/pjt_templates.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2998 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/plugin_mgr.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:34:40.853996 pypeman-0.5.6/pypeman/plugins/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/plugins/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4262 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/plugins/base.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:34:40.853996 pypeman-0.5.6/pypeman/plugins/remoteadmin/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/plugins/remoteadmin/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      712 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/plugins/remoteadmin/plugin.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1033 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/plugins/remoteadmin/urls.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8801 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/plugins/remoteadmin/views.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    18518 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/remoteadmin.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3790 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/test.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:34:40.853996 pypeman-0.5.6/pypeman/tests/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6135 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/common.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:34:40.857996 pypeman-0.5.6/pypeman/tests/data/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       47 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/data/csv_test_data.csv
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      121 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/data/hl7_test_data.HL7
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       28 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/data/new_meta.meta
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        9 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/data/old_meta.meta
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/data/testfile.ok
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       15 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/data/testfile.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      747 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/pytest_helpers.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:34:40.857996 pypeman-0.5.6/pypeman/tests/settings/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/settings/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       40 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/settings/test_setting_1.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/settings/test_settings_default.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      128 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/settings/test_settings_persistence.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      165 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/settings/test_settings_sqlite_persist.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/settings/test_settings_testloop.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:34:40.857996 pypeman-0.5.6/pypeman/tests/test_app/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_app/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_app/project.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      320 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_app/settings.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      279 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_app/settings2.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:34:40.857996 pypeman-0.5.6/pypeman/tests/test_app_testing/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      138 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_app_testing/project.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       77 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_app_testing/settings.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      313 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_app_testing/tests.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    50783 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_channel.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2680 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_ctx_nodes.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6548 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_debug.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2030 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_graph.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       97 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_import_mods.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      500 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_imports.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4487 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_message.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14281 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_msgstore.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    30338 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_nodes.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6176 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_remoteadmin.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      806 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_settings.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4079 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/test_testing.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2810 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tests/tests_bin.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1407 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tool_commands.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:34:40.857996 pypeman-0.5.6/pypeman/tools/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tools/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1763 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tools/send_from_store.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3396 2024-05-17 13:22:31.000000 pypeman-0.5.6/pypeman/tools/view_store.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-05-17 13:34:40.849996 pypeman-0.5.6/pypeman.egg-info/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3077 2024-05-17 13:34:40.000000 pypeman-0.5.6/pypeman.egg-info/PKG-INFO
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2594 2024-05-17 13:34:40.000000 pypeman-0.5.6/pypeman.egg-info/SOURCES.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        1 2024-05-17 13:34:40.000000 pypeman-0.5.6/pypeman.egg-info/dependency_links.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       91 2024-05-17 13:34:40.000000 pypeman-0.5.6/pypeman.egg-info/entry_points.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      175 2024-05-17 13:34:40.000000 pypeman-0.5.6/pypeman.egg-info/requires.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        8 2024-05-17 13:34:40.000000 pypeman-0.5.6/pypeman.egg-info/top_level.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      279 2024-05-17 13:34:40.857996 pypeman-0.5.6/setup.cfg
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2593 2024-05-17 13:22:31.000000 pypeman-0.5.6/setup.py
```

### Comparing `pypeman-0.5.5/LICENSE` & `pypeman-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/PKG-INFO` & `pypeman-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypeman
-Version: 0.5.5
+Version: 0.5.6
 Summary: Minimalistic but pragmatic ESB / ETL / EAI in Python
 Home-page: https://github.com/mhcomm/pypeman
 Author: Jeremie Pardou
 Author-email: jeremie@jeremiez.net
 License: Apache Software License
 Keywords: esb etl eai pipeline data processing asyncio http ftp hl7
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pypeman-0.5.5/README.rst` & `pypeman-0.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/channels.py` & `pypeman-0.5.6/pypeman/channels.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     :param wait_subchans: Boolean, if set to True, channels will wait for suchannel ends for sending,
     speed response and process a new message
     """
     STARTING, WAITING, PROCESSING, STOPPING, STOPPED = range(5)
     STATE_NAMES = ['STARTING', 'WAITING', 'PROCESSING', 'STOPPING', 'STOPPED']
 
     def __init__(self, name=None, parent_channel=None, loop=None, message_store_factory=None,
-                 wait_subchans=False):
+                 wait_subchans=False, verbose_name=None):
 
         self.uuid = uuid.uuid4()
 
         all_channels.append(self)
         self._nodes = []
         self._node_map = {}
         self._status = BaseChannel.STOPPED
@@ -107,14 +107,18 @@
             self.parent_uids = None
 
         if self.name in _channel_names:
             raise NameError(
                 "Duplicate channel name %r . "
                 "Channel names must be unique !" % self.name
             )
+        if verbose_name:
+            self.verbose_name = verbose_name
+        else:
+            self.verbose_name = self.name
 
         _channel_names.add(self.name)
 
         if loop is None:
             self.loop = asyncio.get_event_loop()
         else:
             self.loop = loop
@@ -388,22 +392,24 @@
                     raise
                 return msg
             except Rejected as exc:
                 self.logger.info("%s REJECT msg %s", str(self), str(msg))
                 msg.chan_exc = exc
                 msg.chan_exc_traceback = traceback.format_exc()
                 await self.message_store.change_message_state(msg_store_id, message.Message.REJECTED)
+                await self.message_store.add_message_meta_infos(msg_store_id, "err_msg", str(exc))
                 if self.reject_nodes and not has_callback:
                     await self.reject_nodes[0].handle(msg.copy())
                 raise
             except Exception as exc:
                 msg.chan_exc = exc
                 msg.chan_exc_traceback = traceback.format_exc()
                 self.logger.error('Error while processing message %s (chan %s)', str(msg), str(self))
                 await self.message_store.change_message_state(msg_store_id, message.Message.ERROR)
+                await self.message_store.add_message_meta_infos(msg_store_id, "err_msg", str(exc))
                 if self.fail_nodes and not has_callback:
                     await self.fail_nodes[0].handle(msg.copy())
                 raise
             finally:
                 self.status = BaseChannel.WAITING
                 self.processed_msgs += 1
                 if self.final_nodes and not has_callback:
@@ -475,14 +481,15 @@
         new_message = msg_dict['message'].renew()
         result = await self.handle(new_message)
         return result
 
     def to_dict(self):
         return {
             'name': self.name,
+            'verbose_name': self.verbose_name,
             'status': BaseChannel.status_id_to_str(self.status),
             'has_message_store': not isinstance(self.message_store, msgstore.NullMessageStore),
             'processed': self.processed_msgs,
         }
 
     def subchannels(self):
         res = []
```

### Comparing `pypeman-0.5.5/pypeman/commands.py` & `pypeman-0.5.6/pypeman/commands.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/conf.py` & `pypeman-0.5.6/pypeman/conf.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/contrib/csv.py` & `pypeman-0.5.6/pypeman/contrib/csv.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/contrib/ctx.py` & `pypeman-0.5.6/pypeman/contrib/ctx.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/contrib/ftp.py` & `pypeman-0.5.6/pypeman/contrib/ftp.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/contrib/hl7.py` & `pypeman-0.5.6/pypeman/contrib/hl7.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/contrib/http.py` & `pypeman-0.5.6/pypeman/contrib/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,18 @@
         if host and sock:
             raise PypemanParamError("There can only be one (parameter host or sock)")
         sock = sock or host or ''
 
         super().__init__(loop=loop, sock=sock, reuse_port=reuse_port)
 
     def add_route(self, *args, **kwargs):
+        """
+        Adds a route to the http server.
+        This is normally called when an http channel is added to this endpoint
+        """
         if self._app is None:
             self._app = web.Application(**self.http_args)
 
         self._app.router.add_route(*args, **kwargs)
 
     async def start(self):
         self.make_socket()
@@ -89,27 +93,39 @@
         else:
             print("No HTTP route.")
             logger.warning("No HTTP route.")
 
 
 class HttpChannel(channels.BaseChannel):
     """
-    Channel that handles Http connection. The Http message is the message payload and some headers
+    Channel that handles Http requests to a given path of the url.
+    The Http message is the message payload and some headers
     become metadata of message. Needs ``aiohttp`` python dependency to work.
 
-    :param endpoint: HTTP endpoint used to get connections.
+    :param endpoint: HTTP endpoint the channel will be using. ( scheme://fqdn:port for example)
     :param method: Method filter.
     :param url: Only matching urls messages will be sent to this channel.
     :param encoding: Encoding of message. Default to 'utf-8'.
+    :param add_headers: if True headers will be added to the message meta data
 
     """
     app = None
 
-    def __init__(self, *args, endpoint=None, method='*', url='/', encoding=None, **kwargs):
+    def __init__(
+        self,
+        *args,
+        endpoint=None,
+        method='*',
+        url='/',
+        encoding=None,
+        add_headers=False,
+        **kwargs
+    ):
         super().__init__(*args, **kwargs)
+        self.add_headers = add_headers
         self.method = method
         self.url = url
         self.encoding = encoding
         if endpoint is None:
             raise TypeError('Missing "endpoint" argument')
         self.http_endpoint = endpoint
 
@@ -128,21 +144,26 @@
         # match infos will be overwritten if coinciding with known keywords like
         # 'url', 'method', . . .
         meta.update({
             'method': request.method,
             'url': str(request.url),
             'get_params': dict(request.query),
             })
+        if self.add_headers:
+            meta["headers"] = [(hdr, val) for (hdr, val) in request.headers.items()]
 
         msg = message.Message(content_type='http_request', payload=content, meta=meta)
         try:
             result = await self.handle(msg)
             encoding = self.encoding or 'utf-8'
             return web.Response(
-                body=str(result.payload).encode(encoding), status=result.meta.get('status', 200))
+                body=str(result.payload).encode(encoding),
+                status=result.meta.get('status', 200),
+                content_type=getattr(result, "content_type", None),
+            )
 
         except channels.Dropped:
             return web.Response(body="Dropped".encode('utf-8'), status=200)
         except Exception as exc:
             logger.exception(
                 "HttpChannel %s raise an error, cannot send 200 speed response, will return 503",
                 str(self))
@@ -172,14 +193,16 @@
                  verify=True, params=None, client_cert=None, cookies=None,
                  binary=False, json=False, send_as_json=False, old_url_parsing=True, **kwargs):
         super().__init__(*args, **kwargs)
         self.url = url
         self.method = method
         self.headers = headers
         self.cookies = cookies
+        if isinstance(auth, tuple):
+            auth = aiohttp.BasicAuth(*auth)
         self.auth = auth
         self.verify = verify
         self.params = params
         self.client_cert = client_cert
         self.url = self.url.replace('%(meta.', '%(')  # TODO: why ???
         self.payload_in_url_dict = 'payload.' in self.url  # TODO: should I remove ?
         self.params_in_url = str_named_param_regex.findall(self.url)
@@ -270,23 +293,24 @@
                     param = param(msg)
                 if isinstance(param, list):
                     for value in param:
                         get_params.append((key, value))
                 else:
                     get_params.append((key, param))
 
-        if isinstance(self.auth, tuple):
-            basic_auth = aiohttp.BasicAuth(self.auth[0], self.auth[1])
-        else:
-            basic_auth = self.auth
+        basic_auth = self.auth
 
         data = None
         if method.lower() in ['put', 'post', 'patch']:
             data = msg.payload
-        async with aiohttp.ClientSession(connector=conn, cookies=cookies) as session:
+        async with aiohttp.ClientSession(
+            connector=conn,
+            cookies=cookies,
+            trust_env=True,  # respect e.g. http_proxy env vars
+        ) as session:
             if self.send_as_json:
                 resp = await session.request(
                         method=method,
                         url=url,
                         auth=basic_auth,
                         headers=headers,
                         params=get_params,
@@ -307,14 +331,15 @@
                 setattr(resp, "content", str(await resp.text()))
         return resp
 
     async def process(self, msg):
         """ handles request """
         resp = await self.handle_request(msg)
         msg.meta["status_code"] = resp.status
+        msg.meta["url"] = str(resp.url)
         resp_content = resp.content
         if self.json:
             try:
                 resp_content = json.loads(resp_content)
             except Exception:
                 logger.exception(
                     "cannot json parse response from url %s (response=%r)",
```

### Comparing `pypeman-0.5.5/pypeman/contrib/time.py` & `pypeman-0.5.6/pypeman/contrib/time.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/contrib/xml.py` & `pypeman-0.5.6/pypeman/contrib/xml.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/debug.py` & `pypeman-0.5.6/pypeman/debug.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/default_settings.py` & `pypeman-0.5.6/pypeman/default_settings.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/endpoints.py` & `pypeman-0.5.6/pypeman/endpoints.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/events.py` & `pypeman-0.5.6/pypeman/events.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/graph.py` & `pypeman-0.5.6/pypeman/graph.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/helpers/cli.py` & `pypeman-0.5.6/pypeman/helpers/cli.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/helpers/lazyload.py` & `pypeman-0.5.6/pypeman/helpers/lazyload.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/helpers/logging.py` & `pypeman-0.5.6/pypeman/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/helpers/reloader.py` & `pypeman-0.5.6/pypeman/helpers/reloader.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/helpers/sleeper.py` & `pypeman-0.5.6/pypeman/helpers/sleeper.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/map_item.py` & `pypeman-0.5.6/pypeman/map_item.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/message.py` & `pypeman-0.5.6/pypeman/message.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/msgstore.py` & `pypeman-0.5.6/pypeman/msgstore.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import dateutil.parser
+import json
 import logging
 import os
 import re
 
 from itertools import islice
 from collections import OrderedDict
 from pathlib import Path
@@ -39,14 +40,32 @@
         """
         Store a message in the store.
 
         :param msg: The message to store.
         :return: Id for this specific message.
         """
 
+    async def add_message_meta_infos(self, id, meta_info_name, info):
+        """
+        Add message meta infos in the store
+
+        :param id: Message specific store id.
+        :param meta_info_name: The name of the meta info to create/update
+        :param info: The info value
+        """
+
+    async def get_message_meta_infos(self, id, meta_info_name=None):
+        """
+        Get message meta infos in the store
+
+        :param id: Message specific store id.
+        :param meta_info_name: (optional) The name of the meta info to get,
+            if not set returns the entire dict
+        """
+
     async def change_message_state(self, id, new_state):
         """
         Change the `id` message state.
 
         :param id: Message specific store id.
         :param new_state: Target state.
         """
@@ -136,14 +155,20 @@
 
     async def store(self, msg):
         return None
 
     async def get(self, id):
         return None
 
+    async def add_message_meta_infos(self, id, meta_info_name, info):
+        return None
+
+    async def get_message_meta_infos(self, id, meta_info_name=None):
+        return None
+
     async def get_preview_str(self, id):
         return None
 
     async def get_msg_content(self, id):
         return None
 
     async def search(self, **kwargs):
@@ -165,14 +190,20 @@
 class FakeMessageStore(MessageStore):
     """ For testing purpose """
 
     async def store(self, msg):
         logger.debug("Should store message %s", msg)
         return 'fake_id'
 
+    async def add_message_meta_infos(self, id, meta_info_name, info):
+        return None
+
+    async def get_message_meta_infos(self, id, meta_info_name=None):
+        return "processed"
+
     async def get(self, id):
         return {'id': id, 'state': 'processed', 'message': None}
 
     async def get_preview_str(self, id):
         return {"id": id, "message_content": "content"}
 
     async def get_msg_content(self, id):
@@ -218,15 +249,21 @@
         msg_id = msg.uuid
         self.messages[msg_id] = {
             'id': msg_id, 'state': Message.PENDING,
             'timestamp': msg.timestamp, 'message': msg.to_dict()}
         return msg_id
 
     async def change_message_state(self, id, new_state):
-        self.messages[id]['state'] = new_state
+        await self.add_message_meta_infos(id, "state", new_state)
+
+    async def add_message_meta_infos(self, id, meta_info_name, info):
+        self.messages[id][meta_info_name] = info
+
+    async def get_message_meta_infos(self, id, meta_info_name=None):
+        return self.messages[id][meta_info_name]
 
     async def get(self, id):
         resp = dict(self.messages[id])
         resp['message'] = Message.from_dict(resp['message'])
         return resp
 
     async def get_preview_str(self, id):
@@ -374,30 +411,96 @@
 
         await self.change_message_state(file_path, Message.PENDING)
 
         self._total += 1
 
         return file_path
 
+    def _is_json_meta(self, id):
+        """Check if the message meta file is a json. If it's not,
+        the message is an old message that doesnt contain other infos in
+        meta except the state
+
+        Args:
+            id (str): The id of the message
+        """
+        meta_fpath = (Path(self.base_path) / id).with_suffix(".meta")
+        if not meta_fpath.exists():
+            return False
+        with meta_fpath.open("r") as fin:
+            try:
+                json.load(fin)
+                return True
+            except json.JSONDecodeError:
+                return False
+
+    def _convert_meta_to_json(self, id):
+        """Convert an old message meta to a new one (json)
+
+        Args:
+            id (str): The id of the message to convert
+        """
+        meta_fpath = (Path(self.base_path) / id).with_suffix(".meta")
+        with meta_fpath.open("r") as fin:
+            state = fin.read()
+        meta_data = {"state": state}
+        with meta_fpath.open("w") as fout:
+            json.dump(meta_data, fout)
+        return meta_data
+
+    async def get_message_meta_infos(self, id, meta_info_name=None):
+        meta_fpath = (Path(self.base_path) / id).with_suffix(".meta")
+        if meta_fpath.exists():
+            is_new_meta_file = self._is_json_meta(id)
+            if not is_new_meta_file:
+                meta_data = self._convert_meta_to_json(id)
+            else:
+                with meta_fpath.open("r") as fin:
+                    meta_data = json.load(fin)
+        else:
+            meta_data = {}
+
+        if meta_info_name:
+            meta_data = meta_data.get(meta_info_name)
+        return meta_data
+
+    async def add_message_meta_infos(self, id, meta_info_name, info):
+        meta_fpath = (Path(self.base_path) / id).with_suffix(".meta")
+        if meta_fpath.exists():
+            is_new_meta_file = self._is_json_meta(id)
+            if not is_new_meta_file:
+                meta_data = self._convert_meta_to_json(id)
+            else:
+                with meta_fpath.open("r") as fin:
+                    meta_data = json.load(fin)
+        else:
+            meta_data = {}
+
+        meta_data[meta_info_name] = info
+        with meta_fpath.open("w") as fout:
+            json.dump(meta_data, fout)
+
     async def change_message_state(self, id, new_state):
-        with open(os.path.join(self.base_path, id + '.meta'), "w") as f:
-            f.write(new_state)
+        await self.add_message_meta_infos(id, "state", new_state)
 
     async def get_message_state(self, id):
-        with open(os.path.join(self.base_path, id + '.meta'), "r") as f:
-            state = f.read()
-            return state
+        return await self.get_message_meta_infos(id, "state")
 
     async def get(self, id):
         if not os.path.exists(os.path.join(self.base_path, id)):
             raise IndexError
 
         with open(os.path.join(self.base_path, id), "rb") as f:
             msg = Message.from_json(f.read().decode('utf-8'))
-            return {'id': id, 'state': await self.get_message_state(id), 'message': msg}
+            return {
+                'id': id,
+                'state': await self.get_message_state(id),
+                'message': msg,
+                "meta": await self.get_message_meta_infos(id)
+            }
 
     async def get_preview_str(self, id):
         msg = await self.get_msg_content(id)
         try:
             msg.payload = str(msg.payload)[:1000]
         except Exception:
             msg.payload = repr(msg.payload)[:1000]
@@ -501,14 +604,18 @@
                             if text:
                                 if not await self.is_txt_in_msg(mid, text):
                                     continue
                             if rtext:
                                 if not await self.is_regex_in_msg(mid, rtext):
                                     continue
                             if start <= position < end:
+                                # TODO: need to do processing of payload
+                                #       before filtering (HL7 / json-str)
+                                # TODO: add filter here
+                                # TODO: can we transfoer into a generator?
                                 result.append(await self.get(mid))
                             position += 1
         return result
 
     async def total(self):
         return self._total
```

### Comparing `pypeman-0.5.5/pypeman/nodes.py` & `pypeman-0.5.6/pypeman/nodes.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/persistence.py` & `pypeman-0.5.6/pypeman/persistence.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 This module contains all persistence related things.
 """
 
 import asyncio
 from concurrent.futures import ThreadPoolExecutor
 from collections import defaultdict
 import importlib
+import logging
 
 from sqlitedict import SqliteDict
 
 from pypeman.conf import settings
 
 SENTINEL = object()
 
+logger = logging.getLogger(__name__)
+
 _backend = None
 
 
 async def get_backend(loop):
     """
     Return the configured backend instance.
 
@@ -29,15 +32,17 @@
             raise Exception("Persistence backend not configured.")
 
         module, _, class_ = settings.PERSISTENCE_BACKEND.rpartition('.')
         loaded_module = importlib.import_module(module)
         _backend = getattr(loaded_module, class_)(loop=loop, **settings.PERSISTENCE_CONFIG)
 
         await _backend.start()
-
+    if _backend.loop != loop:
+        logger.warning("Backend loop not the same as loop argument, changing it")
+        _backend.loop = loop
     return _backend
 
 
 class MemoryBackend():
     """
     Memory persistence backend.
     Only for testing purpose as this is not really persistent.
```

### Comparing `pypeman-0.5.5/pypeman/pjt_templates.py` & `pypeman-0.5.6/pypeman/pjt_templates.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/plugin_mgr.py` & `pypeman-0.5.6/pypeman/plugin_mgr.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/plugins/base.py` & `pypeman-0.5.6/pypeman/plugins/base.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/plugins/remoteadmin/plugin.py` & `pypeman-0.5.6/pypeman/plugins/remoteadmin/plugin.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/plugins/remoteadmin/urls.py` & `pypeman-0.5.6/pypeman/plugins/remoteadmin/urls.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/plugins/remoteadmin/views.py` & `pypeman-0.5.6/pypeman/plugins/remoteadmin/views.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/remoteadmin.py` & `pypeman-0.5.6/pypeman/remoteadmin.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman/test.py` & `pypeman-0.5.6/pypeman/test.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.5/pypeman.egg-info/PKG-INFO` & `pypeman-0.5.6/pypeman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypeman
-Version: 0.5.5
+Version: 0.5.6
 Summary: Minimalistic but pragmatic ESB / ETL / EAI in Python
 Home-page: https://github.com/mhcomm/pypeman
 Author: Jeremie Pardou
 Author-email: jeremie@jeremiez.net
 License: Apache Software License
 Keywords: esb etl eai pipeline data processing asyncio http ftp hl7
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pypeman-0.5.5/setup.py` & `pypeman-0.5.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -37,20 +37,29 @@
 
     license="Apache Software License",
     packages=[
         "pypeman",
         "pypeman.contrib",
         "pypeman.helpers",
         "pypeman.plugins",
-        "pypeman.plugins.remoteadmin"
+        "pypeman.plugins.remoteadmin",
+        "pypeman.tests",
+        "pypeman.tests.test_app",
+        "pypeman.tests.test_app_testing",
+        "pypeman.tests.settings",
+        "pypeman.tools",
     ],
 
+    package_data={
+        "pypeman.tests": ["data/*"],
+    },
     entry_points={
         "console_scripts": [
             "pypeman = pypeman.commands:cli",
+            "pypeman_tool = pypeman.tool_commands:main",
         ]
     },
 
     test_suite="nose.collector",
     install_requires=[
         "click",
         "daemonlite",
```

