# Comparing `tmp/caraml-store-0.1.6.tar.gz` & `tmp/caraml-store-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/caraml-store-0.1.6.tar", last modified: Tue Nov 21 04:06:37 2023, max compression
+gzip compressed data, was "dist/caraml-store-0.1.7.tar", last modified: Fri May 17 03:16:06 2024, max compression
```

## Comparing `caraml-store-0.1.6.tar` & `caraml-store-0.1.7.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:37.000000 caraml-store-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-11-21 04:06:37.000000 caraml-store-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:27.000000 caraml-store-0.1.6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:37.000000 caraml-store-0.1.6/caraml_store.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-11-21 04:06:37.000000 caraml-store-0.1.6/caraml_store.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-11-21 04:06:37.000000 caraml-store-0.1.6/caraml_store.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 04:06:37.000000 caraml-store-0.1.6/caraml_store.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-21 04:06:37.000000 caraml-store-0.1.6/caraml_store.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-21 04:06:37.000000 caraml-store-0.1.6/caraml_store.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:37.000000 caraml-store-0.1.6/feast/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14160 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:37.000000 caraml-store-0.1.6/feast/core/
--rw-r--r--   0 runner    (1001) docker     (127)    12810 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/CoreService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/CoreService_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    30397 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/CoreService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/DataFormat_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/DataFormat_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/DataFormat_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/DataSource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/DataSource_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/DataSource_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/Entity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/Entity_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/Entity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/FeatureTable_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/FeatureTable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/FeatureTable_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/Feature_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/Feature_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/Feature_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/OnlineStore_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/OnlineStore_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/OnlineStore_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/SparkOverride_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/SparkOverride_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/SparkOverride_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/data_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    10381 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    12703 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/feature_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:37.000000 caraml-store-0.1.6/feast/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/gcp/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:37.000000 caraml-store-0.1.6/feast/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/loaders/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/online_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/online_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:37.000000 caraml-store-0.1.6/feast/serving/
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/serving/ServingService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/serving/ServingService_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/serving/ServingService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/serving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:37.000000 caraml-store-0.1.6/feast/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/types/Field_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/types/Field_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/types/Field_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/types/Value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/types/Value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/types/Value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast/value_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:37.000000 caraml-store-0.1.6/feast_spark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast_spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:37.000000 caraml-store-0.1.6/feast_spark/api/
--rw-r--r--   0 runner    (1001) docker     (127)     8977 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast_spark/api/JobService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9235 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast_spark/api/JobService_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15698 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast_spark/api/JobService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:27.000000 caraml-store-0.1.6/feast_spark/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-21 04:06:27.000000 caraml-store-0.1.6/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-11-21 04:06:27.000000 caraml-store-0.1.6/requirements-ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-21 04:06:37.000000 caraml-store-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2023-11-21 04:06:27.000000 caraml-store-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:37.000000 caraml-store-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:27.000000 caraml-store-0.1.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:37.000000 caraml-store-0.1.6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-11-21 04:06:27.000000 caraml-store-0.1.6/tests/data/test_feature_table.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2023-11-21 04:06:27.000000 caraml-store-0.1.6/tests/test_model_protobuf_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 04:06:37.000000 caraml-store-0.1.6/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)      936 2023-11-21 04:06:27.000000 caraml-store-0.1.6/utils/compile_protos.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:16:06.000000 caraml-store-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-17 03:16:06.000000 caraml-store-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:15:46.000000 caraml-store-0.1.7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:16:06.000000 caraml-store-0.1.7/caraml_store.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-17 03:16:06.000000 caraml-store-0.1.7/caraml_store.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-17 03:16:06.000000 caraml-store-0.1.7/caraml_store.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:16:06.000000 caraml-store-0.1.7/caraml_store.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-17 03:16:06.000000 caraml-store-0.1.7/caraml_store.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 03:16:06.000000 caraml-store-0.1.7/caraml_store.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:16:06.000000 caraml-store-0.1.7/feast/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:16:06.000000 caraml-store-0.1.7/feast/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/CoreService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/CoreService_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    30397 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/CoreService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/DataFormat_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/DataFormat_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/DataFormat_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/DataSource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/DataSource_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/DataSource_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/Entity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/Entity_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/Entity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/FeatureTable_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/FeatureTable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/FeatureTable_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/Feature_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/Feature_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/Feature_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/OnlineStore_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/OnlineStore_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/OnlineStore_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/SparkOverride_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/SparkOverride_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/SparkOverride_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12703 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/feature_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:16:06.000000 caraml-store-0.1.7/feast/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/gcp/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:16:06.000000 caraml-store-0.1.7/feast/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/loaders/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/online_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/online_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:16:06.000000 caraml-store-0.1.7/feast/serving/
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/serving/ServingService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/serving/ServingService_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/serving/ServingService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/serving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:16:06.000000 caraml-store-0.1.7/feast/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/types/Field_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/types/Field_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/types/Field_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/types/Value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/types/Value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/types/Value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast/value_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:16:06.000000 caraml-store-0.1.7/feast_spark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast_spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:16:06.000000 caraml-store-0.1.7/feast_spark/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast_spark/api/JobService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast_spark/api/JobService_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19353 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast_spark/api/JobService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:15:46.000000 caraml-store-0.1.7/feast_spark/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 03:15:46.000000 caraml-store-0.1.7/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-17 03:15:46.000000 caraml-store-0.1.7/requirements-ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:16:06.000000 caraml-store-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-17 03:15:46.000000 caraml-store-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:16:06.000000 caraml-store-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:15:46.000000 caraml-store-0.1.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:16:06.000000 caraml-store-0.1.7/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-17 03:15:46.000000 caraml-store-0.1.7/tests/data/test_feature_table.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-17 03:15:46.000000 caraml-store-0.1.7/tests/test_model_protobuf_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:16:06.000000 caraml-store-0.1.7/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      936 2024-05-17 03:15:46.000000 caraml-store-0.1.7/utils/compile_protos.sh
```

### Comparing `caraml-store-0.1.6/caraml_store.egg-info/SOURCES.txt` & `caraml-store-0.1.7/caraml_store.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/client.py` & `caraml-store-0.1.7/feast/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     StartOfflineToOnlineIngestionJobRequest,
     StartOfflineToOnlineIngestionJobResponse,
     GetHistoricalFeaturesRequest,
     GetHistoricalFeaturesResponse,
     GetJobRequest,
     ListJobsRequest,
     Job,
-    ScheduleOfflineToOnlineIngestionJobRequest,
+    ScheduleOfflineToOnlineIngestionJobRequest, ScheduledJob, ListScheduledJobsRequest, StartStreamIngestionJobResponse,
+    StartStreamIngestionJobRequest, JobType, INVALID_JOB,
 )
 from feast_spark.api.JobService_pb2_grpc import JobServiceStub
 
 
 @dataclass
 class Client:
     registry_url: Optional[str] = None
@@ -288,14 +289,32 @@
         request = StartOfflineToOnlineIngestionJobRequest(
             project=project, table_name=feature_table, delta_ingestion=delta_ingestion
         )
         request.start_date.FromDatetime(start)
         request.end_date.FromDatetime(end)
         return self._job_service.StartOfflineToOnlineIngestionJob(request)
 
+    def start_stream_ingestion(
+        self,
+        feature_table: str,
+        project: str
+    ) -> StartStreamIngestionJobResponse:
+        """
+        Starts or update a stream ingestion job for the given feature table
+        Args:
+            feature_table: feature table name
+            project: Feast project name
+
+        Returns: StartStreamIngestionJobResponse
+        """
+        request = StartStreamIngestionJobRequest(
+            project=project, table_name=feature_table
+        )
+        return self._job_service.StartStreamIngestionJob(request)
+
     def schedule_offline_to_online_ingestion(
         self,
         feature_table: str,
         project: str,
         ingestion_timespan: int,
         cron_schedule: str,
     ):
@@ -368,28 +387,41 @@
 
         Returns: Job protobuf object
         """
         request = GetJobRequest(job_id=job_id)
         response = self._job_service.GetJob(request)
         return response.job
 
-    def list_job(self, table: str, project: str, include_terminated=True) -> List[Job]:
+    def list_job(self, table: str = "", project: str = "", include_terminated=True, job_type: JobType = INVALID_JOB) -> List[Job]:
         """
         List job details
         Args:
+            include_terminated: include terminated jobs
             table: feature table name
             project: feast project name
-            include_terminated: include terminated jobs
+            job_type: job type
 
         Returns: List of Job protobuf object
         """
-        request = ListJobsRequest(table_name=table, project=project, include_terminated=include_terminated)
+        request = ListJobsRequest(table_name=table, project=project, include_terminated=include_terminated, type=job_type)
         response = self._job_service.ListJobs(request)
         return response.jobs
 
+    def list_scheduled_job(self, project = "", table_name = "") -> List[ScheduledJob]:
+        """
+        List scheduled jobs
+        Args:
+            project: Filter by project, if non empty.
+            table_name: Filter by table name, if non empty
+        Returns: List of Scheduled Job protobuf object
+        """
+        request = ListScheduledJobsRequest(project=project, table_name=table_name)
+        response = self._job_service.ListScheduledJob(request)
+        return response.jobs
+
     def delete_feature_table(self, feature_table: str, project: str):
         """
         Delete Feature Table
         Args:
             feature_table: feature table name
             project: project name
         """
```

### Comparing `caraml-store-0.1.6/feast/core/CoreService_pb2.py` & `caraml-store-0.1.7/feast/core/CoreService_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/core/CoreService_pb2.pyi` & `caraml-store-0.1.7/feast/core/CoreService_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/core/CoreService_pb2_grpc.py` & `caraml-store-0.1.7/feast/core/CoreService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/core/DataFormat_pb2.py` & `caraml-store-0.1.7/feast/core/DataFormat_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/core/DataFormat_pb2.pyi` & `caraml-store-0.1.7/feast/core/DataFormat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/core/DataSource_pb2.py` & `caraml-store-0.1.7/feast/core/DataSource_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/core/DataSource_pb2.pyi` & `caraml-store-0.1.7/feast/core/DataSource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/core/Entity_pb2.py` & `caraml-store-0.1.7/feast/core/Entity_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/core/Entity_pb2.pyi` & `caraml-store-0.1.7/feast/core/Entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/core/FeatureTable_pb2.py` & `caraml-store-0.1.7/feast/core/FeatureTable_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/core/FeatureTable_pb2.pyi` & `caraml-store-0.1.7/feast/core/FeatureTable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/core/Feature_pb2.py` & `caraml-store-0.1.7/feast/core/Feature_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/core/Feature_pb2.pyi` & `caraml-store-0.1.7/feast/core/Feature_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/core/OnlineStore_pb2.py` & `caraml-store-0.1.7/feast/core/OnlineStore_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/core/OnlineStore_pb2.pyi` & `caraml-store-0.1.7/feast/core/OnlineStore_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/core/SparkOverride_pb2.py` & `caraml-store-0.1.7/feast/core/SparkOverride_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/core/SparkOverride_pb2.pyi` & `caraml-store-0.1.7/feast/core/SparkOverride_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/data_format.py` & `caraml-store-0.1.7/feast/data_format.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/data_source.py` & `caraml-store-0.1.7/feast/data_source.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/entity.py` & `caraml-store-0.1.7/feast/entity.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/feature.py` & `caraml-store-0.1.7/feast/feature.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/feature_table.py` & `caraml-store-0.1.7/feast/feature_table.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/gcp/staging.py` & `caraml-store-0.1.7/feast/gcp/staging.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/loaders/file.py` & `caraml-store-0.1.7/feast/loaders/file.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/online_response.py` & `caraml-store-0.1.7/feast/online_response.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/online_store.py` & `caraml-store-0.1.7/feast/online_store.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/serving/ServingService_pb2.py` & `caraml-store-0.1.7/feast/serving/ServingService_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/serving/ServingService_pb2.pyi` & `caraml-store-0.1.7/feast/serving/ServingService_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/serving/ServingService_pb2_grpc.py` & `caraml-store-0.1.7/feast/serving/ServingService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/types/Field_pb2.py` & `caraml-store-0.1.7/feast/types/Field_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/types/Field_pb2.pyi` & `caraml-store-0.1.7/feast/types/Field_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/types/Value_pb2.py` & `caraml-store-0.1.7/feast/types/Value_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast/types/Value_pb2.pyi` & `caraml-store-0.1.7/feast/types/Value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/feast_spark/api/JobService_pb2.py` & `caraml-store-0.1.7/feast_spark/api/JobService_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,62 +11,72 @@
 _sym_db = _symbol_database.Default()
 
 
 from feast.core import DataSource_pb2 as feast_dot_core_dot_DataSource__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n feast_spark/api/JobService.proto\x12\x0f\x66\x65\x61st_spark.api\x1a\x1b\x66\x65\x61st/core/DataSource.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xa6\x05\n\x03Job\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12,\n\x04type\x18\x02 \x01(\x0e\x32\x18.feast_spark.api.JobTypeR\x04type\x12\x32\n\x06status\x18\x03 \x01(\x0e\x32\x1a.feast_spark.api.JobStatusR\x06status\x12\x12\n\x04hash\x18\x04 \x01(\tR\x04hash\x12\x39\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartTime\x12\x45\n\tretrieval\x18\x06 \x01(\x0b\x32%.feast_spark.api.Job.RetrievalJobMetaH\x00R\tretrieval\x12S\n\x0f\x62\x61tch_ingestion\x18\x07 \x01(\x0b\x32(.feast_spark.api.Job.OfflineToOnlineMetaH\x00R\x0e\x62\x61tchIngestion\x12T\n\x10stream_ingestion\x18\x08 \x01(\x0b\x32\'.feast_spark.api.Job.StreamToOnlineMetaH\x00R\x0fstreamIngestion\x12\x17\n\x07log_uri\x18\t \x01(\tR\x06logUri\x12#\n\rerror_message\x18\n \x01(\tR\x0c\x65rrorMessage\x1a;\n\x10RetrievalJobMeta\x12\'\n\x0foutput_location\x18\x01 \x01(\tR\x0eoutputLocation\x1a\x34\n\x13OfflineToOnlineMeta\x12\x1d\n\ntable_name\x18\x01 \x01(\tR\ttableName\x1a\x33\n\x12StreamToOnlineMeta\x12\x1d\n\ntable_name\x18\x01 \x01(\tR\ttableNameB\x06\n\x04meta\"\xfd\x01\n\'StartOfflineToOnlineIngestionJobRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x12\x39\n\nstart_date\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartDate\x12\x35\n\x08\x65nd_date\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x65ndDate\x12\'\n\x0f\x64\x65lta_ingestion\x18\x05 \x01(\x08R\x0e\x64\x65ltaIngestion\"\xb4\x01\n(StartOfflineToOnlineIngestionJobResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12@\n\x0ejob_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cjobStartTime\x12\x1d\n\ntable_name\x18\x03 \x01(\tR\ttableName\x12\x17\n\x07log_uri\x18\x04 \x01(\tR\x06logUri\"\xb9\x01\n*ScheduleOfflineToOnlineIngestionJobRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x12-\n\x12ingestion_timespan\x18\x03 \x01(\x05R\x11ingestionTimespan\x12#\n\rcron_schedule\x18\x04 \x01(\tR\x0c\x63ronSchedule\"-\n+ScheduleOfflineToOnlineIngestionJobResponse\"g\n,UnscheduleOfflineToOnlineIngestionJobRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\"/\n-UnscheduleOfflineToOnlineIngestionJobResponse\"\xe6\x01\n\x1cGetHistoricalFeaturesRequest\x12!\n\x0c\x66\x65\x61ture_refs\x18\x01 \x03(\tR\x0b\x66\x65\x61tureRefs\x12;\n\rentity_source\x18\x02 \x01(\x0b\x32\x16.feast.core.DataSourceR\x0c\x65ntitySource\x12\x18\n\x07project\x18\x03 \x01(\tR\x07project\x12\'\n\x0foutput_location\x18\x04 \x01(\tR\x0eoutputLocation\x12#\n\routput_format\x18\x05 \x01(\tR\x0coutputFormat\"\xb2\x01\n\x1dGetHistoricalFeaturesResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12&\n\x0foutput_file_uri\x18\x02 \x01(\tR\routputFileUri\x12@\n\x0ejob_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cjobStartTime\x12\x17\n\x07log_uri\x18\x04 \x01(\tR\x06logUri\"y\n\x0fListJobsRequest\x12-\n\x12include_terminated\x18\x01 \x01(\x08R\x11includeTerminated\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x12\x18\n\x07project\x18\x03 \x01(\tR\x07project\"<\n\x10ListJobsResponse\x12(\n\x04jobs\x18\x01 \x03(\x0b\x32\x14.feast_spark.api.JobR\x04jobs\"&\n\rGetJobRequest\x12\x15\n\x06job_id\x18\x01 \x01(\tR\x05jobId\"8\n\x0eGetJobResponse\x12&\n\x03job\x18\x01 \x01(\x0b\x32\x14.feast_spark.api.JobR\x03job\")\n\x10\x43\x61ncelJobRequest\x12\x15\n\x06job_id\x18\x01 \x01(\tR\x05jobId\"\x13\n\x11\x43\x61ncelJobResponse\"T\n\x17GetHealthMetricsRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1f\n\x0btable_names\x18\x02 \x03(\tR\ntableNames\"J\n\x18GetHealthMetricsResponse\x12\x16\n\x06passed\x18\x01 \x03(\tR\x06passed\x12\x16\n\x06\x66\x61iled\x18\x02 \x03(\tR\x06\x66\x61iled*`\n\x07JobType\x12\x0f\n\x0bINVALID_JOB\x10\x00\x12\x17\n\x13\x42\x41TCH_INGESTION_JOB\x10\x01\x12\x18\n\x14STREAM_INGESTION_JOB\x10\x02\x12\x11\n\rRETRIEVAL_JOB\x10\x04*~\n\tJobStatus\x12\x16\n\x12JOB_STATUS_INVALID\x10\x00\x12\x16\n\x12JOB_STATUS_PENDING\x10\x01\x12\x16\n\x12JOB_STATUS_RUNNING\x10\x02\x12\x13\n\x0fJOB_STATUS_DONE\x10\x03\x12\x14\n\x10JOB_STATUS_ERROR\x10\x04\x32\xc3\x07\n\nJobService\x12\x97\x01\n StartOfflineToOnlineIngestionJob\x12\x38.feast_spark.api.StartOfflineToOnlineIngestionJobRequest\x1a\x39.feast_spark.api.StartOfflineToOnlineIngestionJobResponse\x12\xa0\x01\n#ScheduleOfflineToOnlineIngestionJob\x12;.feast_spark.api.ScheduleOfflineToOnlineIngestionJobRequest\x1a<.feast_spark.api.ScheduleOfflineToOnlineIngestionJobResponse\x12\xa6\x01\n%UnscheduleOfflineToOnlineIngestionJob\x12=.feast_spark.api.UnscheduleOfflineToOnlineIngestionJobRequest\x1a>.feast_spark.api.UnscheduleOfflineToOnlineIngestionJobResponse\x12v\n\x15GetHistoricalFeatures\x12-.feast_spark.api.GetHistoricalFeaturesRequest\x1a..feast_spark.api.GetHistoricalFeaturesResponse\x12O\n\x08ListJobs\x12 .feast_spark.api.ListJobsRequest\x1a!.feast_spark.api.ListJobsResponse\x12R\n\tCancelJob\x12!.feast_spark.api.CancelJobRequest\x1a\".feast_spark.api.CancelJobResponse\x12I\n\x06GetJob\x12\x1e.feast_spark.api.GetJobRequest\x1a\x1f.feast_spark.api.GetJobResponse\x12g\n\x10GetHealthMetrics\x12(.feast_spark.api.GetHealthMetricsRequest\x1a).feast_spark.api.GetHealthMetricsResponseB\x86\x01\n$dev.caraml.store.protobuf.jobserviceB\x0fJobServiceProtoZMgithub.com/caraml-dev/caraml-store/caraml-store-sdk/go/protos/feast_spark/apib\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n feast_spark/api/JobService.proto\x12\x0f\x66\x65\x61st_spark.api\x1a\x1b\x66\x65\x61st/core/DataSource.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xab\x01\n\x0cScheduledJob\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x12\x18\n\x07project\x18\x03 \x01(\tR\x07project\x12-\n\x12ingestion_timespan\x18\x04 \x01(\x05R\x11ingestionTimespan\x12#\n\rcron_schedule\x18\x05 \x01(\tR\x0c\x63ronSchedule\"\xa6\x05\n\x03Job\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12,\n\x04type\x18\x02 \x01(\x0e\x32\x18.feast_spark.api.JobTypeR\x04type\x12\x32\n\x06status\x18\x03 \x01(\x0e\x32\x1a.feast_spark.api.JobStatusR\x06status\x12\x12\n\x04hash\x18\x04 \x01(\tR\x04hash\x12\x39\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartTime\x12\x45\n\tretrieval\x18\x06 \x01(\x0b\x32%.feast_spark.api.Job.RetrievalJobMetaH\x00R\tretrieval\x12S\n\x0f\x62\x61tch_ingestion\x18\x07 \x01(\x0b\x32(.feast_spark.api.Job.OfflineToOnlineMetaH\x00R\x0e\x62\x61tchIngestion\x12T\n\x10stream_ingestion\x18\x08 \x01(\x0b\x32\'.feast_spark.api.Job.StreamToOnlineMetaH\x00R\x0fstreamIngestion\x12\x17\n\x07log_uri\x18\t \x01(\tR\x06logUri\x12#\n\rerror_message\x18\n \x01(\tR\x0c\x65rrorMessage\x1a;\n\x10RetrievalJobMeta\x12\'\n\x0foutput_location\x18\x01 \x01(\tR\x0eoutputLocation\x1a\x34\n\x13OfflineToOnlineMeta\x12\x1d\n\ntable_name\x18\x01 \x01(\tR\ttableName\x1a\x33\n\x12StreamToOnlineMeta\x12\x1d\n\ntable_name\x18\x01 \x01(\tR\ttableNameB\x06\n\x04meta\"\xfd\x01\n\'StartOfflineToOnlineIngestionJobRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x12\x39\n\nstart_date\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartDate\x12\x35\n\x08\x65nd_date\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x65ndDate\x12\'\n\x0f\x64\x65lta_ingestion\x18\x05 \x01(\x08R\x0e\x64\x65ltaIngestion\"\xb4\x01\n(StartOfflineToOnlineIngestionJobResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12@\n\x0ejob_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cjobStartTime\x12\x1d\n\ntable_name\x18\x03 \x01(\tR\ttableName\x12\x17\n\x07log_uri\x18\x04 \x01(\tR\x06logUri\"Y\n\x1eStartStreamIngestionJobRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\"1\n\x1fStartStreamIngestionJobResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\"\xb9\x01\n*ScheduleOfflineToOnlineIngestionJobRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x12-\n\x12ingestion_timespan\x18\x03 \x01(\x05R\x11ingestionTimespan\x12#\n\rcron_schedule\x18\x04 \x01(\tR\x0c\x63ronSchedule\"-\n+ScheduleOfflineToOnlineIngestionJobResponse\"g\n,UnscheduleOfflineToOnlineIngestionJobRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\"/\n-UnscheduleOfflineToOnlineIngestionJobResponse\"\xe6\x01\n\x1cGetHistoricalFeaturesRequest\x12!\n\x0c\x66\x65\x61ture_refs\x18\x01 \x03(\tR\x0b\x66\x65\x61tureRefs\x12;\n\rentity_source\x18\x02 \x01(\x0b\x32\x16.feast.core.DataSourceR\x0c\x65ntitySource\x12\x18\n\x07project\x18\x03 \x01(\tR\x07project\x12\'\n\x0foutput_location\x18\x04 \x01(\tR\x0eoutputLocation\x12#\n\routput_format\x18\x05 \x01(\tR\x0coutputFormat\"\xb2\x01\n\x1dGetHistoricalFeaturesResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12&\n\x0foutput_file_uri\x18\x02 \x01(\tR\routputFileUri\x12@\n\x0ejob_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cjobStartTime\x12\x17\n\x07log_uri\x18\x04 \x01(\tR\x06logUri\"\xa7\x01\n\x0fListJobsRequest\x12-\n\x12include_terminated\x18\x01 \x01(\x08R\x11includeTerminated\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x12\x18\n\x07project\x18\x03 \x01(\tR\x07project\x12,\n\x04type\x18\x04 \x01(\x0e\x32\x18.feast_spark.api.JobTypeR\x04type\"S\n\x18ListScheduledJobsRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\"<\n\x10ListJobsResponse\x12(\n\x04jobs\x18\x01 \x03(\x0b\x32\x14.feast_spark.api.JobR\x04jobs\"N\n\x19ListScheduledJobsResponse\x12\x31\n\x04jobs\x18\x01 \x03(\x0b\x32\x1d.feast_spark.api.ScheduledJobR\x04jobs\"&\n\rGetJobRequest\x12\x15\n\x06job_id\x18\x01 \x01(\tR\x05jobId\"8\n\x0eGetJobResponse\x12&\n\x03job\x18\x01 \x01(\x0b\x32\x14.feast_spark.api.JobR\x03job\")\n\x10\x43\x61ncelJobRequest\x12\x15\n\x06job_id\x18\x01 \x01(\tR\x05jobId\"\x13\n\x11\x43\x61ncelJobResponse\"T\n\x17GetHealthMetricsRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1f\n\x0btable_names\x18\x02 \x03(\tR\ntableNames\"J\n\x18GetHealthMetricsResponse\x12\x16\n\x06passed\x18\x01 \x03(\tR\x06passed\x12\x16\n\x06\x66\x61iled\x18\x02 \x03(\tR\x06\x66\x61iled*`\n\x07JobType\x12\x0f\n\x0bINVALID_JOB\x10\x00\x12\x17\n\x13\x42\x41TCH_INGESTION_JOB\x10\x01\x12\x18\n\x14STREAM_INGESTION_JOB\x10\x02\x12\x11\n\rRETRIEVAL_JOB\x10\x04*~\n\tJobStatus\x12\x16\n\x12JOB_STATUS_INVALID\x10\x00\x12\x16\n\x12JOB_STATUS_PENDING\x10\x01\x12\x16\n\x12JOB_STATUS_RUNNING\x10\x02\x12\x13\n\x0fJOB_STATUS_DONE\x10\x03\x12\x14\n\x10JOB_STATUS_ERROR\x10\x04\x32\xad\t\n\nJobService\x12\x97\x01\n StartOfflineToOnlineIngestionJob\x12\x38.feast_spark.api.StartOfflineToOnlineIngestionJobRequest\x1a\x39.feast_spark.api.StartOfflineToOnlineIngestionJobResponse\x12|\n\x17StartStreamIngestionJob\x12/.feast_spark.api.StartStreamIngestionJobRequest\x1a\x30.feast_spark.api.StartStreamIngestionJobResponse\x12\xa0\x01\n#ScheduleOfflineToOnlineIngestionJob\x12;.feast_spark.api.ScheduleOfflineToOnlineIngestionJobRequest\x1a<.feast_spark.api.ScheduleOfflineToOnlineIngestionJobResponse\x12\xa6\x01\n%UnscheduleOfflineToOnlineIngestionJob\x12=.feast_spark.api.UnscheduleOfflineToOnlineIngestionJobRequest\x1a>.feast_spark.api.UnscheduleOfflineToOnlineIngestionJobResponse\x12v\n\x15GetHistoricalFeatures\x12-.feast_spark.api.GetHistoricalFeaturesRequest\x1a..feast_spark.api.GetHistoricalFeaturesResponse\x12O\n\x08ListJobs\x12 .feast_spark.api.ListJobsRequest\x1a!.feast_spark.api.ListJobsResponse\x12j\n\x11ListScheduledJobs\x12).feast_spark.api.ListScheduledJobsRequest\x1a*.feast_spark.api.ListScheduledJobsResponse\x12R\n\tCancelJob\x12!.feast_spark.api.CancelJobRequest\x1a\".feast_spark.api.CancelJobResponse\x12I\n\x06GetJob\x12\x1e.feast_spark.api.GetJobRequest\x1a\x1f.feast_spark.api.GetJobResponse\x12g\n\x10GetHealthMetrics\x12(.feast_spark.api.GetHealthMetricsRequest\x1a).feast_spark.api.GetHealthMetricsResponseB\x86\x01\n$dev.caraml.store.protobuf.jobserviceB\x0fJobServiceProtoZMgithub.com/caraml-dev/caraml-store/caraml-store-sdk/go/protos/feast_spark/apib\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'feast_spark.api.JobService_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n$dev.caraml.store.protobuf.jobserviceB\017JobServiceProtoZMgithub.com/caraml-dev/caraml-store/caraml-store-sdk/go/protos/feast_spark/api'
-  _JOBTYPE._serialized_start=2547
-  _JOBTYPE._serialized_end=2643
-  _JOBSTATUS._serialized_start=2645
-  _JOBSTATUS._serialized_end=2771
-  _JOB._serialized_start=116
-  _JOB._serialized_end=794
-  _JOB_RETRIEVALJOBMETA._serialized_start=620
-  _JOB_RETRIEVALJOBMETA._serialized_end=679
-  _JOB_OFFLINETOONLINEMETA._serialized_start=681
-  _JOB_OFFLINETOONLINEMETA._serialized_end=733
-  _JOB_STREAMTOONLINEMETA._serialized_start=735
-  _JOB_STREAMTOONLINEMETA._serialized_end=786
-  _STARTOFFLINETOONLINEINGESTIONJOBREQUEST._serialized_start=797
-  _STARTOFFLINETOONLINEINGESTIONJOBREQUEST._serialized_end=1050
-  _STARTOFFLINETOONLINEINGESTIONJOBRESPONSE._serialized_start=1053
-  _STARTOFFLINETOONLINEINGESTIONJOBRESPONSE._serialized_end=1233
-  _SCHEDULEOFFLINETOONLINEINGESTIONJOBREQUEST._serialized_start=1236
-  _SCHEDULEOFFLINETOONLINEINGESTIONJOBREQUEST._serialized_end=1421
-  _SCHEDULEOFFLINETOONLINEINGESTIONJOBRESPONSE._serialized_start=1423
-  _SCHEDULEOFFLINETOONLINEINGESTIONJOBRESPONSE._serialized_end=1468
-  _UNSCHEDULEOFFLINETOONLINEINGESTIONJOBREQUEST._serialized_start=1470
-  _UNSCHEDULEOFFLINETOONLINEINGESTIONJOBREQUEST._serialized_end=1573
-  _UNSCHEDULEOFFLINETOONLINEINGESTIONJOBRESPONSE._serialized_start=1575
-  _UNSCHEDULEOFFLINETOONLINEINGESTIONJOBRESPONSE._serialized_end=1622
-  _GETHISTORICALFEATURESREQUEST._serialized_start=1625
-  _GETHISTORICALFEATURESREQUEST._serialized_end=1855
-  _GETHISTORICALFEATURESRESPONSE._serialized_start=1858
-  _GETHISTORICALFEATURESRESPONSE._serialized_end=2036
-  _LISTJOBSREQUEST._serialized_start=2038
-  _LISTJOBSREQUEST._serialized_end=2159
-  _LISTJOBSRESPONSE._serialized_start=2161
-  _LISTJOBSRESPONSE._serialized_end=2221
-  _GETJOBREQUEST._serialized_start=2223
-  _GETJOBREQUEST._serialized_end=2261
-  _GETJOBRESPONSE._serialized_start=2263
-  _GETJOBRESPONSE._serialized_end=2319
-  _CANCELJOBREQUEST._serialized_start=2321
-  _CANCELJOBREQUEST._serialized_end=2362
-  _CANCELJOBRESPONSE._serialized_start=2364
-  _CANCELJOBRESPONSE._serialized_end=2383
-  _GETHEALTHMETRICSREQUEST._serialized_start=2385
-  _GETHEALTHMETRICSREQUEST._serialized_end=2469
-  _GETHEALTHMETRICSRESPONSE._serialized_start=2471
-  _GETHEALTHMETRICSRESPONSE._serialized_end=2545
-  _JOBSERVICE._serialized_start=2774
-  _JOBSERVICE._serialized_end=3737
+  _JOBTYPE._serialized_start=3075
+  _JOBTYPE._serialized_end=3171
+  _JOBSTATUS._serialized_start=3173
+  _JOBSTATUS._serialized_end=3299
+  _SCHEDULEDJOB._serialized_start=116
+  _SCHEDULEDJOB._serialized_end=287
+  _JOB._serialized_start=290
+  _JOB._serialized_end=968
+  _JOB_RETRIEVALJOBMETA._serialized_start=794
+  _JOB_RETRIEVALJOBMETA._serialized_end=853
+  _JOB_OFFLINETOONLINEMETA._serialized_start=855
+  _JOB_OFFLINETOONLINEMETA._serialized_end=907
+  _JOB_STREAMTOONLINEMETA._serialized_start=909
+  _JOB_STREAMTOONLINEMETA._serialized_end=960
+  _STARTOFFLINETOONLINEINGESTIONJOBREQUEST._serialized_start=971
+  _STARTOFFLINETOONLINEINGESTIONJOBREQUEST._serialized_end=1224
+  _STARTOFFLINETOONLINEINGESTIONJOBRESPONSE._serialized_start=1227
+  _STARTOFFLINETOONLINEINGESTIONJOBRESPONSE._serialized_end=1407
+  _STARTSTREAMINGESTIONJOBREQUEST._serialized_start=1409
+  _STARTSTREAMINGESTIONJOBREQUEST._serialized_end=1498
+  _STARTSTREAMINGESTIONJOBRESPONSE._serialized_start=1500
+  _STARTSTREAMINGESTIONJOBRESPONSE._serialized_end=1549
+  _SCHEDULEOFFLINETOONLINEINGESTIONJOBREQUEST._serialized_start=1552
+  _SCHEDULEOFFLINETOONLINEINGESTIONJOBREQUEST._serialized_end=1737
+  _SCHEDULEOFFLINETOONLINEINGESTIONJOBRESPONSE._serialized_start=1739
+  _SCHEDULEOFFLINETOONLINEINGESTIONJOBRESPONSE._serialized_end=1784
+  _UNSCHEDULEOFFLINETOONLINEINGESTIONJOBREQUEST._serialized_start=1786
+  _UNSCHEDULEOFFLINETOONLINEINGESTIONJOBREQUEST._serialized_end=1889
+  _UNSCHEDULEOFFLINETOONLINEINGESTIONJOBRESPONSE._serialized_start=1891
+  _UNSCHEDULEOFFLINETOONLINEINGESTIONJOBRESPONSE._serialized_end=1938
+  _GETHISTORICALFEATURESREQUEST._serialized_start=1941
+  _GETHISTORICALFEATURESREQUEST._serialized_end=2171
+  _GETHISTORICALFEATURESRESPONSE._serialized_start=2174
+  _GETHISTORICALFEATURESRESPONSE._serialized_end=2352
+  _LISTJOBSREQUEST._serialized_start=2355
+  _LISTJOBSREQUEST._serialized_end=2522
+  _LISTSCHEDULEDJOBSREQUEST._serialized_start=2524
+  _LISTSCHEDULEDJOBSREQUEST._serialized_end=2607
+  _LISTJOBSRESPONSE._serialized_start=2609
+  _LISTJOBSRESPONSE._serialized_end=2669
+  _LISTSCHEDULEDJOBSRESPONSE._serialized_start=2671
+  _LISTSCHEDULEDJOBSRESPONSE._serialized_end=2749
+  _GETJOBREQUEST._serialized_start=2751
+  _GETJOBREQUEST._serialized_end=2789
+  _GETJOBRESPONSE._serialized_start=2791
+  _GETJOBRESPONSE._serialized_end=2847
+  _CANCELJOBREQUEST._serialized_start=2849
+  _CANCELJOBREQUEST._serialized_end=2890
+  _CANCELJOBRESPONSE._serialized_start=2892
+  _CANCELJOBRESPONSE._serialized_end=2911
+  _GETHEALTHMETRICSREQUEST._serialized_start=2913
+  _GETHEALTHMETRICSREQUEST._serialized_end=2997
+  _GETHEALTHMETRICSRESPONSE._serialized_start=2999
+  _GETHEALTHMETRICSRESPONSE._serialized_end=3073
+  _JOBSERVICE._serialized_start=3302
+  _JOBSERVICE._serialized_end=4499
 # @@protoc_insertion_point(module_scope)
```

### Comparing `caraml-store-0.1.6/feast_spark/api/JobService_pb2.pyi` & `caraml-store-0.1.7/feast_spark/api/JobService_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -117,29 +117,45 @@
     start_time: _timestamp_pb2.Timestamp
     status: JobStatus
     stream_ingestion: Job.StreamToOnlineMeta
     type: JobType
     def __init__(self, id: _Optional[str] = ..., type: _Optional[_Union[JobType, str]] = ..., status: _Optional[_Union[JobStatus, str]] = ..., hash: _Optional[str] = ..., start_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., retrieval: _Optional[_Union[Job.RetrievalJobMeta, _Mapping]] = ..., batch_ingestion: _Optional[_Union[Job.OfflineToOnlineMeta, _Mapping]] = ..., stream_ingestion: _Optional[_Union[Job.StreamToOnlineMeta, _Mapping]] = ..., log_uri: _Optional[str] = ..., error_message: _Optional[str] = ...) -> None: ...
 
 class ListJobsRequest(_message.Message):
-    __slots__ = ["include_terminated", "project", "table_name"]
+    __slots__ = ["include_terminated", "project", "table_name", "type"]
     INCLUDE_TERMINATED_FIELD_NUMBER: _ClassVar[int]
     PROJECT_FIELD_NUMBER: _ClassVar[int]
     TABLE_NAME_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
     include_terminated: bool
     project: str
     table_name: str
-    def __init__(self, include_terminated: bool = ..., table_name: _Optional[str] = ..., project: _Optional[str] = ...) -> None: ...
+    type: JobType
+    def __init__(self, include_terminated: bool = ..., table_name: _Optional[str] = ..., project: _Optional[str] = ..., type: _Optional[_Union[JobType, str]] = ...) -> None: ...
 
 class ListJobsResponse(_message.Message):
     __slots__ = ["jobs"]
     JOBS_FIELD_NUMBER: _ClassVar[int]
     jobs: _containers.RepeatedCompositeFieldContainer[Job]
     def __init__(self, jobs: _Optional[_Iterable[_Union[Job, _Mapping]]] = ...) -> None: ...
 
+class ListScheduledJobsRequest(_message.Message):
+    __slots__ = ["project", "table_name"]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
+    TABLE_NAME_FIELD_NUMBER: _ClassVar[int]
+    project: str
+    table_name: str
+    def __init__(self, project: _Optional[str] = ..., table_name: _Optional[str] = ...) -> None: ...
+
+class ListScheduledJobsResponse(_message.Message):
+    __slots__ = ["jobs"]
+    JOBS_FIELD_NUMBER: _ClassVar[int]
+    jobs: _containers.RepeatedCompositeFieldContainer[ScheduledJob]
+    def __init__(self, jobs: _Optional[_Iterable[_Union[ScheduledJob, _Mapping]]] = ...) -> None: ...
+
 class ScheduleOfflineToOnlineIngestionJobRequest(_message.Message):
     __slots__ = ["cron_schedule", "ingestion_timespan", "project", "table_name"]
     CRON_SCHEDULE_FIELD_NUMBER: _ClassVar[int]
     INGESTION_TIMESPAN_FIELD_NUMBER: _ClassVar[int]
     PROJECT_FIELD_NUMBER: _ClassVar[int]
     TABLE_NAME_FIELD_NUMBER: _ClassVar[int]
     cron_schedule: str
@@ -148,14 +164,28 @@
     table_name: str
     def __init__(self, project: _Optional[str] = ..., table_name: _Optional[str] = ..., ingestion_timespan: _Optional[int] = ..., cron_schedule: _Optional[str] = ...) -> None: ...
 
 class ScheduleOfflineToOnlineIngestionJobResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
+class ScheduledJob(_message.Message):
+    __slots__ = ["cron_schedule", "id", "ingestion_timespan", "project", "table_name"]
+    CRON_SCHEDULE_FIELD_NUMBER: _ClassVar[int]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    INGESTION_TIMESPAN_FIELD_NUMBER: _ClassVar[int]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
+    TABLE_NAME_FIELD_NUMBER: _ClassVar[int]
+    cron_schedule: str
+    id: str
+    ingestion_timespan: int
+    project: str
+    table_name: str
+    def __init__(self, id: _Optional[str] = ..., table_name: _Optional[str] = ..., project: _Optional[str] = ..., ingestion_timespan: _Optional[int] = ..., cron_schedule: _Optional[str] = ...) -> None: ...
+
 class StartOfflineToOnlineIngestionJobRequest(_message.Message):
     __slots__ = ["delta_ingestion", "end_date", "project", "start_date", "table_name"]
     DELTA_INGESTION_FIELD_NUMBER: _ClassVar[int]
     END_DATE_FIELD_NUMBER: _ClassVar[int]
     PROJECT_FIELD_NUMBER: _ClassVar[int]
     START_DATE_FIELD_NUMBER: _ClassVar[int]
     TABLE_NAME_FIELD_NUMBER: _ClassVar[int]
@@ -174,14 +204,28 @@
     TABLE_NAME_FIELD_NUMBER: _ClassVar[int]
     id: str
     job_start_time: _timestamp_pb2.Timestamp
     log_uri: str
     table_name: str
     def __init__(self, id: _Optional[str] = ..., job_start_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., table_name: _Optional[str] = ..., log_uri: _Optional[str] = ...) -> None: ...
 
+class StartStreamIngestionJobRequest(_message.Message):
+    __slots__ = ["project", "table_name"]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
+    TABLE_NAME_FIELD_NUMBER: _ClassVar[int]
+    project: str
+    table_name: str
+    def __init__(self, project: _Optional[str] = ..., table_name: _Optional[str] = ...) -> None: ...
+
+class StartStreamIngestionJobResponse(_message.Message):
+    __slots__ = ["id"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    id: str
+    def __init__(self, id: _Optional[str] = ...) -> None: ...
+
 class UnscheduleOfflineToOnlineIngestionJobRequest(_message.Message):
     __slots__ = ["project", "table_name"]
     PROJECT_FIELD_NUMBER: _ClassVar[int]
     TABLE_NAME_FIELD_NUMBER: _ClassVar[int]
     project: str
     table_name: str
     def __init__(self, project: _Optional[str] = ..., table_name: _Optional[str] = ...) -> None: ...
```

### Comparing `caraml-store-0.1.6/feast_spark/api/JobService_pb2_grpc.py` & `caraml-store-0.1.7/feast_spark/api/JobService_pb2_grpc.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,19 @@
             channel: A grpc.Channel.
         """
         self.StartOfflineToOnlineIngestionJob = channel.unary_unary(
                 '/feast_spark.api.JobService/StartOfflineToOnlineIngestionJob',
                 request_serializer=feast__spark_dot_api_dot_JobService__pb2.StartOfflineToOnlineIngestionJobRequest.SerializeToString,
                 response_deserializer=feast__spark_dot_api_dot_JobService__pb2.StartOfflineToOnlineIngestionJobResponse.FromString,
                 )
+        self.StartStreamIngestionJob = channel.unary_unary(
+                '/feast_spark.api.JobService/StartStreamIngestionJob',
+                request_serializer=feast__spark_dot_api_dot_JobService__pb2.StartStreamIngestionJobRequest.SerializeToString,
+                response_deserializer=feast__spark_dot_api_dot_JobService__pb2.StartStreamIngestionJobResponse.FromString,
+                )
         self.ScheduleOfflineToOnlineIngestionJob = channel.unary_unary(
                 '/feast_spark.api.JobService/ScheduleOfflineToOnlineIngestionJob',
                 request_serializer=feast__spark_dot_api_dot_JobService__pb2.ScheduleOfflineToOnlineIngestionJobRequest.SerializeToString,
                 response_deserializer=feast__spark_dot_api_dot_JobService__pb2.ScheduleOfflineToOnlineIngestionJobResponse.FromString,
                 )
         self.UnscheduleOfflineToOnlineIngestionJob = channel.unary_unary(
                 '/feast_spark.api.JobService/UnscheduleOfflineToOnlineIngestionJob',
@@ -35,14 +40,19 @@
                 response_deserializer=feast__spark_dot_api_dot_JobService__pb2.GetHistoricalFeaturesResponse.FromString,
                 )
         self.ListJobs = channel.unary_unary(
                 '/feast_spark.api.JobService/ListJobs',
                 request_serializer=feast__spark_dot_api_dot_JobService__pb2.ListJobsRequest.SerializeToString,
                 response_deserializer=feast__spark_dot_api_dot_JobService__pb2.ListJobsResponse.FromString,
                 )
+        self.ListScheduledJobs = channel.unary_unary(
+                '/feast_spark.api.JobService/ListScheduledJobs',
+                request_serializer=feast__spark_dot_api_dot_JobService__pb2.ListScheduledJobsRequest.SerializeToString,
+                response_deserializer=feast__spark_dot_api_dot_JobService__pb2.ListScheduledJobsResponse.FromString,
+                )
         self.CancelJob = channel.unary_unary(
                 '/feast_spark.api.JobService/CancelJob',
                 request_serializer=feast__spark_dot_api_dot_JobService__pb2.CancelJobRequest.SerializeToString,
                 response_deserializer=feast__spark_dot_api_dot_JobService__pb2.CancelJobResponse.FromString,
                 )
         self.GetJob = channel.unary_unary(
                 '/feast_spark.api.JobService/GetJob',
@@ -62,14 +72,21 @@
     def StartOfflineToOnlineIngestionJob(self, request, context):
         """Start job to ingest data from offline store into online store
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def StartStreamIngestionJob(self, request, context):
+        """Start job to ingest data from streaming source into online store
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def ScheduleOfflineToOnlineIngestionJob(self, request, context):
         """Start scheduled job to ingest data from offline store into online store
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -90,14 +107,21 @@
     def ListJobs(self, request, context):
         """List all types of jobs
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def ListScheduledJobs(self, request, context):
+        """List all scheduled jobs
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def CancelJob(self, request, context):
         """Cancel a single job
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -119,14 +143,19 @@
 def add_JobServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'StartOfflineToOnlineIngestionJob': grpc.unary_unary_rpc_method_handler(
                     servicer.StartOfflineToOnlineIngestionJob,
                     request_deserializer=feast__spark_dot_api_dot_JobService__pb2.StartOfflineToOnlineIngestionJobRequest.FromString,
                     response_serializer=feast__spark_dot_api_dot_JobService__pb2.StartOfflineToOnlineIngestionJobResponse.SerializeToString,
             ),
+            'StartStreamIngestionJob': grpc.unary_unary_rpc_method_handler(
+                    servicer.StartStreamIngestionJob,
+                    request_deserializer=feast__spark_dot_api_dot_JobService__pb2.StartStreamIngestionJobRequest.FromString,
+                    response_serializer=feast__spark_dot_api_dot_JobService__pb2.StartStreamIngestionJobResponse.SerializeToString,
+            ),
             'ScheduleOfflineToOnlineIngestionJob': grpc.unary_unary_rpc_method_handler(
                     servicer.ScheduleOfflineToOnlineIngestionJob,
                     request_deserializer=feast__spark_dot_api_dot_JobService__pb2.ScheduleOfflineToOnlineIngestionJobRequest.FromString,
                     response_serializer=feast__spark_dot_api_dot_JobService__pb2.ScheduleOfflineToOnlineIngestionJobResponse.SerializeToString,
             ),
             'UnscheduleOfflineToOnlineIngestionJob': grpc.unary_unary_rpc_method_handler(
                     servicer.UnscheduleOfflineToOnlineIngestionJob,
@@ -139,14 +168,19 @@
                     response_serializer=feast__spark_dot_api_dot_JobService__pb2.GetHistoricalFeaturesResponse.SerializeToString,
             ),
             'ListJobs': grpc.unary_unary_rpc_method_handler(
                     servicer.ListJobs,
                     request_deserializer=feast__spark_dot_api_dot_JobService__pb2.ListJobsRequest.FromString,
                     response_serializer=feast__spark_dot_api_dot_JobService__pb2.ListJobsResponse.SerializeToString,
             ),
+            'ListScheduledJobs': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListScheduledJobs,
+                    request_deserializer=feast__spark_dot_api_dot_JobService__pb2.ListScheduledJobsRequest.FromString,
+                    response_serializer=feast__spark_dot_api_dot_JobService__pb2.ListScheduledJobsResponse.SerializeToString,
+            ),
             'CancelJob': grpc.unary_unary_rpc_method_handler(
                     servicer.CancelJob,
                     request_deserializer=feast__spark_dot_api_dot_JobService__pb2.CancelJobRequest.FromString,
                     response_serializer=feast__spark_dot_api_dot_JobService__pb2.CancelJobResponse.SerializeToString,
             ),
             'GetJob': grpc.unary_unary_rpc_method_handler(
                     servicer.GetJob,
@@ -182,14 +216,31 @@
         return grpc.experimental.unary_unary(request, target, '/feast_spark.api.JobService/StartOfflineToOnlineIngestionJob',
             feast__spark_dot_api_dot_JobService__pb2.StartOfflineToOnlineIngestionJobRequest.SerializeToString,
             feast__spark_dot_api_dot_JobService__pb2.StartOfflineToOnlineIngestionJobResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def StartStreamIngestionJob(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/feast_spark.api.JobService/StartStreamIngestionJob',
+            feast__spark_dot_api_dot_JobService__pb2.StartStreamIngestionJobRequest.SerializeToString,
+            feast__spark_dot_api_dot_JobService__pb2.StartStreamIngestionJobResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def ScheduleOfflineToOnlineIngestionJob(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -250,14 +301,31 @@
         return grpc.experimental.unary_unary(request, target, '/feast_spark.api.JobService/ListJobs',
             feast__spark_dot_api_dot_JobService__pb2.ListJobsRequest.SerializeToString,
             feast__spark_dot_api_dot_JobService__pb2.ListJobsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def ListScheduledJobs(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/feast_spark.api.JobService/ListScheduledJobs',
+            feast__spark_dot_api_dot_JobService__pb2.ListScheduledJobsRequest.SerializeToString,
+            feast__spark_dot_api_dot_JobService__pb2.ListScheduledJobsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def CancelJob(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `caraml-store-0.1.6/setup.py` & `caraml-store-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/tests/data/test_feature_table.yaml` & `caraml-store-0.1.7/tests/data/test_feature_table.yaml`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/tests/test_model_protobuf_conversion.py` & `caraml-store-0.1.7/tests/test_model_protobuf_conversion.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.6/utils/compile_protos.sh` & `caraml-store-0.1.7/utils/compile_protos.sh`

 * *Files identical despite different names*

