# Comparing `tmp/elphem-0.2.0.tar.gz` & `tmp/elphem-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elphem-0.2.0.tar", last modified: Wed Apr 17 09:09:59 2024, max compression
+gzip compressed data, was "elphem-0.3.1.tar", last modified: Fri May 17 14:54:33 2024, max compression
```

## Comparing `elphem-0.2.0.tar` & `elphem-0.3.1.tar`

### file list

```diff
@@ -1,56 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.025802 elphem-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 09:09:55.000000 elphem-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-04-17 09:09:59.025802 elphem-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-17 09:09:55.000000 elphem-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.021802 elphem-0.2.0/elphem/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.021802 elphem-0.2.0/elphem/const/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/const/atomic_weight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/const/brillouin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3006 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/const/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.021802 elphem-0.2.0/elphem/electron/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/electron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/electron/free.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.021802 elphem-0.2.0/elphem/elph/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/elph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/elph/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/elph/epr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/elph/self_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/elph/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.021802 elphem-0.2.0/elphem/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/lattice/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9629 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/lattice/empty.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4768 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/lattice/rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.021802 elphem-0.2.0/elphem/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/phonon/debye.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.025802 elphem-0.2.0/elphem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-04-17 09:09:59.000000 elphem-0.2.0/elphem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-17 09:09:59.000000 elphem-0.2.0/elphem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:09:59.000000 elphem-0.2.0/elphem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 09:09:59.000000 elphem-0.2.0/elphem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 09:09:59.000000 elphem-0.2.0/elphem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:09:59.025802 elphem-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-17 09:09:55.000000 elphem-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.021802 elphem-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.025802 elphem-0.2.0/tests/const/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/const/test_atomic_weight.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/const/test_brillouin.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/const/test_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.025802 elphem-0.2.0/tests/electron/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/electron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/electron/test_free.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.025802 elphem-0.2.0/tests/elph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/elph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/elph/test_epr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/elph/test_self_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/elph/test_spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.025802 elphem-0.2.0/tests/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/lattice/test_empty_lattice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.025802 elphem-0.2.0/tests/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/phonon/test_debye.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.215528 elphem-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 14:54:28.000000 elphem-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-05-17 14:54:33.215528 elphem-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-17 14:54:28.000000 elphem-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.207527 elphem-0.3.1/elphem/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.211528 elphem-0.3.1/elphem/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/common/atomic_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/common/brillouin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/common/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/common/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/common/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/common/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.211528 elphem-0.3.1/elphem/electron/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/electron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/electron/electron.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.211528 elphem-0.3.1/elphem/elph/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/elph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/elph/electron_phonon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/elph/green_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.211528 elphem-0.3.1/elphem/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/lattice/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/lattice/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/lattice/lattice_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/lattice/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/lattice/primitive_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/lattice/reciprocal_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/lattice/rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.211528 elphem-0.3.1/elphem/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-17 14:54:28.000000 elphem-0.3.1/elphem/phonon/phonon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.215528 elphem-0.3.1/elphem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-05-17 14:54:33.000000 elphem-0.3.1/elphem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-17 14:54:33.000000 elphem-0.3.1/elphem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:54:33.000000 elphem-0.3.1/elphem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 14:54:33.000000 elphem-0.3.1/elphem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 14:54:33.000000 elphem-0.3.1/elphem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:54:33.215528 elphem-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-17 14:54:28.000000 elphem-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.211528 elphem-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.215528 elphem-0.3.1/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/common/test_atomic_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/common/test_brillouin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/common/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.215528 elphem-0.3.1/tests/electron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/electron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/electron/test_electron.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.215528 elphem-0.3.1/tests/elph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/elph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/elph/test_self_energy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.215528 elphem-0.3.1/tests/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/lattice/test_lattice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:33.215528 elphem-0.3.1/tests/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-17 14:54:28.000000 elphem-0.3.1/tests/phonon/test_phonon.py
```

### Comparing `elphem-0.2.0/LICENSE` & `elphem-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elphem-0.2.0/elphem/const/atomic_weight.py` & `elphem-0.3.1/elphem/common/atomic_weight.py`

 * *Files identical despite different names*

### Comparing `elphem-0.2.0/elphem/const/unit.py` & `elphem-0.3.1/elphem/common/unit.py`

 * *Files identical despite different names*

### Comparing `elphem-0.2.0/elphem/elph/distribution.py` & `elphem-0.3.1/elphem/common/distribution.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,53 @@
 import sys
 import numpy as np
 
-from elphem.const.unit import Energy
-
-# Setting up system-related constants and warning filters
-float_min = sys.float_info.min
-float_max = sys.float_info.max
-
-def safe_divide(a: np.ndarray | float | int, b: np.ndarray | float | int, default=np.nan):
-    """
-    Safely divides two numbers, arrays, or a combination thereof, with optional handling of division by zero.
-
-    Args:
-        a (np.ndarray | float | int): Numerator, can be a number or an array.
-        b (np.ndarray | float | int): Denominator, can be a number or an array.
-        default (float | int, optional): Value to use when division by zero occurs. Default is NaN.
-
-    Returns:
-        np.ndarray: Result of the division, with division by zero handled gracefully.
-    """
-    a_array = np.full_like(b, a)
-    with np.errstate(divide='ignore', invalid='ignore'):
-        result = np.divide(a_array, b, out=np.full_like(b, default), where=b != 0)
-    return result
+from elphem.common.unit import Energy
+from elphem.common.function import safe_divide
 
 def boltzmann_distribution(temperature: float, energy: float | np.ndarray) -> float | np.ndarray:
     """
     Calculates the occupation number of particles following the Boltzmann distribution.
 
     Args:
         temperature (float): Temperature in Kelvin.
         energy (float | np.ndarray): Energy value(s) in Hartree atomic units.
 
     Returns:
         float | np.ndarray: Occupation number(s) based on the Boltzmann distribution.
     """
+
+    # Setting up system-related constants and warning filters
+    float_min = sys.float_info.min
+    float_max = sys.float_info.max
+
     kbt = max(temperature * Energy.KELVIN["->"], float_min)
     beta = safe_divide(1.0, kbt, default=float_max)
 
     ln = - beta * energy
-    return np.exp(ln, out=np.zeros_like(energy), where=ln > -np.log(float_max))
+    
+    safe_ln_min = np.log(float_min)
+    safe_ln_max = np.log(float_max)
+    
+    return np.exp(ln, out=np.zeros_like(energy), where=((ln > safe_ln_min) & (ln < safe_ln_max)))
 
 def fermi_distribution(temperature: float, energy: float | np.ndarray) -> float | np.ndarray:
     """
     Calculates the occupation number of particles following the Fermi-Dirac distribution.
 
     Args:
         temperature (float): Temperature in Kelvin.
         energy (float | np.ndarray): Energy value(s) in Hartree atomic units.
 
     Returns:
         float | np.ndarray: Occupation number(s) based on the Fermi-Dirac distribution.
     """
     boltzmann_factor = boltzmann_distribution(temperature, energy)
     inv_boltzmann_factor = safe_divide(1.0, boltzmann_factor)
+
     return safe_divide(1.0, inv_boltzmann_factor + 1.0)
 
 def bose_distribution(temperature: float, energy: float | np.ndarray) -> float | np.ndarray:
     """
     Calculates the occupation number of particles following the Bose-Einstein distribution.
 
     Args:
@@ -65,23 +55,23 @@
         energy (float | np.ndarray): Energy value(s) in Hartree atomic units.
 
     Returns:
         float | np.ndarray: Occupation number(s) based on the Bose-Einstein distribution.
     """
     boltzmann_factor = boltzmann_distribution(temperature, energy)
     inv_boltzmann_factor = safe_divide(1.0, boltzmann_factor)
+    
     return safe_divide(1.0, inv_boltzmann_factor - 1.0)
 
 def gaussian_distribution(sigma: float, energy: float | np.ndarray) -> float | np.ndarray:
     """
     Calculates the probability density of particles following the Gaussian distribution.
 
     Args:
         sigma (float): Standard deviation of the Gaussian distribution.
         energy (float | np.ndarray): Energy value(s) to evaluate the Gaussian function.
 
     Returns:
         float | np.ndarray: Probability density(s) based on the Gaussian distribution.
     """
-    if sigma == 0:
-        raise ValueError("Sigma must not be zero.")
+    
     return np.exp(- energy ** 2 / (2.0 * sigma ** 2)) / (np.sqrt(2.0 * np.pi) * sigma)
```

### Comparing `elphem-0.2.0/elphem/lattice/empty.py` & `elphem-0.3.1/elphem/lattice/reciprocal_cell.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,290 +1,357 @@
 import numpy as np
+import re
 from dataclasses import dataclass
 
-from elphem.lattice.rotation import LatticeRotation
-from elphem.const.brillouin import SpecialPoints
-
-@dataclass
-class LatticeConstant:
-    """Defines the lattice constants and angles for a crystal structure.
+from elphem.lattice.cell import Cell3D, Cell2D, Cell1D
+from elphem.lattice.primitive_cell import PrimitiveCell3D, PrimitiveCell2D, PrimitiveCell1D
+from elphem.lattice.lattice_constant import LatticeConstant3D, LatticeConstant2D, LatticeConstant1D
+from elphem.common.brillouin import SpecialPoints3D, SpecialPoints2D, SpecialPoints1D
+from elphem.lattice.path import PathValues
 
+class ReciprocalCell:
+    """A class for reciprocal cells
     Attributes:
-        a (float): Length of the first lattice vector.
-        b (float): Length of the second lattice vector.
-        c (float): Length of the third lattice vector.
-        alpha (float): Angle between b and c lattice vectors.
-        beta (float): Angle between a and c lattice vectors.
-        gamma (float): Angle between a and b lattice vectors.
-        crystal_structure (str): The type of crystal structure (e.g., 'bcc', 'fcc', 'sc').
+        n_dim (int): Number of dimensions
     """
-    a: float
-    b: float
-    c: float
-    alpha: float
-    beta: float
-    gamma: float
-    crystal_structure: str
+    def __init__(self):
+        self.n_dim = None
     
-    def __post_init__(self):
-        """Converts angles to radians and stores lengths and angles as numpy arrays."""
-        self.length = np.array([self.a, self.b, self.c])
-        self.angle = np.radians(np.array([self.alpha, self.beta, self.gamma]))
-        
-    def rescale(self, factor: float) -> None:
-        """Rescales the lattice constants by a given factor.
+    @staticmethod
+    def split_fractional_k_name(fractional_k_name: str) -> tuple:
+        """Split fractional special k points.
 
         Args:
-            factor (float): The factor by which the lattice lengths are multiplied.
-        """
-        self.length *= factor
+            fractional_k_name (str): A string of fractional special k points
 
-class Cell:
-    """Base class for a crystal cell, providing basic structure and methods."""
-    def __init__(self):
-        """Initializes the Cell with a basis matrix."""
-        self.basis = self.build()
-    
-    def build(self) -> np.ndarray:
-        """Builds the default identity matrix for the cell basis.
+        Raises:
+            ValueError: If the string format is invalid.
 
         Returns:
-            np.ndarray: A 3x3 identity matrix.
+            tuple: fraction and the name of a special k point.
         """
-        return np.identity(3)
-    
-    def volume(self) -> float:
-        """Calculates the volume of the cell.
+        match = re.match(r"([0-9.]*)([A-Z]+)", fractional_k_name)
+        
+        if match:
+            fraction_str = match.group(1)
+            k_name = match.group(2)
 
-        Returns:
-            float: The volume calculated using the determinant of the basis vectors.
-        """
-        volume = np.dot(self.basis[0], np.cross(self.basis[1], self.basis[2]))
-        return volume
-    
-    def element(self, a: np.ndarray) -> np.ndarray:
-        """Transforms a vector a by the basis matrix.
+            number = float(fraction_str) if fraction_str else 1.0
+            
+            return number, k_name
+        else:
+            raise ValueError("Invalid input string format. Ensure the input contains only a combination of numbers and k-names.")
+
+    def get_path(self, fractional_k_names: list[str], n_split: int) -> PathValues:
+        """Calculates a path through specified special points in the Brillouin zone.
 
         Args:
-            a (np.ndarray): The vector to transform.
+            fractional_k_names (list[str]): List of special point names to form the path.
+            n_split (int): Number of points between each special point.
 
         Returns:
-            np.ndarray: The transformed vector.
+            k_path (PathValue): Values with path.
         """
-        x = np.dot(a, self.basis)
-        return x
+        fractional_k_names_tuple = [self.split_fractional_k_name(fractional_k_name) for fractional_k_name in fractional_k_names]
+        
+        k_via = [fractional_k_name[0] * self.calculate_special_k(fractional_k_name[1]) for fractional_k_name in fractional_k_names_tuple]
+        n_via = len(k_via) - 1
 
-    @staticmethod
-    def optimize(basis: np.ndarray) -> np.ndarray:
-        """Optimizes the cell basis using the LatticeRotation utility.
+        major_scales = np.empty((n_via+1,))
+        minor_scales = np.empty((n_via * n_split,))
+        k = np.empty((n_via * n_split, self.n_dim))
+
+        count = 0
+        length_part = 0.0
+        major_scales[0] = 0.0
+
+        for i in range(n_via):
+            direction = k_via[i+1] - k_via[i]
+            length = np.linalg.norm(direction)
+
+            x = np.linspace(0.0, 1.0, n_split)
+            
+            for j in range(n_split):
+                k[count] = k_via[i] + x[j] * direction
+                minor_scales[count] = x[j] * length + length_part
+                count += 1
+            
+            length_part += length
+            major_scales[i+1] = length_part
+
+        k_path = PathValues(major_scales, minor_scales, k)
 
+        return k_path
+    
+    def get_reciprocal_vectors(self, n_g: int) -> np.ndarray:
+        """Generate the reciprocal lattice vectors used to define the Brillouin zone boundaries.
+        
         Args:
-            basis (np.ndarray): The basis matrix to optimize.
+            n_g: Number of reciprocal lattice vectors
 
         Returns:
-            np.ndarray: The optimized basis matrix.
+            np.ndarray: A numpy array of reciprocal lattice vectors.
         """
-        axis = np.array([1.0] * 3)
+        if self.n_dim == 3:
+            n_cut = np.ceil(np.cbrt(n_g))
+        elif self.n_dim == 2:
+            n_cut = np.ceil(np.sqrt(n_g))
+        elif self.n_dim == 1:
+            n_cut = np.ceil(np.abs(n_g))
+        else:
+            raise ValueError("n_cut = 1, 2, 3")
+
+        n_array = np.arange(-n_cut, n_cut + 1)
+
+        grids = np.meshgrid(*([n_array] * self.n_dim), indexing='ij')
         
-        basis = LatticeRotation.optimize(basis, axis)
+        grid_points = np.stack(grids, axis=-1).reshape(-1, self.n_dim)
         
-        return basis
+        g = grid_points @ self.basis
+        g_norm = np.linalg.norm(g, axis=-1).round(decimals=5)
+        g_norm_unique = np.unique(g_norm)
+
+        g_list = []
+
+        for g_ref in g_norm_unique:
+            count = 0
+            degeneracy = 0
+            for g_compare in g_norm:
+                if g_compare == g_ref:
+                    g_list.append(g[count])
+                    degeneracy += 1
+                count += 1
+
+        return np.array(g_list[0:n_g])
+    
+    def calculate_special_k(k_name: str) -> None:
+        pass
 
 @dataclass
-class PrimitiveCell(Cell):
-    """Defines the primitive cell for a crystal based on the lattice constants."""
-    lattice_constant: LatticeConstant
+class ReciprocalCell3D(ReciprocalCell, Cell3D):
+    """Class for the 3D reciprocal cell for a crystal based on the lattice constants of the primitive cell.
+    
+    Attributes:
+        lattice_constant (LatticeConstant3D): Lattice constants.
+        basis (np.ndarray): A numpy array of basis.
+        volume (float): The volume.
+    """
+    lattice_constant: LatticeConstant3D
     
     def __post_init__(self):
-        """Initializes and builds the basis for the primitive cell."""
+        """Initializes and builds the basis for the reciprocal cell."""
+        Cell3D.__init__(self)
         self.basis = self.build()
+        self.volume = self.calculate_volume()
     
     def build(self) -> np.ndarray:
-        """Constructs the basis matrix for the primitive cell from lattice constants and angles.
+        """Constructs the basis matrix for the reciprocal cell from the primitive cell.
 
         Returns:
-            np.ndarray: The basis matrix of the primitive cell.
+            basis (np.ndarray): The basis matrix of the reciprocal cell.
         """
-        length = self.lattice_constant.length
-        angle = self.lattice_constant.angle
+        primitive_cell = PrimitiveCell3D(self.lattice_constant)
 
         basis = np.zeros((3,3))
+        
+        primitive_vector = primitive_cell.basis
+        for i in range(3):
+            j = (i+1) % 3
+            k = (i+2) % 3
+            basis[i] = np.cross(primitive_vector[j], primitive_vector[k])
 
-        basis[0][0] = length[0]
-        basis[1][0] = length[1] * np.cos(angle[2])
-        basis[1][1] = length[1] * np.sin(angle[2])
-
-        basis[2][0] = length[2] * np.cos(angle[1])
-        basis[2][1] = length[2] * (np.cos(angle[0]) - np.cos(angle[1]) * np.cos(angle[2])) / np.sin(angle[2])
-        basis[2][2] = np.sqrt(length[2] ** 2 - np.sum(basis[2]**2))
-
-        basis = self.optimize(basis)
+        basis *= 2.0 * np.pi / primitive_cell.volume
         
         return basis
 
+    def get_monkhorst_pack_grid(self, n_x: int, n_y: int, n_z: int) -> np.ndarray:
+        """Get 3D Monkhorst and Pack grid
+
+        Args:
+            n_x (int): Number of x-direction points
+            n_y (int): Number of y-direction points
+            n_z (int): Number of z-direction points
+
+        Returns:
+            aligned_k (np.ndarray): A numpy array of k points
+        """
+        x = (2 * np.arange(1, n_x + 1) - n_x - 1) / (2 * n_x)
+        y = (2 * np.arange(1, n_y + 1) - n_y - 1) / (2 * n_y)
+        z = (2 * np.arange(1, n_z + 1) - n_z - 1) / (2 * n_z)
+
+        bx = np.broadcast_to(x[:, np.newaxis, np.newaxis], (n_x, n_y, n_z))
+        by = np.broadcast_to(y[np.newaxis, :, np.newaxis], (n_x, n_y, n_z))
+        bz = np.broadcast_to(z[np.newaxis, np.newaxis, :], (n_x, n_y, n_z))
+
+        aligned_k = np.stack([bx, by, bz], axis=-1).reshape(-1, 3) @ self.basis
+
+        return aligned_k
+
+    def calculate_special_k(self, k_name: str) -> np.ndarray:
+        """Retrieves the coordinates of special k-points based on the crystal structure.
+
+        Args:
+            k_name (str): The name of the special point.
+
+        Returns:
+            np.ndarray: The coordinates of the special point.
+
+        Raises:
+            ValueError: If an invalid crystal structure name is provided.
+        """
+        if self.lattice_constant.crystal_structure == 'bcc':
+            special_point = SpecialPoints3D.BCC[k_name]
+        elif self.lattice_constant.crystal_structure == 'fcc':
+            special_point = SpecialPoints3D.FCC[k_name]
+        elif self.lattice_constant.crystal_structure == 'sc':
+            special_point = SpecialPoints3D.SC[k_name]
+        else:
+            raise ValueError("Invalid name specified.")
+        
+        return np.array(special_point) @ self.basis
+
 @dataclass
-class ReciprocalCell(Cell):
-    """Defines the reciprocal cell for a crystal based on the lattice constants of the primitive cell."""
-    lattice_constant: LatticeConstant
+class ReciprocalCell2D(ReciprocalCell, Cell2D):
+    """Class for the 2D reciprocal cell for a crystal based on the lattice constants of the primitive cell.
+    
+    Attributes:
+        lattice_constant (LatticeConstant2D): Lattice constants.
+        basis (np.ndarray): A numpy array of basis.
+        volume (float): The volume.
+    """
+    lattice_constant: LatticeConstant2D
     
     def __post_init__(self):
         """Initializes and builds the basis for the reciprocal cell."""
+        Cell2D.__init__(self)
         self.basis = self.build()
+        self.volume = self.calculate_volume()
     
     def build(self) -> np.ndarray:
         """Constructs the basis matrix for the reciprocal cell from the primitive cell.
 
         Returns:
-            np.ndarray: The basis matrix of the reciprocal cell.
+            basis (np.ndarray): The basis matrix of the reciprocal cell.
         """
-        primitive_cell = PrimitiveCell(self.lattice_constant)
+        primitive_cell = PrimitiveCell2D(self.lattice_constant)
 
-        basis = np.zeros((3,3))
+        basis = np.zeros((2,2))
         
         primitive_vector = primitive_cell.basis
-        for i in range(3):
-            j = (i+1) % 3
-            k = (i+2) % 3
-            basis[i] = np.cross(primitive_vector[j], primitive_vector[k])
 
-        basis *= 2.0 * np.pi / primitive_cell.volume()
+        quarter_rotation_matrix = np.array([
+            [0.0, -1.0],
+            [1.0, 0.0]
+        ])
+        
+        for i in range(2):
+            j = (i+1) % 2
+            rotated_primitive_vector = quarter_rotation_matrix @ primitive_vector[j]
+            basis[i] = rotated_primitive_vector / np.dot(primitive_vector[i], rotated_primitive_vector) * 2.0 * np.pi
         
         return basis
 
-    def path(self, k_names: list[str], n: int) -> np.ndarray:
-        """Calculates a path through specified special points in the Brillouin zone.
+    def get_monkhorst_pack_grid(self, n_x: int, n_y: int) -> np.ndarray:
+        """Get 2D Monkhorst and Pack grid
 
         Args:
-            k_names (list[str]): List of special point names to form the path.
-            n (int): Number of points between each special point.
+            n_x (int): Number of x-direction points
+            n_y (int): Number of y-direction points
 
         Returns:
-            tuple: Returns the total length of the path, the path coordinates, and the lengths at special points.
+            aligned_k (np.ndarray): A numpy array of k points
         """
-        k_via = [self.get_special_k(s) for s in k_names]
 
-        n_via = len(k_via) - 1
+        x = (2 * np.arange(1, n_x + 1) - n_x - 1) / (2 * n_x)
+        y = (2 * np.arange(1, n_y + 1) - n_y - 1) / (2 * n_y)
 
-        total_length = np.empty((n_via * n,))
-        special_length = np.empty((n_via+1,))
-        k = np.empty((n_via * n, 3))
+        bx = np.broadcast_to(x[:, np.newaxis], (n_x, n_y))
+        by = np.broadcast_to(y[np.newaxis, :], (n_x, n_y))
 
-        count = 0
-        length_part = 0.0
-        special_length[0] = 0.0
+        aligned_k = np.stack([bx, by], axis=-1).reshape(-1, 2) @ self.basis
 
-        for i in range(n_via):
-            direction = (np.array(k_via[i+1]) - np.array(k_via[i])) @ self.basis
-            length = np.linalg.norm(direction)
-
-            x = np.linspace(0.0, 1.0, n)
-                        
-            for j in range(n):
-                k[count] = k_via[i] @ self.basis + x[j] * direction
-                total_length[count] = x[j] * length + length_part
-                count += 1
-            
-            length_part += length
-            special_length[i+1] = length_part
+        return aligned_k
 
-        return total_length, k, special_length
-
-    def get_special_k(self, k_name: str) -> np.ndarray:
+    def calculate_special_k(self, k_name: str) -> np.ndarray:
         """Retrieves the coordinates of special k-points based on the crystal structure.
 
         Args:
             k_name (str): The name of the special point.
 
         Returns:
             np.ndarray: The coordinates of the special point.
 
         Raises:
             ValueError: If an invalid crystal structure name is provided.
         """
-        if self.lattice_constant.crystal_structure == 'bcc':
-            return SpecialPoints.BCC[k_name]
-        elif self.lattice_constant.crystal_structure == 'fcc':
-            return SpecialPoints.FCC[k_name]
-        elif self.lattice_constant.crystal_structure == 'sc':
-            return SpecialPoints.SC[k_name]
+        if self.lattice_constant.crystal_structure == 'square':
+            special_point = SpecialPoints2D.Square[k_name]
+        elif self.lattice_constant.crystal_structure == 'hexagonal':
+            special_point = SpecialPoints2D.Hexagonal[k_name]
         else:
             raise ValueError("Invalid name specified.")
+        
+        return np.array(special_point) @ self.basis
 
 @dataclass
-class EmptyLattice:
-    """A class to simulate an empty lattice for a given crystal structure and lattice constant a."""
-    crystal_structure: str
-    a: float
+class ReciprocalCell1D(ReciprocalCell, Cell1D):
+    """Class for the 1D reciprocal cell for a crystal based on the lattice constants of the primitive cell.
+    
+    Attributes:
+        lattice_constant (LatticeConstant1D): Lattice constants.
+        basis (np.ndarray): A numpy array of basis.
+        volume (float): The volume.
+    """
 
+    lattice_constant: LatticeConstant1D
+    
     def __post_init__(self):
-        """Initializes the lattice constants, primitive, and reciprocal cells along with their volumes and bases."""
-        self.constants = self.get_lattice_constant()
-        self.primitive_cell = PrimitiveCell(self.constants)
-        self.reciprocal_cell = ReciprocalCell(self.constants)
-
-        self.volume = {
-            "primitive": self.primitive_cell.volume(),
-            "reciprocal": self.reciprocal_cell.volume()
-        }
-        self.basis = {
-            "primitive": self.primitive_cell.basis,
-            "reciprocal": self.reciprocal_cell.basis
-        }
-
-    def get_lattice_constant(self) -> LatticeConstant:
-        """Determines lattice constants based on the crystal structure.
+        """Initializes and builds the basis for the reciprocal cell."""
+        Cell1D.__init__(self)
+        self.basis = self.build()
+        self.volume = self.calculate_volume()
+    
+    def build(self) -> np.ndarray:
+        """Constructs the basis matrix for the reciprocal cell from the primitive cell.
 
         Returns:
-            LatticeConstant: The lattice constants and angles for the specified crystal structure.
-
-        Raises:
-            ValueError: If an invalid crystal structure name is specified.
+            np.ndarray: The basis matrix of the reciprocal cell.
         """
-        crystal_structure_lower = self.crystal_structure.lower()
-
-        alpha_values = {
-            'bcc': 109.47,
-            'fcc': 60.0,
-            'sc': 90.0
-        }
-
-        alpha = alpha_values.get(crystal_structure_lower)
+        primitive_cell = PrimitiveCell1D(self.lattice_constant)
+        
+        primitive_vector = primitive_cell.basis
 
-        if alpha is not None:
-            return LatticeConstant(self.a, self.a, self.a, alpha, alpha, alpha, crystal_structure_lower)
-        else:
-            raise ValueError("Invalid crystal structure specified.")
+        basis = 2.0 * np.pi / primitive_vector
         
-    def grid(self, *n: list[np.ndarray], space="reciprocal") -> np.ndarray:
-        """Generates a grid in the specified lattice space (either 'primitive' or 'reciprocal').
+        return basis
+
+    def get_monkhorst_pack_grid(self, n_x: int) -> np.ndarray:
+        """Get 1D Monkhorst and Pack grid
 
         Args:
-            n (list[np.ndarray]): List of points defining the grid dimensions.
-            space (str): Specifies whether the grid is in the primitive or reciprocal space.
+            n_x (int): Number of x-direction points
 
         Returns:
-            np.ndarray: A grid generated based on the specified dimensions and space.
+            aligned_k (np.ndarray): A numpy array of k points
         """
-        basis = self.basis[space]
+
+        x = (2 * np.arange(1, n_x + 1) - n_x - 1) / (2 * n_x)
+
+        aligned_k = np.stack([x], axis=-1).reshape(-1, 1) @ self.basis
         
-        n_array = np.array(n)
-        n_point = len(n_array)
-        n_array = n_array.reshape(n_array.size,)
+        return aligned_k
 
-        grid = np.meshgrid(*[np.arange(-i, i) for i in n_array])
-        grid = np.array(grid)
+    def calculate_special_k(self, k_name: str) -> np.ndarray:
+        """Retrieves the coordinates of special k-points based on the crystal structure.
 
-        grid_set = []
-        j = 0
-        for i in range(n_point):
-            x = grid[j:j+3]
-            y = np.empty(x[0].shape + (3,))
-            for k in range(3):
-                y[...,k] = x[k]
+        Args:
+            k_name (str): The name of the special point.
 
-            grid_set.append(y @ basis)
-            j += 3
+        Returns:
+            np.ndarray: The coordinates of the special point.
 
-        if len(grid_set) == 1:
-            return grid_set[0]
-        else:
-            return tuple(grid_set)
+        Raises:
+            ValueError: If an invalid crystal structure name is provided.
+        """
+        special_point = SpecialPoints1D.Line[k_name]
+        
+        return special_point * self.basis
```

### Comparing `elphem-0.2.0/elphem/lattice/rotation.py` & `elphem-0.3.1/elphem/lattice/rotation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,62 @@
 import numpy as np
 from scipy.spatial.transform import Rotation
 
 class LatticeRotation:
-    """Provides methods to optimize and adjust lattice orientations through rotation operations."""
+    @staticmethod
+    def normalize(v: np.ndarray) -> np.ndarray:
+        """Normalize the given vector.
+
+        Args:
+            v (np.ndarray): The vector to normalize.
+
+        Returns:
+            np.ndarray: The normalized vector.
+
+        Raises:
+            ValueError: If the input vector is zero.
+        """
+        v_norm = np.linalg.norm(v)
+
+        if v_norm == 0.0:
+            return v
+
+        return v / v_norm
+
+class LatticeRotation3D(LatticeRotation):
+    """Provides methods to optimize and adjust 3D lattice orientations through rotation operations."""
     
     @classmethod
-    def optimize(cls, basis: np.ndarray, axis: np.ndarray) -> np.ndarray:
+    def calculate_optimized_basis(cls, basis: np.ndarray, axis: np.ndarray) -> np.ndarray:
         """Optimize the rotation of the given basis to align with the specified axis.
 
         Args:
             basis (np.ndarray): The basis vectors of the lattice to be rotated.
             axis (np.ndarray): The target axis for alignment.
 
         Returns:
             np.ndarray: The optimized basis vectors aligned as closely as possible to the target axis.
 
         Raises:
             ValueError: If the axis vector is zero.
         """
-        basis_rotated = cls.match(basis, axis)
-        basis_rotated = cls.search_posture(basis_rotated, axis)
+        basis_rotated = cls.search_optimized_direction(basis, axis)
+        basis_rotated = cls.search_optimized_posture(basis_rotated, axis)
         return basis_rotated
 
     @classmethod
-    def match(cls, basis: np.ndarray, axis: np.ndarray) -> np.ndarray:
-        """Match the given basis direction to the specified axis using quaternion rotation.
+    def search_optimized_direction(cls, basis: np.ndarray, axis: np.ndarray) -> np.ndarray:
+        """search_optimized_direction the given basis direction to the specified axis using quaternion rotation.
 
         Args:
             basis (np.ndarray): The initial basis vectors.
             axis (np.ndarray): The axis to align the basis vectors to.
 
         Returns:
-            np.ndarray: The basis vectors rotated to match the direction of the axis.
+            np.ndarray: The basis vectors rotated to search_optimized_direction the direction of the axis.
 
         Raises:
             ValueError: If the axis vector is zero.
         """
         if np.linalg.norm(axis) == 0.0:
             raise ValueError("Axis vector should not be zero.")
         
@@ -56,15 +77,15 @@
 
         rotation = Rotation.from_quat(quaternion)
         basis_rotated = rotation.apply(basis)
         
         return basis_rotated
 
     @classmethod
-    def around_axis(cls, axis: np.ndarray, v: np.ndarray, theta: float) -> np.ndarray:
+    def rotate_vector_around_axis(cls, axis: np.ndarray, v: np.ndarray, theta: float) -> np.ndarray:
         """Rotate vector v around the given axis by angle theta.
 
         Args:
             axis (np.ndarray): The axis of rotation.
             v (np.ndarray): The vector to rotate.
             theta (float): The angle in radians to rotate the vector.
 
@@ -82,15 +103,15 @@
         v_rotated = cos_theta * v
         v_rotated += np.sin(theta) * np.cross(axis, v)
         v_rotated += (1.0 - cos_theta) * axis_dot_v * axis
 
         return v_rotated
 
     @classmethod
-    def search_posture(cls, basis: np.ndarray, axis: np.ndarray, angle_max: float = 360.0) -> np.ndarray:
+    def search_optimized_posture(cls, basis: np.ndarray, axis: np.ndarray, angle_max: float = 360.0) -> np.ndarray:
         """Search for the best posture of the basis aligned with the given axis.
 
         Args:
             basis (np.ndarray): The basis to be rotated.
             axis (np.ndarray): The axis to align with.
             angle_max (float): The maximum angle range to search in degrees.
 
@@ -108,41 +129,77 @@
         basis_searched = basis
         
         n = np.zeros(basis.shape)
         u = np.identity(3)
                     
         axis_normalized = cls.normalize(axis)
         for theta in angle:
-            basis_rotated = cls.around_axis(axis_normalized, basis, theta)
+            basis_rotated = cls.rotate_vector_around_axis(axis_normalized, basis, theta)
             
             s = 0.0
             for i in range(3):
                 j = i
                 k = (i+1) % 3
                 n[i] = np.cross(basis_rotated[j], basis_rotated[k])
                 s += np.dot(n[i], u[i])
             
             if s < s_min:
                 s_min = s
                 basis_searched = basis_rotated
 
         return basis_searched
 
-    @staticmethod
-    def normalize(v: np.ndarray) -> np.ndarray:
-        """Normalize the given vector.
+class LatticeRotation2D(LatticeRotation):
+    """Provides methods to optimize and adjust 2D lattice orientations through rotation operations."""
+    
+    @classmethod
+    def calculate_optimized_basis(cls, basis: np.ndarray, axis: np.ndarray) -> np.ndarray:
+        """Optimize the rotation of the given basis to align with the specified axis.
 
         Args:
-            v (np.ndarray): The vector to normalize.
+            basis (np.ndarray): The basis vectors of the lattice to be rotated.
+            axis (np.ndarray): The target axis for alignment.
 
         Returns:
-            np.ndarray: The normalized vector.
+            np.ndarray: The optimized basis vectors aligned as closely as possible to the target axis.
 
         Raises:
-            ValueError: If the input vector is zero.
+            ValueError: If the axis vector is zero.
         """
-        v_norm = np.linalg.norm(v)
+        basis_rotated = cls.search_optimized_direction(basis, axis)
+        return basis_rotated
 
-        if v_norm == 0.0:
-            return v
+    @classmethod
+    def search_optimized_direction(cls, basis: np.ndarray, axis: np.ndarray) -> np.ndarray:
+        """search_optimized_direction the given basis direction to the specified axis using quaternion rotation.
+
+        Args:
+            basis (np.ndarray): The initial basis vectors.
+            axis (np.ndarray): The axis to align the basis vectors to.
+
+        Returns:
+            np.ndarray: The basis vectors rotated to search_optimized_direction the direction of the axis.
+
+        Raises:
+            ValueError: If the axis vector is zero.
+        """
+        if np.linalg.norm(axis) == 0.0:
+            raise ValueError("Axis vector should not be zero.")
+        
+        direction = cls.normalize(basis[0] + basis[1])
+        n = cls.normalize(axis)
+
+        dot = np.dot(direction, n)
 
-        return v / v_norm
+        theta = np.arccos(dot)
+        
+        sin_theta = np.sin(theta)
+        cos_theta = np.cos(theta)
+        
+        rotation_matrix = np.array([
+            [cos_theta, -sin_theta],
+            [sin_theta, cos_theta]
+        ])
+
+        basis_rotated = basis @ rotation_matrix
+        
+        return basis_rotated
```

### Comparing `elphem-0.2.0/elphem.egg-info/SOURCES.txt` & `elphem-0.3.1/elphem.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -3,38 +3,42 @@
 setup.py
 elphem/__init__.py
 elphem.egg-info/PKG-INFO
 elphem.egg-info/SOURCES.txt
 elphem.egg-info/dependency_links.txt
 elphem.egg-info/requires.txt
 elphem.egg-info/top_level.txt
-elphem/const/__init__.py
-elphem/const/atomic_weight.py
-elphem/const/brillouin.py
-elphem/const/unit.py
+elphem/common/__init__.py
+elphem/common/atomic_weight.py
+elphem/common/brillouin.py
+elphem/common/distribution.py
+elphem/common/function.py
+elphem/common/stdout.py
+elphem/common/unit.py
 elphem/electron/__init__.py
-elphem/electron/free.py
+elphem/electron/electron.py
 elphem/elph/__init__.py
-elphem/elph/distribution.py
-elphem/elph/epr.py
-elphem/elph/self_energy.py
-elphem/elph/spectrum.py
+elphem/elph/electron_phonon.py
+elphem/elph/green_function.py
 elphem/lattice/__init__.py
-elphem/lattice/empty.py
+elphem/lattice/cell.py
+elphem/lattice/lattice.py
+elphem/lattice/lattice_constant.py
+elphem/lattice/path.py
+elphem/lattice/primitive_cell.py
+elphem/lattice/reciprocal_cell.py
 elphem/lattice/rotation.py
 elphem/phonon/__init__.py
-elphem/phonon/debye.py
+elphem/phonon/phonon.py
 tests/__init__.py
-tests/const/__init__.py
-tests/const/test_atomic_weight.py
-tests/const/test_brillouin.py
-tests/const/test_unit.py
+tests/common/__init__.py
+tests/common/test_atomic_weight.py
+tests/common/test_brillouin.py
+tests/common/test_unit.py
 tests/electron/__init__.py
-tests/electron/test_free.py
+tests/electron/test_electron.py
 tests/elph/__init__.py
-tests/elph/test_epr.py
 tests/elph/test_self_energy.py
-tests/elph/test_spectrum.py
 tests/lattice/__init__.py
-tests/lattice/test_empty_lattice.py
+tests/lattice/test_lattice.py
 tests/phonon/__init__.py
-tests/phonon/test_debye.py
+tests/phonon/test_phonon.py
```

### Comparing `elphem-0.2.0/setup.py` & `elphem-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 DESCRIPTION = 'Elphem: Calculating electron-phonon interactions with the empty lattice.'
 NAME = 'elphem'
 AUTHOR = 'Kohei Ishii'
 AUTHOR_EMAIL = ''
 URL = 'https://github.com/cohsh/elphem'
 LICENSE = 'MIT'
 DOWNLOAD_URL = URL
-VERSION = '0.2.0'
+VERSION = '0.3.1'
 PYTHON_REQUIRES = '>=3.10'
 INSTALL_REQUIRES = ['numpy', 'scipy']
 
 CLASSIFIERS=[
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3.10',
```

### Comparing `elphem-0.2.0/tests/const/test_unit.py` & `elphem-0.3.1/tests/common/test_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from unittest import TestCase
-from elphem.const.unit import *
+from elphem.common.unit import *
 
 class TestUnit(TestCase):
     def test_byte(self):
         size = Byte.get_str(2**30)
         self.assertEqual(size, "1.0 GB")
     
     def test_length(self):
```

