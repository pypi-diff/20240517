# Comparing `tmp/myqueue-24.1.0.tar.gz` & `tmp/myqueue-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myqueue-24.1.0.tar", last modified: Tue Jan  2 13:19:09 2024, max compression
+gzip compressed data, was "myqueue-24.5.0.tar", last modified: Mon May  6 06:37:38 2024, max compression
```

## Comparing `myqueue-24.1.0.tar` & `myqueue-24.5.0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2024-01-02 13:19:09.920953 myqueue-24.1.0/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      120 2021-06-29 08:22:33.000000 myqueue-24.1.0/.gitignore
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      893 2023-07-31 09:31:00.000000 myqueue-24.1.0/.gitlab-ci.yml
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      417 2021-06-29 08:22:33.000000 myqueue-24.1.0/.mailmap
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      199 2024-01-02 12:19:36.000000 myqueue-24.1.0/.readthedocs.yml
--rw-r--r--   0 jensj     (1000) jensj     (1000)      117 2019-12-20 07:21:33.000000 myqueue-24.1.0/CHANGELOG.rst
--rw-r--r--   0 jensj     (1000) jensj     (1000)      118 2019-12-20 07:21:33.000000 myqueue-24.1.0/CONTRIBUTING.rst
--rw-r--r--   0 jensj     (1000) jensj     (1000)    35147 2019-11-07 08:34:48.000000 myqueue-24.1.0/LICENSE
--rw-r--r--   0 jensj     (1000) jensj     (1000)       27 2019-11-07 09:17:12.000000 myqueue-24.1.0/MANIFEST.in
--rw-r--r--   0 jensj     (1000) jensj     (1000)    45828 2024-01-02 13:19:09.920953 myqueue-24.1.0/PKG-INFO
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4281 2024-01-02 12:19:36.000000 myqueue-24.1.0/README.rst
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2024-01-02 13:19:09.912953 myqueue-24.1.0/docs/
--rw-r--r--   0 jensj     (1000) jensj     (1000)      580 2018-11-29 09:27:16.000000 myqueue-24.1.0/docs/Makefile
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2024-01-02 13:19:09.912953 myqueue-24.1.0/docs/_static/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3290 2022-03-24 11:07:34.000000 myqueue-24.1.0/docs/_static/favicon.ico
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8061 2022-03-24 11:07:34.000000 myqueue-24.1.0/docs/_static/logo.svg
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1938 2022-11-07 09:53:00.000000 myqueue-24.1.0/docs/api.rst
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    17375 2024-01-02 12:19:36.000000 myqueue-24.1.0/docs/cli.rst
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5990 2024-01-02 12:19:36.000000 myqueue-24.1.0/docs/conf.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6426 2022-11-14 10:09:07.000000 myqueue-24.1.0/docs/configuration.rst
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      949 2024-01-02 12:19:36.000000 myqueue-24.1.0/docs/development.rst
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7563 2022-11-14 10:09:07.000000 myqueue-24.1.0/docs/documentation.rst
--rw-r--r--   0 jensj     (1000) jensj     (1000)      267 2019-12-19 08:34:44.000000 myqueue-24.1.0/docs/example_config.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1965 2022-11-03 07:40:03.000000 myqueue-24.1.0/docs/howitworks.rst
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      865 2022-11-03 07:40:03.000000 myqueue-24.1.0/docs/howto.rst
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1615 2023-07-31 09:31:00.000000 myqueue-24.1.0/docs/index.rst
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      488 2024-01-02 12:19:36.000000 myqueue-24.1.0/docs/installation.rst
--rw-r--r--   0 jensj     (1000) jensj     (1000)     5469 2020-01-30 08:22:44.000000 myqueue-24.1.0/docs/paper.bib
--rw-r--r--   0 jensj     (1000) jensj     (1000)     5263 2020-01-30 08:22:44.000000 myqueue-24.1.0/docs/paper.md
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2024-01-02 13:19:09.912953 myqueue-24.1.0/docs/prime/
--rw-r--r--   0 jensj     (1000) jensj     (1000)      190 2019-02-05 13:24:32.000000 myqueue-24.1.0/docs/prime/check.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      398 2022-03-24 11:07:29.000000 myqueue-24.1.0/docs/prime/factor.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      164 2021-06-29 08:22:33.000000 myqueue-24.1.0/docs/prime/workflow.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4252 2022-11-03 07:40:03.000000 myqueue-24.1.0/docs/quickstart.rst
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    10138 2024-01-02 13:18:16.000000 myqueue-24.1.0/docs/releasenotes.rst
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       28 2024-01-02 12:19:36.000000 myqueue-24.1.0/docs/requirements.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    13693 2022-11-07 09:53:00.000000 myqueue-24.1.0/docs/workflows.rst
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      158 2022-11-14 10:09:07.000000 myqueue-24.1.0/mypy.ini
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2024-01-02 13:19:09.912953 myqueue-24.1.0/myqueue/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      791 2024-01-02 12:19:36.000000 myqueue-24.1.0/myqueue/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      112 2020-10-26 11:54:40.000000 myqueue-24.1.0/myqueue/__main__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4428 2022-11-07 09:53:00.000000 myqueue-24.1.0/myqueue/caching.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    23093 2024-01-02 12:19:36.000000 myqueue-24.1.0/myqueue/cli.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7603 2022-11-15 08:19:16.000000 myqueue-24.1.0/myqueue/commands.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4471 2024-01-02 12:19:36.000000 myqueue-24.1.0/myqueue/complete.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6766 2023-07-31 09:31:00.000000 myqueue-24.1.0/myqueue/config.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4419 2022-11-07 09:52:56.000000 myqueue-24.1.0/myqueue/daemon.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4148 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/email.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1445 2024-01-02 13:14:56.000000 myqueue-24.1.0/myqueue/errors.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1425 2022-11-14 10:09:07.000000 myqueue-24.1.0/myqueue/hold.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4238 2024-01-02 12:19:36.000000 myqueue-24.1.0/myqueue/info.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1726 2024-01-02 13:14:56.000000 myqueue-24.1.0/myqueue/kick.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1146 2023-07-31 09:31:00.000000 myqueue-24.1.0/myqueue/migration.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1514 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/modify.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4118 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/pretty.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2022-10-13 08:16:27.000000 myqueue-24.1.0/myqueue/py.typed
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    13614 2023-07-31 09:31:00.000000 myqueue-24.1.0/myqueue/queue.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1089 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/remove.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8180 2023-07-31 09:31:00.000000 myqueue-24.1.0/myqueue/resources.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      976 2022-11-14 10:09:07.000000 myqueue-24.1.0/myqueue/resubmit.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2024-01-02 13:19:09.916953 myqueue-24.1.0/myqueue/schedulers/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      963 2022-10-13 08:16:27.000000 myqueue-24.1.0/myqueue/schedulers/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8033 2022-11-28 13:30:30.000000 myqueue-24.1.0/myqueue/schedulers/local.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4152 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/schedulers/lsf.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2975 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/schedulers/pbs.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1975 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/schedulers/scheduler.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4417 2023-07-31 09:31:00.000000 myqueue-24.1.0/myqueue/schedulers/slurm.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3959 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/schedulers/test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2190 2023-07-31 09:31:00.000000 myqueue-24.1.0/myqueue/selection.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2940 2022-10-13 08:16:27.000000 myqueue-24.1.0/myqueue/states.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3922 2022-12-01 11:32:09.000000 myqueue-24.1.0/myqueue/submitting.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      756 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/syncronize.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    13876 2022-11-28 13:38:43.000000 myqueue-24.1.0/myqueue/task.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2024-01-02 13:19:09.916953 myqueue-24.1.0/myqueue/test/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      440 2022-04-11 07:59:32.000000 myqueue-24.1.0/myqueue/test/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1430 2022-11-07 09:53:00.000000 myqueue-24.1.0/myqueue/test/caching_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      285 2022-03-24 11:07:29.000000 myqueue-24.1.0/myqueue/test/command_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1358 2023-07-31 09:31:00.000000 myqueue-24.1.0/myqueue/test/complete_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      523 2022-03-24 11:07:29.000000 myqueue-24.1.0/myqueue/test/config_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1858 2022-11-14 10:09:07.000000 myqueue-24.1.0/myqueue/test/conftest.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      803 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/test/daemon_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      635 2023-07-31 09:31:00.000000 myqueue-24.1.0/myqueue/test/error_msg_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      650 2022-11-08 11:54:44.000000 myqueue-24.1.0/myqueue/test/flow1.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      421 2022-03-24 11:07:29.000000 myqueue-24.1.0/myqueue/test/flow2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      787 2022-03-24 11:07:29.000000 myqueue-24.1.0/myqueue/test/hello.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2250 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/test/local_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      309 2022-03-24 11:07:29.000000 myqueue-24.1.0/myqueue/test/lock_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      215 2022-03-24 11:07:29.000000 myqueue-24.1.0/myqueue/test/mod.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2810 2022-11-08 11:54:44.000000 myqueue-24.1.0/myqueue/test/more_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5439 2024-01-02 13:14:56.000000 myqueue-24.1.0/myqueue/test/mq_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      740 2022-11-28 13:38:43.000000 myqueue-24.1.0/myqueue/test/name_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      953 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/test/notify_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      271 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/test/pp_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      305 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/test/queue_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      235 2022-03-24 11:07:29.000000 myqueue-24.1.0/myqueue/test/resources_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4215 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/test/rst_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2196 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/test/scheduler_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      459 2022-11-03 07:40:03.000000 myqueue-24.1.0/myqueue/test/sqlite_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1617 2022-11-14 10:09:07.000000 myqueue-24.1.0/myqueue/test/task_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      455 2022-03-24 11:07:29.000000 myqueue-24.1.0/myqueue/test/utils_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5605 2023-07-31 09:31:00.000000 myqueue-24.1.0/myqueue/test/workflow_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     9194 2023-07-31 09:31:00.000000 myqueue-24.1.0/myqueue/utils.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    18585 2022-12-01 11:32:09.000000 myqueue-24.1.0/myqueue/workflow.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2024-01-02 13:19:09.916953 myqueue-24.1.0/myqueue.egg-info/
--rw-r--r--   0 jensj     (1000) jensj     (1000)    45828 2024-01-02 13:19:09.000000 myqueue-24.1.0/myqueue.egg-info/PKG-INFO
--rw-r--r--   0 jensj     (1000) jensj     (1000)     2234 2024-01-02 13:19:09.000000 myqueue-24.1.0/myqueue.egg-info/SOURCES.txt
--rw-r--r--   0 jensj     (1000) jensj     (1000)        1 2024-01-02 13:19:09.000000 myqueue-24.1.0/myqueue.egg-info/dependency_links.txt
--rw-r--r--   0 jensj     (1000) jensj     (1000)       40 2024-01-02 13:19:09.000000 myqueue-24.1.0/myqueue.egg-info/entry_points.txt
--rw-r--r--   0 jensj     (1000) jensj     (1000)       47 2020-01-17 10:53:06.000000 myqueue-24.1.0/myqueue.egg-info/pbr.json
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       46 2024-01-02 13:19:09.000000 myqueue-24.1.0/myqueue.egg-info/requires.txt
--rw-r--r--   0 jensj     (1000) jensj     (1000)        8 2024-01-02 13:19:09.000000 myqueue-24.1.0/myqueue.egg-info/top_level.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1098 2024-01-02 13:15:34.000000 myqueue-24.1.0/pyproject.toml
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      100 2021-06-29 08:22:33.000000 myqueue-24.1.0/pytest.ini
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       38 2024-01-02 13:19:09.920953 myqueue-24.1.0/setup.cfg
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2024-05-06 06:37:38.805702 myqueue-24.5.0/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      120 2021-06-29 08:22:33.000000 myqueue-24.5.0/.gitignore
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      893 2023-07-31 09:31:00.000000 myqueue-24.5.0/.gitlab-ci.yml
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      417 2021-06-29 08:22:33.000000 myqueue-24.5.0/.mailmap
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      199 2024-01-02 12:19:36.000000 myqueue-24.5.0/.readthedocs.yml
+-rw-r--r--   0 jensj     (1000) jensj     (1000)      117 2019-12-20 07:21:33.000000 myqueue-24.5.0/CHANGELOG.rst
+-rw-r--r--   0 jensj     (1000) jensj     (1000)      118 2019-12-20 07:21:33.000000 myqueue-24.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 jensj     (1000) jensj     (1000)    35147 2019-11-07 08:34:48.000000 myqueue-24.5.0/LICENSE
+-rw-r--r--   0 jensj     (1000) jensj     (1000)       27 2019-11-07 09:17:12.000000 myqueue-24.5.0/MANIFEST.in
+-rw-r--r--   0 jensj     (1000) jensj     (1000)    45828 2024-05-06 06:37:38.805702 myqueue-24.5.0/PKG-INFO
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4281 2024-01-02 12:19:36.000000 myqueue-24.5.0/README.rst
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2024-05-06 06:37:38.797702 myqueue-24.5.0/docs/
+-rw-r--r--   0 jensj     (1000) jensj     (1000)      580 2018-11-29 09:27:16.000000 myqueue-24.5.0/docs/Makefile
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2024-05-06 06:37:38.797702 myqueue-24.5.0/docs/_static/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3290 2022-03-24 11:07:34.000000 myqueue-24.5.0/docs/_static/favicon.ico
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8061 2022-03-24 11:07:34.000000 myqueue-24.5.0/docs/_static/logo.svg
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1938 2022-11-07 09:53:00.000000 myqueue-24.5.0/docs/api.rst
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    18149 2024-05-06 06:33:49.000000 myqueue-24.5.0/docs/cli.rst
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5990 2024-01-02 12:19:36.000000 myqueue-24.5.0/docs/conf.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6754 2024-05-06 06:33:49.000000 myqueue-24.5.0/docs/configuration.rst
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      949 2024-01-02 12:19:36.000000 myqueue-24.5.0/docs/development.rst
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7563 2024-05-06 06:33:44.000000 myqueue-24.5.0/docs/documentation.rst
+-rw-r--r--   0 jensj     (1000) jensj     (1000)      267 2019-12-19 08:34:44.000000 myqueue-24.5.0/docs/example_config.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1965 2022-11-03 07:40:03.000000 myqueue-24.5.0/docs/howitworks.rst
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      865 2022-11-03 07:40:03.000000 myqueue-24.5.0/docs/howto.rst
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1615 2023-07-31 09:31:00.000000 myqueue-24.5.0/docs/index.rst
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      488 2024-01-02 12:19:36.000000 myqueue-24.5.0/docs/installation.rst
+-rw-r--r--   0 jensj     (1000) jensj     (1000)     5469 2020-01-30 08:22:44.000000 myqueue-24.5.0/docs/paper.bib
+-rw-r--r--   0 jensj     (1000) jensj     (1000)     5263 2020-01-30 08:22:44.000000 myqueue-24.5.0/docs/paper.md
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2024-05-06 06:37:38.797702 myqueue-24.5.0/docs/prime/
+-rw-r--r--   0 jensj     (1000) jensj     (1000)      190 2019-02-05 13:24:32.000000 myqueue-24.5.0/docs/prime/check.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      398 2022-03-24 11:07:29.000000 myqueue-24.5.0/docs/prime/factor.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      164 2021-06-29 08:22:33.000000 myqueue-24.5.0/docs/prime/workflow.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4252 2022-11-03 07:40:03.000000 myqueue-24.5.0/docs/quickstart.rst
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    10432 2024-05-06 06:36:54.000000 myqueue-24.5.0/docs/releasenotes.rst
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       28 2024-01-02 12:19:36.000000 myqueue-24.5.0/docs/requirements.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    13693 2022-11-07 09:53:00.000000 myqueue-24.5.0/docs/workflows.rst
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      158 2022-11-14 10:09:07.000000 myqueue-24.5.0/mypy.ini
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2024-05-06 06:37:38.801702 myqueue-24.5.0/myqueue/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      791 2024-01-02 12:19:36.000000 myqueue-24.5.0/myqueue/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      112 2020-10-26 11:54:40.000000 myqueue-24.5.0/myqueue/__main__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4428 2022-11-07 09:53:00.000000 myqueue-24.5.0/myqueue/caching.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    23485 2024-05-06 06:33:44.000000 myqueue-24.5.0/myqueue/cli.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7603 2022-11-15 08:19:16.000000 myqueue-24.5.0/myqueue/commands.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4471 2024-01-02 12:19:36.000000 myqueue-24.5.0/myqueue/complete.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6878 2024-05-06 06:33:49.000000 myqueue-24.5.0/myqueue/config.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4419 2022-11-07 09:52:56.000000 myqueue-24.5.0/myqueue/daemon.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4148 2022-11-03 07:40:03.000000 myqueue-24.5.0/myqueue/email.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1445 2024-01-02 13:14:56.000000 myqueue-24.5.0/myqueue/errors.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1425 2022-11-14 10:09:07.000000 myqueue-24.5.0/myqueue/hold.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4238 2024-01-02 12:19:36.000000 myqueue-24.5.0/myqueue/info.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1726 2024-01-02 13:14:56.000000 myqueue-24.5.0/myqueue/kick.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1146 2023-07-31 09:31:00.000000 myqueue-24.5.0/myqueue/migration.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1514 2022-11-03 07:40:03.000000 myqueue-24.5.0/myqueue/modify.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4118 2022-11-03 07:40:03.000000 myqueue-24.5.0/myqueue/pretty.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2022-10-13 08:16:27.000000 myqueue-24.5.0/myqueue/py.typed
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    13614 2023-07-31 09:31:00.000000 myqueue-24.5.0/myqueue/queue.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1089 2022-11-03 07:40:03.000000 myqueue-24.5.0/myqueue/remove.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8391 2024-05-06 06:33:44.000000 myqueue-24.5.0/myqueue/resources.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      976 2022-11-14 10:09:07.000000 myqueue-24.5.0/myqueue/resubmit.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2024-05-06 06:37:38.805702 myqueue-24.5.0/myqueue/schedulers/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      963 2022-10-13 08:16:27.000000 myqueue-24.5.0/myqueue/schedulers/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8033 2022-11-28 13:30:30.000000 myqueue-24.5.0/myqueue/schedulers/local.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4185 2024-01-24 15:26:55.000000 myqueue-24.5.0/myqueue/schedulers/lsf.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3008 2024-01-24 15:26:55.000000 myqueue-24.5.0/myqueue/schedulers/pbs.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1975 2022-11-03 07:40:03.000000 myqueue-24.5.0/myqueue/schedulers/scheduler.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4669 2024-05-06 06:33:49.000000 myqueue-24.5.0/myqueue/schedulers/slurm.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3959 2022-11-03 07:40:03.000000 myqueue-24.5.0/myqueue/schedulers/test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2190 2023-07-31 09:31:00.000000 myqueue-24.5.0/myqueue/selection.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2940 2022-10-13 08:16:27.000000 myqueue-24.5.0/myqueue/states.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3922 2022-12-01 11:32:09.000000 myqueue-24.5.0/myqueue/submitting.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      756 2022-11-03 07:40:03.000000 myqueue-24.5.0/myqueue/syncronize.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    13876 2022-11-28 13:38:43.000000 myqueue-24.5.0/myqueue/task.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2024-05-06 06:37:38.805702 myqueue-24.5.0/myqueue/test/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      440 2022-04-11 07:59:32.000000 myqueue-24.5.0/myqueue/test/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1430 2022-11-07 09:53:00.000000 myqueue-24.5.0/myqueue/test/caching_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      285 2022-03-24 11:07:29.000000 myqueue-24.5.0/myqueue/test/command_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1358 2023-07-31 09:31:00.000000 myqueue-24.5.0/myqueue/test/complete_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      523 2022-03-24 11:07:29.000000 myqueue-24.5.0/myqueue/test/config_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1858 2022-11-14 10:09:07.000000 myqueue-24.5.0/myqueue/test/conftest.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      803 2022-11-03 07:40:03.000000 myqueue-24.5.0/myqueue/test/daemon_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      635 2023-07-31 09:31:00.000000 myqueue-24.5.0/myqueue/test/error_msg_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      650 2022-11-08 11:54:44.000000 myqueue-24.5.0/myqueue/test/flow1.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      421 2022-03-24 11:07:29.000000 myqueue-24.5.0/myqueue/test/flow2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      787 2022-03-24 11:07:29.000000 myqueue-24.5.0/myqueue/test/hello.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2250 2022-11-03 07:40:03.000000 myqueue-24.5.0/myqueue/test/local_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      309 2022-03-24 11:07:29.000000 myqueue-24.5.0/myqueue/test/lock_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      215 2022-03-24 11:07:29.000000 myqueue-24.5.0/myqueue/test/mod.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2810 2022-11-08 11:54:44.000000 myqueue-24.5.0/myqueue/test/more_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5439 2024-01-02 13:14:56.000000 myqueue-24.5.0/myqueue/test/mq_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      740 2022-11-28 13:38:43.000000 myqueue-24.5.0/myqueue/test/name_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      953 2022-11-03 07:40:03.000000 myqueue-24.5.0/myqueue/test/notify_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      271 2022-11-03 07:40:03.000000 myqueue-24.5.0/myqueue/test/pp_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      305 2022-11-03 07:40:03.000000 myqueue-24.5.0/myqueue/test/queue_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      235 2022-03-24 11:07:29.000000 myqueue-24.5.0/myqueue/test/resources_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4215 2022-11-03 07:40:03.000000 myqueue-24.5.0/myqueue/test/rst_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2196 2022-11-03 07:40:03.000000 myqueue-24.5.0/myqueue/test/scheduler_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      459 2022-11-03 07:40:03.000000 myqueue-24.5.0/myqueue/test/sqlite_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1617 2022-11-14 10:09:07.000000 myqueue-24.5.0/myqueue/test/task_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      455 2022-03-24 11:07:29.000000 myqueue-24.5.0/myqueue/test/utils_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5605 2023-07-31 09:31:00.000000 myqueue-24.5.0/myqueue/test/workflow_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     9194 2023-07-31 09:31:00.000000 myqueue-24.5.0/myqueue/utils.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    18585 2022-12-01 11:32:09.000000 myqueue-24.5.0/myqueue/workflow.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2024-05-06 06:37:38.805702 myqueue-24.5.0/myqueue.egg-info/
+-rw-r--r--   0 jensj     (1000) jensj     (1000)    45828 2024-05-06 06:37:38.000000 myqueue-24.5.0/myqueue.egg-info/PKG-INFO
+-rw-r--r--   0 jensj     (1000) jensj     (1000)     2234 2024-05-06 06:37:38.000000 myqueue-24.5.0/myqueue.egg-info/SOURCES.txt
+-rw-r--r--   0 jensj     (1000) jensj     (1000)        1 2024-05-06 06:37:38.000000 myqueue-24.5.0/myqueue.egg-info/dependency_links.txt
+-rw-r--r--   0 jensj     (1000) jensj     (1000)       40 2024-05-06 06:37:38.000000 myqueue-24.5.0/myqueue.egg-info/entry_points.txt
+-rw-r--r--   0 jensj     (1000) jensj     (1000)       47 2020-01-17 10:53:06.000000 myqueue-24.5.0/myqueue.egg-info/pbr.json
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       46 2024-05-06 06:37:38.000000 myqueue-24.5.0/myqueue.egg-info/requires.txt
+-rw-r--r--   0 jensj     (1000) jensj     (1000)        8 2024-05-06 06:37:38.000000 myqueue-24.5.0/myqueue.egg-info/top_level.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1098 2024-05-06 06:36:04.000000 myqueue-24.5.0/pyproject.toml
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      100 2021-06-29 08:22:33.000000 myqueue-24.5.0/pytest.ini
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       38 2024-05-06 06:37:38.805702 myqueue-24.5.0/setup.cfg
```

### Comparing `myqueue-24.1.0/.gitlab-ci.yml` & `myqueue-24.5.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/LICENSE` & `myqueue-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/PKG-INFO` & `myqueue-24.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myqueue
-Version: 24.1.0
+Version: 24.5.0
 Summary: Frontend for SLURM/LSF/PBS
 Maintainer-email: Jens Jørgen Mortensen <jjmo@dtu.dk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myqueue-24.1.0/README.rst` & `myqueue-24.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/docs/Makefile` & `myqueue-24.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/docs/_static/favicon.ico` & `myqueue-24.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/docs/_static/logo.svg` & `myqueue-24.5.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/docs/api.rst` & `myqueue-24.5.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/docs/cli.rst` & `myqueue-24.5.0/docs/cli.rst`

 * *Files 4% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
 .. _submit:
 
 Submit: Submit task(s) to queue
 -------------------------------
 
 usage: mq submit [-h] [-d DEPENDENCIES] [-n NAME] [--restart N]
-                 [--max-tasks MAX_TASKS] [-R RESOURCES] [-w]
+                 [--max-tasks MAX_TASKS] [-R c[:p][:n]:t[:w]] [-w]
                  [-X EXTRA_SCHEDULER_ARGS] [-z] [-v] [-q] [-T]
                  task [folder ...]
 
 Submit task(s) to queue.
 
 Example::
 
@@ -151,19 +151,24 @@
   -n NAME, --name NAME  Name used for task.
   --restart N           Restart N times if task times out or runs out of
                         memory. Time-limit will be doubled for a timed out
                         task and number of cores will be increased to the next
                         number of nodes for a task that runs out of memory.
   --max-tasks MAX_TASKS
                         Maximum number of tasks to submit.
-  -R RESOURCES, --resources RESOURCES
-                        Examples: "8:1h", 8 cores for 1 hour. Use "m" for
-                        minutes, "h" for hours and "d" for days. "16:1:30m":
-                        16 cores, 1 process, half an hour. "1:xeon40:5m": 1
-                        core on "xeon40" for 5 minutes.
+  -R c[:p][:n]:t[:w], --resources c[:p][:n]:t[:w]
+                        Where c=cores, p=processes, n=nodename, t=tmax and
+                        w=weight. Number of cores and tmax must always be
+                        specified. Examples: "8:1h", 8 cores for 1 hour. Use
+                        "m" for minutes, "h" for hours and "d" for days.
+                        "16:1:30m": 16 cores, 1 process, half an hour.
+                        "40:xeon40:5m": 40 cores on "xeon40" for 5 minutes.
+                        "40:1:xeon40:5m": 40 cores and 1 process on "xeon40"
+                        for 5 minutes. "40:1:xeon40:5m:0.5": same as previous,
+                        but with a weight of 0.5.
   -w, --workflow        Write <task-name>.state file when task has finished.
   -X EXTRA_SCHEDULER_ARGS, --extra-scheduler-args EXTRA_SCHEDULER_ARGS
                         Extra arguments for scheudler. Example: -X bla-bla.
                         For arguments that start with a dash, leave out the
                         space: -X--gres=gpu:4 or -X=--gres=gpu:4. Can be used
                         multiple times.
   -z, --dry-run         Show what will happen without doing anything.
@@ -173,36 +178,41 @@
 
 
 .. _resubmit:
 
 Resubmit: Resubmit done, failed or timed-out tasks
 --------------------------------------------------
 
-usage: mq resubmit [-h] [--keep] [-R RESOURCES] [-w] [-X EXTRA_SCHEDULER_ARGS]
-                   [-s qhrdFCTMaA] [-i ID] [-n NAME] [-e ERROR] [-z] [-v] [-q]
-                   [-T] [-r]
+usage: mq resubmit [-h] [--keep] [-R c[:p][:n]:t[:w]] [-w]
+                   [-X EXTRA_SCHEDULER_ARGS] [-s qhrdFCTMaA] [-i ID] [-n NAME]
+                   [-e ERROR] [-z] [-v] [-q] [-T] [-r]
                    [folder ...]
 
 Resubmit done, failed or timed-out tasks.
 
 Example::
 
     $ mq resubmit -i 4321  # resubmit job with id=4321
 
 folder:
     Task-folder. Use --recursive (or -r) to include subfolders.
 
 options:
   -h, --help            show this help message and exit
   --keep                Do not remove old tasks.
-  -R RESOURCES, --resources RESOURCES
-                        Examples: "8:1h", 8 cores for 1 hour. Use "m" for
-                        minutes, "h" for hours and "d" for days. "16:1:30m":
-                        16 cores, 1 process, half an hour. "1:xeon40:5m": 1
-                        core on "xeon40" for 5 minutes.
+  -R c[:p][:n]:t[:w], --resources c[:p][:n]:t[:w]
+                        Where c=cores, p=processes, n=nodename, t=tmax and
+                        w=weight. Number of cores and tmax must always be
+                        specified. Examples: "8:1h", 8 cores for 1 hour. Use
+                        "m" for minutes, "h" for hours and "d" for days.
+                        "16:1:30m": 16 cores, 1 process, half an hour.
+                        "40:xeon40:5m": 40 cores on "xeon40" for 5 minutes.
+                        "40:1:xeon40:5m": 40 cores and 1 process on "xeon40"
+                        for 5 minutes. "40:1:xeon40:5m:0.5": same as previous,
+                        but with a weight of 0.5.
   -w, --workflow        Write <task-name>.state file when task has finished.
   -X EXTRA_SCHEDULER_ARGS, --extra-scheduler-args EXTRA_SCHEDULER_ARGS
                         Extra arguments for scheudler. Example: -X bla-bla.
                         For arguments that start with a dash, leave out the
                         space: -X--gres=gpu:4 or -X=--gres=gpu:4. Can be used
                         multiple times.
   -s qhrdFCTMaA, --states qhrdFCTMaA
```

### Comparing `myqueue-24.1.0/docs/conf.py` & `myqueue-24.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/docs/configuration.rst` & `myqueue-24.5.0/docs/configuration.rst`

 * *Files 9% similar despite different names*

```diff
@@ -46,14 +46,18 @@
      - :ref:`mpiexec`
      - ``str``
      - ``'mpiexec'``
    * - ``parallel_python``
      - :ref:`parallel_python`
      - ``str``
      - ``'python3'``
+   * - ``serial_python``
+     - :ref:`serial_python`
+     - ``str``
+     - ``'python3'``
    * - ``extra_args``
      - :ref:`extra_args`
      - ``list[str]``
      - ``[]``
    * - ``maximum_total_task_weight``
      - :ref:`task_weight`
      - ``float``
@@ -182,14 +186,24 @@
 For MPI4PY_, you don't need an MPI-enabled interpreter.
 
 .. _MPI4PY: https://mpi4py.readthedocs.io/en/stable/index.html
 .. _ASAP: https://wiki.fysik.dtu.dk/asap
 .. _GPAW: https://wiki.fysik.dtu.dk/gpaw
 
 
+.. _serial_python:
+
+Serial Python interpreter
+=========================
+
+By defaul, ``python3`` is used as the Python interpreter for serial jobs.
+Use the ``serial_python`` configuration variable if you want to set it to
+something else.
+
+
 .. _extra_args:
 
 Extra arguments for submit command
 ==================================
 
 Add extra arguments to the ``sbatch``, ``qsub`` or ``bsub`` command.
 Example::
```

### Comparing `myqueue-24.1.0/docs/development.rst` & `myqueue-24.5.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/docs/documentation.rst` & `myqueue-24.5.0/docs/documentation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -129,24 +129,24 @@
 .. _resources:
 
 Resources
 =========
 
 A resource specification has the form::
 
-    cores[:nodename][:processes]:tmax[:weight]
+    cores[:processes][:nodename]:tmax[:weight]
 
 * ``cores``: Number of cores to reserve.
 
-* ``nodename``: Node-name
-  (defaults to best match in :ref:`the list of node-types <nodes>`).
-
 * ``processes``: Number of MPI processes to start
   (defaults to number of cores).
 
+* ``nodename``: Node-name
+  (defaults to best match in :ref:`the list of node-types <nodes>`).
+
 * ``tmax``: Maximum time (use *s*, *m*, *h* and *d* for seconds, minutes,
   hours and days respectively).
 
 * ``weight``: weight of a task.  Can be used to limit the number of
   simultaneously running tasks.  See :ref:`task_weight`.
   Defaults to 0.
```

### Comparing `myqueue-24.1.0/docs/howitworks.rst` & `myqueue-24.5.0/docs/howitworks.rst`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/docs/howto.rst` & `myqueue-24.5.0/docs/howto.rst`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/docs/index.rst` & `myqueue-24.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/docs/paper.bib` & `myqueue-24.5.0/docs/paper.bib`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/docs/paper.md` & `myqueue-24.5.0/docs/paper.md`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/docs/quickstart.rst` & `myqueue-24.5.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/docs/releasenotes.rst` & `myqueue-24.5.0/docs/releasenotes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,24 @@
 
 Next release
 ============
 
 * ...
 
 
+Version 24.5.0
+==============
+
+* SLURM jobs will now be submitted with ``--cpus-per-task`` set to the correct
+  value.
+* The ``MYQUEUE_TASK_ID`` environment variable will now be set to
+  the task ID so that running tasks can inspect it.
+* New configuration variable for :ref:`serial_python`.
+
+
 Version 24.1.0
 ==============
 
 * Drop support for Python 3.7.
 * Move from ``setup.py`` to ``pyproject.toml``.
 * The :ref:`resubmit <resubmit>` command will now remove the old task.
   Use ``--keep`` to get the old behavior.
```

### Comparing `myqueue-24.1.0/docs/workflows.rst` & `myqueue-24.5.0/docs/workflows.rst`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/__init__.py` & `myqueue-24.5.0/myqueue/__init__.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/caching.py` & `myqueue-24.5.0/myqueue/caching.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/cli.py` & `myqueue-24.5.0/myqueue/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,19 +237,26 @@
 
         if cmd == 'remove':
             a('-f', '--force', action='store_true',
               help='Remove also workflow tasks.')
 
         if cmd in ['resubmit', 'submit']:
             a('-R', '--resources',
-              help='Examples: "8:1h", 8 cores for 1 hour. '
+              metavar='c[:p][:n]:t[:w]',
+              help='Where c=cores, p=processes, n=nodename, t=tmax and '
+              'w=weight.  Number of cores and tmax must always be specified. '
+              'Examples: "8:1h", 8 cores for 1 hour. '
               'Use "m" for minutes, '
               '"h" for hours and "d" for days. '
               '"16:1:30m": 16 cores, 1 process, half an hour. '
-              '"1:xeon40:5m":  1 core on "xeon40" for 5 minutes.')
+              '"40:xeon40:5m": 40 cores on "xeon40" for 5 minutes. '
+              '"40:1:xeon40:5m": 40 cores and 1 process on "xeon40" '
+              'for 5 minutes. '
+              '"40:1:xeon40:5m:0.5": same as previous, but with a weight '
+              'of 0.5.')
             a('-w', '--workflow', action='store_true',
               help='Write <task-name>.state file when task has finished.')
             a('-X', '--extra-scheduler-args', action='append', default=[],
               help='Extra arguments for scheudler.  Example: '
               '-X bla-bla.  For arguments that start with a dash, '
               'leave out the space: -X--gres=gpu:4 or -X=--gres=gpu:4. '
               'Can be used multiple times.')
```

### Comparing `myqueue-24.1.0/myqueue/commands.py` & `myqueue-24.5.0/myqueue/commands.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/complete.py` & `myqueue-24.5.0/myqueue/complete.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/config.py` & `myqueue-24.5.0/myqueue/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,30 @@
 from pathlib import Path
 from typing import Any
 
 
 class Configuration:
     def __init__(self,
                  scheduler: str,
+                 *,
                  nodes: list[tuple[str, dict[str, Any]]] = None,
+                 serial_python: str = 'python3',
                  parallel_python: str = 'python3',
                  mpiexec: str = 'mpiexec',
                  extra_args: list[str] = None,
                  maximum_total_task_weight: float = inf,
                  default_task_weight: float = 0.0,
                  notifications: dict[str, str] = None,
                  home: Path = None):
         """Configuration object.
 
         """
         self.scheduler = scheduler
         self.nodes = nodes or []
+        self.serial_python = serial_python
         self.parallel_python = parallel_python
         self.mpiexec = mpiexec
         self.extra_args = extra_args or []
         self.maximum_total_task_weight = maximum_total_task_weight
         self.default_task_weight = default_task_weight
         self.notifications = notifications or {}
         self.home = home or Path.cwd()
```

### Comparing `myqueue-24.1.0/myqueue/daemon.py` & `myqueue-24.5.0/myqueue/daemon.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/email.py` & `myqueue-24.5.0/myqueue/email.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/errors.py` & `myqueue-24.5.0/myqueue/errors.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/hold.py` & `myqueue-24.5.0/myqueue/hold.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/info.py` & `myqueue-24.5.0/myqueue/info.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/kick.py` & `myqueue-24.5.0/myqueue/kick.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/migration.py` & `myqueue-24.5.0/myqueue/migration.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/modify.py` & `myqueue-24.5.0/myqueue/modify.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/pretty.py` & `myqueue-24.5.0/myqueue/pretty.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/queue.py` & `myqueue-24.5.0/myqueue/queue.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/remove.py` & `myqueue-24.5.0/myqueue/remove.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/resources.py` & `myqueue-24.5.0/myqueue/resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,18 @@
         self.nodename = nodename
         self.tmax = tmax or 600  # seconds
         self.weight = weight
 
         if processes == 0:
             self.processes = self.cores
         else:
+            if processes > self.cores:
+                raise ValueError(
+                    'Bad resource string: Number of processes '
+                    f'bigger than number of cores!  See {RESOURCES_URL}')
             self.processes = processes
 
     def set_default_weight(self, weight: float) -> None:
         if self.weight == -1.0:
             self.weight = weight
 
     @staticmethod
```

### Comparing `myqueue-24.1.0/myqueue/resubmit.py` & `myqueue-24.5.0/myqueue/resubmit.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/schedulers/__init__.py` & `myqueue-24.5.0/myqueue/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/schedulers/local.py` & `myqueue-24.5.0/myqueue/schedulers/local.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/schedulers/lsf.py` & `myqueue-24.5.0/myqueue/schedulers/lsf.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,16 +46,16 @@
             cmd = 'mpiexec ' + cmd.replace('python3',
                                            self.config.parallel_python)
 
         home = self.config.home
 
         script = (
             '#!/bin/bash -l\n'
-            'id=$LSB_JOBID\n'
-            f'mq={home}/.myqueue/lsf-$id\n')
+            'export MYQUEUE_TASK_ID=$LSB_JOBID\n'
+            f'mq={home}/.myqueue/lsf-$MYQUEUE_TASK_ID\n')
 
         script += self.get_venv_activation_line()
 
         script += (
             '(touch $mq-0 && \\\n'
             f' cd {str(task.folder)!r} && \\\n'
             f' {cmd} && \\\n'
```

### Comparing `myqueue-24.1.0/myqueue/schedulers/pbs.py` & `myqueue-24.5.0/myqueue/schedulers/pbs.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 
         script = '#!/bin/bash -l\n'
 
         script += self.get_venv_activation_line()
 
         script += (
             '#!/bin/bash -l\n'
-            'id=${PBS_JOBID%.*}\n'
-            f'mq={home}/.myqueue/pbs-$id\n'
+            'export MYQUEUE_TASK_ID=${PBS_JOBID%.*}\n'
+            f'mq={home}/.myqueue/pbs-$MYQUEUE_TASK_ID\n'
             f'(touch $mq-0 && cd {task.folder} && {cmd} && touch $mq-1) || '
             'touch $mq-2\n')
 
         if dry_run:
             print(qsub, script)
             return 1
```

### Comparing `myqueue-24.1.0/myqueue/schedulers/scheduler.py` & `myqueue-24.5.0/myqueue/schedulers/scheduler.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/schedulers/slurm.py` & `myqueue-24.5.0/myqueue/schedulers/slurm.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,23 @@
     def submit(self,
                task: Task,
                dry_run: bool = False,
                verbose: bool = False) -> int:
         nodelist = self.config.nodes
         nodes, nodename, nodedct = task.resources.select(nodelist)
 
+        ntasks = task.resources.processes
+        cpus_per_task = task.resources.cores // ntasks
         name = task.cmd.short_name
         sbatch = ['sbatch',
                   f'--partition={nodename}',
                   f'--job-name={name}',
                   f'--time={ceil(task.resources.tmax / 60)}',
-                  f'--ntasks={task.resources.cores}',
+                  f'--ntasks={ntasks}',
+                  f'--cpus-per-task={cpus_per_task}',
                   f'--nodes={nodes}',
                   f'--chdir={task.folder}',
                   f'--output={name}.%j.out',
                   f'--error={name}.%j.err']
 
         extra_args = self.config.extra_args + nodedct.get('extra_args', [])
         sbatch += extra_args
@@ -40,27 +43,29 @@
             if 'OMP_NUM_THREADS' not in os.environ:
                 env.append(('OMP_NUM_THREADS', '1'))
             mpiexec = self.config.mpiexec
             if 'mpiargs' in nodedct:
                 mpiexec += ' ' + nodedct['mpiargs']
             cmd = mpiexec + ' ' + cmd.replace('python3',
                                               self.config.parallel_python)
+        else:
+            cmd = cmd.replace('python3', self.config.serial_python)
 
         # Use bash for the script
         script = '#!/bin/bash -l\n'
 
         # Add environment variables
         if len(env) > 0:
             script += '\n'.join(f'export {name}={val}' for name, val in env)
             script += '\n'
 
         home = self.config.home
         script += (
-            'id=$SLURM_JOB_ID\n'
-            f'mq={home}/.myqueue/slurm-$id\n')
+            'export MYQUEUE_TASK_ID=$SLURM_JOB_ID\n'
+            f'mq={home}/.myqueue/slurm-$MYQUEUE_TASK_ID\n')
 
         script += self.get_venv_activation_line()
 
         script += (
             '(touch $mq-0 && \\\n'
             f' cd {str(task.folder)!r} && \\\n'
             f' {cmd} && \\\n'
```

### Comparing `myqueue-24.1.0/myqueue/schedulers/test.py` & `myqueue-24.5.0/myqueue/schedulers/test.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/selection.py` & `myqueue-24.5.0/myqueue/selection.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/states.py` & `myqueue-24.5.0/myqueue/states.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/submitting.py` & `myqueue-24.5.0/myqueue/submitting.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/syncronize.py` & `myqueue-24.5.0/myqueue/syncronize.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/task.py` & `myqueue-24.5.0/myqueue/task.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/caching_test.py` & `myqueue-24.5.0/myqueue/test/caching_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/complete_test.py` & `myqueue-24.5.0/myqueue/test/complete_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/config_test.py` & `myqueue-24.5.0/myqueue/test/config_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/conftest.py` & `myqueue-24.5.0/myqueue/test/conftest.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/daemon_test.py` & `myqueue-24.5.0/myqueue/test/daemon_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/error_msg_test.py` & `myqueue-24.5.0/myqueue/test/error_msg_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/flow1.py` & `myqueue-24.5.0/myqueue/test/flow1.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/hello.py` & `myqueue-24.5.0/myqueue/test/hello.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/local_test.py` & `myqueue-24.5.0/myqueue/test/local_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/more_test.py` & `myqueue-24.5.0/myqueue/test/more_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/mq_test.py` & `myqueue-24.5.0/myqueue/test/mq_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/name_test.py` & `myqueue-24.5.0/myqueue/test/name_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/notify_test.py` & `myqueue-24.5.0/myqueue/test/notify_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/rst_test.py` & `myqueue-24.5.0/myqueue/test/rst_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/scheduler_test.py` & `myqueue-24.5.0/myqueue/test/scheduler_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/task_test.py` & `myqueue-24.5.0/myqueue/test/task_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/test/workflow_test.py` & `myqueue-24.5.0/myqueue/test/workflow_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/utils.py` & `myqueue-24.5.0/myqueue/utils.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue/workflow.py` & `myqueue-24.5.0/myqueue/workflow.py`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/myqueue.egg-info/PKG-INFO` & `myqueue-24.5.0/myqueue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myqueue
-Version: 24.1.0
+Version: 24.5.0
 Summary: Frontend for SLURM/LSF/PBS
 Maintainer-email: Jens Jørgen Mortensen <jjmo@dtu.dk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myqueue-24.1.0/myqueue.egg-info/SOURCES.txt` & `myqueue-24.5.0/myqueue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myqueue-24.1.0/pyproject.toml` & `myqueue-24.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "myqueue"
-version = "24.1.0"
+version = "24.5.0"
 description = "Frontend for SLURM/LSF/PBS"
 
 readme = "README.rst"
 license = {file = "LICENSE"}
 dependencies = ["rich", "networkx", "typing_extensions"]
 requires-python = ">=3.8"
 maintainers = [{name = "Jens Jørgen Mortensen", email = "jjmo@dtu.dk"}]
```

