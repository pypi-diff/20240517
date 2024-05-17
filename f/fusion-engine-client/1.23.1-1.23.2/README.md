# Comparing `tmp/fusion_engine_client-1.23.1.tar.gz` & `tmp/fusion_engine_client-1.23.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion_engine_client-1.23.1.tar", last modified: Tue May 14 18:18:41 2024, max compression
+gzip compressed data, was "fusion_engine_client-1.23.2.tar", last modified: Fri May 17 17:48:13 2024, max compression
```

## Comparing `fusion_engine_client-1.23.1.tar` & `fusion_engine_client-1.23.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.956756 fusion_engine_client-1.23.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-14 18:18:41.956756 fusion_engine_client-1.23.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14885 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.944756 fusion_engine_client-1.23.1/fusion_engine_client/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.948756 fusion_engine_client-1.23.1/fusion_engine_client/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   128072 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/analysis/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/analysis/attitude.py
--rw-r--r--   0 runner    (1001) docker     (127)    47575 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/analysis/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.948756 fusion_engine_client-1.23.1/fusion_engine_client/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/applications/import_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      313 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/applications/p1_display.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4443 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/applications/p1_extract.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6809 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/applications/p1_lband_extract.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16262 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/applications/p1_print.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.952756 fusion_engine_client-1.23.1/fusion_engine_client/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62220 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/control.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    29955 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/fault_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/gnss_corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/measurement_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    50595 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/measurements.py
--rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/ros.py
--rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/signal_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    35741 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/messages/timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.952756 fusion_engine_client-1.23.1/fusion_engine_client/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17531 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/parsers/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/parsers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/parsers/fast_indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24420 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/parsers/file_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    28048 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/parsers/mixed_log_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.952756 fusion_engine_client-1.23.1/fusion_engine_client/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16721 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/bin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24918 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/time_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/fusion_engine_client/utils/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.956756 fusion_engine_client-1.23.1/fusion_engine_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-14 18:18:41.000000 fusion_engine_client-1.23.1/fusion_engine_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-14 18:18:41.000000 fusion_engine_client-1.23.1/fusion_engine_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:18:41.000000 fusion_engine_client-1.23.1/fusion_engine_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-14 18:18:41.000000 fusion_engine_client-1.23.1/fusion_engine_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-14 18:18:41.000000 fusion_engine_client-1.23.1/fusion_engine_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 18:18:41.000000 fusion_engine_client-1.23.1/fusion_engine_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 18:18:41.956756 fusion_engine_client-1.23.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:18:41.956756 fusion_engine_client-1.23.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19673 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_file_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_message_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_mixed_log_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13200 2024-05-14 18:18:08.000000 fusion_engine_client-1.23.1/tests/test_time_range.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:48:13.789488 fusion_engine_client-1.23.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-17 17:48:13.789488 fusion_engine_client-1.23.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14885 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:48:13.777488 fusion_engine_client-1.23.2/fusion_engine_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:48:13.781488 fusion_engine_client-1.23.2/fusion_engine_client/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   128072 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/analysis/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/analysis/attitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47575 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/analysis/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:48:13.781488 fusion_engine_client-1.23.2/fusion_engine_client/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/applications/import_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      313 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/applications/p1_display.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4443 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/applications/p1_extract.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6809 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/applications/p1_lband_extract.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16262 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/applications/p1_print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:48:13.785488 fusion_engine_client-1.23.2/fusion_engine_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63450 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/messages/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/messages/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/messages/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29955 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/messages/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/messages/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/messages/fault_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/messages/gnss_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/messages/measurement_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50595 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/messages/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/messages/ros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/messages/signal_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35741 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/messages/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/messages/timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:48:13.785488 fusion_engine_client-1.23.2/fusion_engine_client/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17531 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/parsers/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/parsers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/parsers/fast_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24420 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/parsers/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28048 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/parsers/mixed_log_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:48:13.785488 fusion_engine_client-1.23.2/fusion_engine_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16721 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/utils/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/utils/bin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/utils/construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/utils/enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24918 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/utils/time_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/fusion_engine_client/utils/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:48:13.789488 fusion_engine_client-1.23.2/fusion_engine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-17 17:48:13.000000 fusion_engine_client-1.23.2/fusion_engine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-17 17:48:13.000000 fusion_engine_client-1.23.2/fusion_engine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 17:48:13.000000 fusion_engine_client-1.23.2/fusion_engine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-17 17:48:13.000000 fusion_engine_client-1.23.2/fusion_engine_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-17 17:48:13.000000 fusion_engine_client-1.23.2/fusion_engine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-17 17:48:13.000000 fusion_engine_client-1.23.2/fusion_engine_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 17:48:13.789488 fusion_engine_client-1.23.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:48:13.789488 fusion_engine_client-1.23.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/tests/test_construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19673 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/tests/test_enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/tests/test_file_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/tests/test_message_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/tests/test_mixed_log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13200 2024-05-17 17:47:38.000000 fusion_engine_client-1.23.2/tests/test_time_range.py
```

### Comparing `fusion_engine_client-1.23.1/PKG-INFO` & `fusion_engine_client-1.23.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.23.1
+Version: 1.23.2
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
-Download-URL: https://github.com/PointOneNav/fusion-engine-client/archive/refs/tags/v1.23.1.tar.gz
+Download-URL: https://github.com/PointOneNav/fusion-engine-client/archive/refs/tags/v1.23.2.tar.gz
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
@@ -23,25 +23,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: construct>=2.10.0
-Requires-Dist: numpy>=1.16.0
+Requires-Dist: packaging>=21.0.0
 Requires-Dist: p1-gpstime>=0.6.3.dev1
+Requires-Dist: construct>=2.10.0
+Requires-Dist: aenum>=3.1.1
 Requires-Dist: argparse-formatter>=1.4
-Requires-Dist: packaging>=21.0.0
-Requires-Dist: pymap3d>=2.4.3
+Requires-Dist: colorama>=0.4.4
 Requires-Dist: plotly>=4.0.0
-Requires-Dist: scipy>=1.5.0
 Requires-Dist: palettable>=3.3.0
-Requires-Dist: colorama>=0.4.4
-Requires-Dist: aenum>=3.1.1
+Requires-Dist: pymap3d>=2.4.3
+Requires-Dist: numpy>=1.16.0
+Requires-Dist: scipy>=1.5.0
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: display
 Provides-Extra: tools
 
 Point One FusionEngine protocol support for real-time interaction and control, plus post-processing data analysis tools.
```

### Comparing `fusion_engine_client-1.23.1/README.md` & `fusion_engine_client-1.23.2/README.md`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/analysis/analyzer.py` & `fusion_engine_client-1.23.2/fusion_engine_client/analysis/analyzer.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/analysis/attitude.py` & `fusion_engine_client-1.23.2/fusion_engine_client/analysis/attitude.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/analysis/data_loader.py` & `fusion_engine_client-1.23.2/fusion_engine_client/analysis/data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/applications/import_utils.py` & `fusion_engine_client-1.23.2/fusion_engine_client/applications/import_utils.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/applications/p1_extract.py` & `fusion_engine_client-1.23.2/fusion_engine_client/applications/p1_extract.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/applications/p1_lband_extract.py` & `fusion_engine_client-1.23.2/fusion_engine_client/applications/p1_lband_extract.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/applications/p1_print.py` & `fusion_engine_client-1.23.2/fusion_engine_client/applications/p1_print.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/messages/configuration.py` & `fusion_engine_client-1.23.2/fusion_engine_client/messages/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 class InterfaceConfigType(IntEnum):
   INVALID = 0
   OUTPUT_DIAGNOSTICS_MESSAGES = 1
   BAUD_RATE = 2
   REMOTE_ADDRESS = 3
   PORT = 4
   ENABLED = 5
+  DIRECTION = 6
+  SOCKET_TYPE = 7
 
 
 class Direction(IntEnum):
     ## Aligned with vehicle +x axis.
     FORWARD = 0
     ## Aligned with vehicle -x axis.
     BACKWARD = 1
@@ -150,25 +152,39 @@
     FORWARD_ACTIVE_LOW = 2
 
 
 class TransportType(IntEnum):
     INVALID = 0
     SERIAL = 1
     FILE = 2
-    TCP_CLIENT = 3
-    TCP_SERVER = 4
-    UDP_CLIENT = 5
-    UDP_SERVER = 6
-    WEBSOCKET_SERVER = 7
+    # RESERVED  3
+    TCP = 4
+    UDP = 5
+    # RESERVED = 6
+    WEBSOCKET = 7
+    UNIX = 8
     ## Set/get the configuration for the interface on which the command was received.
     CURRENT = 254
     ## Set/get the configuration for the all I/O interfaces.
     ALL = 255
 
 
+class TransportDirection(IntEnum):
+    INVALID = 0
+    SERVER = 1
+    CLIENT = 2
+
+
+class SocketType(IntEnum):
+    INVALID = 0
+    STREAM = 1
+    DATAGRAM = 2
+    SEQPACKET = 3
+
+
 class UpdateAction(IntEnum):
     REPLACE = 0
 
 
 class ProtocolType(IntEnum):
     INVALID = 0
     FUSION_ENGINE = 1
@@ -410,14 +426,25 @@
         value: bool = False
 
     # Construct to serialize 8 bit boolean types.
     BoolConstruct = Struct(
         "value" / Flag,
     )
 
+    # Enum helpers.
+    @staticmethod
+    def _define_enum_classes(enum_type, construct_type=Int8ul):
+        class EnumVal(NamedTuple):
+            value: enum_type = list(enum_type)[0]
+        construct = AutoEnum(construct_type, enum_type)
+        return EnumVal, construct
+
+    TransportDirectionVal, TransportDirectionConstruct = _define_enum_classes(TransportDirection, Int8ul)
+    SocketTypeVal, SocketTypeConstruct = _define_enum_classes(SocketType, Int8ul)
+
     class StringVal(NamedTuple):
         """!
         @brief String value specifier.
         """
         value: str = ""
 
     @staticmethod
@@ -903,42 +930,63 @@
 @_conf_gen.create_config_class(ConfigType.HEADING_BIAS, _conf_gen.HeadingBiasConstruct)
 class HeadingBias(_conf_gen.HeadingBias):
     """!
     @brief Horizontal and vertical heading bias.
     """
     pass
 
+
 @_conf_gen.create_interface_config_class(InterfaceConfigType.BAUD_RATE, _conf_gen.UInt32Construct)
 class InterfaceBaudRateConfig(_conf_gen.IntegerVal):
     """!
     @brief Interface baud configuration settings.
     """
     pass
 
+
 @_conf_gen.create_interface_config_class(InterfaceConfigType.PORT, _conf_gen.UInt16Construct)
 class InterfacePortConfig(_conf_gen.IntegerVal):
     """!
     @brief Interface network port configuration settings.
     """
     pass
 
+
 @_conf_gen.create_interface_config_class(InterfaceConfigType.REMOTE_ADDRESS, _conf_gen.StringConstruct(64))
 class InterfaceRemoteAddressConfig(_conf_gen.StringVal):
     """!
     @brief Configure the network address for a client to connect to.
     """
     pass
 
+
 @_conf_gen.create_interface_config_class(InterfaceConfigType.ENABLED, _conf_gen.BoolConstruct)
 class InterfaceEnabledConfig(_conf_gen.BoolVal):
     """!
     @brief Interface enabled/disabled configuration settings.
     """
     pass
 
+
+@_conf_gen.create_interface_config_class(InterfaceConfigType.DIRECTION, _conf_gen.TransportDirectionConstruct)
+class InterfaceDirectionConfig(_conf_gen.TransportDirectionVal):
+    """!
+    @brief Interface transport direction (client/server) configuration settings.
+    """
+    pass
+
+
+@_conf_gen.create_interface_config_class(InterfaceConfigType.SOCKET_TYPE, _conf_gen.SocketTypeConstruct)
+class InterfaceSocketTypeConfig(_conf_gen.SocketTypeVal):
+    """!
+    @brief UNIX domain socket type configuration (stream, datagram, sequence).
+    """
+    pass
+
+
 @_conf_gen.create_interface_config_class(InterfaceConfigType.OUTPUT_DIAGNOSTICS_MESSAGES, _conf_gen.BoolConstruct)
 class InterfaceDiagnosticMessagesEnabled(_conf_gen.BoolVal):
     """!
     @brief Enable/disable output of diagnostic data on this interface.
     """
     pass
```

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/messages/control.py` & `fusion_engine_client-1.23.2/fusion_engine_client/messages/control.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/messages/defs.py` & `fusion_engine_client-1.23.2/fusion_engine_client/messages/defs.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/messages/device.py` & `fusion_engine_client-1.23.2/fusion_engine_client/messages/device.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/messages/fault_control.py` & `fusion_engine_client-1.23.2/fusion_engine_client/messages/fault_control.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/messages/gnss_corrections.py` & `fusion_engine_client-1.23.2/fusion_engine_client/messages/gnss_corrections.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/messages/measurement_details.py` & `fusion_engine_client-1.23.2/fusion_engine_client/messages/measurement_details.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/messages/measurements.py` & `fusion_engine_client-1.23.2/fusion_engine_client/messages/measurements.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/messages/ros.py` & `fusion_engine_client-1.23.2/fusion_engine_client/messages/ros.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/messages/signal_defs.py` & `fusion_engine_client-1.23.2/fusion_engine_client/messages/signal_defs.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/messages/solution.py` & `fusion_engine_client-1.23.2/fusion_engine_client/messages/solution.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/messages/timestamp.py` & `fusion_engine_client-1.23.2/fusion_engine_client/messages/timestamp.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/parsers/decoder.py` & `fusion_engine_client-1.23.2/fusion_engine_client/parsers/decoder.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/parsers/encoder.py` & `fusion_engine_client-1.23.2/fusion_engine_client/parsers/encoder.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/parsers/fast_indexer.py` & `fusion_engine_client-1.23.2/fusion_engine_client/parsers/fast_indexer.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/parsers/file_index.py` & `fusion_engine_client-1.23.2/fusion_engine_client/parsers/file_index.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/parsers/mixed_log_reader.py` & `fusion_engine_client-1.23.2/fusion_engine_client/parsers/mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/utils/argument_parser.py` & `fusion_engine_client-1.23.2/fusion_engine_client/utils/argument_parser.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/utils/bin_utils.py` & `fusion_engine_client-1.23.2/fusion_engine_client/utils/bin_utils.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/utils/construct_utils.py` & `fusion_engine_client-1.23.2/fusion_engine_client/utils/construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/utils/enum_utils.py` & `fusion_engine_client-1.23.2/fusion_engine_client/utils/enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/utils/log.py` & `fusion_engine_client-1.23.2/fusion_engine_client/utils/log.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/utils/numpy_utils.py` & `fusion_engine_client-1.23.2/fusion_engine_client/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/utils/time_range.py` & `fusion_engine_client-1.23.2/fusion_engine_client/utils/time_range.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client/utils/trace.py` & `fusion_engine_client-1.23.2/fusion_engine_client/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client.egg-info/PKG-INFO` & `fusion_engine_client-1.23.2/fusion_engine_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.23.1
+Version: 1.23.2
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
-Download-URL: https://github.com/PointOneNav/fusion-engine-client/archive/refs/tags/v1.23.1.tar.gz
+Download-URL: https://github.com/PointOneNav/fusion-engine-client/archive/refs/tags/v1.23.2.tar.gz
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
@@ -23,25 +23,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: construct>=2.10.0
-Requires-Dist: numpy>=1.16.0
+Requires-Dist: packaging>=21.0.0
 Requires-Dist: p1-gpstime>=0.6.3.dev1
+Requires-Dist: construct>=2.10.0
+Requires-Dist: aenum>=3.1.1
 Requires-Dist: argparse-formatter>=1.4
-Requires-Dist: packaging>=21.0.0
-Requires-Dist: pymap3d>=2.4.3
+Requires-Dist: colorama>=0.4.4
 Requires-Dist: plotly>=4.0.0
-Requires-Dist: scipy>=1.5.0
 Requires-Dist: palettable>=3.3.0
-Requires-Dist: colorama>=0.4.4
-Requires-Dist: aenum>=3.1.1
+Requires-Dist: pymap3d>=2.4.3
+Requires-Dist: numpy>=1.16.0
+Requires-Dist: scipy>=1.5.0
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: display
 Provides-Extra: tools
 
 Point One FusionEngine protocol support for real-time interaction and control, plus post-processing data analysis tools.
```

### Comparing `fusion_engine_client-1.23.1/fusion_engine_client.egg-info/SOURCES.txt` & `fusion_engine_client-1.23.2/fusion_engine_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/setup.py` & `fusion_engine_client-1.23.2/setup.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/tests/test_config.py` & `fusion_engine_client-1.23.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/tests/test_construct_utils.py` & `fusion_engine_client-1.23.2/tests/test_construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/tests/test_data_loader.py` & `fusion_engine_client-1.23.2/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/tests/test_decoder.py` & `fusion_engine_client-1.23.2/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/tests/test_encoder.py` & `fusion_engine_client-1.23.2/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/tests/test_enum_utils.py` & `fusion_engine_client-1.23.2/tests/test_enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/tests/test_file_index.py` & `fusion_engine_client-1.23.2/tests/test_file_index.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/tests/test_message_defs.py` & `fusion_engine_client-1.23.2/tests/test_message_defs.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/tests/test_mixed_log_reader.py` & `fusion_engine_client-1.23.2/tests/test_mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion_engine_client-1.23.1/tests/test_time_range.py` & `fusion_engine_client-1.23.2/tests/test_time_range.py`

 * *Files identical despite different names*

