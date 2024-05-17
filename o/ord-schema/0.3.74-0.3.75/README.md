# Comparing `tmp/ord-schema-0.3.74.tar.gz` & `tmp/ord_schema-0.3.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ord-schema-0.3.74.tar", last modified: Wed Apr 10 14:44:49 2024, max compression
+gzip compressed data, was "ord_schema-0.3.75.tar", last modified: Fri Apr 12 20:50:49 2024, max compression
```

## Comparing `ord-schema-0.3.74.tar` & `ord_schema-0.3.75.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:44:49.192983 ord-schema-0.3.74/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-10 14:44:33.000000 ord-schema-0.3.74/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 14:44:33.000000 ord-schema-0.3.74/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 14:44:33.000000 ord-schema-0.3.74/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-10 14:44:49.192983 ord-schema-0.3.74/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-10 14:44:33.000000 ord-schema-0.3.74/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:44:49.180983 ord-schema-0.3.74/ord_schema/
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/frozen_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/frozen_message_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:44:49.180983 ord-schema-0.3.74/ord_schema/macros/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/macros/solutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/macros/solutions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/macros/workups.py
--rw-r--r--   0 runner    (1001) docker     (127)    36688 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/message_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/message_helpers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:44:49.184983 ord-schema-0.3.74/ord_schema/orm/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/orm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/orm/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/orm/database_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/orm/mappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/orm/mappers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/orm/rdkit_mappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/orm/rdkit_mappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:44:49.184983 ord-schema-0.3.74/ord_schema/proto/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/proto/dataset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/proto/dataset_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/proto/dataset_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    49297 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/proto/reaction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    91519 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/proto/reaction_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/proto/reaction_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/proto/test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/resolvers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:44:49.188984 ord-schema-0.3.74/ord_schema/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/build_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/check_pb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/check_pb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/enumerate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/enumerate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22381 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/parse_uspto.py
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/process_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    21548 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/process_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/validate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/scripts/validate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/templating_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17564 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/units_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/updates_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    47179 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/validations.py
--rw-r--r--   0 runner    (1001) docker     (127)    23136 2024-04-10 14:44:33.000000 ord-schema-0.3.74/ord_schema/validations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:44:49.188984 ord-schema-0.3.74/ord_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-10 14:44:49.000000 ord-schema-0.3.74/ord_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-10 14:44:49.000000 ord-schema-0.3.74/ord_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:44:49.000000 ord-schema-0.3.74/ord_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-10 14:44:49.000000 ord-schema-0.3.74/ord_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 14:44:49.000000 ord-schema-0.3.74/ord_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:44:49.188984 ord-schema-0.3.74/proto/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-10 14:44:33.000000 ord-schema-0.3.74/proto/dataset.proto
--rw-r--r--   0 runner    (1001) docker     (127)    46965 2024-04-10 14:44:33.000000 ord-schema-0.3.74/proto/reaction.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-10 14:44:33.000000 ord-schema-0.3.74/proto/test.proto
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-10 14:44:33.000000 ord-schema-0.3.74/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:44:49.192983 ord-schema-0.3.74/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-10 14:44:36.000000 ord-schema-0.3.74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:50:49.387121 ord_schema-0.3.75/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-12 20:50:36.000000 ord_schema-0.3.75/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 20:50:36.000000 ord_schema-0.3.75/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 20:50:36.000000 ord_schema-0.3.75/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-12 20:50:49.387121 ord_schema-0.3.75/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-12 20:50:36.000000 ord_schema-0.3.75/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:50:49.375121 ord_schema-0.3.75/ord_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/frozen_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/frozen_message_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:50:49.379121 ord_schema-0.3.75/ord_schema/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/macros/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/macros/solutions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/macros/workups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36688 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/message_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/message_helpers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:50:49.379121 ord_schema-0.3.75/ord_schema/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/orm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/orm/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/orm/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/orm/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/orm/mappers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/orm/rdkit_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/orm/rdkit_mappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:50:49.379121 ord_schema-0.3.75/ord_schema/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/proto/dataset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/proto/dataset_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/proto/dataset_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49297 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/proto/reaction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91519 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/proto/reaction_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/proto/reaction_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/proto/test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/resolvers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:50:49.383121 ord_schema-0.3.75/ord_schema/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/scripts/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/scripts/build_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/scripts/check_pb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/scripts/check_pb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/scripts/enumerate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/scripts/enumerate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22381 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/scripts/parse_uspto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/scripts/process_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21548 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/scripts/process_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/scripts/validate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/scripts/validate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/templating_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17564 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/updates_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47179 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23136 2024-04-12 20:50:36.000000 ord_schema-0.3.75/ord_schema/validations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:50:49.383121 ord_schema-0.3.75/ord_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-12 20:50:49.000000 ord_schema-0.3.75/ord_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-12 20:50:49.000000 ord_schema-0.3.75/ord_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 20:50:49.000000 ord_schema-0.3.75/ord_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-12 20:50:49.000000 ord_schema-0.3.75/ord_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 20:50:49.000000 ord_schema-0.3.75/ord_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:50:49.383121 ord_schema-0.3.75/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-12 20:50:36.000000 ord_schema-0.3.75/proto/dataset.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    46965 2024-04-12 20:50:36.000000 ord_schema-0.3.75/proto/reaction.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-12 20:50:36.000000 ord_schema-0.3.75/proto/test.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-12 20:50:36.000000 ord_schema-0.3.75/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 20:50:49.387121 ord_schema-0.3.75/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-12 20:50:38.000000 ord_schema-0.3.75/setup.py
```

### Comparing `ord-schema-0.3.74/LICENSE` & `ord_schema-0.3.75/LICENSE`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/PKG-INFO` & `ord_schema-0.3.75/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.74
+Version: 0.3.75
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.74/README.md` & `ord_schema-0.3.75/README.md`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/__init__.py` & `ord_schema-0.3.75/ord_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/frozen_message.py` & `ord_schema-0.3.75/ord_schema/frozen_message.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/frozen_message_test.py` & `ord_schema-0.3.75/ord_schema/frozen_message_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/logging.py` & `ord_schema-0.3.75/ord_schema/logging.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/macros/__init__.py` & `ord_schema-0.3.75/ord_schema/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/macros/solutions.py` & `ord_schema-0.3.75/ord_schema/macros/solutions.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/macros/solutions_test.py` & `ord_schema-0.3.75/ord_schema/macros/solutions_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/macros/workups.py` & `ord_schema-0.3.75/ord_schema/macros/workups.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/message_helpers.py` & `ord_schema-0.3.75/ord_schema/message_helpers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/message_helpers_test.py` & `ord_schema-0.3.75/ord_schema/message_helpers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/orm/__init__.py` & `ord_schema-0.3.75/ord_schema/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/orm/conftest.py` & `ord_schema-0.3.75/ord_schema/orm/conftest.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/orm/database.py` & `ord_schema-0.3.75/ord_schema/orm/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import time
 import os
 from unittest.mock import patch
 
 from sqlalchemy import cast, delete, func, select, text, update
 from sqlalchemy.dialects.postgresql import insert
 from sqlalchemy.engine import Engine
-from sqlalchemy.exc import OperationalError
+from sqlalchemy.exc import OperationalError, NotSupportedError
 from sqlalchemy.orm import Session
 
 from ord_schema.logging import get_logger
 from ord_schema.orm.mappers import Base, Mappers, from_proto
 from ord_schema.orm.rdkit_mappers import CString, FingerprintType, RDKitMol, RDKitReaction
 from ord_schema.proto import dataset_pb2
 
@@ -51,22 +51,24 @@
         try:
             connection.execute(text("CREATE EXTENSION IF NOT EXISTS tsm_system_rows"))  # For random sampling.
         except OperationalError:
             logger.warning("tsm_system_rows cartridge is not installed; random sampling will be disabled")
     with engine.begin() as connection:
         connection.execute(text("CREATE SCHEMA IF NOT EXISTS ord"))
         connection.execute(text("CREATE SCHEMA IF NOT EXISTS rdkit"))
-        try:
+    try:
+        with engine.begin() as connection:
             # NOTE(skearnes): The RDKit PostgreSQL extension works best in the public schema.
             connection.execute(text("CREATE EXTENSION IF NOT EXISTS rdkit"))
-            rdkit_cartridge = True
-        except OperationalError:
+        rdkit_cartridge = True
+    except (OperationalError, NotSupportedError):
+        with engine.begin() as connection:
             logger.warning("RDKit PostgreSQL cartridge is not installed; structure search will be disabled")
             connection.execute(text("CREATE EXTENSION IF NOT EXISTS btree_gist"))
-            rdkit_cartridge = False
+        rdkit_cartridge = False
     with patch.dict(os.environ, {"ORD_POSTGRES_RDKIT": "1" if rdkit_cartridge else "0"}):
         Base.metadata.create_all(engine)
     return rdkit_cartridge
 
 
 def add_dataset(dataset: dataset_pb2.Dataset, session: Session) -> None:
     """Adds a dataset to the database."""
```

### Comparing `ord-schema-0.3.74/ord_schema/orm/database_test.py` & `ord_schema-0.3.75/ord_schema/orm/database_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/orm/mappers.py` & `ord_schema-0.3.75/ord_schema/orm/mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/orm/mappers_test.py` & `ord_schema-0.3.75/ord_schema/orm/mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/orm/rdkit_mappers.py` & `ord_schema-0.3.75/ord_schema/orm/rdkit_mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/proto/__init__.py` & `ord_schema-0.3.75/ord_schema/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/proto/dataset_pb2.py` & `ord_schema-0.3.75/ord_schema/proto/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/proto/dataset_pb2.pyi` & `ord_schema-0.3.75/ord_schema/proto/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/proto/dataset_pb2_test.py` & `ord_schema-0.3.75/ord_schema/proto/dataset_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/proto/reaction_pb2.py` & `ord_schema-0.3.75/ord_schema/proto/reaction_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/proto/reaction_pb2.pyi` & `ord_schema-0.3.75/ord_schema/proto/reaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/proto/reaction_pb2_test.py` & `ord_schema-0.3.75/ord_schema/proto/reaction_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/proto/test_pb2.py` & `ord_schema-0.3.75/ord_schema/proto/test_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/resolvers.py` & `ord_schema-0.3.75/ord_schema/resolvers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/resolvers_test.py` & `ord_schema-0.3.75/ord_schema/resolvers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/scripts/__init__.py` & `ord_schema-0.3.75/ord_schema/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/scripts/build_dataset.py` & `ord_schema-0.3.75/ord_schema/scripts/build_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/scripts/build_dataset_test.py` & `ord_schema-0.3.75/ord_schema/scripts/build_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/scripts/check_pb.py` & `ord_schema-0.3.75/ord_schema/scripts/check_pb.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/scripts/check_pb_test.py` & `ord_schema-0.3.75/ord_schema/scripts/check_pb_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/scripts/enumerate_dataset.py` & `ord_schema-0.3.75/ord_schema/scripts/enumerate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/scripts/enumerate_dataset_test.py` & `ord_schema-0.3.75/ord_schema/scripts/enumerate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/scripts/parse_uspto.py` & `ord_schema-0.3.75/ord_schema/scripts/parse_uspto.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/scripts/process_dataset.py` & `ord_schema-0.3.75/ord_schema/scripts/process_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/scripts/process_dataset_test.py` & `ord_schema-0.3.75/ord_schema/scripts/process_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/scripts/validate_dataset.py` & `ord_schema-0.3.75/ord_schema/scripts/validate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/scripts/validate_dataset_test.py` & `ord_schema-0.3.75/ord_schema/scripts/validate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/templating.py` & `ord_schema-0.3.75/ord_schema/templating.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/templating_test.py` & `ord_schema-0.3.75/ord_schema/templating_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/units.py` & `ord_schema-0.3.75/ord_schema/units.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/units_test.py` & `ord_schema-0.3.75/ord_schema/units_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/updates.py` & `ord_schema-0.3.75/ord_schema/updates.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/updates_test.py` & `ord_schema-0.3.75/ord_schema/updates_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/validations.py` & `ord_schema-0.3.75/ord_schema/validations.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema/validations_test.py` & `ord_schema-0.3.75/ord_schema/validations_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema.egg-info/PKG-INFO` & `ord_schema-0.3.75/ord_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.74
+Version: 0.3.75
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.74/ord_schema.egg-info/SOURCES.txt` & `ord_schema-0.3.75/ord_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/ord_schema.egg-info/requires.txt` & `ord_schema-0.3.75/ord_schema.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/proto/dataset.proto` & `ord_schema-0.3.75/proto/dataset.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/proto/reaction.proto` & `ord_schema-0.3.75/proto/reaction.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/proto/test.proto` & `ord_schema-0.3.75/proto/test.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.74/setup.py` & `ord_schema-0.3.75/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 with open("README.md") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="ord-schema",
-    version="0.3.74",
+    version="0.3.75",
     description="Schema for the Open Reaction Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Open-Reaction-Database/ord-schema",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

