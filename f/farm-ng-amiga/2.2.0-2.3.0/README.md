# Comparing `tmp/farm_ng_amiga-2.2.0.tar.gz` & `tmp/farm_ng_amiga-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "farm_ng_amiga-2.2.0.tar", last modified: Wed Jan 17 00:33:14 2024, max compression
+gzip compressed data, was "farm_ng_amiga-2.3.0.tar", last modified: Fri May 17 21:41:07 2024, max compression
```

## Comparing `farm_ng_amiga-2.2.0.tar` & `farm_ng_amiga-2.3.0.tar`

### file list

```diff
@@ -1,62 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:33:14.566221 farm_ng_amiga-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    15960 2024-01-17 00:32:55.000000 farm_ng_amiga-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-01-17 00:33:14.566221 farm_ng_amiga-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-01-17 00:32:55.000000 farm_ng_amiga-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:33:14.554221 farm_ng_amiga-2.2.0/py/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:33:14.554221 farm_ng_amiga-2.2.0/py/farm_ng/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:33:14.554221 farm_ng_amiga-2.2.0/py/farm_ng/amiga/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-01-17 00:32:55.000000 farm_ng_amiga-2.2.0/py/farm_ng/amiga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/amiga/amiga.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/amiga/amiga_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/amiga/amiga_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/amiga/amiga_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:33:14.558221 farm_ng_amiga-2.2.0/py/farm_ng/canbus/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-01-17 00:32:55.000000 farm_ng_amiga-2.2.0/py/farm_ng/canbus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/canbus/amiga_v6.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/canbus/amiga_v6_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/canbus/amiga_v6_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/canbus/amiga_v6_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/canbus/canbus.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/canbus/canbus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/canbus/canbus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/canbus/canbus_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-01-17 00:32:55.000000 farm_ng_amiga-2.2.0/py/farm_ng/canbus/packet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:33:14.558221 farm_ng_amiga-2.2.0/py/farm_ng/filter/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-01-17 00:32:55.000000 farm_ng_amiga-2.2.0/py/farm_ng/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/filter/filter.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/filter/filter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/filter/filter_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/filter/filter_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:33:14.558221 farm_ng_amiga-2.2.0/py/farm_ng/gps/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-01-17 00:32:55.000000 farm_ng_amiga-2.2.0/py/farm_ng/gps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/gps/gps.proto
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/gps/gps_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/gps/gps_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/gps/gps_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:33:14.558221 farm_ng_amiga-2.2.0/py/farm_ng/imu/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-01-17 00:32:55.000000 farm_ng_amiga-2.2.0/py/farm_ng/imu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/imu/imu_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/imu/imu_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/imu/imu_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:33:14.562221 farm_ng_amiga-2.2.0/py/farm_ng/oak/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-01-17 00:32:55.000000 farm_ng_amiga-2.2.0/py/farm_ng/oak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/oak/oak.proto
--rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/oak/oak_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/oak/oak_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/oak/oak_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:33:14.562221 farm_ng_amiga-2.2.0/py/farm_ng/track/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-01-17 00:32:55.000000 farm_ng_amiga-2.2.0/py/farm_ng/track/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/track/track.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/track/track_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/track/track_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng/track/track_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-01-17 00:32:55.000000 farm_ng_amiga-2.2.0/py/farm_ng/track/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 00:33:14.562221 farm_ng_amiga-2.2.0/py/farm_ng_amiga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng_amiga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng_amiga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng_amiga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng_amiga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-17 00:33:14.000000 farm_ng_amiga-2.2.0/py/farm_ng_amiga.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-01-17 00:32:55.000000 farm_ng_amiga-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-01-17 00:33:14.566221 farm_ng_amiga-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-01-17 00:32:55.000000 farm_ng_amiga-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:41:07.704064 farm_ng_amiga-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    15960 2024-05-17 21:40:48.000000 farm_ng_amiga-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-17 21:41:07.704064 farm_ng_amiga-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-17 21:40:48.000000 farm_ng_amiga-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:41:07.692064 farm_ng_amiga-2.3.0/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:41:07.692064 farm_ng_amiga-2.3.0/py/farm_ng/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:41:07.692064 farm_ng_amiga-2.3.0/py/farm_ng/amiga/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-17 21:40:48.000000 farm_ng_amiga-2.3.0/py/farm_ng/amiga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/amiga/amiga.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/amiga/amiga_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/amiga/amiga_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/amiga/amiga_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:41:07.696064 farm_ng_amiga-2.3.0/py/farm_ng/canbus/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-17 21:40:48.000000 farm_ng_amiga-2.3.0/py/farm_ng/canbus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8371 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/canbus/amiga_v6.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/canbus/amiga_v6_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/canbus/amiga_v6_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/canbus/amiga_v6_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/canbus/canbus.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/canbus/canbus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/canbus/canbus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/canbus/canbus_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17188 2024-05-17 21:40:48.000000 farm_ng_amiga-2.3.0/py/farm_ng/canbus/packet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/canbus/tool_control.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/canbus/tool_control_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/canbus/tool_control_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/canbus/tool_control_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:41:07.696064 farm_ng_amiga-2.3.0/py/farm_ng/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-17 21:40:48.000000 farm_ng_amiga-2.3.0/py/farm_ng/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/filter/filter.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/filter/filter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/filter/filter_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/filter/filter_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:41:07.696064 farm_ng_amiga-2.3.0/py/farm_ng/gps/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-17 21:40:48.000000 farm_ng_amiga-2.3.0/py/farm_ng/gps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/gps/gps.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/gps/gps_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9509 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/gps/gps_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/gps/gps_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:41:07.700064 farm_ng_amiga-2.3.0/py/farm_ng/imu/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-17 21:40:48.000000 farm_ng_amiga-2.3.0/py/farm_ng/imu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/imu/imu_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/imu/imu_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/imu/imu_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:41:07.700064 farm_ng_amiga-2.3.0/py/farm_ng/oak/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-17 21:40:48.000000 farm_ng_amiga-2.3.0/py/farm_ng/oak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/oak/oak.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/oak/oak_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/oak/oak_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/oak/oak_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:41:07.700064 farm_ng_amiga-2.3.0/py/farm_ng/track/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-17 21:40:48.000000 farm_ng_amiga-2.3.0/py/farm_ng/track/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/track/track.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/track/track_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/track/track_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng/track/track_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-17 21:40:48.000000 farm_ng_amiga-2.3.0/py/farm_ng/track/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:41:07.700064 farm_ng_amiga-2.3.0/py/farm_ng_amiga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng_amiga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng_amiga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng_amiga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng_amiga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 21:41:07.000000 farm_ng_amiga-2.3.0/py/farm_ng_amiga.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-17 21:40:48.000000 farm_ng_amiga-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-17 21:41:07.704064 farm_ng_amiga-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-17 21:40:48.000000 farm_ng_amiga-2.3.0/setup.py
```

### Comparing `farm_ng_amiga-2.2.0/LICENSE` & `farm_ng_amiga-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `farm_ng_amiga-2.2.0/PKG-INFO` & `farm_ng_amiga-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: farm_ng_amiga
-Version: 2.2.0
+Version: 2.3.0
 Summary: Amiga development kit for third party hardware or software extensions
 Home-page: https://github.com/farm-ng/farm-ng-amiga
 Download-URL: https://github.com/farm-ng/farm-ng-amiga
 Author: farm-ng Inc.
 Author-email: info@farm-ng.com
 Keywords: robotics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `farm_ng_amiga-2.2.0/README.md` & `farm_ng_amiga-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/amiga/__init__.py` & `farm_ng_amiga-2.3.0/py/farm_ng/amiga/__init__.py`

 * *Files identical despite different names*

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/amiga/amiga.proto` & `farm_ng_amiga-2.3.0/py/farm_ng/amiga/amiga.proto`

 * *Files identical despite different names*

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/amiga/amiga_pb2.py` & `farm_ng_amiga-2.3.0/py/farm_ng/amiga/amiga_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/amiga/amiga.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -17,19 +17,19 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x66\x61rm_ng/amiga/amiga.proto\x12\x13\x66\x61rm_ng.amiga.proto\x1a\x15\x66\x61rm_ng/imu/imu.proto\x1a\x17\x66\x61rm_ng/core/pose.proto\"\xdf\x02\n\x10\x41migaRobotConfig\x12/\n\tpose_tree\x18\x01 \x01(\x0b\x32\x1c.farm_ng.core.proto.PoseTree\x12=\n\x04imus\x18\x03 \x03(\x0b\x32/.farm_ng.amiga.proto.AmigaRobotConfig.ImusEntry\x12\x41\n\x06wheels\x18\x04 \x03(\x0b\x32\x31.farm_ng.amiga.proto.AmigaRobotConfig.WheelsEntry\x1aG\n\tImusEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.farm_ng.imu.proto.ImuBias:\x02\x38\x01\x1aO\n\x0bWheelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .farm_ng.amiga.proto.WheelConfig:\x02\x38\x01\"Y\n\x0bWheelConfig\x12\x11\n\tcanbus_id\x18\x02 \x01(\r\x12\x1d\n\x15wheel_from_motor_rate\x18\x04 \x01(\x01\x12\x18\n\x10wheel_diameter_m\x18\x05 \x01(\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.amiga.amiga_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  _globals['_AMIGAROBOTCONFIG_IMUSENTRY']._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
+  _globals['_AMIGAROBOTCONFIG_IMUSENTRY']._loaded_options = None
   _globals['_AMIGAROBOTCONFIG_IMUSENTRY']._serialized_options = b'8\001'
-  _globals['_AMIGAROBOTCONFIG_WHEELSENTRY']._options = None
+  _globals['_AMIGAROBOTCONFIG_WHEELSENTRY']._loaded_options = None
   _globals['_AMIGAROBOTCONFIG_WHEELSENTRY']._serialized_options = b'8\001'
   _globals['_AMIGAROBOTCONFIG']._serialized_start=99
   _globals['_AMIGAROBOTCONFIG']._serialized_end=450
   _globals['_AMIGAROBOTCONFIG_IMUSENTRY']._serialized_start=298
   _globals['_AMIGAROBOTCONFIG_IMUSENTRY']._serialized_end=369
   _globals['_AMIGAROBOTCONFIG_WHEELSENTRY']._serialized_start=371
   _globals['_AMIGAROBOTCONFIG_WHEELSENTRY']._serialized_end=450
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/amiga/amiga_pb2.pyi` & `farm_ng_amiga-2.3.0/py/farm_ng/amiga/amiga_pb2.pyi`

 * *Files identical despite different names*

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/canbus/__init__.py` & `farm_ng_amiga-2.3.0/py/farm_ng/canbus/__init__.py`

 * *Files identical despite different names*

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/canbus/amiga_v6_pb2.py` & `farm_ng_amiga-2.3.0/py/farm_ng/canbus/canbus_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: farm_ng/canbus/amiga_v6.proto
-# Protobuf Python Version: 4.25.0
+# source: farm_ng/canbus/canbus.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from farm_ng.canbus import canbus_pb2 as farm__ng_dot_canbus_dot_canbus__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x66\x61rm_ng/canbus/amiga_v6.proto\x12\x14\x66\x61rm_ng.canbus.proto\x1a\x1b\x66\x61rm_ng/canbus/canbus.proto\"\xcb\x01\n\nAmigaTpdo1\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\r\n\x05stamp\x18\x02 \x01(\x01\x12>\n\rcontrol_state\x18\x03 \x01(\x0e\x32\'.farm_ng.canbus.proto.AmigaControlState\x12\x16\n\x0emeasured_speed\x18\x04 \x01(\x01\x12\x1d\n\x15measured_angular_rate\x18\x05 \x01(\x01\x12\x10\n\x08pto_bits\x18\x06 \x01(\r\x12\x14\n\x0chbridge_bits\x18\x07 \x01(\r\"\x7f\n\tAmigaPdo2\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\r\n\x05stamp\x18\x02 \x01(\x01\x12\x13\n\x0bmotor_a_rpm\x18\x03 \x01(\x05\x12\x13\n\x0bmotor_b_rpm\x18\x04 \x01(\x05\x12\x13\n\x0bmotor_c_rpm\x18\x05 \x01(\x05\x12\x13\n\x0bmotor_d_rpm\x18\x06 \x01(\x05\"\xbb\x01\n\x12\x41migaV6CanbusState\x12\x35\n\x0b\x61miga_tpdo1\x18\x01 \x01(\x0b\x32 .farm_ng.canbus.proto.AmigaTpdo1\x12\x37\n\x0cmotor_states\x18\x02 \x01(\x0b\x32!.farm_ng.canbus.proto.MotorStates\x12\x1c\n\x14\x62\x61ttery_charge_level\x18\x03 \x01(\x01\x12\x17\n\x0flast_send_error\x18\x04 \x01(\x08*\xaa\x01\n\x11\x41migaControlState\x12\x0e\n\nSTATE_BOOT\x10\x00\x12\x16\n\x12STATE_MANUAL_READY\x10\x01\x12\x17\n\x13STATE_MANUAL_ACTIVE\x10\x02\x12\x13\n\x0fSTATE_CC_ACTIVE\x10\x03\x12\x14\n\x10STATE_AUTO_READY\x10\x04\x12\x15\n\x11STATE_AUTO_ACTIVE\x10\x05\x12\x12\n\x0eSTATE_ESTOPPED\x10\x06\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66\x61rm_ng/canbus/canbus.proto\x12\x14\x66\x61rm_ng.canbus.proto\"Y\n\x07Twist2d\x12\x19\n\x11linear_velocity_x\x18\x01 \x01(\x02\x12\x19\n\x11linear_velocity_y\x18\x02 \x01(\x02\x12\x18\n\x10\x61ngular_velocity\x18\x03 \x01(\x02\"g\n\x10RawCanbusMessage\x12\r\n\x05stamp\x18\x01 \x01(\x01\x12\n\n\x02id\x18\x02 \x01(\r\x12\r\n\x05\x65rror\x18\x03 \x01(\x08\x12\x1b\n\x13remote_transmission\x18\x04 \x01(\x08\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\"M\n\x11RawCanbusMessages\x12\x38\n\x08messages\x18\x01 \x03(\x0b\x32&.farm_ng.canbus.proto.RawCanbusMessage\"{\n\nMotorState\x12\r\n\x05stamp\x18\x01 \x01(\x01\x12\n\n\x02id\x18\x02 \x01(\r\x12\x0e\n\x06status\x18\x03 \x01(\r\x12\x0b\n\x03rpm\x18\x04 \x01(\x05\x12\x0f\n\x07voltage\x18\x05 \x01(\x01\x12\x0f\n\x07\x63urrent\x18\x06 \x01(\x01\x12\x13\n\x0btemperature\x18\x07 \x01(\x05\"?\n\x0bMotorStates\x12\x30\n\x06motors\x18\x01 \x03(\x0b\x32 .farm_ng.canbus.proto.MotorState*`\n\x15MotorControllerStatus\x12\x13\n\x0fPRE_OPERATIONAL\x10\x00\x12\x08\n\x04IDLE\x10\x01\x12\x14\n\x10POST_OPERATIONAL\x10\x02\x12\x07\n\x03RUN\x10\x03\x12\t\n\x05\x46\x41ULT\x10\x04\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.canbus.amiga_v6_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  _globals['_AMIGACONTROLSTATE']._serialized_start=610
-  _globals['_AMIGACONTROLSTATE']._serialized_end=780
-  _globals['_AMIGATPDO1']._serialized_start=85
-  _globals['_AMIGATPDO1']._serialized_end=288
-  _globals['_AMIGAPDO2']._serialized_start=290
-  _globals['_AMIGAPDO2']._serialized_end=417
-  _globals['_AMIGAV6CANBUSSTATE']._serialized_start=420
-  _globals['_AMIGAV6CANBUSSTATE']._serialized_end=607
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.canbus.canbus_pb2', _globals)
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
+  _globals['_MOTORCONTROLLERSTATUS']._serialized_start=518
+  _globals['_MOTORCONTROLLERSTATUS']._serialized_end=614
+  _globals['_TWIST2D']._serialized_start=53
+  _globals['_TWIST2D']._serialized_end=142
+  _globals['_RAWCANBUSMESSAGE']._serialized_start=144
+  _globals['_RAWCANBUSMESSAGE']._serialized_end=247
+  _globals['_RAWCANBUSMESSAGES']._serialized_start=249
+  _globals['_RAWCANBUSMESSAGES']._serialized_end=326
+  _globals['_MOTORSTATE']._serialized_start=328
+  _globals['_MOTORSTATE']._serialized_end=451
+  _globals['_MOTORSTATES']._serialized_start=453
+  _globals['_MOTORSTATES']._serialized_end=516
 # @@protoc_insertion_point(module_scope)
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/canbus/amiga_v6_pb2.pyi` & `farm_ng_amiga-2.3.0/py/farm_ng/canbus/canbus_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,74 @@
-from farm_ng.canbus import canbus_pb2 as _canbus_pb2
+from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class AmigaControlState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+class MotorControllerStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
-    STATE_BOOT: _ClassVar[AmigaControlState]
-    STATE_MANUAL_READY: _ClassVar[AmigaControlState]
-    STATE_MANUAL_ACTIVE: _ClassVar[AmigaControlState]
-    STATE_CC_ACTIVE: _ClassVar[AmigaControlState]
-    STATE_AUTO_READY: _ClassVar[AmigaControlState]
-    STATE_AUTO_ACTIVE: _ClassVar[AmigaControlState]
-    STATE_ESTOPPED: _ClassVar[AmigaControlState]
-STATE_BOOT: AmigaControlState
-STATE_MANUAL_READY: AmigaControlState
-STATE_MANUAL_ACTIVE: AmigaControlState
-STATE_CC_ACTIVE: AmigaControlState
-STATE_AUTO_READY: AmigaControlState
-STATE_AUTO_ACTIVE: AmigaControlState
-STATE_ESTOPPED: AmigaControlState
-
-class AmigaTpdo1(_message.Message):
-    __slots__ = ("node_id", "stamp", "control_state", "measured_speed", "measured_angular_rate", "pto_bits", "hbridge_bits")
-    NODE_ID_FIELD_NUMBER: _ClassVar[int]
+    PRE_OPERATIONAL: _ClassVar[MotorControllerStatus]
+    IDLE: _ClassVar[MotorControllerStatus]
+    POST_OPERATIONAL: _ClassVar[MotorControllerStatus]
+    RUN: _ClassVar[MotorControllerStatus]
+    FAULT: _ClassVar[MotorControllerStatus]
+PRE_OPERATIONAL: MotorControllerStatus
+IDLE: MotorControllerStatus
+POST_OPERATIONAL: MotorControllerStatus
+RUN: MotorControllerStatus
+FAULT: MotorControllerStatus
+
+class Twist2d(_message.Message):
+    __slots__ = ("linear_velocity_x", "linear_velocity_y", "angular_velocity")
+    LINEAR_VELOCITY_X_FIELD_NUMBER: _ClassVar[int]
+    LINEAR_VELOCITY_Y_FIELD_NUMBER: _ClassVar[int]
+    ANGULAR_VELOCITY_FIELD_NUMBER: _ClassVar[int]
+    linear_velocity_x: float
+    linear_velocity_y: float
+    angular_velocity: float
+    def __init__(self, linear_velocity_x: _Optional[float] = ..., linear_velocity_y: _Optional[float] = ..., angular_velocity: _Optional[float] = ...) -> None: ...
+
+class RawCanbusMessage(_message.Message):
+    __slots__ = ("stamp", "id", "error", "remote_transmission", "data")
     STAMP_FIELD_NUMBER: _ClassVar[int]
-    CONTROL_STATE_FIELD_NUMBER: _ClassVar[int]
-    MEASURED_SPEED_FIELD_NUMBER: _ClassVar[int]
-    MEASURED_ANGULAR_RATE_FIELD_NUMBER: _ClassVar[int]
-    PTO_BITS_FIELD_NUMBER: _ClassVar[int]
-    HBRIDGE_BITS_FIELD_NUMBER: _ClassVar[int]
-    node_id: int
+    ID_FIELD_NUMBER: _ClassVar[int]
+    ERROR_FIELD_NUMBER: _ClassVar[int]
+    REMOTE_TRANSMISSION_FIELD_NUMBER: _ClassVar[int]
+    DATA_FIELD_NUMBER: _ClassVar[int]
     stamp: float
-    control_state: AmigaControlState
-    measured_speed: float
-    measured_angular_rate: float
-    pto_bits: int
-    hbridge_bits: int
-    def __init__(self, node_id: _Optional[int] = ..., stamp: _Optional[float] = ..., control_state: _Optional[_Union[AmigaControlState, str]] = ..., measured_speed: _Optional[float] = ..., measured_angular_rate: _Optional[float] = ..., pto_bits: _Optional[int] = ..., hbridge_bits: _Optional[int] = ...) -> None: ...
-
-class AmigaPdo2(_message.Message):
-    __slots__ = ("node_id", "stamp", "motor_a_rpm", "motor_b_rpm", "motor_c_rpm", "motor_d_rpm")
-    NODE_ID_FIELD_NUMBER: _ClassVar[int]
+    id: int
+    error: bool
+    remote_transmission: bool
+    data: bytes
+    def __init__(self, stamp: _Optional[float] = ..., id: _Optional[int] = ..., error: bool = ..., remote_transmission: bool = ..., data: _Optional[bytes] = ...) -> None: ...
+
+class RawCanbusMessages(_message.Message):
+    __slots__ = ("messages",)
+    MESSAGES_FIELD_NUMBER: _ClassVar[int]
+    messages: _containers.RepeatedCompositeFieldContainer[RawCanbusMessage]
+    def __init__(self, messages: _Optional[_Iterable[_Union[RawCanbusMessage, _Mapping]]] = ...) -> None: ...
+
+class MotorState(_message.Message):
+    __slots__ = ("stamp", "id", "status", "rpm", "voltage", "current", "temperature")
     STAMP_FIELD_NUMBER: _ClassVar[int]
-    MOTOR_A_RPM_FIELD_NUMBER: _ClassVar[int]
-    MOTOR_B_RPM_FIELD_NUMBER: _ClassVar[int]
-    MOTOR_C_RPM_FIELD_NUMBER: _ClassVar[int]
-    MOTOR_D_RPM_FIELD_NUMBER: _ClassVar[int]
-    node_id: int
+    ID_FIELD_NUMBER: _ClassVar[int]
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    RPM_FIELD_NUMBER: _ClassVar[int]
+    VOLTAGE_FIELD_NUMBER: _ClassVar[int]
+    CURRENT_FIELD_NUMBER: _ClassVar[int]
+    TEMPERATURE_FIELD_NUMBER: _ClassVar[int]
     stamp: float
-    motor_a_rpm: int
-    motor_b_rpm: int
-    motor_c_rpm: int
-    motor_d_rpm: int
-    def __init__(self, node_id: _Optional[int] = ..., stamp: _Optional[float] = ..., motor_a_rpm: _Optional[int] = ..., motor_b_rpm: _Optional[int] = ..., motor_c_rpm: _Optional[int] = ..., motor_d_rpm: _Optional[int] = ...) -> None: ...
-
-class AmigaV6CanbusState(_message.Message):
-    __slots__ = ("amiga_tpdo1", "motor_states", "battery_charge_level", "last_send_error")
-    AMIGA_TPDO1_FIELD_NUMBER: _ClassVar[int]
-    MOTOR_STATES_FIELD_NUMBER: _ClassVar[int]
-    BATTERY_CHARGE_LEVEL_FIELD_NUMBER: _ClassVar[int]
-    LAST_SEND_ERROR_FIELD_NUMBER: _ClassVar[int]
-    amiga_tpdo1: AmigaTpdo1
-    motor_states: _canbus_pb2.MotorStates
-    battery_charge_level: float
-    last_send_error: bool
-    def __init__(self, amiga_tpdo1: _Optional[_Union[AmigaTpdo1, _Mapping]] = ..., motor_states: _Optional[_Union[_canbus_pb2.MotorStates, _Mapping]] = ..., battery_charge_level: _Optional[float] = ..., last_send_error: bool = ...) -> None: ...
+    id: int
+    status: int
+    rpm: int
+    voltage: float
+    current: float
+    temperature: int
+    def __init__(self, stamp: _Optional[float] = ..., id: _Optional[int] = ..., status: _Optional[int] = ..., rpm: _Optional[int] = ..., voltage: _Optional[float] = ..., current: _Optional[float] = ..., temperature: _Optional[int] = ...) -> None: ...
+
+class MotorStates(_message.Message):
+    __slots__ = ("motors",)
+    MOTORS_FIELD_NUMBER: _ClassVar[int]
+    motors: _containers.RepeatedCompositeFieldContainer[MotorState]
+    def __init__(self, motors: _Optional[_Iterable[_Union[MotorState, _Mapping]]] = ...) -> None: ...
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/canbus/canbus.proto` & `farm_ng_amiga-2.3.0/py/farm_ng/canbus/canbus.proto`

 * *Files identical despite different names*

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/canbus/packet.py` & `farm_ng_amiga-2.3.0/py/farm_ng/canbus/packet.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,29 +9,41 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
+import logging
 import time
 from enum import IntEnum
 from struct import pack
 from struct import unpack
 
 from farm_ng.canbus import amiga_v6_pb2
 from farm_ng.canbus import canbus_pb2
 from farm_ng.core.stamp import timestamp_from_monotonic
 from farm_ng.core.timestamp_pb2 import Timestamp
 
-# TODO: add some comments about the CAN bus protocol
+# Important CAN node IDs
 DASHBOARD_NODE_ID = 0xE
 PENDANT_NODE_ID = 0xF
-BRAIN_NODE_ID = 0x1F
-SDK_NODE_ID = 0x2A
+
+
+class PendantButtons(IntEnum):
+    """Bit field for pendant buttons."""
+
+    PAUSE = 0x01  # Square
+    BRAKE = 0x02  # Circle
+    PTO = 0x04  # Triangle
+    CRUISE = 0x08  # Cross (X)
+    LEFT = 0x10  # D-pad left
+    UP = 0x20  # D-pad up
+    RIGHT = 0x40  # D-pad right
+    DOWN = 0x80  # D-pad down
 
 
 class AmigaControlState(IntEnum):
     """State of the Amiga vehicle control unit (VCU)"""
 
     # TODO: add some comments about this states
     STATE_BOOT = 0
@@ -40,27 +52,31 @@
     STATE_CC_ACTIVE = 3
     STATE_AUTO_READY = 4
     STATE_AUTO_ACTIVE = 5
     STATE_ESTOPPED = 6
 
 
 class ActuatorCommands(IntEnum):
+    """Commands for the linear and rotary actuators."""
+
     passive = 0x0
     forward = 0x1
     stopped = 0x2
     reverse = 0x3
 
 
 def actuator_bits_cmd(
     a0=ActuatorCommands.passive, a1=ActuatorCommands.passive, a2=ActuatorCommands.passive, a3=ActuatorCommands.passive
 ):
+    """Returns the command bits for up to four linear or rotary actuators."""
     return a0.value + (a1.value << 2) + (a2.value << 4) + (a3.value << 6)
 
 
 def actuator_bits_read(bits):
+    """Parses the command bits for up to four linear or rotary actuators."""
     a0 = ActuatorCommands(bits & 0x3)
     a1 = ActuatorCommands((bits >> 2) & 0x3)
     a2 = ActuatorCommands((bits >> 4) & 0x3)
     a3 = ActuatorCommands((bits >> 6) & 0x3)
     return (a0, a1, a2, a3)
 
 
@@ -85,29 +101,41 @@
 
     def age(self):
         """Age of the most recent message."""
         return time.monotonic() - self.stamp.stamp
 
 
 def make_amiga_rpdo1_proto(
-    state_req: AmigaControlState, cmd_speed: float, cmd_ang_rate: float, pto_bits: int = 0x0, hbridge_bits: int = 0x0
+    state_req: AmigaControlState = AmigaControlState.STATE_ESTOPPED,
+    cmd_speed: float = 0.0,
+    cmd_ang_rate: float = 0.0,
+    pto_bits: int = 0x0,
+    hbridge_bits: int = 0x0,
 ) -> canbus_pb2.RawCanbusMessage:
     """Creates a canbus_pb2.RawCanbusMessage.
 
     Uses the AmigaRpdo1 structure and formatting, that can be sent
     directly to the canbus service to be formatted and send on the CAN bus.
 
+    WARNING: Deprecated starting with farm-ng-amiga v2.3.0
+    Please use AmigaRpdo1.to_raw_canbus_message() instead.
+
     Args:
         state_req: State of the Amiga vehicle control unit (VCU).
         cmd_speed: Command speed in meters per second.
         cmd_ang_rate: Command angular rate in radians per second.
+        pto_bits: byte with encoded bits for PTO auto control
+        hbridge_bits: byte with encoded bits for h-bridge auto control
 
     Returns:
         An instance of a canbus_pb2.RawCanbusMessage.
     """
+    logging.warning("make_amiga_rpdo1_proto is deprecated as of v2.3.0")
+    logging.warning("Use AmigaRpdo1.to_raw_canbus_message() instead.")
+
     # TODO: add some checkers, or make python CHECK_API
     return canbus_pb2.RawCanbusMessage(
         id=AmigaRpdo1.cob_id + DASHBOARD_NODE_ID,
         data=AmigaRpdo1(
             state_req=state_req,
             cmd_speed=cmd_speed,
             cmd_ang_rate=cmd_ang_rate,
@@ -154,33 +182,38 @@
             self.pto_bits,
             self.hbridge_bits,
         )
 
     def decode(self, data):
         """Decodes CAN message data and populates the values of the class."""
         if len(data) == 5:
-            # TODO: Instate warning when dashboard fw v0.1.9 is released
-            # warnings.warn(
-            #     "Please update dashboard firmware to >= v0.1.9."
-            #     " New AmigaTpdo1 packets include more data. Support will be removed in farm_ng_amiga v0.0.9",
-            #     stacklevel=2,
-            # )
+            logging.warning("Please update dashboard firmware to >= v0.1.9 to use updated AmigaRpdo1 packet format.")
+
             (self.state_req, cmd_speed, cmd_ang_rate) = unpack(self.legacy_format, data)
             self.cmd_speed = cmd_speed / 1000.0
             self.cmd_ang_rate = cmd_ang_rate / 1000.0
         else:
             (self.state_req, cmd_speed, cmd_ang_rate, self.pto_bits, self.hbridge_bits) = unpack(self.format, data)
             self.cmd_speed = cmd_speed / 1000.0
             self.cmd_ang_rate = cmd_ang_rate / 1000.0
 
     def __str__(self):
         return "AMIGA RPDO1 Request state {} Command speed {:0.3f} Command angular rate {:0.3f}".format(
             self.state_req, self.cmd_speed, self.cmd_ang_rate
         ) + " Command PTO bits 0x{:x} Command h-bridge bits 0x{:x}".format(self.pto_bits, self.hbridge_bits)
 
+    def to_raw_canbus_message(self) -> canbus_pb2.RawCanbusMessage:
+        """Packs the class data into a canbus_pb2.RawCanbusMessage.
+
+        Returns: An instance of a canbus_pb2.RawCanbusMessage.
+        """
+        return canbus_pb2.RawCanbusMessage(
+            stamp=self.stamp.stamp, id=self.cob_id + DASHBOARD_NODE_ID, data=self.encode()
+        )
+
 
 class AmigaTpdo1(Packet):
     """State, speed, and angular rate of the Amiga vehicle control unit (VCU).
 
     New in fw v0.1.9 / farm-ng-amiga v0.0.7: Add pto & hbridge control. Message data is now 8 bytes (was 5).
     """
 
@@ -215,20 +248,16 @@
             self.pto_bits,
             self.hbridge_bits,
         )
 
     def decode(self, data):
         """Decodes CAN message data and populates the values of the class."""
         if len(data) == 5:
-            # TODO: Instate warning when dashboard fw v0.1.9 is released
-            # warnings.warn(
-            #     "Please update dashboard firmware to >= v0.1.9."
-            #     " New AmigaTpdo1 packets include more data. Support will be removed in farm_ng_amiga v0.0.9",
-            #     stacklevel=2,
-            # )
+            logging.warning("Please update dashboard firmware to >= v0.1.9 to use updated AmigaTpdo1 packet format.")
+
             (self.state, meas_speed, meas_ang_rate) = unpack(self.legacy_format, data)
             self.meas_speed = meas_speed / 1000.0
             self.meas_ang_rate = meas_ang_rate / 1000.0
         else:
             (self.state, meas_speed, meas_ang_rate, self.pto_bits, self.hbridge_bits) = unpack(self.format, data)
             self.meas_speed = meas_speed / 1000.0
             self.meas_ang_rate = meas_ang_rate / 1000.0
@@ -264,32 +293,56 @@
         obj.state = AmigaControlState(proto.control_state)
         obj.meas_speed = proto.measured_speed
         obj.meas_ang_rate = proto.measured_angular_rate
         obj.pto_bits = proto.pto_bits
         obj.hbridge_bits = proto.hbridge_bits
         return obj
 
+    @classmethod
+    def from_raw_canbus_message(cls, message: canbus_pb2.RawCanbusMessage) -> AmigaTpdo1:
+        """Parses a canbus_pb2.RawCanbusMessage.
+
+        IFF the message came from the dashboard and contains AmigaTpdo1 structure,
+        formatting, and cobid.
+
+        Args:
+            message: The raw canbus message to parse.
+
+        Returns:
+            The parsed AmigaTpdo1 message.
+        """
+        if message.id != cls.cob_id + DASHBOARD_NODE_ID:
+            raise ValueError(f"Expected message from dashboard, received message from node {message.id - cls.cob_id}")
+
+        return cls.from_can_data(message.data, stamp=message.stamp)
+
     def __str__(self):
         return "AMIGA TPDO1 Amiga state {} Measured speed {:0.3f} Measured angular rate {:0.3f} @ time {}".format(
             self.state, self.meas_speed, self.meas_ang_rate, self.stamp.stamp
         ) + " PTO bits 0x{:x} h-bridge bits 0x{:x}".format(self.pto_bits, self.hbridge_bits)
 
 
 def parse_amiga_tpdo1_proto(message: canbus_pb2.RawCanbusMessage) -> AmigaTpdo1 | None:
     """Parses a canbus_pb2.RawCanbusMessage.
 
     IFF the message came from the dashboard and contains AmigaTpdo1 structure,
     formatting, and cobid.
 
+    WARNING: Deprecated starting with farm-ng-amiga v2.3.0
+    Please use AmigaTpdo1.from_raw_canbus_message() instead.
+
     Args:
         message: The raw canbus message to parse.
 
     Returns:
         The parsed AmigaTpdo1 message, or None if the message is not a valid AmigaTpdo1 message.
     """
+    logging.warning("parse_amiga_tpdo1_proto is deprecated as of v2.3.0")
+    logging.warning("Use AmigaTpdo1.from_raw_canbus_message() instead.")
+
     # TODO: add some checkers, or make python CHECK_API
     if message.id != AmigaTpdo1.cob_id + DASHBOARD_NODE_ID:
         return None
     return AmigaTpdo1.from_can_data(message.data, stamp=message.stamp)
 
 
 class MotorControllerStatus(IntEnum):
@@ -355,7 +408,86 @@
     def __str__(self):
         return (
             "Motor state - id {:01X} status {} rpm {:4} voltage {:.3f} "
             "current {:.3f} temperature {:.1f} @ time {:.3f}".format(
                 self.id, self.status.name, self.rpm, self.voltage, self.current, self.temperature, self.timestamp
             )
         )
+
+
+class PendantState(Packet):
+    """State of the Pendant (joystick position & pressed buttons)"""
+
+    scale = 32767
+    format = "<hhI"
+    cob_id = 0x180
+
+    def __init__(self, x=0, y=0, buttons=0):
+        self.x = x  # [-1.0, 1.0] => [left, right]
+        self.y = y  # [-1.0, 1.0] => [reverse, forward]
+        self.buttons = buttons
+        self.stamp_packet(time.monotonic())
+
+    def encode(self):
+        """Returns the data contained by the class encoded as CAN message data."""
+        return pack(self.format, int(self.x * self.scale), int(self.y * self.scale), self.buttons)
+
+    def decode(self, data):
+        """Decodes CAN message data and populates the values of the class."""
+
+        (xi, yi, self.buttons) = unpack(self.format, data)
+        self.x = xi / self.scale
+        self.y = yi / self.scale
+
+    def to_proto(self) -> amiga_v6_pb2.PendantState:
+        """Packs the class data into a PendantState proto message.
+
+        Returns: An instance of a PendantState proto.
+        """
+        return amiga_v6_pb2.PendantState(
+            node_id=PENDANT_NODE_ID, stamp=self.stamp.stamp, x=self.x, y=self.y, buttons=self.buttons
+        )
+
+    @classmethod
+    def from_proto(cls, proto: amiga_v6_pb2.PendantState) -> PendantState:
+        """Creates an instance of the class from a proto message.
+
+        Args:
+            proto: The PendantState proto message to parse.
+        """
+        # Check for correct proto
+        if not isinstance(proto, amiga_v6_pb2.PendantState):
+            raise TypeError(f"Expected amiga_v6_pb2.PendantState proto, received {type(proto)}")
+
+        obj = cls()
+        obj.stamp_packet(proto.stamp)
+        obj.x = proto.x
+        obj.y = proto.y
+        obj.buttons = proto.buttons
+        return obj
+
+    @classmethod
+    def from_raw_canbus_message(cls, message: canbus_pb2.RawCanbusMessage) -> PendantState:
+        """Parses a canbus_pb2.RawCanbusMessage.
+
+        IFF the message came from the pendant and contains PendantState structure,
+        formatting, and cobid.
+
+        Args:
+            message: The raw canbus message to parse.
+
+        Returns:
+            The parsed PendantState message.
+        """
+        if message.id != cls.cob_id + PENDANT_NODE_ID:
+            raise ValueError(f"Expected message from pendant, received message from node {message.id}")
+
+        return cls.from_can_data(message.data, stamp=message.stamp)
+
+    def is_button_pressed(self, button: PendantButtons) -> bool:
+        """Returns True if the button is pressed."""
+        if not isinstance(button, PendantButtons):
+            raise TypeError(f"Expected PendantButtons, received {type(button)}")
+        return bool(self.buttons & button)
+
+    def __str__(self):
+        return "x {:0.3f} y {:0.3f} buttons {}".format(self.x, self.y, self.buttons)
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/filter/__init__.py` & `farm_ng_amiga-2.3.0/py/farm_ng/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/filter/filter.proto` & `farm_ng_amiga-2.3.0/py/farm_ng/filter/filter.proto`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,19 @@
   GPS_ERROR_X_HIGH = 1;
   GPS_ERROR_Y_HIGH = 2;
   STD_DEV_X_HIGH = 3;
   STD_DEV_Y_HIGH = 4;
   STD_DEV_W_HIGH = 5;
   NO_GYRO_MEASUREMENTS = 6;
   GYRO_MEASUREMENTS_DELAYED = 7;
+  INVALID_GPS_MESSAGE = 8;
+  NO_GPS_MEASUREMENTS = 9;
+  GPS_MEASUREMENTS_DELAYED = 10;
+  NO_WHEEL_ODOMETRY_MEASUREMENTS = 11;
+  WHEEL_ODOMETRY_MEASUREMENTS_DELAYED = 12;
   OTHER_DIVERGENCE_REASON = 99;
 }
 
 message FilterState {
   // UKF state
   farm_ng.core.proto.Pose pose = 1;
   bool has_converged = 2;
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/filter/filter_pb2.py` & `farm_ng_amiga-2.3.0/py/farm_ng/filter/filter_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/filter/filter.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from farm_ng.core import linalg_pb2 as farm__ng_dot_core_dot_linalg__pb2
 from farm_ng.core import pose_pb2 as farm__ng_dot_core_dot_pose__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66\x61rm_ng/filter/filter.proto\x12\x14\x66\x61rm_ng.filter.proto\x1a\x19\x66\x61rm_ng/core/linalg.proto\x1a\x17\x66\x61rm_ng/core/pose.proto\"\xa7\x02\n\x0b\x46ilterState\x12&\n\x04pose\x18\x01 \x01(\x0b\x32\x18.farm_ng.core.proto.Pose\x12\x15\n\rhas_converged\x18\x02 \x01(\x08\x12\x15\n\ris_calibrated\x18\x03 \x01(\x08\x12\x39\n\x14uncertainty_diagonal\x18\x04 \x01(\x0b\x32\x1b.farm_ng.core.proto.VecXF64\x12/\n\ninnovation\x18\x05 \x01(\x0b\x32\x1b.farm_ng.core.proto.VecXF64\x12\x0f\n\x07heading\x18\x06 \x01(\x01\x12\x45\n\x13\x64ivergence_criteria\x18\x07 \x03(\x0e\x32(.farm_ng.filter.proto.DivergenceCriteria\"N\n\x0b\x46ilterTrack\x12\x31\n\x06states\x18\x01 \x03(\x0b\x32!.farm_ng.filter.proto.FilterState\x12\x0c\n\x04name\x18\x02 \x01(\t*\xf0\x01\n\x12\x44ivergenceCriteria\x12\x1c\n\x18UNKNOWN_DIVERGENCE_STATE\x10\x00\x12\x14\n\x10GPS_ERROR_X_HIGH\x10\x01\x12\x14\n\x10GPS_ERROR_Y_HIGH\x10\x02\x12\x12\n\x0eSTD_DEV_X_HIGH\x10\x03\x12\x12\n\x0eSTD_DEV_Y_HIGH\x10\x04\x12\x12\n\x0eSTD_DEV_W_HIGH\x10\x05\x12\x18\n\x14NO_GYRO_MEASUREMENTS\x10\x06\x12\x1d\n\x19GYRO_MEASUREMENTS_DELAYED\x10\x07\x12\x1b\n\x17OTHER_DIVERGENCE_REASON\x10\x63\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66\x61rm_ng/filter/filter.proto\x12\x14\x66\x61rm_ng.filter.proto\x1a\x19\x66\x61rm_ng/core/linalg.proto\x1a\x17\x66\x61rm_ng/core/pose.proto\"\xa7\x02\n\x0b\x46ilterState\x12&\n\x04pose\x18\x01 \x01(\x0b\x32\x18.farm_ng.core.proto.Pose\x12\x15\n\rhas_converged\x18\x02 \x01(\x08\x12\x15\n\ris_calibrated\x18\x03 \x01(\x08\x12\x39\n\x14uncertainty_diagonal\x18\x04 \x01(\x0b\x32\x1b.farm_ng.core.proto.VecXF64\x12/\n\ninnovation\x18\x05 \x01(\x0b\x32\x1b.farm_ng.core.proto.VecXF64\x12\x0f\n\x07heading\x18\x06 \x01(\x01\x12\x45\n\x13\x64ivergence_criteria\x18\x07 \x03(\x0e\x32(.farm_ng.filter.proto.DivergenceCriteria\"N\n\x0b\x46ilterTrack\x12\x31\n\x06states\x18\x01 \x03(\x0b\x32!.farm_ng.filter.proto.FilterState\x12\x0c\n\x04name\x18\x02 \x01(\t*\x8d\x03\n\x12\x44ivergenceCriteria\x12\x1c\n\x18UNKNOWN_DIVERGENCE_STATE\x10\x00\x12\x14\n\x10GPS_ERROR_X_HIGH\x10\x01\x12\x14\n\x10GPS_ERROR_Y_HIGH\x10\x02\x12\x12\n\x0eSTD_DEV_X_HIGH\x10\x03\x12\x12\n\x0eSTD_DEV_Y_HIGH\x10\x04\x12\x12\n\x0eSTD_DEV_W_HIGH\x10\x05\x12\x18\n\x14NO_GYRO_MEASUREMENTS\x10\x06\x12\x1d\n\x19GYRO_MEASUREMENTS_DELAYED\x10\x07\x12\x17\n\x13INVALID_GPS_MESSAGE\x10\x08\x12\x17\n\x13NO_GPS_MEASUREMENTS\x10\t\x12\x1c\n\x18GPS_MEASUREMENTS_DELAYED\x10\n\x12\"\n\x1eNO_WHEEL_ODOMETRY_MEASUREMENTS\x10\x0b\x12\'\n#WHEEL_ODOMETRY_MEASUREMENTS_DELAYED\x10\x0c\x12\x1b\n\x17OTHER_DIVERGENCE_REASON\x10\x63\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.filter.filter_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_DIVERGENCECRITERIA']._serialized_start=484
-  _globals['_DIVERGENCECRITERIA']._serialized_end=724
+  _globals['_DIVERGENCECRITERIA']._serialized_end=881
   _globals['_FILTERSTATE']._serialized_start=106
   _globals['_FILTERSTATE']._serialized_end=401
   _globals['_FILTERTRACK']._serialized_start=403
   _globals['_FILTERTRACK']._serialized_end=481
 # @@protoc_insertion_point(module_scope)
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/filter/filter_pb2.pyi` & `farm_ng_amiga-2.3.0/py/farm_ng/filter/filter_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -14,23 +14,33 @@
     GPS_ERROR_X_HIGH: _ClassVar[DivergenceCriteria]
     GPS_ERROR_Y_HIGH: _ClassVar[DivergenceCriteria]
     STD_DEV_X_HIGH: _ClassVar[DivergenceCriteria]
     STD_DEV_Y_HIGH: _ClassVar[DivergenceCriteria]
     STD_DEV_W_HIGH: _ClassVar[DivergenceCriteria]
     NO_GYRO_MEASUREMENTS: _ClassVar[DivergenceCriteria]
     GYRO_MEASUREMENTS_DELAYED: _ClassVar[DivergenceCriteria]
+    INVALID_GPS_MESSAGE: _ClassVar[DivergenceCriteria]
+    NO_GPS_MEASUREMENTS: _ClassVar[DivergenceCriteria]
+    GPS_MEASUREMENTS_DELAYED: _ClassVar[DivergenceCriteria]
+    NO_WHEEL_ODOMETRY_MEASUREMENTS: _ClassVar[DivergenceCriteria]
+    WHEEL_ODOMETRY_MEASUREMENTS_DELAYED: _ClassVar[DivergenceCriteria]
     OTHER_DIVERGENCE_REASON: _ClassVar[DivergenceCriteria]
 UNKNOWN_DIVERGENCE_STATE: DivergenceCriteria
 GPS_ERROR_X_HIGH: DivergenceCriteria
 GPS_ERROR_Y_HIGH: DivergenceCriteria
 STD_DEV_X_HIGH: DivergenceCriteria
 STD_DEV_Y_HIGH: DivergenceCriteria
 STD_DEV_W_HIGH: DivergenceCriteria
 NO_GYRO_MEASUREMENTS: DivergenceCriteria
 GYRO_MEASUREMENTS_DELAYED: DivergenceCriteria
+INVALID_GPS_MESSAGE: DivergenceCriteria
+NO_GPS_MEASUREMENTS: DivergenceCriteria
+GPS_MEASUREMENTS_DELAYED: DivergenceCriteria
+NO_WHEEL_ODOMETRY_MEASUREMENTS: DivergenceCriteria
+WHEEL_ODOMETRY_MEASUREMENTS_DELAYED: DivergenceCriteria
 OTHER_DIVERGENCE_REASON: DivergenceCriteria
 
 class FilterState(_message.Message):
     __slots__ = ("pose", "has_converged", "is_calibrated", "uncertainty_diagonal", "innovation", "heading", "divergence_criteria")
     POSE_FIELD_NUMBER: _ClassVar[int]
     HAS_CONVERGED_FIELD_NUMBER: _ClassVar[int]
     IS_CALIBRATED_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/gps/__init__.py` & `farm_ng_amiga-2.3.0/py/farm_ng/gps/__init__.py`

 * *Files identical despite different names*

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/gps/gps.proto` & `farm_ng_amiga-2.3.0/py/farm_ng/gps/gps.proto`

 * *Files 4% similar despite different names*

```diff
@@ -29,30 +29,31 @@
     bool heading_vehicle_valid = 3; // heading of vehicle is valid
 }
 
 message UtcStamp {
     // Based (closely) on the fields in NAV-PVT message
     // https://github.com/KumarRobotics/ublox/blob/master/ublox_msgs/msg/NavPVT.msg
     // But tweaked to match the UBX NAV-PVT message we get from the Ublox
+    reserved 14; // Removed fields cannot be reused
 
-    int32 iTOW = 1;    // uint32 iTOW  -> GPS Millisecond time of week [ms]
-    int32 year = 2;    // uint16 year  -> Year (UTC)
-    int32 month = 3;   // uint8 month  -> Month, range 1..12 (UTC)
-    int32 day = 4;     // uint8 day    -> Day of month, range 1..31 (UTC)
-    int32 hour = 5;    // uint8 hour   -> Hour of day, range 0..23 (UTC)
-    int32 min = 6;     // uint8 min    -> Minute of hour, range 0..59 (UTC)
-    int32 sec = 7;     // uint8 second -> Seconds of minute, range 0..60 (UTC)
-    int32 nano = 8;    // int32 nano   -> Fraction of second, range -1e9 .. 1e9 (UTC)
-    int32 tAcc = 9;    // uint32 tAcc  -> Time accuracy estimate (UTC)
+    uint32 iTOW = 1;    // uint32 iTOW  -> GPS Millisecond time of week [ms]
+    uint32 year = 2;    // uint16 year  -> Year (UTC)
+    uint32 month = 3;   // uint8 month  -> Month, range 1..12 (UTC)
+    uint32 day = 4;     // uint8 day    -> Day of month, range 1..31 (UTC)
+    uint32 hour = 5;    // uint8 hour   -> Hour of day, range 0..23 (UTC)
+    uint32 min = 6;     // uint8 min    -> Minute of hour, range 0..59 (UTC)
+    uint32 sec = 7;     // uint8 second -> Seconds of minute, range 0..60 (UTC)
+    int32 nano = 8;     // int32 nano   -> Fraction of second, range -1e9 .. 1e9 (UTC)
+    uint32 tAcc = 9;    // uint32 tAcc  -> Time accuracy estimate (UTC)
 
     // Validity flags
-    int32 valid_date = 11;     // uint8 validDate -> Valid UTC Date
-    int32 valid_time = 12;     // uint8 validTime -> Valid UTC Time of Day
-    int32 fully_resolved = 13; // uint8 fullyResolved -> UTC time of day has been fully resolved (no seconds uncertainty)
-    int32 valid_mag = 14;      // uint8 validMag -> Valid Magnetic Declination
+    bool valid_date = 11;     // uint8 validDate -> Valid UTC Date
+    bool valid_time = 12;     // uint8 validTime -> Valid UTC Time of Day
+    bool fully_resolved = 13; // uint8 fullyResolved -> UTC time of day has been fully resolved (no seconds uncertainty)
+    // Removed: int32 valid_mag = 14; // uint8 validMag -> Valid Magnetic Declination
 }
 
 message GpsFrame { // NAV-PVT
     farm_ng.core.proto.Timestamp stamp = 1;      // seconds, host receive time in monotonic clock
     farm_ng.core.proto.Timestamp gps_time = 14;  // seconds, measurement sample time converted to POSIX clock
     double longitude = 2;           // angle from meridian (Wgs84), radians (+ive easterly)
     double latitude = 3;            // angle from equator (Wgs84), radians  (+ive northerly)
@@ -63,47 +64,62 @@
     double ground_speed = 8;        // m/s Ground Speed (2-D)
     float speed_accuracy = 9;       // m/s Speed accuracy estimate
     double vel_north = 10;          // m/s N.E.D. north velocity
     double vel_east =11;            // m/s N.E.D. east velocity
     double vel_down = 12;           // m/s N.E.D. down velocity
     float horizontal_accuracy = 15; // stddev m/s?
     float vertical_accuracy = 16;   // stddev m/s?
-    int32 position_mode = 17;       // GNSSfix Type: 0: no fix 1: dead reckoning only 2: 2D-fix 3: 3D-fix 4: GNSS + dead reckoning combined 5: time only fix
+    uint32 position_mode = 17;      // GNSSfix Type: 0: no fix 1: dead reckoning only 2: 2D-fix 3: 3D-fix 4: GNSS + dead reckoning combined 5: time only fix
     double p_dop = 18;              // Position DOP [1 / 0.01]
     double height = 19;             // Height above ellipsoid
     GpsFrameStatus status = 13;
     UtcStamp utc_stamp = 20;
+    uint32 num_satellites = 21;      // Number of satellites used in Nav Solution
 }
 
 message RelativePositionFrame { // NAV-RELPOSNED
   farm_ng.core.proto.Timestamp stamp = 1;    // seconds, host receive time in monotonic clock
   farm_ng.core.proto.Timestamp gps_time = 2; // seconds, measurement sample time converted to POSIX clock
-  int32 base_station_id = 3;
+  uint32 base_station_id = 3;
   double relative_pose_north = 4;    // northerly distance from base in meters
   double relative_pose_east = 5;     // easterly distance from base in meters
   double relative_pose_down = 6;     // down distance from base in meters
   double relative_pose_heading = 7;  // bearing in radians (check?)
   double relative_pose_length = 8;   // radial distance in meters (check?)
   bool rel_pos_valid = 9;            // if relative position components and accuracies are valid and, in moving base mode only, if baseline is valid
   bool rel_heading_valid = 10;       // 1 if the components of the relative position vector (including the high-precision parts) are normalized
   float accuracy_north = 11;         // stddev meters
   float accuracy_east = 12;          // stddev meters
   float accuracy_down = 13;          // stddev meters
   float accuracy_length = 14;        // stddev meters
   float accuracy_heading = 15;       // stddev radians (check?)
-  int32 carr_soln = 16;              // Carrier phase range solution status: 0 = no carrier phase range solution 1 = carrier phase range solution with floating ambiguities 2 = carrier phase range solution with fixed ambiguities
+  uint32 carr_soln = 16;              // Carrier phase range solution status: 0 = no carrier phase range solution 1 = carrier phase range solution with floating ambiguities 2 = carrier phase range solution with fixed ambiguities
   bool is_moving = 17;               // 1 if the receiver is operating in moving base mode
   bool ref_obs_miss = 18;            // 1 if extrapolated reference observations were used to compute moving base solution this epoch
   bool ref_pos_miss = 19;            // 1 if extrapolated reference position was used to compute moving base solution this epoch
   bool ref_pos_normalized = 20;      // ?
   bool gnss_fix_ok = 21;
   bool base_coords_known = 22;       // 1 if the base / reference station coordinates are known
   GpsCoordinates base_coords = 23;   // base / reference station coordinates, if known
 }
 
-message GpsCoordinates{
+message GpsCoordinates {
   // Not necessarily a reading directly from the GPS receiver.
   // Likely a created / calculated set of GPS coordinates.
   double longitude = 1; // angle from meridian (Wgs84), radians (+ive easterly)
   double latitude = 2;  // angle from equator (Wgs84), radians  (+ive northerly)
   double altitude = 3;  // meters above Wgs84 reference geoid
 }
+
+message EcefCoordinates {
+  farm_ng.core.proto.Timestamp stamp = 1;    // seconds, host receive time in monotonic clock
+  farm_ng.core.proto.Timestamp gps_time = 2; // seconds, measurement sample time converted to POSIX clock
+  double x = 3;    // meters
+  double y = 4;    // meters
+  double z = 5;    // meters
+  float accuracy = 6;   // stddev meters
+  EcefFlags flags = 7;
+}
+
+message EcefFlags {
+  bool INVALID_ECEF = 1;
+}
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/gps/gps_pb2.py` & `farm_ng_amiga-2.3.0/py/farm_ng/gps/gps_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/gps/gps.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from farm_ng.core import timestamp_pb2 as farm__ng_dot_core_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x66\x61rm_ng/gps/gps.proto\x12\x11\x66\x61rm_ng.gps.proto\x1a\x1c\x66\x61rm_ng/core/timestamp.proto\"t\n\x0eGpsFrameStatus\x12\x1b\n\x13time_fully_resolved\x18\x01 \x01(\x08\x12\x13\n\x0bgnss_fix_ok\x18\x02 \x01(\x08\x12\x11\n\tdiff_soln\x18\x04 \x01(\x08\x12\x1d\n\x15heading_vehicle_valid\x18\x03 \x01(\x08\"\xd9\x01\n\x08UtcStamp\x12\x0c\n\x04iTOW\x18\x01 \x01(\x05\x12\x0c\n\x04year\x18\x02 \x01(\x05\x12\r\n\x05month\x18\x03 \x01(\x05\x12\x0b\n\x03\x64\x61y\x18\x04 \x01(\x05\x12\x0c\n\x04hour\x18\x05 \x01(\x05\x12\x0b\n\x03min\x18\x06 \x01(\x05\x12\x0b\n\x03sec\x18\x07 \x01(\x05\x12\x0c\n\x04nano\x18\x08 \x01(\x05\x12\x0c\n\x04tAcc\x18\t \x01(\x05\x12\x12\n\nvalid_date\x18\x0b \x01(\x05\x12\x12\n\nvalid_time\x18\x0c \x01(\x05\x12\x16\n\x0e\x66ully_resolved\x18\r \x01(\x05\x12\x11\n\tvalid_mag\x18\x0e \x01(\x05\"\xa1\x04\n\x08GpsFrame\x12,\n\x05stamp\x18\x01 \x01(\x0b\x32\x1d.farm_ng.core.proto.Timestamp\x12/\n\x08gps_time\x18\x0e \x01(\x0b\x32\x1d.farm_ng.core.proto.Timestamp\x12\x11\n\tlongitude\x18\x02 \x01(\x01\x12\x10\n\x08latitude\x18\x03 \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x04 \x01(\x01\x12\x17\n\x0fheading_vehicle\x18\x05 \x01(\x01\x12\x16\n\x0eheading_motion\x18\x06 \x01(\x01\x12\x18\n\x10heading_accuracy\x18\x07 \x01(\x02\x12\x14\n\x0cground_speed\x18\x08 \x01(\x01\x12\x16\n\x0espeed_accuracy\x18\t \x01(\x02\x12\x11\n\tvel_north\x18\n \x01(\x01\x12\x10\n\x08vel_east\x18\x0b \x01(\x01\x12\x10\n\x08vel_down\x18\x0c \x01(\x01\x12\x1b\n\x13horizontal_accuracy\x18\x0f \x01(\x02\x12\x19\n\x11vertical_accuracy\x18\x10 \x01(\x02\x12\x15\n\rposition_mode\x18\x11 \x01(\x05\x12\r\n\x05p_dop\x18\x12 \x01(\x01\x12\x0e\n\x06height\x18\x13 \x01(\x01\x12\x31\n\x06status\x18\r \x01(\x0b\x32!.farm_ng.gps.proto.GpsFrameStatus\x12.\n\tutc_stamp\x18\x14 \x01(\x0b\x32\x1b.farm_ng.gps.proto.UtcStamp\"\xa2\x05\n\x15RelativePositionFrame\x12,\n\x05stamp\x18\x01 \x01(\x0b\x32\x1d.farm_ng.core.proto.Timestamp\x12/\n\x08gps_time\x18\x02 \x01(\x0b\x32\x1d.farm_ng.core.proto.Timestamp\x12\x17\n\x0f\x62\x61se_station_id\x18\x03 \x01(\x05\x12\x1b\n\x13relative_pose_north\x18\x04 \x01(\x01\x12\x1a\n\x12relative_pose_east\x18\x05 \x01(\x01\x12\x1a\n\x12relative_pose_down\x18\x06 \x01(\x01\x12\x1d\n\x15relative_pose_heading\x18\x07 \x01(\x01\x12\x1c\n\x14relative_pose_length\x18\x08 \x01(\x01\x12\x15\n\rrel_pos_valid\x18\t \x01(\x08\x12\x19\n\x11rel_heading_valid\x18\n \x01(\x08\x12\x16\n\x0e\x61\x63\x63uracy_north\x18\x0b \x01(\x02\x12\x15\n\raccuracy_east\x18\x0c \x01(\x02\x12\x15\n\raccuracy_down\x18\r \x01(\x02\x12\x17\n\x0f\x61\x63\x63uracy_length\x18\x0e \x01(\x02\x12\x18\n\x10\x61\x63\x63uracy_heading\x18\x0f \x01(\x02\x12\x11\n\tcarr_soln\x18\x10 \x01(\x05\x12\x11\n\tis_moving\x18\x11 \x01(\x08\x12\x14\n\x0cref_obs_miss\x18\x12 \x01(\x08\x12\x14\n\x0cref_pos_miss\x18\x13 \x01(\x08\x12\x1a\n\x12ref_pos_normalized\x18\x14 \x01(\x08\x12\x13\n\x0bgnss_fix_ok\x18\x15 \x01(\x08\x12\x19\n\x11\x62\x61se_coords_known\x18\x16 \x01(\x08\x12\x36\n\x0b\x62\x61se_coords\x18\x17 \x01(\x0b\x32!.farm_ng.gps.proto.GpsCoordinates\"G\n\x0eGpsCoordinates\x12\x11\n\tlongitude\x18\x01 \x01(\x01\x12\x10\n\x08latitude\x18\x02 \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x66\x61rm_ng/gps/gps.proto\x12\x11\x66\x61rm_ng.gps.proto\x1a\x1c\x66\x61rm_ng/core/timestamp.proto\"t\n\x0eGpsFrameStatus\x12\x1b\n\x13time_fully_resolved\x18\x01 \x01(\x08\x12\x13\n\x0bgnss_fix_ok\x18\x02 \x01(\x08\x12\x11\n\tdiff_soln\x18\x04 \x01(\x08\x12\x1d\n\x15heading_vehicle_valid\x18\x03 \x01(\x08\"\xcc\x01\n\x08UtcStamp\x12\x0c\n\x04iTOW\x18\x01 \x01(\r\x12\x0c\n\x04year\x18\x02 \x01(\r\x12\r\n\x05month\x18\x03 \x01(\r\x12\x0b\n\x03\x64\x61y\x18\x04 \x01(\r\x12\x0c\n\x04hour\x18\x05 \x01(\r\x12\x0b\n\x03min\x18\x06 \x01(\r\x12\x0b\n\x03sec\x18\x07 \x01(\r\x12\x0c\n\x04nano\x18\x08 \x01(\x05\x12\x0c\n\x04tAcc\x18\t \x01(\r\x12\x12\n\nvalid_date\x18\x0b \x01(\x08\x12\x12\n\nvalid_time\x18\x0c \x01(\x08\x12\x16\n\x0e\x66ully_resolved\x18\r \x01(\x08J\x04\x08\x0e\x10\x0f\"\xb9\x04\n\x08GpsFrame\x12,\n\x05stamp\x18\x01 \x01(\x0b\x32\x1d.farm_ng.core.proto.Timestamp\x12/\n\x08gps_time\x18\x0e \x01(\x0b\x32\x1d.farm_ng.core.proto.Timestamp\x12\x11\n\tlongitude\x18\x02 \x01(\x01\x12\x10\n\x08latitude\x18\x03 \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x04 \x01(\x01\x12\x17\n\x0fheading_vehicle\x18\x05 \x01(\x01\x12\x16\n\x0eheading_motion\x18\x06 \x01(\x01\x12\x18\n\x10heading_accuracy\x18\x07 \x01(\x02\x12\x14\n\x0cground_speed\x18\x08 \x01(\x01\x12\x16\n\x0espeed_accuracy\x18\t \x01(\x02\x12\x11\n\tvel_north\x18\n \x01(\x01\x12\x10\n\x08vel_east\x18\x0b \x01(\x01\x12\x10\n\x08vel_down\x18\x0c \x01(\x01\x12\x1b\n\x13horizontal_accuracy\x18\x0f \x01(\x02\x12\x19\n\x11vertical_accuracy\x18\x10 \x01(\x02\x12\x15\n\rposition_mode\x18\x11 \x01(\r\x12\r\n\x05p_dop\x18\x12 \x01(\x01\x12\x0e\n\x06height\x18\x13 \x01(\x01\x12\x31\n\x06status\x18\r \x01(\x0b\x32!.farm_ng.gps.proto.GpsFrameStatus\x12.\n\tutc_stamp\x18\x14 \x01(\x0b\x32\x1b.farm_ng.gps.proto.UtcStamp\x12\x16\n\x0enum_satellites\x18\x15 \x01(\r\"\xa2\x05\n\x15RelativePositionFrame\x12,\n\x05stamp\x18\x01 \x01(\x0b\x32\x1d.farm_ng.core.proto.Timestamp\x12/\n\x08gps_time\x18\x02 \x01(\x0b\x32\x1d.farm_ng.core.proto.Timestamp\x12\x17\n\x0f\x62\x61se_station_id\x18\x03 \x01(\r\x12\x1b\n\x13relative_pose_north\x18\x04 \x01(\x01\x12\x1a\n\x12relative_pose_east\x18\x05 \x01(\x01\x12\x1a\n\x12relative_pose_down\x18\x06 \x01(\x01\x12\x1d\n\x15relative_pose_heading\x18\x07 \x01(\x01\x12\x1c\n\x14relative_pose_length\x18\x08 \x01(\x01\x12\x15\n\rrel_pos_valid\x18\t \x01(\x08\x12\x19\n\x11rel_heading_valid\x18\n \x01(\x08\x12\x16\n\x0e\x61\x63\x63uracy_north\x18\x0b \x01(\x02\x12\x15\n\raccuracy_east\x18\x0c \x01(\x02\x12\x15\n\raccuracy_down\x18\r \x01(\x02\x12\x17\n\x0f\x61\x63\x63uracy_length\x18\x0e \x01(\x02\x12\x18\n\x10\x61\x63\x63uracy_heading\x18\x0f \x01(\x02\x12\x11\n\tcarr_soln\x18\x10 \x01(\r\x12\x11\n\tis_moving\x18\x11 \x01(\x08\x12\x14\n\x0cref_obs_miss\x18\x12 \x01(\x08\x12\x14\n\x0cref_pos_miss\x18\x13 \x01(\x08\x12\x1a\n\x12ref_pos_normalized\x18\x14 \x01(\x08\x12\x13\n\x0bgnss_fix_ok\x18\x15 \x01(\x08\x12\x19\n\x11\x62\x61se_coords_known\x18\x16 \x01(\x08\x12\x36\n\x0b\x62\x61se_coords\x18\x17 \x01(\x0b\x32!.farm_ng.gps.proto.GpsCoordinates\"G\n\x0eGpsCoordinates\x12\x11\n\tlongitude\x18\x01 \x01(\x01\x12\x10\n\x08latitude\x18\x02 \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x01\"\xd0\x01\n\x0f\x45\x63\x65\x66\x43oordinates\x12,\n\x05stamp\x18\x01 \x01(\x0b\x32\x1d.farm_ng.core.proto.Timestamp\x12/\n\x08gps_time\x18\x02 \x01(\x0b\x32\x1d.farm_ng.core.proto.Timestamp\x12\t\n\x01x\x18\x03 \x01(\x01\x12\t\n\x01y\x18\x04 \x01(\x01\x12\t\n\x01z\x18\x05 \x01(\x01\x12\x10\n\x08\x61\x63\x63uracy\x18\x06 \x01(\x02\x12+\n\x05\x66lags\x18\x07 \x01(\x0b\x32\x1c.farm_ng.gps.proto.EcefFlags\"!\n\tEcefFlags\x12\x14\n\x0cINVALID_ECEF\x18\x01 \x01(\x08\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.gps.gps_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_GPSFRAMESTATUS']._serialized_start=74
   _globals['_GPSFRAMESTATUS']._serialized_end=190
   _globals['_UTCSTAMP']._serialized_start=193
-  _globals['_UTCSTAMP']._serialized_end=410
-  _globals['_GPSFRAME']._serialized_start=413
-  _globals['_GPSFRAME']._serialized_end=958
-  _globals['_RELATIVEPOSITIONFRAME']._serialized_start=961
-  _globals['_RELATIVEPOSITIONFRAME']._serialized_end=1635
-  _globals['_GPSCOORDINATES']._serialized_start=1637
-  _globals['_GPSCOORDINATES']._serialized_end=1708
+  _globals['_UTCSTAMP']._serialized_end=397
+  _globals['_GPSFRAME']._serialized_start=400
+  _globals['_GPSFRAME']._serialized_end=969
+  _globals['_RELATIVEPOSITIONFRAME']._serialized_start=972
+  _globals['_RELATIVEPOSITIONFRAME']._serialized_end=1646
+  _globals['_GPSCOORDINATES']._serialized_start=1648
+  _globals['_GPSCOORDINATES']._serialized_end=1719
+  _globals['_ECEFCOORDINATES']._serialized_start=1722
+  _globals['_ECEFCOORDINATES']._serialized_end=1930
+  _globals['_ECEFFLAGS']._serialized_start=1932
+  _globals['_ECEFFLAGS']._serialized_end=1965
 # @@protoc_insertion_point(module_scope)
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/gps/gps_pb2.pyi` & `farm_ng_amiga-2.3.0/py/farm_ng/gps/gps_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,45 +14,43 @@
     time_fully_resolved: bool
     gnss_fix_ok: bool
     diff_soln: bool
     heading_vehicle_valid: bool
     def __init__(self, time_fully_resolved: bool = ..., gnss_fix_ok: bool = ..., diff_soln: bool = ..., heading_vehicle_valid: bool = ...) -> None: ...
 
 class UtcStamp(_message.Message):
-    __slots__ = ("iTOW", "year", "month", "day", "hour", "min", "sec", "nano", "tAcc", "valid_date", "valid_time", "fully_resolved", "valid_mag")
+    __slots__ = ("iTOW", "year", "month", "day", "hour", "min", "sec", "nano", "tAcc", "valid_date", "valid_time", "fully_resolved")
     ITOW_FIELD_NUMBER: _ClassVar[int]
     YEAR_FIELD_NUMBER: _ClassVar[int]
     MONTH_FIELD_NUMBER: _ClassVar[int]
     DAY_FIELD_NUMBER: _ClassVar[int]
     HOUR_FIELD_NUMBER: _ClassVar[int]
     MIN_FIELD_NUMBER: _ClassVar[int]
     SEC_FIELD_NUMBER: _ClassVar[int]
     NANO_FIELD_NUMBER: _ClassVar[int]
     TACC_FIELD_NUMBER: _ClassVar[int]
     VALID_DATE_FIELD_NUMBER: _ClassVar[int]
     VALID_TIME_FIELD_NUMBER: _ClassVar[int]
     FULLY_RESOLVED_FIELD_NUMBER: _ClassVar[int]
-    VALID_MAG_FIELD_NUMBER: _ClassVar[int]
     iTOW: int
     year: int
     month: int
     day: int
     hour: int
     min: int
     sec: int
     nano: int
     tAcc: int
-    valid_date: int
-    valid_time: int
-    fully_resolved: int
-    valid_mag: int
-    def __init__(self, iTOW: _Optional[int] = ..., year: _Optional[int] = ..., month: _Optional[int] = ..., day: _Optional[int] = ..., hour: _Optional[int] = ..., min: _Optional[int] = ..., sec: _Optional[int] = ..., nano: _Optional[int] = ..., tAcc: _Optional[int] = ..., valid_date: _Optional[int] = ..., valid_time: _Optional[int] = ..., fully_resolved: _Optional[int] = ..., valid_mag: _Optional[int] = ...) -> None: ...
+    valid_date: bool
+    valid_time: bool
+    fully_resolved: bool
+    def __init__(self, iTOW: _Optional[int] = ..., year: _Optional[int] = ..., month: _Optional[int] = ..., day: _Optional[int] = ..., hour: _Optional[int] = ..., min: _Optional[int] = ..., sec: _Optional[int] = ..., nano: _Optional[int] = ..., tAcc: _Optional[int] = ..., valid_date: bool = ..., valid_time: bool = ..., fully_resolved: bool = ...) -> None: ...
 
 class GpsFrame(_message.Message):
-    __slots__ = ("stamp", "gps_time", "longitude", "latitude", "altitude", "heading_vehicle", "heading_motion", "heading_accuracy", "ground_speed", "speed_accuracy", "vel_north", "vel_east", "vel_down", "horizontal_accuracy", "vertical_accuracy", "position_mode", "p_dop", "height", "status", "utc_stamp")
+    __slots__ = ("stamp", "gps_time", "longitude", "latitude", "altitude", "heading_vehicle", "heading_motion", "heading_accuracy", "ground_speed", "speed_accuracy", "vel_north", "vel_east", "vel_down", "horizontal_accuracy", "vertical_accuracy", "position_mode", "p_dop", "height", "status", "utc_stamp", "num_satellites")
     STAMP_FIELD_NUMBER: _ClassVar[int]
     GPS_TIME_FIELD_NUMBER: _ClassVar[int]
     LONGITUDE_FIELD_NUMBER: _ClassVar[int]
     LATITUDE_FIELD_NUMBER: _ClassVar[int]
     ALTITUDE_FIELD_NUMBER: _ClassVar[int]
     HEADING_VEHICLE_FIELD_NUMBER: _ClassVar[int]
     HEADING_MOTION_FIELD_NUMBER: _ClassVar[int]
@@ -65,14 +63,15 @@
     HORIZONTAL_ACCURACY_FIELD_NUMBER: _ClassVar[int]
     VERTICAL_ACCURACY_FIELD_NUMBER: _ClassVar[int]
     POSITION_MODE_FIELD_NUMBER: _ClassVar[int]
     P_DOP_FIELD_NUMBER: _ClassVar[int]
     HEIGHT_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     UTC_STAMP_FIELD_NUMBER: _ClassVar[int]
+    NUM_SATELLITES_FIELD_NUMBER: _ClassVar[int]
     stamp: _timestamp_pb2.Timestamp
     gps_time: _timestamp_pb2.Timestamp
     longitude: float
     latitude: float
     altitude: float
     heading_vehicle: float
     heading_motion: float
@@ -85,15 +84,16 @@
     horizontal_accuracy: float
     vertical_accuracy: float
     position_mode: int
     p_dop: float
     height: float
     status: GpsFrameStatus
     utc_stamp: UtcStamp
-    def __init__(self, stamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., gps_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., longitude: _Optional[float] = ..., latitude: _Optional[float] = ..., altitude: _Optional[float] = ..., heading_vehicle: _Optional[float] = ..., heading_motion: _Optional[float] = ..., heading_accuracy: _Optional[float] = ..., ground_speed: _Optional[float] = ..., speed_accuracy: _Optional[float] = ..., vel_north: _Optional[float] = ..., vel_east: _Optional[float] = ..., vel_down: _Optional[float] = ..., horizontal_accuracy: _Optional[float] = ..., vertical_accuracy: _Optional[float] = ..., position_mode: _Optional[int] = ..., p_dop: _Optional[float] = ..., height: _Optional[float] = ..., status: _Optional[_Union[GpsFrameStatus, _Mapping]] = ..., utc_stamp: _Optional[_Union[UtcStamp, _Mapping]] = ...) -> None: ...
+    num_satellites: int
+    def __init__(self, stamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., gps_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., longitude: _Optional[float] = ..., latitude: _Optional[float] = ..., altitude: _Optional[float] = ..., heading_vehicle: _Optional[float] = ..., heading_motion: _Optional[float] = ..., heading_accuracy: _Optional[float] = ..., ground_speed: _Optional[float] = ..., speed_accuracy: _Optional[float] = ..., vel_north: _Optional[float] = ..., vel_east: _Optional[float] = ..., vel_down: _Optional[float] = ..., horizontal_accuracy: _Optional[float] = ..., vertical_accuracy: _Optional[float] = ..., position_mode: _Optional[int] = ..., p_dop: _Optional[float] = ..., height: _Optional[float] = ..., status: _Optional[_Union[GpsFrameStatus, _Mapping]] = ..., utc_stamp: _Optional[_Union[UtcStamp, _Mapping]] = ..., num_satellites: _Optional[int] = ...) -> None: ...
 
 class RelativePositionFrame(_message.Message):
     __slots__ = ("stamp", "gps_time", "base_station_id", "relative_pose_north", "relative_pose_east", "relative_pose_down", "relative_pose_heading", "relative_pose_length", "rel_pos_valid", "rel_heading_valid", "accuracy_north", "accuracy_east", "accuracy_down", "accuracy_length", "accuracy_heading", "carr_soln", "is_moving", "ref_obs_miss", "ref_pos_miss", "ref_pos_normalized", "gnss_fix_ok", "base_coords_known", "base_coords")
     STAMP_FIELD_NUMBER: _ClassVar[int]
     GPS_TIME_FIELD_NUMBER: _ClassVar[int]
     BASE_STATION_ID_FIELD_NUMBER: _ClassVar[int]
     RELATIVE_POSE_NORTH_FIELD_NUMBER: _ClassVar[int]
@@ -146,7 +146,31 @@
     LONGITUDE_FIELD_NUMBER: _ClassVar[int]
     LATITUDE_FIELD_NUMBER: _ClassVar[int]
     ALTITUDE_FIELD_NUMBER: _ClassVar[int]
     longitude: float
     latitude: float
     altitude: float
     def __init__(self, longitude: _Optional[float] = ..., latitude: _Optional[float] = ..., altitude: _Optional[float] = ...) -> None: ...
+
+class EcefCoordinates(_message.Message):
+    __slots__ = ("stamp", "gps_time", "x", "y", "z", "accuracy", "flags")
+    STAMP_FIELD_NUMBER: _ClassVar[int]
+    GPS_TIME_FIELD_NUMBER: _ClassVar[int]
+    X_FIELD_NUMBER: _ClassVar[int]
+    Y_FIELD_NUMBER: _ClassVar[int]
+    Z_FIELD_NUMBER: _ClassVar[int]
+    ACCURACY_FIELD_NUMBER: _ClassVar[int]
+    FLAGS_FIELD_NUMBER: _ClassVar[int]
+    stamp: _timestamp_pb2.Timestamp
+    gps_time: _timestamp_pb2.Timestamp
+    x: float
+    y: float
+    z: float
+    accuracy: float
+    flags: EcefFlags
+    def __init__(self, stamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., gps_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., x: _Optional[float] = ..., y: _Optional[float] = ..., z: _Optional[float] = ..., accuracy: _Optional[float] = ..., flags: _Optional[_Union[EcefFlags, _Mapping]] = ...) -> None: ...
+
+class EcefFlags(_message.Message):
+    __slots__ = ("INVALID_ECEF",)
+    INVALID_ECEF_FIELD_NUMBER: _ClassVar[int]
+    INVALID_ECEF: bool
+    def __init__(self, INVALID_ECEF: bool = ...) -> None: ...
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/imu/__init__.py` & `farm_ng_amiga-2.3.0/py/farm_ng/imu/__init__.py`

 * *Files identical despite different names*

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/imu/imu_pb2.py` & `farm_ng_amiga-2.3.0/py/farm_ng/imu/imu_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/imu/imu.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -17,14 +17,14 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x66\x61rm_ng/imu/imu.proto\x12\x11\x66\x61rm_ng.imu.proto\x1a\x19\x66\x61rm_ng/core/linalg.proto\x1a\x16\x66\x61rm_ng/core/lie.proto\"m\n\x07ImuBias\x12.\n\tgyro_bias\x18\x01 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F64\x12\x32\n\raccelero_bias\x18\x02 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F64\"\xd8\x01\n\x03Imu\x12\x35\n\x10\x61ngular_velocity\x18\x02 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F64\x12\x38\n\x13linear_acceleration\x18\x03 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F64\x12\x36\n\x0borientation\x18\x04 \x01(\x0b\x32!.farm_ng.core.proto.QuaternionF64\x12(\n\x04\x62ias\x18\x05 \x01(\x0b\x32\x1a.farm_ng.imu.proto.ImuBiasb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.imu.imu_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_IMUBIAS']._serialized_start=95
   _globals['_IMUBIAS']._serialized_end=204
   _globals['_IMU']._serialized_start=207
   _globals['_IMU']._serialized_end=423
 # @@protoc_insertion_point(module_scope)
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/imu/imu_pb2.pyi` & `farm_ng_amiga-2.3.0/py/farm_ng/imu/imu_pb2.pyi`

 * *Files identical despite different names*

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/oak/__init__.py` & `farm_ng_amiga-2.3.0/py/farm_ng/oak/__init__.py`

 * *Files identical despite different names*

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/oak/oak_pb2.py` & `farm_ng_amiga-2.3.0/py/farm_ng/oak/oak_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,71 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/oak/oak.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from farm_ng.core import linalg_pb2 as farm__ng_dot_core_dot_linalg__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x66\x61rm_ng/oak/oak.proto\x12\x11\x66\x61rm_ng.oak.proto\x1a\x19\x66\x61rm_ng/core/linalg.proto\"c\n\x0e\x43\x61meraSettings\x12\x15\n\rauto_exposure\x18\x01 \x01(\x08\x12\x15\n\rexposure_time\x18\x02 \x01(\r\x12\x11\n\tiso_value\x18\x03 \x01(\r\x12\x10\n\x08lens_pos\x18\x04 \x01(\r\"\xc6\x01\n\x0cOakImageMeta\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\x03\x12\x14\n\x0cinstance_num\x18\x02 \x01(\x03\x12\x14\n\x0csequence_num\x18\x03 \x01(\x03\x12\x11\n\ttimestamp\x18\x04 \x01(\x01\x12\x18\n\x10timestamp_device\x18\x05 \x01(\x01\x12\x16\n\x0etimestamp_recv\x18\x07 \x01(\x01\x12\x33\n\x08settings\x18\x06 \x01(\x0b\x32!.farm_ng.oak.proto.CameraSettings\"M\n\x08OakFrame\x12-\n\x04meta\x18\x01 \x01(\x0b\x32\x1f.farm_ng.oak.proto.OakImageMeta\x12\x12\n\nimage_data\x18\x02 \x01(\x0c\"\xa1\x01\n\x07OakGyro\x12)\n\x04gyro\x18\x01 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F32\x12\x14\n\x0csequence_num\x18\x02 \x01(\x05\x12\x10\n\x08\x61\x63\x63uracy\x18\x03 \x01(\t\x12\x11\n\ttimestamp\x18\x04 \x01(\x01\x12\x18\n\x10timestamp_device\x18\x05 \x01(\x01\x12\x16\n\x0etimestamp_recv\x18\x06 \x01(\x01\"\xa9\x01\n\x0bOakAccelero\x12-\n\x08\x61\x63\x63\x65lero\x18\x01 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F32\x12\x14\n\x0csequence_num\x18\x02 \x01(\x05\x12\x10\n\x08\x61\x63\x63uracy\x18\x03 \x01(\t\x12\x11\n\ttimestamp\x18\x04 \x01(\x01\x12\x18\n\x10timestamp_device\x18\x05 \x01(\x01\x12\x16\n\x0etimestamp_recv\x18\x06 \x01(\x01\"x\n\x0cOakImuPacket\x12/\n\x0bgyro_packet\x18\x01 \x01(\x0b\x32\x1a.farm_ng.oak.proto.OakGyro\x12\x37\n\x0f\x61\x63\x63\x65lero_packet\x18\x02 \x01(\x0b\x32\x1e.farm_ng.oak.proto.OakAccelero\"A\n\rOakImuPackets\x12\x30\n\x07packets\x18\x01 \x03(\x0b\x32\x1f.farm_ng.oak.proto.OakImuPacket\"7\n\rOakDeviceInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04mxid\x18\x02 \x01(\t\x12\n\n\x02ip\x18\x03 \x01(\t\"\xed\x02\n\x0cOakSyncFrame\x12)\n\x04left\x18\x01 \x01(\x0b\x32\x1b.farm_ng.oak.proto.OakFrame\x12*\n\x05right\x18\x02 \x01(\x0b\x32\x1b.farm_ng.oak.proto.OakFrame\x12(\n\x03rgb\x18\x03 \x01(\x0b\x32\x1b.farm_ng.oak.proto.OakFrame\x12.\n\tdisparity\x18\x04 \x01(\x0b\x32\x1b.farm_ng.oak.proto.OakFrame\x12(\n\x02nn\x18\x05 \x01(\x0b\x32\x1c.farm_ng.oak.proto.OakNNData\x12\x35\n\x0bimu_packets\x18\x06 \x01(\x0b\x32 .farm_ng.oak.proto.OakImuPackets\x12\x14\n\x0csequence_num\x18\x07 \x01(\x03\x12\x35\n\x0b\x64\x65vice_info\x18\x08 \x01(\x0b\x32 .farm_ng.oak.proto.OakDeviceInfo\"}\n\tOakNNData\x12-\n\x04meta\x18\x01 \x01(\x0b\x32\x1f.farm_ng.oak.proto.OakImageMeta\x12\x14\n\x0cnum_channels\x18\x02 \x01(\r\x12\x0e\n\x06height\x18\x03 \x01(\r\x12\r\n\x05width\x18\x04 \x01(\r\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\"\"\n\x04Pair\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"2\n\x08Metadata\x12&\n\x05pairs\x18\x01 \x03(\x0b\x32\x17.farm_ng.oak.proto.Pair\"n\n\rOakDataSample\x12.\n\x05\x66rame\x18\x01 \x01(\x0b\x32\x1f.farm_ng.oak.proto.OakSyncFrame\x12-\n\x08metadata\x18\x02 \x01(\x0b\x32\x1b.farm_ng.oak.proto.Metadata\")\n\x0eRotationMatrix\x12\x17\n\x0frotation_matrix\x18\x01 \x03(\x01\"\xa8\x01\n\nExtrinsics\x12\x17\n\x0frotation_matrix\x18\x01 \x03(\x01\x12\x35\n\x10spec_translation\x18\x02 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F32\x12\x18\n\x10to_camera_socket\x18\x03 \x01(\x05\x12\x30\n\x0btranslation\x18\x04 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F32\"\xec\x01\n\nCameraData\x12\x15\n\rcamera_number\x18\x01 \x01(\r\x12\x13\n\x0b\x63\x61mera_type\x18\x02 \x01(\x05\x12\x18\n\x10\x64istortion_coeff\x18\x03 \x03(\x01\x12\x31\n\nextrinsics\x18\x04 \x01(\x0b\x32\x1d.farm_ng.oak.proto.Extrinsics\x12\x0e\n\x06height\x18\x05 \x01(\r\x12\x18\n\x10intrinsic_matrix\x18\x06 \x03(\x01\x12\x15\n\rlens_position\x18\x07 \x01(\r\x12\x15\n\rspec_hfov_deg\x18\x08 \x01(\x01\x12\r\n\x05width\x18\t \x01(\r\"\x95\x01\n\x17StereoRectificationData\x12\x1a\n\x12left_camera_socket\x18\x01 \x01(\r\x12\x1f\n\x17rectified_rotation_left\x18\x02 \x03(\x01\x12 \n\x18rectified_rotation_right\x18\x03 \x03(\x01\x12\x1b\n\x13right_camera_socket\x18\x04 \x01(\r\"\xb4\x03\n\x0eOakCalibration\x12\x12\n\nbatch_name\x18\x01 \x01(\t\x12\x12\n\nbatch_time\x18\x02 \x01(\x05\x12\x12\n\nboard_conf\x18\x03 \x01(\t\x12\x14\n\x0c\x62oard_custom\x18\x04 \x01(\t\x12\x12\n\nboard_name\x18\x05 \x01(\t\x12\x15\n\rboard_options\x18\x06 \x01(\x05\x12\x11\n\tboard_rev\x18\x07 \x01(\t\x12\x32\n\x0b\x63\x61mera_data\x18\x08 \x03(\x0b\x32\x1d.farm_ng.oak.proto.CameraData\x12\x15\n\rhardware_conf\x18\t \x01(\t\x12\x35\n\x0eimu_extrinsics\x18\n \x01(\x0b\x32\x1d.farm_ng.oak.proto.Extrinsics\x12\x1a\n\x12miscellaneous_data\x18\x0b \x03(\t\x12\x14\n\x0cproduct_name\x18\x0c \x01(\t\x12M\n\x19stereo_rectification_data\x18\r \x01(\x0b\x32*.farm_ng.oak.proto.StereoRectificationData\x12\x0f\n\x07version\x18\x0e \x01(\rb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x66\x61rm_ng/oak/oak.proto\x12\x11\x66\x61rm_ng.oak.proto\x1a\x19\x66\x61rm_ng/core/linalg.proto\"c\n\x0e\x43\x61meraSettings\x12\x15\n\rauto_exposure\x18\x01 \x01(\x08\x12\x15\n\rexposure_time\x18\x02 \x01(\r\x12\x11\n\tiso_value\x18\x03 \x01(\r\x12\x10\n\x08lens_pos\x18\x04 \x01(\r\"\xe2\x01\n\x0e\x45ncoderOptions\x12\x32\n\x07profile\x18\x01 \x01(\x0e\x32!.farm_ng.oak.proto.EncoderProfile\x12=\n\x11rate_control_mode\x18\x02 \x01(\x0e\x32\".farm_ng.oak.proto.RateControlMode\x12\"\n\x1a\x63\x62r_preferred_bitrate_kbps\x18\x03 \x01(\r\x12\x1c\n\x14vbr_or_mjpeg_quality\x18\x04 \x01(\r\x12\x1b\n\x13\x66rames_per_keyframe\x18\x05 \x01(\r\"\x82\x02\n\x0cOakImageMeta\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\x03\x12\x14\n\x0cinstance_num\x18\x02 \x01(\x03\x12\x14\n\x0csequence_num\x18\x03 \x01(\x03\x12\x11\n\ttimestamp\x18\x04 \x01(\x01\x12\x18\n\x10timestamp_device\x18\x05 \x01(\x01\x12\x16\n\x0etimestamp_recv\x18\x07 \x01(\x01\x12\x33\n\x08settings\x18\x06 \x01(\x0b\x32!.farm_ng.oak.proto.CameraSettings\x12:\n\x0f\x65ncoder_options\x18\x08 \x01(\x0b\x32!.farm_ng.oak.proto.EncoderOptions\"M\n\x08OakFrame\x12-\n\x04meta\x18\x01 \x01(\x0b\x32\x1f.farm_ng.oak.proto.OakImageMeta\x12\x12\n\nimage_data\x18\x02 \x01(\x0c\"\xa1\x01\n\x07OakGyro\x12)\n\x04gyro\x18\x01 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F32\x12\x14\n\x0csequence_num\x18\x02 \x01(\x05\x12\x10\n\x08\x61\x63\x63uracy\x18\x03 \x01(\t\x12\x11\n\ttimestamp\x18\x04 \x01(\x01\x12\x18\n\x10timestamp_device\x18\x05 \x01(\x01\x12\x16\n\x0etimestamp_recv\x18\x06 \x01(\x01\"\xa9\x01\n\x0bOakAccelero\x12-\n\x08\x61\x63\x63\x65lero\x18\x01 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F32\x12\x14\n\x0csequence_num\x18\x02 \x01(\x05\x12\x10\n\x08\x61\x63\x63uracy\x18\x03 \x01(\t\x12\x11\n\ttimestamp\x18\x04 \x01(\x01\x12\x18\n\x10timestamp_device\x18\x05 \x01(\x01\x12\x16\n\x0etimestamp_recv\x18\x06 \x01(\x01\"x\n\x0cOakImuPacket\x12/\n\x0bgyro_packet\x18\x01 \x01(\x0b\x32\x1a.farm_ng.oak.proto.OakGyro\x12\x37\n\x0f\x61\x63\x63\x65lero_packet\x18\x02 \x01(\x0b\x32\x1e.farm_ng.oak.proto.OakAccelero\"A\n\rOakImuPackets\x12\x30\n\x07packets\x18\x01 \x03(\x0b\x32\x1f.farm_ng.oak.proto.OakImuPacket\"\x87\x01\n\x17OakTrackedFeaturePacket\x12\'\n\x02xy\x18\x01 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec2F32\x12\n\n\x02id\x18\x02 \x01(\x05\x12\x0b\n\x03\x61ge\x18\x03 \x01(\x05\x12\x13\n\x0bharrisScore\x18\x04 \x01(\x02\x12\x15\n\rtrackingError\x18\x05 \x01(\x02\"\xb2\x01\n\x18OakTrackedFeaturePackets\x12;\n\x07packets\x18\x01 \x03(\x0b\x32*.farm_ng.oak.proto.OakTrackedFeaturePacket\x12\x14\n\x0csequence_num\x18\x02 \x01(\x03\x12\x11\n\ttimestamp\x18\x03 \x01(\x01\x12\x18\n\x10timestamp_device\x18\x04 \x01(\x01\x12\x16\n\x0etimestamp_recv\x18\x05 \x01(\x01\"7\n\rOakDeviceInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04mxid\x18\x02 \x01(\t\x12\n\n\x02ip\x18\x03 \x01(\t\"\xed\x02\n\x0cOakSyncFrame\x12)\n\x04left\x18\x01 \x01(\x0b\x32\x1b.farm_ng.oak.proto.OakFrame\x12*\n\x05right\x18\x02 \x01(\x0b\x32\x1b.farm_ng.oak.proto.OakFrame\x12(\n\x03rgb\x18\x03 \x01(\x0b\x32\x1b.farm_ng.oak.proto.OakFrame\x12.\n\tdisparity\x18\x04 \x01(\x0b\x32\x1b.farm_ng.oak.proto.OakFrame\x12(\n\x02nn\x18\x05 \x01(\x0b\x32\x1c.farm_ng.oak.proto.OakNNData\x12\x35\n\x0bimu_packets\x18\x06 \x01(\x0b\x32 .farm_ng.oak.proto.OakImuPackets\x12\x14\n\x0csequence_num\x18\x07 \x01(\x03\x12\x35\n\x0b\x64\x65vice_info\x18\x08 \x01(\x0b\x32 .farm_ng.oak.proto.OakDeviceInfo\"}\n\tOakNNData\x12-\n\x04meta\x18\x01 \x01(\x0b\x32\x1f.farm_ng.oak.proto.OakImageMeta\x12\x14\n\x0cnum_channels\x18\x02 \x01(\r\x12\x0e\n\x06height\x18\x03 \x01(\r\x12\r\n\x05width\x18\x04 \x01(\r\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\"\"\n\x04Pair\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"2\n\x08Metadata\x12&\n\x05pairs\x18\x01 \x03(\x0b\x32\x17.farm_ng.oak.proto.Pair\"n\n\rOakDataSample\x12.\n\x05\x66rame\x18\x01 \x01(\x0b\x32\x1f.farm_ng.oak.proto.OakSyncFrame\x12-\n\x08metadata\x18\x02 \x01(\x0b\x32\x1b.farm_ng.oak.proto.Metadata\")\n\x0eRotationMatrix\x12\x17\n\x0frotation_matrix\x18\x01 \x03(\x01\"\xa8\x01\n\nExtrinsics\x12\x17\n\x0frotation_matrix\x18\x01 \x03(\x01\x12\x35\n\x10spec_translation\x18\x02 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F32\x12\x18\n\x10to_camera_socket\x18\x03 \x01(\x05\x12\x30\n\x0btranslation\x18\x04 \x01(\x0b\x32\x1b.farm_ng.core.proto.Vec3F32\"\xec\x01\n\nCameraData\x12\x15\n\rcamera_number\x18\x01 \x01(\r\x12\x13\n\x0b\x63\x61mera_type\x18\x02 \x01(\x05\x12\x18\n\x10\x64istortion_coeff\x18\x03 \x03(\x01\x12\x31\n\nextrinsics\x18\x04 \x01(\x0b\x32\x1d.farm_ng.oak.proto.Extrinsics\x12\x0e\n\x06height\x18\x05 \x01(\r\x12\x18\n\x10intrinsic_matrix\x18\x06 \x03(\x01\x12\x15\n\rlens_position\x18\x07 \x01(\r\x12\x15\n\rspec_hfov_deg\x18\x08 \x01(\x01\x12\r\n\x05width\x18\t \x01(\r\"\x95\x01\n\x17StereoRectificationData\x12\x1a\n\x12left_camera_socket\x18\x01 \x01(\r\x12\x1f\n\x17rectified_rotation_left\x18\x02 \x03(\x01\x12 \n\x18rectified_rotation_right\x18\x03 \x03(\x01\x12\x1b\n\x13right_camera_socket\x18\x04 \x01(\r\"\xb4\x03\n\x0eOakCalibration\x12\x12\n\nbatch_name\x18\x01 \x01(\t\x12\x12\n\nbatch_time\x18\x02 \x01(\x05\x12\x12\n\nboard_conf\x18\x03 \x01(\t\x12\x14\n\x0c\x62oard_custom\x18\x04 \x01(\t\x12\x12\n\nboard_name\x18\x05 \x01(\t\x12\x15\n\rboard_options\x18\x06 \x01(\x05\x12\x11\n\tboard_rev\x18\x07 \x01(\t\x12\x32\n\x0b\x63\x61mera_data\x18\x08 \x03(\x0b\x32\x1d.farm_ng.oak.proto.CameraData\x12\x15\n\rhardware_conf\x18\t \x01(\t\x12\x35\n\x0eimu_extrinsics\x18\n \x01(\x0b\x32\x1d.farm_ng.oak.proto.Extrinsics\x12\x1a\n\x12miscellaneous_data\x18\x0b \x03(\t\x12\x14\n\x0cproduct_name\x18\x0c \x01(\t\x12M\n\x19stereo_rectification_data\x18\r \x01(\x0b\x32*.farm_ng.oak.proto.StereoRectificationData\x12\x0f\n\x07version\x18\x0e \x01(\r*[\n\x0e\x45ncoderProfile\x12\x11\n\rH264_BASELINE\x10\x00\x12\r\n\tH264_HIGH\x10\x01\x12\r\n\tH264_MAIN\x10\x02\x12\r\n\tH265_MAIN\x10\x03\x12\t\n\x05MJPEG\x10\x04*#\n\x0fRateControlMode\x12\x07\n\x03\x43\x42R\x10\x00\x12\x07\n\x03VBR\x10\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.oak.oak_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
+  _globals['_ENCODERPROFILE']._serialized_start=3381
+  _globals['_ENCODERPROFILE']._serialized_end=3472
+  _globals['_RATECONTROLMODE']._serialized_start=3474
+  _globals['_RATECONTROLMODE']._serialized_end=3509
   _globals['_CAMERASETTINGS']._serialized_start=71
   _globals['_CAMERASETTINGS']._serialized_end=170
-  _globals['_OAKIMAGEMETA']._serialized_start=173
-  _globals['_OAKIMAGEMETA']._serialized_end=371
-  _globals['_OAKFRAME']._serialized_start=373
-  _globals['_OAKFRAME']._serialized_end=450
-  _globals['_OAKGYRO']._serialized_start=453
-  _globals['_OAKGYRO']._serialized_end=614
-  _globals['_OAKACCELERO']._serialized_start=617
-  _globals['_OAKACCELERO']._serialized_end=786
-  _globals['_OAKIMUPACKET']._serialized_start=788
-  _globals['_OAKIMUPACKET']._serialized_end=908
-  _globals['_OAKIMUPACKETS']._serialized_start=910
-  _globals['_OAKIMUPACKETS']._serialized_end=975
-  _globals['_OAKDEVICEINFO']._serialized_start=977
-  _globals['_OAKDEVICEINFO']._serialized_end=1032
-  _globals['_OAKSYNCFRAME']._serialized_start=1035
-  _globals['_OAKSYNCFRAME']._serialized_end=1400
-  _globals['_OAKNNDATA']._serialized_start=1402
-  _globals['_OAKNNDATA']._serialized_end=1527
-  _globals['_PAIR']._serialized_start=1529
-  _globals['_PAIR']._serialized_end=1563
-  _globals['_METADATA']._serialized_start=1565
-  _globals['_METADATA']._serialized_end=1615
-  _globals['_OAKDATASAMPLE']._serialized_start=1617
-  _globals['_OAKDATASAMPLE']._serialized_end=1727
-  _globals['_ROTATIONMATRIX']._serialized_start=1729
-  _globals['_ROTATIONMATRIX']._serialized_end=1770
-  _globals['_EXTRINSICS']._serialized_start=1773
-  _globals['_EXTRINSICS']._serialized_end=1941
-  _globals['_CAMERADATA']._serialized_start=1944
-  _globals['_CAMERADATA']._serialized_end=2180
-  _globals['_STEREORECTIFICATIONDATA']._serialized_start=2183
-  _globals['_STEREORECTIFICATIONDATA']._serialized_end=2332
-  _globals['_OAKCALIBRATION']._serialized_start=2335
-  _globals['_OAKCALIBRATION']._serialized_end=2771
+  _globals['_ENCODEROPTIONS']._serialized_start=173
+  _globals['_ENCODEROPTIONS']._serialized_end=399
+  _globals['_OAKIMAGEMETA']._serialized_start=402
+  _globals['_OAKIMAGEMETA']._serialized_end=660
+  _globals['_OAKFRAME']._serialized_start=662
+  _globals['_OAKFRAME']._serialized_end=739
+  _globals['_OAKGYRO']._serialized_start=742
+  _globals['_OAKGYRO']._serialized_end=903
+  _globals['_OAKACCELERO']._serialized_start=906
+  _globals['_OAKACCELERO']._serialized_end=1075
+  _globals['_OAKIMUPACKET']._serialized_start=1077
+  _globals['_OAKIMUPACKET']._serialized_end=1197
+  _globals['_OAKIMUPACKETS']._serialized_start=1199
+  _globals['_OAKIMUPACKETS']._serialized_end=1264
+  _globals['_OAKTRACKEDFEATUREPACKET']._serialized_start=1267
+  _globals['_OAKTRACKEDFEATUREPACKET']._serialized_end=1402
+  _globals['_OAKTRACKEDFEATUREPACKETS']._serialized_start=1405
+  _globals['_OAKTRACKEDFEATUREPACKETS']._serialized_end=1583
+  _globals['_OAKDEVICEINFO']._serialized_start=1585
+  _globals['_OAKDEVICEINFO']._serialized_end=1640
+  _globals['_OAKSYNCFRAME']._serialized_start=1643
+  _globals['_OAKSYNCFRAME']._serialized_end=2008
+  _globals['_OAKNNDATA']._serialized_start=2010
+  _globals['_OAKNNDATA']._serialized_end=2135
+  _globals['_PAIR']._serialized_start=2137
+  _globals['_PAIR']._serialized_end=2171
+  _globals['_METADATA']._serialized_start=2173
+  _globals['_METADATA']._serialized_end=2223
+  _globals['_OAKDATASAMPLE']._serialized_start=2225
+  _globals['_OAKDATASAMPLE']._serialized_end=2335
+  _globals['_ROTATIONMATRIX']._serialized_start=2337
+  _globals['_ROTATIONMATRIX']._serialized_end=2378
+  _globals['_EXTRINSICS']._serialized_start=2381
+  _globals['_EXTRINSICS']._serialized_end=2549
+  _globals['_CAMERADATA']._serialized_start=2552
+  _globals['_CAMERADATA']._serialized_end=2788
+  _globals['_STEREORECTIFICATIONDATA']._serialized_start=2791
+  _globals['_STEREORECTIFICATIONDATA']._serialized_end=2940
+  _globals['_OAKCALIBRATION']._serialized_start=2943
+  _globals['_OAKCALIBRATION']._serialized_end=3379
 # @@protoc_insertion_point(module_scope)
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/oak/oak_pb2.pyi` & `farm_ng_amiga-2.3.0/py/farm_ng/oak/oak_pb2.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,81 @@
 from farm_ng.core import linalg_pb2 as _linalg_pb2
 from google.protobuf.internal import containers as _containers
+from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
+class EncoderProfile(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = ()
+    H264_BASELINE: _ClassVar[EncoderProfile]
+    H264_HIGH: _ClassVar[EncoderProfile]
+    H264_MAIN: _ClassVar[EncoderProfile]
+    H265_MAIN: _ClassVar[EncoderProfile]
+    MJPEG: _ClassVar[EncoderProfile]
+
+class RateControlMode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = ()
+    CBR: _ClassVar[RateControlMode]
+    VBR: _ClassVar[RateControlMode]
+H264_BASELINE: EncoderProfile
+H264_HIGH: EncoderProfile
+H264_MAIN: EncoderProfile
+H265_MAIN: EncoderProfile
+MJPEG: EncoderProfile
+CBR: RateControlMode
+VBR: RateControlMode
+
 class CameraSettings(_message.Message):
     __slots__ = ("auto_exposure", "exposure_time", "iso_value", "lens_pos")
     AUTO_EXPOSURE_FIELD_NUMBER: _ClassVar[int]
     EXPOSURE_TIME_FIELD_NUMBER: _ClassVar[int]
     ISO_VALUE_FIELD_NUMBER: _ClassVar[int]
     LENS_POS_FIELD_NUMBER: _ClassVar[int]
     auto_exposure: bool
     exposure_time: int
     iso_value: int
     lens_pos: int
     def __init__(self, auto_exposure: bool = ..., exposure_time: _Optional[int] = ..., iso_value: _Optional[int] = ..., lens_pos: _Optional[int] = ...) -> None: ...
 
+class EncoderOptions(_message.Message):
+    __slots__ = ("profile", "rate_control_mode", "cbr_preferred_bitrate_kbps", "vbr_or_mjpeg_quality", "frames_per_keyframe")
+    PROFILE_FIELD_NUMBER: _ClassVar[int]
+    RATE_CONTROL_MODE_FIELD_NUMBER: _ClassVar[int]
+    CBR_PREFERRED_BITRATE_KBPS_FIELD_NUMBER: _ClassVar[int]
+    VBR_OR_MJPEG_QUALITY_FIELD_NUMBER: _ClassVar[int]
+    FRAMES_PER_KEYFRAME_FIELD_NUMBER: _ClassVar[int]
+    profile: EncoderProfile
+    rate_control_mode: RateControlMode
+    cbr_preferred_bitrate_kbps: int
+    vbr_or_mjpeg_quality: int
+    frames_per_keyframe: int
+    def __init__(self, profile: _Optional[_Union[EncoderProfile, str]] = ..., rate_control_mode: _Optional[_Union[RateControlMode, str]] = ..., cbr_preferred_bitrate_kbps: _Optional[int] = ..., vbr_or_mjpeg_quality: _Optional[int] = ..., frames_per_keyframe: _Optional[int] = ...) -> None: ...
+
 class OakImageMeta(_message.Message):
-    __slots__ = ("category", "instance_num", "sequence_num", "timestamp", "timestamp_device", "timestamp_recv", "settings")
+    __slots__ = ("category", "instance_num", "sequence_num", "timestamp", "timestamp_device", "timestamp_recv", "settings", "encoder_options")
     CATEGORY_FIELD_NUMBER: _ClassVar[int]
     INSTANCE_NUM_FIELD_NUMBER: _ClassVar[int]
     SEQUENCE_NUM_FIELD_NUMBER: _ClassVar[int]
     TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
     TIMESTAMP_DEVICE_FIELD_NUMBER: _ClassVar[int]
     TIMESTAMP_RECV_FIELD_NUMBER: _ClassVar[int]
     SETTINGS_FIELD_NUMBER: _ClassVar[int]
+    ENCODER_OPTIONS_FIELD_NUMBER: _ClassVar[int]
     category: int
     instance_num: int
     sequence_num: int
     timestamp: float
     timestamp_device: float
     timestamp_recv: float
     settings: CameraSettings
-    def __init__(self, category: _Optional[int] = ..., instance_num: _Optional[int] = ..., sequence_num: _Optional[int] = ..., timestamp: _Optional[float] = ..., timestamp_device: _Optional[float] = ..., timestamp_recv: _Optional[float] = ..., settings: _Optional[_Union[CameraSettings, _Mapping]] = ...) -> None: ...
+    encoder_options: EncoderOptions
+    def __init__(self, category: _Optional[int] = ..., instance_num: _Optional[int] = ..., sequence_num: _Optional[int] = ..., timestamp: _Optional[float] = ..., timestamp_device: _Optional[float] = ..., timestamp_recv: _Optional[float] = ..., settings: _Optional[_Union[CameraSettings, _Mapping]] = ..., encoder_options: _Optional[_Union[EncoderOptions, _Mapping]] = ...) -> None: ...
 
 class OakFrame(_message.Message):
     __slots__ = ("meta", "image_data")
     META_FIELD_NUMBER: _ClassVar[int]
     IMAGE_DATA_FIELD_NUMBER: _ClassVar[int]
     meta: OakImageMeta
     image_data: bytes
@@ -86,14 +123,42 @@
 
 class OakImuPackets(_message.Message):
     __slots__ = ("packets",)
     PACKETS_FIELD_NUMBER: _ClassVar[int]
     packets: _containers.RepeatedCompositeFieldContainer[OakImuPacket]
     def __init__(self, packets: _Optional[_Iterable[_Union[OakImuPacket, _Mapping]]] = ...) -> None: ...
 
+class OakTrackedFeaturePacket(_message.Message):
+    __slots__ = ("xy", "id", "age", "harrisScore", "trackingError")
+    XY_FIELD_NUMBER: _ClassVar[int]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    AGE_FIELD_NUMBER: _ClassVar[int]
+    HARRISSCORE_FIELD_NUMBER: _ClassVar[int]
+    TRACKINGERROR_FIELD_NUMBER: _ClassVar[int]
+    xy: _linalg_pb2.Vec2F32
+    id: int
+    age: int
+    harrisScore: float
+    trackingError: float
+    def __init__(self, xy: _Optional[_Union[_linalg_pb2.Vec2F32, _Mapping]] = ..., id: _Optional[int] = ..., age: _Optional[int] = ..., harrisScore: _Optional[float] = ..., trackingError: _Optional[float] = ...) -> None: ...
+
+class OakTrackedFeaturePackets(_message.Message):
+    __slots__ = ("packets", "sequence_num", "timestamp", "timestamp_device", "timestamp_recv")
+    PACKETS_FIELD_NUMBER: _ClassVar[int]
+    SEQUENCE_NUM_FIELD_NUMBER: _ClassVar[int]
+    TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
+    TIMESTAMP_DEVICE_FIELD_NUMBER: _ClassVar[int]
+    TIMESTAMP_RECV_FIELD_NUMBER: _ClassVar[int]
+    packets: _containers.RepeatedCompositeFieldContainer[OakTrackedFeaturePacket]
+    sequence_num: int
+    timestamp: float
+    timestamp_device: float
+    timestamp_recv: float
+    def __init__(self, packets: _Optional[_Iterable[_Union[OakTrackedFeaturePacket, _Mapping]]] = ..., sequence_num: _Optional[int] = ..., timestamp: _Optional[float] = ..., timestamp_device: _Optional[float] = ..., timestamp_recv: _Optional[float] = ...) -> None: ...
+
 class OakDeviceInfo(_message.Message):
     __slots__ = ("name", "mxid", "ip")
     NAME_FIELD_NUMBER: _ClassVar[int]
     MXID_FIELD_NUMBER: _ClassVar[int]
     IP_FIELD_NUMBER: _ClassVar[int]
     name: str
     mxid: str
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/track/__init__.py` & `farm_ng_amiga-2.3.0/py/farm_ng/track/__init__.py`

 * *Files identical despite different names*

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/track/track.proto` & `farm_ng_amiga-2.3.0/py/farm_ng/track/track.proto`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,16 @@
   // Following the track completed successfully
   TRACK_COMPLETE = 5;
   // Following the track failed (e.g., deviated too far from the track)
   TRACK_FAILED = 6;
   // Following the track was aborted (e.g., ability to control was lost)
   // See RobotStatus for more details
   TRACK_ABORTED = 7;
+  // Following the track was cancelled (e.g., user requested)
+  TRACK_CANCELLED = 8;
 }
 
 // Message representing the status of a robot's controlability
 message RobotStatus {
   enum FailureMode {
     // Failure mode is unknown
     FAILURE_UNSPECIFIED = 0;
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/track/track_pb2.py` & `farm_ng_amiga-2.3.0/py/farm_ng/track/track_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: farm_ng/track/track.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from farm_ng.core import lie_pb2 as farm__ng_dot_core_dot_lie__pb2
 from farm_ng.core import pose_pb2 as farm__ng_dot_core_dot_pose__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x66\x61rm_ng/track/track.proto\x12\x13\x66\x61rm_ng.track.proto\x1a\x16\x66\x61rm_ng/core/lie.proto\x1a\x17\x66\x61rm_ng/core/pose.proto\"4\n\x05Track\x12+\n\twaypoints\x18\x01 \x03(\x0b\x32\x18.farm_ng.core.proto.Pose\"\x81\x01\n\x12TrackFollowRequest\x12)\n\x05track\x18\x01 \x01(\x0b\x32\x1a.farm_ng.track.proto.Track\x12@\n\x11\x64riving_direction\x18\x02 \x01(\x0e\x32%.farm_ng.track.proto.DrivingDirection\"\x82\x02\n\x12TrackFollowerState\x12\x38\n\x06status\x18\x01 \x01(\x0b\x32(.farm_ng.track.proto.TrackFollowerStatus\x12<\n\x08progress\x18\x02 \x01(\x0b\x32*.farm_ng.track.proto.TrackFollowerProgress\x12\x39\n\x05poses\x18\x03 \x01(\x0b\x32*.farm_ng.track.proto.TrackFollowerPoseTree\x12\x39\n\x08\x63ommands\x18\x04 \x01(\x0b\x32\'.farm_ng.core.proto.Isometry3F64Tangent\"\x87\x02\n\x13TrackFollowerStatus\x12:\n\x0ctrack_status\x18\x01 \x01(\x0e\x32$.farm_ng.track.proto.TrackStatusEnum\x12\x36\n\x0crobot_status\x18\x02 \x01(\x0b\x32 .farm_ng.track.proto.RobotStatus\x12@\n\x11\x64riving_direction\x18\x03 \x01(\x0e\x32%.farm_ng.track.proto.DrivingDirection\x12:\n\x0ewaypoint_order\x18\x04 \x01(\x0e\x32\".farm_ng.track.proto.WaypointOrder\"\xfd\x01\n\x0bRobotStatus\x12\x14\n\x0c\x63ontrollable\x18\x01 \x01(\x08\x12\x43\n\rfailure_modes\x18\x02 \x03(\x0e\x32,.farm_ng.track.proto.RobotStatus.FailureMode\"\x92\x01\n\x0b\x46\x61ilureMode\x12\x17\n\x13\x46\x41ILURE_UNSPECIFIED\x10\x00\x12\x12\n\x0e\x43\x41NBUS_TIMEOUT\x10\n\x12\x16\n\x12\x41UTO_MODE_DISABLED\x10\x0b\x12\x15\n\x11\x43\x41NBUS_SEND_ERROR\x10\x0c\x12\x12\n\x0e\x46ILTER_TIMEOUT\x10\x14\x12\x13\n\x0f\x46ILTER_DIVERGED\x10\x15\"\xd0\x01\n\x15TrackFollowerProgress\x12\x12\n\ntrack_size\x18\x01 \x01(\x05\x12\x1b\n\x13goal_waypoint_index\x18\x02 \x01(\x05\x12\x1e\n\x16\x63losest_waypoint_index\x18\x03 \x01(\x05\x12\x16\n\x0e\x64istance_total\x18\x04 \x01(\x01\x12\x1a\n\x12\x64istance_remaining\x18\x05 \x01(\x01\x12\x16\n\x0e\x64uration_total\x18\x06 \x01(\x01\x12\x1a\n\x12\x64uration_remaining\x18\x07 \x01(\x01\"\xbd\x01\n\x15TrackFollowerPoseTree\x12\x32\n\x10world_from_robot\x18\x01 \x01(\x0b\x32\x18.farm_ng.core.proto.Pose\x12\x31\n\x0frobot_from_goal\x18\x02 \x01(\x0b\x32\x18.farm_ng.core.proto.Pose\x12=\n\x1brobot_from_closest_waypoint\x18\x03 \x01(\x0b\x32\x18.farm_ng.core.proto.Pose*[\n\x10\x44rivingDirection\x12\x19\n\x15\x44IRECTION_UNSPECIFIED\x10\x00\x12\x15\n\x11\x44IRECTION_FORWARD\x10\x01\x12\x15\n\x11\x44IRECTION_REVERSE\x10\x02*N\n\rWaypointOrder\x12\x15\n\x11ORDER_UNSPECIFIED\x10\x00\x12\x12\n\x0eORDER_STANDARD\x10\x01\x12\x12\n\x0eORDER_REVERSED\x10\x02*\xab\x01\n\x0fTrackStatusEnum\x12\x15\n\x11TRACK_UNSPECIFIED\x10\x00\x12\x0f\n\x0bTRACK_EMPTY\x10\x01\x12\x10\n\x0cTRACK_LOADED\x10\x02\x12\x13\n\x0fTRACK_FOLLOWING\x10\x03\x12\x10\n\x0cTRACK_PAUSED\x10\x04\x12\x12\n\x0eTRACK_COMPLETE\x10\x05\x12\x10\n\x0cTRACK_FAILED\x10\x06\x12\x11\n\rTRACK_ABORTED\x10\x07\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x66\x61rm_ng/track/track.proto\x12\x13\x66\x61rm_ng.track.proto\x1a\x16\x66\x61rm_ng/core/lie.proto\x1a\x17\x66\x61rm_ng/core/pose.proto\"4\n\x05Track\x12+\n\twaypoints\x18\x01 \x03(\x0b\x32\x18.farm_ng.core.proto.Pose\"\x81\x01\n\x12TrackFollowRequest\x12)\n\x05track\x18\x01 \x01(\x0b\x32\x1a.farm_ng.track.proto.Track\x12@\n\x11\x64riving_direction\x18\x02 \x01(\x0e\x32%.farm_ng.track.proto.DrivingDirection\"\x82\x02\n\x12TrackFollowerState\x12\x38\n\x06status\x18\x01 \x01(\x0b\x32(.farm_ng.track.proto.TrackFollowerStatus\x12<\n\x08progress\x18\x02 \x01(\x0b\x32*.farm_ng.track.proto.TrackFollowerProgress\x12\x39\n\x05poses\x18\x03 \x01(\x0b\x32*.farm_ng.track.proto.TrackFollowerPoseTree\x12\x39\n\x08\x63ommands\x18\x04 \x01(\x0b\x32\'.farm_ng.core.proto.Isometry3F64Tangent\"\x87\x02\n\x13TrackFollowerStatus\x12:\n\x0ctrack_status\x18\x01 \x01(\x0e\x32$.farm_ng.track.proto.TrackStatusEnum\x12\x36\n\x0crobot_status\x18\x02 \x01(\x0b\x32 .farm_ng.track.proto.RobotStatus\x12@\n\x11\x64riving_direction\x18\x03 \x01(\x0e\x32%.farm_ng.track.proto.DrivingDirection\x12:\n\x0ewaypoint_order\x18\x04 \x01(\x0e\x32\".farm_ng.track.proto.WaypointOrder\"\xfd\x01\n\x0bRobotStatus\x12\x14\n\x0c\x63ontrollable\x18\x01 \x01(\x08\x12\x43\n\rfailure_modes\x18\x02 \x03(\x0e\x32,.farm_ng.track.proto.RobotStatus.FailureMode\"\x92\x01\n\x0b\x46\x61ilureMode\x12\x17\n\x13\x46\x41ILURE_UNSPECIFIED\x10\x00\x12\x12\n\x0e\x43\x41NBUS_TIMEOUT\x10\n\x12\x16\n\x12\x41UTO_MODE_DISABLED\x10\x0b\x12\x15\n\x11\x43\x41NBUS_SEND_ERROR\x10\x0c\x12\x12\n\x0e\x46ILTER_TIMEOUT\x10\x14\x12\x13\n\x0f\x46ILTER_DIVERGED\x10\x15\"\xd0\x01\n\x15TrackFollowerProgress\x12\x12\n\ntrack_size\x18\x01 \x01(\x05\x12\x1b\n\x13goal_waypoint_index\x18\x02 \x01(\x05\x12\x1e\n\x16\x63losest_waypoint_index\x18\x03 \x01(\x05\x12\x16\n\x0e\x64istance_total\x18\x04 \x01(\x01\x12\x1a\n\x12\x64istance_remaining\x18\x05 \x01(\x01\x12\x16\n\x0e\x64uration_total\x18\x06 \x01(\x01\x12\x1a\n\x12\x64uration_remaining\x18\x07 \x01(\x01\"\xbd\x01\n\x15TrackFollowerPoseTree\x12\x32\n\x10world_from_robot\x18\x01 \x01(\x0b\x32\x18.farm_ng.core.proto.Pose\x12\x31\n\x0frobot_from_goal\x18\x02 \x01(\x0b\x32\x18.farm_ng.core.proto.Pose\x12=\n\x1brobot_from_closest_waypoint\x18\x03 \x01(\x0b\x32\x18.farm_ng.core.proto.Pose*[\n\x10\x44rivingDirection\x12\x19\n\x15\x44IRECTION_UNSPECIFIED\x10\x00\x12\x15\n\x11\x44IRECTION_FORWARD\x10\x01\x12\x15\n\x11\x44IRECTION_REVERSE\x10\x02*N\n\rWaypointOrder\x12\x15\n\x11ORDER_UNSPECIFIED\x10\x00\x12\x12\n\x0eORDER_STANDARD\x10\x01\x12\x12\n\x0eORDER_REVERSED\x10\x02*\xc0\x01\n\x0fTrackStatusEnum\x12\x15\n\x11TRACK_UNSPECIFIED\x10\x00\x12\x0f\n\x0bTRACK_EMPTY\x10\x01\x12\x10\n\x0cTRACK_LOADED\x10\x02\x12\x13\n\x0fTRACK_FOLLOWING\x10\x03\x12\x10\n\x0cTRACK_PAUSED\x10\x04\x12\x12\n\x0eTRACK_COMPLETE\x10\x05\x12\x10\n\x0cTRACK_FAILED\x10\x06\x12\x11\n\rTRACK_ABORTED\x10\x07\x12\x13\n\x0fTRACK_CANCELLED\x10\x08\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'farm_ng.track.track_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_DRIVINGDIRECTION']._serialized_start=1471
   _globals['_DRIVINGDIRECTION']._serialized_end=1562
   _globals['_WAYPOINTORDER']._serialized_start=1564
   _globals['_WAYPOINTORDER']._serialized_end=1642
   _globals['_TRACKSTATUSENUM']._serialized_start=1645
-  _globals['_TRACKSTATUSENUM']._serialized_end=1816
+  _globals['_TRACKSTATUSENUM']._serialized_end=1837
   _globals['_TRACK']._serialized_start=99
   _globals['_TRACK']._serialized_end=151
   _globals['_TRACKFOLLOWREQUEST']._serialized_start=154
   _globals['_TRACKFOLLOWREQUEST']._serialized_end=283
   _globals['_TRACKFOLLOWERSTATE']._serialized_start=286
   _globals['_TRACKFOLLOWERSTATE']._serialized_end=544
   _globals['_TRACKFOLLOWERSTATUS']._serialized_start=547
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/track/track_pb2.pyi` & `farm_ng_amiga-2.3.0/py/farm_ng/track/track_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -26,28 +26,30 @@
     TRACK_EMPTY: _ClassVar[TrackStatusEnum]
     TRACK_LOADED: _ClassVar[TrackStatusEnum]
     TRACK_FOLLOWING: _ClassVar[TrackStatusEnum]
     TRACK_PAUSED: _ClassVar[TrackStatusEnum]
     TRACK_COMPLETE: _ClassVar[TrackStatusEnum]
     TRACK_FAILED: _ClassVar[TrackStatusEnum]
     TRACK_ABORTED: _ClassVar[TrackStatusEnum]
+    TRACK_CANCELLED: _ClassVar[TrackStatusEnum]
 DIRECTION_UNSPECIFIED: DrivingDirection
 DIRECTION_FORWARD: DrivingDirection
 DIRECTION_REVERSE: DrivingDirection
 ORDER_UNSPECIFIED: WaypointOrder
 ORDER_STANDARD: WaypointOrder
 ORDER_REVERSED: WaypointOrder
 TRACK_UNSPECIFIED: TrackStatusEnum
 TRACK_EMPTY: TrackStatusEnum
 TRACK_LOADED: TrackStatusEnum
 TRACK_FOLLOWING: TrackStatusEnum
 TRACK_PAUSED: TrackStatusEnum
 TRACK_COMPLETE: TrackStatusEnum
 TRACK_FAILED: TrackStatusEnum
 TRACK_ABORTED: TrackStatusEnum
+TRACK_CANCELLED: TrackStatusEnum
 
 class Track(_message.Message):
     __slots__ = ("waypoints",)
     WAYPOINTS_FIELD_NUMBER: _ClassVar[int]
     waypoints: _containers.RepeatedCompositeFieldContainer[_pose_pb2.Pose]
     def __init__(self, waypoints: _Optional[_Iterable[_Union[_pose_pb2.Pose, _Mapping]]] = ...) -> None: ...
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng/track/utils.py` & `farm_ng_amiga-2.3.0/py/farm_ng/track/utils.py`

 * *Files identical despite different names*

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng_amiga.egg-info/PKG-INFO` & `farm_ng_amiga-2.3.0/py/farm_ng_amiga.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: farm_ng_amiga
-Version: 2.2.0
+Version: 2.3.0
 Summary: Amiga development kit for third party hardware or software extensions
 Home-page: https://github.com/farm-ng/farm-ng-amiga
 Download-URL: https://github.com/farm-ng/farm-ng-amiga
 Author: farm-ng Inc.
 Author-email: info@farm-ng.com
 Keywords: robotics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `farm_ng_amiga-2.2.0/py/farm_ng_amiga.egg-info/SOURCES.txt` & `farm_ng_amiga-2.3.0/py/farm_ng_amiga.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 py/farm_ng/canbus/amiga_v6_pb2.pyi
 py/farm_ng/canbus/amiga_v6_pb2_grpc.py
 py/farm_ng/canbus/canbus.proto
 py/farm_ng/canbus/canbus_pb2.py
 py/farm_ng/canbus/canbus_pb2.pyi
 py/farm_ng/canbus/canbus_pb2_grpc.py
 py/farm_ng/canbus/packet.py
+py/farm_ng/canbus/tool_control.proto
+py/farm_ng/canbus/tool_control_pb2.py
+py/farm_ng/canbus/tool_control_pb2.pyi
+py/farm_ng/canbus/tool_control_pb2_grpc.py
 py/farm_ng/filter/__init__.py
 py/farm_ng/filter/filter.proto
 py/farm_ng/filter/filter_pb2.py
 py/farm_ng/filter/filter_pb2.pyi
 py/farm_ng/filter/filter_pb2_grpc.py
 py/farm_ng/gps/__init__.py
 py/farm_ng/gps/gps.proto
```

### Comparing `farm_ng_amiga-2.2.0/setup.cfg` & `farm_ng_amiga-2.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = farm_ng_amiga
-version = 2.2.0
+version = 2.3.0
 description = Amiga development kit for third party hardware or software extensions
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = farm-ng Inc.
 author_email = info@farm-ng.com
 url = https://github.com/farm-ng/farm-ng-amiga
 download_url = https://github.com/farm-ng/farm-ng-amiga
```

### Comparing `farm_ng_amiga-2.2.0/setup.py` & `farm_ng_amiga-2.3.0/setup.py`

 * *Files identical despite different names*

