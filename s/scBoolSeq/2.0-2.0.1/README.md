# Comparing `tmp/scBoolSeq-2.0.tar.gz` & `tmp/scBoolSeq-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scBoolSeq-2.0.tar", last modified: Thu Oct 19 13:34:12 2023, max compression
+gzip compressed data, was "scBoolSeq-2.0.1.tar", last modified: Fri Oct 20 22:13:37 2023, max compression
```

## Comparing `scBoolSeq-2.0.tar` & `scBoolSeq-2.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 13:34:12.401429 scBoolSeq-2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2023-10-19 13:34:12.401429 scBoolSeq-2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2023-10-19 13:33:56.000000 scBoolSeq-2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 13:34:12.397429 scBoolSeq-2.0/scBoolSeq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2023-10-19 13:34:12.000000 scBoolSeq-2.0/scBoolSeq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-10-19 13:34:12.000000 scBoolSeq-2.0/scBoolSeq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 13:34:12.000000 scBoolSeq-2.0/scBoolSeq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-19 13:34:12.000000 scBoolSeq-2.0/scBoolSeq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-19 13:34:12.000000 scBoolSeq-2.0/scBoolSeq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 13:34:12.401429 scBoolSeq-2.0/scboolseq/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-10-19 13:33:56.000000 scBoolSeq-2.0/scboolseq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-10-19 13:33:56.000000 scBoolSeq-2.0/scboolseq/_core_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-10-19 13:33:56.000000 scBoolSeq-2.0/scboolseq/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2023-10-19 13:33:56.000000 scBoolSeq-2.0/scboolseq/_scboolseq_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-10-19 13:33:56.000000 scBoolSeq-2.0/scboolseq/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    30562 2023-10-19 13:33:56.000000 scBoolSeq-2.0/scboolseq/binarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2023-10-19 13:33:56.000000 scBoolSeq-2.0/scboolseq/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    30725 2023-10-19 13:33:56.000000 scBoolSeq-2.0/scboolseq/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-10-19 13:33:56.000000 scBoolSeq-2.0/scboolseq/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-19 13:34:12.401429 scBoolSeq-2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      920 2023-10-19 13:33:56.000000 scBoolSeq-2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 22:13:37.953834 scBoolSeq-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7531 2023-10-20 22:13:37.953834 scBoolSeq-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2023-10-20 22:13:27.000000 scBoolSeq-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 22:13:37.949834 scBoolSeq-2.0.1/scBoolSeq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7531 2023-10-20 22:13:37.000000 scBoolSeq-2.0.1/scBoolSeq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-10-20 22:13:37.000000 scBoolSeq-2.0.1/scBoolSeq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-20 22:13:37.000000 scBoolSeq-2.0.1/scBoolSeq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-20 22:13:37.000000 scBoolSeq-2.0.1/scBoolSeq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-20 22:13:37.000000 scBoolSeq-2.0.1/scBoolSeq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 22:13:37.953834 scBoolSeq-2.0.1/scboolseq/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2023-10-20 22:13:27.000000 scBoolSeq-2.0.1/scboolseq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-10-20 22:13:27.000000 scBoolSeq-2.0.1/scboolseq/_core_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2023-10-20 22:13:27.000000 scBoolSeq-2.0.1/scboolseq/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2023-10-20 22:13:27.000000 scBoolSeq-2.0.1/scboolseq/_scboolseq_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2023-10-20 22:13:27.000000 scBoolSeq-2.0.1/scboolseq/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30562 2023-10-20 22:13:27.000000 scBoolSeq-2.0.1/scboolseq/binarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2023-10-20 22:13:27.000000 scBoolSeq-2.0.1/scboolseq/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30790 2023-10-20 22:13:27.000000 scBoolSeq-2.0.1/scboolseq/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-10-20 22:13:27.000000 scBoolSeq-2.0.1/scboolseq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-20 22:13:37.953834 scBoolSeq-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2023-10-20 22:13:27.000000 scBoolSeq-2.0.1/setup.py
```

### Comparing `scBoolSeq-2.0/PKG-INFO` & `scBoolSeq-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scBoolSeq
-Version: 2.0
+Version: 2.0.1
 Summary: scBoolSeq: Linking scRNA-Seq Statistics and Boolean Dynamics.
 Home-page: https://github.com/bnediction/scBoolSeq
 Author: Gustavo Magaña López
 Author-email: gustavo.magana@labri.fr
 License: BSD-3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -14,34 +14,29 @@
 
 # scBoolSeq
 
 scRNA-Seq data binarisation and synthetic generation from Boolean dynamics.
 
 ## Installation
 
-We recommend installing `scBoolSeq` via `conda`, but we provide as well a standard `pip` installation. 
-
-### Conda
+### Pip
 
 ```
-conda install -c conda-forge -c colomoto scboolseq
+pip install scboolseq
 ```
 
-### Pip
+### Conda
 
 ```
-pip install scboolseq
+conda install -c conda-forge -c colomoto scboolseq
 ```
 
 ### Docker
 
-The `scBoolSeq` command can be invoked using the `bnediction/scboolseq` image:
-```
-docker run --rm -it -v $PWD:/data -w /data bnediction/scboolseq scBoolSeq ...
-```
+`scBoolSeq` is included in the [ColoMoTo Docker](http://colomoto.org/notebook) distribution.
 
 ## Usage
 
 <!--
 ### Command line
 
 scBoolSeq provides a rich CLI allowing programmatic access to its main functionalities, namely the `binarization` of RNA-Seq data and the
```

### Comparing `scBoolSeq-2.0/README.md` & `scBoolSeq-2.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 
 # scBoolSeq
 
 scRNA-Seq data binarisation and synthetic generation from Boolean dynamics.
 
 ## Installation
 
-We recommend installing `scBoolSeq` via `conda`, but we provide as well a standard `pip` installation. 
-
-### Conda
+### Pip
 
 ```
-conda install -c conda-forge -c colomoto scboolseq
+pip install scboolseq
 ```
 
-### Pip
+### Conda
 
 ```
-pip install scboolseq
+conda install -c conda-forge -c colomoto scboolseq
 ```
 
 ### Docker
 
-The `scBoolSeq` command can be invoked using the `bnediction/scboolseq` image:
-```
-docker run --rm -it -v $PWD:/data -w /data bnediction/scboolseq scBoolSeq ...
-```
+`scBoolSeq` is included in the [ColoMoTo Docker](http://colomoto.org/notebook) distribution.
 
 ## Usage
 
 <!--
 ### Command line
 
 scBoolSeq provides a rich CLI allowing programmatic access to its main functionalities, namely the `binarization` of RNA-Seq data and the
```

### Comparing `scBoolSeq-2.0/scBoolSeq.egg-info/PKG-INFO` & `scBoolSeq-2.0.1/scBoolSeq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scBoolSeq
-Version: 2.0
+Version: 2.0.1
 Summary: scBoolSeq: Linking scRNA-Seq Statistics and Boolean Dynamics.
 Home-page: https://github.com/bnediction/scBoolSeq
 Author: Gustavo Magaña López
 Author-email: gustavo.magana@labri.fr
 License: BSD-3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -14,34 +14,29 @@
 
 # scBoolSeq
 
 scRNA-Seq data binarisation and synthetic generation from Boolean dynamics.
 
 ## Installation
 
-We recommend installing `scBoolSeq` via `conda`, but we provide as well a standard `pip` installation. 
-
-### Conda
+### Pip
 
 ```
-conda install -c conda-forge -c colomoto scboolseq
+pip install scboolseq
 ```
 
-### Pip
+### Conda
 
 ```
-pip install scboolseq
+conda install -c conda-forge -c colomoto scboolseq
 ```
 
 ### Docker
 
-The `scBoolSeq` command can be invoked using the `bnediction/scboolseq` image:
-```
-docker run --rm -it -v $PWD:/data -w /data bnediction/scboolseq scBoolSeq ...
-```
+`scBoolSeq` is included in the [ColoMoTo Docker](http://colomoto.org/notebook) distribution.
 
 ## Usage
 
 <!--
 ### Command line
 
 scBoolSeq provides a rich CLI allowing programmatic access to its main functionalities, namely the `binarization` of RNA-Seq data and the
```

### Comparing `scBoolSeq-2.0/scboolseq/_core_utils.py` & `scBoolSeq-2.0.1/scboolseq/_core_utils.py`

 * *Files identical despite different names*

### Comparing `scBoolSeq-2.0/scboolseq/_scboolseq_core.py` & `scBoolSeq-2.0.1/scboolseq/_scboolseq_core.py`

 * *Files identical despite different names*

### Comparing `scBoolSeq-2.0/scboolseq/_types.py` & `scBoolSeq-2.0.1/scboolseq/_types.py`

 * *Files identical despite different names*

### Comparing `scBoolSeq-2.0/scboolseq/binarization.py` & `scBoolSeq-2.0.1/scboolseq/binarization.py`

 * *Files identical despite different names*

### Comparing `scBoolSeq-2.0/scboolseq/meta.py` & `scBoolSeq-2.0.1/scboolseq/meta.py`

 * *Files identical despite different names*

### Comparing `scBoolSeq-2.0/scboolseq/simulation.py` & `scBoolSeq-2.0.1/scboolseq/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -828,14 +828,15 @@
     # https://numpy.org/doc/stable/reference/random/parallel.html
     _seed_sequence_generator = np.random.SeedSequence(seed)
     child_seeds = _seed_sequence_generator.spawn(n_threads)
     streams = [np.random.default_rng(s) for s in child_seeds]
     modes = len(child_seeds) * [dropout_mode]
 
     if n_threads > 1:
+        n_threads = min(n_threads, simulation_criteria.shape[0])
         _criteria_ls = np.array_split(simulation_criteria, n_threads)
         _binary_ls = np.array_split(binary_df, n_threads, axis=1)
         with mp.Pool(n_threads) as pool:
             ret_list = pool.starmap(
                 _simulate_subset, zip(_binary_ls, _criteria_ls, streams, modes)
             )
         return pd.concat(ret_list, axis=1)
```

### Comparing `scBoolSeq-2.0/scboolseq/utils.py` & `scBoolSeq-2.0.1/scboolseq/utils.py`

 * *Files identical despite different names*

### Comparing `scBoolSeq-2.0/setup.py` & `scBoolSeq-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8
 
 from setuptools import find_packages
 from setuptools import setup
 
 NAME = "scBoolSeq"
-VERSION = "2.0"
+VERSION = "2.0.1"
 
 setup(
     name=NAME,
     version=VERSION,
     author="Gustavo Magaña López",
     author_email="gustavo.magana@labri.fr",
     url="https://github.com/bnediction/scBoolSeq",
```

