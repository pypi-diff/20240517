# Comparing `tmp/MRCpy-2.2.0.tar.gz` & `tmp/MRCpy-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MRCpy-2.2.0.tar", last modified: Mon Apr  8 09:54:31 2024, max compression
+gzip compressed data, was "MRCpy-2.3.0.tar", last modified: Fri May 17 13:36:32 2024, max compression
```

## Comparing `MRCpy-2.2.0.tar` & `MRCpy-2.3.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-08 09:54:31.810796 MRCpy-2.2.0/
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-08 09:54:31.496069 MRCpy-2.2.0/MRCpy/
--rw-r--r--   0 kbondugula   (503) staff       (20)      245 2024-04-03 16:53:57.000000 MRCpy-2.2.0/MRCpy/__init__.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    27156 2024-04-03 16:52:42.000000 MRCpy-2.2.0/MRCpy/amrc.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    17242 2024-02-13 15:23:47.000000 MRCpy-2.2.0/MRCpy/base_mrc.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    28710 2024-02-28 16:31:33.000000 MRCpy-2.2.0/MRCpy/cmrc.py
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-08 09:54:31.500474 MRCpy-2.2.0/MRCpy/datasets/
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     1089 2024-01-28 20:51:11.000000 MRCpy-2.2.0/MRCpy/datasets/__init__.py
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-08 09:54:31.787275 MRCpy-2.2.0/MRCpy/datasets/data/
--rw-r--r--   0 kbondugula   (503) staff       (20)  7075696 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-sci_Test.csv
--rw-r--r--   0 kbondugula   (503) staff       (20) 10629747 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-sci_Train.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  2002192 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-sci_shortTest.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  2002231 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-sci_shortTrain.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  6519380 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-talk_Test.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  9787043 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-talk_Train.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    32719 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/credit.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    23118 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/diabetes.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    16851 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/ecoli.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    11293 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/glass.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     3121 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/haberman.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    21189 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/indianLiverPatient.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     4789 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/iris.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)   732608 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/letter-recognition.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    13796 2023-04-27 10:30:22.000000 MRCpy-2.2.0/MRCpy/datasets/data/mammographic.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)   834087 2023-04-27 10:30:25.000000 MRCpy-2.2.0/MRCpy/datasets/data/optdigits.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  6344664 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/rec-vs-sci_Test.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  9534428 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/rec-vs-sci_Train.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  5788382 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/rec-vs-talk_Test.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  8691659 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/rec-vs-talk_Train.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    85710 2023-04-27 10:30:25.000000 MRCpy-2.2.0/MRCpy/datasets/data/redwine.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  5766341 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/sci-vs-talk_Test.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)  8659812 2024-01-16 12:39:02.000000 MRCpy-2.2.0/MRCpy/datasets/data/sci-vs-talk_Train.csv
--rwxr-xr-x   0 kbondugula   (503) staff       (20)   370691 2023-04-27 10:30:25.000000 MRCpy-2.2.0/MRCpy/datasets/data/segment.csv
--rw-r--r--   0 kbondugula   (503) staff       (20)   300394 2023-04-27 10:30:25.000000 MRCpy-2.2.0/MRCpy/datasets/data/usenet2.csv
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-08 09:54:31.801458 MRCpy-2.2.0/MRCpy/datasets/descr/
--rw-r--r--   0 kbondugula   (503) staff       (20)     2106 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/adult.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)     1048 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/catsvsdogs_features_resnet18.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     2218 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/credit.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     1102 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/diabetes.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     3022 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/ecoli.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     3666 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/glass.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     1535 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/haberman.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     2582 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/indianLiverPatient.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     2998 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/iris.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     2734 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/letter-recognition.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     3479 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/mammographic.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)      815 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/mnist_features_resnet18.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     2388 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/optdigits.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)     3305 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/redwine.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)     5250 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/satellite.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)     2432 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/segment.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)       89 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/usenet2.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)        0 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/vehicle.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)     1316 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/yearbook.rst
--rw-r--r--   0 kbondugula   (503) staff       (20)     1143 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/datasets/descr/yearbook_features_resnet18.rst
--rwxr-xr-x   0 kbondugula   (503) staff       (20)    52570 2024-02-09 13:02:57.000000 MRCpy-2.2.0/MRCpy/datasets/load.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    22506 2024-04-02 14:12:29.000000 MRCpy-2.2.0/MRCpy/dwgcs.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    28630 2024-02-13 15:34:58.000000 MRCpy-2.2.0/MRCpy/mrc.py
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-08 09:54:31.805497 MRCpy-2.2.0/MRCpy/phi/
--rw-r--r--   0 kbondugula   (503) staff       (20)      320 2024-02-09 17:31:55.000000 MRCpy-2.2.0/MRCpy/phi/__init__.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    10306 2024-01-30 14:36:53.000000 MRCpy-2.2.0/MRCpy/phi/base_phi.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     9282 2024-01-05 12:47:57.000000 MRCpy-2.2.0/MRCpy/phi/random_fourier_phi.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     9145 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/phi/random_relu_phi.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     6784 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/phi/threshold_phi.py
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-08 09:54:31.810465 MRCpy-2.2.0/MRCpy/solvers/
--rw-r--r--   0 kbondugula   (503) staff       (20)       82 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/solvers/__init__.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     1820 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/solvers/adam.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     9604 2024-02-12 18:48:43.000000 MRCpy-2.2.0/MRCpy/solvers/cg.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     2259 2024-02-12 18:46:27.000000 MRCpy-2.2.0/MRCpy/solvers/cvx.py
--rw-r--r--   0 kbondugula   (503) staff       (20)    12950 2024-01-25 13:26:36.000000 MRCpy-2.2.0/MRCpy/solvers/nesterov.py
--rw-r--r--   0 kbondugula   (503) staff       (20)     2833 2023-04-27 10:30:27.000000 MRCpy-2.2.0/MRCpy/solvers/sgd.py
-drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-04-08 09:54:31.499222 MRCpy-2.2.0/MRCpy.egg-info/
--rw-r--r--   0 kbondugula   (503) staff       (20)     4980 2024-04-08 09:54:31.000000 MRCpy-2.2.0/MRCpy.egg-info/PKG-INFO
--rw-r--r--   0 kbondugula   (503) staff       (20)     2312 2024-04-08 09:54:31.000000 MRCpy-2.2.0/MRCpy.egg-info/SOURCES.txt
--rw-r--r--   0 kbondugula   (503) staff       (20)        1 2024-04-08 09:54:31.000000 MRCpy-2.2.0/MRCpy.egg-info/dependency_links.txt
--rw-r--r--   0 kbondugula   (503) staff       (20)        1 2024-04-08 09:54:31.000000 MRCpy-2.2.0/MRCpy.egg-info/not-zip-safe
--rw-r--r--   0 kbondugula   (503) staff       (20)       64 2024-04-08 09:54:31.000000 MRCpy-2.2.0/MRCpy.egg-info/requires.txt
--rw-r--r--   0 kbondugula   (503) staff       (20)        6 2024-04-08 09:54:31.000000 MRCpy-2.2.0/MRCpy.egg-info/top_level.txt
--rw-r--r--   0 kbondugula   (503) staff       (20)     4980 2024-04-08 09:54:31.810941 MRCpy-2.2.0/PKG-INFO
--rw-r--r--   0 kbondugula   (503) staff       (20)     4316 2024-02-14 10:00:13.000000 MRCpy-2.2.0/README.md
--rw-r--r--   0 kbondugula   (503) staff       (20)      778 2024-04-03 16:53:29.000000 MRCpy-2.2.0/pyproject.toml
--rw-r--r--   0 kbondugula   (503) staff       (20)      160 2024-04-08 09:54:31.811552 MRCpy-2.2.0/setup.cfg
--rw-r--r--   0 kbondugula   (503) staff       (20)     2357 2024-02-14 09:37:45.000000 MRCpy-2.2.0/setup.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-05-17 13:36:32.454054 MRCpy-2.3.0/
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-05-17 13:36:31.919381 MRCpy-2.3.0/MRCpy/
+-rw-r--r--   0 kbondugula   (503) staff       (20)      245 2024-05-17 13:29:43.000000 MRCpy-2.3.0/MRCpy/__init__.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    27156 2024-04-03 16:52:42.000000 MRCpy-2.3.0/MRCpy/amrc.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    17242 2024-02-13 15:23:47.000000 MRCpy-2.3.0/MRCpy/base_mrc.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    28733 2024-05-17 13:28:12.000000 MRCpy-2.3.0/MRCpy/cmrc.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-05-17 13:36:31.925273 MRCpy-2.3.0/MRCpy/datasets/
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     1089 2024-01-28 20:51:11.000000 MRCpy-2.3.0/MRCpy/datasets/__init__.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-05-17 13:36:32.425891 MRCpy-2.3.0/MRCpy/datasets/data/
+-rw-r--r--   0 kbondugula   (503) staff       (20)  7075696 2024-01-16 12:39:02.000000 MRCpy-2.3.0/MRCpy/datasets/data/comp-vs-sci_Test.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20) 10629747 2024-01-16 12:39:02.000000 MRCpy-2.3.0/MRCpy/datasets/data/comp-vs-sci_Train.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  2002192 2024-01-16 12:39:02.000000 MRCpy-2.3.0/MRCpy/datasets/data/comp-vs-sci_shortTest.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  2002231 2024-01-16 12:39:02.000000 MRCpy-2.3.0/MRCpy/datasets/data/comp-vs-sci_shortTrain.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  6519380 2024-01-16 12:39:02.000000 MRCpy-2.3.0/MRCpy/datasets/data/comp-vs-talk_Test.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  9787043 2024-01-16 12:39:02.000000 MRCpy-2.3.0/MRCpy/datasets/data/comp-vs-talk_Train.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    32719 2023-04-27 10:30:22.000000 MRCpy-2.3.0/MRCpy/datasets/data/credit.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    23118 2023-04-27 10:30:22.000000 MRCpy-2.3.0/MRCpy/datasets/data/diabetes.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    16851 2023-04-27 10:30:22.000000 MRCpy-2.3.0/MRCpy/datasets/data/ecoli.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    11293 2023-04-27 10:30:22.000000 MRCpy-2.3.0/MRCpy/datasets/data/glass.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     3121 2023-04-27 10:30:22.000000 MRCpy-2.3.0/MRCpy/datasets/data/haberman.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    21189 2023-04-27 10:30:22.000000 MRCpy-2.3.0/MRCpy/datasets/data/indianLiverPatient.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     4789 2023-04-27 10:30:22.000000 MRCpy-2.3.0/MRCpy/datasets/data/iris.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)   732608 2023-04-27 10:30:22.000000 MRCpy-2.3.0/MRCpy/datasets/data/letter-recognition.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    13796 2023-04-27 10:30:22.000000 MRCpy-2.3.0/MRCpy/datasets/data/mammographic.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)   834087 2023-04-27 10:30:25.000000 MRCpy-2.3.0/MRCpy/datasets/data/optdigits.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  6344664 2024-01-16 12:39:02.000000 MRCpy-2.3.0/MRCpy/datasets/data/rec-vs-sci_Test.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  9534428 2024-01-16 12:39:02.000000 MRCpy-2.3.0/MRCpy/datasets/data/rec-vs-sci_Train.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  5788382 2024-01-16 12:39:02.000000 MRCpy-2.3.0/MRCpy/datasets/data/rec-vs-talk_Test.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  8691659 2024-01-16 12:39:02.000000 MRCpy-2.3.0/MRCpy/datasets/data/rec-vs-talk_Train.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    85710 2023-04-27 10:30:25.000000 MRCpy-2.3.0/MRCpy/datasets/data/redwine.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  5766341 2024-01-16 12:39:02.000000 MRCpy-2.3.0/MRCpy/datasets/data/sci-vs-talk_Test.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)  8659812 2024-01-16 12:39:02.000000 MRCpy-2.3.0/MRCpy/datasets/data/sci-vs-talk_Train.csv
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)   370691 2023-04-27 10:30:25.000000 MRCpy-2.3.0/MRCpy/datasets/data/segment.csv
+-rw-r--r--   0 kbondugula   (503) staff       (20)   300394 2023-04-27 10:30:25.000000 MRCpy-2.3.0/MRCpy/datasets/data/usenet2.csv
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-05-17 13:36:32.444859 MRCpy-2.3.0/MRCpy/datasets/descr/
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2106 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/adult.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)     1048 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/catsvsdogs_features_resnet18.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     2218 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/credit.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     1102 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/diabetes.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     3022 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/ecoli.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     3666 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/glass.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     1535 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/haberman.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     2582 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/indianLiverPatient.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     2998 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/iris.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     2734 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/letter-recognition.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     3479 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/mammographic.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)      815 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/mnist_features_resnet18.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     2388 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/optdigits.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)     3305 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/redwine.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)     5250 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/satellite.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2432 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/segment.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)       89 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/usenet2.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)        0 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/vehicle.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)     1316 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/yearbook.rst
+-rw-r--r--   0 kbondugula   (503) staff       (20)     1143 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/datasets/descr/yearbook_features_resnet18.rst
+-rwxr-xr-x   0 kbondugula   (503) staff       (20)    52570 2024-02-09 13:02:57.000000 MRCpy-2.3.0/MRCpy/datasets/load.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    23199 2024-05-17 13:27:44.000000 MRCpy-2.3.0/MRCpy/dwgcs.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    28630 2024-02-13 15:34:58.000000 MRCpy-2.3.0/MRCpy/mrc.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-05-17 13:36:32.448946 MRCpy-2.3.0/MRCpy/phi/
+-rw-r--r--   0 kbondugula   (503) staff       (20)      320 2024-02-09 17:31:55.000000 MRCpy-2.3.0/MRCpy/phi/__init__.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    10324 2024-05-13 12:53:43.000000 MRCpy-2.3.0/MRCpy/phi/base_phi.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     9282 2024-01-05 12:47:57.000000 MRCpy-2.3.0/MRCpy/phi/random_fourier_phi.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     9145 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/phi/random_relu_phi.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     6784 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/phi/threshold_phi.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-05-17 13:36:32.453674 MRCpy-2.3.0/MRCpy/solvers/
+-rw-r--r--   0 kbondugula   (503) staff       (20)       82 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/solvers/__init__.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     1820 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/solvers/adam.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     9604 2024-02-12 18:48:43.000000 MRCpy-2.3.0/MRCpy/solvers/cg.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2271 2024-05-17 13:20:48.000000 MRCpy-2.3.0/MRCpy/solvers/cvx.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)    12950 2024-01-25 13:26:36.000000 MRCpy-2.3.0/MRCpy/solvers/nesterov.py
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2833 2023-04-27 10:30:27.000000 MRCpy-2.3.0/MRCpy/solvers/sgd.py
+drwxr-xr-x   0 kbondugula   (503) staff       (20)        0 2024-05-17 13:36:31.923556 MRCpy-2.3.0/MRCpy.egg-info/
+-rw-r--r--   0 kbondugula   (503) staff       (20)     4980 2024-05-17 13:36:31.000000 MRCpy-2.3.0/MRCpy.egg-info/PKG-INFO
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2312 2024-05-17 13:36:31.000000 MRCpy-2.3.0/MRCpy.egg-info/SOURCES.txt
+-rw-r--r--   0 kbondugula   (503) staff       (20)        1 2024-05-17 13:36:31.000000 MRCpy-2.3.0/MRCpy.egg-info/dependency_links.txt
+-rw-r--r--   0 kbondugula   (503) staff       (20)        1 2024-05-17 13:36:31.000000 MRCpy-2.3.0/MRCpy.egg-info/not-zip-safe
+-rw-r--r--   0 kbondugula   (503) staff       (20)       64 2024-05-17 13:36:31.000000 MRCpy-2.3.0/MRCpy.egg-info/requires.txt
+-rw-r--r--   0 kbondugula   (503) staff       (20)        6 2024-05-17 13:36:31.000000 MRCpy-2.3.0/MRCpy.egg-info/top_level.txt
+-rw-r--r--   0 kbondugula   (503) staff       (20)     4980 2024-05-17 13:36:32.454254 MRCpy-2.3.0/PKG-INFO
+-rw-r--r--   0 kbondugula   (503) staff       (20)     4316 2024-02-14 10:00:13.000000 MRCpy-2.3.0/README.md
+-rw-r--r--   0 kbondugula   (503) staff       (20)      778 2024-05-17 13:29:35.000000 MRCpy-2.3.0/pyproject.toml
+-rw-r--r--   0 kbondugula   (503) staff       (20)      160 2024-05-17 13:36:32.454774 MRCpy-2.3.0/setup.cfg
+-rw-r--r--   0 kbondugula   (503) staff       (20)     2357 2024-02-14 09:37:45.000000 MRCpy-2.3.0/setup.py
```

### Comparing `MRCpy-2.2.0/MRCpy/amrc.py` & `MRCpy-2.3.0/MRCpy/amrc.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/base_mrc.py` & `MRCpy-2.3.0/MRCpy/base_mrc.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/cmrc.py` & `MRCpy-2.3.0/MRCpy/cmrc.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,38 +397,37 @@
 
         # Supress the depreciation warnings
         warnings.simplefilter('ignore')
 
         # In case of 0-1 loss, learn constraints using the phi
         # These constraints are used in the optimization instead of phi
 
-        if self.loss == '0-1':
-            # Summing up the phi configurations
-            # for all possible subsets of classes for each instance
-            F = np.vstack(list(np.sum(phi[:, S, ], axis=1)
-                           for numVals in range(1, self.n_classes + 1)
-                           for S in it.combinations(np.arange(self.n_classes),
-                                                    numVals)))
-
-            # Compute the corresponding length of the subset of classes
-            # for which sums computed for each instance
-            cardS = np.arange(1, self.n_classes + 1).\
-                repeat([n * scs.comb(self.n_classes, numVals)
-                        for numVals in np.arange(1,
-                        self.n_classes + 1)])
-
         if self.solver == 'cvx':
             # Use CVXpy for the convex optimization of the MRC.
 
             # Variables
             mu = cvx.Variable(m)
 
             if self.loss == '0-1':
                 # Constraints in case of 0-1 loss function
 
+                # Summing up the phi configurations
+                # for all possible subsets of classes for each instance
+                F = np.vstack(list(np.sum(phi[:, S, ], axis=1)
+                               for numVals in range(1, self.n_classes + 1)
+                               for S in it.combinations(np.arange(self.n_classes),
+                                                        numVals)))
+
+                # Compute the corresponding length of the subset of classes
+                # for which sums computed for each instance
+                cardS = np.arange(1, self.n_classes + 1).\
+                    repeat([n * scs.comb(self.n_classes, numVals)
+                            for numVals in np.arange(1,
+                            self.n_classes + 1)])
+
                 M = F / (cardS[:, np.newaxis])
                 h = 1 - (1 / cardS)
 
                 # Calculate the psi function and
                 # add it to the objective function
                 # First we calculate the all possible values of psi
                 # for all the points
@@ -606,24 +605,24 @@
         g : `array`-like of shape (n_features)
             Gradient of psi for a given solution and feature mapping.
 
         psi_value : `int`
             The value of psi for a given solution and feature mapping.
         '''
 
-        v = phi@mu
+        v = phi @ mu
         indices = np.argsort(v)[::-1]
         value = v[indices[0]] - 1
         g = phi[indices[0],:]
 
         for k in range(1, self.n_classes):
-            new_value = (k * value + v[indices[k]]) / (k+1)
+            new_value = (k * value + v[indices[k]]) / (k + 1)
             if new_value >= value:
                 value = new_value
-                g = (k * g + phi[indices[k],:]) / (k+1)
+                g = (k * g + phi[indices[k],:]) / (k + 1)
             else:
                 break
 
         return g, (value + 1)
 
     def get_upper_bound(self):
         '''
```

### Comparing `MRCpy-2.2.0/MRCpy/datasets/__init__.py` & `MRCpy-2.3.0/MRCpy/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-sci_Test.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/comp-vs-sci_Test.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-sci_Train.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/comp-vs-sci_Train.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-sci_shortTest.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/comp-vs-sci_shortTest.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-sci_shortTrain.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/comp-vs-sci_shortTrain.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-talk_Test.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/comp-vs-talk_Test.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/comp-vs-talk_Train.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/comp-vs-talk_Train.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/credit.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/credit.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/diabetes.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/diabetes.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/ecoli.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/ecoli.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/glass.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/glass.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/haberman.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/haberman.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/indianLiverPatient.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/indianLiverPatient.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/iris.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/iris.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/letter-recognition.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/letter-recognition.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/mammographic.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/mammographic.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/optdigits.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/optdigits.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/rec-vs-sci_Test.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/rec-vs-sci_Test.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/rec-vs-sci_Train.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/rec-vs-sci_Train.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/rec-vs-talk_Test.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/rec-vs-talk_Test.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/rec-vs-talk_Train.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/rec-vs-talk_Train.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/redwine.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/redwine.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/sci-vs-talk_Test.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/sci-vs-talk_Test.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/sci-vs-talk_Train.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/sci-vs-talk_Train.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/segment.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/segment.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/data/usenet2.csv` & `MRCpy-2.3.0/MRCpy/datasets/data/usenet2.csv`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/adult.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/adult.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/catsvsdogs_features_resnet18.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/catsvsdogs_features_resnet18.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/credit.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/credit.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/diabetes.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/diabetes.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/ecoli.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/ecoli.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/glass.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/glass.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/haberman.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/haberman.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/indianLiverPatient.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/indianLiverPatient.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/iris.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/iris.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/letter-recognition.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/letter-recognition.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/mammographic.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/mammographic.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/mnist_features_resnet18.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/mnist_features_resnet18.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/optdigits.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/optdigits.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/redwine.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/redwine.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/satellite.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/satellite.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/segment.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/segment.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/yearbook.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/yearbook.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/descr/yearbook_features_resnet18.rst` & `MRCpy-2.3.0/MRCpy/datasets/descr/yearbook_features_resnet18.rst`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/datasets/load.py` & `MRCpy-2.3.0/MRCpy/datasets/load.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/dwgcs.py` & `MRCpy-2.3.0/MRCpy/dwgcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -379,18 +379,19 @@
                 beta_ >= np.zeros((n, 1)),
                 beta_ <= (self.B / np.sqrt(self.D)) * np.ones((n, 1)),
                 cvx.sum(beta_) / n - 1 <= epsilon_,
                 -  epsilon_ <= cvx.sum(beta_) / n - 1,
             ]
             problem = cvx.Problem(objective,constraints)
             try:
-                problem.solve(solver = 'ECOS')
+                # Fixing tolerance to ensure replicability across different machines.
+                problem.solve(solver = 'ECOS', feastol = 1e-4, reltol = 1e-3, abstol = 1e-3)
             except cvx.error.SolverError:
                 try:
-                    problem.solve(solver = 'OSQP')
+                    problem.solve(solver = 'SCS')
                 except cvx.error.SolverError:
                     raise ValueError('CVXpy couldn\'t find a solution for ' + \
                                      'alpha and beta .... ' + \
                          'The problem is ', problem.status)
 
             self.beta_ = beta_.value
             self.alpha_ = alpha_
@@ -408,18 +409,19 @@
                 alpha_ >= np.zeros((n, 1)),
                 alpha_ <= np.ones((n, 1)),
                 cvx.sum(alpha_) / t - 1 <= epsilon_,
                 -  epsilon_ <= cvx.sum(alpha_) / t - 1,
             ]
             problem = cvx.Problem(objective,constraints)
             try:
-                problem.solve(solver = 'ECOS')
+                # Fixing tolerance to ensure replicability across different machines.
+                problem.solve(solver = 'ECOS', feastol = 1e-4, reltol = 1e-3, abstol = 1e-3)
             except cvx.error.SolverError:
                 try:
-                    problem.solve(solver = 'OSQP')
+                    problem.solve(solver = 'SCS')
                 except cvx.error.SolverError:
                     raise ValueError('CVXpy couldn\'t find a solution for ' + \
                                      'alpha and beta .... ' + \
                          'The problem is ', problem.status)
 
             self.beta_ = beta_
             self.alpha_ = alpha_.value
@@ -439,27 +441,31 @@
                 alpha_ <= np.ones((t, 1)),
                 cvx.sum(beta_) / n - cvx.sum(alpha_) / t <= epsilon_,
                 - epsilon_ <= cvx.sum(beta_) / n - cvx.sum(alpha_) / t,
                 cvx.norm(alpha_ - np.ones((t, 1))) <= (1 - 1 / np.sqrt(self.D)) * np.sqrt(t)
             ]
             problem = cvx.Problem(objective,constraints)
             try:
-                problem.solve(solver = 'ECOS')
+                # Fixing tolerance to ensure replicability across different machines.
+                problem.solve(solver = 'ECOS', feastol = 1e-4, reltol = 1e-3, abstol = 1e-3)
             except cvx.error.SolverError:
                 try:
-                    problem.solve(solver = 'OSQP')
+                    problem.solve(solver = 'SCS')
                 except cvx.error.SolverError:
                     raise ValueError('CVXpy couldn\'t find a solution for ' + \
                                      'alpha and beta .... ' + \
                          'The problem is ', problem.status)
 
             self.beta_ = beta_.value
             self.alpha_ = alpha_.value
             self.min_DWKMM = problem.value
 
+        self.alpha_[np.isclose(self.alpha_, 0, atol = 1e-5)] = 0
+        self.beta_[np.isclose(self.beta_, 0, atol = 1e-5)] = 0
+
         return self
 
 
     def compute_tau(self, xTr, yTr):
         '''
         Compute mean estimate tau using the given training instances.
 
@@ -528,24 +534,26 @@
             lambda_ >= np.zeros(d),
             cvx.sum(cvx.reshape(p, (n_classes, t)),axis=0) == np.ones(t) / t,
             p >= np.zeros((t * n_classes, 1))
         ]
 
         problem = cvx.Problem(objective, constraints)
         try:
-            problem.solve(solver = 'ECOS')
+            # Fixing tolerance to ensure replicability across different machines.
+            problem.solve(solver = 'ECOS', feastol = 1e-4, reltol = 1e-4, abstol = 1e-4)
         except cvx.error.SolverError:
             try:
-                problem.solve(solver = 'OSQP')
+                problem.solve(solver = 'SCS')
             except cvx.error.SolverError:
                 raise ValueError('CVXpy couldn\'t find a solution for ' + \
                                      'lambda .... ' + \
                          'The problem is ', prob.status)
 
         lambda_ = np.maximum(lambda_.value, 0)
+        lambda_[np.isclose(lambda_, 0)] = 0
 
         return lambda_
     
     def compute_phi(self, X):
         '''
         Compute the feature mapping corresponding to instances given
         for learning the classifiers and prediction.
```

### Comparing `MRCpy-2.2.0/MRCpy/mrc.py` & `MRCpy-2.3.0/MRCpy/mrc.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/phi/base_phi.py` & `MRCpy-2.3.0/MRCpy/phi/base_phi.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         # Efficient configuration in case of binary classification.
         if self.n_classes == 2 and not self.one_hot:
             X_feat[Y == 1, :] = X_feat[Y == 1, :] * -1
             phi = X_feat
 
         # One-hot encoding for multi-class classification.
         else:
-            phi = np.zeros((n, self.n_classes * X_feat.shape[1]))
+            phi = np.zeros((n, self.n_classes * X_feat.shape[1]), dtype=np.float64)
             tweaked_eye_mat = (np.eye(self.n_classes))[Y, :]
             for i in range(n):
                 phi[i, :] = np.kron(tweaked_eye_mat[i], X_feat[i, :])
 
         return phi
 
     def eval_x(self, X):
```

### Comparing `MRCpy-2.2.0/MRCpy/phi/random_fourier_phi.py` & `MRCpy-2.3.0/MRCpy/phi/random_fourier_phi.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/phi/random_relu_phi.py` & `MRCpy-2.3.0/MRCpy/phi/random_relu_phi.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/phi/threshold_phi.py` & `MRCpy-2.3.0/MRCpy/phi/threshold_phi.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/solvers/adam.py` & `MRCpy-2.3.0/MRCpy/solvers/adam.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/solvers/cg.py` & `MRCpy-2.3.0/MRCpy/solvers/cg.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/solvers/cvx.py` & `MRCpy-2.3.0/MRCpy/solvers/cvx.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,33 +34,33 @@
 
     # Solve the problem
     prob = cvx.Problem(objective, constraints)
     try:
         prob.solve(solver=cvx_solvers[0], verbose=False)
         mu_ = mu.value
     except:
-        print('Warning: ' + cvx_solvers[0] + \
-              ' solver couldn\'t solve the problem.\n' + \
-              'Trying with the other solvers ...')
+        # print('Warning: ' + cvx_solvers[0] + \
+        #       ' solver couldn\'t solve the problem.\n' + \
+        #       'Trying with the other solvers ...')
         mu_ = None
 
     # if the solver could not find values of mu for the given solver
     if mu_ is None:
 
         # try with a different solver for solution
         for s in cvx_solvers[1:]:
 
             # Solve the problem
             try:
                 prob.solve(solver=s, verbose=False)
                 mu_ = mu.value
             except:
-                print('Warning: ' + s + \
-                      ' solver couldn\'t solve the problem.\n' + \
-                      'Trying with other solvers')
+                # print('Warning: ' + s + \
+                #       ' solver couldn\'t solve the problem.\n' + \
+                #       'Trying with other solvers')
                 mu_ = None
 
             # Check the values
             mu_ = mu.value
 
             # Break the loop once the solution is obtained
             if mu_ is not None:
```

### Comparing `MRCpy-2.2.0/MRCpy/solvers/nesterov.py` & `MRCpy-2.3.0/MRCpy/solvers/nesterov.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy/solvers/sgd.py` & `MRCpy-2.3.0/MRCpy/solvers/sgd.py`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/MRCpy.egg-info/PKG-INFO` & `MRCpy-2.3.0/MRCpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MRCpy
-Version: 2.2.0
+Version: 2.3.0
 Summary: Library for minimax risk classifiers
 Home-page: https://github.com/MachineLearningBCAM/MRCpy
 Author-email: Kartheek Bondugula <kbondugula@bcamath.org>
 Project-URL: Homepage, https://github.com/MachineLearningBCAM/MRCpy
 Project-URL: Issues, https://github.com/MachineLearningBCAM/MRCpy/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `MRCpy-2.2.0/MRCpy.egg-info/SOURCES.txt` & `MRCpy-2.3.0/MRCpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/PKG-INFO` & `MRCpy-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MRCpy
-Version: 2.2.0
+Version: 2.3.0
 Summary: Library for minimax risk classifiers
 Home-page: https://github.com/MachineLearningBCAM/MRCpy
 Author-email: Kartheek Bondugula <kbondugula@bcamath.org>
 Project-URL: Homepage, https://github.com/MachineLearningBCAM/MRCpy
 Project-URL: Issues, https://github.com/MachineLearningBCAM/MRCpy/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `MRCpy-2.2.0/README.md` & `MRCpy-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `MRCpy-2.2.0/pyproject.toml` & `MRCpy-2.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "MRCpy"
-version = "2.2.0"
+version = "2.3.0"
 authors = [
   { name="Kartheek Bondugula", email="kbondugula@bcamath.org" },
 ]
 description = "Library for minimax risk classifiers"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `MRCpy-2.2.0/setup.py` & `MRCpy-2.3.0/setup.py`

 * *Files identical despite different names*

