# Comparing `tmp/farm_ng_core-2.2.0.tar.gz` & `tmp/farm_ng_core-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "farm_ng_core-2.2.0.tar", last modified: Wed Jan 17 00:00:54 2024, max compression
+gzip compressed data, was "farm_ng_core-2.3.0.tar", last modified: Fri May 17 20:16:39 2024, max compression
```

## Comparing `farm_ng_core-2.2.0.tar` & `farm_ng_core-2.3.0.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:00:54.345028 farm_ng_core-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-01-17 00:00:54.345028 farm_ng_core-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:00:54.329028 farm_ng_core-2.2.0/cpp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:00:54.329028 farm_ng_core-2.2.0/cpp/farm_ng/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:00:54.329028 farm_ng_core-2.2.0/cpp/farm_ng/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:00:54.333028 farm_ng_core-2.2.0/cpp/farm_ng/core/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/cpp/farm_ng/core/logging/backtrace.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/cpp/farm_ng/core/logging/expected.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/cpp/farm_ng/core/logging/format.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/cpp/farm_ng/core/logging/logger.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:00:54.329028 farm_ng_core-2.2.0/py/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:00:54.329028 farm_ng_core-2.2.0/py/farm_ng/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:00:54.341028 farm_ng_core-2.2.0/py/farm_ng/core/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/py/farm_ng/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/calculus.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/calculus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/calculus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/calculus_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/color.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/color_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/color_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/color_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/event.proto
--rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/py/farm_ng/core/event_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/py/farm_ng/core/event_client_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/event_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/event_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/event_service.proto
--rw-r--r--   0 runner    (1001) docker     (127)    18859 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/py/farm_ng/core/event_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/py/farm_ng/core/event_service_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/event_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/event_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/event_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19929 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/py/farm_ng/core/event_service_recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/py/farm_ng/core/event_service_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)    11169 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/py/farm_ng/core/events_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10452 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/py/farm_ng/core/events_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/examples.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/examples_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/examples_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/examples_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/geometry.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/geometry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/geometry_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/geometry_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/image.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/image_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/image_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/image_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/lie.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/lie_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/lie_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/lie_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/linalg.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/linalg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/linalg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/linalg_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/pose.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/pose_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/pose_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/pose_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/py/farm_ng/core/pose_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/sensor.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/sensor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/sensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/sensor_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/py/farm_ng/core/stamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/std.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/std_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/std_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/std_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/timestamp.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/timestamp_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/timestamp_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/timestamp_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/uri.proto
--rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/py/farm_ng/core/uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/uri_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/uri_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng/core/uri_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:00:54.345028 farm_ng_core-2.2.0/py/farm_ng_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-17 00:00:54.000000 farm_ng_core-2.2.0/py/farm_ng_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:00:54.345028 farm_ng_core-2.2.0/py/pybind/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/py/pybind/farm_ng_core_pybind.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/py/pybind/lie_pybind.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/py/pybind/linalg_pybind.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-01-17 00:00:54.345028 farm_ng_core-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-01-17 00:00:43.000000 farm_ng_core-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:16:39.980167 farm_ng_core-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-05-17 20:16:39.980167 farm_ng_core-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:16:39.956167 farm_ng_core-2.3.0/cpp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:16:39.956167 farm_ng_core-2.3.0/cpp/farm_ng/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:16:39.956167 farm_ng_core-2.3.0/cpp/farm_ng/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:16:39.960167 farm_ng_core-2.3.0/cpp/farm_ng/core/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/cpp/farm_ng/core/logging/backtrace.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/cpp/farm_ng/core/logging/expected.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/cpp/farm_ng/core/logging/format.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/cpp/farm_ng/core/logging/logger.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:16:39.960167 farm_ng_core-2.3.0/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:16:39.960167 farm_ng_core-2.3.0/py/farm_ng/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:16:39.976167 farm_ng_core-2.3.0/py/farm_ng/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/py/farm_ng/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/calculus.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/calculus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/calculus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/calculus_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/color.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/color_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/color_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/color_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/event.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/py/farm_ng/core/event_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/py/farm_ng/core/event_client_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/event_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/event_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/event_service.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    18859 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/py/farm_ng/core/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/py/farm_ng/core/event_service_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/event_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/event_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/event_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19929 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/py/farm_ng/core/event_service_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/py/farm_ng/core/event_service_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11169 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/py/farm_ng/core/events_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/py/farm_ng/core/events_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/examples.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/examples_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/examples_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/examples_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/geometry.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/geometry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/geometry_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/geometry_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/image.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/image_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/image_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/image_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/lie.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/lie_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/lie_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/lie_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/linalg.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/linalg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/linalg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/linalg_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/pose.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/pose_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/pose_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/pose_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/py/farm_ng/core/pose_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/sensor.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/sensor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/sensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/sensor_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/py/farm_ng/core/stamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/std.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/std_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/std_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/std_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/timestamp.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/timestamp_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/timestamp_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/timestamp_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/uri.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/py/farm_ng/core/uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/uri_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/uri_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng/core/uri_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:16:39.976167 farm_ng_core-2.3.0/py/farm_ng_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 20:16:39.000000 farm_ng_core-2.3.0/py/farm_ng_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:16:39.976167 farm_ng_core-2.3.0/py/pybind/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/py/pybind/farm_ng_core_pybind.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/py/pybind/lie_pybind.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/py/pybind/linalg_pybind.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-17 20:16:39.980167 farm_ng_core-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-17 20:16:32.000000 farm_ng_core-2.3.0/setup.py
```

### Comparing `farm_ng_core-2.2.0/LICENSE` & `farm_ng_core-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/PKG-INFO` & `farm_ng_core-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: farm_ng_core
-Version: 2.2.0
+Version: 2.3.0
 Home-page: https://github.com/farm-ng/farm-ng-core
 Download-URL: https://github.com/farm-ng/farm-ng-core
 Author: Farm-ng Inc.
 Author-email: info@farm-ng.com
 Keywords: robotics,open-source
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: farm_ng_core Version: 2.2.0 Home-page: https://
+Metadata-Version: 2.1 Name: farm_ng_core Version: 2.3.0 Home-page: https://
 github.com/farm-ng/farm-ng-core Download-URL: https://github.com/farm-ng/farm-
 ng-core Author: Farm-ng Inc. Author-email: info@farm-ng.com Keywords:
 robotics,open-source Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
 Classifier: Framework :: Robot Framework Requires-Python: >=3.8 Description-
```

### Comparing `farm_ng_core-2.2.0/README.md` & `farm_ng_core-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/cpp/farm_ng/core/logging/backtrace.cpp` & `farm_ng_core-2.3.0/cpp/farm_ng/core/logging/backtrace.cpp`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/cpp/farm_ng/core/logging/expected.cpp` & `farm_ng_core-2.3.0/cpp/farm_ng/core/logging/expected.cpp`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/cpp/farm_ng/core/logging/format.cpp` & `farm_ng_core-2.3.0/cpp/farm_ng/core/logging/format.cpp`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/cpp/farm_ng/core/logging/logger.cpp` & `farm_ng_core-2.3.0/cpp/farm_ng/core/logging/logger.cpp`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/calculus.proto` & `farm_ng_core-2.3.0/py/farm_ng/core/calculus.proto`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/calculus_pb2.py` & `farm_ng_core-2.3.0/py/farm_ng/core/calculus_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/core/calculus.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -16,16 +16,16 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66\x61rm_ng/core/calculus.proto\x12\x12\x66\x61rm_ng.core.proto\x1a\x19\x66\x61rm_ng/core/linalg.proto\"7\n\tRegionI32\x12\x10\n\x08is_empty\x18\x01 \x01(\x08\x12\x0b\n\x03min\x18\x02 \x01(\x05\x12\x0b\n\x03max\x18\x03 \x01(\x05\"7\n\tRegionF32\x12\x10\n\x08is_empty\x18\x01 \x01(\x08\x12\x0b\n\x03min\x18\x02 \x01(\x02\x12\x0b\n\x03max\x18\x03 \x01(\x02\"7\n\tRegionF64\x12\x10\n\x08is_empty\x18\x01 \x01(\x08\x12\x0b\n\x03min\x18\x02 \x01(\x01\x12\x0b\n\x03max\x18\x03 \x01(\x01\"r\n\nRegion2F64\x12\x10\n\x08is_empty\x18\x01 \x01(\x08\x12(\n\x03min\x18\x02 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec2F64\x12(\n\x03max\x18\x03 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec2F64\"E\n\x14RepeatedG0Region2F64\x12-\n\x05value\x18\x01 \x03(\x0b\x32\x1e.farm_ng.core.proto.Region2F64b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.core.calculus_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_REGIONI32']._serialized_start=78
   _globals['_REGIONI32']._serialized_end=133
   _globals['_REGIONF32']._serialized_start=135
   _globals['_REGIONF32']._serialized_end=190
   _globals['_REGIONF64']._serialized_start=192
   _globals['_REGIONF64']._serialized_end=247
   _globals['_REGION2F64']._serialized_start=249
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/calculus_pb2.pyi` & `farm_ng_core-2.3.0/py/farm_ng/core/calculus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/color.proto` & `farm_ng_core-2.3.0/py/farm_ng/core/color.proto`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/color_pb2.py` & `farm_ng_core-2.3.0/py/farm_ng/core/color_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/core/color.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,12 +15,12 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x66\x61rm_ng/core/color.proto\x12\x12\x66\x61rm_ng.core.proto\"3\n\x05\x43olor\x12\t\n\x01r\x18\x01 \x01(\x02\x12\t\n\x01g\x18\x02 \x01(\x02\x12\t\n\x01\x62\x18\x03 \x01(\x02\x12\t\n\x01\x61\x18\x04 \x01(\x02\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.core.color_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_COLOR']._serialized_start=48
   _globals['_COLOR']._serialized_end=99
 # @@protoc_insertion_point(module_scope)
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/color_pb2.pyi` & `farm_ng_core-2.3.0/py/farm_ng/core/color_pb2.pyi`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/event.proto` & `farm_ng_core-2.3.0/py/farm_ng/core/event.proto`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/event_client.py` & `farm_ng_core-2.3.0/py/farm_ng/core/event_client.py`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/event_client_manager.py` & `farm_ng_core-2.3.0/py/farm_ng/core/event_client_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from farm_ng.core.event_client import EventClient
 from farm_ng.core.event_service_pb2 import (
     EventServiceConfig,
     EventServiceConfigList,
     SubscribeRequest,
 )
+from farm_ng.core.uri import get_service_name
 from farm_ng.core.uri_pb2 import Uri
 
 __all__ = ["EventClientSubscriptionManager"]
 
 
 class EventClientSubscriptionManager:
     """Class for the event client subscription manager.
@@ -82,45 +83,46 @@
             if config.port is None:
                 msg = "Port is not set for service"
                 raise ValueError(msg)
             # update the service config
             clients.update({config.name: EventClient(config)})
         return clients
 
-    def _try_register_topic(self, service_name: str, uri_path: str) -> bool:
+    def _try_register_topic(self, client_name: str, uri: Uri) -> bool:
         """Attempts to register a topic for a service.
 
         Args:
-            service_name: The name of the service.
-            uri_path: The path of the topic.
+            client_name: The name of the client to register the topic for.
+            uri: The uri to register.
 
         Returns:
             True if the topic was registered successfully, False otherwise.
         """
-        if service_name not in self._clients:
-            self.logger.warning("Service %s not found", service_name)
+        if client_name not in self._clients:
+            self.logger.warning("Service %s not found", client_name)
             return False
 
         # make the key for the subscription map
-        service_path: str = f"{service_name}{uri_path}"
+        service_name = get_service_name(uri)
+        topic_name: str = f"{service_name}{uri.path}"
 
-        if service_path in self._subscriptions:
-            # self.logger.warning("Topic %s already registered", service_path)
+        if topic_name in self._subscriptions:
+            # self.logger.warning("Topic %s already registered", topic_name)
             return False
 
         subscribe_request = SubscribeRequest(
             uri=Uri(
-                path=uri_path,
+                path=uri.path,
                 query=f"service_name={service_name}",
             ),
             every_n=1,
         )
 
-        self.logger.info("Registering topic %s", service_path)
-        self._subscriptions[service_path] = subscribe_request
+        self.logger.info("Registering topic %s for client %s", topic_name, client_name)
+        self._subscriptions[topic_name] = subscribe_request
 
         return True
 
     async def update_subscriptions_for_client(self, client: EventClient) -> None:
         """Updates the subscriptions for a client.
 
         Args:
@@ -129,15 +131,15 @@
         while True:
             # get the list of uris from the client
             uris: list[Uri] = await client.list_uris()
 
             # register the topics
             uri: Uri
             for uri in uris:
-                self._try_register_topic(client.config.name, uri.path)
+                self._try_register_topic(client.config.name, uri)
 
             await asyncio.sleep(1.0)
 
     async def update_subscriptions(self) -> None:
         """Serves the subscriptions once to create the topics in foxglove."""
         tasks: list[asyncio.Task] = []
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/event_pb2.py` & `farm_ng_core-2.3.0/py/farm_ng/core/event_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/core/event.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -17,12 +17,12 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x66\x61rm_ng/core/event.proto\x12\x12\x66\x61rm_ng.core.proto\x1a\x16\x66\x61rm_ng/core/uri.proto\x1a\x1c\x66\x61rm_ng/core/timestamp.proto\"\x8a\x01\n\x05\x45vent\x12$\n\x03uri\x18\x01 \x01(\x0b\x32\x17.farm_ng.core.proto.Uri\x12\x31\n\ntimestamps\x18\x02 \x03(\x0b\x32\x1d.farm_ng.core.proto.Timestamp\x12\x16\n\x0epayload_length\x18\x03 \x01(\x03\x12\x10\n\x08sequence\x18\x04 \x01(\x03\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.core.event_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_EVENT']._serialized_start=103
   _globals['_EVENT']._serialized_end=241
 # @@protoc_insertion_point(module_scope)
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/event_pb2.pyi` & `farm_ng_core-2.3.0/py/farm_ng/core/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/event_service.proto` & `farm_ng_core-2.3.0/py/farm_ng/core/event_service.proto`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/event_service.py` & `farm_ng_core-2.3.0/py/farm_ng/core/event_service.py`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/event_service_metrics.py` & `farm_ng_core-2.3.0/py/farm_ng/core/event_service_metrics.py`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/event_service_pb2.py` & `farm_ng_core-2.3.0/py/farm_ng/core/event_service_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/core/event_service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -17,17 +17,17 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n farm_ng/core/event_service.proto\x12\x12\x66\x61rm_ng.core.proto\x1a\x16\x66\x61rm_ng/core/uri.proto\x1a\x18\x66\x61rm_ng/core/event.proto\"I\n\x10SubscribeRequest\x12$\n\x03uri\x18\x01 \x01(\x0b\x32\x17.farm_ng.core.proto.Uri\x12\x0f\n\x07\x65very_n\x18\x02 \x01(\r\"K\n\x0eSubscribeReply\x12(\n\x05\x65vent\x18\x01 \x01(\x0b\x32\x19.farm_ng.core.proto.Event\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\"P\n\x13RequestReplyRequest\x12(\n\x05\x65vent\x18\x01 \x01(\x0b\x32\x19.farm_ng.core.proto.Event\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\"N\n\x11RequestReplyReply\x12(\n\x05\x65vent\x18\x01 \x01(\x0b\x32\x19.farm_ng.core.proto.Event\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\"~\n\x0cRequestReply\x12\x38\n\x07request\x18\x01 \x01(\x0b\x32\'.farm_ng.core.proto.RequestReplyRequest\x12\x34\n\x05reply\x18\x02 \x01(\x0b\x32%.farm_ng.core.proto.RequestReplyReply\"\x11\n\x0fListUrisRequest\"6\n\rListUrisReply\x12%\n\x04uris\x18\x01 \x03(\x0b\x32\x17.farm_ng.core.proto.Uri\"\xe0\x02\n\x12\x45ventServiceConfig\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x0c\n\x04host\x18\x03 \x01(\t\x12;\n\rsubscriptions\x18\x04 \x03(\x0b\x32$.farm_ng.core.proto.SubscribeRequest\x12%\n\x04uris\x18\x05 \x03(\x0b\x32\x17.farm_ng.core.proto.Uri\x12\x0c\n\x04\x61rgs\x18\x06 \x03(\t\x12\x42\n\tlog_level\x18\x07 \x01(\x0e\x32/.farm_ng.core.proto.EventServiceConfig.LogLevel\"j\n\x08LogLevel\x12\n\n\x06NOTSET\x10\x00\x12\x0c\n\x08\x43RITICAL\x10\x32\x12\t\n\x05\x46\x41TAL\x10\x32\x12\t\n\x05\x45RROR\x10(\x12\x0b\n\x07WARNING\x10\x1e\x12\x08\n\x04WARN\x10\x1e\x12\x08\n\x04INFO\x10\x14\x12\t\n\x05\x44\x45\x42UG\x10\n\x1a\x02\x10\x01\"Q\n\x16\x45ventServiceConfigList\x12\x37\n\x07\x63onfigs\x18\x01 \x03(\x0b\x32&.farm_ng.core.proto.EventServiceConfig2\xa1\x02\n\x0c\x45ventService\x12T\n\x08listUris\x12#.farm_ng.core.proto.ListUrisRequest\x1a!.farm_ng.core.proto.ListUrisReply\"\x00\x12Y\n\tsubscribe\x12$.farm_ng.core.proto.SubscribeRequest\x1a\".farm_ng.core.proto.SubscribeReply\"\x00\x30\x01\x12`\n\x0crequestReply\x12\'.farm_ng.core.proto.RequestReplyRequest\x1a%.farm_ng.core.proto.RequestReplyReply\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.core.event_service_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  _globals['_EVENTSERVICECONFIG_LOGLEVEL']._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
+  _globals['_EVENTSERVICECONFIG_LOGLEVEL']._loaded_options = None
   _globals['_EVENTSERVICECONFIG_LOGLEVEL']._serialized_options = b'\020\001'
   _globals['_SUBSCRIBEREQUEST']._serialized_start=106
   _globals['_SUBSCRIBEREQUEST']._serialized_end=179
   _globals['_SUBSCRIBEREPLY']._serialized_start=181
   _globals['_SUBSCRIBEREPLY']._serialized_end=256
   _globals['_REQUESTREPLYREQUEST']._serialized_start=258
   _globals['_REQUESTREPLYREQUEST']._serialized_end=338
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/event_service_pb2.pyi` & `farm_ng_core-2.3.0/py/farm_ng/core/event_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/event_service_recorder.py` & `farm_ng_core-2.3.0/py/farm_ng/core/event_service_recorder.py`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/event_service_tool.py` & `farm_ng_core-2.3.0/py/farm_ng/core/event_service_tool.py`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/events_file_reader.py` & `farm_ng_core-2.3.0/py/farm_ng/core/events_file_reader.py`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/events_file_writer.py` & `farm_ng_core-2.3.0/py/farm_ng/core/events_file_writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,33 +21,43 @@
 
 __all__ = [
     "EventsFileWriter",
     "proto_to_json_file",
 ]
 
 
-def proto_to_json_file(file_path: str | Path, proto_message: Message) -> bool:
+def proto_to_json_file(
+    file_path: str | Path,
+    proto_message: Message,
+    preserving_proto_field_name=False,
+) -> bool:
     """Write a proto Message to a JSON file. The parent directory of the file must exist.
 
     Args:
         file_path (str | Path): The path to the JSON file to create / overwrite.
         proto_message (Message): The proto message to write to the JSON file.
+        preserving_proto_field_name (bool): See MessageToJson in https://googleapis.dev/python/protobuf/latest/google/protobuf/json_format.html
 
     Returns:
         True if the file was written successfully, False otherwise.
     """
     if isinstance(file_path, str):
         file_path = Path(file_path).absolute()
 
     if not file_path.parent.is_dir():
         print(f"Invalid directory: {file_path.parent!s}")
         return False
 
     with Path(file_path).open("w", encoding="utf-8") as file:
-        file.write(MessageToJson(proto_message))
+        file.write(
+            MessageToJson(
+                proto_message,
+                preserving_proto_field_name=preserving_proto_field_name,
+            ),
+        )
         file.write("\n")
 
     return True
 
 
 class EventsFileWriter:
     """Write events to a file."""
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/examples.proto` & `farm_ng_core-2.3.0/py/farm_ng/core/examples.proto`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/examples_pb2.py` & `farm_ng_core-2.3.0/py/farm_ng/core/examples_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/core/examples.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,14 +15,14 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66\x61rm_ng/core/examples.proto\x12\x12\x66\x61rm_ng.core.proto\",\n\x0eStructExample1\x12\x0f\n\x07integer\x18\x01 \x01(\x01\x12\t\n\x01\x66\x18\x02 \x01(\x02\"O\n\x0eStructExample2\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\x03\x65x1\x18\x02 \x01(\x0b\x32\".farm_ng.core.proto.StructExample1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.core.examples_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_STRUCTEXAMPLE1']._serialized_start=51
   _globals['_STRUCTEXAMPLE1']._serialized_end=95
   _globals['_STRUCTEXAMPLE2']._serialized_start=97
   _globals['_STRUCTEXAMPLE2']._serialized_end=176
 # @@protoc_insertion_point(module_scope)
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/examples_pb2.pyi` & `farm_ng_core-2.3.0/py/farm_ng/core/examples_pb2.pyi`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/geometry.proto` & `farm_ng_core-2.3.0/py/farm_ng/core/geometry.proto`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/geometry_pb2.py` & `farm_ng_core-2.3.0/py/farm_ng/core/geometry_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/core/geometry.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -16,14 +16,14 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66\x61rm_ng/core/geometry.proto\x12\x12\x66\x61rm_ng.core.proto\x1a\x19\x66\x61rm_ng/core/linalg.proto\"8\n\x0bUnitVec3F64\x12)\n\x04vec3\x18\x01 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F64\"Q\n\x0eHyperplane3F64\x12/\n\x06normal\x18\x01 \x01(\x0b\x32\x1f.farm_ng.core.proto.UnitVec3F64\x12\x0e\n\x06offset\x18\x02 \x01(\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.core.geometry_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_UNITVEC3F64']._serialized_start=78
   _globals['_UNITVEC3F64']._serialized_end=134
   _globals['_HYPERPLANE3F64']._serialized_start=136
   _globals['_HYPERPLANE3F64']._serialized_end=217
 # @@protoc_insertion_point(module_scope)
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/geometry_pb2.pyi` & `farm_ng_core-2.3.0/py/farm_ng/core/geometry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/image.proto` & `farm_ng_core-2.3.0/py/farm_ng/core/image.proto`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/image_pb2.py` & `farm_ng_core-2.3.0/py/farm_ng/core/image_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/core/image.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,16 +15,16 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x66\x61rm_ng/core/image.proto\x12\x12\x66\x61rm_ng.core.proto\"*\n\tImageSize\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\"O\n\x0bImageLayout\x12+\n\x04size\x18\x01 \x01(\x0b\x32\x1d.farm_ng.core.proto.ImageSize\x12\x13\n\x0bpitch_bytes\x18\x02 \x01(\r\"[\n\x0bPixelFormat\x12\x13\n\x0bnumber_type\x18\x01 \x01(\t\x12\x16\n\x0enum_components\x18\x02 \x01(\x05\x12\x1f\n\x17num_bytes_per_component\x18\x03 \x01(\x05\"\x80\x01\n\x08\x44ynImage\x12/\n\x06layout\x18\x01 \x01(\x0b\x32\x1f.farm_ng.core.proto.ImageLayout\x12\x35\n\x0cpixel_format\x18\x02 \x01(\x0b\x32\x1f.farm_ng.core.proto.PixelFormat\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.core.image_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_IMAGESIZE']._serialized_start=48
   _globals['_IMAGESIZE']._serialized_end=90
   _globals['_IMAGELAYOUT']._serialized_start=92
   _globals['_IMAGELAYOUT']._serialized_end=171
   _globals['_PIXELFORMAT']._serialized_start=173
   _globals['_PIXELFORMAT']._serialized_end=264
   _globals['_DYNIMAGE']._serialized_start=267
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/image_pb2.pyi` & `farm_ng_core-2.3.0/py/farm_ng/core/image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/lie.proto` & `farm_ng_core-2.3.0/py/farm_ng/core/lie.proto`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/lie_pb2.py` & `farm_ng_core-2.3.0/py/farm_ng/core/lie_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/core/lie.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -16,16 +16,16 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x66\x61rm_ng/core/lie.proto\x12\x12\x66\x61rm_ng.core.proto\x1a\x19\x66\x61rm_ng/core/linalg.proto\"H\n\rQuaternionF64\x12)\n\x04imag\x18\x01 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F64\x12\x0c\n\x04real\x18\x02 \x01(\x01\"\x1d\n\x0cRotation2F64\x12\r\n\x05theta\x18\x01 \x01(\x01\"t\n\x0cIsometry2F64\x12\x32\n\x08rotation\x18\x01 \x01(\x0b\x32 .farm_ng.core.proto.Rotation2F64\x12\x30\n\x0btranslation\x18\x02 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec2F64\"J\n\x0cRotation3F64\x12:\n\x0funit_quaternion\x18\x01 \x01(\x0b\x32!.farm_ng.core.proto.QuaternionF64\"t\n\x0cIsometry3F64\x12\x32\n\x08rotation\x18\x01 \x01(\x0b\x32 .farm_ng.core.proto.Rotation3F64\x12\x30\n\x0btranslation\x18\x02 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F64\"\x82\x01\n\x13Isometry3F64Tangent\x12\x34\n\x0flinear_velocity\x18\x01 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F64\x12\x35\n\x10\x61ngular_velocity\x18\x02 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F64b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.core.lie_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_QUATERNIONF64']._serialized_start=73
   _globals['_QUATERNIONF64']._serialized_end=145
   _globals['_ROTATION2F64']._serialized_start=147
   _globals['_ROTATION2F64']._serialized_end=176
   _globals['_ISOMETRY2F64']._serialized_start=178
   _globals['_ISOMETRY2F64']._serialized_end=294
   _globals['_ROTATION3F64']._serialized_start=296
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/lie_pb2.pyi` & `farm_ng_core-2.3.0/py/farm_ng/core/lie_pb2.pyi`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/linalg.proto` & `farm_ng_core-2.3.0/py/farm_ng/core/linalg.proto`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/linalg_pb2.py` & `farm_ng_core-2.3.0/py/farm_ng/core/linalg_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/core/linalg.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,16 +15,16 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x66\x61rm_ng/core/linalg.proto\x12\x12\x66\x61rm_ng.core.proto\"\x1f\n\x07Vec2I64\x12\t\n\x01x\x18\x01 \x01(\x03\x12\t\n\x01y\x18\x02 \x01(\x03\"\x1f\n\x07Vec2F32\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\"\x1f\n\x07Vec2F64\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\"*\n\x07Vec3I64\x12\t\n\x01x\x18\x01 \x01(\x03\x12\t\n\x01y\x18\x02 \x01(\x03\x12\t\n\x01z\x18\x03 \x01(\x03\"*\n\x07Vec3F32\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\t\n\x01z\x18\x03 \x01(\x02\"*\n\x07Vec3F64\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\x12\t\n\x01z\x18\x03 \x01(\x01\"a\n\x07Mat2F32\x12*\n\x05\x63ol_0\x18\x01 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec2F32\x12*\n\x05\x63ol_1\x18\x02 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec2F32\"a\n\x07Mat2F64\x12*\n\x05\x63ol_0\x18\x01 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec2F64\x12*\n\x05\x63ol_1\x18\x02 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec2F64\"\x8d\x01\n\x07Mat3F32\x12*\n\x05\x63ol_0\x18\x01 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F32\x12*\n\x05\x63ol_1\x18\x02 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F32\x12*\n\x05\x63ol_2\x18\x03 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F32\"\x8d\x01\n\x07Mat3F64\x12*\n\x05\x63ol_0\x18\x01 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F64\x12*\n\x05\x63ol_1\x18\x02 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F64\x12*\n\x05\x63ol_2\x18\x03 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F64\"\x17\n\x07VecXF32\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x02\"\x17\n\x07VecXF64\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x01\"3\n\x07MatXF32\x12\x0c\n\x04rows\x18\x01 \x01(\x05\x12\x0c\n\x04\x63ols\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x03 \x03(\x02\"3\n\x07MatXF64\x12\x0c\n\x04rows\x18\x01 \x01(\x05\x12\x0c\n\x04\x63ols\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x03 \x03(\x02\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.core.linalg_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_VEC2I64']._serialized_start=49
   _globals['_VEC2I64']._serialized_end=80
   _globals['_VEC2F32']._serialized_start=82
   _globals['_VEC2F32']._serialized_end=113
   _globals['_VEC2F64']._serialized_start=115
   _globals['_VEC2F64']._serialized_end=146
   _globals['_VEC3I64']._serialized_start=148
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/linalg_pb2.pyi` & `farm_ng_core-2.3.0/py/farm_ng/core/linalg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/pose.proto` & `farm_ng_core-2.3.0/py/farm_ng/core/pose.proto`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/pose_pb2.py` & `farm_ng_core-2.3.0/py/farm_ng/core/pose_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/core/pose.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -16,14 +16,14 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17\x66\x61rm_ng/core/pose.proto\x12\x12\x66\x61rm_ng.core.proto\x1a\x16\x66\x61rm_ng/core/lie.proto\"\xa0\x01\n\x04Pose\x12\x32\n\x08\x61_from_b\x18\x01 \x01(\x0b\x32 .farm_ng.core.proto.Isometry3F64\x12\x0f\n\x07\x66rame_a\x18\x02 \x01(\t\x12\x0f\n\x07\x66rame_b\x18\x03 \x01(\t\x12\x42\n\x11tangent_of_b_in_a\x18\x04 \x01(\x0b\x32\'.farm_ng.core.proto.Isometry3F64Tangent\"3\n\x08PoseTree\x12\'\n\x05poses\x18\x01 \x03(\x0b\x32\x18.farm_ng.core.proto.Poseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.core.pose_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_POSE']._serialized_start=72
   _globals['_POSE']._serialized_end=232
   _globals['_POSETREE']._serialized_start=234
   _globals['_POSETREE']._serialized_end=285
 # @@protoc_insertion_point(module_scope)
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/pose_pb2.pyi` & `farm_ng_core-2.3.0/py/farm_ng/core/pose_pb2.pyi`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/pose_tree.py` & `farm_ng_core-2.3.0/py/farm_ng/core/pose_tree.py`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/sensor.proto` & `farm_ng_core-2.3.0/py/farm_ng/core/sensor.proto`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/sensor_pb2.py` & `farm_ng_core-2.3.0/py/farm_ng/core/sensor_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/core/sensor.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -17,16 +17,16 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x66\x61rm_ng/core/sensor.proto\x12\x12\x66\x61rm_ng.core.proto\x1a\x18\x66\x61rm_ng/core/image.proto\x1a\x16\x66\x61rm_ng/core/lie.proto\"i\n\x0b\x43\x61meraModel\x12\x31\n\nimage_size\x18\x01 \x01(\x0b\x32\x1d.farm_ng.core.proto.ImageSize\x12\x17\n\x0f\x64istortion_type\x18\x02 \x01(\t\x12\x0e\n\x06params\x18\x03 \x03(\x01\"F\n\x0c\x43\x61meraModels\x12\x36\n\rcamera_models\x18\x01 \x03(\x0b\x32\x1f.farm_ng.core.proto.CameraModel\"+\n\x0e\x43lippingPlanes\x12\x0c\n\x04near\x18\x01 \x01(\x02\x12\x0b\n\x03\x66\x61r\x18\x02 \x01(\x02\"}\n\x0bRigidCamera\x12\x33\n\nintrinsics\x18\x01 \x01(\x0b\x32\x1f.farm_ng.core.proto.CameraModel\x12\x39\n\x0frig_from_camera\x18\x02 \x01(\x0b\x32 .farm_ng.core.proto.Isometry3F64\"/\n\tGyroModel\x12\x12\n\nmodel_type\x18\x01 \x01(\t\x12\x0e\n\x06params\x18\x02 \x03(\x01\"3\n\rAcceleroModel\x12\x12\n\nmodel_type\x18\x01 \x01(\t\x12\x0e\n\x06params\x18\x02 \x03(\x01\"x\n\x08ImuModel\x12\x31\n\ngyro_model\x18\x01 \x01(\x0b\x32\x1d.farm_ng.core.proto.GyroModel\x12\x39\n\x0e\x61\x63\x63\x65lero_model\x18\x02 \x01(\x0b\x32!.farm_ng.core.proto.AcceleroModelb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.core.sensor_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_CAMERAMODEL']._serialized_start=99
   _globals['_CAMERAMODEL']._serialized_end=204
   _globals['_CAMERAMODELS']._serialized_start=206
   _globals['_CAMERAMODELS']._serialized_end=276
   _globals['_CLIPPINGPLANES']._serialized_start=278
   _globals['_CLIPPINGPLANES']._serialized_end=321
   _globals['_RIGIDCAMERA']._serialized_start=323
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/sensor_pb2.pyi` & `farm_ng_core-2.3.0/py/farm_ng/core/sensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/stamp.py` & `farm_ng_core-2.3.0/py/farm_ng/core/stamp.py`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/std.proto` & `farm_ng_core-2.3.0/py/farm_ng/core/std.proto`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/std_pb2.py` & `farm_ng_core-2.3.0/py/farm_ng/core/std_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/core/std.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,16 +15,16 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x66\x61rm_ng/core/std.proto\x12\x12\x66\x61rm_ng.core.proto\"3\n\x0fOptionalG0Float\x12\r\n\x05value\x18\x01 \x01(\x02\x12\x11\n\thas_value\x18\x02 \x01(\x08\"4\n\x10OptionalG0Double\x12\r\n\x05value\x18\x01 \x01(\x01\x12\x11\n\thas_value\x18\x02 \x01(\x08\"3\n\x0fOptionalG0Int32\x12\r\n\x05value\x18\x01 \x01(\x05\x12\x11\n\thas_value\x18\x02 \x01(\x08\"3\n\x0fOptionalG0Int64\x12\r\n\x05value\x18\x01 \x01(\x03\x12\x11\n\thas_value\x18\x02 \x01(\x08\"2\n\x0eOptionalG0Bool\x12\r\n\x05value\x18\x01 \x01(\x08\x12\x11\n\thas_value\x18\x02 \x01(\x08\"4\n\x10OptionalG0String\x12\r\n\x05value\x18\x01 \x01(\t\x12\x11\n\thas_value\x18\x02 \x01(\x08\"%\n\x0e\x46ileSystemPath\x12\x13\n\x0bpath_string\x18\x01 \x01(\tb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.core.std_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_OPTIONALG0FLOAT']._serialized_start=46
   _globals['_OPTIONALG0FLOAT']._serialized_end=97
   _globals['_OPTIONALG0DOUBLE']._serialized_start=99
   _globals['_OPTIONALG0DOUBLE']._serialized_end=151
   _globals['_OPTIONALG0INT32']._serialized_start=153
   _globals['_OPTIONALG0INT32']._serialized_end=204
   _globals['_OPTIONALG0INT64']._serialized_start=206
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/std_pb2.pyi` & `farm_ng_core-2.3.0/py/farm_ng/core/std_pb2.pyi`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/timestamp.proto` & `farm_ng_core-2.3.0/py/farm_ng/core/timestamp.proto`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/timestamp_pb2.py` & `farm_ng_core-2.3.0/py/farm_ng/core/timestamp_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/core/timestamp.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,12 +15,12 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x66\x61rm_ng/core/timestamp.proto\x12\x12\x66\x61rm_ng.core.proto\"A\n\tTimestamp\x12\r\n\x05stamp\x18\x01 \x01(\x01\x12\x12\n\nclock_name\x18\x02 \x01(\t\x12\x11\n\tsemantics\x18\x03 \x01(\tb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.core.timestamp_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_TIMESTAMP']._serialized_start=52
   _globals['_TIMESTAMP']._serialized_end=117
 # @@protoc_insertion_point(module_scope)
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/timestamp_pb2.pyi` & `farm_ng_core-2.3.0/py/farm_ng/core/timestamp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/uri.proto` & `farm_ng_core-2.3.0/py/farm_ng/core/uri.proto`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/uri.py` & `farm_ng_core-2.3.0/py/farm_ng/core/uri.py`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/uri_pb2.py` & `farm_ng_core-2.3.0/py/farm_ng/core/uri_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/core/uri.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,12 +15,12 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x66\x61rm_ng/core/uri.proto\x12\x12\x66\x61rm_ng.core.proto\"E\n\x03Uri\x12\x0e\n\x06scheme\x18\x01 \x01(\t\x12\x11\n\tauthority\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12\r\n\x05query\x18\x04 \x01(\tb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.core.uri_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_URI']._serialized_start=46
   _globals['_URI']._serialized_end=115
 # @@protoc_insertion_point(module_scope)
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng/core/uri_pb2.pyi` & `farm_ng_core-2.3.0/py/farm_ng/core/uri_pb2.pyi`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/farm_ng_core.egg-info/PKG-INFO` & `farm_ng_core-2.3.0/py/farm_ng_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: farm_ng_core
-Version: 2.2.0
+Version: 2.3.0
 Home-page: https://github.com/farm-ng/farm-ng-core
 Download-URL: https://github.com/farm-ng/farm-ng-core
 Author: Farm-ng Inc.
 Author-email: info@farm-ng.com
 Keywords: robotics,open-source
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: farm_ng_core Version: 2.2.0 Home-page: https://
+Metadata-Version: 2.1 Name: farm_ng_core Version: 2.3.0 Home-page: https://
 github.com/farm-ng/farm-ng-core Download-URL: https://github.com/farm-ng/farm-
 ng-core Author: Farm-ng Inc. Author-email: info@farm-ng.com Keywords:
 robotics,open-source Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
 Classifier: Framework :: Robot Framework Requires-Python: >=3.8 Description-
```

### Comparing `farm_ng_core-2.2.0/py/farm_ng_core.egg-info/SOURCES.txt` & `farm_ng_core-2.3.0/py/farm_ng_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/pybind/farm_ng_core_pybind.cpp` & `farm_ng_core-2.3.0/py/pybind/farm_ng_core_pybind.cpp`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/pybind/lie_pybind.cpp` & `farm_ng_core-2.3.0/py/pybind/lie_pybind.cpp`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/py/pybind/linalg_pybind.cpp` & `farm_ng_core-2.3.0/py/pybind/linalg_pybind.cpp`

 * *Files identical despite different names*

### Comparing `farm_ng_core-2.2.0/setup.cfg` & `farm_ng_core-2.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = farm_ng_core
-version = 2.2.0
+version = 2.3.0
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Farm-ng Inc.
 author_email = info@farm-ng.com
 url = https://github.com/farm-ng/farm-ng-core
 download_url = https://github.com/farm-ng/farm-ng-core
```

### Comparing `farm_ng_core-2.2.0/setup.py` & `farm_ng_core-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     BuildProtosEggInfo,
     BuildProtosInstall,
     CleanFilesCommand,
 )
 from pybind11.setup_helpers import ParallelCompile, Pybind11Extension, build_ext
 from setuptools import setup
 
-__version__ = "2.2.0"
+__version__ = "2.3.0"
 
 
 platform_cxx_flags = []
 
 if sys.platform.startswith("darwin"):
     print("Running on macOS")
     platform_cxx_flags = [
```

