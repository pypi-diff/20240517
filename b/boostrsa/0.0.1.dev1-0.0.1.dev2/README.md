# Comparing `tmp/boostrsa-0.0.1.dev1-py3-none-any.whl.zip` & `tmp/boostrsa-0.0.1.dev2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 10832 bytes, number of entries: 17
+Zip file size: 11029 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx        0 b- defN 24-May-09 11:03 boostrsa/__init__.py
--rw-rw-r--  2.0 unx     8803 b- defN 24-May-09 11:03 boostrsa/searchlight.py
+-rw-rw-r--  2.0 unx      100 b- defN 24-May-09 11:03 boostrsa/boostrsa_types.py
+-rw-rw-r--  2.0 unx     8812 b- defN 24-May-16 23:42 boostrsa/searchlight.py
 -rw-rw-r--  2.0 unx      100 b- defN 24-May-09 11:03 boostrsa/types.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-May-09 11:03 boostrsa/cores/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-May-09 11:03 boostrsa/cores/cpgpu/__init__.py
 -rw-rw-r--  2.0 unx     4494 b- defN 24-May-09 11:03 boostrsa/cores/cpgpu/stats.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-May-09 11:03 boostrsa/cores/cpu/__init__.py
 -rw-rw-r--  2.0 unx     1046 b- defN 24-May-09 11:03 boostrsa/cores/cpu/matrix.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-May-09 11:03 boostrsa/cores/gpu/__init__.py
 -rw-rw-r--  2.0 unx     1329 b- defN 24-May-09 11:03 boostrsa/cores/gpu/basic_operations.py
 -rw-rw-r--  2.0 unx      669 b- defN 24-May-09 11:03 boostrsa/cores/gpu/mask.py
 -rw-rw-r--  2.0 unx     3551 b- defN 24-May-09 11:03 boostrsa/cores/gpu/matrix.py
--rw-rw-r--  2.0 unx     1069 b- defN 24-May-16 23:34 boostrsa-0.0.1.dev1.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     2943 b- defN 24-May-16 23:34 boostrsa-0.0.1.dev1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-16 23:34 boostrsa-0.0.1.dev1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 24-May-16 23:34 boostrsa-0.0.1.dev1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1413 b- defN 24-May-16 23:34 boostrsa-0.0.1.dev1.dist-info/RECORD
-17 files, 25518 bytes uncompressed, 8478 bytes compressed:  66.8%
+-rw-rw-r--  2.0 unx     1069 b- defN 24-May-16 23:43 boostrsa-0.0.1.dev2.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     2943 b- defN 24-May-16 23:43 boostrsa-0.0.1.dev2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-16 23:43 boostrsa-0.0.1.dev2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 24-May-16 23:43 boostrsa-0.0.1.dev2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1495 b- defN 24-May-16 23:43 boostrsa-0.0.1.dev2.dist-info/RECORD
+18 files, 25709 bytes uncompressed, 8547 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: boostrsa/__init__.py
 Comment: 
 
+Filename: boostrsa/boostrsa_types.py
+Comment: 
+
 Filename: boostrsa/searchlight.py
 Comment: 
 
 Filename: boostrsa/types.py
 Comment: 
 
 Filename: boostrsa/cores/__init__.py
@@ -30,23 +33,23 @@
 
 Filename: boostrsa/cores/gpu/mask.py
 Comment: 
 
 Filename: boostrsa/cores/gpu/matrix.py
 Comment: 
 
-Filename: boostrsa-0.0.1.dev1.dist-info/LICENSE.txt
+Filename: boostrsa-0.0.1.dev2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: boostrsa-0.0.1.dev1.dist-info/METADATA
+Filename: boostrsa-0.0.1.dev2.dist-info/METADATA
 Comment: 
 
-Filename: boostrsa-0.0.1.dev1.dist-info/WHEEL
+Filename: boostrsa-0.0.1.dev2.dist-info/WHEEL
 Comment: 
 
-Filename: boostrsa-0.0.1.dev1.dist-info/top_level.txt
+Filename: boostrsa-0.0.1.dev2.dist-info/top_level.txt
 Comment: 
 
-Filename: boostrsa-0.0.1.dev1.dist-info/RECORD
+Filename: boostrsa-0.0.1.dev2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## boostrsa/searchlight.py

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 from numba import cuda, jit
 import cupy as cp
 import itertools
 from tqdm import trange
 
 # Custom Libraries
-from types import ShrinkageMethod
+from boostrsa_types import ShrinkageMethod
 from cores.cpu.matrix import convert_1d_to_symmertic, mean_fold_variance
 from cores.cpgpu.stats import _covariance_diag, _covariance_eye
 from cores.gpu.mask import set_mask
 from cores.gpu.matrix import calc_kernel, rdm_from_kernel
 
 # Functions
 def calc_sl_precision(residuals,
```

## Comparing `boostrsa-0.0.1.dev1.dist-info/LICENSE.txt` & `boostrsa-0.0.1.dev2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `boostrsa-0.0.1.dev1.dist-info/METADATA` & `boostrsa-0.0.1.dev2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boostrsa
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: This is toolbox for boosting calculation speed using GPU
 Home-page: https://github.com/SeojinYoon/boostrsa.git
 Author: seojin
 Author-email: pures1@hanyang.ac.kr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `boostrsa-0.0.1.dev1.dist-info/RECORD` & `boostrsa-0.0.1.dev2.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 boostrsa/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-boostrsa/searchlight.py,sha256=KMVqjdhCU_ZNZe92hYJEWuAlS3s5JoA0rv2uciGSqQs,8803
+boostrsa/boostrsa_types.py,sha256=lebVS3iq3tWoUr6EtQqFOSQ6DebK65-QcdvmPhNBcmc,100
+boostrsa/searchlight.py,sha256=EMg-RCgifMZ105d2hprIq-EZsioiyym9tDBU9VnT-wk,8812
 boostrsa/types.py,sha256=lebVS3iq3tWoUr6EtQqFOSQ6DebK65-QcdvmPhNBcmc,100
 boostrsa/cores/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 boostrsa/cores/cpgpu/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 boostrsa/cores/cpgpu/stats.py,sha256=fKIOfchntSeGXkEYUyay5Tv2sx7ZFcLZekYHV8Jw9SM,4494
 boostrsa/cores/cpu/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 boostrsa/cores/cpu/matrix.py,sha256=u8xwPP1NZy2EEbZuQfBs7zgEewMfXMXNO0CdnHWbqgk,1046
 boostrsa/cores/gpu/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 boostrsa/cores/gpu/basic_operations.py,sha256=JXG_AenOLbkFZivdcBqjq9bEpR5Tg8pZ58Uh8DeE0dU,1329
 boostrsa/cores/gpu/mask.py,sha256=PJ5IBElI9QK-5gKnaHzM_McwiTdI4eAUjLaeXU1wUp0,669
 boostrsa/cores/gpu/matrix.py,sha256=8ZC9I1MuF-9No30XyCLw7bCET7UgYels-3_WJh5j-64,3551
-boostrsa-0.0.1.dev1.dist-info/LICENSE.txt,sha256=rRxZ2W7igWGwEeG4euxXY27O0EpCLXsfNJDA6flkrAk,1069
-boostrsa-0.0.1.dev1.dist-info/METADATA,sha256=M6BH-IYm6axXU08a3ylLXfBQT52Qzqyr_aMhqY6aw9U,2943
-boostrsa-0.0.1.dev1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-boostrsa-0.0.1.dev1.dist-info/top_level.txt,sha256=B-iYD_cA6HhxZfPlR0O10gaczZ5lv9yMAbsWqRhc1Ms,9
-boostrsa-0.0.1.dev1.dist-info/RECORD,,
+boostrsa-0.0.1.dev2.dist-info/LICENSE.txt,sha256=rRxZ2W7igWGwEeG4euxXY27O0EpCLXsfNJDA6flkrAk,1069
+boostrsa-0.0.1.dev2.dist-info/METADATA,sha256=6OANFaIyBJVRm5zgAipb5V8odaTf7dlHqHKvhcQfSak,2943
+boostrsa-0.0.1.dev2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+boostrsa-0.0.1.dev2.dist-info/top_level.txt,sha256=B-iYD_cA6HhxZfPlR0O10gaczZ5lv9yMAbsWqRhc1Ms,9
+boostrsa-0.0.1.dev2.dist-info/RECORD,,
```

