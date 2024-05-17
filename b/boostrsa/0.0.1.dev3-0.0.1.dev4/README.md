# Comparing `tmp/boostrsa-0.0.1.dev3.tar.gz` & `tmp/boostrsa-0.0.1.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boostrsa-0.0.1.dev3.tar", last modified: Thu May 16 23:48:03 2024, max compression
+gzip compressed data, was "boostrsa-0.0.1.dev4.tar", last modified: Fri May 17 08:38:05 2024, max compression
```

## Comparing `boostrsa-0.0.1.dev3.tar` & `boostrsa-0.0.1.dev4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-16 23:48:03.882949 boostrsa-0.0.1.dev3/
--rw-rw-r--   0 seojin    (1007) seojin    (1008)     1069 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev3/LICENSE.txt
--rw-r--r--   0 seojin    (1007) seojin    (1008)     2943 2024-05-16 23:48:03.882949 boostrsa-0.0.1.dev3/PKG-INFO
--rw-rw-r--   0 seojin    (1007) seojin    (1008)     2417 2024-05-16 13:38:32.000000 boostrsa-0.0.1.dev3/README.md
--rw-rw-r--   0 seojin    (1007) seojin    (1008)       38 2024-05-16 23:48:03.882949 boostrsa-0.0.1.dev3/setup.cfg
--rw-rw-r--   0 seojin    (1007) seojin    (1008)      851 2024-05-16 23:47:48.000000 boostrsa-0.0.1.dev3/setup.py
-drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-16 23:48:03.878949 boostrsa-0.0.1.dev3/src/
-drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-16 23:48:03.882949 boostrsa-0.0.1.dev3/src/boostrsa/
--rw-rw-r--   0 seojin    (1007) seojin    (1008)        0 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev3/src/boostrsa/__init__.py
--rw-rw-r--   0 seojin    (1007) seojin    (1008)      100 2024-05-09 11:03:42.000000 boostrsa-0.0.1.dev3/src/boostrsa/boostrsa_types.py
-drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-16 23:48:03.882949 boostrsa-0.0.1.dev3/src/boostrsa/cores/
--rw-rw-r--   0 seojin    (1007) seojin    (1008)        0 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev3/src/boostrsa/cores/__init__.py
-drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-16 23:48:03.882949 boostrsa-0.0.1.dev3/src/boostrsa/cores/cpgpu/
--rw-rw-r--   0 seojin    (1007) seojin    (1008)        0 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev3/src/boostrsa/cores/cpgpu/__init__.py
--rw-rw-r--   0 seojin    (1007) seojin    (1008)     4494 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev3/src/boostrsa/cores/cpgpu/stats.py
-drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-16 23:48:03.882949 boostrsa-0.0.1.dev3/src/boostrsa/cores/cpu/
--rw-rw-r--   0 seojin    (1007) seojin    (1008)        0 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev3/src/boostrsa/cores/cpu/__init__.py
--rw-rw-r--   0 seojin    (1007) seojin    (1008)     1046 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev3/src/boostrsa/cores/cpu/matrix.py
-drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-16 23:48:03.882949 boostrsa-0.0.1.dev3/src/boostrsa/cores/gpu/
--rw-rw-r--   0 seojin    (1007) seojin    (1008)        0 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev3/src/boostrsa/cores/gpu/__init__.py
--rw-rw-r--   0 seojin    (1007) seojin    (1008)     1329 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev3/src/boostrsa/cores/gpu/basic_operations.py
--rw-rw-r--   0 seojin    (1007) seojin    (1008)      669 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev3/src/boostrsa/cores/gpu/mask.py
--rw-rw-r--   0 seojin    (1007) seojin    (1008)     3551 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev3/src/boostrsa/cores/gpu/matrix.py
--rw-rw-r--   0 seojin    (1007) seojin    (1008)     8812 2024-05-16 23:42:36.000000 boostrsa-0.0.1.dev3/src/boostrsa/searchlight.py
-drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-16 23:48:03.882949 boostrsa-0.0.1.dev3/src/boostrsa.egg-info/
--rw-r--r--   0 seojin    (1007) seojin    (1008)     2943 2024-05-16 23:48:03.000000 boostrsa-0.0.1.dev3/src/boostrsa.egg-info/PKG-INFO
--rw-rw-r--   0 seojin    (1007) seojin    (1008)      627 2024-05-16 23:48:03.000000 boostrsa-0.0.1.dev3/src/boostrsa.egg-info/SOURCES.txt
--rw-rw-r--   0 seojin    (1007) seojin    (1008)        1 2024-05-16 23:48:03.000000 boostrsa-0.0.1.dev3/src/boostrsa.egg-info/dependency_links.txt
--rw-rw-r--   0 seojin    (1007) seojin    (1008)       18 2024-05-16 23:48:03.000000 boostrsa-0.0.1.dev3/src/boostrsa.egg-info/requires.txt
--rw-rw-r--   0 seojin    (1007) seojin    (1008)        9 2024-05-16 23:48:03.000000 boostrsa-0.0.1.dev3/src/boostrsa.egg-info/top_level.txt
-drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-16 23:48:03.882949 boostrsa-0.0.1.dev3/tests/
--rw-rw-r--   0 seojin    (1007) seojin    (1008)       46 2024-05-09 13:50:20.000000 boostrsa-0.0.1.dev3/tests/test_module1.py
+drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-17 08:38:05.956519 boostrsa-0.0.1.dev4/
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)     1069 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev4/LICENSE.txt
+-rw-r--r--   0 seojin    (1007) seojin    (1008)     3181 2024-05-17 08:38:05.956519 boostrsa-0.0.1.dev4/PKG-INFO
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)     2655 2024-05-17 08:35:20.000000 boostrsa-0.0.1.dev4/README.md
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)       38 2024-05-17 08:38:05.956519 boostrsa-0.0.1.dev4/setup.cfg
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)      851 2024-05-16 23:57:01.000000 boostrsa-0.0.1.dev4/setup.py
+drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-17 08:38:05.956519 boostrsa-0.0.1.dev4/src/
+drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-17 08:38:05.956519 boostrsa-0.0.1.dev4/src/boostrsa/
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)        0 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev4/src/boostrsa/__init__.py
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)      100 2024-05-09 11:03:42.000000 boostrsa-0.0.1.dev4/src/boostrsa/boostrsa_types.py
+drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-17 08:38:05.956519 boostrsa-0.0.1.dev4/src/boostrsa/cores/
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)        0 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev4/src/boostrsa/cores/__init__.py
+drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-17 08:38:05.956519 boostrsa-0.0.1.dev4/src/boostrsa/cores/cpgpu/
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)        0 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev4/src/boostrsa/cores/cpgpu/__init__.py
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)     4505 2024-05-16 23:56:02.000000 boostrsa-0.0.1.dev4/src/boostrsa/cores/cpgpu/stats.py
+drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-17 08:38:05.956519 boostrsa-0.0.1.dev4/src/boostrsa/cores/cpu/
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)        0 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev4/src/boostrsa/cores/cpu/__init__.py
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)     1046 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev4/src/boostrsa/cores/cpu/matrix.py
+drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-17 08:38:05.956519 boostrsa-0.0.1.dev4/src/boostrsa/cores/gpu/
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)        0 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev4/src/boostrsa/cores/gpu/__init__.py
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)     1329 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev4/src/boostrsa/cores/gpu/basic_operations.py
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)      669 2024-05-09 11:03:41.000000 boostrsa-0.0.1.dev4/src/boostrsa/cores/gpu/mask.py
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)     3570 2024-05-17 00:04:02.000000 boostrsa-0.0.1.dev4/src/boostrsa/cores/gpu/matrix.py
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)     8857 2024-05-16 23:59:45.000000 boostrsa-0.0.1.dev4/src/boostrsa/searchlight.py
+drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-17 08:38:05.956519 boostrsa-0.0.1.dev4/src/boostrsa.egg-info/
+-rw-r--r--   0 seojin    (1007) seojin    (1008)     3181 2024-05-17 08:38:05.000000 boostrsa-0.0.1.dev4/src/boostrsa.egg-info/PKG-INFO
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)      627 2024-05-17 08:38:05.000000 boostrsa-0.0.1.dev4/src/boostrsa.egg-info/SOURCES.txt
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)        1 2024-05-17 08:38:05.000000 boostrsa-0.0.1.dev4/src/boostrsa.egg-info/dependency_links.txt
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)       18 2024-05-17 08:38:05.000000 boostrsa-0.0.1.dev4/src/boostrsa.egg-info/requires.txt
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)        9 2024-05-17 08:38:05.000000 boostrsa-0.0.1.dev4/src/boostrsa.egg-info/top_level.txt
+drwxrwxr-x   0 seojin    (1007) seojin    (1008)        0 2024-05-17 08:38:05.956519 boostrsa-0.0.1.dev4/tests/
+-rw-rw-r--   0 seojin    (1007) seojin    (1008)       46 2024-05-09 13:50:20.000000 boostrsa-0.0.1.dev4/tests/test_module1.py
```

### Comparing `boostrsa-0.0.1.dev3/LICENSE.txt` & `boostrsa-0.0.1.dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `boostrsa-0.0.1.dev3/PKG-INFO` & `boostrsa-0.0.1.dev4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boostrsa
-Version: 0.0.1.dev3
+Version: 0.0.1.dev4
 Summary: This is toolbox for boosting calculation speed using GPU
 Home-page: https://github.com/SeojinYoon/boostrsa.git
 Author: seojin
 Author-email: pures1@hanyang.ac.kr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,38 +26,46 @@
 
 Basically, this library uses a Nvidia's GPU instead of CPU for parallel processing. In the searchlight analysis, the data targeted for constructing the RDM in volvxes a voxel and its neighboring voxels. That is well-suited for parallel processing since the calculations for each target are independent of one another. This library utilizes GPU-compatible libraries such as Numba and Cupy to facilitate this process.
 
 ## Dependencies
 
 To use this library, you need to have a Nvidia's GPU and CUDA. Additionally, this library heavily relies on Cupy and Numba. It is essential to install the appropriate versions of these libraries.
 
-### Cupy
+### cupy
 
 Cupy is designed to work with specific versions of CUDA. See cupy's guide and install appropriate version in correspond to your system (https://github.com/cupy/cupy).
 
 Please check your cuda version to install cupy.
 - versions
     - cupy-cuda10x (for cuda 10)
     - cupy-cuda11x (for cuda 11)
     - cupy-cuda12x (for cuda 12)
     
 
 If you installed the cuda10 in your computer, then install cupy-cuda10x. install cupy-cuda10x. ex) pip install cupy-cuda10x
 
-### Numba
+### numba
 
 The numba library is a powerful tool that enbales python functions to be compiled to machine code at runtime using the LLVM. One of its key features is the ability to generate native code for different architectures, including CPUs and GPUs, which greatly accelerates the execution of data-heavy and computationally intense python code.
 
 Please see installation guideline of numba (https://numba.pydata.org/numba-doc/latest/user/installing.html).
 
 Pip installation). 
+
 - pip install numba
 
+### rsatoolbox
+
+The rsatoolbox is a Python library specifically designed for Representational Similarity Analysis (RSA). 
+
+Please see installation guideline of rsatoolbox (https://github.com/rsagroup/rsatoolbox)
+
+- pip install rsatoolbox
 
-## Installation
+# Installation
 
 pip install boostrsa
 
 # Checked version
 
 These are the latest checked environment.
```

### Comparing `boostrsa-0.0.1.dev3/README.md` & `boostrsa-0.0.1.dev4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,38 +9,46 @@
 
 Basically, this library uses a Nvidia's GPU instead of CPU for parallel processing. In the searchlight analysis, the data targeted for constructing the RDM in volvxes a voxel and its neighboring voxels. That is well-suited for parallel processing since the calculations for each target are independent of one another. This library utilizes GPU-compatible libraries such as Numba and Cupy to facilitate this process.
 
 ## Dependencies
 
 To use this library, you need to have a Nvidia's GPU and CUDA. Additionally, this library heavily relies on Cupy and Numba. It is essential to install the appropriate versions of these libraries.
 
-### Cupy
+### cupy
 
 Cupy is designed to work with specific versions of CUDA. See cupy's guide and install appropriate version in correspond to your system (https://github.com/cupy/cupy).
 
 Please check your cuda version to install cupy.
 - versions
     - cupy-cuda10x (for cuda 10)
     - cupy-cuda11x (for cuda 11)
     - cupy-cuda12x (for cuda 12)
     
 
 If you installed the cuda10 in your computer, then install cupy-cuda10x. install cupy-cuda10x. ex) pip install cupy-cuda10x
 
-### Numba
+### numba
 
 The numba library is a powerful tool that enbales python functions to be compiled to machine code at runtime using the LLVM. One of its key features is the ability to generate native code for different architectures, including CPUs and GPUs, which greatly accelerates the execution of data-heavy and computationally intense python code.
 
 Please see installation guideline of numba (https://numba.pydata.org/numba-doc/latest/user/installing.html).
 
 Pip installation). 
+
 - pip install numba
 
+### rsatoolbox
+
+The rsatoolbox is a Python library specifically designed for Representational Similarity Analysis (RSA). 
+
+Please see installation guideline of rsatoolbox (https://github.com/rsagroup/rsatoolbox)
+
+- pip install rsatoolbox
 
-## Installation
+# Installation
 
 pip install boostrsa
 
 # Checked version
 
 These are the latest checked environment.
```

### Comparing `boostrsa-0.0.1.dev3/setup.py` & `boostrsa-0.0.1.dev4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "boostrsa",
-    version = "0.0.1dev3",
+    version = "0.0.1dev4",
     author = "seojin",
     author_email = "pures1@hanyang.ac.kr",
     description = "This is toolbox for boosting calculation speed using GPU",
     long_description = long_description,
     long_description_content_type="text/markdown",
     url = "https://github.com/SeojinYoon/boostrsa.git",
     packages = find_packages(where = "src"),
```

### Comparing `boostrsa-0.0.1.dev3/src/boostrsa/cores/cpgpu/stats.py` & `boostrsa-0.0.1.dev4/src/boostrsa/cores/cpgpu/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import numpy as np
 import cupy as cp
 from numba import cuda, jit
-from boostrsa.src.types import ShrinkageMethod
-from boostrsa.src.gpu.basic_operations import outer_sum_square, outer_sum
-from boostrsa.src.gpu.matrix import diag, eyes
-from boostrsa.src.gpu.basic_operations import scaling
+from boostrsa.boostrsa_types import ShrinkageMethod
+from boostrsa.cores.gpu.basic_operations import outer_sum_square, outer_sum
+from boostrsa.cores.gpu.matrix import diag, eyes
+from boostrsa.cores.gpu.basic_operations import scaling
 
 def _covariance_eye(residuals, threads_per_block = 1024):
     """
     Computes an optimal shrinkage estimate of a sample covariance matrix as described by the following publication:
     **matrix should be demeaned before!
     
     Ledoit and Wolfe (2004): "A well-conditioned estimator for large-dimensional covariance matrices"
```

### Comparing `boostrsa-0.0.1.dev3/src/boostrsa/cores/cpu/matrix.py` & `boostrsa-0.0.1.dev4/src/boostrsa/cores/cpu/matrix.py`

 * *Files identical despite different names*

### Comparing `boostrsa-0.0.1.dev3/src/boostrsa/cores/gpu/basic_operations.py` & `boostrsa-0.0.1.dev4/src/boostrsa/cores/gpu/basic_operations.py`

 * *Files identical despite different names*

### Comparing `boostrsa-0.0.1.dev3/src/boostrsa/cores/gpu/mask.py` & `boostrsa-0.0.1.dev4/src/boostrsa/cores/gpu/mask.py`

 * *Files identical despite different names*

### Comparing `boostrsa-0.0.1.dev3/src/boostrsa/cores/gpu/matrix.py` & `boostrsa-0.0.1.dev4/src/boostrsa/cores/gpu/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from numba import cuda, jit
-from basic_operations import matmul
+from boostrsa.cores.gpu.basic_operations import matmul
 
 @jit(nopython=True)
 def upper_tri_1d_index(i, j, n_col, k):
     """
     Get upper triangle 1d index
     
     if k = 1)
```

### Comparing `boostrsa-0.0.1.dev3/src/boostrsa/searchlight.py` & `boostrsa-0.0.1.dev4/src/boostrsa/searchlight.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import numpy as np
 from numba import cuda, jit
 import cupy as cp
 import itertools
 from tqdm import trange
 
 # Custom Libraries
-from boostrsa_types import ShrinkageMethod
-from cores.cpu.matrix import convert_1d_to_symmertic, mean_fold_variance
-from cores.cpgpu.stats import _covariance_diag, _covariance_eye
-from cores.gpu.mask import set_mask
-from cores.gpu.matrix import calc_kernel, rdm_from_kernel
+from boostrsa.boostrsa_types import ShrinkageMethod
+from boostrsa.cores.cpu.matrix import convert_1d_to_symmertic, mean_fold_variance
+from boostrsa.cores.cpgpu.stats import _covariance_diag, _covariance_eye
+from boostrsa.cores.gpu.mask import set_mask
+from boostrsa.cores.gpu.matrix import calc_kernel, rdm_from_kernel
 
 # Functions
 def calc_sl_precision(residuals, 
                       neighbors, 
                       n_split_data, 
                       masking_indexes, 
                       n_thread_per_block = 1024,
```

### Comparing `boostrsa-0.0.1.dev3/src/boostrsa.egg-info/PKG-INFO` & `boostrsa-0.0.1.dev4/src/boostrsa.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boostrsa
-Version: 0.0.1.dev3
+Version: 0.0.1.dev4
 Summary: This is toolbox for boosting calculation speed using GPU
 Home-page: https://github.com/SeojinYoon/boostrsa.git
 Author: seojin
 Author-email: pures1@hanyang.ac.kr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,38 +26,46 @@
 
 Basically, this library uses a Nvidia's GPU instead of CPU for parallel processing. In the searchlight analysis, the data targeted for constructing the RDM in volvxes a voxel and its neighboring voxels. That is well-suited for parallel processing since the calculations for each target are independent of one another. This library utilizes GPU-compatible libraries such as Numba and Cupy to facilitate this process.
 
 ## Dependencies
 
 To use this library, you need to have a Nvidia's GPU and CUDA. Additionally, this library heavily relies on Cupy and Numba. It is essential to install the appropriate versions of these libraries.
 
-### Cupy
+### cupy
 
 Cupy is designed to work with specific versions of CUDA. See cupy's guide and install appropriate version in correspond to your system (https://github.com/cupy/cupy).
 
 Please check your cuda version to install cupy.
 - versions
     - cupy-cuda10x (for cuda 10)
     - cupy-cuda11x (for cuda 11)
     - cupy-cuda12x (for cuda 12)
     
 
 If you installed the cuda10 in your computer, then install cupy-cuda10x. install cupy-cuda10x. ex) pip install cupy-cuda10x
 
-### Numba
+### numba
 
 The numba library is a powerful tool that enbales python functions to be compiled to machine code at runtime using the LLVM. One of its key features is the ability to generate native code for different architectures, including CPUs and GPUs, which greatly accelerates the execution of data-heavy and computationally intense python code.
 
 Please see installation guideline of numba (https://numba.pydata.org/numba-doc/latest/user/installing.html).
 
 Pip installation). 
+
 - pip install numba
 
+### rsatoolbox
+
+The rsatoolbox is a Python library specifically designed for Representational Similarity Analysis (RSA). 
+
+Please see installation guideline of rsatoolbox (https://github.com/rsagroup/rsatoolbox)
+
+- pip install rsatoolbox
 
-## Installation
+# Installation
 
 pip install boostrsa
 
 # Checked version
 
 These are the latest checked environment.
```

### Comparing `boostrsa-0.0.1.dev3/src/boostrsa.egg-info/SOURCES.txt` & `boostrsa-0.0.1.dev4/src/boostrsa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

