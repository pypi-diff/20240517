# Comparing `tmp/luma-ml-0.8.0.tar.gz` & `tmp/luma-ml-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luma-ml-0.8.0.tar", last modified: Tue May 14 16:47:33 2024, max compression
+gzip compressed data, was "luma-ml-0.8.1.tar", last modified: Fri May 17 14:28:21 2024, max compression
```

## Comparing `luma-ml-0.8.0.tar` & `luma-ml-0.8.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.180191 luma-ml-0.8.0/
--rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.8.0/LICENSE
--rw-r--r--   0 chanlee    (501) staff       (20)     5552 2024-05-14 16:47:33.179664 luma-ml-0.8.0/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     4946 2024-05-14 16:40:36.000000 luma-ml-0.8.0/README.md
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.126357 luma-ml-0.8.0/luma/
--rw-r--r--   0 chanlee    (501) staff       (20)    10872 2024-05-12 19:39:10.000000 luma-ml-0.8.0/luma/__import__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.8.0/luma/__init__.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.133221 luma-ml-0.8.0/luma/classifier/
--rw-r--r--   0 chanlee    (501) staff       (20)    12563 2024-05-13 11:38:17.000000 luma-ml-0.8.0/luma/classifier/discriminant.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7935 2024-05-13 11:35:13.000000 luma-ml-0.8.0/luma/classifier/logistic.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-04-21 11:35:39.000000 luma-ml-0.8.0/luma/classifier/naive_bayes.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9070 2024-05-13 11:30:20.000000 luma-ml-0.8.0/luma/classifier/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9174 2024-05-13 11:33:07.000000 luma-ml-0.8.0/luma/classifier/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9806 2024-05-13 11:36:04.000000 luma-ml-0.8.0/luma/classifier/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.142844 luma-ml-0.8.0/luma/clustering/
--rw-r--r--   0 chanlee    (501) staff       (20)    18057 2024-05-13 11:42:50.000000 luma-ml-0.8.0/luma/clustering/affinity.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17889 2024-05-13 11:50:11.000000 luma-ml-0.8.0/luma/clustering/density.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7697 2024-05-13 11:51:42.000000 luma-ml-0.8.0/luma/clustering/hierarchy.py
--rw-r--r--   0 chanlee    (501) staff       (20)    18307 2024-05-13 11:55:03.000000 luma-ml-0.8.0/luma/clustering/kmeans.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8192 2024-05-13 11:55:57.000000 luma-ml-0.8.0/luma/clustering/mixture.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11602 2024-05-13 11:57:37.000000 luma-ml-0.8.0/luma/clustering/spectral.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.144920 luma-ml-0.8.0/luma/core/
--rw-r--r--   0 chanlee    (501) staff       (20)     5924 2024-05-13 11:58:02.000000 luma-ml-0.8.0/luma/core/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)      446 2024-05-13 11:58:51.000000 luma-ml-0.8.0/luma/core/main.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11013 2024-05-13 12:05:21.000000 luma-ml-0.8.0/luma/core/super.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.148692 luma-ml-0.8.0/luma/ensemble/
--rw-r--r--   0 chanlee    (501) staff       (20)    10046 2024-05-13 12:09:42.000000 luma-ml-0.8.0/luma/ensemble/bagging.py
--rw-r--r--   0 chanlee    (501) staff       (20)    19721 2024-05-13 12:15:52.000000 luma-ml-0.8.0/luma/ensemble/boost.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10280 2024-05-13 12:20:38.000000 luma-ml-0.8.0/luma/ensemble/forest.py
--rw-r--r--   0 chanlee    (501) staff       (20)    14109 2024-05-13 12:31:18.000000 luma-ml-0.8.0/luma/ensemble/stack.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6779 2024-05-13 12:36:00.000000 luma-ml-0.8.0/luma/ensemble/vote.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.150594 luma-ml-0.8.0/luma/interface/
--rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-05-13 12:36:06.000000 luma-ml-0.8.0/luma/interface/exception.py
--rw-r--r--   0 chanlee    (501) staff       (20)     4885 2024-05-13 12:44:14.000000 luma-ml-0.8.0/luma/interface/typing.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16195 2024-05-13 15:45:21.000000 luma-ml-0.8.0/luma/interface/util.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.152982 luma-ml-0.8.0/luma/metric/
--rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma-ml-0.8.0/luma/metric/classification.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5917 2024-05-13 15:46:55.000000 luma-ml-0.8.0/luma/metric/clustering.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-05-13 15:46:57.000000 luma-ml-0.8.0/luma/metric/distance.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-05-13 15:46:59.000000 luma-ml-0.8.0/luma/metric/regression.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.153317 luma-ml-0.8.0/luma/migrate/
--rw-r--r--   0 chanlee    (501) staff       (20)     3764 2024-05-13 16:18:47.000000 luma-ml-0.8.0/luma/migrate/port.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.155579 luma-ml-0.8.0/luma/model_selection/
--rw-r--r--   0 chanlee    (501) staff       (20)     3438 2024-05-13 16:20:58.000000 luma-ml-0.8.0/luma/model_selection/cv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8041 2024-05-13 16:29:29.000000 luma-ml-0.8.0/luma/model_selection/fold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12244 2024-05-13 16:35:00.000000 luma-ml-0.8.0/luma/model_selection/search.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5736 2024-05-13 16:40:23.000000 luma-ml-0.8.0/luma/model_selection/split.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.159938 luma-ml-0.8.0/luma/neural/
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.162910 luma-ml-0.8.0/luma/neural/_layers/
--rw-r--r--   0 chanlee    (501) staff       (20)     6748 2024-05-12 09:16:35.000000 luma-ml-0.8.0/luma/neural/_layers/_act.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17921 2024-05-12 08:56:53.000000 luma-ml-0.8.0/luma/neural/_layers/_conv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1108 2024-05-12 09:15:57.000000 luma-ml-0.8.0/luma/neural/_layers/_drop.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2313 2024-05-12 09:17:05.000000 luma-ml-0.8.0/luma/neural/_layers/_linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10640 2024-05-12 19:37:14.000000 luma-ml-0.8.0/luma/neural/_layers/_norm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9291 2024-05-12 09:04:21.000000 luma-ml-0.8.0/luma/neural/_layers/_pool.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.164149 luma-ml-0.8.0/luma/neural/_models/
--rw-r--r--   0 chanlee    (501) staff       (20)    14219 2024-05-12 19:37:23.000000 luma-ml-0.8.0/luma/neural/_models/_imagenet.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12645 2024-05-11 19:57:06.000000 luma-ml-0.8.0/luma/neural/_models/_lenet.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9602 2024-05-12 07:21:21.000000 luma-ml-0.8.0/luma/neural/_models/_simple.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12024 2024-05-13 17:00:56.000000 luma-ml-0.8.0/luma/neural/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)    15726 2024-05-13 17:44:43.000000 luma-ml-0.8.0/luma/neural/block.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1319 2024-05-09 19:24:30.000000 luma-ml-0.8.0/luma/neural/init.py
--rw-r--r--   0 chanlee    (501) staff       (20)    22917 2024-05-13 19:10:14.000000 luma-ml-0.8.0/luma/neural/layer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-05-13 19:10:16.000000 luma-ml-0.8.0/luma/neural/loss.py
--rw-r--r--   0 chanlee    (501) staff       (20)    25998 2024-05-13 19:25:58.000000 luma-ml-0.8.0/luma/neural/network.py
--rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-05-09 17:12:02.000000 luma-ml-0.8.0/luma/neural/optimizer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8582 2024-05-13 19:27:55.000000 luma-ml-0.8.0/luma/neural/single.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.164395 luma-ml-0.8.0/luma/pipe/
--rw-r--r--   0 chanlee    (501) staff       (20)     7308 2024-05-13 19:32:18.000000 luma-ml-0.8.0/luma/pipe/pipeline.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.167026 luma-ml-0.8.0/luma/preprocessing/
--rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.8.0/luma/preprocessing/encoder.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.8.0/luma/preprocessing/imputer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3653 2024-05-13 19:32:35.000000 luma-ml-0.8.0/luma/preprocessing/outlier.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2624 2024-05-13 19:33:29.000000 luma-ml-0.8.0/luma/preprocessing/scaler.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.169823 luma-ml-0.8.0/luma/reduction/
--rw-r--r--   0 chanlee    (501) staff       (20)    19132 2024-05-13 19:40:06.000000 luma-ml-0.8.0/luma/reduction/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    40387 2024-05-13 19:55:48.000000 luma-ml-0.8.0/luma/reduction/manifold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17019 2024-05-14 09:45:27.000000 luma-ml-0.8.0/luma/reduction/selection.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.175673 luma-ml-0.8.0/luma/regressor/
--rw-r--r--   0 chanlee    (501) staff       (20)    19882 2024-05-14 09:56:22.000000 luma-ml-0.8.0/luma/regressor/general.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12687 2024-05-14 10:03:42.000000 luma-ml-0.8.0/luma/regressor/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6755 2024-05-14 10:04:13.000000 luma-ml-0.8.0/luma/regressor/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3098 2024-05-14 10:05:44.000000 luma-ml-0.8.0/luma/regressor/poly.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11070 2024-05-14 14:33:09.000000 luma-ml-0.8.0/luma/regressor/robust.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7805 2024-05-14 14:45:46.000000 luma-ml-0.8.0/luma/regressor/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7415 2024-05-14 14:59:17.000000 luma-ml-0.8.0/luma/regressor/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.176714 luma-ml-0.8.0/luma/visual/
--rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.8.0/luma/visual/eda.py
--rw-r--r--   0 chanlee    (501) staff       (20)    25027 2024-05-14 16:39:15.000000 luma-ml-0.8.0/luma/visual/evaluation.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.178430 luma-ml-0.8.0/luma_ml.egg-info/
--rw-r--r--   0 chanlee    (501) staff       (20)     5552 2024-05-14 16:47:33.000000 luma-ml-0.8.0/luma_ml.egg-info/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     1948 2024-05-14 16:47:33.000000 luma-ml-0.8.0/luma_ml.egg-info/SOURCES.txt
--rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-05-14 16:47:33.000000 luma-ml-0.8.0/luma_ml.egg-info/dependency_links.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-14 16:47:33.000000 luma-ml-0.8.0/luma_ml.egg-info/requires.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-05-14 16:47:33.000000 luma-ml-0.8.0/luma_ml.egg-info/top_level.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-14 16:47:33.180270 luma-ml-0.8.0/setup.cfg
--rw-r--r--   0 chanlee    (501) staff       (20)      842 2024-05-14 16:47:29.000000 luma-ml-0.8.0/setup.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-14 16:47:33.178977 luma-ml-0.8.0/test/
--rw-r--r--   0 chanlee    (501) staff       (20)      647 2024-04-29 02:58:00.000000 luma-ml-0.8.0/test/__act.py
--rw-r--r--   0 chanlee    (501) staff       (20)      499 2024-05-14 15:56:10.000000 luma-ml-0.8.0/test/__test.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.912562 luma-ml-0.8.1/
+-rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.8.1/LICENSE
+-rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-05-17 14:28:21.912167 luma-ml-0.8.1/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     4948 2024-05-17 14:25:43.000000 luma-ml-0.8.1/README.md
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.886076 luma-ml-0.8.1/luma/
+-rw-r--r--   0 chanlee    (501) staff       (20)    11001 2024-05-17 14:03:21.000000 luma-ml-0.8.1/luma/__import__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.8.1/luma/__init__.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.888825 luma-ml-0.8.1/luma/classifier/
+-rw-r--r--   0 chanlee    (501) staff       (20)    12563 2024-05-13 11:38:17.000000 luma-ml-0.8.1/luma/classifier/discriminant.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7935 2024-05-13 11:35:13.000000 luma-ml-0.8.1/luma/classifier/logistic.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-04-21 11:35:39.000000 luma-ml-0.8.1/luma/classifier/naive_bayes.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9070 2024-05-13 11:30:20.000000 luma-ml-0.8.1/luma/classifier/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9174 2024-05-13 11:33:07.000000 luma-ml-0.8.1/luma/classifier/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9806 2024-05-13 11:36:04.000000 luma-ml-0.8.1/luma/classifier/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.891696 luma-ml-0.8.1/luma/clustering/
+-rw-r--r--   0 chanlee    (501) staff       (20)    18057 2024-05-13 11:42:50.000000 luma-ml-0.8.1/luma/clustering/affinity.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17889 2024-05-13 11:50:11.000000 luma-ml-0.8.1/luma/clustering/density.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7697 2024-05-13 11:51:42.000000 luma-ml-0.8.1/luma/clustering/hierarchy.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    18307 2024-05-13 11:55:03.000000 luma-ml-0.8.1/luma/clustering/kmeans.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8192 2024-05-13 11:55:57.000000 luma-ml-0.8.1/luma/clustering/mixture.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11602 2024-05-13 11:57:37.000000 luma-ml-0.8.1/luma/clustering/spectral.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.892645 luma-ml-0.8.1/luma/core/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5924 2024-05-13 11:58:02.000000 luma-ml-0.8.1/luma/core/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      446 2024-05-13 11:58:51.000000 luma-ml-0.8.1/luma/core/main.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11013 2024-05-13 12:05:21.000000 luma-ml-0.8.1/luma/core/super.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.894914 luma-ml-0.8.1/luma/ensemble/
+-rw-r--r--   0 chanlee    (501) staff       (20)    10046 2024-05-13 12:09:42.000000 luma-ml-0.8.1/luma/ensemble/bagging.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19721 2024-05-13 12:15:52.000000 luma-ml-0.8.1/luma/ensemble/boost.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10280 2024-05-13 12:20:38.000000 luma-ml-0.8.1/luma/ensemble/forest.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    14109 2024-05-13 12:31:18.000000 luma-ml-0.8.1/luma/ensemble/stack.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6779 2024-05-13 12:36:00.000000 luma-ml-0.8.1/luma/ensemble/vote.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.895674 luma-ml-0.8.1/luma/interface/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-05-13 12:36:06.000000 luma-ml-0.8.1/luma/interface/exception.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7413 2024-05-17 07:30:53.000000 luma-ml-0.8.1/luma/interface/typing.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16195 2024-05-13 15:45:21.000000 luma-ml-0.8.1/luma/interface/util.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.896558 luma-ml-0.8.1/luma/metric/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma-ml-0.8.1/luma/metric/classification.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5917 2024-05-13 15:46:55.000000 luma-ml-0.8.1/luma/metric/clustering.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-05-13 15:46:57.000000 luma-ml-0.8.1/luma/metric/distance.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-05-13 15:46:59.000000 luma-ml-0.8.1/luma/metric/regression.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.896944 luma-ml-0.8.1/luma/migrate/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3764 2024-05-13 16:18:47.000000 luma-ml-0.8.1/luma/migrate/port.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.898363 luma-ml-0.8.1/luma/model_selection/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3438 2024-05-13 16:20:58.000000 luma-ml-0.8.1/luma/model_selection/cv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8041 2024-05-13 16:29:29.000000 luma-ml-0.8.1/luma/model_selection/fold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12244 2024-05-13 16:35:00.000000 luma-ml-0.8.1/luma/model_selection/search.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5736 2024-05-13 16:40:23.000000 luma-ml-0.8.1/luma/model_selection/split.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.900096 luma-ml-0.8.1/luma/neural/
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.901722 luma-ml-0.8.1/luma/neural/_layers/
+-rw-r--r--   0 chanlee    (501) staff       (20)     6748 2024-05-12 09:16:35.000000 luma-ml-0.8.1/luma/neural/_layers/_act.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    18113 2024-05-16 17:18:35.000000 luma-ml-0.8.1/luma/neural/_layers/_conv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     4144 2024-05-16 17:19:42.000000 luma-ml-0.8.1/luma/neural/_layers/_drop.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2313 2024-05-12 09:17:05.000000 luma-ml-0.8.1/luma/neural/_layers/_linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10790 2024-05-16 17:20:47.000000 luma-ml-0.8.1/luma/neural/_layers/_norm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9441 2024-05-16 17:21:47.000000 luma-ml-0.8.1/luma/neural/_layers/_pool.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.902354 luma-ml-0.8.1/luma/neural/_models/
+-rw-r--r--   0 chanlee    (501) staff       (20)    36463 2024-05-17 14:00:42.000000 luma-ml-0.8.1/luma/neural/_models/_imagenet.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12758 2024-05-17 07:23:08.000000 luma-ml-0.8.1/luma/neural/_models/_lenet.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9639 2024-05-17 07:21:18.000000 luma-ml-0.8.1/luma/neural/_models/_simple.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12024 2024-05-13 17:00:56.000000 luma-ml-0.8.1/luma/neural/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16608 2024-05-17 13:11:54.000000 luma-ml-0.8.1/luma/neural/block.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1319 2024-05-09 19:24:30.000000 luma-ml-0.8.1/luma/neural/init.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    25743 2024-05-16 14:22:33.000000 luma-ml-0.8.1/luma/neural/layer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-05-13 19:10:16.000000 luma-ml-0.8.1/luma/neural/loss.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    41603 2024-05-17 14:26:11.000000 luma-ml-0.8.1/luma/neural/network.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-05-09 17:12:02.000000 luma-ml-0.8.1/luma/neural/optimizer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8582 2024-05-13 19:27:55.000000 luma-ml-0.8.1/luma/neural/single.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.902568 luma-ml-0.8.1/luma/pipe/
+-rw-r--r--   0 chanlee    (501) staff       (20)     7308 2024-05-13 19:32:18.000000 luma-ml-0.8.1/luma/pipe/pipeline.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.903866 luma-ml-0.8.1/luma/preprocessing/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.8.1/luma/preprocessing/encoder.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.8.1/luma/preprocessing/imputer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3653 2024-05-13 19:32:35.000000 luma-ml-0.8.1/luma/preprocessing/outlier.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2624 2024-05-13 19:33:29.000000 luma-ml-0.8.1/luma/preprocessing/scaler.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.905487 luma-ml-0.8.1/luma/reduction/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19132 2024-05-13 19:40:06.000000 luma-ml-0.8.1/luma/reduction/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    40387 2024-05-13 19:55:48.000000 luma-ml-0.8.1/luma/reduction/manifold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17019 2024-05-14 09:45:27.000000 luma-ml-0.8.1/luma/reduction/selection.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.908619 luma-ml-0.8.1/luma/regressor/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19882 2024-05-14 09:56:22.000000 luma-ml-0.8.1/luma/regressor/general.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12687 2024-05-14 10:03:42.000000 luma-ml-0.8.1/luma/regressor/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6755 2024-05-14 10:04:13.000000 luma-ml-0.8.1/luma/regressor/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3098 2024-05-14 10:05:44.000000 luma-ml-0.8.1/luma/regressor/poly.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11070 2024-05-14 14:33:09.000000 luma-ml-0.8.1/luma/regressor/robust.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7805 2024-05-14 14:45:46.000000 luma-ml-0.8.1/luma/regressor/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7415 2024-05-14 14:59:17.000000 luma-ml-0.8.1/luma/regressor/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.909233 luma-ml-0.8.1/luma/visual/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.8.1/luma/visual/eda.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    25027 2024-05-14 16:39:15.000000 luma-ml-0.8.1/luma/visual/evaluation.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.910557 luma-ml-0.8.1/luma_ml.egg-info/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-05-17 14:28:21.000000 luma-ml-0.8.1/luma_ml.egg-info/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     1948 2024-05-17 14:28:21.000000 luma-ml-0.8.1/luma_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-05-17 14:28:21.000000 luma-ml-0.8.1/luma_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-17 14:28:21.000000 luma-ml-0.8.1/luma_ml.egg-info/requires.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-05-17 14:28:21.000000 luma-ml-0.8.1/luma_ml.egg-info/top_level.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-17 14:28:21.912633 luma-ml-0.8.1/setup.cfg
+-rw-r--r--   0 chanlee    (501) staff       (20)      842 2024-05-17 14:28:15.000000 luma-ml-0.8.1/setup.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.911467 luma-ml-0.8.1/test/
+-rw-r--r--   0 chanlee    (501) staff       (20)      647 2024-04-29 02:58:00.000000 luma-ml-0.8.1/test/__act.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      429 2024-05-17 14:02:51.000000 luma-ml-0.8.1/test/__test.py
```

### Comparing `luma-ml-0.8.0/LICENSE` & `luma-ml-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/PKG-INFO` & `luma-ml-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.8.0
+Version: 0.8.1
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.56k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.71k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.8.0</td>
+                    <td>0.8.1</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~22K</td>
+                    <td>~23.8K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.8.0 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.8.1 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.56k-red][GitHub code size in bytes][Code Style]
+5.71k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.8.0
-Lines of Code  ~22K
+Latest Version 0.8.1
+Lines of Code  ~23.8K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.8.0/README.md` & `luma-ml-0.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.56k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.71k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -89,19 +89,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.8.0</td>
+                    <td>0.8.1</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~22K</td>
+                    <td>~23.8K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.56k-red][GitHub code size in bytes][Code Style]
+5.71k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -24,12 +24,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.8.0
-Lines of Code  ~22K
+Latest Version 0.8.1
+Lines of Code  ~23.8K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.8.0/luma/__import__.py` & `luma-ml-0.8.1/luma/__import__.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,24 @@
     AdamWOptimizer,
     NAdamOptimizer,
 )
 from luma.neural.loss import CrossEntropy, BinaryCrossEntropy, MSELoss
 from luma.neural.init import KaimingInit, XavierInit
 from luma.neural.block import ConvBlock1D, ConvBlock2D, ConvBlock3D, DenseBlock
 from luma.neural.network import SimpleMLP, SimpleCNN
-from luma.neural.network import LeNet_1, LeNet_4, AlexNet, ZFNet
+from luma.neural.network import (
+    LeNet_1,
+    LeNet_4,
+    AlexNet,
+    ZFNet,
+    VGGNet_11,
+    VGGNet_13,
+    VGGNet_16,
+    VGGNet_19,
+)
 
 from luma.metric.classification import Accuracy, Precision, Recall, F1Score, Specificity
 from luma.metric.regression import (
     MeanAbsoluteError,
     MeanSquaredError,
     RootMeanSquaredError,
     MeanAbsolutePercentageError,
@@ -261,15 +270,16 @@
 
     CrossEntropy, BinaryCrossEntropy, MSELoss
 
     KaimingInit, XavierInit
 
     ConvBlock1D, ConvBlock2D, ConvBlock3D, DenseBlock
 
-    SimpleMLP, SimpleCNN, LeNet_1, LeNet_4, AlexNet, ZFNet
+    SimpleMLP, SimpleCNN, LeNet_1, LeNet_4, AlexNet, ZFNet,
+    VGGNet_11, VGGNet_13, VGGNet_16, VGGNet_19
 
     # ------------------- [ luma.metric ] ----------------------
     Accuracy, Precision, Recall, F1Score, Specificity
 
     MeanAbsoluteError, MeanSquaredError, RootMeanSquaredError,
     MeanAbsolutePercentageError, RSquaredScore,
     AdjustedRSquaredScore
```

### Comparing `luma-ml-0.8.0/luma/__init__.py` & `luma-ml-0.8.1/luma/__init__.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/classifier/discriminant.py` & `luma-ml-0.8.1/luma/classifier/discriminant.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/classifier/logistic.py` & `luma-ml-0.8.1/luma/classifier/logistic.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/classifier/naive_bayes.py` & `luma-ml-0.8.1/luma/classifier/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/classifier/neighbors.py` & `luma-ml-0.8.1/luma/classifier/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/classifier/svm.py` & `luma-ml-0.8.1/luma/classifier/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/classifier/tree.py` & `luma-ml-0.8.1/luma/classifier/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/clustering/affinity.py` & `luma-ml-0.8.1/luma/clustering/affinity.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/clustering/density.py` & `luma-ml-0.8.1/luma/clustering/density.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/clustering/hierarchy.py` & `luma-ml-0.8.1/luma/clustering/hierarchy.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/clustering/kmeans.py` & `luma-ml-0.8.1/luma/clustering/kmeans.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/clustering/mixture.py` & `luma-ml-0.8.1/luma/clustering/mixture.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/clustering/spectral.py` & `luma-ml-0.8.1/luma/clustering/spectral.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/core/base.py` & `luma-ml-0.8.1/luma/core/base.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/core/super.py` & `luma-ml-0.8.1/luma/core/super.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/ensemble/bagging.py` & `luma-ml-0.8.1/luma/ensemble/bagging.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/ensemble/boost.py` & `luma-ml-0.8.1/luma/ensemble/boost.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/ensemble/forest.py` & `luma-ml-0.8.1/luma/ensemble/forest.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/ensemble/stack.py` & `luma-ml-0.8.1/luma/ensemble/stack.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/ensemble/vote.py` & `luma-ml-0.8.1/luma/ensemble/vote.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/interface/exception.py` & `luma-ml-0.8.1/luma/interface/exception.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/interface/util.py` & `luma-ml-0.8.1/luma/interface/util.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/metric/classification.py` & `luma-ml-0.8.1/luma/metric/classification.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/metric/clustering.py` & `luma-ml-0.8.1/luma/metric/clustering.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/metric/distance.py` & `luma-ml-0.8.1/luma/metric/distance.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/metric/regression.py` & `luma-ml-0.8.1/luma/metric/regression.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/migrate/port.py` & `luma-ml-0.8.1/luma/migrate/port.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/model_selection/cv.py` & `luma-ml-0.8.1/luma/model_selection/cv.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/model_selection/fold.py` & `luma-ml-0.8.1/luma/model_selection/fold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/model_selection/search.py` & `luma-ml-0.8.1/luma/model_selection/search.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/model_selection/split.py` & `luma-ml-0.8.1/luma/model_selection/split.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/neural/_layers/_act.py` & `luma-ml-0.8.1/luma/neural/_layers/_act.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/neural/_layers/_conv.py` & `luma-ml-0.8.1/luma/neural/_layers/_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
         self,
         in_channels: int,
         out_channels: int,
         filter_size: int,
         stride: int = 1,
         padding: Literal["valid", "same"] = "same",
         initializer: InitUtil.InitStr = None,
-        optimizer: Optimizer = None,
+        optimizer: Optimizer | None = None,
         lambda_: float = 0.0,
-        random_state: int = None,
+        random_state: int | None = None,
     ) -> None:
         super().__init__()
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.filter_size = filter_size
         self.stride = stride
         self.padding = padding
@@ -51,14 +51,15 @@
                 "filter_size": ("0<,+inf", int),
                 "stride": ("0<,+inf", int),
                 "lambda_": ("0,+inf", None),
             }
         )
         self.check_param_ranges()
 
+    @Tensor.force_dim(3)
     def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
         _ = is_train
         self.input_ = X
         batch_size, channels, width = X.shape
 
         if self.in_channels != channels:
             raise ValueError(
@@ -85,14 +86,15 @@
                 result = np.fft.irfft(result_fft, n=padded_w)
 
                 out[i, f] = result[pad_w : padded_w - pad_w : self.stride][:out_width]
 
         out += self.biases_[:, :, np.newaxis]
         return out
 
+    @Tensor.force_dim(3)
     def backward(self, d_out: Tensor) -> Tensor:
         X = self.input_
         batch_size, channels, width = X.shape
         pad_w, padded_w = self._get_padding_dim(width)
 
         dX_padded = np.zeros((batch_size, channels, padded_w))
         self.dW = np.zeros_like(self.weights_)
@@ -154,17 +156,17 @@
         self,
         in_channels: int,
         out_channels: int,
         filter_size: int,
         stride: int = 1,
         padding: Literal["valid", "same"] = "same",
         initializer: InitUtil.InitStr = None,
-        optimizer: Optimizer = None,
+        optimizer: Optimizer | None = None,
         lambda_: float = 0.0,
-        random_state: int = None,
+        random_state: int | None = None,
     ) -> None:
         super().__init__()
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.filter_size = filter_size
         self.stride = stride
         self.padding = padding
@@ -190,14 +192,15 @@
                 "filter_size": ("0<,+inf", int),
                 "stride": ("0<,+inf", int),
                 "lambda_": ("0,+inf", None),
             }
         )
         self.check_param_ranges()
 
+    @Tensor.force_dim(4)
     def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
         _ = is_train
         self.input_ = X
         batch_size, channels, height, width = X.shape
 
         if self.in_channels != channels:
             raise ValueError(
@@ -237,14 +240,15 @@
                     pad_w : padded_w - pad_w : self.stride,
                 ]
                 out[i, f] = sampled_result[:out_height, :out_width]
 
         out += self.biases_[:, :, np.newaxis, np.newaxis]
         return out
 
+    @Tensor.force_dim(4)
     def backward(self, d_out: Tensor) -> Tensor:
         X = self.input_
         batch_size, channels, height, width = X.shape
         pad_h, pad_w, padded_h, padded_w = self._get_padding_dim(height, width)
 
         dX_padded = np.zeros((batch_size, channels, padded_h, padded_w))
         self.dW = np.zeros_like(self.weights_)
@@ -319,17 +323,17 @@
         self,
         in_channels: int,
         out_channels: int,
         filter_size: int,
         stride: int = 1,
         padding: Literal["valid", "same"] = "same",
         initializer: InitUtil.InitStr = None,
-        optimizer: Optimizer = None,
+        optimizer: Optimizer | None = None,
         lambda_: float = 0.0,
-        random_state: int = None,
+        random_state: int | None = None,
     ) -> None:
         super().__init__()
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.filter_size = filter_size
         self.stride = stride
         self.padding = padding
@@ -356,14 +360,15 @@
                 "filter_size": ("0<,+inf", int),
                 "stride": ("0<,+inf", int),
                 "lambda_": ("0,+inf", None),
             }
         )
         self.check_param_ranges()
 
+    @Tensor.force_dim(5)
     def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
         _ = is_train
         self.input_ = X
         batch_size, channels, depth, height, width = X.shape
 
         if self.in_channels != channels:
             raise ValueError(
@@ -408,14 +413,15 @@
                     pad_w : padded_w - pad_w : self.stride,
                 ]
                 out[i, f] = sampled_result[:out_depth, :out_height, :out_width]
 
         out += self.biases_[:, :, np.newaxis, np.newaxis, np.newaxis]
         return out
 
+    @Tensor.force_dim(5)
     def backward(self, d_out: Tensor) -> Tensor:
         X = self.input_
         batch_size, channels, depth, height, width = X.shape
         pad_d, pad_h, pad_w, padded_d, padded_h, padded_w = self._get_padding_dim(
             depth, height, width
         )
```

### Comparing `luma-ml-0.8.0/luma/neural/_layers/_linear.py` & `luma-ml-0.8.1/luma/neural/_layers/_linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/neural/_layers/_norm.py` & `luma-ml-0.8.1/luma/neural/_layers/_norm.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         self.gamma = np.ones((1, in_features, 1))
         self.beta = np.zeros((1, in_features, 1))
         self.weights_ = [self.gamma, self.beta]
 
         self.running_mean = np.zeros((1, in_features, 1))
         self.running_var = np.ones((1, in_features, 1))
 
+    @Tensor.force_dim(3)
     def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
         if is_train:
             batch_mean = np.mean(X, axis=(0, 2), keepdims=True)
             batch_var = np.var(X, axis=(0, 2), keepdims=True)
 
             self.running_mean = (
                 self.momentum * self.running_mean + (1 - self.momentum) * batch_mean
@@ -50,14 +51,15 @@
             self.X_norm = (X - self.running_mean) / np.sqrt(
                 self.running_var + self.epsilon
             )
 
         out = self.weights_[0] * self.X_norm + self.weights_[1]
         return out
 
+    @Tensor.force_dim(3)
     def backward(self, d_out: Tensor) -> Tensor:
         batch_size, _, width = d_out.shape
 
         dX_norm = d_out * self.weights_[0]
         dgamma = np.sum(d_out * self.X_norm, axis=(0, 2), keepdims=True)
         dbeta = np.sum(d_out, axis=(0, 2), keepdims=True)
         self.dW = [dgamma, dbeta]
@@ -95,14 +97,15 @@
         gamma_ = np.ones((1, in_features, 1, 1))
         beta_ = np.zeros((1, in_features, 1, 1))
         self.weights_ = [gamma_, beta_]
 
         self.running_mean = np.zeros((1, in_features, 1, 1))
         self.running_var = np.ones((1, in_features, 1, 1))
 
+    @Tensor.force_dim(4)
     def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
         if is_train:
             batch_mean = np.mean(X, axis=(0, 2, 3), keepdims=True)
             batch_var = np.var(X, axis=(0, 2, 3), keepdims=True)
 
             self.running_mean = (
                 self.momentum * self.running_mean + (1 - self.momentum) * batch_mean
@@ -116,14 +119,15 @@
             self.X_norm = (X - self.running_mean) / np.sqrt(
                 self.running_var + self.epsilon
             )
 
         out = self.weights_[0] * self.X_norm + self.weights_[1]
         return out
 
+    @Tensor.force_dim(4)
     def backward(self, d_out: Tensor) -> Tensor:
         batch_size, _, height, width = d_out.shape
         dX_norm = d_out * self.weights_[0]
 
         dgamma = np.sum(d_out * self.X_norm, axis=(0, 2, 3), keepdims=True)
         dbeta = np.sum(d_out, axis=(0, 2, 3), keepdims=True)
         self.dW = [dgamma, dbeta]
@@ -160,14 +164,15 @@
         self.gamma = np.ones((1, in_features, 1, 1, 1))
         self.beta = np.zeros((1, in_features, 1, 1, 1))
         self.weights_ = [self.gamma, self.beta]
 
         self.running_mean = np.zeros((1, in_features, 1, 1, 1))
         self.running_var = np.ones((1, in_features, 1, 1, 1))
 
+    @Tensor.force_dim(5)
     def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
         if is_train:
             batch_mean = np.mean(X, axis=(0, 2, 3, 4), keepdims=True)
             batch_var = np.var(X, axis=(0, 2, 3, 4), keepdims=True)
 
             self.running_mean = (
                 self.momentum * self.running_mean + (1 - self.momentum) * batch_mean
@@ -181,14 +186,15 @@
             self.X_norm = (X - self.running_mean) / np.sqrt(
                 self.running_var + self.epsilon
             )
 
         out = self.weights_[0] * self.X_norm + self.weights_[1]
         return out
 
+    @Tensor.force_dim(5)
     def backward(self, d_out: Tensor) -> Tensor:
         batch_size, _, depth, height, width = d_out.shape
 
         dX_norm = d_out * self.weights_[0]
         dgamma = np.sum(d_out * self.X_norm, axis=(0, 2, 3, 4), keepdims=True)
         dbeta = np.sum(d_out, axis=(0, 2, 3, 4), keepdims=True)
         self.dW = [dgamma, dbeta]
```

### Comparing `luma-ml-0.8.0/luma/neural/_layers/_pool.py` & `luma-ml-0.8.1/luma/neural/_layers/_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
             {
                 "filter_size": ("0<,+inf", int),
                 "stride": ("0<,+inf", int),
             }
         )
         self.check_param_ranges()
 
+    @Tensor.force_dim(3)
     def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
         _ = is_train
         self.input_ = X
         batch_size, channels, width = X.shape
 
         out_width = 1 + (width - self.filter_size) // self.stride
         out: Tensor = np.zeros((batch_size, channels, out_width))
@@ -46,14 +47,15 @@
             elif self.mode == "avg":
                 out[:, :, i] = np.mean(window, axis=2)
             else:
                 raise UnsupportedParameterError(self.mode)
 
         return out
 
+    @Tensor.force_dim(3)
     def backward(self, d_out: Tensor) -> Tensor:
         X = self.input_
         _, _, out_width = d_out.shape
         self.dX = np.zeros_like(X)
 
         for i in range(out_width):
             w_start, w_end = self._get_pooling_bounds(i)
@@ -99,14 +101,15 @@
             {
                 "filter_size": ("0<,+inf", int),
                 "stride": ("0<,+inf", int),
             }
         )
         self.check_param_ranges()
 
+    @Tensor.force_dim(4)
     def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
         _ = is_train
         self.input_ = X
         batch_size, channels, height, width = X.shape
 
         out_height = 1 + (height - self.filter_size) // self.stride
         out_width = 1 + (width - self.filter_size) // self.stride
@@ -122,14 +125,15 @@
                 elif self.mode == "avg":
                     out[:, :, i, j] = np.mean(window, axis=(2, 3))
                 else:
                     raise UnsupportedParameterError(self.mode)
 
         return out
 
+    @Tensor.force_dim(4)
     def backward(self, d_out: Tensor) -> Tensor:
         X = self.input_
         _, _, out_height, out_width = d_out.shape
         self.dX = np.zeros_like(X)
 
         for i in range(out_height):
             for j in range(out_width):
@@ -182,14 +186,15 @@
             {
                 "filter_size": ("0<,+inf", int),
                 "stride": ("0<,+inf", int),
             }
         )
         self.check_param_ranges()
 
+    @Tensor.force_dim(5)
     def forward(self, X: Tensor, is_train: bool = False) -> Tensor:
         _ = is_train
         self.input_ = X
         batch_size, channels, depth, height, width = X.shape
 
         out_depth = 1 + (depth - self.filter_size) // self.stride
         out_height = 1 + (height - self.filter_size) // self.stride
@@ -217,14 +222,15 @@
                     elif self.mode == "avg":
                         out[:, :, i, j, k] = np.mean(window, axis=(2, 3, 4))
                     else:
                         raise UnsupportedParameterError(self.mode)
 
         return out
 
+    @Tensor.force_dim(5)
     def backward(self, d_out: Tensor) -> Tensor:
         X = self.input_
         _, _, out_depth, out_height, out_width = d_out.shape
         self.dX = np.zeros_like(X)
 
         for i in range(out_depth):
             for j in range(out_height):
```

### Comparing `luma-ml-0.8.0/luma/neural/_models/_imagenet.py` & `luma-ml-0.8.1/luma/neural/_models/_lenet.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,160 @@
 from typing import Self, override
 
 from luma.core.super import Estimator, Evaluator, Optimizer, Supervised
 from luma.interface.typing import Matrix, Tensor, Vector
-from luma.interface.util import Clone, InitUtil
+from luma.interface.util import InitUtil
 from luma.metric.classification import Accuracy
 
 from luma.neural.base import Loss, NeuralModel
-from luma.neural.loss import CrossEntropy
 from luma.neural.block import ConvBlock2D, DenseBlock
-from luma.neural.layer import (
-    Activation,
-    Dense,
-    Flatten,
-    LocalResponseNorm,
-    Sequential,
-)
+from luma.neural.layer import Activation, Dense, Flatten, Sequential
+from luma.neural.loss import CrossEntropy
+
+
+__all__ = ("_LeNet_1", "_LeNet_4", "_LeNet_5")
+
+
+class _LeNet_1(Estimator, Supervised, NeuralModel):
+    def __init__(
+        self,
+        optimizer: Optimizer,
+        activation: Activation.FuncType = Activation.Tanh,
+        loss: Loss = CrossEntropy(),
+        initializer: InitUtil.InitStr = None,
+        out_features: int = 10,
+        batch_size: int = 100,
+        n_epochs: int = 100,
+        learning_rate: float = 0.01,
+        valid_size: float = 0.1,
+        lambda_: float = 0.0,
+        early_stopping: bool = False,
+        patience: int = 10,
+        shuffle: bool = True,
+        random_state: int = None,
+        deep_verbose: bool = False,
+    ) -> None:
+        self.activation = activation
+        self.optimizer = optimizer
+        self.loss = loss
+        self.initializer = initializer
+        self.out_features = out_features
+        self.lambda_ = lambda_
+        self.shuffle = shuffle
+        self.random_state = random_state
+        self._fitted = False
+
+        super().__init__(
+            batch_size,
+            n_epochs,
+            learning_rate,
+            valid_size,
+            early_stopping,
+            patience,
+            deep_verbose,
+        )
+        super().__init_model__()
+        self.model = Sequential()
+        self.optimizer.set_params(learning_rate=self.learning_rate)
+        self.model.set_optimizer(optimizer=self.optimizer)
+
+        self.feature_sizes_ = [
+            [1, 4, 8],
+            [8 * 4 * 4, self.out_features],
+        ]
+        self.feature_shapes_ = [
+            [(1, 4), (4, 8)],
+            [(8 * 4 * 4, self.out_features)],
+        ]
+
+        self.set_param_ranges(
+            {
+                "out_features": ("0<,+inf", int),
+                "batch_size": ("0<,+inf", int),
+                "n_epochs": ("0<,+inf", int),
+                "learning_rate": ("0<,+inf", None),
+                "valid_size": ("0<,<1", None),
+                "dropout_rate": ("0,1", None),
+                "lambda_": ("0,+inf", None),
+                "patience": (f"0<,+inf", int),
+            }
+        )
+        self.check_param_ranges()
+        self._build_model()
+
+    def _build_model(self) -> None:
+        self.model += ConvBlock2D(
+            1,
+            4,
+            filter_size=5,
+            stride=1,
+            activation=self.activation,
+            initializer=self.initializer,
+            padding="valid",
+            lambda_=self.lambda_,
+            do_batch_norm=False,
+            pool_filter_size=2,
+            pool_stride=2,
+            pool_mode="avg",
+            random_state=self.random_state,
+        )
+        self.model += ConvBlock2D(
+            4,
+            8,
+            filter_size=5,
+            stride=1,
+            activation=self.activation,
+            initializer=self.initializer,
+            padding="valid",
+            lambda_=self.lambda_,
+            do_batch_norm=False,
+            pool_filter_size=2,
+            pool_stride=2,
+            pool_mode="avg",
+            random_state=self.random_state,
+        )
+
+        self.model += Flatten()
+        self.model += Dense(
+            8 * 4 * 4,
+            self.out_features,
+            lambda_=self.lambda_,
+            random_state=self.random_state,
+        )
+
+    @Tensor.force_dim(4)
+    def fit(self, X: Tensor, y: Matrix) -> Self:
+        return super(_LeNet_1, self).fit_nn(X, y)
 
+    @override
+    @Tensor.force_dim(4)
+    def predict(self, X: Tensor, argmax: bool = True) -> Matrix | Vector:
+        return super(_LeNet_1, self).predict_nn(X, argmax)
 
-__all__ = ("_AlexNet", "_ZFNet")
+    @override
+    @Tensor.force_dim(4)
+    def score(
+        self,
+        X: Tensor,
+        y: Matrix,
+        metric: Evaluator = Accuracy,
+        argmax: bool = True,
+    ) -> float:
+        return super(_LeNet_1, self).score_nn(X, y, metric, argmax)
 
 
-class _AlexNet(Estimator, Supervised, NeuralModel):
+class _LeNet_4(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
         optimizer: Optimizer,
-        activation: Activation.FuncType = Activation.ReLU(),
+        activation: Activation.FuncType = Activation.Tanh,
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
-        out_features: int = 1000,
-        batch_size: int = 128,
+        out_features: int = 10,
+        batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
         dropout_rate: float = 0.5,
         early_stopping: bool = False,
         patience: int = 10,
@@ -62,20 +184,20 @@
         )
         super().__init_model__()
         self.model = Sequential()
         self.optimizer.set_params(learning_rate=self.learning_rate)
         self.model.set_optimizer(optimizer=self.optimizer)
 
         self.feature_sizes_ = [
-            [3, 96, 256, 384, 384, 256],
-            [256 * 6 * 6, 4096, 4096, self.out_features],
+            [1, 4, 16],
+            [16 * 5 * 5, 120, self.out_features],
         ]
         self.feature_shapes_ = [
-            self._get_feature_shapes(self.feature_sizes_[0]),
-            self._get_feature_shapes(self.feature_sizes_[1]),
+            [(1, 4), (4, 16)],
+            [(16 * 5 * 5, 120), (120, self.out_features)],
         ]
 
         self.set_param_ranges(
             {
                 "out_features": ("0<,+inf", int),
                 "batch_size": ("0<,+inf", int),
                 "n_epochs": ("0<,+inf", int),
@@ -86,184 +208,92 @@
                 "patience": (f"0<,+inf", int),
             }
         )
         self.check_param_ranges()
         self._build_model()
 
     def _build_model(self) -> None:
-        self.model += (
-            "ConvBlock_1",
-            ConvBlock2D(
-                3,
-                96,
-                filter_size=11,
-                stride=4,
-                activation=Clone(self.activation).get,
-                initializer=self.initializer,
-                padding="valid",
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                pool_filter_size=3,
-                pool_stride=2,
-                pool_mode="max",
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "LRN_1",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += (
-            "ConvBlock_2",
-            ConvBlock2D(
-                96,
-                256,
-                filter_size=5,
-                stride=1,
-                activation=Clone(self.activation).get,
-                initializer=self.initializer,
-                padding="same",
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                pool_filter_size=3,
-                pool_stride=2,
-                pool_mode="max",
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "LRN_2",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += (
-            "ConvBlock_3",
-            ConvBlock2D(
-                256,
-                384,
-                filter_size=3,
-                stride=1,
-                activation=Clone(self.activation).get,
-                initializer=self.initializer,
-                padding="same",
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                do_pooling=False,
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "LRN_3",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += (
-            "ConvBlock_4",
-            ConvBlock2D(
-                384,
-                384,
-                filter_size=3,
-                stride=1,
-                activation=Clone(self.activation).get,
-                initializer=self.initializer,
-                padding="same",
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                do_pooling=False,
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "LRN_4",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += (
-            "ConvBlock_5",
-            ConvBlock2D(
-                384,
-                256,
-                filter_size=3,
-                stride=1,
-                activation=Clone(self.activation).get,
-                initializer=self.initializer,
-                padding="same",
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                pool_filter_size=3,
-                pool_stride=2,
-                pool_mode="max",
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "LRN_5",
-            LocalResponseNorm(depth=5),
+        self.model += ConvBlock2D(
+            1,
+            4,
+            filter_size=5,
+            stride=1,
+            activation=self.activation,
+            initializer=self.initializer,
+            padding="valid",
+            lambda_=self.lambda_,
+            do_batch_norm=False,
+            pool_filter_size=2,
+            pool_stride=2,
+            pool_mode="avg",
+            random_state=self.random_state,
+        )
+        self.model += ConvBlock2D(
+            4,
+            16,
+            filter_size=5,
+            stride=1,
+            activation=self.activation,
+            initializer=self.initializer,
+            padding="valid",
+            lambda_=self.lambda_,
+            do_batch_norm=False,
+            pool_filter_size=2,
+            pool_stride=2,
+            pool_mode="avg",
+            random_state=self.random_state,
         )
 
         self.model += Flatten()
-        self.model += (
-            "DenseBlock_1",
-            DenseBlock(
-                256 * 6 * 6,
-                4096,
-                activation=Clone(self.activation).get,
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                dropout_rate=self.dropout_rate,
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "DenseBlock_2",
-            DenseBlock(
-                4096,
-                4096,
-                activation=Clone(self.activation).get,
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                dropout_rate=self.dropout_rate,
-                random_state=self.random_state,
-            ),
+        self.model += DenseBlock(
+            16 * 5 * 5,
+            120,
+            activation=self.activation,
+            lambda_=self.lambda_,
+            do_batch_norm=False,
+            do_dropout=False,
+            random_state=self.random_state,
         )
         self.model += Dense(
-            4096,
+            120,
             self.out_features,
             lambda_=self.lambda_,
             random_state=self.random_state,
         )
 
+    @Tensor.force_dim(4)
     def fit(self, X: Tensor, y: Matrix) -> Self:
-        return super(_AlexNet, self).fit_nn(X, y)
+        return super(_LeNet_4, self).fit_nn(X, y)
 
     @override
+    @Tensor.force_dim(4)
     def predict(self, X: Tensor, argmax: bool = True) -> Matrix | Vector:
-        return super(_AlexNet, self).predict_nn(X, argmax)
+        return super(_LeNet_4, self).predict_nn(X, argmax)
 
     @override
+    @Tensor.force_dim(4)
     def score(
         self,
         X: Tensor,
         y: Matrix,
         metric: Evaluator = Accuracy,
         argmax: bool = True,
     ) -> float:
-        return super(_AlexNet, self).score_nn(X, y, metric, argmax)
+        return super(_LeNet_4, self).score_nn(X, y, metric, argmax)
 
 
-class _ZFNet(Estimator, Supervised, NeuralModel):
+class _LeNet_5(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
         optimizer: Optimizer,
-        activation: Activation.FuncType = Activation.ReLU(),
+        activation: Activation.FuncType = Activation.Tanh,
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
-        out_features: int = 1000,
-        batch_size: int = 128,
+        out_features: int = 10,
+        batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
         dropout_rate: float = 0.5,
         early_stopping: bool = False,
         patience: int = 10,
@@ -293,20 +323,20 @@
         )
         super().__init_model__()
         self.model = Sequential()
         self.optimizer.set_params(learning_rate=self.learning_rate)
         self.model.set_optimizer(optimizer=self.optimizer)
 
         self.feature_sizes_ = [
-            [3, 96, 256, 384, 384, 256],
-            [256 * 6 * 6, 4096, 4096, self.out_features],
+            [1, 6, 16],
+            [16 * 5 * 5, 120, 84, self.out_features],
         ]
         self.feature_shapes_ = [
-            self._get_feature_shapes(self.feature_sizes_[0]),
-            self._get_feature_shapes(self.feature_sizes_[1]),
+            [(1, 6), (6, 16)],
+            [(16 * 5 * 5, 120), (120, 84), (84, self.out_features)],
         ]
 
         self.set_param_ranges(
             {
                 "out_features": ("0<,+inf", int),
                 "batch_size": ("0<,+inf", int),
                 "n_epochs": ("0<,+inf", int),
@@ -317,166 +347,83 @@
                 "patience": (f"0<,+inf", int),
             }
         )
         self.check_param_ranges()
         self._build_model()
 
     def _build_model(self) -> None:
-        self.model += (
-            "ConvBlock_1",
-            ConvBlock2D(
-                3,
-                96,
-                filter_size=7,
-                stride=2,
-                activation=Clone(self.activation).get,
-                initializer=self.initializer,
-                padding="valid",
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                pool_filter_size=3,
-                pool_stride=2,
-                pool_mode="max",
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "LRN_1",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += (
-            "ConvBlock_2",
-            ConvBlock2D(
-                96,
-                256,
-                filter_size=5,
-                stride=2,
-                activation=Clone(self.activation).get,
-                initializer=self.initializer,
-                padding="same",
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                pool_filter_size=3,
-                pool_stride=2,
-                pool_mode="max",
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "LRN_2",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += (
-            "ConvBlock_3",
-            ConvBlock2D(
-                256,
-                384,
-                filter_size=3,
-                stride=1,
-                activation=Clone(self.activation).get,
-                initializer=self.initializer,
-                padding="same",
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                do_pooling=False,
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "LRN_3",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += (
-            "ConvBlock_4",
-            ConvBlock2D(
-                384,
-                384,
-                filter_size=3,
-                stride=1,
-                activation=Clone(self.activation).get,
-                initializer=self.initializer,
-                padding="same",
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                do_pooling=False,
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "LRN_4",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += (
-            "ConvBlock_5",
-            ConvBlock2D(
-                384,
-                256,
-                filter_size=3,
-                stride=1,
-                activation=Clone(self.activation).get,
-                initializer=self.initializer,
-                padding="same",
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                pool_filter_size=3,
-                pool_stride=2,
-                pool_mode="max",
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "LRN_5",
-            LocalResponseNorm(depth=5),
+        self.model += ConvBlock2D(
+            1,
+            6,
+            filter_size=5,
+            stride=1,
+            activation=self.activation,
+            initializer=self.initializer,
+            padding="valid",
+            lambda_=self.lambda_,
+            do_batch_norm=False,
+            pool_filter_size=2,
+            pool_stride=2,
+            pool_mode="avg",
+            random_state=self.random_state,
+        )
+        self.model += ConvBlock2D(
+            6,
+            16,
+            filter_size=5,
+            stride=1,
+            activation=self.activation,
+            initializer=self.initializer,
+            padding="valid",
+            lambda_=self.lambda_,
+            do_batch_norm=False,
+            pool_filter_size=2,
+            pool_stride=2,
+            pool_mode="avg",
+            random_state=self.random_state,
         )
 
         self.model += Flatten()
-        self.model += (
-            "DenseBlock_1",
-            DenseBlock(
-                256 * 6 * 6,
-                4096,
-                activation=Clone(self.activation).get,
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                dropout_rate=self.dropout_rate,
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "DenseBlock_2",
-            DenseBlock(
-                4096,
-                4096,
-                activation=Clone(self.activation).get,
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                dropout_rate=self.dropout_rate,
-                random_state=self.random_state,
-            ),
+        self.model += DenseBlock(
+            16 * 5 * 5,
+            120,
+            activation=self.activation,
+            lambda_=self.lambda_,
+            do_batch_norm=False,
+            do_dropout=False,
+            random_state=self.random_state,
+        )
+        self.model += DenseBlock(
+            120,
+            84,
+            activation=self.activation,
+            lambda_=self.lambda_,
+            do_batch_norm=False,
+            do_dropout=False,
+            random_state=self.random_state,
         )
         self.model += Dense(
-            4096,
+            84,
             self.out_features,
             lambda_=self.lambda_,
             random_state=self.random_state,
         )
 
+    @Tensor.force_dim(4)
     def fit(self, X: Tensor, y: Matrix) -> Self:
-        return super(_ZFNet, self).fit_nn(X, y)
+        return super(_LeNet_5, self).fit_nn(X, y)
 
     @override
+    @Tensor.force_dim(4)
     def predict(self, X: Tensor, argmax: bool = True) -> Matrix | Vector:
-        return super(_ZFNet, self).predict_nn(X, argmax)
+        return super(_LeNet_5, self).predict_nn(X, argmax)
 
     @override
+    @Tensor.force_dim(4)
     def score(
         self,
         X: Tensor,
         y: Matrix,
         metric: Evaluator = Accuracy,
         argmax: bool = True,
     ) -> float:
-        return super(_ZFNet, self).score_nn(X, y, metric, argmax)
+        return super(_LeNet_5, self).score_nn(X, y, metric, argmax)
```

### Comparing `luma-ml-0.8.0/luma/neural/_models/_lenet.py` & `luma-ml-0.8.1/luma/neural/_models/_simple.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,178 +1,56 @@
-from typing import Self, override
+from typing import Literal, Self, override
 
 from luma.core.super import Estimator, Evaluator, Optimizer, Supervised
 from luma.interface.typing import Matrix, Tensor, Vector
-from luma.interface.util import Clone, InitUtil
-from luma.metric.classification import Accuracy
+from luma.interface.util import InitUtil
 
 from luma.neural.base import Loss, NeuralModel
 from luma.neural.block import ConvBlock2D, DenseBlock
-from luma.neural.layer import Activation, Dense, Flatten, Sequential
-from luma.neural.loss import CrossEntropy
+from luma.neural.layer import Activation, Dense, Dropout, Flatten, Sequential
 
 
-__all__ = ("_LeNet_1", "_LeNet_4", "_LeNet_5")
+__all__ = ("_SimpleMLP", "_SimpleCNN")
 
 
-class _LeNet_1(Estimator, Supervised, NeuralModel):
+class _SimpleMLP(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
+        in_features: int,
+        out_features: int,
+        hidden_layers: list[int] | int,
+        *,
+        activation: Activation.FuncType,
         optimizer: Optimizer,
-        activation: Activation.FuncType = Activation.Tanh(),
-        loss: Loss = CrossEntropy(),
+        loss: Loss,
         initializer: InitUtil.InitStr = None,
-        out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
-        learning_rate: float = 0.01,
+        learning_rate: float = 0.001,
         valid_size: float = 0.1,
+        dropout_rate: float = 0.5,
         lambda_: float = 0.0,
         early_stopping: bool = False,
         patience: int = 10,
         shuffle: bool = True,
         random_state: int = None,
         deep_verbose: bool = False,
     ) -> None:
-        self.activation = activation
-        self.optimizer = optimizer
-        self.loss = loss
-        self.initializer = initializer
+        self.in_features = in_features
         self.out_features = out_features
-        self.lambda_ = lambda_
-        self.shuffle = shuffle
-        self.random_state = random_state
-        self._fitted = False
-
-        super().__init__(
-            batch_size,
-            n_epochs,
-            learning_rate,
-            valid_size,
-            early_stopping,
-            patience,
-            deep_verbose,
-        )
-        super().__init_model__()
-        self.model = Sequential()
-        self.optimizer.set_params(learning_rate=self.learning_rate)
-        self.model.set_optimizer(optimizer=self.optimizer)
-
-        self.feature_sizes_ = [
-            [1, 4, 8],
-            [8 * 4 * 4, self.out_features],
-        ]
-        self.feature_shapes_ = [
-            [(1, 4), (4, 8)],
-            [(8 * 4 * 4, self.out_features)],
-        ]
-
-        self.set_param_ranges(
-            {
-                "out_features": ("0<,+inf", int),
-                "batch_size": ("0<,+inf", int),
-                "n_epochs": ("0<,+inf", int),
-                "learning_rate": ("0<,+inf", None),
-                "valid_size": ("0<,<1", None),
-                "dropout_rate": ("0,1", None),
-                "lambda_": ("0,+inf", None),
-                "patience": (f"0<,+inf", int),
-            }
-        )
-        self.check_param_ranges()
-        self._build_model()
-
-    def _build_model(self) -> None:
-        self.model += ConvBlock2D(
-            1,
-            4,
-            filter_size=5,
-            stride=1,
-            activation=Clone(self.activation).get,
-            initializer=self.initializer,
-            padding="valid",
-            lambda_=self.lambda_,
-            do_batch_norm=False,
-            pool_filter_size=2,
-            pool_stride=2,
-            pool_mode="avg",
-            random_state=self.random_state,
-        )
-        self.model += ConvBlock2D(
-            4,
-            8,
-            filter_size=5,
-            stride=1,
-            activation=Clone(self.activation).get,
-            initializer=self.initializer,
-            padding="valid",
-            lambda_=self.lambda_,
-            do_batch_norm=False,
-            pool_filter_size=2,
-            pool_stride=2,
-            pool_mode="avg",
-            random_state=self.random_state,
-        )
-
-        self.model += Flatten()
-        self.model += Dense(
-            8 * 4 * 4,
-            self.out_features,
-            lambda_=self.lambda_,
-            random_state=self.random_state,
-        )
-
-    def fit(self, X: Tensor, y: Matrix) -> Self:
-        return super(_LeNet_1, self).fit_nn(X, y)
-
-    @override
-    def predict(self, X: Tensor, argmax: bool = True) -> Matrix | Vector:
-        return super(_LeNet_1, self).predict_nn(X, argmax)
-
-    @override
-    def score(
-        self,
-        X: Tensor,
-        y: Matrix,
-        metric: Evaluator = Accuracy,
-        argmax: bool = True,
-    ) -> float:
-        return super(_LeNet_1, self).score_nn(X, y, metric, argmax)
-
-
-class _LeNet_4(Estimator, Supervised, NeuralModel):
-    def __init__(
-        self,
-        optimizer: Optimizer,
-        activation: Activation.FuncType = Activation.Tanh(),
-        loss: Loss = CrossEntropy(),
-        initializer: InitUtil.InitStr = None,
-        out_features: int = 10,
-        batch_size: int = 100,
-        n_epochs: int = 100,
-        learning_rate: float = 0.01,
-        valid_size: float = 0.1,
-        lambda_: float = 0.0,
-        dropout_rate: float = 0.5,
-        early_stopping: bool = False,
-        patience: int = 10,
-        shuffle: bool = True,
-        random_state: int = None,
-        deep_verbose: bool = False,
-    ) -> None:
+        self.hidden_layers = hidden_layers
+        self.initializer = initializer
         self.activation = activation
         self.optimizer = optimizer
         self.loss = loss
-        self.initializer = initializer
-        self.out_features = out_features
-        self.lambda_ = lambda_
         self.dropout_rate = dropout_rate
+        self.lambda_ = lambda_
         self.shuffle = shuffle
         self.random_state = random_state
-        self._fitted = False
+        self.fitted_ = False
 
         super().__init__(
             batch_size,
             n_epochs,
             learning_rate,
             valid_size,
             early_stopping,
@@ -180,132 +58,124 @@
             deep_verbose,
         )
         super().__init_model__()
         self.model = Sequential()
         self.optimizer.set_params(learning_rate=self.learning_rate)
         self.model.set_optimizer(optimizer=self.optimizer)
 
+        if isinstance(self.hidden_layers, int):
+            self.hidden_layers = [self.hidden_layers]
+
         self.feature_sizes_ = [
-            [1, 4, 16],
-            [16 * 5 * 5, 120, self.out_features],
-        ]
-        self.feature_shapes_ = [
-            [(1, 4), (4, 16)],
-            [(16 * 5 * 5, 120), (120, self.out_features)],
+            self.in_features,
+            *self.hidden_layers,
+            self.out_features,
         ]
+        self.feature_shapes_ = self._get_feature_shapes(self.feature_sizes_)
 
         self.set_param_ranges(
             {
+                "in_features": ("0<,+inf", int),
                 "out_features": ("0<,+inf", int),
                 "batch_size": ("0<,+inf", int),
                 "n_epochs": ("0<,+inf", int),
                 "learning_rate": ("0<,+inf", None),
                 "valid_size": ("0<,<1", None),
                 "dropout_rate": ("0,1", None),
                 "lambda_": ("0,+inf", None),
                 "patience": (f"0<,+inf", int),
             }
         )
         self.check_param_ranges()
         self._build_model()
 
     def _build_model(self) -> None:
-        self.model += ConvBlock2D(
-            1,
-            4,
-            filter_size=5,
-            stride=1,
-            activation=Clone(self.activation).get,
-            initializer=self.initializer,
-            padding="valid",
-            lambda_=self.lambda_,
-            do_batch_norm=False,
-            pool_filter_size=2,
-            pool_stride=2,
-            pool_mode="avg",
-            random_state=self.random_state,
-        )
-        self.model += ConvBlock2D(
-            4,
-            16,
-            filter_size=5,
-            stride=1,
-            activation=Clone(self.activation).get,
-            initializer=self.initializer,
-            padding="valid",
-            lambda_=self.lambda_,
-            do_batch_norm=False,
-            pool_filter_size=2,
-            pool_stride=2,
-            pool_mode="avg",
-            random_state=self.random_state,
-        )
-
-        self.model += Flatten()
-        self.model += DenseBlock(
-            16 * 5 * 5,
-            120,
-            activation=Clone(self.activation).get,
-            lambda_=self.lambda_,
-            do_batch_norm=False,
-            do_dropout=False,
-            random_state=self.random_state,
-        )
-        self.model += Dense(
-            120,
-            self.out_features,
-            lambda_=self.lambda_,
-            random_state=self.random_state,
-        )
+        for i, (in_, out_) in enumerate(self.feature_shapes_):
+            self.model += Dense(
+                in_,
+                out_,
+                initializer=self.initializer,
+                lambda_=self.lambda_,
+                random_state=self.random_state,
+            )
+            if i < len(self.feature_shapes_) - 1:
+                self.model += self.activation()
+                self.model += Dropout(
+                    dropout_rate=self.dropout_rate,
+                    random_state=self.random_state,
+                )
 
-    def fit(self, X: Tensor, y: Matrix) -> Self:
-        return super(_LeNet_4, self).fit_nn(X, y)
+    def fit(self, X: Matrix, y: Matrix) -> Self:
+        return super(_SimpleMLP, self).fit_nn(X, y)
 
     @override
-    def predict(self, X: Tensor, argmax: bool = True) -> Matrix | Vector:
-        return super(_LeNet_4, self).predict_nn(X, argmax)
+    def predict(self, X: Matrix, argmax: bool = True) -> Matrix | Vector:
+        return super(_SimpleMLP, self).predict_nn(X, argmax)
 
     @override
     def score(
-        self,
-        X: Tensor,
-        y: Matrix,
-        metric: Evaluator = Accuracy,
-        argmax: bool = True,
+        self, X: Matrix, y: Matrix, metric: Evaluator, argmax: bool = True
     ) -> float:
-        return super(_LeNet_4, self).score_nn(X, y, metric, argmax)
+        return super(_SimpleMLP, self).score_nn(X, y, metric, argmax)
 
 
-class _LeNet_5(Estimator, Supervised, NeuralModel):
+class _SimpleCNN(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
+        in_channels_list: list[int] | int,
+        in_features_list: list[int] | int,
+        out_channels: int,
+        out_features: int,
+        filter_size: int,
+        *,
+        activation: Activation.FuncType,
         optimizer: Optimizer,
-        activation: Activation.FuncType = Activation.Tanh(),
-        loss: Loss = CrossEntropy(),
+        loss: Loss,
         initializer: InitUtil.InitStr = None,
-        out_features: int = 10,
+        padding: Literal["same", "valid"] = "same",
+        stride: int = 1,
+        do_batch_norm: bool = True,
+        momentum: float = 0.9,
+        do_pooling: bool = True,
+        pool_filter_size: int = 2,
+        pool_stride: int = 2,
+        pool_mode: Literal["max", "avg"] = "max",
+        do_dropout: bool = True,
+        dropout_rate: float = 0.5,
         batch_size: int = 100,
         n_epochs: int = 100,
-        learning_rate: float = 0.01,
+        learning_rate: float = 0.001,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
-        dropout_rate: float = 0.5,
         early_stopping: bool = False,
         patience: int = 10,
         shuffle: bool = True,
         random_state: int = None,
         deep_verbose: bool = False,
     ) -> None:
+        self.in_channels_list = in_channels_list
+        self.in_features_list = in_features_list
+        self.out_channels = out_channels
+        self.out_features = out_features
+        self.filter_size = filter_size
         self.activation = activation
         self.optimizer = optimizer
         self.loss = loss
         self.initializer = initializer
-        self.out_features = out_features
-        self.lambda_ = lambda_
+        self.padding = padding
+        self.stride = stride
+        self.do_batch_norm = do_batch_norm
+        self.momentum = momentum
+        self.do_pooling = do_pooling
+        self.pool_filter_size = pool_filter_size
+        self.pool_stride = pool_stride
+        self.pool_mode = pool_mode
+        self.do_dropout = do_dropout
         self.dropout_rate = dropout_rate
+        self.lambda_ = lambda_
         self.shuffle = shuffle
         self.random_state = random_state
         self._fitted = False
 
         super().__init__(
             batch_size,
             n_epochs,
@@ -316,105 +186,98 @@
             deep_verbose,
         )
         super().__init_model__()
         self.model = Sequential()
         self.optimizer.set_params(learning_rate=self.learning_rate)
         self.model.set_optimizer(optimizer=self.optimizer)
 
+        if isinstance(self.in_channels_list, int):
+            self.in_channels_list = [self.in_channels_list]
+        if isinstance(self.in_features_list, int):
+            self.in_features_list = [self.in_features_list]
+
         self.feature_sizes_ = [
-            [1, 6, 16],
-            [16 * 5 * 5, 120, 84, self.out_features],
+            [*self.in_channels_list, self.out_channels],
+            [*self.in_features_list, self.out_features],
         ]
         self.feature_shapes_ = [
-            [(1, 6), (6, 16)],
-            [(16 * 5 * 5, 120), (120, 84), (84, self.out_features)],
+            [*self._get_feature_shapes(self.feature_sizes_[0])],
+            [*self._get_feature_shapes(self.feature_sizes_[1])],
         ]
 
         self.set_param_ranges(
             {
+                "out_channels": ("0<,+inf", int),
                 "out_features": ("0<,+inf", int),
+                "filter_size": ("0<,+inf", int),
+                "stride": ("0<,+inf", int),
+                "momentum": ("0,1", None),
+                "pool_filter_size": ("0<,+inf", int),
+                "pool_stride": ("0<,+inf", int),
+                "dropout_rate": ("0,1", None),
                 "batch_size": ("0<,+inf", int),
                 "n_epochs": ("0<,+inf", int),
                 "learning_rate": ("0<,+inf", None),
                 "valid_size": ("0<,<1", None),
                 "dropout_rate": ("0,1", None),
                 "lambda_": ("0,+inf", None),
                 "patience": (f"0<,+inf", int),
             }
         )
         self.check_param_ranges()
         self._build_model()
 
     def _build_model(self) -> None:
-        self.model += ConvBlock2D(
-            1,
-            6,
-            filter_size=5,
-            stride=1,
-            activation=Clone(self.activation).get,
-            initializer=self.initializer,
-            padding="valid",
-            lambda_=self.lambda_,
-            do_batch_norm=False,
-            pool_filter_size=2,
-            pool_stride=2,
-            pool_mode="avg",
-            random_state=self.random_state,
-        )
-        self.model += ConvBlock2D(
-            6,
-            16,
-            filter_size=5,
-            stride=1,
-            activation=Clone(self.activation).get,
-            initializer=self.initializer,
-            padding="valid",
-            lambda_=self.lambda_,
-            do_batch_norm=False,
-            pool_filter_size=2,
-            pool_stride=2,
-            pool_mode="avg",
-            random_state=self.random_state,
-        )
+        for in_, out_ in self.feature_shapes_[0]:
+            self.model += ConvBlock2D(
+                in_,
+                out_,
+                self.filter_size,
+                activation=self.activation,
+                initializer=self.initializer,
+                padding=self.padding,
+                stride=self.stride,
+                lambda_=self.lambda_,
+                do_batch_norm=self.do_batch_norm,
+                momentum=self.momentum,
+                do_pooling=self.do_pooling,
+                pool_filter_size=self.pool_filter_size,
+                pool_stride=self.pool_stride,
+                pool_mode=self.pool_mode,
+                random_state=self.random_state,
+            )
 
         self.model += Flatten()
-        self.model += DenseBlock(
-            16 * 5 * 5,
-            120,
-            activation=Clone(self.activation).get,
-            lambda_=self.lambda_,
-            do_batch_norm=False,
-            do_dropout=False,
-            random_state=self.random_state,
-        )
-        self.model += DenseBlock(
-            120,
-            84,
-            activation=Clone(self.activation).get,
-            lambda_=self.lambda_,
-            do_batch_norm=False,
-            do_dropout=False,
-            random_state=self.random_state,
-        )
-        self.model += Dense(
-            84,
-            self.out_features,
-            lambda_=self.lambda_,
-            random_state=self.random_state,
-        )
+        for i, (in_, out_) in enumerate(self.feature_shapes_[1]):
+            if i < len(self.feature_shapes_[1]) - 1:
+                self.model += DenseBlock(
+                    in_,
+                    out_,
+                    activation=self.activation,
+                    lambda_=self.lambda_,
+                    do_dropout=self.do_dropout,
+                    dropout_rate=self.dropout_rate,
+                    random_state=self.random_state,
+                )
+            else:
+                self.model += Dense(
+                    in_,
+                    out_,
+                    lambda_=self.lambda_,
+                    random_state=self.random_state,
+                )
 
+    @Tensor.force_dim(4)
     def fit(self, X: Tensor, y: Matrix) -> Self:
-        return super(_LeNet_5, self).fit_nn(X, y)
+        return super(_SimpleCNN, self).fit_nn(X, y)
 
     @override
+    @Tensor.force_dim(4)
     def predict(self, X: Tensor, argmax: bool = True) -> Matrix | Vector:
-        return super(_LeNet_5, self).predict_nn(X, argmax)
+        return super(_SimpleCNN, self).predict_nn(X, argmax)
 
     @override
+    @Tensor.force_dim(4)
     def score(
-        self,
-        X: Tensor,
-        y: Matrix,
-        metric: Evaluator = Accuracy,
-        argmax: bool = True,
+        self, X: Tensor, y: Matrix, metric: Evaluator, argmax: bool = True
     ) -> float:
-        return super(_LeNet_5, self).score_nn(X, y, metric, argmax)
+        return super(_SimpleCNN, self).score_nn(X, y, metric, argmax)
```

### Comparing `luma-ml-0.8.0/luma/neural/base.py` & `luma-ml-0.8.1/luma/neural/base.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/neural/block.py` & `luma-ml-0.8.1/luma/neural/block.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from dataclasses import dataclass
 from typing import Literal, override
 import numpy as np
 
 from luma.core.super import Optimizer
 from luma.interface.typing import TensorLike
 from luma.interface.util import InitUtil
 
@@ -12,14 +13,32 @@
     "ConvBlock1D",
     "ConvBlock2D",
     "ConvBlock3D",
     "DenseBlock",
 )
 
 
+@dataclass
+class ConvBlockArgs:
+    filter_size: int
+    activation: Activation.FuncType
+    optimizer: Optimizer | None = None
+    initializer: InitUtil.InitStr = None
+    padding: Literal["same", "valid"] = "same"
+    stride: int = 1
+    lambda_: float = 0.0
+    do_batch_norm: bool = True
+    momentum: float = 0.9
+    do_pooling: bool = True
+    pool_filter_size: int = 2
+    pool_stride: int = 2
+    pool_mode: Literal["max", "avg"] = "max"
+    random_state: int | None = None
+
+
 class ConvBlock1D(Sequential):
     """
     Convolutional block for 1-dimensional data.
 
     A convolutional block in a neural network typically consists of a
     convolutional layer followed by a nonlinear activation function,
     and a pooling layer to reduce spatial dimensions.
@@ -88,15 +107,15 @@
         lambda_: float = 0.0,
         do_batch_norm: bool = True,
         momentum: float = 0.9,
         do_pooling: bool = True,
         pool_filter_size: int = 2,
         pool_stride: int = 2,
         pool_mode: Literal["max", "avg"] = "max",
-        random_state: int = None,
+        random_state: int | None = None,
     ) -> None:
         super(ConvBlock1D, self).__init__(
             Convolution1D(
                 in_channels,
                 out_channels,
                 filter_size,
                 stride,
@@ -111,15 +130,15 @@
             super(ConvBlock1D, self).__add__(
                 BatchNorm1D(
                     out_channels,
                     momentum,
                 )
             )
         super(ConvBlock1D, self).__add__(
-            activation,
+            activation(),
         )
         if do_pooling:
             super(ConvBlock1D, self).__add__(
                 Pooling1D(
                     pool_filter_size,
                     pool_stride,
                     pool_mode,
@@ -213,15 +232,15 @@
         lambda_: float = 0.0,
         do_batch_norm: bool = True,
         momentum: float = 0.9,
         do_pooling: bool = True,
         pool_filter_size: int = 2,
         pool_stride: int = 2,
         pool_mode: Literal["max", "avg"] = "max",
-        random_state: int = None,
+        random_state: int | None = None,
     ) -> None:
         super(ConvBlock2D, self).__init__(
             Convolution2D(
                 in_channels,
                 out_channels,
                 filter_size,
                 stride,
@@ -236,15 +255,15 @@
             super(ConvBlock2D, self).__add__(
                 BatchNorm2D(
                     out_channels,
                     momentum,
                 )
             )
         super(ConvBlock2D, self).__add__(
-            activation,
+            activation(),
         )
         if do_pooling:
             super(ConvBlock2D, self).__add__(
                 Pooling2D(
                     pool_filter_size,
                     pool_stride,
                     pool_mode,
@@ -338,15 +357,15 @@
         lambda_: float = 0.0,
         do_batch_norm: bool = True,
         momentum: float = 0.9,
         do_pooling: bool = True,
         pool_filter_size: int = 2,
         pool_stride: int = 2,
         pool_mode: Literal["max", "avg"] = "max",
-        random_state: int = None,
+        random_state: int | None = None,
     ) -> None:
         super(ConvBlock3D, self).__init__(
             Convolution3D(
                 in_channels,
                 out_channels,
                 filter_size,
                 stride,
@@ -361,15 +380,15 @@
             super(ConvBlock3D, self).__add__(
                 BatchNorm3D(
                     out_channels,
                     momentum,
                 )
             )
         super(ConvBlock3D, self).__add__(
-            activation,
+            activation(),
         )
         if do_pooling:
             super(ConvBlock3D, self).__add__(
                 Pooling3D(
                     pool_filter_size,
                     pool_stride,
                     pool_mode,
@@ -387,14 +406,27 @@
                 "pool_filter_size": ("0<,+inf", int),
                 "pool_stride": ("0<,+inf", int),
             }
         )
         self.check_param_ranges()
 
 
+@dataclass
+class DenseBlockArgs:
+    activation: Activation.FuncType
+    optimizer: Optimizer | None = None
+    initializer: InitUtil.InitStr = None
+    lambda_: float = 0.0
+    do_batch_norm: float = True
+    momentum: float = 0.9
+    do_dropout: bool = True
+    dropout_rate: float = 0.5
+    random_state: int | None = None
+
+
 class DenseBlock(Sequential):
     """
     A typical dense block in a neural network configuration often
     includes a series of fully connected (dense) layers. Each layer
     within the block connects every input neuron to every output
     neuron through learned weights. Activation functions, such as ReLU,
     are applied after each dense layer to introduce non-linear processing,
@@ -441,15 +473,15 @@
         optimizer: Optimizer = None,
         initializer: InitUtil.InitStr = None,
         lambda_: float = 0.0,
         do_batch_norm: float = True,
         momentum: float = 0.9,
         do_dropout: bool = True,
         dropout_rate: float = 0.5,
-        random_state: int = None,
+        random_state: int | None = None,
     ) -> None:
         super(DenseBlock, self).__init__(
             Dense(
                 in_features,
                 out_features,
                 initializer,
                 optimizer,
@@ -461,15 +493,15 @@
             super(DenseBlock, self).__add__(
                 BatchNorm1D(
                     1,
                     momentum,
                 )
             )
         super(DenseBlock, self).__add__(
-            activation,
+            activation(),
         )
         if do_dropout:
             super(DenseBlock, self).__add__(
                 Dropout(
                     dropout_rate,
                     random_state,
                 ),
```

### Comparing `luma-ml-0.8.0/luma/neural/init.py` & `luma-ml-0.8.1/luma/neural/init.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/neural/layer.py` & `luma-ml-0.8.1/luma/neural/layer.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     "Convolution2D",
     "Convolution3D",
     "Pooling1D",
     "Pooling2D",
     "Pooling3D",
     "Dense",
     "Dropout",
+    "Dropout1D",
+    "Dropout2D",
+    "Dropout3D",
     "Flatten",
     "Activation",
     "BatchNorm1D",
     "BatchNorm2D",
     "BatchNorm3D",
     "LocalResponseNorm",
     "LayerNorm",
@@ -412,17 +415,108 @@
     `dropout_rate` : float, default=0.5
         The fraction of input units to drop during training
     `random_state` : int, optional, default=None
         Seed for various random sampling processes
 
     Notes
     -----
-    - During inference, dropout is typically turned off, and the layer behaves
-      as the identity function.
+    - This class applies dropout for every element in the input with any shape.
+    """
+
+    def __init__(
+        self, dropout_rate: float = 0.5, random_state: int | None = None
+    ) -> None:
+        super().__init__(dropout_rate, random_state)
+
+
+class Dropout1D(_drop._Dropout1D):
+    """
+    Dropout layer for 1-dimensional data.
+
+    Dropout is a regularization technique used during training to prevent
+    overfitting by randomly setting a fraction of input units to zero during
+    the forward pass. This helps in reducing co-adaptation of neurons and
+    encourages the network to learn more robust features.
+
+    Parameters
+    ----------
+    `dropout_rate` : float, default=0.5
+        The fraction of input units to drop during training
+    `random_state` : int, optional, default=None
+        Seed for various random sampling processes
+
+    Notes
+    -----
+    - The input `X` must have the form of 3D-array(`Tensor`).
+
+        ```py
+        X.shape = (batch_size, channels, width)
+        ```
+    """
+
+    def __init__(
+        self, dropout_rate: float = 0.5, random_state: int | None = None
+    ) -> None:
+        super().__init__(dropout_rate, random_state)
+
+
+class Dropout2D(_drop._Dropout2D):
+    """
+    Dropout layer for 2-dimensional data.
+
+    Dropout is a regularization technique used during training to prevent
+    overfitting by randomly setting a fraction of input units to zero during
+    the forward pass. This helps in reducing co-adaptation of neurons and
+    encourages the network to learn more robust features.
 
+    Parameters
+    ----------
+    `dropout_rate` : float, default=0.5
+        The fraction of input units to drop during training
+    `random_state` : int, optional, default=None
+        Seed for various random sampling processes
+
+    Notes
+    -----
+    - The input `X` must have the form of 4D-array(`Tensor`).
+
+        ```py
+        X.shape = (batch_size, channels, height, width)
+        ```
+    """
+
+    def __init__(
+        self, dropout_rate: float = 0.5, random_state: int | None = None
+    ) -> None:
+        super().__init__(dropout_rate, random_state)
+
+
+class Dropout3D(_drop._Dropout3D):
+    """
+    Dropout layer for 3-dimensional data.
+
+    Dropout is a regularization technique used during training to prevent
+    overfitting by randomly setting a fraction of input units to zero during
+    the forward pass. This helps in reducing co-adaptation of neurons and
+    encourages the network to learn more robust features.
+
+    Parameters
+    ----------
+    `dropout_rate` : float, default=0.5
+        The fraction of input units to drop during training
+    `random_state` : int, optional, default=None
+        Seed for various random sampling processes
+
+    Notes
+    -----
+    - The input `X` must have the form of 5D-array(`Tensor`).
+
+        ```py
+        X.shape = (batch_size, channels, depth, height, width)
+        ```
     """
 
     def __init__(
         self, dropout_rate: float = 0.5, random_state: int | None = None
     ) -> None:
         super().__init__(dropout_rate, random_state)
```

### Comparing `luma-ml-0.8.0/luma/neural/loss.py` & `luma-ml-0.8.1/luma/neural/loss.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/neural/network.py` & `luma-ml-0.8.1/luma/neural/network.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     "SimpleMLP",
     "SimpleCNN",
     "LeNet_1",
     "LeNet_4",
     "LeNet_5",
     "AlexNet",
     "ZFNet",
+    "VGGNet_11",
+    "VGGNet_13",
+    "VGGNet_16",
+    "VGGNet_19",
 )
 
 
 class SimpleMLP(_simple._SimpleMLP):
     """
     An MLP (Multilayer Perceptron) is a type of artificial neural network
     composed of at least three layers: an input layer, one or more hidden
@@ -211,32 +215,32 @@
     --------
     ```py
     model = SimpleCNN(
         in_channels_list=[1, 6],
         in_features_list=[96, 16],
         out_channels=12,
         out_features=10,
-        activation=Activation.ReLU(),
+        activation=Activation.ReLU,
         ...,
     )
     ```
     This model has the same structure with:
     ```py
     model = Sequential(
         Convolution(1, 6),  # First convolution block
-        Activation.ReLU(),
+        Activation.ReLU,
         Pooling(),
 
         Convolution(6, 12),  # Second convolution block
-        Activation.ReLU(),
+        Activation.ReLU,
         Pooling(),
 
         Flatten(),
         Dense(96, 16),  # Dense block
-        Activation.ReLU(),
+        Activation.ReLU,
         Dropout(),
 
         Dense(16, 10),  # Final dense layer
     )
     ```
     """
 
@@ -338,15 +342,15 @@
     ```
     Parameter Size:
     ```txt
     2,180 weights, 22 biases -> 2,202 params
     ```
     Parameters
     ----------
-    `activation` : FuncType, default=Activation.Tanh()
+    `activation` : FuncType, default=Activation.Tanh
         Type of activation function
     `optimizer` : Optimizer
         Type of optimizer for weight update
     `loss` : Loss, default=CrossEntropy()
         Type of loss function
     `initializer` : InitStr, default=None
         Type of weight initializer
@@ -375,15 +379,15 @@
     Code Recognition." Neural Computation, vol. 1, no. 4, 1989, pp. 541-551.
 
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
-        activation: Activation.FuncType = Activation.Tanh(),
+        activation: Activation.FuncType = Activation.Tanh,
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
@@ -440,15 +444,15 @@
     ```
     Parameter Size:
     ```txt
     50,902 weights, 150 biases -> 51,052 params
     ```
     Parameters
     ----------
-    `activation` : FuncType, default=Activation.Tanh()
+    `activation` : FuncType, default=Activation.Tanh
         Type of activation function
     `optimizer` : Optimizer
         Type of optimizer for weight update
     `loss` : Loss, default=CrossEntropy()
         Type of loss function
     `initializer` : InitStr, default=None
         Type of weight initializer
@@ -476,15 +480,15 @@
     1. LeCun, Yann, et al. "Backpropagation Applied to Handwritten Zip
     Code Recognition." Neural Computation, vol. 1, no. 4, 1989, pp. 541-551.
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
-        activation: Activation.FuncType = Activation.Tanh(),
+        activation: Activation.FuncType = Activation.Tanh,
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
@@ -544,15 +548,15 @@
     ```
     Parameter Size:
     ```txt
     61,474 weights, 236 biases -> 61,710 params
     ```
     Parameters
     ----------
-    `activation` : FuncType, default=Activation.Tanh()
+    `activation` : FuncType, default=Activation.Tanh
         Type of activation function
     `optimizer` : Optimizer
         Type of optimizer for weight update
     `loss` : Loss, default=CrossEntropy()
         Type of loss function
     `initializer` : InitStr, default=None
         Type of weight initializer
@@ -580,15 +584,15 @@
     1. LeCun, Yann, et al. "Backpropagation Applied to Handwritten Zip
     Code Recognition." Neural Computation, vol. 1, no. 4, 1989, pp. 541-551.
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
-        activation: Activation.FuncType = Activation.Tanh(),
+        activation: Activation.FuncType = Activation.Tanh,
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
@@ -656,15 +660,15 @@
     ```
     Parameter Size:
     ```txt
     62,367,776 weights, 10,568 biases -> 62,378,344 params
     ```
     Parameters
     ----------
-    `activation` : FuncType, default=Activation.ReLU()
+    `activation` : FuncType, default=Activation.ReLU
         Type of activation function
     `optimizer` : Optimizer
         Type of optimizer for weight update
     `loss` : Loss, default=CrossEntropy()
         Type of loss function
     `initializer` : InitStr, default=None
         Type of weight initializer
@@ -694,15 +698,15 @@
     Information Processing Systems, 2012.
 
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
-        activation: Activation.FuncType = Activation.ReLU(),
+        activation: Activation.FuncType = Activation.ReLU,
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
@@ -771,15 +775,15 @@
     ```
     Parameter Size:
     ```txt
     58,292,000 weights, 9,578 biases -> 58,301,578 params
     ```
     Parameters
     ----------
-    `activation` : FuncType, default=Activation.ReLU()
+    `activation` : FuncType, default=Activation.ReLU
         Type of activation function
     `optimizer` : Optimizer
         Type of optimizer for weight update
     `loss` : Loss, default=CrossEntropy()
         Type of loss function
     `initializer` : InitStr, default=None
         Type of weight initializer
@@ -808,15 +812,497 @@
     Convolutional Networks." European conference on computer vision, 2014.
 
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
-        activation: Activation.FuncType = Activation.ReLU(),
+        activation: Activation.FuncType = Activation.ReLU,
+        loss: Loss = CrossEntropy(),
+        initializer: InitUtil.InitStr = None,
+        out_features: int = 1000,
+        batch_size: int = 100,
+        n_epochs: int = 100,
+        learning_rate: float = 0.01,
+        valid_size: float = 0.1,
+        lambda_: float = 0,
+        dropout_rate: float = 0.5,
+        early_stopping: bool = False,
+        patience: int = 10,
+        shuffle: bool = True,
+        random_state: int | None = None,
+        deep_verbose: bool = False,
+    ) -> None:
+        super().__init__(
+            optimizer,
+            activation,
+            loss,
+            initializer,
+            out_features,
+            batch_size,
+            n_epochs,
+            learning_rate,
+            valid_size,
+            lambda_,
+            dropout_rate,
+            early_stopping,
+            patience,
+            shuffle,
+            random_state,
+            deep_verbose,
+        )
+
+
+class VGGNet_11(_imagenet._VGGNet_11):
+    """
+    VGG11 is a simplified variant of the VGG network architecture that was designed
+    to enhance image recognition performance through deeper networks with smaller
+    convolutional filters. This model was introduced by Karen Simonyan and Andrew
+    Zisserman in their paper and is notable for its simplicity and effectiveness
+    in image classification tasks.
+
+    Structure
+    ---------
+    Input:
+    ```py
+    Tensor[..., 3, 224, 224]
+    ```
+    Convolutional Blocks:
+    ```py
+    ConvBlock2D(3, 64) -> Pooling2D(2, 2, "max") ->  # Conv_1
+    ConvBlock2D(64, 128) -> Pooling2D(2, 2, "max") ->  # Conv_2
+
+    ConvBlock2D(128, 256, do_pooling=False) ->  # Conv_3
+    ConvBlock2D(256, 256) -> Pooling2D(2, 2, "max") ->  # Conv_4
+
+    ConvBlock2D(256, 512, do_pooling=False) ->  # Conv_5
+    ConvBlock2D(512, 512) -> Pooling2D(2, 2, "max") ->  # Conv_6
+
+    ConvBlock2D(512, 512, do_pooling=False) ->  # Conv_7
+    ConvBlock2D(512, 512) -> Pooling2D(2, 2, "max") ->  # Conv_8
+    ```
+    Fully Connected Layers:
+    ```py
+    Flatten ->
+    DenseBlock(512 * 7 * 7, 4096) -> DenseBlock(4096, 4096) ->
+    Dense(4096, 1000)
+    ```
+    Output:
+    ```py
+    Matrix[..., 1000]
+    ```
+    Parameter Size:
+    ```txt
+    132,851,392 weights, 11,944 biases -> 132,863,336 params
+    ```
+    Parameters
+    ----------
+    `activation` : FuncType, default=Activation.ReLU
+        Type of activation function
+    `optimizer` : Optimizer
+        Type of optimizer for weight update
+    `loss` : Loss, default=CrossEntropy()
+        Type of loss function
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `out_features` : int, default=1000
+        Number of output features
+    `batch_size` : int, default=100
+        Size of a single mini-batch
+    `n_epochs` : int, default=100
+        Number of epochs for training
+    `learning_rate` : float, default=0.01
+        Step size during optimization process
+    `valid_size` : float, default=0.1
+        Fractional size of validation set
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `early_stopping` : bool, default=False
+        Whether to early-stop the training when the valid score stagnates
+    `patience` : int, default=10
+        Number of epochs to wait until early-stopping
+    `shuffle` : bool, default=True
+        Whethter to shuffle the data at the beginning of every epoch
+
+    References
+    ----------
+    1. Simonyan, Karen, and Andrew Zisserman. "Very Deep Convolutional Networks for
+    Large-Scale Image Recognition." arXiv preprint arXiv:1409.1556, 2014.
+    """
+
+    def __init__(
+        self,
+        optimizer: Optimizer,
+        activation: Activation.FuncType = Activation.ReLU,
+        loss: Loss = CrossEntropy(),
+        initializer: InitUtil.InitStr = None,
+        out_features: int = 1000,
+        batch_size: int = 100,
+        n_epochs: int = 100,
+        learning_rate: float = 0.01,
+        valid_size: float = 0.1,
+        lambda_: float = 0,
+        dropout_rate: float = 0.5,
+        early_stopping: bool = False,
+        patience: int = 10,
+        shuffle: bool = True,
+        random_state: int | None = None,
+        deep_verbose: bool = False,
+    ) -> None:
+        super().__init__(
+            optimizer,
+            activation,
+            loss,
+            initializer,
+            out_features,
+            batch_size,
+            n_epochs,
+            learning_rate,
+            valid_size,
+            lambda_,
+            dropout_rate,
+            early_stopping,
+            patience,
+            shuffle,
+            random_state,
+            deep_verbose,
+        )
+
+
+class VGGNet_13(_imagenet._VGGNet_13):
+    """
+    VGG13 is ont of the variants of the VGG network architecture that was designed
+    to enhance image recognition performance through deeper networks with smaller
+    convolutional filters. This model was introduced by Karen Simonyan and Andrew
+    Zisserman in their paper and is notable for its simplicity and effectiveness
+    in image classification tasks.
+
+    Structure
+    ---------
+    Input:
+    ```py
+    Tensor[..., 3, 224, 224]
+    ```
+    Convolutional Blocks:
+    ```py
+    ConvBlock2D(3, 64, do_pooling=False) ->  # Conv_1
+    ConvBlock2D(64, 64) -> Pooling2D(2, 2, "max") ->  # Conv_2
+
+    ConvBlock2D(64, 128, do_pooling=False) ->  # Conv_3
+    ConvBlock2D(128, 128) -> Pooling2D(2, 2, "max") ->  # Conv_4
+
+    ConvBlock2D(128, 256, do_pooling=False) ->  # Conv_5
+    ConvBlock2D(256, 256) -> Pooling2D(2, 2, "max") ->  # Conv_6
+
+    ConvBlock2D(256, 512, do_pooling=False) ->  # Conv_7
+    ConvBlock2D(512, 512) -> Pooling2D(2, 2, "max") ->  # Conv_8
+
+    ConvBlock2D(512, 512, do_pooling=False) ->  # Conv_9
+    ConvBlock2D(512, 512) -> Pooling2D(2, 2, "max") ->  # Conv_10
+    ```
+    Fully Connected Layers:
+    ```py
+    Flatten ->
+    DenseBlock(512 * 7 * 7, 4096) -> DenseBlock(4096, 4096) ->
+    Dense(4096, 1000)
+    ```
+    Output:
+    ```py
+    Matrix[..., 1000]
+    ```
+    Parameter Size:
+    ```txt
+    133,035,712 weights, 12,136 biases -> 133,047,848 params
+    ```
+    Parameters
+    ----------
+    `activation` : FuncType, default=Activation.ReLU
+        Type of activation function
+    `optimizer` : Optimizer
+        Type of optimizer for weight update
+    `loss` : Loss, default=CrossEntropy()
+        Type of loss function
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `out_features` : int, default=1000
+        Number of output features
+    `batch_size` : int, default=100
+        Size of a single mini-batch
+    `n_epochs` : int, default=100
+        Number of epochs for training
+    `learning_rate` : float, default=0.01
+        Step size during optimization process
+    `valid_size` : float, default=0.1
+        Fractional size of validation set
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `early_stopping` : bool, default=False
+        Whether to early-stop the training when the valid score stagnates
+    `patience` : int, default=10
+        Number of epochs to wait until early-stopping
+    `shuffle` : bool, default=True
+        Whethter to shuffle the data at the beginning of every epoch
+
+    References
+    ----------
+    1. Simonyan, Karen, and Andrew Zisserman. "Very Deep Convolutional Networks for
+    Large-Scale Image Recognition." arXiv preprint arXiv:1409.1556, 2014.
+    """
+
+    def __init__(
+        self,
+        optimizer: Optimizer,
+        activation: Activation.FuncType = Activation.ReLU,
+        loss: Loss = CrossEntropy(),
+        initializer: InitUtil.InitStr = None,
+        out_features: int = 1000,
+        batch_size: int = 100,
+        n_epochs: int = 100,
+        learning_rate: float = 0.01,
+        valid_size: float = 0.1,
+        lambda_: float = 0,
+        dropout_rate: float = 0.5,
+        early_stopping: bool = False,
+        patience: int = 10,
+        shuffle: bool = True,
+        random_state: int | None = None,
+        deep_verbose: bool = False,
+    ) -> None:
+        super().__init__(
+            optimizer,
+            activation,
+            loss,
+            initializer,
+            out_features,
+            batch_size,
+            n_epochs,
+            learning_rate,
+            valid_size,
+            lambda_,
+            dropout_rate,
+            early_stopping,
+            patience,
+            shuffle,
+            random_state,
+            deep_verbose,
+        )
+
+
+class VGGNet_16(_imagenet._VGGNet_16):
+    """
+    VGG16 is ont of the variants of the VGG network architecture that was designed
+    to enhance image recognition performance through deeper networks with smaller
+    convolutional filters. This model was introduced by Karen Simonyan and Andrew
+    Zisserman in their paper and is notable for its simplicity and effectiveness
+    in image classification tasks.
+
+    Structure
+    ---------
+    Input:
+    ```py
+    Tensor[..., 3, 224, 224]
+    ```
+    Convolutional Blocks:
+    ```py
+    ConvBlock2D(3, 64, do_pooling=False) ->  # Conv_1
+    ConvBlock2D(64, 64) -> Pooling2D(2, 2, "max") ->  # Conv_2
+
+    ConvBlock2D(64, 128, do_pooling=False) ->  # Conv_3
+    ConvBlock2D(128, 128) -> Pooling2D(2, 2, "max") ->  # Conv_4
+
+    ConvBlock2D(128, 256, do_pooling=False) ->  # Conv_5
+    ConvBlock2D(256, 256, do_pooling=False) ->  # Conv_6
+    ConvBlock2D(256, 256) -> Pooling2D(2, 2, "max") ->  # Conv_7
+
+    ConvBlock2D(256, 512, do_pooling=False) ->  # Conv_8
+    ConvBlock2D(512, 512, do_pooling=False) ->  # Conv_9
+    ConvBlock2D(512, 512) -> Pooling2D(2, 2, "max") ->  # Conv_10
+
+    ConvBlock2D(512, 512, do_pooling=False) ->  # Conv_11
+    ConvBlock2D(512, 512, do_pooling=False) ->  # Conv_12
+    ConvBlock2D(512, 512) -> Pooling2D(2, 2, "max") ->  # Conv_13
+    ```
+    Fully Connected Layers:
+    ```py
+    Flatten ->
+    DenseBlock(512 * 7 * 7, 4096) -> DenseBlock(4096, 4096) ->
+    Dense(4096, 1000)
+    ```
+    Output:
+    ```py
+    Matrix[..., 1000]
+    ```
+    Parameter Size:
+    ```txt
+    138,344,128 weights, 13,416 biases -> 138,357,544 params
+    ```
+    Parameters
+    ----------
+    `activation` : FuncType, default=Activation.ReLU
+        Type of activation function
+    `optimizer` : Optimizer
+        Type of optimizer for weight update
+    `loss` : Loss, default=CrossEntropy()
+        Type of loss function
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `out_features` : int, default=1000
+        Number of output features
+    `batch_size` : int, default=100
+        Size of a single mini-batch
+    `n_epochs` : int, default=100
+        Number of epochs for training
+    `learning_rate` : float, default=0.01
+        Step size during optimization process
+    `valid_size` : float, default=0.1
+        Fractional size of validation set
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `early_stopping` : bool, default=False
+        Whether to early-stop the training when the valid score stagnates
+    `patience` : int, default=10
+        Number of epochs to wait until early-stopping
+    `shuffle` : bool, default=True
+        Whethter to shuffle the data at the beginning of every epoch
+
+    References
+    ----------
+    1. Simonyan, Karen, and Andrew Zisserman. "Very Deep Convolutional Networks for
+    Large-Scale Image Recognition." arXiv preprint arXiv:1409.1556, 2014.
+    """
+
+    def __init__(
+        self,
+        optimizer: Optimizer,
+        activation: Activation.FuncType = Activation.ReLU,
+        loss: Loss = CrossEntropy(),
+        initializer: InitUtil.InitStr = None,
+        out_features: int = 1000,
+        batch_size: int = 100,
+        n_epochs: int = 100,
+        learning_rate: float = 0.01,
+        valid_size: float = 0.1,
+        lambda_: float = 0,
+        dropout_rate: float = 0.5,
+        early_stopping: bool = False,
+        patience: int = 10,
+        shuffle: bool = True,
+        random_state: int | None = None,
+        deep_verbose: bool = False,
+    ) -> None:
+        super().__init__(
+            optimizer,
+            activation,
+            loss,
+            initializer,
+            out_features,
+            batch_size,
+            n_epochs,
+            learning_rate,
+            valid_size,
+            lambda_,
+            dropout_rate,
+            early_stopping,
+            patience,
+            shuffle,
+            random_state,
+            deep_verbose,
+        )
+
+
+class VGGNet_19(_imagenet._VGGNet_19):
+    """
+    VGG19 is ont of the variants of the VGG network architecture that was designed
+    to enhance image recognition performance through deeper networks with smaller
+    convolutional filters. This model was introduced by Karen Simonyan and Andrew
+    Zisserman in their paper and is notable for its simplicity and effectiveness
+    in image classification tasks.
+
+    Structure
+    ---------
+    Input:
+    ```py
+    Tensor[..., 3, 224, 224]
+    ```
+    Convolutional Blocks:
+    ```py
+    ConvBlock2D(3, 64, do_pooling=False) ->  # Conv_1
+    ConvBlock2D(64, 64) -> Pooling2D(2, 2, "max") ->  # Conv_2
+
+    ConvBlock2D(64, 128, do_pooling=False) ->  # Conv_3
+    ConvBlock2D(128, 128) -> Pooling2D(2, 2, "max") ->  # Conv_4
+
+    ConvBlock2D(128, 256, do_pooling=False) ->  # Conv_5
+    ConvBlock2D(256, 256, do_pooling=False) ->  # Conv_6
+    ConvBlock2D(256, 256, do_pooling=False) ->  # Conv_7
+    ConvBlock2D(256, 256) -> Pooling2D(2, 2, "max") ->  # Conv_8
+
+    ConvBlock2D(256, 512, do_pooling=False) ->  # Conv_9
+    ConvBlock2D(512, 512, do_pooling=False) ->  # Conv_10
+    ConvBlock2D(512, 512, do_pooling=False) ->  # Conv_11
+    ConvBlock2D(512, 512) -> Pooling2D(2, 2, "max") ->  # Conv_12
+
+    ConvBlock2D(512, 512, do_pooling=False) ->  # Conv_13
+    ConvBlock2D(512, 512, do_pooling=False) ->  # Conv_14
+    ConvBlock2D(512, 512, do_pooling=False) ->  # Conv_15
+    ConvBlock2D(512, 512) -> Pooling2D(2, 2, "max") ->  # Conv_16
+    ```
+    Fully Connected Layers:
+    ```py
+    Flatten ->
+    DenseBlock(512 * 7 * 7, 4096) -> DenseBlock(4096, 4096) ->
+    Dense(4096, 1000)
+    ```
+    Output:
+    ```py
+    Matrix[..., 1000]
+    ```
+    Parameter Size:
+    ```txt
+    143,652,544 weights, 14,696 biases -> 143,667,240 params
+    ```
+    Parameters
+    ----------
+    `activation` : FuncType, default=Activation.ReLU
+        Type of activation function
+    `optimizer` : Optimizer
+        Type of optimizer for weight update
+    `loss` : Loss, default=CrossEntropy()
+        Type of loss function
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `out_features` : int, default=1000
+        Number of output features
+    `batch_size` : int, default=100
+        Size of a single mini-batch
+    `n_epochs` : int, default=100
+        Number of epochs for training
+    `learning_rate` : float, default=0.01
+        Step size during optimization process
+    `valid_size` : float, default=0.1
+        Fractional size of validation set
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `early_stopping` : bool, default=False
+        Whether to early-stop the training when the valid score stagnates
+    `patience` : int, default=10
+        Number of epochs to wait until early-stopping
+    `shuffle` : bool, default=True
+        Whethter to shuffle the data at the beginning of every epoch
+
+    References
+    ----------
+    1. Simonyan, Karen, and Andrew Zisserman. "Very Deep Convolutional Networks for
+    Large-Scale Image Recognition." arXiv preprint arXiv:1409.1556, 2014.
+    """
+
+    def __init__(
+        self,
+        optimizer: Optimizer,
+        activation: Activation.FuncType = Activation.ReLU,
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
```

### Comparing `luma-ml-0.8.0/luma/neural/optimizer.py` & `luma-ml-0.8.1/luma/neural/optimizer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/neural/single.py` & `luma-ml-0.8.1/luma/neural/single.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/pipe/pipeline.py` & `luma-ml-0.8.1/luma/pipe/pipeline.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/preprocessing/encoder.py` & `luma-ml-0.8.1/luma/preprocessing/encoder.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/preprocessing/imputer.py` & `luma-ml-0.8.1/luma/preprocessing/imputer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/preprocessing/outlier.py` & `luma-ml-0.8.1/luma/preprocessing/outlier.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/preprocessing/scaler.py` & `luma-ml-0.8.1/luma/preprocessing/scaler.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/reduction/linear.py` & `luma-ml-0.8.1/luma/reduction/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/reduction/manifold.py` & `luma-ml-0.8.1/luma/reduction/manifold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/reduction/selection.py` & `luma-ml-0.8.1/luma/reduction/selection.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/regressor/general.py` & `luma-ml-0.8.1/luma/regressor/general.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/regressor/linear.py` & `luma-ml-0.8.1/luma/regressor/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/regressor/neighbors.py` & `luma-ml-0.8.1/luma/regressor/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/regressor/poly.py` & `luma-ml-0.8.1/luma/regressor/poly.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/regressor/robust.py` & `luma-ml-0.8.1/luma/regressor/robust.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/regressor/svm.py` & `luma-ml-0.8.1/luma/regressor/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/regressor/tree.py` & `luma-ml-0.8.1/luma/regressor/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/visual/eda.py` & `luma-ml-0.8.1/luma/visual/eda.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma/visual/evaluation.py` & `luma-ml-0.8.1/luma/visual/evaluation.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/luma_ml.egg-info/PKG-INFO` & `luma-ml-0.8.1/luma_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.8.0
+Version: 0.8.1
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.56k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.71k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.8.0</td>
+                    <td>0.8.1</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~22K</td>
+                    <td>~23.8K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.8.0 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.8.1 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.56k-red][GitHub code size in bytes][Code Style]
+5.71k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.8.0
-Lines of Code  ~22K
+Latest Version 0.8.1
+Lines of Code  ~23.8K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.8.0/luma_ml.egg-info/SOURCES.txt` & `luma-ml-0.8.1/luma_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.0/setup.py` & `luma-ml-0.8.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="luma-ml",
-    version="0.8.0",
+    version="0.8.1",
     author="ChanLumerico",
     author_email="greensox284@gmail.com",
     description="A Comprehensive Python Module for Machine Learning and Data Science",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ChanLumerico/luma",
     packages=setuptools.find_namespace_packages(),
```

### Comparing `luma-ml-0.8.0/test/__act.py` & `luma-ml-0.8.1/test/__act.py`

 * *Files identical despite different names*

