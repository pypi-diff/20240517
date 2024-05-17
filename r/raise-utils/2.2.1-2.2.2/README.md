# Comparing `tmp/raise_utils-2.2.1.tar.gz` & `tmp/raise_utils-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raise_utils-2.2.1.tar", last modified: Wed Mar 20 05:27:57 2024, max compression
+gzip compressed data, was "raise_utils-2.2.2.tar", last modified: Fri May 17 02:17:51 2024, max compression
```

## Comparing `raise_utils-2.2.1.tar` & `raise_utils-2.2.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-03-20 05:27:57.205926 raise_utils-2.2.1/
--rw-r--r--   0 ryedida    (501) staff       (20)    26526 2020-08-30 18:58:05.000000 raise_utils-2.2.1/LICENSE
--rw-r--r--   0 ryedida    (501) staff       (20)       68 2024-01-07 02:27:16.000000 raise_utils-2.2.1/MANIFEST.in
--rw-r--r--   0 ryedida    (501) staff       (20)     3114 2024-03-20 05:27:57.205353 raise_utils-2.2.1/PKG-INFO
--rw-r--r--   0 ryedida    (501) staff       (20)     2554 2024-01-07 02:27:35.000000 raise_utils-2.2.1/README.md
--rw-r--r--   0 ryedida    (501) staff       (20)      690 2024-03-20 05:27:17.000000 raise_utils-2.2.1/pyproject.toml
-drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-03-20 05:27:57.180111 raise_utils-2.2.1/raise_utils/
--rw-r--r--   0 ryedida    (501) staff       (20)       22 2024-03-20 05:27:03.000000 raise_utils-2.2.1/raise_utils/__init__.py
-drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-03-20 05:27:57.182899 raise_utils-2.2.1/raise_utils/data/
--rw-r--r--   0 ryedida    (501) staff       (20)      114 2020-09-01 01:32:09.000000 raise_utils-2.2.1/raise_utils/data/__init__.py
--rw-r--r--   0 ryedida    (501) staff       (20)     5595 2024-01-13 00:33:28.000000 raise_utils-2.2.1/raise_utils/data/data.py
-drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-03-20 05:27:57.183753 raise_utils-2.2.1/raise_utils/experiments/
--rw-r--r--   0 ryedida    (501) staff       (20)       58 2020-09-01 01:33:15.000000 raise_utils-2.2.1/raise_utils/experiments/__init__.py
--rw-r--r--   0 ryedida    (501) staff       (20)     3390 2024-01-24 21:15:10.000000 raise_utils-2.2.1/raise_utils/experiments/experiment.py
-drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-03-20 05:27:57.184474 raise_utils-2.2.1/raise_utils/hooks/
--rw-r--r--   0 ryedida    (501) staff       (20)       41 2020-09-17 01:03:00.000000 raise_utils-2.2.1/raise_utils/hooks/__init__.py
--rw-r--r--   0 ryedida    (501) staff       (20)      730 2020-09-17 01:02:03.000000 raise_utils-2.2.1/raise_utils/hooks/hooks.py
-drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-03-20 05:27:57.187189 raise_utils-2.2.1/raise_utils/hyperparams/
--rw-r--r--   0 ryedida    (501) staff       (20)      217 2023-10-30 22:46:24.000000 raise_utils-2.2.1/raise_utils/hyperparams/__init__.py
--rw-r--r--   0 ryedida    (501) staff       (20)     5082 2024-02-16 08:27:08.000000 raise_utils-2.2.1/raise_utils/hyperparams/dodge.py
--rw-r--r--   0 ryedida    (501) staff       (20)     4693 2023-01-10 20:48:53.000000 raise_utils-2.2.1/raise_utils/hyperparams/ghost.py
--rw-r--r--   0 ryedida    (501) staff       (20)     4201 2023-09-13 07:08:15.000000 raise_utils-2.2.1/raise_utils/hyperparams/hpo.py
--rw-r--r--   0 ryedida    (501) staff       (20)     9069 2024-01-13 00:34:34.000000 raise_utils-2.2.1/raise_utils/hyperparams/multi_ghost.py
--rw-r--r--   0 ryedida    (501) staff       (20)        0 2023-06-03 04:35:45.000000 raise_utils-2.2.1/raise_utils/hyperparams/smoothie.py
-drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-03-20 05:27:57.188747 raise_utils-2.2.1/raise_utils/interpret/
--rw-r--r--   0 ryedida    (501) staff       (20)      188 2023-09-04 06:47:35.000000 raise_utils-2.2.1/raise_utils/interpret/__init__.py
--rw-r--r--   0 ryedida    (501) staff       (20)     7217 2022-01-01 10:43:53.000000 raise_utils-2.2.1/raise_utils/interpret/interpret.py
--rw-r--r--   0 ryedida    (501) staff       (20)     2897 2024-02-05 02:13:44.000000 raise_utils-2.2.1/raise_utils/interpret/kw.py
--rw-r--r--   0 ryedida    (501) staff       (20)     1350 2021-12-07 01:33:29.000000 raise_utils-2.2.1/raise_utils/interpret/scottknott.py
--rw-r--r--   0 ryedida    (501) staff       (20)     8990 2021-12-07 01:39:56.000000 raise_utils-2.2.1/raise_utils/interpret/sk.py
-drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-03-20 05:27:57.193087 raise_utils-2.2.1/raise_utils/learners/
--rw-r--r--   0 ryedida    (501) staff       (20)      492 2024-02-14 08:17:41.000000 raise_utils-2.2.1/raise_utils/learners/__init__.py
--rw-r--r--   0 ryedida    (501) staff       (20)     4340 2024-01-24 20:58:16.000000 raise_utils-2.2.1/raise_utils/learners/autoencoder.py
--rw-r--r--   0 ryedida    (501) staff       (20)     4734 2024-02-16 09:17:36.000000 raise_utils-2.2.1/raise_utils/learners/feedforward.py
--rw-r--r--   0 ryedida    (501) staff       (20)     3911 2023-01-10 20:30:32.000000 raise_utils-2.2.1/raise_utils/learners/learner.py
--rw-r--r--   0 ryedida    (501) staff       (20)      718 2020-09-01 01:36:18.000000 raise_utils-2.2.1/raise_utils/learners/logreg.py
--rw-r--r--   0 ryedida    (501) staff       (20)     4159 2024-01-13 00:37:54.000000 raise_utils-2.2.1/raise_utils/learners/multiclassdl.py
--rw-r--r--   0 ryedida    (501) staff       (20)      336 2020-09-01 01:36:35.000000 raise_utils-2.2.1/raise_utils/learners/nb.py
--rw-r--r--   0 ryedida    (501) staff       (20)      651 2020-09-01 01:36:46.000000 raise_utils-2.2.1/raise_utils/learners/rf.py
--rw-r--r--   0 ryedida    (501) staff       (20)     3717 2020-09-01 18:09:54.000000 raise_utils-2.2.1/raise_utils/learners/svm.py
--rw-r--r--   0 ryedida    (501) staff       (20)      649 2020-09-01 06:56:10.000000 raise_utils-2.2.1/raise_utils/learners/tree.py
-drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-03-20 05:27:57.194198 raise_utils-2.2.1/raise_utils/metrics/
--rw-r--r--   0 ryedida    (501) staff       (20)       62 2020-09-01 01:37:32.000000 raise_utils-2.2.1/raise_utils/metrics/__init__.py
--rw-r--r--   0 ryedida    (501) staff       (20)     6080 2023-01-18 19:43:26.000000 raise_utils-2.2.1/raise_utils/metrics/impl.py
--rw-r--r--   0 ryedida    (501) staff       (20)     2844 2022-02-24 04:19:18.000000 raise_utils-2.2.1/raise_utils/metrics/metrics.py
-drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-03-20 05:27:57.199582 raise_utils-2.2.1/raise_utils/transforms/
--rw-r--r--   0 ryedida    (501) staff       (20)      118 2021-09-24 01:53:58.000000 raise_utils-2.2.1/raise_utils/transforms/__init__.py
--rw-r--r--   0 ryedida    (501) staff       (20)     4942 2024-02-16 08:56:15.000000 raise_utils-2.2.1/raise_utils/transforms/cfs.py
--rw-r--r--   0 ryedida    (501) staff       (20)     1221 2020-08-13 22:45:52.000000 raise_utils-2.2.1/raise_utils/transforms/inliers.py
--rw-r--r--   0 ryedida    (501) staff       (20)      150 2021-02-24 22:33:36.000000 raise_utils-2.2.1/raise_utils/transforms/null.py
--rw-r--r--   0 ryedida    (501) staff       (20)  1088707 2024-03-20 05:22:01.000000 raise_utils-2.2.1/raise_utils/transforms/remove_labels.c
--rw-r--r--   0 ryedida    (501) staff       (20)     1534 2024-01-25 06:06:33.000000 raise_utils-2.2.1/raise_utils/transforms/remove_labels.pyx
-drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-03-20 05:27:57.201517 raise_utils-2.2.1/raise_utils/transforms/text/
--rw-r--r--   0 ryedida    (501) staff       (20)        0 2020-08-16 20:40:06.000000 raise_utils-2.2.1/raise_utils/transforms/text/__init__.py
--rw-r--r--   0 ryedida    (501) staff       (20)      802 2020-09-01 07:05:39.000000 raise_utils-2.2.1/raise_utils/transforms/text/hashing.py
--rw-r--r--   0 ryedida    (501) staff       (20)      989 2020-09-01 07:05:47.000000 raise_utils-2.2.1/raise_utils/transforms/text/lda.py
--rw-r--r--   0 ryedida    (501) staff       (20)      751 2020-09-01 07:05:58.000000 raise_utils-2.2.1/raise_utils/transforms/text/tf.py
--rw-r--r--   0 ryedida    (501) staff       (20)      799 2020-09-01 07:06:06.000000 raise_utils-2.2.1/raise_utils/transforms/text/tfidf.py
--rw-r--r--   0 ryedida    (501) staff       (20)     1164 2021-09-24 01:53:58.000000 raise_utils-2.2.1/raise_utils/transforms/text/transform.py
--rw-r--r--   0 ryedida    (501) staff       (20)     4321 2024-03-20 05:26:07.000000 raise_utils-2.2.1/raise_utils/transforms/transform.py
--rw-r--r--   0 ryedida    (501) staff       (20)     2487 2024-01-24 20:54:33.000000 raise_utils-2.2.1/raise_utils/transforms/wfo.py
-drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-03-20 05:27:57.202914 raise_utils-2.2.1/raise_utils/utils/
--rw-r--r--   0 ryedida    (501) staff       (20)       91 2022-02-24 05:05:51.000000 raise_utils-2.2.1/raise_utils/utils/__init__.py
--rw-r--r--   0 ryedida    (501) staff       (20)     1051 2023-08-30 00:21:00.000000 raise_utils-2.2.1/raise_utils/utils/data_utils.py
--rw-r--r--   0 ryedida    (501) staff       (20)     1000 2022-02-24 05:05:50.000000 raise_utils-2.2.1/raise_utils/utils/utils.py
-drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-03-20 05:27:57.204422 raise_utils-2.2.1/raise_utils.egg-info/
--rw-r--r--   0 ryedida    (501) staff       (20)     3114 2024-03-20 05:27:56.000000 raise_utils-2.2.1/raise_utils.egg-info/PKG-INFO
--rw-r--r--   0 ryedida    (501) staff       (20)     1825 2024-03-20 05:27:57.000000 raise_utils-2.2.1/raise_utils.egg-info/SOURCES.txt
--rw-r--r--   0 ryedida    (501) staff       (20)        1 2024-03-20 05:27:56.000000 raise_utils-2.2.1/raise_utils.egg-info/dependency_links.txt
--rw-r--r--   0 ryedida    (501) staff       (20)      117 2024-03-20 05:27:56.000000 raise_utils-2.2.1/raise_utils.egg-info/requires.txt
--rw-r--r--   0 ryedida    (501) staff       (20)       26 2024-03-20 05:27:56.000000 raise_utils-2.2.1/raise_utils.egg-info/top_level.txt
--rw-r--r--   0 ryedida    (501) staff       (20)       38 2024-03-20 05:27:57.206010 raise_utils-2.2.1/setup.cfg
--rw-r--r--   0 ryedida    (501) staff       (20)     1327 2024-03-20 05:27:09.000000 raise_utils-2.2.1/setup.py
-drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-03-20 05:27:57.203360 raise_utils-2.2.1/tests/
--rw-r--r--   0 ryedida    (501) staff       (20)       79 2021-02-13 00:46:39.000000 raise_utils-2.2.1/tests/test_package.py
+drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-05-17 02:17:51.782765 raise_utils-2.2.2/
+-rw-r--r--   0 ryedida    (501) staff       (20)    26526 2020-08-30 18:58:05.000000 raise_utils-2.2.2/LICENSE
+-rw-r--r--   0 ryedida    (501) staff       (20)       68 2024-01-07 02:27:16.000000 raise_utils-2.2.2/MANIFEST.in
+-rw-r--r--   0 ryedida    (501) staff       (20)     3114 2024-05-17 02:17:51.781110 raise_utils-2.2.2/PKG-INFO
+-rw-r--r--   0 ryedida    (501) staff       (20)     2554 2024-01-07 02:27:35.000000 raise_utils-2.2.2/README.md
+-rw-r--r--   0 ryedida    (501) staff       (20)      661 2024-05-17 02:17:31.000000 raise_utils-2.2.2/pyproject.toml
+drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-05-17 02:17:51.756249 raise_utils-2.2.2/raise_utils/
+-rw-r--r--   0 ryedida    (501) staff       (20)       22 2024-05-17 02:17:38.000000 raise_utils-2.2.2/raise_utils/__init__.py
+drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-05-17 02:17:51.762766 raise_utils-2.2.2/raise_utils/data/
+-rw-r--r--   0 ryedida    (501) staff       (20)      114 2020-09-01 01:32:09.000000 raise_utils-2.2.2/raise_utils/data/__init__.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     5595 2024-01-13 00:33:28.000000 raise_utils-2.2.2/raise_utils/data/data.py
+drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-05-17 02:17:51.763620 raise_utils-2.2.2/raise_utils/experiments/
+-rw-r--r--   0 ryedida    (501) staff       (20)       58 2020-09-01 01:33:15.000000 raise_utils-2.2.2/raise_utils/experiments/__init__.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     3390 2024-01-24 21:15:10.000000 raise_utils-2.2.2/raise_utils/experiments/experiment.py
+drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-05-17 02:17:51.764340 raise_utils-2.2.2/raise_utils/hooks/
+-rw-r--r--   0 ryedida    (501) staff       (20)       41 2020-09-17 01:03:00.000000 raise_utils-2.2.2/raise_utils/hooks/__init__.py
+-rw-r--r--   0 ryedida    (501) staff       (20)      730 2020-09-17 01:02:03.000000 raise_utils-2.2.2/raise_utils/hooks/hooks.py
+drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-05-17 02:17:51.766449 raise_utils-2.2.2/raise_utils/hyperparams/
+-rw-r--r--   0 ryedida    (501) staff       (20)      217 2023-10-30 22:46:24.000000 raise_utils-2.2.2/raise_utils/hyperparams/__init__.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     5082 2024-02-16 08:27:08.000000 raise_utils-2.2.2/raise_utils/hyperparams/dodge.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     4693 2023-01-10 20:48:53.000000 raise_utils-2.2.2/raise_utils/hyperparams/ghost.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     4201 2023-09-13 07:08:15.000000 raise_utils-2.2.2/raise_utils/hyperparams/hpo.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     9069 2024-01-13 00:34:34.000000 raise_utils-2.2.2/raise_utils/hyperparams/multi_ghost.py
+-rw-r--r--   0 ryedida    (501) staff       (20)        0 2023-06-03 04:35:45.000000 raise_utils-2.2.2/raise_utils/hyperparams/smoothie.py
+drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-05-17 02:17:51.768094 raise_utils-2.2.2/raise_utils/interpret/
+-rw-r--r--   0 ryedida    (501) staff       (20)      188 2023-09-04 06:47:35.000000 raise_utils-2.2.2/raise_utils/interpret/__init__.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     7217 2022-01-01 10:43:53.000000 raise_utils-2.2.2/raise_utils/interpret/interpret.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     2897 2024-02-05 02:13:44.000000 raise_utils-2.2.2/raise_utils/interpret/kw.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     1370 2024-05-17 02:12:13.000000 raise_utils-2.2.2/raise_utils/interpret/scottknott.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     8990 2021-12-07 01:39:56.000000 raise_utils-2.2.2/raise_utils/interpret/sk.py
+drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-05-17 02:17:51.771294 raise_utils-2.2.2/raise_utils/learners/
+-rw-r--r--   0 ryedida    (501) staff       (20)      492 2024-02-14 08:17:41.000000 raise_utils-2.2.2/raise_utils/learners/__init__.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     4444 2024-03-20 06:49:01.000000 raise_utils-2.2.2/raise_utils/learners/autoencoder.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     4734 2024-02-16 09:17:36.000000 raise_utils-2.2.2/raise_utils/learners/feedforward.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     3911 2023-01-10 20:30:32.000000 raise_utils-2.2.2/raise_utils/learners/learner.py
+-rw-r--r--   0 ryedida    (501) staff       (20)      718 2020-09-01 01:36:18.000000 raise_utils-2.2.2/raise_utils/learners/logreg.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     4159 2024-03-20 05:59:25.000000 raise_utils-2.2.2/raise_utils/learners/multiclassdl.py
+-rw-r--r--   0 ryedida    (501) staff       (20)      336 2020-09-01 01:36:35.000000 raise_utils-2.2.2/raise_utils/learners/nb.py
+-rw-r--r--   0 ryedida    (501) staff       (20)      651 2020-09-01 01:36:46.000000 raise_utils-2.2.2/raise_utils/learners/rf.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     3717 2020-09-01 18:09:54.000000 raise_utils-2.2.2/raise_utils/learners/svm.py
+-rw-r--r--   0 ryedida    (501) staff       (20)      649 2020-09-01 06:56:10.000000 raise_utils-2.2.2/raise_utils/learners/tree.py
+drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-05-17 02:17:51.772194 raise_utils-2.2.2/raise_utils/metrics/
+-rw-r--r--   0 ryedida    (501) staff       (20)       62 2020-09-01 01:37:32.000000 raise_utils-2.2.2/raise_utils/metrics/__init__.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     6080 2023-01-18 19:43:26.000000 raise_utils-2.2.2/raise_utils/metrics/impl.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     2844 2022-02-24 04:19:18.000000 raise_utils-2.2.2/raise_utils/metrics/metrics.py
+drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-05-17 02:17:51.777058 raise_utils-2.2.2/raise_utils/transforms/
+-rw-r--r--   0 ryedida    (501) staff       (20)      118 2021-09-24 01:53:58.000000 raise_utils-2.2.2/raise_utils/transforms/__init__.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     4942 2024-02-16 08:56:15.000000 raise_utils-2.2.2/raise_utils/transforms/cfs.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     1221 2020-08-13 22:45:52.000000 raise_utils-2.2.2/raise_utils/transforms/inliers.py
+-rw-r--r--   0 ryedida    (501) staff       (20)      150 2021-02-24 22:33:36.000000 raise_utils-2.2.2/raise_utils/transforms/null.py
+-rw-r--r--   0 ryedida    (501) staff       (20)  1088358 2024-03-26 22:14:19.000000 raise_utils-2.2.2/raise_utils/transforms/remove_labels.c
+-rw-r--r--   0 ryedida    (501) staff       (20)     1534 2024-01-25 06:06:33.000000 raise_utils-2.2.2/raise_utils/transforms/remove_labels.pyx
+drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-05-17 02:17:51.779028 raise_utils-2.2.2/raise_utils/transforms/text/
+-rw-r--r--   0 ryedida    (501) staff       (20)        0 2020-08-16 20:40:06.000000 raise_utils-2.2.2/raise_utils/transforms/text/__init__.py
+-rw-r--r--   0 ryedida    (501) staff       (20)      802 2020-09-01 07:05:39.000000 raise_utils-2.2.2/raise_utils/transforms/text/hashing.py
+-rw-r--r--   0 ryedida    (501) staff       (20)      989 2020-09-01 07:05:47.000000 raise_utils-2.2.2/raise_utils/transforms/text/lda.py
+-rw-r--r--   0 ryedida    (501) staff       (20)      751 2020-09-01 07:05:58.000000 raise_utils-2.2.2/raise_utils/transforms/text/tf.py
+-rw-r--r--   0 ryedida    (501) staff       (20)      799 2020-09-01 07:06:06.000000 raise_utils-2.2.2/raise_utils/transforms/text/tfidf.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     1164 2021-09-24 01:53:58.000000 raise_utils-2.2.2/raise_utils/transforms/text/transform.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     4249 2024-03-20 05:53:55.000000 raise_utils-2.2.2/raise_utils/transforms/transform.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     2487 2024-01-24 20:54:33.000000 raise_utils-2.2.2/raise_utils/transforms/wfo.py
+drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-05-17 02:17:51.780054 raise_utils-2.2.2/raise_utils/utils/
+-rw-r--r--   0 ryedida    (501) staff       (20)       91 2022-02-24 05:05:51.000000 raise_utils-2.2.2/raise_utils/utils/__init__.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     1051 2023-08-30 00:21:00.000000 raise_utils-2.2.2/raise_utils/utils/data_utils.py
+-rw-r--r--   0 ryedida    (501) staff       (20)     1000 2022-02-24 05:05:50.000000 raise_utils-2.2.2/raise_utils/utils/utils.py
+drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-05-17 02:17:51.780723 raise_utils-2.2.2/raise_utils.egg-info/
+-rw-r--r--   0 ryedida    (501) staff       (20)     3114 2024-05-17 02:17:51.000000 raise_utils-2.2.2/raise_utils.egg-info/PKG-INFO
+-rw-r--r--   0 ryedida    (501) staff       (20)     1825 2024-05-17 02:17:51.000000 raise_utils-2.2.2/raise_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 ryedida    (501) staff       (20)        1 2024-05-17 02:17:51.000000 raise_utils-2.2.2/raise_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 ryedida    (501) staff       (20)      117 2024-05-17 02:17:51.000000 raise_utils-2.2.2/raise_utils.egg-info/requires.txt
+-rw-r--r--   0 ryedida    (501) staff       (20)       26 2024-05-17 02:17:51.000000 raise_utils-2.2.2/raise_utils.egg-info/top_level.txt
+-rw-r--r--   0 ryedida    (501) staff       (20)       38 2024-05-17 02:17:51.782869 raise_utils-2.2.2/setup.cfg
+-rw-r--r--   0 ryedida    (501) staff       (20)     1327 2024-05-17 02:17:22.000000 raise_utils-2.2.2/setup.py
+drwxr-xr-x   0 ryedida    (501) staff       (20)        0 2024-05-17 02:17:51.780373 raise_utils-2.2.2/tests/
+-rw-r--r--   0 ryedida    (501) staff       (20)       79 2021-02-13 00:46:39.000000 raise_utils-2.2.2/tests/test_package.py
```

### Comparing `raise_utils-2.2.1/LICENSE` & `raise_utils-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/PKG-INFO` & `raise_utils-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raise_utils
-Version: 2.2.1
+Version: 2.2.2
 Summary: RAISE lab package (LGPL-3.0-or-later)
 Home-page: https://github.com/yrahul3910/raise
 Author: RAISE, NC State University
 Author-email: ryedida@ncsu.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scikit-learn>=0.23.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: raise_utils Version: 2.2.1 Summary: RAISE lab
+Metadata-Version: 2.1 Name: raise_utils Version: 2.2.2 Summary: RAISE lab
 package (LGPL-3.0-or-later) Home-page: https://github.com/yrahul3910/raise
 Author: RAISE, NC State University Author-email: ryedida@ncsu.edu Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: scikit-
 learn>=0.23.2 Requires-Dist: keras>=3.0.0 Requires-Dist: numpy>=1.19.2
 Requires-Dist: pandas Requires-Dist: cvxopt Requires-Dist: colorama Requires-
 Dist: hyperopt Requires-Dist: imblearn Requires-Dist: Cython Requires-Dist:
 tabulate Requires-Dist: statsmodels
```

### Comparing `raise_utils-2.2.1/README.md` & `raise_utils-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/pyproject.toml` & `raise_utils-2.2.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "raise-utils"
-version = "2.2.1"
+version = "2.2.2"
 description = "RAISE lab package"
 authors = ["Rahul Yedida <rahul.yedida@pm.me>"]
 license = "LGPL 2.1"
 readme = "README.md"
 packages = [{include = "raise_utils"}]
 
 [tool.poetry.dependencies]
@@ -12,19 +12,19 @@
 pytest-cov = "^4.1.0"
 cvxopt = "^1.3.1"
 pandas = "^2.0.2"
 numpy = "^1.23.2"
 colorama = "^0.4.6"
 hyperopt = "^0.2.7"
 coverage = "^7.2.7"
-ray = {extras = ["tune"], version = "^2.5.0"}
 scikit-learn = ">=0.23.2"
 imblearn = "^0.0"
 bohb-hpo = "^0.5.2"
 Cython = "^0.29.24"
 tabulate = "^0.8.9"
 keras = "^3.0.0"
 statsmodels = "^0.14.0"
+python = ">=3.9"
 
 [build-system]
 requires = ["setuptools", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
```

### Comparing `raise_utils-2.2.1/raise_utils/data/data.py` & `raise_utils-2.2.2/raise_utils/data/data.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/experiments/experiment.py` & `raise_utils-2.2.2/raise_utils/experiments/experiment.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/hooks/hooks.py` & `raise_utils-2.2.2/raise_utils/hooks/hooks.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/hyperparams/dodge.py` & `raise_utils-2.2.2/raise_utils/hyperparams/dodge.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/hyperparams/ghost.py` & `raise_utils-2.2.2/raise_utils/hyperparams/ghost.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/hyperparams/hpo.py` & `raise_utils-2.2.2/raise_utils/hyperparams/hpo.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/hyperparams/multi_ghost.py` & `raise_utils-2.2.2/raise_utils/hyperparams/multi_ghost.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/interpret/interpret.py` & `raise_utils-2.2.2/raise_utils/interpret/interpret.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/interpret/kw.py` & `raise_utils-2.2.2/raise_utils/interpret/kw.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/interpret/scottknott.py` & `raise_utils-2.2.2/raise_utils/interpret/scottknott.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 
     def pprint(self):
         """Pretty-print the results."""
         Rx.show(Rx.sk(Rx.data(**self.data), effect=self.effect))
 
     def get_results(self):
         """Gets the Scott-Knott results."""
-        return Rx.sk(Rx.data(**self.data))
+        return Rx.sk(Rx.data(**self.data), effect=self.effect)
```

### Comparing `raise_utils-2.2.1/raise_utils/interpret/sk.py` & `raise_utils-2.2.2/raise_utils/interpret/sk.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/learners/autoencoder.py` & `raise_utils-2.2.2/raise_utils/learners/autoencoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import keras
 from keras.models import Model
 from keras.layers import Dense, Input
 from keras.callbacks import EarlyStopping
 import numpy as np
 from raise_utils.learners.learner import Learner
 
 
@@ -77,16 +78,14 @@
 
         dec_intermediate = Dense(
             self.x_train.shape[1], name='decoded', activation='relu')(dec_intermediate)
 
         self.model = Model(inputs=enc_inp, outputs=dec_intermediate)
         self.encoder = Model(inputs=enc_inp, outputs=enc_intermediate)
 
-        self.model.summary()
-
         dec_inp = Input(shape=(self.n_out,))
         for layer in self.model.layers[-1 - len(self.n_units):]:
             dec_intermediate_values = layer(
                 dec_intermediate_values) if 'dec_intermediate_values' in locals() else layer(dec_inp)
         self.decoder = Model(inputs=dec_inp, outputs=dec_intermediate_values)
 
     def fit(self) -> None:
@@ -109,15 +108,20 @@
         Encodes an input.
 
         :param x - The input to be encoded
         """
         if self.model is None:
             raise AssertionError('Model is None.')
 
-        return self.encoder(x)
+        encoded = self.encoder(x)
+
+        if keras.config.backend() == "torch":
+            encoded = encoded.detach().numpy()
+
+        return encoded
 
     def decode(self, x: np.ndarray) -> np.ndarray:
         """
         Decodes an input from the encoded dimensionality.
 
         :param x - The encoded input.
         """
```

### Comparing `raise_utils-2.2.1/raise_utils/learners/feedforward.py` & `raise_utils-2.2.2/raise_utils/learners/feedforward.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/learners/learner.py` & `raise_utils-2.2.2/raise_utils/learners/learner.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/learners/logreg.py` & `raise_utils-2.2.2/raise_utils/learners/logreg.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/learners/multiclassdl.py` & `raise_utils-2.2.2/raise_utils/learners/multiclassdl.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/learners/rf.py` & `raise_utils-2.2.2/raise_utils/learners/rf.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/learners/svm.py` & `raise_utils-2.2.2/raise_utils/learners/svm.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/learners/tree.py` & `raise_utils-2.2.2/raise_utils/learners/tree.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/metrics/impl.py` & `raise_utils-2.2.2/raise_utils/metrics/impl.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/metrics/metrics.py` & `raise_utils-2.2.2/raise_utils/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/transforms/cfs.py` & `raise_utils-2.2.2/raise_utils/transforms/cfs.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/transforms/inliers.py` & `raise_utils-2.2.2/raise_utils/transforms/inliers.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/transforms/remove_labels.c` & `raise_utils-2.2.2/raise_utils/transforms/remove_labels.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.9 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "remove_labels",
         "sources": [
             "raise_utils/transforms/remove_labels.pyx"
@@ -32,18 +32,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x030009F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -728,16 +728,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1081,15 +1086,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1168,15 +1173,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1274,32 +1279,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -25638,15 +25626,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `raise_utils-2.2.1/raise_utils/transforms/remove_labels.pyx` & `raise_utils-2.2.2/raise_utils/transforms/remove_labels.pyx`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/transforms/text/hashing.py` & `raise_utils-2.2.2/raise_utils/transforms/text/hashing.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/transforms/text/lda.py` & `raise_utils-2.2.2/raise_utils/transforms/text/lda.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/transforms/text/tf.py` & `raise_utils-2.2.2/raise_utils/transforms/text/tf.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/transforms/text/tfidf.py` & `raise_utils-2.2.2/raise_utils/transforms/text/tfidf.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/transforms/text/transform.py` & `raise_utils-2.2.2/raise_utils/transforms/text/transform.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/transforms/transform.py` & `raise_utils-2.2.2/raise_utils/transforms/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 from raise_utils.transforms.null import NullTransform
 from raise_utils.transforms.text.transform import TextTransform
 from raise_utils.transforms.wfo import WeightedFuzzyOversampler
 from raise_utils.transforms.wfo import RadiallyWeightedFuzzyOversampler
 from raise_utils.data import Data
 import numpy as np
 import keras
-import pyximport
-
-pyximport.install()
-
 from remove_labels import Smooth  # noqa: F402
 
 if keras.config.backend() == "torch":
     from torch import FloatTensor, Tensor
 
 transformers = {
     "normalize": Normalizer,
@@ -103,15 +99,15 @@
                 else:
                     data.x_train = self.transformer.fit_transform(data.x_train)
 
                 if self.name != "wfo" and self.name != "rwfo":
                     data.x_test = self.transformer.transform(data.x_test)
             else:
                 if len(data.x_train) > self.transformer.k_neighbors:
-                    self.transformer = SMOTE(k_neighbors=len(data.x_train) - 1)
+                    self.transformer = SMOTE()
 
                 data.x_train, data.y_train = self.transformer.fit_resample(
                     data.x_train, data.y_train)
 
             if revert_to_tensor:
                 data.x_train = FloatTensor(data.x_train)
                 data.x_test = FloatTensor(data.x_test)
```

### Comparing `raise_utils-2.2.1/raise_utils/transforms/wfo.py` & `raise_utils-2.2.2/raise_utils/transforms/wfo.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/utils/data_utils.py` & `raise_utils-2.2.2/raise_utils/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils/utils/utils.py` & `raise_utils-2.2.2/raise_utils/utils/utils.py`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/raise_utils.egg-info/PKG-INFO` & `raise_utils-2.2.2/raise_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: raise-utils
-Version: 2.2.1
+Name: raise_utils
+Version: 2.2.2
 Summary: RAISE lab package (LGPL-3.0-or-later)
 Home-page: https://github.com/yrahul3910/raise
 Author: RAISE, NC State University
 Author-email: ryedida@ncsu.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scikit-learn>=0.23.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: raise-utils Version: 2.2.1 Summary: RAISE lab
+Metadata-Version: 2.1 Name: raise_utils Version: 2.2.2 Summary: RAISE lab
 package (LGPL-3.0-or-later) Home-page: https://github.com/yrahul3910/raise
 Author: RAISE, NC State University Author-email: ryedida@ncsu.edu Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: scikit-
 learn>=0.23.2 Requires-Dist: keras>=3.0.0 Requires-Dist: numpy>=1.19.2
 Requires-Dist: pandas Requires-Dist: cvxopt Requires-Dist: colorama Requires-
 Dist: hyperopt Requires-Dist: imblearn Requires-Dist: Cython Requires-Dist:
 tabulate Requires-Dist: statsmodels
```

### Comparing `raise_utils-2.2.1/raise_utils.egg-info/SOURCES.txt` & `raise_utils-2.2.2/raise_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raise_utils-2.2.1/setup.py` & `raise_utils-2.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ext_modules = cythonize(Extension(
     name="remove_labels",
     sources=["raise_utils/transforms/remove_labels.pyx"]
 ))
 
 setup(name='raise_utils',
-      version='2.2.1',
+      version='2.2.2',
       description='RAISE lab package (LGPL-3.0-or-later)',
       author='RAISE, NC State University',
       author_email='ryedida@ncsu.edu',
       long_description=open(os.path.join(
           os.path.dirname(__file__), 'README.md')).read(),
       long_description_content_type='text/markdown',
       url='https://github.com/yrahul3910/raise',
```

