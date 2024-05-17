# Comparing `tmp/datapools-1.0.52.tar.gz` & `tmp/datapools-1.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-1.0.52.tar", last modified: Wed May 15 15:14:40 2024, max compression
+gzip compressed data, was "datapools-1.0.53.tar", last modified: Fri May 17 15:05:14 2024, max compression
```

## Comparing `datapools-1.0.52.tar` & `datapools-1.0.53.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.635722 datapools-1.0.52/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 15:14:28.000000 datapools-1.0.52/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    18164 2024-05-15 15:14:28.000000 datapools-1.0.52/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-15 15:14:28.000000 datapools-1.0.52/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 15:14:28.000000 datapools-1.0.52/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-15 15:14:40.635722 datapools-1.0.52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-15 15:14:28.000000 datapools-1.0.52/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.623722 datapools-1.0.52/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.623722 datapools-1.0.52/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.623722 datapools-1.0.52/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/common/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.627722 datapools-1.0.52/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.627722 datapools-1.0.52/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/common/tasks_db/redis.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.627722 datapools-1.0.52/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/producer/base_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.627722 datapools-1.0.52/datapools/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.627722 datapools-1.0.52/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.627722 datapools-1.0.52/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.627722 datapools-1.0.52/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.627722 datapools-1.0.52/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.627722 datapools-1.0.52/datapools/worker/plugins/deutsche_welle/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/deutsche_welle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.631722 datapools-1.0.52/datapools/worker/plugins/freesound_org/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/freesound_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/freesound_org/freesound_org.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.631722 datapools-1.0.52/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.631722 datapools-1.0.52/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.631722 datapools-1.0.52/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.631722 datapools-1.0.52/datapools/worker/plugins/theguardian/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/theguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/theguardian/theguardian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.631722 datapools-1.0.52/datapools/worker/plugins/washingtonpost/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/washingtonpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/washingtonpost/washingtonpost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.631722 datapools-1.0.52/datapools/worker/plugins/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/wikipedia/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.631722 datapools-1.0.52/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16563 2024-05-15 15:14:28.000000 datapools-1.0.52/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.631722 datapools-1.0.52/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-15 15:14:40.000000 datapools-1.0.52/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-15 15:14:40.000000 datapools-1.0.52/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:14:40.000000 datapools-1.0.52/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 15:14:40.000000 datapools-1.0.52/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-15 15:14:40.000000 datapools-1.0.52/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 15:14:40.000000 datapools-1.0.52/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:14:40.635722 datapools-1.0.52/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-15 15:14:28.000000 datapools-1.0.52/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:40.631722 datapools-1.0.52/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:14:28.000000 datapools-1.0.52/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-15 15:14:28.000000 datapools-1.0.52/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-15 15:14:28.000000 datapools-1.0.52/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.985175 datapools-1.0.53/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-17 15:04:58.000000 datapools-1.0.53/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    18645 2024-05-17 15:04:58.000000 datapools-1.0.53/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-17 15:04:58.000000 datapools-1.0.53/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-17 15:04:58.000000 datapools-1.0.53/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-17 15:05:14.985175 datapools-1.0.53/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-17 15:04:58.000000 datapools-1.0.53/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.973175 datapools-1.0.53/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.973175 datapools-1.0.53/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.977175 datapools-1.0.53/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.977175 datapools-1.0.53/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.977175 datapools-1.0.53/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.977175 datapools-1.0.53/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.977175 datapools-1.0.53/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.977175 datapools-1.0.53/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.977175 datapools-1.0.53/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/freesound_org/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/freesound_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/freesound_org/freesound_org.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.981175 datapools-1.0.53/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.985175 datapools-1.0.53/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16563 2024-05-17 15:04:58.000000 datapools-1.0.53/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.985175 datapools-1.0.53/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-17 15:05:14.000000 datapools-1.0.53/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-17 15:05:14.000000 datapools-1.0.53/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:05:14.000000 datapools-1.0.53/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-17 15:05:14.000000 datapools-1.0.53/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 15:05:14.000000 datapools-1.0.53/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 15:05:14.000000 datapools-1.0.53/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 15:05:14.985175 datapools-1.0.53/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-17 15:04:58.000000 datapools-1.0.53/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:05:14.985175 datapools-1.0.53/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 15:04:58.000000 datapools-1.0.53/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-17 15:04:58.000000 datapools-1.0.53/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-17 15:04:58.000000 datapools-1.0.53/tests/test_base.py
```

### Comparing `datapools-1.0.52/HISTORY.md` & `datapools-1.0.53/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 Changelog
 =========
 
 
+(unreleased)
+------------
+- . [sergpsu]
+- . [sergpsu]
+- Scheduler backend api errors processing. [sergpsu]
+- BackendAPI stubborn mode. [sergpsu]
+- Merge remote-tracking branch 'origin/master' into sergpsu-fixes.
+  [sergpsu]
+- Merge pull request #69 from torrentsai/sergpsu-fixes. [S]
+
+  f8king linter
+- Merge pull request #68 from torrentsai/sergpsu-fixes. [S]
+
+  Redis pubsub on crawler session
+
+
+1.0.52 (2024-05-15)
+-------------------
+- Release: version 1.0.52 🚀 [sergpsu]
+
+
 1.0.51 (2024-05-15)
 -------------------
 - Release: version 1.0.51 🚀 [sergpsu]
 - Linter. [sergpsu]
 - Linter. [sergpsu]
```

### Comparing `datapools-1.0.52/LICENSE` & `datapools-1.0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/PKG-INFO` & `datapools-1.0.53/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.52
+Version: 1.0.53
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.52/README.md` & `datapools-1.0.53/README.md`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/api.py` & `datapools-1.0.53/datapools/api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/cli.py` & `datapools-1.0.53/datapools/cli.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/common/backend_api.py` & `datapools-1.0.53/datapools/common/backend_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -63,7 +63,8 @@
                 if r.status_code == 200:
                     return r.json()
                 else:
                     logger.error(f"Non 200 http response {r=}")
                     raise BackendAPIException("non 200 response")
             except httpx.ConnectError as e:
                 logger.error(f"Failed connect Backend API server: {e}")
+                raise BackendAPIException("Failed connect backend")
```

### Comparing `datapools-1.0.52/datapools/common/queues/__init__.py` & `datapools-1.0.53/datapools/common/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/common/queues/rabbitmq.py` & `datapools-1.0.53/datapools/common/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/common/queues/types.py` & `datapools-1.0.53/datapools/common/queues/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/common/session_manager.py` & `datapools-1.0.53/datapools/common/session_manager.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/common/stoppable.py` & `datapools-1.0.53/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/common/storage/base_storage.py` & `datapools-1.0.53/datapools/common/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/common/storage/file_storage.py` & `datapools-1.0.53/datapools/common/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/common/tasks_db/redis.py.bak` & `datapools-1.0.53/datapools/common/tasks_db/redis.py.bak`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.53/datapools/common/tasks_db/tasks_db.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/common/types.py` & `datapools-1.0.53/datapools/common/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/producer/base_producer.py` & `datapools-1.0.53/datapools/producer/base_producer.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
                         else:
                             raise Exception(f"!!!!!!!!!!!!!!! BUG: unexpected {message=} {qm=}")
 
                         await self.eval_queue.mark_done(message)
                     except BackendAPIException as e:
                         logger.error("Catched BackendAPIException")
                         logger.error(traceback.format_exc())
-                        await self.eval_queue.reject(message, requeue=False)
+                        await self.eval_queue.reject(message)
                         await asyncio.sleep(5)
                     except Exception as e:
                         logger.error("Catched Exception")
                         logger.error(traceback.format_exc())
                         await self.eval_queue.reject(message, requeue=False)
 
         except Exception as e:
```

### Comparing `datapools-1.0.52/datapools/scheduler/scheduler.py` & `datapools-1.0.53/datapools/scheduler/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 
 # import json
 # import time
 import traceback
 from typing import Optional
 
-from ..common.backend_api import BackendAPI
+from ..common.backend_api import BackendAPI, BackendAPIException
 from ..common.logger import logger
 from ..common.queues import GenericQueue, QueueMessage, QueueMessageType, QueueRole
 
 # from .common.tasks_db import Hash
 # from .common.tasks_db.redis import RedisTasksDB
 from ..common.session_manager import SessionManager
 from ..common.stoppable import Stoppable
@@ -239,17 +239,23 @@
                         elif qm.type == QueueMessageType.Report:
                             await self._set_task_status(qm.session_id, qm.data)
                         elif qm.type == QueueMessageType.Stop:
                             logger.info("scheduler: got stop from worker")
                             self.stop_task_processed.set()
                         else:
                             logger.error(f"Unsupported QueueMessage {qm=}")
+                        await self.reports_queue.mark_done(message)
 
-                    except Exception as e:
-                        logger.error(f"Failed decode {message.body=} {message=}")
+                    except BackendAPIException as e:
+                        logger.error("Catched BackendAPIException")
                         logger.error(traceback.format_exc())
+                        await self.reports_queue.reject(message)
+                        await asyncio.sleep(5)
 
-                    await self.reports_queue.mark_done(message)
+                    except Exception as e:
+                        logger.error(traceback.format_exc())
+                        await self.reports_queue.reject(message, requeue=False)
+                        await asyncio.sleep(5)
 
         except Exception as e:
             logger.error(f"!!!!!!! Exception in CrawlerScheduler::reports_loop() {e}")
             logger.error(traceback.format_exc())
```

### Comparing `datapools-1.0.52/datapools/worker/plugins/base_plugin.py` & `datapools-1.0.53/datapools/worker/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.53/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/worker/plugins/default/default.py` & `datapools-1.0.53/datapools/worker/plugins/default/default.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/worker/plugins/deutsche_welle/deutsche_welle.py` & `datapools-1.0.53/datapools/worker/plugins/deutsche_welle/deutsche_welle.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/worker/plugins/freesound_org/freesound_org.py` & `datapools-1.0.53/datapools/worker/plugins/freesound_org/freesound_org.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.53/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/worker/plugins/imageshack/imageshack.py` & `datapools-1.0.53/datapools/worker/plugins/imageshack/imageshack.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.53/datapools/worker/plugins/s3/s3.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/worker/plugins/theguardian/theguardian.py` & `datapools-1.0.53/datapools/worker/plugins/theguardian/theguardian.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/worker/plugins/washingtonpost/washingtonpost.py` & `datapools-1.0.53/datapools/worker/plugins/washingtonpost/washingtonpost.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/worker/plugins/wikipedia/wikipedia.py` & `datapools-1.0.53/datapools/worker/plugins/wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/worker/plugins/youtube_channel/youtube_channel.py` & `datapools-1.0.53/datapools/worker/plugins/youtube_channel/youtube_channel.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools/worker/worker.py` & `datapools-1.0.53/datapools/worker/worker.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/datapools.egg-info/PKG-INFO` & `datapools-1.0.53/datapools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.52
+Version: 1.0.53
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.52/datapools.egg-info/SOURCES.txt` & `datapools-1.0.53/datapools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/setup.py` & `datapools-1.0.53/setup.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.52/tests/test_base.py` & `datapools-1.0.53/tests/test_base.py`

 * *Files identical despite different names*

