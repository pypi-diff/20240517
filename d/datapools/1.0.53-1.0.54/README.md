# Comparing `tmp/datapools-1.0.53.tar.gz` & `tmp/datapools-1.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-1.0.53.tar", last modified: Fri May 17 15:05:14 2024, max compression
+gzip compressed data, was "datapools-1.0.54.tar", last modified: Fri May 17 19:41:21 2024, max compression
```

## Comparing `datapools-1.0.53.tar` & `datapools-1.0.54.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.985175 datapools-1.0.53/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-17 15:04:58.000000 datapools-1.0.53/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    18645 2024-05-17 15:04:58.000000 datapools-1.0.53/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-17 15:04:58.000000 datapools-1.0.53/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-17 15:04:58.000000 datapools-1.0.53/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-17 15:05:14.985175 datapools-1.0.53/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-17 15:04:58.000000 datapools-1.0.53/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.973175 datapools-1.0.53/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.973175 datapools-1.0.53/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.977175 datapools-1.0.53/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.977175 datapools-1.0.53/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.977175 datapools-1.0.53/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/tasks_db/redis.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.977175 datapools-1.0.53/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/producer/base_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.977175 datapools-1.0.53/datapools/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.977175 datapools-1.0.53/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.977175 datapools-1.0.53/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/deutsche_welle/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/deutsche_welle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/freesound_org/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/freesound_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/freesound_org/freesound_org.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/theguardian/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/theguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/theguardian/theguardian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/washingtonpost/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/washingtonpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/washingtonpost/washingtonpost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/wikipedia/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.985175 datapools-1.0.53/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16563 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.985175 datapools-1.0.53/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-17 15:05:14.000000 datapools-1.0.53/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-17 15:05:14.000000 datapools-1.0.53/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:05:14.000000 datapools-1.0.53/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-17 15:05:14.000000 datapools-1.0.53/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 15:05:14.000000 datapools-1.0.53/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 15:05:14.000000 datapools-1.0.53/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 15:05:14.985175 datapools-1.0.53/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-17 15:04:58.000000 datapools-1.0.53/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.985175 datapools-1.0.53/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 15:04:58.000000 datapools-1.0.53/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-17 15:04:58.000000 datapools-1.0.53/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-17 15:04:58.000000 datapools-1.0.53/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.060544 datapools-1.0.54/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-17 19:41:12.000000 datapools-1.0.54/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-05-17 19:41:12.000000 datapools-1.0.54/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-17 19:41:12.000000 datapools-1.0.54/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-17 19:41:12.000000 datapools-1.0.54/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-17 19:41:21.060544 datapools-1.0.54/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-17 19:41:12.000000 datapools-1.0.54/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.048544 datapools-1.0.54/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.052544 datapools-1.0.54/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.052544 datapools-1.0.54/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.052544 datapools-1.0.54/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.052544 datapools-1.0.54/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.052544 datapools-1.0.54/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.052544 datapools-1.0.54/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.056544 datapools-1.0.54/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.056544 datapools-1.0.54/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.056544 datapools-1.0.54/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.056544 datapools-1.0.54/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.056544 datapools-1.0.54/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.056544 datapools-1.0.54/datapools/worker/plugins/freesound_org/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/freesound_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/freesound_org/freesound_org.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.056544 datapools-1.0.54/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.056544 datapools-1.0.54/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.056544 datapools-1.0.54/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.056544 datapools-1.0.54/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.056544 datapools-1.0.54/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.060544 datapools-1.0.54/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.060544 datapools-1.0.54/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16563 2024-05-17 19:41:12.000000 datapools-1.0.54/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.060544 datapools-1.0.54/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-17 19:41:21.000000 datapools-1.0.54/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-17 19:41:21.000000 datapools-1.0.54/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:41:21.000000 datapools-1.0.54/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-17 19:41:21.000000 datapools-1.0.54/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 19:41:21.000000 datapools-1.0.54/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 19:41:21.000000 datapools-1.0.54/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:41:21.060544 datapools-1.0.54/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-17 19:41:12.000000 datapools-1.0.54/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:21.060544 datapools-1.0.54/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:41:12.000000 datapools-1.0.54/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-17 19:41:12.000000 datapools-1.0.54/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-17 19:41:12.000000 datapools-1.0.54/tests/test_base.py
```

### Comparing `datapools-1.0.53/HISTORY.md` & `datapools-1.0.54/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Scheduler loop stabilization. [sergpsu]
+
+
+1.0.53 (2024-05-17)
+-------------------
+- Release: version 1.0.53 🚀 [sergpsu]
 - . [sergpsu]
 - . [sergpsu]
 - Scheduler backend api errors processing. [sergpsu]
 - BackendAPI stubborn mode. [sergpsu]
 - Merge remote-tracking branch 'origin/master' into sergpsu-fixes.
   [sergpsu]
 - Merge pull request #69 from torrentsai/sergpsu-fixes. [S]
```

### Comparing `datapools-1.0.53/LICENSE` & `datapools-1.0.54/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/PKG-INFO` & `datapools-1.0.54/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.53
+Version: 1.0.54
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.53/README.md` & `datapools-1.0.54/README.md`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/api.py` & `datapools-1.0.54/datapools/api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/cli.py` & `datapools-1.0.54/datapools/cli.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/common/backend_api.py` & `datapools-1.0.54/datapools/common/backend_api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/common/queues/__init__.py` & `datapools-1.0.54/datapools/common/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/common/queues/rabbitmq.py` & `datapools-1.0.54/datapools/common/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/common/queues/types.py` & `datapools-1.0.54/datapools/common/queues/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/common/session_manager.py` & `datapools-1.0.54/datapools/common/session_manager.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/common/stoppable.py` & `datapools-1.0.54/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/common/storage/base_storage.py` & `datapools-1.0.54/datapools/common/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/common/storage/file_storage.py` & `datapools-1.0.54/datapools/common/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/common/tasks_db/redis.py.bak` & `datapools-1.0.54/datapools/common/tasks_db/redis.py.bak`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.54/datapools/common/tasks_db/tasks_db.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/common/types.py` & `datapools-1.0.54/datapools/common/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/producer/base_producer.py` & `datapools-1.0.54/datapools/producer/base_producer.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/scheduler/scheduler.py` & `datapools-1.0.54/datapools/scheduler/scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -198,27 +198,36 @@
             while not await self.is_stopped():
                 if self.session_manager.is_ready():
                     hints = await self._get_hints()
                     if hints is not None:
                         for hint in hints:
                             logger.info(f"got hint: {hint}")
 
-                            if await self._add_task(hint.get("session_id"), hint):
-                                if "id" in hint:
-                                    await self.api.set_hint_url_status(
-                                        hint["id"], CrawlerHintURLStatus.Processing, hint["session_id"]
-                                    )
-                            else:
-                                logger.error("failed add task, REJECTING")
-                                if "id" in hint:
-                                    await self.api.set_hint_url_status(
-                                        hint["id"],
-                                        CrawlerHintURLStatus.Rejected,
-                                    )
-                                    self.session_manager.remove(hint["session_id"])
+                            # catching set_hint_url_status BackendAPIException: if backend fails then trying again and again
+                            while not await self.is_stopped():
+                                if await self._add_task(hint.get("session_id"), hint):
+                                    try:
+                                        if "id" in hint:
+                                            await self.api.set_hint_url_status(
+                                                hint["id"], CrawlerHintURLStatus.Processing, hint["session_id"]
+                                            )
+                                        else:
+                                            logger.error("failed add task, REJECTING")
+                                            if "id" in hint:
+                                                await self.api.set_hint_url_status(
+                                                    hint["id"],
+                                                    CrawlerHintURLStatus.Rejected,
+                                                )
+                                                self.session_manager.remove(hint["session_id"])
+                                        break
+                                    except BackendAPIException as e:
+                                        logger.error("Catched BackendAPIException")
+                                        logger.error(traceback.format_exc())
+                                        await asyncio.sleep(5)
+                                        # ..and loop again
 
                     if not self.cfg.CLI_MODE:
                         await asyncio.sleep(self.cfg.BACKEND_HINTS_PERIOD)
                 else:
                     await asyncio.sleep(1)
         except Exception as e:
             logger.error(f"!!!!!!! Exception in CrawlerScheduler::hints_loop() {e}")
```

### Comparing `datapools-1.0.53/datapools/worker/plugins/base_plugin.py` & `datapools-1.0.54/datapools/worker/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.54/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/worker/plugins/default/default.py` & `datapools-1.0.54/datapools/worker/plugins/default/default.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/worker/plugins/deutsche_welle/deutsche_welle.py` & `datapools-1.0.54/datapools/worker/plugins/deutsche_welle/deutsche_welle.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/worker/plugins/freesound_org/freesound_org.py` & `datapools-1.0.54/datapools/worker/plugins/freesound_org/freesound_org.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.54/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/worker/plugins/imageshack/imageshack.py` & `datapools-1.0.54/datapools/worker/plugins/imageshack/imageshack.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.54/datapools/worker/plugins/s3/s3.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/worker/plugins/theguardian/theguardian.py` & `datapools-1.0.54/datapools/worker/plugins/theguardian/theguardian.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/worker/plugins/washingtonpost/washingtonpost.py` & `datapools-1.0.54/datapools/worker/plugins/washingtonpost/washingtonpost.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/worker/plugins/wikipedia/wikipedia.py` & `datapools-1.0.54/datapools/worker/plugins/wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/worker/plugins/youtube_channel/youtube_channel.py` & `datapools-1.0.54/datapools/worker/plugins/youtube_channel/youtube_channel.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools/worker/worker.py` & `datapools-1.0.54/datapools/worker/worker.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/datapools.egg-info/PKG-INFO` & `datapools-1.0.54/datapools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.53
+Version: 1.0.54
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.53/datapools.egg-info/SOURCES.txt` & `datapools-1.0.54/datapools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/setup.py` & `datapools-1.0.54/setup.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.53/tests/test_base.py` & `datapools-1.0.54/tests/test_base.py`

 * *Files identical despite different names*

