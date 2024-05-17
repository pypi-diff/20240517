# Comparing `tmp/pdme-1.3.0.tar.gz` & `tmp/pdme-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdme-1.3.0.tar", max compression
+gzip compressed data, was "pdme-1.4.0.tar", max compression
```

## Comparing `pdme-1.3.0.tar` & `pdme-1.4.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1229 2024-05-17 00:23:46.157294 pdme-1.3.0/README.md
--rw-r--r--   0        0        0      154 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/__init__.py
--rw-r--r--   0        0        0     1578 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/calculations/__init__.py
--rw-r--r--   0        0        0     1939 2024-05-17 00:24:12.778603 pdme-1.3.0/pdme/calculations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      184 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/inputs/__init__.py
--rw-r--r--   0        0        0      315 2024-05-17 00:24:13.050617 pdme-1.3.0/pdme/inputs/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1471 2024-05-17 00:24:13.050617 pdme-1.3.0/pdme/inputs/__pycache__/dot_inputs.cpython-39.pyc
--rw-r--r--   0        0        0      688 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/inputs/dot_inputs.py
--rw-r--r--   0        0        0      536 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/measurement/__init__.py
--rw-r--r--   0        0        0      642 2024-05-17 00:24:13.086618 pdme-1.3.0/pdme/measurement/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1642 2024-05-17 00:24:13.090618 pdme-1.3.0/pdme/measurement/__pycache__/dot_measure.cpython-39.pyc
--rw-r--r--   0        0        0     1864 2024-05-17 00:24:13.090618 pdme-1.3.0/pdme/measurement/__pycache__/dot_pair_measure.cpython-39.pyc
--rw-r--r--   0        0        0     1818 2024-05-17 00:24:13.098619 pdme-1.3.0/pdme/measurement/__pycache__/input_types.cpython-39.pyc
--rw-r--r--   0        0        0     9719 2024-05-17 00:24:13.094619 pdme-1.3.0/pdme/measurement/__pycache__/oscillating_dipole.cpython-39.pyc
--rw-r--r--   0        0        0      984 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/measurement/dot_measure.py
--rw-r--r--   0        0        0     1224 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/measurement/dot_pair_measure.py
--rw-r--r--   0        0        0     1131 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/measurement/input_types.py
--rw-r--r--   0        0        0     6903 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/measurement/oscillating_dipole.py
--rw-r--r--   0        0        0       70 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/meta.py
--rw-r--r--   0        0        0     1066 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/model/__init__.py
--rw-r--r--   0        0        0      988 2024-05-17 00:24:13.126620 pdme-1.3.0/pdme/model/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2740 2024-05-17 00:24:13.142621 pdme-1.3.0/pdme/model/__pycache__/fixed_magnitude_model.cpython-39.pyc
--rw-r--r--   0        0        0     5039 2024-05-17 00:24:13.162622 pdme-1.3.0/pdme/model/__pycache__/log_spaced_random_choice_fixed_orientation_model.cpython-39.pyc
--rw-r--r--   0        0        0     5083 2024-05-17 00:24:13.154622 pdme-1.3.0/pdme/model/__pycache__/log_spaced_random_choice_model.cpython-39.pyc
--rw-r--r--   0        0        0     4757 2024-05-17 00:24:13.158622 pdme-1.3.0/pdme/model/__pycache__/log_spaced_random_choice_xy_model.cpython-39.pyc
--rw-r--r--   0        0        0     3850 2024-05-17 00:24:13.130621 pdme-1.3.0/pdme/model/__pycache__/model.cpython-39.pyc
--rw-r--r--   0        0        0     2928 2024-05-17 00:24:13.146621 pdme-1.3.0/pdme/model/__pycache__/multidipole_fixed_magnitude_model.cpython-39.pyc
--rw-r--r--   0        0        0     3362 2024-05-17 00:24:13.150622 pdme-1.3.0/pdme/model/__pycache__/random_count_multidipole_fixed_magnitude_model.cpython-39.pyc
--rw-r--r--   0        0        0     2367 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/model/fixed_magnitude_model.py
--rw-r--r--   0        0        0     5158 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/model/log_spaced_random_choice_fixed_orientation_model.py
--rw-r--r--   0        0        0     5332 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/model/log_spaced_random_choice_model.py
--rw-r--r--   0        0        0     4699 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/model/log_spaced_random_choice_xy_model.py
--rw-r--r--   0        0        0     3594 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/model/model.py
--rw-r--r--   0        0        0     2560 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/model/multidipole_fixed_magnitude_model.py
--rw-r--r--   0        0        0     3076 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/model/random_count_multidipole_fixed_magnitude_model.py
--rw-r--r--   0        0        0        0 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/py.typed
--rw-r--r--   0        0        0     1875 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/subspace_simulation/__init__.py
--rw-r--r--   0        0        0     2807 2024-05-17 00:24:13.130621 pdme-1.3.0/pdme/subspace_simulation/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      842 2024-05-17 00:24:13.134621 pdme-1.3.0/pdme/subspace_simulation/__pycache__/mcmc_costs.cpython-39.pyc
--rw-r--r--   0        0        0      575 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/subspace_simulation/mcmc_costs.py
--rw-r--r--   0        0        0        0 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/util/__init__.py
--rw-r--r--   0        0        0      167 2024-05-17 00:24:13.134621 pdme-1.3.0/pdme/util/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4170 2024-05-17 00:24:13.414635 pdme-1.3.0/pdme/util/__pycache__/fast_nonlocal_spectrum.cpython-39.pyc
--rw-r--r--   0        0        0     5553 2024-05-17 00:24:13.138621 pdme-1.3.0/pdme/util/__pycache__/fast_v_calc.cpython-39.pyc
--rw-r--r--   0        0        0     9670 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/util/fast_nonlocal_spectrum.py
--rw-r--r--   0        0        0     7195 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/util/fast_v_calc.py
--rw-r--r--   0        0        0      965 2024-05-17 00:23:46.161294 pdme-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 pdme-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1229 2024-05-17 02:07:59.842429 pdme-1.4.0/README.md
+-rw-r--r--   0        0        0      154 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/__init__.py
+-rw-r--r--   0        0        0     1578 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/calculations/__init__.py
+-rw-r--r--   0        0        0     1939 2024-05-17 02:08:28.811901 pdme-1.4.0/pdme/calculations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      184 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/inputs/__init__.py
+-rw-r--r--   0        0        0      315 2024-05-17 02:08:29.323927 pdme-1.4.0/pdme/inputs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1471 2024-05-17 02:08:29.323927 pdme-1.4.0/pdme/inputs/__pycache__/dot_inputs.cpython-39.pyc
+-rw-r--r--   0        0        0      688 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/inputs/dot_inputs.py
+-rw-r--r--   0        0        0      536 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/measurement/__init__.py
+-rw-r--r--   0        0        0      642 2024-05-17 02:08:29.371930 pdme-1.4.0/pdme/measurement/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1642 2024-05-17 02:08:29.371930 pdme-1.4.0/pdme/measurement/__pycache__/dot_measure.cpython-39.pyc
+-rw-r--r--   0        0        0     1864 2024-05-17 02:08:29.375930 pdme-1.4.0/pdme/measurement/__pycache__/dot_pair_measure.cpython-39.pyc
+-rw-r--r--   0        0        0     1818 2024-05-17 02:08:29.379930 pdme-1.4.0/pdme/measurement/__pycache__/input_types.cpython-39.pyc
+-rw-r--r--   0        0        0     9719 2024-05-17 02:08:29.379930 pdme-1.4.0/pdme/measurement/__pycache__/oscillating_dipole.cpython-39.pyc
+-rw-r--r--   0        0        0      984 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/measurement/dot_measure.py
+-rw-r--r--   0        0        0     1224 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/measurement/dot_pair_measure.py
+-rw-r--r--   0        0        0     1131 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/measurement/input_types.py
+-rw-r--r--   0        0        0     6903 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/measurement/oscillating_dipole.py
+-rw-r--r--   0        0        0       70 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/meta.py
+-rw-r--r--   0        0        0     1066 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/model/__init__.py
+-rw-r--r--   0        0        0      988 2024-05-17 02:08:29.407931 pdme-1.4.0/pdme/model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2740 2024-05-17 02:08:29.415932 pdme-1.4.0/pdme/model/__pycache__/fixed_magnitude_model.cpython-39.pyc
+-rw-r--r--   0        0        0     5039 2024-05-17 02:08:29.431933 pdme-1.4.0/pdme/model/__pycache__/log_spaced_random_choice_fixed_orientation_model.cpython-39.pyc
+-rw-r--r--   0        0        0     5083 2024-05-17 02:08:29.423932 pdme-1.4.0/pdme/model/__pycache__/log_spaced_random_choice_model.cpython-39.pyc
+-rw-r--r--   0        0        0     4757 2024-05-17 02:08:29.427932 pdme-1.4.0/pdme/model/__pycache__/log_spaced_random_choice_xy_model.cpython-39.pyc
+-rw-r--r--   0        0        0     3850 2024-05-17 02:08:29.407931 pdme-1.4.0/pdme/model/__pycache__/model.cpython-39.pyc
+-rw-r--r--   0        0        0     2928 2024-05-17 02:08:29.419932 pdme-1.4.0/pdme/model/__pycache__/multidipole_fixed_magnitude_model.cpython-39.pyc
+-rw-r--r--   0        0        0     3362 2024-05-17 02:08:29.419932 pdme-1.4.0/pdme/model/__pycache__/random_count_multidipole_fixed_magnitude_model.cpython-39.pyc
+-rw-r--r--   0        0        0     2367 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/model/fixed_magnitude_model.py
+-rw-r--r--   0        0        0     5158 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/model/log_spaced_random_choice_fixed_orientation_model.py
+-rw-r--r--   0        0        0     5332 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/model/log_spaced_random_choice_model.py
+-rw-r--r--   0        0        0     4699 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/model/log_spaced_random_choice_xy_model.py
+-rw-r--r--   0        0        0     3594 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/model/model.py
+-rw-r--r--   0        0        0     2560 2024-05-17 02:07:59.842429 pdme-1.4.0/pdme/model/multidipole_fixed_magnitude_model.py
+-rw-r--r--   0        0        0     3076 2024-05-17 02:07:59.846429 pdme-1.4.0/pdme/model/random_count_multidipole_fixed_magnitude_model.py
+-rw-r--r--   0        0        0        0 2024-05-17 02:07:59.846429 pdme-1.4.0/pdme/py.typed
+-rw-r--r--   0        0        0     1875 2024-05-17 02:07:59.846429 pdme-1.4.0/pdme/subspace_simulation/__init__.py
+-rw-r--r--   0        0        0     2807 2024-05-17 02:08:29.407931 pdme-1.4.0/pdme/subspace_simulation/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1062 2024-05-17 02:08:29.411932 pdme-1.4.0/pdme/subspace_simulation/__pycache__/mcmc_costs.cpython-39.pyc
+-rw-r--r--   0        0        0      885 2024-05-17 02:07:59.846429 pdme-1.4.0/pdme/subspace_simulation/mcmc_costs.py
+-rw-r--r--   0        0        0        0 2024-05-17 02:07:59.846429 pdme-1.4.0/pdme/util/__init__.py
+-rw-r--r--   0        0        0      167 2024-05-17 02:08:29.411932 pdme-1.4.0/pdme/util/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4170 2024-05-17 02:08:29.671945 pdme-1.4.0/pdme/util/__pycache__/fast_nonlocal_spectrum.cpython-39.pyc
+-rw-r--r--   0        0        0     5553 2024-05-17 02:08:29.415932 pdme-1.4.0/pdme/util/__pycache__/fast_v_calc.cpython-39.pyc
+-rw-r--r--   0        0        0     9670 2024-05-17 02:07:59.846429 pdme-1.4.0/pdme/util/fast_nonlocal_spectrum.py
+-rw-r--r--   0        0        0     7195 2024-05-17 02:07:59.846429 pdme-1.4.0/pdme/util/fast_v_calc.py
+-rw-r--r--   0        0        0      965 2024-05-17 02:07:59.846429 pdme-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 pdme-1.4.0/PKG-INFO
```

### Comparing `pdme-1.3.0/README.md` & `pdme-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/calculations/__init__.py` & `pdme-1.4.0/pdme/calculations/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/calculations/__pycache__/__init__.cpython-39.pyc` & `pdme-1.4.0/pdme/calculations/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 1578 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 2a06 0000  a.........Ff*...
+00000000: 610d 0d0a 0000 0000 ffbb 4666 2a06 0000  a.........Ff*...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 5a00 6401 6402 6c01 5a01 6502 6502 6502  Z.d.d.l.Z.e.e.e.
 00000040: 6403 9c03 6404 6405 8404 5a03 6501 6a04  d...d.d...Z.e.j.
 00000050: 6501 6a04 6501 6a04 6502 6406 9c04 6407  e.j.e.j.e.d...d.
 00000060: 6408 8404 5a05 6501 6a04 6501 6a04 6501  d...Z.e.j.e.j.e.
 00000070: 6a04 6501 6a04 6406 9c04 6409 640a 8404  j.e.j.d...d.d...
@@ -57,15 +57,15 @@
 00000380: 206f 7220 6a75 7374 2063 6861 6e67 6520   or just change 
 00000390: 6974 2074 6865 6e2e 0a09 e902 0000 0029  it then........)
 000003a0: 02da 056e 756d 7079 da02 7069 2902 7202  ...numpy..pi).r.
 000003b0: 0000 0072 0300 0000 a900 7208 0000 00fa  ...r......r.....
 000003c0: 542f 686f 6d65 2f6a 656e 6b69 6e73 2f61  T/home/jenkins/a
 000003d0: 6765 6e74 2f77 6f72 6b73 7061 6365 2f67  gent/workspace/g
 000003e0: 6974 6561 2d70 6879 7369 6373 5f70 646d  itea-physics_pdm
-000003f0: 655f 312e 332e 302f 7064 6d65 2f63 616c  e_1.3.0/pdme/cal
+000003f0: 655f 312e 342e 302f 7064 6d65 2f63 616c  e_1.4.0/pdme/cal
 00000400: 6375 6c61 7469 6f6e 732f 5f5f 696e 6974  culations/__init
 00000410: 5f5f 2e70 79da 0e74 656c 6567 7261 7068  __.py..telegraph
 00000420: 5f62 6574 6108 0000 0073 0200 0000 000a  _beta....s......
 00000430: 720a 0000 0029 04da 0170 da01 73da 0172  r....)...p..s..r
 00000440: 7204 0000 0063 0300 0000 0000 0000 0000  r....c..........
 00000450: 0000 0400 0000 0400 0000 4300 0000 7326  ..........C...s&
 00000460: 0000 007c 027c 0118 007d 037c 00a0 007c  ...|.|...}.|...|
```

### Comparing `pdme-1.3.0/pdme/inputs/__pycache__/dot_inputs.cpython-39.pyc` & `pdme-1.4.0/pdme/inputs/__pycache__/dot_inputs.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 688 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 b002 0000  a.........Ff....
+00000000: 610d 0d0a 0000 0000 ffbb 4666 b002 0000  a.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6504 6500 6a03 6a06 1900  m.Z...e.e.j.j...
 00000060: 6504 6507 1900 6504 6505 6500 6a03 6a06  e.e...e.e.e.j.j.
 00000070: 6507 6602 1900 1900 6403 9c03 6404 6405  e.f.....d...d.d.
@@ -25,15 +25,15 @@
 00000180: 0200 0000 0400 0000 1300 0000 7314 0000  ............s...
 00000190: 0067 007c 005d 0c7d 0188 007c 0166 0291  .g.|.].}...|.f..
 000001a0: 0271 0453 00a9 0072 0700 0000 a902 da02  .q.S...r........
 000001b0: 2e30 da01 66a9 01da 0364 6f74 7207 0000  .0..f....dotr...
 000001c0: 00fa 502f 686f 6d65 2f6a 656e 6b69 6e73  ..P/home/jenkins
 000001d0: 2f61 6765 6e74 2f77 6f72 6b73 7061 6365  /agent/workspace
 000001e0: 2f67 6974 6561 2d70 6879 7369 6373 5f70  /gitea-physics_p
-000001f0: 646d 655f 312e 332e 302f 7064 6d65 2f69  dme_1.3.0/pdme/i
+000001f0: 646d 655f 312e 342e 302f 7064 6d65 2f69  dme_1.4.0/pdme/i
 00000200: 6e70 7574 732f 646f 745f 696e 7075 7473  nputs/dot_inputs
 00000210: 2e70 79da 0a3c 6c69 7374 636f 6d70 3e0a  .py..<listcomp>.
 00000220: 0000 00f3 0000 0000 7a3a 696e 7075 7473  ........z:inputs
 00000230: 5f77 6974 685f 6672 6571 7565 6e63 795f  _with_frequency_
 00000240: 7261 6e67 652e 3c6c 6f63 616c 733e 2e3c  range.<locals>.<
 00000250: 6c69 7374 636f 6d70 3e2e 3c6c 6973 7463  listcomp>.<listc
 00000260: 6f6d 703e 7207 0000 00a9 0172 0900 0000  omp>r......r....
```

### Comparing `pdme-1.3.0/pdme/inputs/dot_inputs.py` & `pdme-1.4.0/pdme/inputs/dot_inputs.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/measurement/__init__.py` & `pdme-1.4.0/pdme/measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/measurement/__pycache__/__init__.cpython-39.pyc` & `pdme-1.4.0/pdme/measurement/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 536 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 1802 0000  a.........Ff....
+00000000: 610d 0d0a 0000 0000 ffbb 4666 1802 0000  a.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 6d08 5a08 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 6d0b 5a0b 0100 6700  d.l.m.Z.m.Z...g.
 00000070: 6405 a201 5a0c 6406 5300 2907 e900 0000  d...Z.d.S.).....
@@ -30,12 +30,12 @@
 000001d0: 7207 0000 005a 1c70 646d 652e 6d65 6173  r....Z.pdme.meas
 000001e0: 7572 656d 656e 742e 696e 7075 745f 7479  urement.input_ty
 000001f0: 7065 7372 0800 0000 7209 0000 00da 075f  pesr....r......_
 00000200: 5f61 6c6c 5f5f a900 720b 0000 0072 0b00  _all__..r....r..
 00000210: 0000 fa53 2f68 6f6d 652f 6a65 6e6b 696e  ...S/home/jenkin
 00000220: 732f 6167 656e 742f 776f 726b 7370 6163  s/agent/workspac
 00000230: 652f 6769 7465 612d 7068 7973 6963 735f  e/gitea-physics_
-00000240: 7064 6d65 5f31 2e33 2e30 2f70 646d 652f  pdme_1.3.0/pdme/
+00000240: 7064 6d65 5f31 2e34 2e30 2f70 646d 652f  pdme_1.4.0/pdme/
 00000250: 6d65 6173 7572 656d 656e 742f 5f5f 696e  measurement/__in
 00000260: 6974 5f5f 2e70 79da 083c 6d6f 6475 6c65  it__.py..<module
 00000270: 3e01 0000 0073 0800 0000 1001 1004 1004  >....s..........
 00000280: 1003                                     ..
```

### Comparing `pdme-1.3.0/pdme/measurement/__pycache__/dot_measure.cpython-39.pyc` & `pdme-1.4.0/pdme/measurement/__pycache__/dot_measure.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 984 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 d803 0000  a.........Ff....
+00000000: 610d 0d0a 0000 0000 ffbb 4666 d803 0000  a.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a02 6501 4700 6403  Z.d.d.l.Z.e.G.d.
 00000050: 6404 8400 6404 8302 8301 5a04 6501 4700  d...d.....Z.e.G.
 00000060: 6405 6406 8400 6406 8302 8301 5a05 6402  d.d...d.....Z.d.
 00000070: 5300 2907 e900 0000 0029 01da 0964 6174  S.)......)...dat
@@ -32,15 +32,15 @@
 000001f0: 0000 4300 0000 7312 0000 0074 00a0 017c  ..C...s....t...|
 00000200: 006a 02a1 017c 005f 0264 0053 00a9 014e  .j...|._.d.S...N
 00000210: 2903 da05 6e75 6d70 79da 0561 7272 6179  )...numpy..array
 00000220: 7205 0000 00a9 01da 0473 656c 66a9 0072  r........self..r
 00000230: 0e00 0000 fa56 2f68 6f6d 652f 6a65 6e6b  .....V/home/jenk
 00000240: 696e 732f 6167 656e 742f 776f 726b 7370  ins/agent/worksp
 00000250: 6163 652f 6769 7465 612d 7068 7973 6963  ace/gitea-physic
-00000260: 735f 7064 6d65 5f31 2e33 2e30 2f70 646d  s_pdme_1.3.0/pdm
+00000260: 735f 7064 6d65 5f31 2e34 2e30 2f70 646d  s_pdme_1.4.0/pdm
 00000270: 652f 6d65 6173 7572 656d 656e 742f 646f  e/measurement/do
 00000280: 745f 6d65 6173 7572 652e 7079 da0d 5f5f  t_measure.py..__
 00000290: 706f 7374 5f69 6e69 745f 5f1b 0000 0073  post_init__....s
 000002a0: 0200 0000 0001 7a1c 446f 744d 6561 7375  ......z.DotMeasu
 000002b0: 7265 6d65 6e74 2e5f 5f70 6f73 745f 696e  rement.__post_in
 000002c0: 6974 5f5f a909 da08 5f5f 6e61 6d65 5f5f  it__....__name__
 000002d0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
```

### Comparing `pdme-1.3.0/pdme/measurement/__pycache__/dot_pair_measure.cpython-39.pyc` & `pdme-1.4.0/pdme/measurement/__pycache__/dot_pair_measure.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 1224 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 c804 0000  a.........Ff....
+00000000: 610d 0d0a 0000 0000 ffbb 4666 c804 0000  a.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a02 6501 4700 6403  Z.d.d.l.Z.e.G.d.
 00000050: 6404 8400 6404 8302 8301 5a04 6501 4700  d...d.....Z.e.G.
 00000060: 6405 6406 8400 6406 8302 8301 5a05 6402  d.d...d.....Z.d.
 00000070: 5300 2907 e900 0000 0029 01da 0964 6174  S.)......)...dat
@@ -38,15 +38,15 @@
 00000250: a001 7c00 6a02 a101 7c00 5f02 7400 a001  ..|.j...|._.t...
 00000260: 7c00 6a03 a101 7c00 5f03 6400 5300 a901  |.j...|._.d.S...
 00000270: 4e29 04da 056e 756d 7079 da05 6172 7261  N)...numpy..arra
 00000280: 7972 0500 0000 7206 0000 00a9 01da 0473  yr....r........s
 00000290: 656c 66a9 0072 0f00 0000 fa5b 2f68 6f6d  elf..r.....[/hom
 000002a0: 652f 6a65 6e6b 696e 732f 6167 656e 742f  e/jenkins/agent/
 000002b0: 776f 726b 7370 6163 652f 6769 7465 612d  workspace/gitea-
-000002c0: 7068 7973 6963 735f 7064 6d65 5f31 2e33  physics_pdme_1.3
+000002c0: 7068 7973 6963 735f 7064 6d65 5f31 2e34  physics_pdme_1.4
 000002d0: 2e30 2f70 646d 652f 6d65 6173 7572 656d  .0/pdme/measurem
 000002e0: 656e 742f 646f 745f 7061 6972 5f6d 6561  ent/dot_pair_mea
 000002f0: 7375 7265 2e70 79da 0d5f 5f70 6f73 745f  sure.py..__post_
 00000300: 696e 6974 5f5f 1f00 0000 7304 0000 0000  init__....s.....
 00000310: 010e 017a 2044 6f74 5061 6972 4d65 6173  ...z DotPairMeas
 00000320: 7572 656d 656e 742e 5f5f 706f 7374 5f69  urement.__post_i
 00000330: 6e69 745f 5fa9 09da 085f 5f6e 616d 655f  nit__....__name_
```

### Comparing `pdme-1.3.0/pdme/measurement/__pycache__/input_types.cpython-39.pyc` & `pdme-1.4.0/pdme/measurement/__pycache__/input_types.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 1131 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 6b04 0000  a.........Ffk...
+00000000: 610d 0d0a 0000 0000 ffbb 4666 6b04 0000  a.........Ffk...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6400 6403 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6400 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6503 6501 6a02 6a0a 650b 6602 1900  ..e.e.j.j.e.f...
 00000070: 5a0c 6503 6501 6a02 6a0a 6501 6a02 6a0a  Z.e.e.j.j.e.j.j.
@@ -29,15 +29,15 @@
 000001c0: 0291 0271 0453 0029 0272 0100 0000 e901  ...q.S.).r......
 000001d0: 0000 00a9 03da 056e 756d 7079 da06 6170  .......numpy..ap
 000001e0: 7065 6e64 da05 6172 7261 79a9 02da 022e  pend..array.....
 000001f0: 30da 0569 6e70 7574 a900 7211 0000 00fa  0..input..r.....
 00000200: 562f 686f 6d65 2f6a 656e 6b69 6e73 2f61  V/home/jenkins/a
 00000210: 6765 6e74 2f77 6f72 6b73 7061 6365 2f67  gent/workspace/g
 00000220: 6974 6561 2d70 6879 7369 6373 5f70 646d  itea-physics_pdm
-00000230: 655f 312e 332e 302f 7064 6d65 2f6d 6561  e_1.3.0/pdme/mea
+00000230: 655f 312e 342e 302f 7064 6d65 2f6d 6561  e_1.4.0/pdme/mea
 00000240: 7375 7265 6d65 6e74 2f69 6e70 7574 5f74  surement/input_t
 00000250: 7970 6573 2e70 79da 0a3c 6c69 7374 636f  ypes.py..<listco
 00000260: 6d70 3e0d 0000 00f3 0000 0000 7a27 646f  mp>.........z'do
 00000270: 745f 696e 7075 7473 5f74 6f5f 6172 7261  t_inputs_to_arra
 00000280: 792e 3c6c 6f63 616c 733e 2e3c 6c69 7374  y.<locals>.<list
 00000290: 636f 6d70 3ea9 0272 0b00 0000 720d 0000  comp>..r....r...
 000002a0: 0029 0172 0700 0000 7211 0000 0072 1100  .).r....r....r..
```

### Comparing `pdme-1.3.0/pdme/measurement/__pycache__/oscillating_dipole.cpython-39.pyc` & `pdme-1.4.0/pdme/measurement/__pycache__/oscillating_dipole.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 6903 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 f71a 0000  a.........Ff....
+00000000: 610d 0d0a 0000 0000 ffbb 4666 f71a 0000  a.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a02 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6404 6c07  m.Z.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6400 6405 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6400 6402 6c0d  m.Z.m.Z...d.d.l.
@@ -62,15 +62,15 @@
 000003d0: 2069 6e74 6f20 6e75 6d70 7920 6172 7261   into numpy arra
 000003e0: 7973 2e0a 0909 4e29 04da 056e 756d 7079  ys....N)...numpy
 000003f0: da05 6172 7261 7972 0c00 0000 720d 0000  ..arrayr....r...
 00000400: 00a9 01da 0473 656c 66a9 0072 1500 0000  .....self..r....
 00000410: fa5d 2f68 6f6d 652f 6a65 6e6b 696e 732f  .]/home/jenkins/
 00000420: 6167 656e 742f 776f 726b 7370 6163 652f  agent/workspace/
 00000430: 6769 7465 612d 7068 7973 6963 735f 7064  gitea-physics_pd
-00000440: 6d65 5f31 2e33 2e30 2f70 646d 652f 6d65  me_1.3.0/pdme/me
+00000440: 6d65 5f31 2e34 2e30 2f70 646d 652f 6d65  me_1.4.0/pdme/me
 00000450: 6173 7572 656d 656e 742f 6f73 6369 6c6c  asurement/oscill
 00000460: 6174 696e 675f 6469 706f 6c65 2e70 79da  ating_dipole.py.
 00000470: 0d5f 5f70 6f73 745f 696e 6974 5f5f 2300  .__post_init__#.
 00000480: 0000 7304 0000 0000 040e 017a 1f4f 7363  ..s........z.Osc
 00000490: 696c 6c61 7469 6e67 4469 706f 6c65 2e5f  illatingDipole._
 000004a0: 5f70 6f73 745f 696e 6974 5f5f 2902 da01  _post_init__)...
 000004b0: 7272 1000 0000 6302 0000 0000 0000 0000  rr....c.........
```

### Comparing `pdme-1.3.0/pdme/measurement/dot_measure.py` & `pdme-1.4.0/pdme/measurement/dot_measure.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/measurement/dot_pair_measure.py` & `pdme-1.4.0/pdme/measurement/dot_pair_measure.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/measurement/input_types.py` & `pdme-1.4.0/pdme/measurement/input_types.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/measurement/oscillating_dipole.py` & `pdme-1.4.0/pdme/measurement/oscillating_dipole.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/model/__init__.py` & `pdme-1.4.0/pdme/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/model/__pycache__/__init__.cpython-39.pyc` & `pdme-1.4.0/pdme/model/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 1066 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 2a04 0000  a.........Ff*...
+00000000: 610d 0d0a 0000 0000 ffbb 4666 2a04 0000  a.........Ff*...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -52,11 +52,11 @@
 00000330: 646f 6d5f 6368 6f69 6365 5f66 6978 6564  dom_choice_fixed
 00000340: 5f6f 7269 656e 7461 7469 6f6e 5f6d 6f64  _orientation_mod
 00000350: 656c 7208 0000 00da 075f 5f61 6c6c 5f5f  elr......__all__
 00000360: a900 720a 0000 0072 0a00 0000 fa4d 2f68  ..r....r.....M/h
 00000370: 6f6d 652f 6a65 6e6b 696e 732f 6167 656e  ome/jenkins/agen
 00000380: 742f 776f 726b 7370 6163 652f 6769 7465  t/workspace/gite
 00000390: 612d 7068 7973 6963 735f 7064 6d65 5f31  a-physics_pdme_1
-000003a0: 2e33 2e30 2f70 646d 652f 6d6f 6465 6c2f  .3.0/pdme/model/
+000003a0: 2e34 2e30 2f70 646d 652f 6d6f 6465 6c2f  .4.0/pdme/model/
 000003b0: 5f5f 696e 6974 5f5f 2e70 79da 083c 6d6f  __init__.py..<mo
 000003c0: 6475 6c65 3e01 0000 0073 0e00 0000 0c01  dule>....s......
 000003d0: 0c01 0c03 0c04 0c04 0c04 0c04            ............
```

### Comparing `pdme-1.3.0/pdme/model/__pycache__/fixed_magnitude_model.cpython-39.pyc` & `pdme-1.4.0/pdme/model/__pycache__/fixed_magnitude_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 2367 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 3f09 0000  a.........Ff?...
+00000000: 610d 0d0a 0000 0000 ffbb 4666 3f09 0000  a.........Ff?...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000060: 8400 6405 6503 8303 5a07 6401 5300 2906  ..d.e...Z.d.S.).
 00000070: e900 0000 004e 2901 da0b 4469 706f 6c65  .....N)...Dipole
@@ -45,15 +45,15 @@
 000002c0: 7261 6e64 6f6d da0b 6465 6661 756c 745f  random..default_
 000002d0: 726e 67da 0372 6e67 2908 da04 7365 6c66  rng..rng)...self
 000002e0: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
 000002f0: 0900 0000 720a 0000 0072 0b00 0000 720c  ....r....r....r.
 00000300: 0000 00a9 0072 1300 0000 fa5a 2f68 6f6d  .....r.....Z/hom
 00000310: 652f 6a65 6e6b 696e 732f 6167 656e 742f  e/jenkins/agent/
 00000320: 776f 726b 7370 6163 652f 6769 7465 612d  workspace/gitea-
-00000330: 7068 7973 6963 735f 7064 6d65 5f31 2e33  physics_pdme_1.3
+00000330: 7068 7973 6963 735f 7064 6d65 5f31 2e34  physics_pdme_1.4
 00000340: 2e30 2f70 646d 652f 6d6f 6465 6c2f 6669  .0/pdme/model/fi
 00000350: 7865 645f 6d61 676e 6974 7564 655f 6d6f  xed_magnitude_mo
 00000360: 6465 6c2e 7079 da08 5f5f 696e 6974 5f5f  del.py..__init__
 00000370: 1400 0000 7310 0000 0000 0a06 0106 0106  ....s...........
 00000380: 0106 0106 0106 0106 017a 2853 696e 676c  .........z(Singl
 00000390: 6544 6970 6f6c 6546 6978 6564 4d61 676e  eDipoleFixedMagn
 000003a0: 6974 7564 654d 6f64 656c 2e5f 5f69 6e69  itudeModel.__ini
```

### Comparing `pdme-1.3.0/pdme/model/__pycache__/log_spaced_random_choice_fixed_orientation_model.cpython-39.pyc` & `pdme-1.4.0/pdme/model/__pycache__/log_spaced_random_choice_fixed_orientation_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 5158 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 2614 0000  a.........Ff&...
+00000000: 610d 0d0a 0000 0000 ffbb 4666 2614 0000  a.........Ff&...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6401 6c07  m.Z.m.Z...d.d.l.
 00000060: 5a07 6400 6404 6c08 6d09 5a09 0100 6400  Z.d.d.l.m.Z...d.
 00000070: 6401 6c0a 5a0b 6507 a00c 650d a101 5a0e  d.l.Z.e...e...Z.
@@ -107,15 +107,15 @@
 000006a0: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
 000006b0: 0d00 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
 000006c0: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
 000006d0: 0000 da02 7078 da02 7079 da02 707a a900  ....px..py..pz..
 000006e0: 7223 0000 00fa 752f 686f 6d65 2f6a 656e  r#....u/home/jen
 000006f0: 6b69 6e73 2f61 6765 6e74 2f77 6f72 6b73  kins/agent/works
 00000700: 7061 6365 2f67 6974 6561 2d70 6879 7369  pace/gitea-physi
-00000710: 6373 5f70 646d 655f 312e 332e 302f 7064  cs_pdme_1.3.0/pd
+00000710: 6373 5f70 646d 655f 312e 342e 302f 7064  cs_pdme_1.4.0/pd
 00000720: 6d65 2f6d 6f64 656c 2f6c 6f67 5f73 7061  me/model/log_spa
 00000730: 6365 645f 7261 6e64 6f6d 5f63 686f 6963  ced_random_choic
 00000740: 655f 6669 7865 645f 6f72 6965 6e74 6174  e_fixed_orientat
 00000750: 696f 6e5f 6d6f 6465 6c2e 7079 da08 5f5f  ion_model.py..__
 00000760: 696e 6974 5f5f 2d00 0000 732c 0000 0000  init__-...s,....
 00000770: 1006 0106 0106 0106 0106 0106 0106 0106  ................
 00000780: 0106 0106 0106 010c 0106 021e 011e 0112  ................
```

### Comparing `pdme-1.3.0/pdme/model/__pycache__/log_spaced_random_choice_model.cpython-39.pyc` & `pdme-1.4.0/pdme/model/__pycache__/log_spaced_random_choice_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 5332 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 d414 0000  a.........Ff....
+00000000: 610d 0d0a 0000 0000 ffbb 4666 d414 0000  a.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6401 6c07  m.Z.m.Z...d.d.l.
 00000060: 5a08 6400 6404 6c09 6d0a 5a0a 0100 4700  Z.d.d.l.m.Z...G.
 00000070: 6405 6406 8400 6406 6503 8303 5a0b 6401  d.d...d.e...Z.d.
@@ -81,15 +81,15 @@
 00000500: 0000 0029 0cda 0473 656c 6672 0700 0000  ...)...selfr....
 00000510: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
 00000520: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
 00000530: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
 00000540: 0000 a900 721a 0000 00fa 632f 686f 6d65  ....r.....c/home
 00000550: 2f6a 656e 6b69 6e73 2f61 6765 6e74 2f77  /jenkins/agent/w
 00000560: 6f72 6b73 7061 6365 2f67 6974 6561 2d70  orkspace/gitea-p
-00000570: 6879 7369 6373 5f70 646d 655f 312e 332e  hysics_pdme_1.3.
+00000570: 6879 7369 6373 5f70 646d 655f 312e 342e  hysics_pdme_1.4.
 00000580: 302f 7064 6d65 2f6d 6f64 656c 2f6c 6f67  0/pdme/model/log
 00000590: 5f73 7061 6365 645f 7261 6e64 6f6d 5f63  _spaced_random_c
 000005a0: 686f 6963 655f 6d6f 6465 6c2e 7079 da08  hoice_model.py..
 000005b0: 5f5f 696e 6974 5f5f 2000 0000 7320 0000  __init__ ...s ..
 000005c0: 0000 0e06 0106 0106 0106 0106 0106 0106  ................
 000005d0: 0106 0106 010c 0106 0110 0102 0108 ff04  ................
 000005e0: 037a 3e4c 6f67 5370 6163 6564 5261 6e64  .z>LogSpacedRand
```

### Comparing `pdme-1.3.0/pdme/model/__pycache__/log_spaced_random_choice_xy_model.cpython-39.pyc` & `pdme-1.4.0/pdme/model/__pycache__/log_spaced_random_choice_xy_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 4699 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 5b12 0000  a.........Ff[...
+00000000: 610d 0d0a 0000 0000 ffbb 4666 5b12 0000  a.........Ff[...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6401 6c07  m.Z.m.Z...d.d.l.
 00000060: 5a08 6400 6404 6c09 6d0a 5a0a 0100 4700  Z.d.d.l.m.Z...G.
 00000070: 6405 6406 8400 6406 6503 8303 5a0b 6401  d.d...d.e...Z.d.
@@ -82,15 +82,15 @@
 00000510: 0029 0cda 0473 656c 6672 0700 0000 7208  .)...selfr....r.
 00000520: 0000 0072 0900 0000 720a 0000 0072 0b00  ...r....r....r..
 00000530: 0000 720c 0000 0072 0d00 0000 720e 0000  ..r....r....r...
 00000540: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
 00000550: a900 721a 0000 00fa 662f 686f 6d65 2f6a  ..r.....f/home/j
 00000560: 656e 6b69 6e73 2f61 6765 6e74 2f77 6f72  enkins/agent/wor
 00000570: 6b73 7061 6365 2f67 6974 6561 2d70 6879  kspace/gitea-phy
-00000580: 7369 6373 5f70 646d 655f 312e 332e 302f  sics_pdme_1.3.0/
+00000580: 7369 6373 5f70 646d 655f 312e 342e 302f  sics_pdme_1.4.0/
 00000590: 7064 6d65 2f6d 6f64 656c 2f6c 6f67 5f73  pdme/model/log_s
 000005a0: 7061 6365 645f 7261 6e64 6f6d 5f63 686f  paced_random_cho
 000005b0: 6963 655f 7879 5f6d 6f64 656c 2e70 79da  ice_xy_model.py.
 000005c0: 085f 5f69 6e69 745f 5f20 0000 0073 2000  .__init__ ...s .
 000005d0: 0000 000e 0601 0601 0601 0601 0601 0601  ................
 000005e0: 0601 0601 0601 0c01 0601 1001 0201 08ff  ................
 000005f0: 0403 7a40 4c6f 6753 7061 6365 6452 616e  ..z@LogSpacedRan
```

### Comparing `pdme-1.3.0/pdme/model/__pycache__/model.cpython-39.pyc` & `pdme-1.4.0/pdme/model/__pycache__/model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 3594 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 0a0e 0000  a.........Ff....
+00000000: 610d 0d0a 0000 0000 ffbb 4666 0a0e 0000  a.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a04 6400 6401 6c05 5a06 6400 6403 6c07  Z.d.d.l.Z.d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6504  m.Z.m.Z.m.Z...e.
 00000070: a00b 650c a101 5a0d 4700 6404 6405 8400  ..e...Z.G.d.d...
@@ -59,15 +59,15 @@
 000003a0: 6672 6571 7565 6e63 7929 2e0a 0909 4ea9  frequency)....N.
 000003b0: 01da 134e 6f74 496d 706c 656d 656e 7465  ...NotImplemente
 000003c0: 6445 7272 6f72 2903 da04 7365 6c66 7207  dError)...selfr.
 000003d0: 0000 0072 0800 0000 a900 720d 0000 00fa  ...r......r.....
 000003e0: 4a2f 686f 6d65 2f6a 656e 6b69 6e73 2f61  J/home/jenkins/a
 000003f0: 6765 6e74 2f77 6f72 6b73 7061 6365 2f67  gent/workspace/g
 00000400: 6974 6561 2d70 6879 7369 6373 5f70 646d  itea-physics_pdm
-00000410: 655f 312e 332e 302f 7064 6d65 2f6d 6f64  e_1.3.0/pdme/mod
+00000410: 655f 312e 342e 302f 7064 6d65 2f6d 6f64  e_1.4.0/pdme/mod
 00000420: 656c 2f6d 6f64 656c 2e70 79da 0b67 6574  el/model.py..get
 00000430: 5f64 6970 6f6c 6573 1300 0000 7302 0000  _dipoles....s...
 00000440: 0000 087a 1744 6970 6f6c 654d 6f64 656c  ...z.DipoleModel
 00000450: 2e67 6574 5f64 6970 6f6c 6573 2904 da01  .get_dipoles)...
 00000460: 6e72 0700 0000 7208 0000 0072 0900 0000  nr....r....r....
 00000470: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
 00000480: 0001 0000 0043 0000 0073 0800 0000 7400  .....C...s....t.
```

### Comparing `pdme-1.3.0/pdme/model/__pycache__/multidipole_fixed_magnitude_model.cpython-39.pyc` & `pdme-1.4.0/pdme/model/__pycache__/multidipole_fixed_magnitude_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 2560 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 000a 0000  a.........Ff....
+00000000: 610d 0d0a 0000 0000 ffbb 4666 000a 0000  a.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000060: 8400 6405 6503 8303 5a07 6401 5300 2906  ..d.e...Z.d.S.).
 00000070: e900 0000 004e 2901 da0b 4469 706f 6c65  .....N)...Dipole
@@ -49,15 +49,15 @@
 00000300: 745f 726e 67da 0372 6e67 720d 0000 0029  t_rng..rngr....)
 00000310: 09da 0473 656c 6672 0600 0000 7207 0000  ...selfr....r...
 00000320: 0072 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
 00000330: 720b 0000 0072 0c00 0000 720d 0000 00a9  r....r....r.....
 00000340: 0072 1400 0000 fa66 2f68 6f6d 652f 6a65  .r.....f/home/je
 00000350: 6e6b 696e 732f 6167 656e 742f 776f 726b  nkins/agent/work
 00000360: 7370 6163 652f 6769 7465 612d 7068 7973  space/gitea-phys
-00000370: 6963 735f 7064 6d65 5f31 2e33 2e30 2f70  ics_pdme_1.3.0/p
+00000370: 6963 735f 7064 6d65 5f31 2e34 2e30 2f70  ics_pdme_1.4.0/p
 00000380: 646d 652f 6d6f 6465 6c2f 6d75 6c74 6964  dme/model/multid
 00000390: 6970 6f6c 655f 6669 7865 645f 6d61 676e  ipole_fixed_magn
 000003a0: 6974 7564 655f 6d6f 6465 6c2e 7079 da08  itude_model.py..
 000003b0: 5f5f 696e 6974 5f5f 1700 0000 7312 0000  __init__....s...
 000003c0: 0000 0b06 0106 0106 0106 0106 0106 0106  ................
 000003d0: 010c 017a 2a4d 756c 7469 706c 6544 6970  ...z*MultipleDip
 000003e0: 6f6c 6546 6978 6564 4d61 676e 6974 7564  oleFixedMagnitud
```

### Comparing `pdme-1.3.0/pdme/model/__pycache__/random_count_multidipole_fixed_magnitude_model.cpython-39.pyc` & `pdme-1.4.0/pdme/model/__pycache__/random_count_multidipole_fixed_magnitude_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 3076 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 040c 0000  a.........Ff....
+00000000: 610d 0d0a 0000 0000 ffbb 4666 040c 0000  a.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000060: 8400 6405 6503 8303 5a07 6401 5300 2906  ..d.e...Z.d.S.).
 00000070: e900 0000 004e 2901 da0b 4469 706f 6c65  .....N)...Dipole
@@ -65,15 +65,15 @@
 00000400: 7272 0e00 0000 290a da04 7365 6c66 7206  rr....)...selfr.
 00000410: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
 00000420: 0000 720a 0000 0072 0b00 0000 720c 0000  ..r....r....r...
 00000430: 0072 0d00 0000 720e 0000 00a9 0072 1700  .r....r......r..
 00000440: 0000 fa73 2f68 6f6d 652f 6a65 6e6b 696e  ...s/home/jenkin
 00000450: 732f 6167 656e 742f 776f 726b 7370 6163  s/agent/workspac
 00000460: 652f 6769 7465 612d 7068 7973 6963 735f  e/gitea-physics_
-00000470: 7064 6d65 5f31 2e33 2e30 2f70 646d 652f  pdme_1.3.0/pdme/
+00000470: 7064 6d65 5f31 2e34 2e30 2f70 646d 652f  pdme_1.4.0/pdme/
 00000480: 6d6f 6465 6c2f 7261 6e64 6f6d 5f63 6f75  model/random_cou
 00000490: 6e74 5f6d 756c 7469 6469 706f 6c65 5f66  nt_multidipole_f
 000004a0: 6978 6564 5f6d 6167 6e69 7475 6465 5f6d  ixed_magnitude_m
 000004b0: 6f64 656c 2e70 79da 085f 5f69 6e69 745f  odel.py..__init_
 000004c0: 5f1a 0000 0073 1c00 0000 000c 0601 0601  _....s..........
 000004d0: 0601 0601 0601 0601 0601 0c01 0601 1001  ................
 000004e0: 0201 08ff 0403 7a35 5261 6e64 6f6d 436f  ......z5RandomCo
```

### Comparing `pdme-1.3.0/pdme/model/fixed_magnitude_model.py` & `pdme-1.4.0/pdme/model/fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/model/log_spaced_random_choice_fixed_orientation_model.py` & `pdme-1.4.0/pdme/model/log_spaced_random_choice_fixed_orientation_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/model/log_spaced_random_choice_model.py` & `pdme-1.4.0/pdme/model/log_spaced_random_choice_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/model/log_spaced_random_choice_xy_model.py` & `pdme-1.4.0/pdme/model/log_spaced_random_choice_xy_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/model/model.py` & `pdme-1.4.0/pdme/model/model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/model/multidipole_fixed_magnitude_model.py` & `pdme-1.4.0/pdme/model/multidipole_fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/model/random_count_multidipole_fixed_magnitude_model.py` & `pdme-1.4.0/pdme/model/random_count_multidipole_fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/subspace_simulation/__init__.py` & `pdme-1.4.0/pdme/subspace_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/subspace_simulation/__pycache__/__init__.cpython-39.pyc` & `pdme-1.4.0/pdme/subspace_simulation/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 1875 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 5307 0000  a.........FfS...
+00000000: 610d 0d0a 0000 0000 ffbb 4666 5307 0000  a.........FfS...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a04 6400  m.Z...d.d.l.Z.d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6501  d.l.m.Z.m.Z...e.
 00000060: 4700 6405 6406 8400 6406 8302 8301 5a08  G.d.d...d.....Z.
 00000070: 4700 6407 6408 8400 6408 8302 5a09 6504  G.d.d...d...Z.e.
@@ -37,15 +37,15 @@
 00000240: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
 00000250: 5f5f 646f 635f 5fda 0566 6c6f 6174 da0f  __doc__..float..
 00000260: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5fa9  __annotations__.
 00000270: 0072 0d00 0000 720d 0000 00fa 5b2f 686f  .r....r.....[/ho
 00000280: 6d65 2f6a 656e 6b69 6e73 2f61 6765 6e74  me/jenkins/agent
 00000290: 2f77 6f72 6b73 7061 6365 2f67 6974 6561  /workspace/gitea
 000002a0: 2d70 6879 7369 6373 5f70 646d 655f 312e  -physics_pdme_1.
-000002b0: 332e 302f 7064 6d65 2f73 7562 7370 6163  3.0/pdme/subspac
+000002b0: 342e 302f 7064 6d65 2f73 7562 7370 6163  4.0/pdme/subspac
 000002c0: 655f 7369 6d75 6c61 7469 6f6e 2f5f 5f69  e_simulation/__i
 000002d0: 6e69 745f 5f2e 7079 7206 0000 000a 0000  nit__.pyr.......
 000002e0: 0073 0e00 0000 0a02 0404 0801 0801 0801  .s..............
 000002f0: 0801 0801 7206 0000 0063 0000 0000 0000  ....r....c......
 00000300: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
 00000310: 0000 732a 0000 0065 005a 0164 005a 0264  ..s*...e.Z.d.Z.d
 00000320: 015a 0365 0465 0519 0064 029c 0164 0364  .Z.e.e...d...d.d
```

### Comparing `pdme-1.3.0/pdme/util/__pycache__/fast_nonlocal_spectrum.cpython-39.pyc` & `pdme-1.4.0/pdme/util/__pycache__/fast_nonlocal_spectrum.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 9670 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 c625 0000  a.........Ff.%..
+00000000: 610d 0d0a 0000 0000 ffbb 4666 c625 0000  a.........Ff.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6501  d.l.Z.d.d.l.Z.e.
 00000040: a002 6503 a101 5a04 6500 6a05 6500 6a05  ..e...Z.e.j.e.j.
 00000050: 6500 6a05 6402 9c03 6403 6404 8404 5a06  e.j.d...d.d...Z.
 00000060: 6500 6a05 6500 6a05 6500 6a05 6405 9c03  e.j.e.j.e.j.d...
 00000070: 6406 6407 8404 5a07 6500 6a05 6500 6a05  d.d...Z.e.j.e.j.
@@ -73,15 +73,15 @@
 00000480: da08 6469 6666 7365 7331 da08 6469 6666  ..diffses1..diff
 00000490: 7365 7332 da06 6e6f 726d 7331 da06 6e6f  ses2..norms1..no
 000004a0: 726d 7332 da08 616c 7068 7365 7331 da08  rms2..alphses1..
 000004b0: 616c 7068 7365 7332 da04 6273 6573 a900  alphses2..bses..
 000004c0: 7232 0000 00fa 5a2f 686f 6d65 2f6a 656e  r2....Z/home/jen
 000004d0: 6b69 6e73 2f61 6765 6e74 2f77 6f72 6b73  kins/agent/works
 000004e0: 7061 6365 2f67 6974 6561 2d70 6879 7369  pace/gitea-physi
-000004f0: 6373 5f70 646d 655f 312e 332e 302f 7064  cs_pdme_1.3.0/pd
+000004f0: 6373 5f70 646d 655f 312e 342e 302f 7064  cs_pdme_1.4.0/pd
 00000500: 6d65 2f75 7469 6c2f 6661 7374 5f6e 6f6e  me/util/fast_non
 00000510: 6c6f 6361 6c5f 7370 6563 7472 756d 2e70  local_spectrum.p
 00000520: 79da 0f66 6173 745f 735f 6e6f 6e6c 6f63  y..fast_s_nonloc
 00000530: 616c 0800 0000 733e 0000 0000 0614 0114  al....s>........
 00000540: 0110 0210 0110 0110 0216 0116 0112 0112  ................
 00000550: 020c 010e 0214 0114 010e 0110 0110 0214  ................
 00000560: 0114 010e 0110 0110 0212 0112 010e 0110  ................
```

### Comparing `pdme-1.3.0/pdme/util/__pycache__/fast_v_calc.cpython-39.pyc` & `pdme-1.4.0/pdme/util/__pycache__/fast_v_calc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May 17 00:23:46 2024 UTC, .py size: 7195 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 92a3 4666 1b1c 0000  a.........Ff....
+00000000: 610d 0d0a 0000 0000 ffbb 4666 1b1c 0000  a.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6501  d.l.Z.d.d.l.Z.e.
 00000040: a002 6503 a101 5a04 6500 6a05 6500 6a05  ..e...Z.e.j.e.j.
 00000050: 6500 6a05 6402 9c03 6403 6404 8404 5a06  e.j.d...d.d...Z.
 00000060: 6500 6a05 6500 6a05 6500 6a05 6405 9c03  e.j.e.j.e.j.d...
 00000070: 6406 6407 8404 5a07 6500 6a05 6500 6a05  d.d...Z.e.j.e.j.
@@ -59,15 +59,15 @@
 000003a0: 6929 0b72 0200 0000 7203 0000 00da 0270  i).r....r......p
 000003b0: 73da 0273 73da 0277 73da 0272 73da 0266  s..ss..ws..rs..f
 000003c0: 73da 0764 6966 6673 6573 da05 6e6f 726d  s..diffses..norm
 000003d0: 73da 0461 7365 73da 0462 7365 73a9 0072  s..ases..bses..r
 000003e0: 2300 0000 fa4f 2f68 6f6d 652f 6a65 6e6b  #....O/home/jenk
 000003f0: 696e 732f 6167 656e 742f 776f 726b 7370  ins/agent/worksp
 00000400: 6163 652f 6769 7465 612d 7068 7973 6963  ace/gitea-physic
-00000410: 735f 7064 6d65 5f31 2e33 2e30 2f70 646d  s_pdme_1.3.0/pdm
+00000410: 735f 7064 6d65 5f31 2e34 2e30 2f70 646d  s_pdme_1.4.0/pdm
 00000420: 652f 7574 696c 2f66 6173 745f 765f 6361  e/util/fast_v_ca
 00000430: 6c63 2e70 79da 1366 6173 745f 7673 5f66  lc.py..fast_vs_f
 00000440: 6f72 5f64 6970 6f6c 6573 0800 0000 7322  or_dipoles....s"
 00000450: 0000 0000 0d14 0114 0210 0210 0110 0110  ................
 00000460: 0314 0210 0414 0210 0214 0110 0216 0110  ................
 00000470: 0436 0210 0272 2500 0000 2903 7202 0000  .6...r%...).r...
 00000480: 00da 0964 6970 6f6c 6573 6573 7204 0000  ...dipolesesr...
```

### Comparing `pdme-1.3.0/pdme/util/fast_nonlocal_spectrum.py` & `pdme-1.4.0/pdme/util/fast_nonlocal_spectrum.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pdme/util/fast_v_calc.py` & `pdme-1.4.0/pdme/util/fast_v_calc.py`

 * *Files identical despite different names*

### Comparing `pdme-1.3.0/pyproject.toml` & `pdme-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdme"
-version = "1.3.0"
+version = "1.4.0"
 description = "Python dipole model evaluator"
 authors = ["Deepak <dmallubhotla+github@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
```

### Comparing `pdme-1.3.0/PKG-INFO` & `pdme-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdme
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python dipole model evaluator
 License: GPL-3.0-only
 Author: Deepak
 Author-email: dmallubhotla+github@gmail.com
 Requires-Python: >=3.8.1,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

