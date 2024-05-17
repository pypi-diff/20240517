# Comparing `tmp/influxdb3-python-0.3.6.tar.gz` & `tmp/influxdb3_python-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-0.3.6.tar", last modified: Thu Jan 25 13:26:18 2024, max compression
+gzip compressed data, was "influxdb3_python-0.4.0.tar", last modified: Wed Apr 17 18:23:23 2024, max compression
```

## Comparing `influxdb3-python-0.3.6.tar` & `influxdb3_python-0.4.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:26:18.501917 influxdb3-python-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-01-25 13:26:18.501917 influxdb3-python-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:26:18.501917 influxdb3-python-0.3.6/influxdb3_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-01-25 13:26:18.000000 influxdb3-python-0.3.6/influxdb3_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-01-25 13:26:18.000000 influxdb3-python-0.3.6/influxdb3_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 13:26:18.000000 influxdb3-python-0.3.6/influxdb3_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-25 13:26:18.000000 influxdb3-python-0.3.6/influxdb3_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-25 13:26:18.000000 influxdb3-python-0.3.6/influxdb3_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:26:18.493917 influxdb3-python-0.3.6/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/read_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:26:18.497918 influxdb3-python-0.3.6/influxdb_client_3/write_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:26:18.497918 influxdb3-python-0.3.6/influxdb_client_3/write_client/_sync/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26797 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/_sync/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15251 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/_sync/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:26:18.497918 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13794 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/influxdb_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/logging_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:26:18.497918 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/util/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/util/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/util/date_utils_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/util/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/util/multiprocessing_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:26:18.497918 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/write/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21344 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/write/dataframe_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/write/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/write/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    25431 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/client/write_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:26:18.497918 influxdb3-python-0.3.6/influxdb_client_3/write_client/domain/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/domain/write_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:26:18.501917 influxdb3-python-0.3.6/influxdb_client_3/write_client/service/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/service/_base_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/service/signin_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/service/signout_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    20552 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/service/write_service.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/influxdb_client_3/write_client/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 13:26:18.501917 influxdb3-python-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:26:18.501917 influxdb3-python-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-01-25 13:26:04.000000 influxdb3-python-0.3.6/tests/test_influxdb_client_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:23:23.633221 influxdb3_python-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-04-17 18:23:23.633221 influxdb3_python-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:23:23.633221 influxdb3_python-0.4.0/influxdb3_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-04-17 18:23:23.000000 influxdb3_python-0.4.0/influxdb3_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-17 18:23:23.000000 influxdb3_python-0.4.0/influxdb3_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 18:23:23.000000 influxdb3_python-0.4.0/influxdb3_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-17 18:23:23.000000 influxdb3_python-0.4.0/influxdb3_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 18:23:23.000000 influxdb3_python-0.4.0/influxdb3_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:23:23.625221 influxdb3_python-0.4.0/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11143 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/read_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:23:23.625221 influxdb3_python-0.4.0/influxdb_client_3/write_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:23:23.625221 influxdb3_python-0.4.0/influxdb_client_3/write_client/_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26917 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/_sync/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15251 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/_sync/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:23:23.629221 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13771 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/influxdb_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/logging_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:23:23.629221 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/util/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/util/date_utils_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/util/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/util/multiprocessing_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:23:23.629221 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/write/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21502 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/write/dataframe_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/write/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/write/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25554 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/client/write_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:23:23.629221 influxdb3_python-0.4.0/influxdb_client_3/write_client/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/domain/write_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:23:23.629221 influxdb3_python-0.4.0/influxdb_client_3/write_client/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/service/_base_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/service/signin_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/service/signout_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20552 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/service/write_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/influxdb_client_3/write_client/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 18:23:23.633221 influxdb3_python-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:23:23.633221 influxdb3_python-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/tests/test_dataframe_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-17 18:23:17.000000 influxdb3_python-0.4.0/tests/test_influxdb_client_3.py
```

### Comparing `influxdb3-python-0.3.6/LICENSE` & `influxdb3_python-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/PKG-INFO` & `influxdb3_python-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.3.6
+Version: 0.4.0
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: reactivex>=4.0.4
 Requires-Dist: certifi>=14.05.14
 Requires-Dist: python_dateutil>=2.5.3
 Requires-Dist: setuptools>=21.0.0
 Requires-Dist: urllib3>=1.26.0
@@ -36,19 +37,22 @@
 <p align="center">
     <a href="https://pypi.org/project/influxdb3-python/">
         <img src="https://img.shields.io/pypi/v/influxdb3-python.svg" alt="PyPI version">
     </a>
     <a href="https://pypi.org/project/influxdb3-python/">
         <img src="https://img.shields.io/pypi/dm/influxdb3-python.svg" alt="PyPI downloads">
     </a>
-    <a href="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/pylint.yml">
-        <img src="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/pylint.yml/badge.svg" alt="Lint Code Base">
+    <a href="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/codeql-analysis.yml">
+        <img src="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/codeql-analysis.yml/badge.svg?branch=main" alt="CodeQL analysis">
     </a>
-        <a href="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/python-publish.yml">
-        <img src="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/python-publish.yml/badge.svg" alt="Lint Code Base">
+    <a href="https://dl.circleci.com/status-badge/redirect/gh/InfluxCommunity/influxdb3-python/tree/main">
+        <img src="https://dl.circleci.com/status-badge/img/gh/InfluxCommunity/influxdb3-python/tree/main.svg?style=svg" alt="CircleCI">
+    </a>
+    <a href="https://codecov.io/gh/InfluxCommunity/influxdb3-python">
+        <img src="https://codecov.io/gh/InfluxCommunity/influxdb3-python/branch/main/graph/badge.svg" alt="Code Cov"/>
     </a>
     <a href="https://influxcommunity.slack.com">
         <img src="https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&style=social" alt="Community Slack">
     </a>
 </p>
 
 # InfluxDB 3.0 Python Client
```

### Comparing `influxdb3-python-0.3.6/README.md` & `influxdb3_python-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 <p align="center">
     <a href="https://pypi.org/project/influxdb3-python/">
         <img src="https://img.shields.io/pypi/v/influxdb3-python.svg" alt="PyPI version">
     </a>
     <a href="https://pypi.org/project/influxdb3-python/">
         <img src="https://img.shields.io/pypi/dm/influxdb3-python.svg" alt="PyPI downloads">
     </a>
-    <a href="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/pylint.yml">
-        <img src="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/pylint.yml/badge.svg" alt="Lint Code Base">
+    <a href="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/codeql-analysis.yml">
+        <img src="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/codeql-analysis.yml/badge.svg?branch=main" alt="CodeQL analysis">
     </a>
-        <a href="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/python-publish.yml">
-        <img src="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/python-publish.yml/badge.svg" alt="Lint Code Base">
+    <a href="https://dl.circleci.com/status-badge/redirect/gh/InfluxCommunity/influxdb3-python/tree/main">
+        <img src="https://dl.circleci.com/status-badge/img/gh/InfluxCommunity/influxdb3-python/tree/main.svg?style=svg" alt="CircleCI">
+    </a>
+    <a href="https://codecov.io/gh/InfluxCommunity/influxdb3-python">
+        <img src="https://codecov.io/gh/InfluxCommunity/influxdb3-python/branch/main/graph/badge.svg" alt="Code Cov"/>
     </a>
     <a href="https://influxcommunity.slack.com">
         <img src="https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&style=social" alt="Community Slack">
     </a>
 </p>
 
 # InfluxDB 3.0 Python Client
```

### Comparing `influxdb3-python-0.3.6/influxdb3_python.egg-info/PKG-INFO` & `influxdb3_python-0.4.0/influxdb3_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.3.6
+Version: 0.4.0
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: reactivex>=4.0.4
 Requires-Dist: certifi>=14.05.14
 Requires-Dist: python_dateutil>=2.5.3
 Requires-Dist: setuptools>=21.0.0
 Requires-Dist: urllib3>=1.26.0
@@ -36,19 +37,22 @@
 <p align="center">
     <a href="https://pypi.org/project/influxdb3-python/">
         <img src="https://img.shields.io/pypi/v/influxdb3-python.svg" alt="PyPI version">
     </a>
     <a href="https://pypi.org/project/influxdb3-python/">
         <img src="https://img.shields.io/pypi/dm/influxdb3-python.svg" alt="PyPI downloads">
     </a>
-    <a href="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/pylint.yml">
-        <img src="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/pylint.yml/badge.svg" alt="Lint Code Base">
+    <a href="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/codeql-analysis.yml">
+        <img src="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/codeql-analysis.yml/badge.svg?branch=main" alt="CodeQL analysis">
     </a>
-        <a href="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/python-publish.yml">
-        <img src="https://github.com/InfluxCommunity/influxdb3-python/actions/workflows/python-publish.yml/badge.svg" alt="Lint Code Base">
+    <a href="https://dl.circleci.com/status-badge/redirect/gh/InfluxCommunity/influxdb3-python/tree/main">
+        <img src="https://dl.circleci.com/status-badge/img/gh/InfluxCommunity/influxdb3-python/tree/main.svg?style=svg" alt="CircleCI">
+    </a>
+    <a href="https://codecov.io/gh/InfluxCommunity/influxdb3-python">
+        <img src="https://codecov.io/gh/InfluxCommunity/influxdb3-python/branch/main/graph/badge.svg" alt="Code Cov"/>
     </a>
     <a href="https://influxcommunity.slack.com">
         <img src="https://img.shields.io/badge/slack-join_chat-white.svg?logo=slack&style=social" alt="Community Slack">
     </a>
 </p>
 
 # InfluxDB 3.0 Python Client
```

### Comparing `influxdb3-python-0.3.6/influxdb3_python.egg-info/SOURCES.txt` & `influxdb3_python-0.4.0/influxdb3_python.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,8 +35,9 @@
 influxdb_client_3/write_client/domain/__init__.py
 influxdb_client_3/write_client/domain/write_precision.py
 influxdb_client_3/write_client/service/__init__.py
 influxdb_client_3/write_client/service/_base_service.py
 influxdb_client_3/write_client/service/signin_service.py
 influxdb_client_3/write_client/service/signout_service.py
 influxdb_client_3/write_client/service/write_service.py
+tests/test_dataframe_serializer.py
 tests/test_influxdb_client_3.py
```

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/__init__.py` & `influxdb3_python-0.4.0/influxdb_client_3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,60 @@
-import urllib.parse, json
+import json
+import urllib.parse
+
 import pyarrow as pa
-from influxdb_client_3.write_client import InfluxDBClient as _InfluxDBClient, WriteOptions, Point
-from influxdb_client_3.write_client.client.write_api import WriteApi as _WriteApi, SYNCHRONOUS, ASYNCHRONOUS, PointSettings
-from influxdb_client_3.write_client.domain.write_precision import WritePrecision
-from influxdb_client_3.write_client.client.exceptions import InfluxDBError
 from pyarrow.flight import FlightClient, Ticket, FlightCallOptions
+
 from influxdb_client_3.read_file import UploadFile
-import urllib.parse
+from influxdb_client_3.write_client import InfluxDBClient as _InfluxDBClient, WriteOptions, Point
+from influxdb_client_3.write_client.client.exceptions import InfluxDBError
+from influxdb_client_3.write_client.client.write_api import WriteApi as _WriteApi, SYNCHRONOUS, ASYNCHRONOUS, \
+    PointSettings
+from influxdb_client_3.write_client.domain.write_precision import WritePrecision
+
 try:
     import polars as pl
+
     polars = True
 except ImportError:
     polars = False
 
 
-
 def write_client_options(**kwargs):
     """
     Function for providing additional arguments for the WriteApi client.
 
     :param kwargs: Additional arguments for the WriteApi client.
     :return: dict with the arguments.
     """
     return kwargs
 
+
 def default_client_options(**kwargs):
     return kwargs
 
+
 def flight_client_options(**kwargs):
     """
     Function for providing additional arguments for the FlightClient.
 
     :param kwargs: Additional arguments for the FlightClient.
     :return: dict with the arguments.
     """
     return kwargs
 
+
 def file_parser_options(**kwargs):
     """
     Function for providing additional arguments for the file parser.
 
     :param kwargs: Additional arguments for the file parser.
     :return: dict with the arguments.
     """
-    return kwargs  
+    return kwargs
 
 
 def _deep_merge(target, source):
     """
     Performs a deep merge of dictionaries or lists,
     recursively merging the contents, handling nested structures, and concatenation of lists.
     """
@@ -63,14 +70,15 @@
         # If both target and source are lists, concatenate them
         target.extend(source)
     else:
         # For other types, simply replace the target with the source
         target = source
     return target
 
+
 class InfluxDBClient3:
     def __init__(
             self,
             host=None,
             org=None,
             database=None,
             token=None,
@@ -95,50 +103,51 @@
         :param flight_client_options: Function for providing additional arguments for the FlightClient.
         :type flight_client_options: callable
         :param kwargs: Additional arguments for the InfluxDB Client.
         """
         self._org = org if org is not None else "default"
         self._database = database
         self._token = token
-        self._write_client_options = write_client_options if write_client_options is not None else default_client_options(write_options=SYNCHRONOUS)
-        
+        self._write_client_options = write_client_options if write_client_options is not None \
+            else default_client_options(write_options=SYNCHRONOUS)
+
         # Parse the host input
         parsed_url = urllib.parse.urlparse(host)
-        
+
         # Determine the protocol (scheme), hostname, and port
         scheme = parsed_url.scheme if parsed_url.scheme else "https"
         hostname = parsed_url.hostname if parsed_url.hostname else host
         port = parsed_url.port if parsed_url.port else 443
 
         # Construct the clients using the parsed values
         if write_port_overwrite is not None:
             port = write_port_overwrite
 
         self._client = _InfluxDBClient(
             url=f"{scheme}://{hostname}:{port}",
             token=self._token,
             org=self._org,
             **kwargs)
-        
+
         self._write_api = _WriteApi(influxdb_client=self._client, **self._write_client_options)
         self._flight_client_options = flight_client_options or {}
-        
+
         if query_port_overwrite is not None:
             port = query_port_overwrite
         self._flight_client = FlightClient(f"grpc+tls://{hostname}:{port}", **self._flight_client_options)
 
     def _merge_options(self, defaults, custom={}):
         """
         Merge default option arguments with custom (user-provided) arguments.
         """
         if len(custom) == 0:
             return defaults
         return _deep_merge(defaults, {key: value for key, value in custom.items()})
 
-    def write(self, record=None, database=None ,**kwargs):
+    def write(self, record=None, database=None, **kwargs):
         """
         Write data to InfluxDB.
 
         :param record: The data point(s) to write.
         :type record: object or list of objects
         :param database: The database to write to. If not provided, uses the database provided during initialization.
         :type database: str
@@ -147,17 +156,17 @@
         if database is None:
             database = self._database
 
         try:
             self._write_api.write(bucket=database, record=record, **kwargs)
         except InfluxDBError as e:
             raise e
-          
 
-    def write_file(self, file, measurement_name=None, tag_columns=None, timestamp_column='time', database=None, file_parser_options=None ,**kwargs):
+    def write_file(self, file, measurement_name=None, tag_columns=None, timestamp_column='time', database=None,
+                   file_parser_options=None, **kwargs):
         """
         Write data from a file to InfluxDB.
 
         :param file: The file to write.
         :type file: str
         :param measurement_name: The name of the measurement.
         :type measurement_name: str
@@ -173,18 +182,18 @@
         """
         if database is None:
             database = self._database
 
         try:
             table = UploadFile(file, file_parser_options).load_file()
             df = table.to_pandas() if isinstance(table, pa.Table) else table
-            self._process_dataframe(df, measurement_name, tag_columns or [], timestamp_column, database=database, **kwargs)
+            self._process_dataframe(df, measurement_name, tag_columns or [], timestamp_column, database=database,
+                                    **kwargs)
         except Exception as e:
             raise e
-            
 
     def _process_dataframe(self, df, measurement_name, tag_columns, timestamp_column, database, **kwargs):
         # This function is factored out for clarity.
         # It processes a DataFrame before writing to InfluxDB.
 
         measurement_column = None
         if measurement_name is None:
@@ -200,17 +209,16 @@
                 print("'measurement' column not found in the dataframe.")
         else:
             df = df.drop(columns=['measurement'], errors='ignore')
             self._write_api.write(bucket=database, record=df,
                                   data_frame_measurement_name=measurement_name,
                                   data_frame_tag_columns=tag_columns,
                                   data_frame_timestamp_column=timestamp_column, **kwargs)
-  
-    
-    def query(self, query, language="sql", mode="all", database=None,**kwargs ):
+
+    def query(self, query, language="sql", mode="all", database=None, **kwargs):
         """
         Query data from InfluxDB.
 
         :param query: The query string.
         :type query: str
         :param language: The query language; "sql" or "influxql" (default is "sql").
         :type language: str
@@ -219,41 +227,39 @@
         :param database: The database to query from. If not provided, uses the database provided during initialization.
         :type database: str
         :param kwargs: FlightClientCallOptions for the query.
         :return: The queried data.
         """
         if mode == "polars" and polars is False:
             raise ImportError("Polars is not installed. Please install it with `pip install polars`.")
-        
-    
 
         if database is None:
             database = self._database
-        
+
         try:
             # Create an authorization header
             optargs = {
                 "headers": [(b"authorization", f"Bearer {self._token}".encode('utf-8'))],
                 "timeout": 300
             }
             opts = self._merge_options(optargs, kwargs)
             _options = FlightCallOptions(**opts)
-            
+
             ticket_data = {"database": database, "sql_query": query, "query_type": language}
             ticket = Ticket(json.dumps(ticket_data).encode('utf-8'))
             flight_reader = self._flight_client.do_get(ticket, _options)
 
             mode_func = {
                 "all": flight_reader.read_all,
                 "pandas": flight_reader.read_pandas,
                 "polars": lambda: pl.from_arrow(flight_reader.read_all()),
                 "chunk": lambda: flight_reader,
                 "reader": flight_reader.to_reader,
                 "schema": lambda: flight_reader.schema
-                
+
             }.get(mode, flight_reader.read_all)
 
             return mode_func() if callable(mode_func) else mode_func
         except Exception as e:
             raise e
 
     def close(self):
@@ -263,15 +269,16 @@
         self._client.close()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
-        
+
+
 __all__ = [
     "InfluxDBClient3",
     "Point",
     "PointSettings",
     "SYNCHRONOUS",
     "ASYNCHRONOUS",
     "WritePrecision",
```

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/read_file.py` & `influxdb3_python-0.4.0/influxdb_client_3/read_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     import pyarrow.orc as orc
 
 
 class UploadFile:
     """
     Class for uploading and reading different types of files.
     """
+
     def __init__(self, file, file_parser_options=None):
         """
         Initialize an UploadFile instance.
 
         :param file: The file to upload.
         :type file: str
         :param kwargs: Additional arguments for file loading functions.
@@ -40,15 +41,15 @@
         elif self._file.endswith(".json"):
             return self.load_json(self._file)
         elif self._file.endswith(".orc"):
             return self.load_orc(self._file)
         else:
             raise ValueError("Unsupported file type")
 
-    def load_feather(self, file ):
+    def load_feather(self, file):
         """
         Load a Feather file.
 
         :param file: The Feather file to load.
         :type file: str
         :return: The loaded Feather file.
         """
@@ -95,10 +96,11 @@
         :param file: The JSON file to load.
         :type file: str
         :return: The loaded JSON file.
         """
         try:
             import pandas as pd
         except ImportError:
-            raise ImportError("Pandas is required for write_file(). Please install it using 'pip install pandas' or 'pip install influxdb3-python[pandas]'")
-        
-        return pd.read_json(file, **self._kwargs)
+            raise ImportError("Pandas is required for write_file(). Please install it using 'pip install pandas' or "
+                              "'pip install influxdb3-python[pandas]'")
+
+        return pd.read_json(file, **self._kwargs)
```

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/__init__.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/__init__.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/_sync/api_client.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/_sync/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,15 @@
         :param klass: class literal, or string of class name.
 
         :return: object.
         """
         if data is None:
             return None
 
-        if type(klass) == str:
+        if klass is str:
             if klass.startswith('list['):
                 sub_kls = re.match(r'list\[(.*)\]', klass).group(1)
                 return [self.__deserialize(sub_data, sub_kls)
                         for sub_data in data]
 
             if klass.startswith('dict('):
                 sub_kls = re.match(r'dict\(([^,]*), (.*)\)', klass).group(2)
@@ -344,21 +344,21 @@
                                    path_params, query_params, header_params,
                                    body, post_params, files,
                                    response_type, auth_settings,
                                    _return_http_data_only, collection_formats,
                                    _preload_content, _request_timeout, urlopen_kw)
         else:
             thread = self.pool.apply_async(self.__call_api, (resource_path,
-                                           method, path_params, query_params,
-                                           header_params, body,
-                                           post_params, files,
-                                           response_type, auth_settings,
-                                           _return_http_data_only,
-                                           collection_formats,
-                                           _preload_content, _request_timeout, urlopen_kw))
+                                                             method, path_params, query_params,
+                                                             header_params, body,
+                                                             post_params, files,
+                                                             response_type, auth_settings,
+                                                             _return_http_data_only,
+                                                             collection_formats,
+                                                             _preload_content, _request_timeout, urlopen_kw))
         return thread
 
     def request(self, method, url, query_params=None, headers=None,
                 post_params=None, body=None, _preload_content=True,
                 _request_timeout=None, **urlopen_kw):
         """Make the HTTP request using RESTClient."""
         if method == "GET":
```

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/_sync/rest.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/_sync/rest.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/client/__init__.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/client/_base.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/client/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """Commons function for Sync and Async client."""
 from __future__ import absolute_import
 
 import base64
 import configparser
 import logging
 import os
-from datetime import datetime, timedelta
-from typing import List, Generator, Any, Union, Iterable, AsyncGenerator
-
-from urllib3 import HTTPResponse
+from typing import Iterable
 
+from influxdb_client_3.write_client.client.write.dataframe_serializer import DataframeSerializer, \
+    PolarsDataframeSerializer
 from influxdb_client_3.write_client.configuration import Configuration
-from influxdb_client_3.write_client.service.write_service import WriteService
-
-from influxdb_client_3.write_client.client.write.dataframe_serializer import DataframeSerializer, PolarsDataframeSerializer
 from influxdb_client_3.write_client.rest import _UTF_8_encoding
+from influxdb_client_3.write_client.service.write_service import WriteService
 
 try:
     import dataclasses
 
     _HAS_DATACLASS = True
 except ModuleNotFoundError:
     _HAS_DATACLASS = False
@@ -204,15 +201,14 @@
         return cls(url, token, debug=debug, timeout=_to_int(timeout), org=org, default_tags=default_tags,
                    enable_gzip=enable_gzip, verify_ssl=_to_bool(verify_ssl), ssl_ca_cert=ssl_ca_cert,
                    cert_file=cert_file, cert_key_file=cert_key_file, cert_key_password=cert_key_password,
                    connection_pool_maxsize=_to_int(connection_pool_maxsize), auth_basic=_to_bool(auth_basic),
                    profilers=profilers, **kwargs)
 
 
-  
 class _BaseWriteApi(object):
     def __init__(self, influxdb_client, point_settings=None):
         self._influxdb_client = influxdb_client
         self._point_settings = point_settings
         self._write_service = WriteService(influxdb_client.api_client)
         if influxdb_client.default_tags:
             for key, value in influxdb_client.default_tags.items():
@@ -256,26 +252,24 @@
             serializer = PolarsDataframeSerializer(record, self._point_settings, write_precision, **kwargs)
             self._serialize(serializer.serialize(), write_precision, payload, **kwargs)
 
         elif 'pandas' in str(type(record)):
             serializer = DataframeSerializer(record, self._point_settings, write_precision, **kwargs)
             self._serialize(serializer.serialize(), write_precision, payload, **kwargs)
 
-
         elif hasattr(record, "_asdict"):
             # noinspection PyProtectedMember
             self._serialize(record._asdict(), write_precision, payload, **kwargs)
         elif _HAS_DATACLASS and dataclasses.is_dataclass(record):
             self._serialize(dataclasses.asdict(record), write_precision, payload, **kwargs)
         elif isinstance(record, Iterable):
             for item in record:
                 self._serialize(item, write_precision, payload, **kwargs)
 
 
-
 class _Configuration(Configuration):
     def __init__(self):
         Configuration.__init__(self)
         self.enable_gzip = False
         self.username = None
         self.password = None
```

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/client/exceptions.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/client/influxdb_client.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/client/influxdb_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """InfluxDBClient is client for API defined in https://github.com/influxdata/influxdb/blob/master/http/swagger.yml."""
 
 from __future__ import absolute_import
 
 import logging
-import warnings
-
 
 from influxdb_client_3.write_client.client._base import _BaseClient
 from influxdb_client_3.write_client.client.write_api import WriteApi, WriteOptions, PointSettings
 
 logger = logging.getLogger('influxdb_client_3.write_client.client.influxdb_client')
 
 
@@ -280,22 +278,16 @@
                                 - `Exception`: an retryable error
 
                              **[batching mode]**
         :return: write api instance
         """
         return WriteApi(influxdb_client=self, write_options=write_options, point_settings=point_settings, **kwargs)
 
-
     def close(self):
         """Shutdown the client."""
         self.__del__()
 
     def __del__(self):
         """Shutdown the client."""
         if self.api_client:
             self.api_client.__del__()
             self.api_client = None
-
-
-
-
-
```

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/client/logging_handler.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/client/logging_handler.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/client/util/date_utils.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/client/util/date_utils.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/client/util/date_utils_pandas.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/client/util/date_utils_pandas.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/client/util/helpers.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/client/util/helpers.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/client/util/multiprocessing_helper.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/client/util/multiprocessing_helper.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/client/warnings.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/client/warnings.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/client/write/__init__.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/client/write/__init__.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/client/write/dataframe_serializer.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/client/write/dataframe_serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 """
 
 import logging
 import math
 import re
 
 from influxdb_client_3.write_client.domain import WritePrecision
-from influxdb_client_3.write_client.client.write.point import _ESCAPE_KEY, _ESCAPE_STRING, _ESCAPE_MEASUREMENT, DEFAULT_WRITE_PRECISION
+from influxdb_client_3.write_client.client.write.point import _ESCAPE_KEY, _ESCAPE_STRING, _ESCAPE_MEASUREMENT, \
+    DEFAULT_WRITE_PRECISION
 
 logger = logging.getLogger('influxdb_client.client.write.dataframe_serializer')
 
 
+def _not_nan(x):
+    from ...extras import pd
+    return not pd.isna(x)
+
+
 def _itertuples(data_frame):
     cols = [data_frame.iloc[:, k] for k in range(len(data_frame.columns))]
     return zip(data_frame.index, *cols)
 
 
-def _not_nan(x):
-    return x == x
-
-
 def _any_not_nan(p, indexes):
     return any(map(lambda x: _not_nan(p[x]), indexes))
 
 
 class DataframeSerializer:
     """Serialize DataFrame into LineProtocols."""
 
@@ -171,15 +173,15 @@
             field_index = index + 1
             val_format = f'p[{field_index}]'
 
             if key in data_frame_tag_columns:
                 # This column is a tag column.
                 if null_columns.iloc[index]:
                     key_value = f"""{{
-                            '' if {val_format} == '' or type({val_format}) == float and math.isnan({val_format}) else
+                            '' if {val_format} == '' or pd.isna({val_format}) else
                             f',{key_format}={{str({val_format}).translate(_ESCAPE_STRING)}}'
                         }}"""
                 else:
                     key_value = f',{key_format}={{str({val_format}).translate(_ESCAPE_KEY)}}'
                 tags.append(key_value)
                 continue
             elif timestamp_column is not None and key in timestamp_column:
@@ -187,28 +189,30 @@
                 continue
 
             # This column is a field column.
             # Note: no comma separator is needed for the first field.
             # It's important to omit it because when the first
             # field column has no nulls, we don't run the comma-removal
             # regexp substitution step.
+
             sep = '' if len(field_indexes) == 0 else ','
-            if issubclass(value.type, np.integer):
-                field_value = f"{sep}{key_format}={{{val_format}}}i"
-            elif issubclass(value.type, np.bool_):
-                field_value = f'{sep}{key_format}={{{val_format}}}'
-            elif issubclass(value.type, np.floating):
+
+            if (issubclass(value.type, np.integer) or issubclass(value.type, np.floating) or
+                    issubclass(value.type, np.bool_)):
+                suffix = 'i' if issubclass(value.type, np.integer) else ''
                 if null_columns.iloc[index]:
-                    field_value = f"""{{"" if math.isnan({val_format}) else f"{sep}{key_format}={{{val_format}}}"}}"""
+                    field_value = (
+                        f"""{{"" if pd.isna({val_format}) else f"{sep}{key_format}={{{val_format}}}{suffix}"}}"""
+                    )
                 else:
-                    field_value = f'{sep}{key_format}={{{val_format}}}'
+                    field_value = f'{sep}{key_format}={{{val_format}}}{suffix}'
             else:
                 if null_columns.iloc[index]:
                     field_value = f"""{{
-                            '' if type({val_format}) == float and math.isnan({val_format}) else
+                            '' if pd.isna({val_format}) else
                             f'{sep}{key_format}="{{str({val_format}).translate(_ESCAPE_STRING)}}"'
                         }}"""
                 else:
                     field_value = f'''{sep}{key_format}="{{str({val_format}).translate(_ESCAPE_STRING)}}"'''
             field_indexes.append(field_index)
             fields.append(field_value)
 
@@ -225,15 +229,15 @@
             timestamp = '{int(p[%s].value / 1e9)}' % timestamp_index
 
         f = eval(f'lambda p: f"""{{measurement_name}}{tags} {fields} {timestamp}"""', {
             'measurement_name': measurement_name,
             '_ESCAPE_KEY': _ESCAPE_KEY,
             '_ESCAPE_STRING': _ESCAPE_STRING,
             'keys': keys,
-            'math': math,
+            'pd': pd,
         })
 
         for k, v in dict(data_frame.dtypes).items():
             if k in data_frame_tag_columns:
                 data_frame[k].replace('', np.nan, inplace=True)
 
         self.data_frame = data_frame
@@ -293,133 +297,128 @@
         :param precision: The precision for the unix timestamps within the body line-protocol.
         :param chunk_size: The size of chunk for serializing into chunks.
         :key data_frame_measurement_name: name of measurement for writing Polars DataFrame
         :key data_frame_tag_columns: list of DataFrame columns which are tags, rest columns will be fields
         :key data_frame_timestamp_column: name of DataFrame column which contains a timestamp.
         :key data_frame_timestamp_timezone: name of the timezone which is used for timestamp column
         """
-        
-        
+
         self.data_frame = data_frame
         self.point_settings = point_settings
         self.precision = precision
         self.chunk_size = chunk_size
         self.measurement_name = kwargs.get("data_frame_measurement_name", "measurement")
         self.tag_columns = kwargs.get("data_frame_tag_columns", [])
         self.timestamp_column = kwargs.get("data_frame_timestamp_column", None)
         self.timestamp_timezone = kwargs.get("data_frame_timestamp_timezone", None)
 
         self.column_indices = {name: index for index, name in enumerate(data_frame.columns)}
 
         if self.timestamp_column is None or self.timestamp_column not in self.column_indices:
-            raise ValueError(f"Timestamp column {self.timestamp_column} not found in DataFrame. Please define a valid timestamp column.")
+            raise ValueError(
+                f"Timestamp column {self.timestamp_column} not found in DataFrame. Please define a valid timestamp "
+                f"column.")
 
         #
         # prepare chunks
         #
         if chunk_size is not None:
             self.number_of_chunks = int(math.ceil(len(data_frame) / float(chunk_size)))
             self.chunk_size = chunk_size
         else:
             self.number_of_chunks = None
-    
-    def escape_key(self,value):
+
+    def escape_key(self, value):
         return str(value).translate(_ESCAPE_KEY)
-    
-    def escape_value(self,value):
+
+    def escape_value(self, value):
         return str(value).translate(_ESCAPE_STRING)
 
-    
     def to_line_protocol(self, row):
         # Filter out None or empty values for tags
         tags = ""
-      
+
         tags = ",".join(
-            f'{self.escape_key(col)}={self.escape_key(row[self.column_indices[col]])}' 
+            f'{self.escape_key(col)}={self.escape_key(row[self.column_indices[col]])}'
             for col in self.tag_columns
             if row[self.column_indices[col]] is not None and row[self.column_indices[col]] != ""
         )
 
         if self.point_settings.defaultTags:
             default_tags = ",".join(
                 f'{self.escape_key(key)}={self.escape_key(value)}'
                 for key, value in self.point_settings.defaultTags.items()
             )
             # Ensure there's a comma between existing tags and default tags if both are present
             if tags and default_tags:
                 tags += ","
             tags += default_tags
-    
-
 
-        
         # add escape symbols for special characters to tags
 
         fields = ",".join(
-            f"{col}=\"{self.escape_value(row[self.column_indices[col]])}\"" if isinstance(row[self.column_indices[col]], str)
-            else f"{col}={str(row[self.column_indices[col]]).lower()}" if isinstance(row[self.column_indices[col]], bool)  # Check for bool first
+            f"{col}=\"{self.escape_value(row[self.column_indices[col]])}\"" if isinstance(row[self.column_indices[col]],
+                                                                                          str)
+            else f"{col}={str(row[self.column_indices[col]]).lower()}" if isinstance(row[self.column_indices[col]],
+                                                                                     bool)  # Check for bool first
             else f"{col}={row[self.column_indices[col]]}i" if isinstance(row[self.column_indices[col]], int)
             else f"{col}={row[self.column_indices[col]]}"
             for col in self.column_indices
-            if col not in self.tag_columns + [self.timestamp_column]
-            and row[self.column_indices[col]] is not None and row[self.column_indices[col]] != ""
+            if col not in self.tag_columns + [self.timestamp_column] and
+            row[self.column_indices[col]] is not None and row[self.column_indices[col]] != ""
         )
 
-
         # Access the Unix timestamp
         timestamp = row[self.column_indices[self.timestamp_column]]
         if tags != "":
             line_protocol = f"{self.measurement_name},{tags} {fields} {timestamp}"
         else:
             line_protocol = f"{self.measurement_name} {fields} {timestamp}"
 
         return line_protocol
 
-    
     def serialize(self, chunk_idx: int = None):
         from ...extras import pl
-        
+
         df = self.data_frame
 
         # Check if the timestamp column is already an integer
         if df[self.timestamp_column].dtype in [pl.Int32, pl.Int64]:
             # The timestamp column is already an integer, assuming it's in Unix format
             pass
         else:
             # Convert timestamp to Unix timestamp based on specified precision
             if self.precision in [None, 'ns']:
-                df = df.with_columns(pl.col(self.timestamp_column).dt.epoch(time_unit="ns").alias(self.timestamp_column))
+                df = df.with_columns(
+                    pl.col(self.timestamp_column).dt.epoch(time_unit="ns").alias(self.timestamp_column))
             elif self.precision == 'us':
-                df = df.with_columns(pl.col(self.timestamp_column).dt.epoch(time_unit="us").alias(self.timestamp_column))
+                df = df.with_columns(
+                    pl.col(self.timestamp_column).dt.epoch(time_unit="us").alias(self.timestamp_column))
             elif self.precision == 'ms':
-                df = df.with_columns(pl.col(self.timestamp_column).dt.epoch(time_unit="ms").alias(self.timestamp_column))
+                df = df.with_columns(
+                    pl.col(self.timestamp_column).dt.epoch(time_unit="ms").alias(self.timestamp_column))
             elif self.precision == 's':
                 df = df.with_columns(pl.col(self.timestamp_column).dt.epoch(time_unit="s").alias(self.timestamp_column))
             else:
                 raise ValueError(f"Unsupported precision: {self.precision}")
-        
+
         if chunk_idx is None:
             chunk = df
         else:
             logger.debug("Serialize chunk %s/%s ...", chunk_idx + 1, self.number_of_chunks)
             chunk = df[chunk_idx * self.chunk_size:(chunk_idx + 1) * self.chunk_size]
 
         # Apply the UDF to each row
-        line_protocol_expr = chunk.apply(self.to_line_protocol,return_dtype=pl.Object)
+        line_protocol_expr = chunk.apply(self.to_line_protocol, return_dtype=pl.Object)
 
         lp = line_protocol_expr['map'].to_list()
 
-
         return lp
 
 
-
-     
-
-
 def data_frame_to_list_of_points(data_frame, point_settings, precision=DEFAULT_WRITE_PRECISION, **kwargs):
     """
     Serialize DataFrame into LineProtocols.
 
     :param data_frame: Pandas DataFrame to serialize
     :param point_settings: Default Tags
     :param precision: The precision for the unix timestamps within the body line-protocol.
@@ -428,22 +427,23 @@
     :key data_frame_timestamp_column: name of DataFrame column which contains a timestamp. The column can be defined as a :class:`~str` value
                                       formatted as `2018-10-26`, `2018-10-26 12:00`, `2018-10-26 12:00:00-05:00`
                                       or other formats and types supported by `pandas.to_datetime <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.to_datetime.html#pandas.to_datetime>`_ - ``DataFrame``
     :key data_frame_timestamp_timezone: name of the timezone which is used for timestamp column - ``DataFrame``
     """  # noqa: E501
     return DataframeSerializer(data_frame, point_settings, precision, **kwargs).serialize()
 
+
 def polars_data_frame_to_list_of_points(data_frame, point_settings, precision=DEFAULT_WRITE_PRECISION, **kwargs):
     """
     Serialize DataFrame into LineProtocols.
 
     :param data_frame: Pandas DataFrame to serialize
     :param point_settings: Default Tags
     :param precision: The precision for the unix timestamps within the body line-protocol.
     :key data_frame_measurement_name: name of measurement for writing Pandas DataFrame
     :key data_frame_tag_columns: list of DataFrame columns which are tags, rest columns will be fields
     :key data_frame_timestamp_column: name of DataFrame column which contains a timestamp. The column can be defined as a :class:`~str` value
                                       formatted as `2018-10-26`, `2018-10-26 12:00`, `2018-10-26 12:00:00-05:00`
                                       or other formats and types supported by `pandas.to_datetime <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.to_datetime.html#pandas.to_datetime>`_ - ``DataFrame``
     :key data_frame_timestamp_timezone: name of the timezone which is used for timestamp column - ``DataFrame``
     """  # noqa: E501
-    return PolarsDataframeSerializer(data_frame, point_settings, precision, **kwargs).serialize()
+    return PolarsDataframeSerializer(data_frame, point_settings, precision, **kwargs).serialize()
```

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/client/write/point.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/client/write/point.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/client/write/retry.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/client/write/retry.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/client/write_api.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/client/write_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 from reactivex import operators as ops, Observable
 from reactivex.scheduler import ThreadPoolScheduler
 from reactivex.subject import Subject
 
 from influxdb_client_3.write_client.domain import WritePrecision
 from influxdb_client_3.write_client.client._base import _BaseWriteApi, _HAS_DATACLASS
 from influxdb_client_3.write_client.client.util.helpers import get_org_query_param
-from influxdb_client_3.write_client.client.write.dataframe_serializer import DataframeSerializer, PolarsDataframeSerializer
+from influxdb_client_3.write_client.client.write.dataframe_serializer import (DataframeSerializer,
+                                                                              PolarsDataframeSerializer)
 from influxdb_client_3.write_client.client.write.point import Point, DEFAULT_WRITE_PRECISION
 from influxdb_client_3.write_client.client.write.retry import WritesRetry
 from influxdb_client_3.write_client.rest import _UTF_8_encoding
 
 logger = logging.getLogger('influxdb_client_3.write_client.client.write_api')
 
-
 if _HAS_DATACLASS:
     import dataclasses
     from dataclasses import dataclass
 
 
 class WriteType(Enum):
     """Configuration which type of writes will client use."""
@@ -456,32 +456,32 @@
 
         elif isinstance(data, Point):
             self._write_batching(bucket, org, data.to_line_protocol(), data.write_precision, **kwargs)
 
         elif isinstance(data, dict):
             self._write_batching(bucket, org, Point.from_dict(data, write_precision=precision, **kwargs),
                                  precision, **kwargs)
-            
+
         elif 'polars' in str(type(data)):
-            serializer = PolarsDataframeSerializer(data, self._point_settings, precision, self._write_options.batch_size,
-                                             **kwargs)
+            serializer = PolarsDataframeSerializer(data,
+                                                   self._point_settings, precision,
+                                                   self._write_options.batch_size, **kwargs)
             for chunk_idx in range(serializer.number_of_chunks):
                 self._write_batching(bucket, org,
                                      serializer.serialize(chunk_idx),
                                      precision, **kwargs)
 
         elif 'pandas' in str(type(data)):
             serializer = DataframeSerializer(data, self._point_settings, precision, self._write_options.batch_size,
                                              **kwargs)
             for chunk_idx in range(serializer.number_of_chunks):
                 self._write_batching(bucket, org,
                                      serializer.serialize(chunk_idx),
                                      precision, **kwargs)
 
-
         elif hasattr(data, "_asdict"):
             # noinspection PyProtectedMember
             self._write_batching(bucket, org, data._asdict(), precision, **kwargs)
 
         elif _HAS_DATACLASS and dataclasses.is_dataclass(data):
             self._write_batching(bucket, org, dataclasses.asdict(data), precision, **kwargs)
```

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/configuration.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/configuration.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/domain/write_precision.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/domain/write_precision.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/extras.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/extras.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/rest.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/rest.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/service/__init__.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/service/__init__.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/service/_base_service.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/service/_base_service.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/service/signin_service.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/service/signin_service.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/service/signout_service.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/service/signout_service.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/influxdb_client_3/write_client/service/write_service.py` & `influxdb3_python-0.4.0/influxdb_client_3/write_client/service/write_service.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.3.6/setup.py` & `influxdb3_python-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,18 +43,19 @@
     long_description_content_type="text/markdown",
     author='InfluxData',
     author_email='contact@influxdata.com',
     url='https://github.com/InfluxCommunity/influxdb3-python',
     packages=find_packages(exclude=['tests', 'tests.*', 'examples', 'examples.*']),
     extras_require={'pandas': ['pandas'], 'polars': ['polars'], 'dataframe': ['pandas', 'polars']},
     install_requires=requires,
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ]
-)
+)
```

### Comparing `influxdb3-python-0.3.6/tests/test_influxdb_client_3.py` & `influxdb3_python-0.4.0/tests/test_influxdb_client_3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import unittest
-from unittest.mock import patch, Mock
+from unittest.mock import patch
+
 from influxdb_client_3 import InfluxDBClient3
 
+
 class TestInfluxDBClient3(unittest.TestCase):
 
     @patch('influxdb_client_3._InfluxDBClient')
     @patch('influxdb_client_3._WriteApi')
     @patch('influxdb_client_3.FlightClient')
     def setUp(self, mock_flight_client, mock_write_api, mock_influx_db_client):
         self.mock_influx_db_client = mock_influx_db_client
@@ -21,18 +23,10 @@
     def test_init(self):
         self.assertEqual(self.client._org, "my_org")
         self.assertEqual(self.client._database, "my_db")
         self.assertEqual(self.client._client, self.mock_influx_db_client.return_value)
         self.assertEqual(self.client._write_api, self.mock_write_api.return_value)
         self.assertEqual(self.client._flight_client, self.mock_flight_client.return_value)
 
-    @patch('influxdb_client_3._WriteApi.write')
-    def test_write(self, mock_write):
-        record = "test_record"
-        self.client.write(record=record)
-        mock_write.assert_called_once_with(bucket=self.client._database, record=record)
-
-    # Add more tests for other methods
-
 
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

