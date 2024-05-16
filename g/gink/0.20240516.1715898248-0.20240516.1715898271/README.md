# Comparing `tmp/gink-0.20240516.1715898248.tar.gz` & `tmp/gink-0.20240516.1715898271.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gink-0.20240516.1715898248.tar", last modified: Thu May 16 22:24:14 2024, max compression
+gzip compressed data, was "gink-0.20240516.1715898271.tar", last modified: Thu May 16 22:24:37 2024, max compression
```

## Comparing `gink-0.20240516.1715898248.tar` & `gink-0.20240516.1715898271.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:14.211816 gink-0.20240516.1715898248/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-16 22:24:14.211816 gink-0.20240516.1715898248/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:14.195816 gink-0.20240516.1715898248/gink/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5932 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:14.199816 gink-0.20240516.1715898248/gink/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:08.000000 gink-0.20240516.1715898248/gink/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-16 22:24:08.000000 gink-0.20240516.1715898248/gink/builders/behavior_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-16 22:24:08.000000 gink-0.20240516.1715898248/gink/builders/bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-16 22:24:08.000000 gink-0.20240516.1715898248/gink/builders/change_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-16 22:24:08.000000 gink-0.20240516.1715898248/gink/builders/claim_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-16 22:24:08.000000 gink-0.20240516.1715898248/gink/builders/clearance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-16 22:24:08.000000 gink-0.20240516.1715898248/gink/builders/container_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-16 22:24:08.000000 gink-0.20240516.1715898248/gink/builders/entry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-16 22:24:08.000000 gink-0.20240516.1715898248/gink/builders/key_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-16 22:24:08.000000 gink-0.20240516.1715898248/gink/builders/log_file_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-16 22:24:08.000000 gink-0.20240516.1715898248/gink/builders/movement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-16 22:24:08.000000 gink-0.20240516.1715898248/gink/builders/muid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-16 22:24:08.000000 gink-0.20240516.1715898248/gink/builders/pair_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-16 22:24:08.000000 gink-0.20240516.1715898248/gink/builders/sync_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-05-16 22:24:08.000000 gink-0.20240516.1715898248/gink/builders/value_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:14.207816 gink-0.20240516.1715898248/gink/impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11596 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/abstract_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/addressable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/bundle_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/bundle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    21568 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13163 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/container.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19822 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/deferred.py
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11828 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)    56473 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/lmdb_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/log_backed_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    21698 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/selectable_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/websocket_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/wsgi_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/impl/wsgi_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:14.211816 gink-0.20240516.1715898248/gink/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_change_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_code_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_demo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_logbackedstore.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_websocket_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-16 22:24:06.000000 gink-0.20240516.1715898248/gink/tests/test_wsgi_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:14.211816 gink-0.20240516.1715898248/gink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-16 22:24:14.000000 gink-0.20240516.1715898248/gink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-16 22:24:14.000000 gink-0.20240516.1715898248/gink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:24:14.000000 gink-0.20240516.1715898248/gink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 22:24:14.000000 gink-0.20240516.1715898248/gink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 22:24:14.000000 gink-0.20240516.1715898248/gink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:24:14.211816 gink-0.20240516.1715898248/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-16 22:24:08.000000 gink-0.20240516.1715898248/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:37.420683 gink-0.20240516.1715898271/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-16 22:24:23.000000 gink-0.20240516.1715898271/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-16 22:24:37.420683 gink-0.20240516.1715898271/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:37.404682 gink-0.20240516.1715898271/gink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5932 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:37.408682 gink-0.20240516.1715898271/gink/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/behavior_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/change_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/claim_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/clearance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/container_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/entry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/header_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/key_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/log_file_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/movement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/muid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/pair_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/sync_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/value_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:37.416683 gink-0.20240516.1715898271/gink/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11596 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/abstract_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/addressable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/bundle_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/bundle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21568 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13163 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/container.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19740 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11828 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56480 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/lmdb_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/log_backed_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21698 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/selectable_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/wsgi_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/wsgi_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:37.420683 gink-0.20240516.1715898271/gink/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_change_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_code_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_logbackedstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_wsgi_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:37.420683 gink-0.20240516.1715898271/gink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-16 22:24:37.000000 gink-0.20240516.1715898271/gink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-16 22:24:37.000000 gink-0.20240516.1715898271/gink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:24:37.000000 gink-0.20240516.1715898271/gink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 22:24:37.000000 gink-0.20240516.1715898271/gink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 22:24:37.000000 gink-0.20240516.1715898271/gink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:24:37.420683 gink-0.20240516.1715898271/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/setup.py
```

### Comparing `gink-0.20240516.1715898248/LICENSE` & `gink-0.20240516.1715898271/LICENSE`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/PKG-INFO` & `gink-0.20240516.1715898271/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240516.1715898248
+Version: 0.20240516.1715898271
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240516.1715898248/README.md` & `gink-0.20240516.1715898271/README.md`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/__init__.py` & `gink-0.20240516.1715898271/gink/__init__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/__main__.py` & `gink-0.20240516.1715898271/gink/__main__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/builders/behavior_pb2.py` & `gink-0.20240516.1715898271/gink/builders/behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/builders/change_pb2.py` & `gink-0.20240516.1715898271/gink/builders/change_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/builders/claim_pb2.py` & `gink-0.20240516.1715898271/gink/builders/claim_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/builders/clearance_pb2.py` & `gink-0.20240516.1715898271/gink/builders/clearance_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/builders/container_pb2.py` & `gink-0.20240516.1715898271/gink/builders/container_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/builders/entry_pb2.py` & `gink-0.20240516.1715898271/gink/builders/entry_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/builders/key_pb2.py` & `gink-0.20240516.1715898271/gink/builders/key_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/builders/log_file_pb2.py` & `gink-0.20240516.1715898271/gink/builders/log_file_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/builders/movement_pb2.py` & `gink-0.20240516.1715898271/gink/builders/movement_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/builders/muid_pb2.py` & `gink-0.20240516.1715898271/gink/builders/muid_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/builders/pair_pb2.py` & `gink-0.20240516.1715898271/gink/builders/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/builders/sync_message_pb2.py` & `gink-0.20240516.1715898271/gink/builders/sync_message_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/builders/value_pb2.py` & `gink-0.20240516.1715898271/gink/builders/value_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/abstract_store.py` & `gink-0.20240516.1715898271/gink/impl/abstract_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/addressable.py` & `gink-0.20240516.1715898271/gink/impl/addressable.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/attribution.py` & `gink-0.20240516.1715898271/gink/impl/attribution.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/box.py` & `gink-0.20240516.1715898271/gink/impl/box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/builders.py` & `gink-0.20240516.1715898271/gink/impl/builders.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,64 +4,71 @@
 from google.protobuf.message import Message # type: ignore
 from enum import IntEnum
 
 from .typedefs import Medallion, MuTimestamp
 
 if TYPE_CHECKING:
 
-    class BundleBuilder(Message):
-        pass
-
 
-    class SyncMessage(Message):
-        pass
+    class HeaderBuilder(Message):
+        timestamp: int
+        medallion: int
+        previous: int
+        comment: str
+        chain_start: int
 
 
     class ChangeBuilder(Message):
         entry: EntryBuilder
         container: ContainerBuilder
         movement: MovementBuilder
 
+
+    class BundleBuilder(Message):
+        header: HeaderBuilder
+        changes: List[ChangeBuilder]
+
+    class SyncMessage(Message):
+        pass
+
+
+
     class Pair:
         left: MuidBuilder
         rite: MuidBuilder
 
+
     class EntryBuilder(Message):
         describing: MuidBuilder
         pointee: MuidBuilder
         behavior: int
         value: ValueBuilder
         container: MuidBuilder
         deletion: bool
         purge: bool
         pair: Pair
         octets: bytes
         key: KeyBuilder
         effective: int
 
-
     class ValueBuilder(Message):
         pass
 
-
     class KeyBuilder(Message):
         pass
 
-
     class ContainerBuilder(Message):
         behavior: int
 
-
     class MovementBuilder(Message):
         container: MuidBuilder
         entry: MuidBuilder
         dest: int
         purge: bool
 
-
     class ClearanceBuilder(Message):
         pass
 
     class MuidBuilder(Message):
         timestamp: MuTimestamp
         medallion: Medallion
         offset: int
@@ -72,15 +79,14 @@
         process_id: int
         claim_time: MuTimestamp
 
     class LogFileBuilder(Message):
         bundles: List[bytes]
         claims: List[ClaimBuilder]
 
-
     class Behavior(IntEnum):
         UNSPECIFIED = 0
         BOX = 1
         SEQUENCE = 2
         KEY_SET = 3
         DIRECTORY = 4
         PAIR_SET = 5
@@ -101,7 +107,8 @@
     from ..builders.bundle_pb2 import Bundle as BundleBuilder
     from ..builders.movement_pb2 import Movement as MovementBuilder
     from ..builders.clearance_pb2 import Clearance as ClearanceBuilder
     from ..builders.muid_pb2 import Muid as MuidBuilder
     from ..builders.behavior_pb2 import Behavior
     from ..builders.log_file_pb2 import LogFile as LogFileBuilder
     from ..builders.claim_pb2 import Claim as ClaimBuilder
+    from ..builders.header_pb2 import Header as HeaderBuilder
```

### Comparing `gink-0.20240516.1715898248/gink/impl/bundle_info.py` & `gink-0.20240516.1715898271/gink/impl/bundle_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 """ Contains the ChangeSetInfo class. """
 from typing import Optional
 from struct import Struct
 
-from .builders import SyncMessage, BundleBuilder
+from .builders import SyncMessage, HeaderBuilder
 from .typedefs import Medallion, MuTimestamp
 from .tuples import Chain
 
 
 class BundleInfo:
     """ Metadata about a particular change set relevant for syncing. """
     _struct = Struct(">QQQQ")
@@ -15,15 +15,15 @@
 
     timestamp: MuTimestamp
     medallion: Medallion
     chain_start: MuTimestamp
     previous: MuTimestamp
     comment: str
 
-    def __init__(self, *, builder: Optional[BundleBuilder] = None, encoded: bytes = b'\x00' * 32, **kwargs):
+    def __init__(self, *, builder: Optional[HeaderBuilder] = None, encoded: bytes = b'\x00' * 32, **kwargs):
 
         if len(encoded) < 32:
             raise ValueError("need at least 32 bytes to unpack")
         unpacked = self._struct.unpack(encoded[0:32])
         (self.timestamp, self.medallion, self.chain_start, self.previous) = unpacked
         self.comment = encoded[32:].decode()
```

### Comparing `gink-0.20240516.1715898248/gink/impl/bundle_wrapper.py` & `gink-0.20240516.1715898271/gink/impl/bundle_wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,9 +15,9 @@
         if self._bundle_builder is None:
             self._bundle_builder = BundleBuilder()
             self._bundle_builder.ParseFromString(self._bundle_bytes)
         return self._bundle_builder
 
     def get_info(self) -> BundleInfo:
         if self._bundle_info is None:
-            self._bundle_info = BundleInfo(builder=self.get_builder())
+            self._bundle_info = BundleInfo(builder=self.get_builder().header)
         return self._bundle_info
```

### Comparing `gink-0.20240516.1715898248/gink/impl/bundler.py` & `gink-0.20240516.1715898271/gink/impl/bundler.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,16 +67,16 @@
              ) -> bytes:
         """ Finalizes a bundle and serializes it. """
         # pylint: disable=maybe-no-member
         if previous is None:
             assert timestamp == chain.chain_start
         else:
             assert chain.chain_start <= previous < timestamp
-            self._bundle_builder.previous = previous  # type: ignore
-        self._bundle_builder.chain_start = chain.chain_start  # type: ignore
-        self._medallion = self._bundle_builder.medallion = chain.medallion  # type: ignore
-        self._timestamp = self._bundle_builder.timestamp = timestamp  # type: ignore
+            self._bundle_builder.header.previous = previous  # type: ignore
+        self._bundle_builder.header.chain_start = chain.chain_start  # type: ignore
+        self._medallion = self._bundle_builder.header.medallion = chain.medallion  # type: ignore
+        self._timestamp = self._bundle_builder.header.timestamp = timestamp  # type: ignore
         if self._comment:
-            self._bundle_builder.comment = self.comment  # type: ignore
+            self._bundle_builder.header.comment = self.comment  # type: ignore
         sealed = self._bundle_builder.SerializeToString()
         self._sealed = sealed
         return sealed
```

### Comparing `gink-0.20240516.1715898248/gink/impl/chain_tracker.py` & `gink-0.20240516.1715898271/gink/impl/chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/coding.py` & `gink-0.20240516.1715898271/gink/impl/coding.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/connection.py` & `gink-0.20240516.1715898271/gink/impl/connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/container.py` & `gink-0.20240516.1715898271/gink/impl/container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/database.py` & `gink-0.20240516.1715898271/gink/impl/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
             self._logger.debug("locally committed bundle: %r", info)
             return info
 
     def _on_bundle(self, bundle_bytes: bytes, bundle_info: BundleInfo) -> None:
         """ Sends a bundle either created locally or received from a peer to other peers.
         """
         outbound_message_with_bundle = SyncMessage()
-        outbound_message_with_bundle.bundle = bundle_bytes  # type: ignore
+        outbound_message_with_bundle.bundle = bundle_bytes
         for peer in self._connections:
             tracker = self._trackers.get(peer)
             if tracker is None:
                 # In this case we haven't received a greeting from the peer, and so don't want to
                 # send any bundles because it might result in gaps in their chain.
                 continue
             if tracker.has(bundle_info):
@@ -205,30 +205,30 @@
             tracker.mark_as_having(bundle_info)
         for callback in self._callbacks:
             callback(bundle_info)
 
     def _receive_data(self, sync_message: SyncMessage, from_peer: Connection):
         with self._lock:
             if sync_message.HasField("bundle"):
-                bundle_bytes = sync_message.bundle  # type: ignore # pylint: disable=maybe-no-member
+                bundle_bytes = sync_message.bundle
                 wrap = BundleWrapper(bundle_bytes)
                 info = wrap.get_info()
                 if (tracker := self._trackers.get(from_peer)):
                     tracker.mark_as_having(info)
                 self._store.apply_bundle(wrap, self._on_bundle)
                 from_peer.send(info.as_acknowledgement())
             elif sync_message.HasField("greeting"):
                 self._logger.debug("received greeting from %s", from_peer)
                 chain_tracker = ChainTracker(sync_message=sync_message)
                 self._trackers[from_peer] = chain_tracker
 
                 def callback(bundle_bytes: bytes, info: BundleInfo):
                     if not chain_tracker.has(info):
                         outgoing_builder = SyncMessage()
-                        outgoing_builder.bundle = bundle_bytes  # type: ignore
+                        outgoing_builder.bundle = bundle_bytes
                         from_peer.send(outgoing_builder)
 
                 self._store.get_bundles(callback=callback)
                 from_peer.set_replied_to_greeting()
             elif sync_message.HasField("ack"):
                 acked_info = BundleInfo.from_ack(sync_message)
                 tracker = self._trackers.get(from_peer)
```

### Comparing `gink-0.20240516.1715898248/gink/impl/deferred.py` & `gink-0.20240516.1715898271/gink/impl/deferred.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/directory.py` & `gink-0.20240516.1715898271/gink/impl/directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/graph.py` & `gink-0.20240516.1715898271/gink/impl/graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/group.py` & `gink-0.20240516.1715898271/gink/impl/group.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/key_set.py` & `gink-0.20240516.1715898271/gink/impl/key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/listener.py` & `gink-0.20240516.1715898271/gink/impl/listener.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/lmdb_store.py` & `gink-0.20240516.1715898271/gink/impl/lmdb_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -985,15 +985,15 @@
                 raise ValueError("haven't been retaining bundles that long")
             bundles_cursor = txn.cursor(self._bundles)
             data_remaining = bundles_cursor.set_range(encode_muts(since))
             while data_remaining:
                 bundle_bytes = bundles_cursor.value()
                 bundle_builder = BundleBuilder()
                 bundle_builder.ParseFromString(bundle_bytes)
-                bundle_info = BundleInfo(builder=bundle_builder)
+                bundle_info = BundleInfo(builder=bundle_builder.header)
                 callback(bundle_bytes, bundle_info)
                 data_remaining = bundles_cursor.next()
 
     def get_chain_tracker(self) -> ChainTracker:
         chain_tracker = ChainTracker()
         with self._handle.begin() as txn:
             infos_cursor = txn.cursor(self._chains)
```

### Comparing `gink-0.20240516.1715898248/gink/impl/lmdb_utilities.py` & `gink-0.20240516.1715898271/gink/impl/lmdb_utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/log_backed_store.py` & `gink-0.20240516.1715898271/gink/impl/log_backed_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/memory_store.py` & `gink-0.20240516.1715898271/gink/impl/memory_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/muid.py` & `gink-0.20240516.1715898271/gink/impl/muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/pair_map.py` & `gink-0.20240516.1715898271/gink/impl/pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/pair_set.py` & `gink-0.20240516.1715898271/gink/impl/pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/property.py` & `gink-0.20240516.1715898271/gink/impl/property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/selectable_console.py` & `gink-0.20240516.1715898271/gink/impl/selectable_console.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/sequence.py` & `gink-0.20240516.1715898271/gink/impl/sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/tuples.py` & `gink-0.20240516.1715898271/gink/impl/tuples.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/typedefs.py` & `gink-0.20240516.1715898271/gink/impl/typedefs.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/utilities.py` & `gink-0.20240516.1715898271/gink/impl/utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/watcher.py` & `gink-0.20240516.1715898271/gink/impl/watcher.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/websocket_connection.py` & `gink-0.20240516.1715898271/gink/impl/websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/wsgi_connection.py` & `gink-0.20240516.1715898271/gink/impl/wsgi_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/impl/wsgi_listener.py` & `gink-0.20240516.1715898271/gink/impl/wsgi_listener.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_box.py` & `gink-0.20240516.1715898271/gink/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_chain_tracker.py` & `gink-0.20240516.1715898271/gink/tests/test_chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_change_set_info.py` & `gink-0.20240516.1715898271/gink/tests/test_change_set_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_code_values.py` & `gink-0.20240516.1715898271/gink/tests/test_code_values.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_container.py` & `gink-0.20240516.1715898271/gink/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_database.py` & `gink-0.20240516.1715898271/gink/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_demo.py` & `gink-0.20240516.1715898271/gink/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_directory.py` & `gink-0.20240516.1715898271/gink/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_graph.py` & `gink-0.20240516.1715898271/gink/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_key_set.py` & `gink-0.20240516.1715898271/gink/tests/test_key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_lmdb_store.py` & `gink-0.20240516.1715898271/gink/tests/test_lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_logbackedstore.py` & `gink-0.20240516.1715898271/gink/tests/test_logbackedstore.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_muid.py` & `gink-0.20240516.1715898271/gink/tests/test_muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_names.py` & `gink-0.20240516.1715898271/gink/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_pair_map.py` & `gink-0.20240516.1715898271/gink/tests/test_pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_pair_set.py` & `gink-0.20240516.1715898271/gink/tests/test_pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_property.py` & `gink-0.20240516.1715898271/gink/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_role.py` & `gink-0.20240516.1715898271/gink/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_sequence.py` & `gink-0.20240516.1715898271/gink/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_store.py` & `gink-0.20240516.1715898271/gink/tests/test_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,20 +40,20 @@
             new_func.__name__ = new_name
             into_where[new_name] = new_func
 
 
 def make_empty_bundle(bundle_info: BundleInfo) -> bytes:
     """ Makes an empty change set that matches the given metadata. """
     builder = BundleBuilder()
-    builder.medallion = bundle_info.medallion  # type: ignore
-    builder.chain_start = bundle_info.chain_start  # type: ignore
-    builder.timestamp = bundle_info.timestamp  # type: ignore
-    builder.previous = bundle_info.previous  # type: ignore
+    builder.header.medallion = bundle_info.medallion  # type: ignore
+    builder.header.chain_start = bundle_info.chain_start  # type: ignore
+    builder.header.timestamp = bundle_info.timestamp  # type: ignore
+    builder.header.previous = bundle_info.previous  # type: ignore
     if bundle_info.comment:
-        builder.comment = bundle_info.comment  # type: ignore
+        builder.header.comment = bundle_info.comment  # type: ignore
     return builder.SerializeToString()  # type: ignore
 
 
 def generic_test_accepts_only_once(store_maker: StoreMaker):
     """ Ensures that the store accepts things as expected. """
     # with closing(store_maker()) as store:
     store = store_maker()
@@ -185,17 +185,19 @@
         assert tracker.has(info4)
         assert not tracker.has(info5)
 
 
 def generic_test_get_ordered_entries(store_maker: StoreMaker):
     """ makes sure that the get_ordered_entries works """
     textproto1 = """
-        medallion: 789
-        chain_start: 123
-        timestamp: 123
+        header {
+            medallion: 789
+            chain_start: 123
+            timestamp: 123
+        }
         changes {
             key: 1
             value {
                 container {
                     behavior: SEQUENCE
                 }
             }
@@ -228,18 +230,20 @@
                     container { offset: 1 }
                     value { characters: "Goodbye, World!" }
                 }
             }
         }
     """
     textproto2 = """
-        medallion: 789
-        chain_start: 123
-        timestamp: 234
-        previous: 123
+        header {
+            medallion: 789
+            chain_start: 123
+            timestamp: 234
+            previous: 123
+        }
         changes {
             key: 1
             value {
                 movement {
                     container { timestamp: 123 offset: 1 }
                     entry { timestamp: 123 offset: 2 }
                 }
@@ -309,17 +313,19 @@
         assert found[1].entry_muid == Muid(123, 789, 4)
 
 
 
 def generic_test_negative_offsets(store_maker: StoreMaker):
     """ makes sure that the get_ordered_entries works """
     textproto1 = """
-        medallion: 789
-        chain_start: 123
-        timestamp: 123
+        header {
+            medallion: 789
+            chain_start: 123
+            timestamp: 123
+        }
         changes {
             key: 1
             value {
                 container {
                     behavior: SEQUENCE
                 }
             }
```

### Comparing `gink-0.20240516.1715898248/gink/tests/test_websocket_connection.py` & `gink-0.20240516.1715898271/gink/tests/test_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink/tests/test_wsgi_server.py` & `gink-0.20240516.1715898271/gink/tests/test_wsgi_server.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898248/gink.egg-info/PKG-INFO` & `gink-0.20240516.1715898271/gink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240516.1715898248
+Version: 0.20240516.1715898271
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240516.1715898248/gink.egg-info/SOURCES.txt` & `gink-0.20240516.1715898271/gink.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 gink/builders/behavior_pb2.py
 gink/builders/bundle_pb2.py
 gink/builders/change_pb2.py
 gink/builders/claim_pb2.py
 gink/builders/clearance_pb2.py
 gink/builders/container_pb2.py
 gink/builders/entry_pb2.py
+gink/builders/header_pb2.py
 gink/builders/key_pb2.py
 gink/builders/log_file_pb2.py
 gink/builders/movement_pb2.py
 gink/builders/muid_pb2.py
 gink/builders/pair_pb2.py
 gink/builders/sync_message_pb2.py
 gink/builders/value_pb2.py
```

### Comparing `gink-0.20240516.1715898248/setup.py` & `gink-0.20240516.1715898271/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name='gink',
-    version='0.20240516.1715898248',
+    version='0.20240516.1715898271',
     description='a system for storing data structures in lmdb',
     url='https://github.com/x5e/gink',
     author='Darin McGill',
     author_email="gink@darinmcgill.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         "Intended Audience :: Developers",
```

