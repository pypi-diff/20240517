# Comparing `tmp/napf-0.0.7.tar.gz` & `tmp/napf-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napf-0.0.7.tar", last modified: Wed Nov 15 16:09:57 2023, max compression
+gzip compressed data, was "napf-0.0.8.tar", last modified: Fri May 17 21:25:39 2024, max compression
```

## Comparing `napf-0.0.7.tar` & `napf-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:09:57.842572 napf-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-11-15 16:09:49.000000 napf-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-15 16:09:49.000000 napf-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2023-11-15 16:09:57.842572 napf-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-11-15 16:09:49.000000 napf-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:09:57.838572 napf-0.0.7/napf/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-11-15 16:09:49.000000 napf-0.0.7/napf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-15 16:09:49.000000 napf-0.0.7/napf/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11622 2023-11-15 16:09:49.000000 napf-0.0.7/napf/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:09:57.838572 napf-0.0.7/napf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2023-11-15 16:09:57.000000 napf-0.0.7/napf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      603 2023-11-15 16:09:57.000000 napf-0.0.7/napf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 16:09:57.000000 napf-0.0.7/napf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 16:09:57.000000 napf-0.0.7/napf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-15 16:09:57.000000 napf-0.0.7/napf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-15 16:09:57.000000 napf-0.0.7/napf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-11-15 16:09:49.000000 napf-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-11-15 16:09:57.842572 napf-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2023-11-15 16:09:49.000000 napf-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:09:57.838572 napf-0.0.7/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2023-11-15 16:09:49.000000 napf-0.0.7/src/napf.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:09:57.838572 napf-0.0.7/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:09:57.842572 napf-0.0.7/src/python/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-11-15 16:09:49.000000 napf-0.0.7/src/python/classes/double_trees.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-11-15 16:09:49.000000 napf-0.0.7/src/python/classes/float_trees.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-11-15 16:09:49.000000 napf-0.0.7/src/python/classes/int_trees.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-11-15 16:09:49.000000 napf-0.0.7/src/python/classes/long_trees.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      516 2023-11-15 16:09:49.000000 napf-0.0.7/src/python/classes/radius_search_result_vectors.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      486 2023-11-15 16:09:49.000000 napf-0.0.7/src/python/napf.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14800 2023-11-15 16:09:49.000000 napf-0.0.7/src/python/pykdt.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2023-11-15 16:09:49.000000 napf-0.0.7/src/python/threadhelper.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:09:57.842572 napf-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2023-11-15 16:09:49.000000 napf-0.0.7/tests/test_init_and_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 16:09:57.842572 napf-0.0.7/third_party/
--rw-r--r--   0 runner    (1001) docker     (127)    89255 2023-11-15 16:09:49.000000 napf-0.0.7/third_party/nanoflann.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:25:39.602674 napf-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 21:25:33.000000 napf-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-17 21:25:33.000000 napf-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-17 21:25:39.602674 napf-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-17 21:25:33.000000 napf-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:25:39.598674 napf-0.0.8/napf/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-17 21:25:33.000000 napf-0.0.8/napf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 21:25:33.000000 napf-0.0.8/napf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11622 2024-05-17 21:25:33.000000 napf-0.0.8/napf/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:25:39.602674 napf-0.0.8/napf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-17 21:25:39.000000 napf-0.0.8/napf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-17 21:25:39.000000 napf-0.0.8/napf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:25:39.000000 napf-0.0.8/napf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:25:39.000000 napf-0.0.8/napf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 21:25:39.000000 napf-0.0.8/napf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-17 21:25:39.000000 napf-0.0.8/napf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-17 21:25:33.000000 napf-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-17 21:25:39.602674 napf-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-17 21:25:33.000000 napf-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:25:39.598674 napf-0.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-17 21:25:33.000000 napf-0.0.8/src/napf.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:25:39.602674 napf-0.0.8/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:25:39.602674 napf-0.0.8/src/python/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-17 21:25:33.000000 napf-0.0.8/src/python/classes/double_trees.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-17 21:25:33.000000 napf-0.0.8/src/python/classes/float_trees.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-17 21:25:33.000000 napf-0.0.8/src/python/classes/int_trees.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-17 21:25:33.000000 napf-0.0.8/src/python/classes/long_trees.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-17 21:25:33.000000 napf-0.0.8/src/python/classes/radius_search_result_vectors.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-17 21:25:33.000000 napf-0.0.8/src/python/napf.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14768 2024-05-17 21:25:33.000000 napf-0.0.8/src/python/pykdt.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-17 21:25:33.000000 napf-0.0.8/src/python/threadhelper.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:25:39.602674 napf-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-17 21:25:33.000000 napf-0.0.8/tests/test_init_and_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:25:39.602674 napf-0.0.8/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)    92645 2024-05-17 21:25:33.000000 napf-0.0.8/third_party/nanoflann.hpp
```

### Comparing `napf-0.0.7/LICENSE` & `napf-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `napf-0.0.7/PKG-INFO` & `napf-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napf
-Version: 0.0.7
+Version: 0.0.8
 Summary: nanoflann python bindings for kdtree.
 Home-page: https://github.com/tataratat/napf
 Author: Jaewook Lee
 Author-email: jaewooklee042@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -24,18 +24,17 @@
 # napf
 [![main](https://github.com/tataratat/napf/actions/workflows/main.yml/badge.svg)](https://github.com/tataratat/napf/actions/workflows/main.yml)
 [![PyPI version](https://badge.fury.io/py/napf.svg)](https://badge.fury.io/py/napf)
 
 [nanoflann](https://github.com/jlblancoc/nanoflann) wrappers for python and maybe fortran.
 
 ## python
-As `nanoflann` offers template classes, separate classes are implemented in `napf` for each ___{datatype, data dimension, distance metric}___. All the search functions are equipped with multi-thread execution. Uses [numpy.ndarray](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) for data input and output.
+As `nanoflann` offers template classes, separate classes are implemented in `napf` for each ___{datatype, distance metric}___. All the search functions are equipped with multi-thread execution. Uses [numpy.ndarray](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) for data input and output.
 Currently, the combinations of following options are supported:
 - `data type`: {__double__, __float__, __int__, __long__}  _(corresponds to {np.float64, np.float32, np.int32, np.int64})_
-- `data dimension`: {__1__, __2__, __3__, __4__, __5__, __6__, __7__, __8__, __9__, __10__, __11__, __12__, __13__, __14__, __15__, __16__, __17__, __18__, __19__, __20__}
 - `distance metric`: {__L1__, __L2__}
 Note that functions return squared distances, when you use the __L2__ metric.
 
 ### quick start
 __install with pip:__
 ```
 pip install --upgrade pip
@@ -48,29 +47,28 @@
 import numpy as np
 
 data = <data in 2D array>
 queries = <query points in 2D array>
 
 kdt = napf.KDT(tree_data=data, metric=1)
 
-indices, distances = kdt.knn_search(
+distances, indices = kdt.knn_search(
     queries=queries,
     kneighbors=3,
     nthread=4,
 )
 ...
 ```
 
 ## fortran
-maybe...
-
+If you need fortran bindings, please let us know by creating an [issue](https://gthub.com/tataratat/napf/issues).
 
 ## Documentation
 This package uses a `sphinx` based documentation. An online version of the documentation can be found at [napf - documentation](https://tataratat.github.io/napf/).
 
 If you want to build the documentation yourself use the following commands in the package root directory.
 ```bash
 pip install -r ./docs/requirements.txt
-sphinx-build -W -b html docs/source docs/build -j auto
+sphinx-build -W -b html docs/source docs/build
 ```
 
 You will find the documentation in the docs/build folder.
```

### Comparing `napf-0.0.7/README.md` & `napf-0.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # napf
 [![main](https://github.com/tataratat/napf/actions/workflows/main.yml/badge.svg)](https://github.com/tataratat/napf/actions/workflows/main.yml)
 [![PyPI version](https://badge.fury.io/py/napf.svg)](https://badge.fury.io/py/napf)
 
 [nanoflann](https://github.com/jlblancoc/nanoflann) wrappers for python and maybe fortran.
 
 ## python
-As `nanoflann` offers template classes, separate classes are implemented in `napf` for each ___{datatype, data dimension, distance metric}___. All the search functions are equipped with multi-thread execution. Uses [numpy.ndarray](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) for data input and output.
+As `nanoflann` offers template classes, separate classes are implemented in `napf` for each ___{datatype, distance metric}___. All the search functions are equipped with multi-thread execution. Uses [numpy.ndarray](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) for data input and output.
 Currently, the combinations of following options are supported:
 - `data type`: {__double__, __float__, __int__, __long__}  _(corresponds to {np.float64, np.float32, np.int32, np.int64})_
-- `data dimension`: {__1__, __2__, __3__, __4__, __5__, __6__, __7__, __8__, __9__, __10__, __11__, __12__, __13__, __14__, __15__, __16__, __17__, __18__, __19__, __20__}
 - `distance metric`: {__L1__, __L2__}
 Note that functions return squared distances, when you use the __L2__ metric.
 
 ### quick start
 __install with pip:__
 ```
 pip install --upgrade pip
@@ -25,29 +24,28 @@
 import numpy as np
 
 data = <data in 2D array>
 queries = <query points in 2D array>
 
 kdt = napf.KDT(tree_data=data, metric=1)
 
-indices, distances = kdt.knn_search(
+distances, indices = kdt.knn_search(
     queries=queries,
     kneighbors=3,
     nthread=4,
 )
 ...
 ```
 
 ## fortran
-maybe...
-
+If you need fortran bindings, please let us know by creating an [issue](https://gthub.com/tataratat/napf/issues).
 
 ## Documentation
 This package uses a `sphinx` based documentation. An online version of the documentation can be found at [napf - documentation](https://tataratat.github.io/napf/).
 
 If you want to build the documentation yourself use the following commands in the package root directory.
 ```bash
 pip install -r ./docs/requirements.txt
-sphinx-build -W -b html docs/source docs/build -j auto
+sphinx-build -W -b html docs/source docs/build
 ```
 
 You will find the documentation in the docs/build folder.
```

### Comparing `napf-0.0.7/napf/base.py` & `napf-0.0.8/napf/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
         queries: (m, d) np.ndarray
           Data type will be casted to the same type as `tree_data`.
         nthread: int
           Default is None and will use self.nthread.
 
         Returns
         --------
-        ids_and_distances: tuple
+        distances_and_ids: tuple
           ((m, 1) np.ndarray - double dists,)
            (m, 1) np.ndarray - uint ids)
         """
         if nthread is None:
             nthread = self.nthread
 
         return self.core_tree.query(
```

### Comparing `napf-0.0.7/napf.egg-info/PKG-INFO` & `napf-0.0.8/napf.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napf
-Version: 0.0.7
+Version: 0.0.8
 Summary: nanoflann python bindings for kdtree.
 Home-page: https://github.com/tataratat/napf
 Author: Jaewook Lee
 Author-email: jaewooklee042@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -24,18 +24,17 @@
 # napf
 [![main](https://github.com/tataratat/napf/actions/workflows/main.yml/badge.svg)](https://github.com/tataratat/napf/actions/workflows/main.yml)
 [![PyPI version](https://badge.fury.io/py/napf.svg)](https://badge.fury.io/py/napf)
 
 [nanoflann](https://github.com/jlblancoc/nanoflann) wrappers for python and maybe fortran.
 
 ## python
-As `nanoflann` offers template classes, separate classes are implemented in `napf` for each ___{datatype, data dimension, distance metric}___. All the search functions are equipped with multi-thread execution. Uses [numpy.ndarray](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) for data input and output.
+As `nanoflann` offers template classes, separate classes are implemented in `napf` for each ___{datatype, distance metric}___. All the search functions are equipped with multi-thread execution. Uses [numpy.ndarray](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html) for data input and output.
 Currently, the combinations of following options are supported:
 - `data type`: {__double__, __float__, __int__, __long__}  _(corresponds to {np.float64, np.float32, np.int32, np.int64})_
-- `data dimension`: {__1__, __2__, __3__, __4__, __5__, __6__, __7__, __8__, __9__, __10__, __11__, __12__, __13__, __14__, __15__, __16__, __17__, __18__, __19__, __20__}
 - `distance metric`: {__L1__, __L2__}
 Note that functions return squared distances, when you use the __L2__ metric.
 
 ### quick start
 __install with pip:__
 ```
 pip install --upgrade pip
@@ -48,29 +47,28 @@
 import numpy as np
 
 data = <data in 2D array>
 queries = <query points in 2D array>
 
 kdt = napf.KDT(tree_data=data, metric=1)
 
-indices, distances = kdt.knn_search(
+distances, indices = kdt.knn_search(
     queries=queries,
     kneighbors=3,
     nthread=4,
 )
 ...
 ```
 
 ## fortran
-maybe...
-
+If you need fortran bindings, please let us know by creating an [issue](https://gthub.com/tataratat/napf/issues).
 
 ## Documentation
 This package uses a `sphinx` based documentation. An online version of the documentation can be found at [napf - documentation](https://tataratat.github.io/napf/).
 
 If you want to build the documentation yourself use the following commands in the package root directory.
 ```bash
 pip install -r ./docs/requirements.txt
-sphinx-build -W -b html docs/source docs/build -j auto
+sphinx-build -W -b html docs/source docs/build
 ```
 
 You will find the documentation in the docs/build folder.
```

### Comparing `napf-0.0.7/napf.egg-info/SOURCES.txt` & `napf-0.0.8/napf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napf-0.0.7/setup.py` & `napf-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `napf-0.0.7/src/napf.hpp` & `napf-0.0.8/src/napf.hpp`

 * *Files identical despite different names*

### Comparing `napf-0.0.7/src/python/classes/radius_search_result_vectors.cpp` & `napf-0.0.8/src/python/classes/radius_search_result_vectors.cpp`

 * *Files identical despite different names*

### Comparing `napf-0.0.7/src/python/pykdt.hpp` & `napf-0.0.8/src/python/pykdt.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -119,16 +119,15 @@
     py::buffer_info i_buf = indices.request();
     IndexType* i_buf_ptr = static_cast<IndexType*>(i_buf.ptr);
     py::array_t<DistT> dist(qlen * kneighbors);
     py::buffer_info d_buf = dist.request();
     DistT* d_buf_ptr = static_cast<DistT*>(d_buf.ptr);
 
     if (kneighbors > static_cast<int>(datalen_)) {
-      std::cout << "WARNING - "
-                << "kneighbors (" << kneighbors
+      std::cout << "WARNING - " << "kneighbors (" << kneighbors
                 << ") is bigger than number of tree data (" << datalen_ << "! "
                 << "Returning arrays `[:, " << datalen_ - kneighbors
                 << ":]` entries will be filled with random indices."
                 << std::endl;
     }
 
     // prepare routine in lambda so that it can be executed with nthreads
@@ -348,17 +347,16 @@
     const py::buffer_info r_buf = radii.request();
     const DistT* r_buf_ptr = static_cast<DistT*>(r_buf.ptr);
     const int rlen = r_buf.shape[0];
 
     // execution ending error is too brutal and merciless
     // print warning and return empty
     if (qlen != rlen) {
-      std::cout << "CRITICAL WARNING - "
-                << "query length (" << qlen << ") and radii length (" << rlen
-                << ") differ! "
+      std::cout << "CRITICAL WARNING - " << "query length (" << qlen
+                << ") and radii length (" << rlen << ") differ! "
                 << "returning empty tuple." << std::endl;
 
       return py::tuple{};
     }
 
     nanoflann::SearchParameters params;
     params.sorted = return_sorted;
```

### Comparing `napf-0.0.7/src/python/threadhelper.hpp` & `napf-0.0.8/src/python/threadhelper.hpp`

 * *Files identical despite different names*

### Comparing `napf-0.0.7/tests/test_init_and_query.py` & `napf-0.0.8/tests/test_init_and_query.py`

 * *Files identical despite different names*

### Comparing `napf-0.0.7/third_party/nanoflann.hpp` & `napf-0.0.8/third_party/nanoflann.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 /***********************************************************************
  * Software License Agreement (BSD License)
  *
  * Copyright 2008-2009  Marius Muja (mariusm@cs.ubc.ca). All rights reserved.
  * Copyright 2008-2009  David G. Lowe (lowe@cs.ubc.ca). All rights reserved.
- * Copyright 2011-2022  Jose Luis Blanco (joseluisblancoc@gmail.com).
+ * Copyright 2011-2024  Jose Luis Blanco (joseluisblancoc@gmail.com).
  *   All rights reserved.
  *
  * THE BSD LICENSE
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions
  * are met:
@@ -45,26 +45,27 @@
 #pragma once
 
 #include <algorithm>
 #include <array>
 #include <atomic>
 #include <cassert>
 #include <cmath>  // for abs()
+#include <cstdint>
 #include <cstdlib>  // for abs()
 #include <functional>  // std::reference_wrapper
 #include <future>
 #include <istream>
 #include <limits>  // std::numeric_limits
 #include <ostream>
 #include <stdexcept>
 #include <unordered_set>
 #include <vector>
 
 /** Library version: 0xMmP (M=Major,m=minor,P=patch) */
-#define NANOFLANN_VERSION 0x150
+#define NANOFLANN_VERSION 0x155
 
 // Avoid conflicting declaration of min/max macros in Windows headers
 #if !defined(NOMINMAX) && \
     (defined(_WIN32) || defined(_WIN32_) || defined(WIN32) || defined(_WIN64))
 #define NOMINMAX
 #ifdef max
 #undef max
@@ -154,14 +155,16 @@
     assign(Container& c, const size_t nElements, const T& value)
 {
     for (size_t i = 0; i < nElements; i++) c[i] = value;
 }
 
 /** @addtogroup result_sets_grp Result set classes
  *  @{ */
+
+/** Result set for KNN searches (N-closest neighbors) */
 template <
     typename _DistanceType, typename _IndexType = size_t,
     typename _CountType = size_t>
 class KNNResultSet
 {
    public:
     using DistanceType = _DistanceType;
@@ -186,16 +189,100 @@
         dists   = dists_;
         count   = 0;
         if (capacity)
             dists[capacity - 1] = (std::numeric_limits<DistanceType>::max)();
     }
 
     CountType size() const { return count; }
+    bool      empty() const { return count == 0; }
+    bool      full() const { return count == capacity; }
+
+    /**
+     * Called during search to add an element matching the criteria.
+     * @return true if the search should be continued, false if the results are
+     * sufficient
+     */
+    bool addPoint(DistanceType dist, IndexType index)
+    {
+        CountType i;
+        for (i = count; i > 0; --i)
+        {
+            /** If defined and two points have the same distance, the one with
+             *  the lowest-index will be returned first. */
+#ifdef NANOFLANN_FIRST_MATCH
+            if ((dists[i - 1] > dist) ||
+                ((dist == dists[i - 1]) && (indices[i - 1] > index)))
+            {
+#else
+            if (dists[i - 1] > dist)
+            {
+#endif
+                if (i < capacity)
+                {
+                    dists[i]   = dists[i - 1];
+                    indices[i] = indices[i - 1];
+                }
+            }
+            else
+                break;
+        }
+        if (i < capacity)
+        {
+            dists[i]   = dist;
+            indices[i] = index;
+        }
+        if (count < capacity) count++;
+
+        // tell caller that the search shall continue
+        return true;
+    }
+
+    DistanceType worstDist() const { return dists[capacity - 1]; }
+};
 
-    bool full() const { return count == capacity; }
+/** Result set for RKNN searches (N-closest neighbors with a maximum radius) */
+template <
+    typename _DistanceType, typename _IndexType = size_t,
+    typename _CountType = size_t>
+class RKNNResultSet
+{
+   public:
+    using DistanceType = _DistanceType;
+    using IndexType    = _IndexType;
+    using CountType    = _CountType;
+
+   private:
+    IndexType*    indices;
+    DistanceType* dists;
+    CountType     capacity;
+    CountType     count;
+    DistanceType  maximumSearchDistanceSquared;
+
+   public:
+    explicit RKNNResultSet(
+        CountType capacity_, DistanceType maximumSearchDistanceSquared_)
+        : indices(nullptr),
+          dists(nullptr),
+          capacity(capacity_),
+          count(0),
+          maximumSearchDistanceSquared(maximumSearchDistanceSquared_)
+    {
+    }
+
+    void init(IndexType* indices_, DistanceType* dists_)
+    {
+        indices = indices_;
+        dists   = dists_;
+        count   = 0;
+        if (capacity) dists[capacity - 1] = maximumSearchDistanceSquared;
+    }
+
+    CountType size() const { return count; }
+    bool      empty() const { return count == 0; }
+    bool      full() const { return count == capacity; }
 
     /**
      * Called during search to add an element matching the criteria.
      * @return true if the search should be continued, false if the results are
      * sufficient
      */
     bool addPoint(DistanceType dist, IndexType index)
@@ -740,26 +827,24 @@
  * object or consolidating fragmented memory.  Second, the decision about
  * how long to keep an object is made at the time of allocation, and there
  * is no need to track down all the objects to free them.
  *
  */
 class PooledAllocator
 {
-    static constexpr size_t WORDSIZE  = 16;
+    static constexpr size_t WORDSIZE  = 16;  // WORDSIZE must >= 8
     static constexpr size_t BLOCKSIZE = 8192;
 
     /* We maintain memory alignment to word boundaries by requiring that all
         allocations be in multiples of the machine wordsize.  */
     /* Size of machine word in bytes.  Must be power of 2. */
     /* Minimum number of bytes requested at a time from	the system.  Must be
      * multiple of WORDSIZE. */
 
-    using Offset    = uint32_t;
-    using Size      = uint32_t;
-    using Dimension = int32_t;
+    using Size = size_t;
 
     Size  remaining_ = 0;  //!< Number of bytes left in current block of storage
     void* base_ = nullptr;  //!< Pointer to base of current block of storage
     void* loc_  = nullptr;  //!< Current location in block to next allocate
 
     void internal_init()
     {
@@ -813,36 +898,30 @@
          */
         if (size > remaining_)
         {
             wastedMemory += remaining_;
 
             /* Allocate new storage. */
             const Size blocksize =
-                (size + sizeof(void*) + (WORDSIZE - 1) > BLOCKSIZE)
-                    ? size + sizeof(void*) + (WORDSIZE - 1)
-                    : BLOCKSIZE;
+                size > BLOCKSIZE ? size + WORDSIZE : BLOCKSIZE + WORDSIZE;
 
             // use the standard C malloc to allocate memory
             void* m = ::malloc(blocksize);
             if (!m)
             {
                 fprintf(stderr, "Failed to allocate memory.\n");
                 throw std::bad_alloc();
             }
 
             /* Fill first word of new block with pointer to previous block. */
             static_cast<void**>(m)[0] = base_;
             base_                     = m;
 
-            Size shift = 0;
-            // int size_t = (WORDSIZE - ( (((size_t)m) + sizeof(void*)) &
-            // (WORDSIZE-1))) & (WORDSIZE-1);
-
-            remaining_ = blocksize - sizeof(void*) - shift;
-            loc_       = (static_cast<char*>(m) + sizeof(void*) + shift);
+            remaining_ = blocksize - WORDSIZE;
+            loc_       = static_cast<char*>(m) + WORDSIZE;
         }
         void* rloc = loc_;
         loc_       = static_cast<char*>(loc_) + size;
         remaining_ -= size;
 
         usedMemory += size;
 
@@ -1143,59 +1222,48 @@
             Offset       idx;
             Dimension    cutfeat;
             DistanceType cutval;
             middleSplit_(obj, left, right - left, idx, cutfeat, cutval, bbox);
 
             node->node_type.sub.divfeat = cutfeat;
 
-            std::future<NodePtr> left_future, right_future;
-
-            BoundingBox left_bbox(bbox);
-            left_bbox[cutfeat].high = cutval;
-            if (++thread_count < n_thread_build_)
-            {
-                left_future = std::async(
-                    std::launch::async, &KDTreeBaseClass::divideTreeConcurrent,
-                    this, std::ref(obj), left, left + idx, std::ref(left_bbox),
-                    std::ref(thread_count), std::ref(mutex));
-            }
-            else
-            {
-                --thread_count;
-                node->child1 = this->divideTreeConcurrent(
-                    obj, left, left + idx, left_bbox, thread_count, mutex);
-            }
+            std::future<NodePtr> right_future;
 
             BoundingBox right_bbox(bbox);
             right_bbox[cutfeat].low = cutval;
             if (++thread_count < n_thread_build_)
             {
+                // Concurrent right sub-tree
                 right_future = std::async(
                     std::launch::async, &KDTreeBaseClass::divideTreeConcurrent,
                     this, std::ref(obj), left + idx, right,
                     std::ref(right_bbox), std::ref(thread_count),
                     std::ref(mutex));
             }
             else
             {
                 --thread_count;
-                node->child2 = this->divideTreeConcurrent(
-                    obj, left + idx, right, right_bbox, thread_count, mutex);
             }
 
-            if (left_future.valid())
-            {
-                node->child1 = left_future.get();
-                --thread_count;
-            }
+            BoundingBox left_bbox(bbox);
+            left_bbox[cutfeat].high = cutval;
+            node->child1            = this->divideTreeConcurrent(
+                           obj, left, left + idx, left_bbox, thread_count, mutex);
+
             if (right_future.valid())
             {
+                // Block and wait for concurrent right sub-tree
                 node->child2 = right_future.get();
                 --thread_count;
             }
+            else
+            {
+                node->child2 = this->divideTreeConcurrent(
+                    obj, left + idx, right, right_bbox, thread_count, mutex);
+            }
 
             node->node_type.sub.divlow  = left_bbox[cutfeat].high;
             node->node_type.sub.divhigh = right_bbox[cutfeat].low;
 
             for (Dimension i = 0; i < dims; ++i)
             {
                 bbox[i].low  = std::min(left_bbox[i].low, right_bbox[i].low);
@@ -1216,33 +1284,34 @@
         for (Dimension i = 1; i < dims; ++i)
         {
             ElementType span = bbox[i].high - bbox[i].low;
             if (span > max_span) { max_span = span; }
         }
         ElementType max_spread = -1;
         cutfeat                = 0;
+        ElementType min_elem = 0, max_elem = 0;
         for (Dimension i = 0; i < dims; ++i)
         {
             ElementType span = bbox[i].high - bbox[i].low;
             if (span > (1 - EPS) * max_span)
             {
-                ElementType min_elem, max_elem;
-                computeMinMax(obj, ind, count, i, min_elem, max_elem);
-                ElementType spread = max_elem - min_elem;
+                ElementType min_elem_, max_elem_;
+                computeMinMax(obj, ind, count, i, min_elem_, max_elem_);
+                ElementType spread = max_elem_ - min_elem_;
                 if (spread > max_spread)
                 {
                     cutfeat    = i;
                     max_spread = spread;
+                    min_elem   = min_elem_;
+                    max_elem   = max_elem_;
                 }
             }
         }
         // split in the middle
         DistanceType split_val = (bbox[cutfeat].low + bbox[cutfeat].high) / 2;
-        ElementType  min_elem, max_elem;
-        computeMinMax(obj, ind, count, cutfeat, min_elem, max_elem);
 
         if (split_val < min_elem)
             cutval = min_elem;
         else if (split_val > max_elem)
             cutval = max_elem;
         else
             cutval = split_val;
@@ -1554,18 +1623,22 @@
         if (Base::n_thread_build_ == 1)
         {
             Base::root_node_ =
                 this->divideTree(*this, 0, Base::size_, Base::root_bbox_);
         }
         else
         {
+#ifndef NANOFLANN_NO_THREADS
             std::atomic<unsigned int> thread_count(0u);
             std::mutex                mutex;
             Base::root_node_ = this->divideTreeConcurrent(
                 *this, 0, Base::size_, Base::root_bbox_, thread_count, mutex);
+#else /* NANOFLANN_NO_THREADS */
+            throw std::runtime_error("Multithreading is disabled");
+#endif /* NANOFLANN_NO_THREADS */
         }
     }
 
     /** \name Query methods
      * @{ */
 
     /**
@@ -1676,14 +1749,42 @@
         const ElementType* query_point, SEARCH_CALLBACK& resultSet,
         const SearchParameters& searchParams = {}) const
     {
         findNeighbors(resultSet, query_point, searchParams);
         return resultSet.size();
     }
 
+    /**
+     * Find the first N neighbors to \a query_point[0:dim-1] within a maximum
+     * radius. The output is given as a vector of pairs, of which the first
+     * element is a point index and the second the corresponding distance.
+     * Previous contents of \a IndicesDists are cleared.
+     *
+     * \sa radiusSearch, findNeighbors
+     * \return Number `N` of valid points in the result set.
+     *
+     * \note If L2 norms are used, all returned distances are actually squared
+     *       distances.
+     *
+     * \note Only the first `N` entries in `out_indices` and `out_distances`
+     *       will be valid. Return is less than `num_closest` only if the
+     *       number of elements in the tree is less than `num_closest`.
+     */
+    Size rknnSearch(
+        const ElementType* query_point, const Size num_closest,
+        IndexType* out_indices, DistanceType* out_distances,
+        const DistanceType& radius) const
+    {
+        nanoflann::RKNNResultSet<DistanceType, IndexType> resultSet(
+            num_closest, radius);
+        resultSet.init(out_indices, out_distances);
+        findNeighbors(resultSet, query_point);
+        return resultSet.size();
+    }
+
     /** @} */
 
    public:
     /** Make sure the auxiliary list \a vind has the same size than the current
      * dataset, and re-generate if size has changed. */
     void init_vind()
     {
@@ -1989,18 +2090,22 @@
         if (Base::n_thread_build_ == 1)
         {
             Base::root_node_ =
                 this->divideTree(*this, 0, Base::size_, Base::root_bbox_);
         }
         else
         {
+#ifndef NANOFLANN_NO_THREADS
             std::atomic<unsigned int> thread_count(0u);
             std::mutex                mutex;
             Base::root_node_ = this->divideTreeConcurrent(
                 *this, 0, Base::size_, Base::root_bbox_, thread_count, mutex);
+#else /* NANOFLANN_NO_THREADS */
+            throw std::runtime_error("Multithreading is disabled");
+#endif /* NANOFLANN_NO_THREADS */
         }
     }
 
     /** \name Query methods
      * @{ */
 
     /**
@@ -2056,19 +2161,20 @@
      *
      * \note Only the first `N` entries in `out_indices` and `out_distances`
      *       will be valid. Return may be less than `num_closest` only if the
      *       number of elements in the tree is less than `num_closest`.
      */
     Size knnSearch(
         const ElementType* query_point, const Size num_closest,
-        IndexType* out_indices, DistanceType* out_distances) const
+        IndexType* out_indices, DistanceType* out_distances,
+        const SearchParameters& searchParams = {}) const
     {
         nanoflann::KNNResultSet<DistanceType, IndexType> resultSet(num_closest);
         resultSet.init(out_indices, out_distances);
-        findNeighbors(resultSet, query_point);
+        findNeighbors(resultSet, query_point, searchParams);
         return resultSet.size();
     }
 
     /**
      * Find all the neighbors to \a query_point[0:dim-1] within a maximum
      * radius. The output is given as a vector of pairs, of which the first
      * element is a point index and the second the corresponding distance.
```

