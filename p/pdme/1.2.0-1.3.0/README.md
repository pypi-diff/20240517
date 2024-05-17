# Comparing `tmp/pdme-1.2.0.tar.gz` & `tmp/pdme-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdme-1.2.0.tar", max compression
+gzip compressed data, was "pdme-1.3.0.tar", max compression
```

## Comparing `pdme-1.2.0.tar` & `pdme-1.3.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1229 2024-05-03 01:57:25.337343 pdme-1.2.0/README.md
--rw-r--r--   0        0        0      154 2024-05-03 01:57:25.337343 pdme-1.2.0/pdme/__init__.py
--rw-r--r--   0        0        0     1578 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/calculations/__init__.py
--rw-r--r--   0        0        0     1939 2024-05-03 01:58:02.999180 pdme-1.2.0/pdme/calculations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      184 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/inputs/__init__.py
--rw-r--r--   0        0        0      315 2024-05-03 01:58:03.315195 pdme-1.2.0/pdme/inputs/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1471 2024-05-03 01:58:03.319195 pdme-1.2.0/pdme/inputs/__pycache__/dot_inputs.cpython-39.pyc
--rw-r--r--   0        0        0      688 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/inputs/dot_inputs.py
--rw-r--r--   0        0        0      536 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/measurement/__init__.py
--rw-r--r--   0        0        0      642 2024-05-03 01:58:03.355197 pdme-1.2.0/pdme/measurement/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1642 2024-05-03 01:58:03.359197 pdme-1.2.0/pdme/measurement/__pycache__/dot_measure.cpython-39.pyc
--rw-r--r--   0        0        0     1864 2024-05-03 01:58:03.359197 pdme-1.2.0/pdme/measurement/__pycache__/dot_pair_measure.cpython-39.pyc
--rw-r--r--   0        0        0     1818 2024-05-03 01:58:03.367198 pdme-1.2.0/pdme/measurement/__pycache__/input_types.cpython-39.pyc
--rw-r--r--   0        0        0     9719 2024-05-03 01:58:03.363197 pdme-1.2.0/pdme/measurement/__pycache__/oscillating_dipole.cpython-39.pyc
--rw-r--r--   0        0        0      984 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/measurement/dot_measure.py
--rw-r--r--   0        0        0     1224 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/measurement/dot_pair_measure.py
--rw-r--r--   0        0        0     1131 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/measurement/input_types.py
--rw-r--r--   0        0        0     6903 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/measurement/oscillating_dipole.py
--rw-r--r--   0        0        0       70 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/meta.py
--rw-r--r--   0        0        0     1066 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/model/__init__.py
--rw-r--r--   0        0        0      988 2024-05-03 01:58:03.395199 pdme-1.2.0/pdme/model/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2740 2024-05-03 01:58:03.407199 pdme-1.2.0/pdme/model/__pycache__/fixed_magnitude_model.cpython-39.pyc
--rw-r--r--   0        0        0     5039 2024-05-03 01:58:03.419200 pdme-1.2.0/pdme/model/__pycache__/log_spaced_random_choice_fixed_orientation_model.cpython-39.pyc
--rw-r--r--   0        0        0     5083 2024-05-03 01:58:03.411200 pdme-1.2.0/pdme/model/__pycache__/log_spaced_random_choice_model.cpython-39.pyc
--rw-r--r--   0        0        0     4757 2024-05-03 01:58:03.415200 pdme-1.2.0/pdme/model/__pycache__/log_spaced_random_choice_xy_model.cpython-39.pyc
--rw-r--r--   0        0        0     3850 2024-05-03 01:58:03.395199 pdme-1.2.0/pdme/model/__pycache__/model.cpython-39.pyc
--rw-r--r--   0        0        0     2928 2024-05-03 01:58:03.407199 pdme-1.2.0/pdme/model/__pycache__/multidipole_fixed_magnitude_model.cpython-39.pyc
--rw-r--r--   0        0        0     3362 2024-05-03 01:58:03.411200 pdme-1.2.0/pdme/model/__pycache__/random_count_multidipole_fixed_magnitude_model.cpython-39.pyc
--rw-r--r--   0        0        0     2367 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/model/fixed_magnitude_model.py
--rw-r--r--   0        0        0     5158 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/model/log_spaced_random_choice_fixed_orientation_model.py
--rw-r--r--   0        0        0     5332 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/model/log_spaced_random_choice_model.py
--rw-r--r--   0        0        0     4699 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/model/log_spaced_random_choice_xy_model.py
--rw-r--r--   0        0        0     3594 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/model/model.py
--rw-r--r--   0        0        0     2560 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/model/multidipole_fixed_magnitude_model.py
--rw-r--r--   0        0        0     3076 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/model/random_count_multidipole_fixed_magnitude_model.py
--rw-r--r--   0        0        0        0 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/py.typed
--rw-r--r--   0        0        0     1364 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/subspace_simulation/__init__.py
--rw-r--r--   0        0        0     2144 2024-05-03 01:58:03.399199 pdme-1.2.0/pdme/subspace_simulation/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      842 2024-05-03 01:58:03.399199 pdme-1.2.0/pdme/subspace_simulation/__pycache__/mcmc_costs.cpython-39.pyc
--rw-r--r--   0        0        0      575 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/subspace_simulation/mcmc_costs.py
--rw-r--r--   0        0        0        0 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/util/__init__.py
--rw-r--r--   0        0        0      167 2024-05-03 01:58:03.399199 pdme-1.2.0/pdme/util/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4170 2024-05-03 01:58:03.659212 pdme-1.2.0/pdme/util/__pycache__/fast_nonlocal_spectrum.cpython-39.pyc
--rw-r--r--   0        0        0     5553 2024-05-03 01:58:03.403199 pdme-1.2.0/pdme/util/__pycache__/fast_v_calc.cpython-39.pyc
--rw-r--r--   0        0        0     9670 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/util/fast_nonlocal_spectrum.py
--rw-r--r--   0        0        0     7195 2024-05-03 01:57:25.341343 pdme-1.2.0/pdme/util/fast_v_calc.py
--rw-r--r--   0        0        0      965 2024-05-03 01:57:25.345343 pdme-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 pdme-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1229 2024-05-17 00:23:46.157294 pdme-1.3.0/README.md
+-rw-r--r--   0        0        0      154 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/__init__.py
+-rw-r--r--   0        0        0     1578 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/calculations/__init__.py
+-rw-r--r--   0        0        0     1939 2024-05-17 00:24:12.778603 pdme-1.3.0/pdme/calculations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      184 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/inputs/__init__.py
+-rw-r--r--   0        0        0      315 2024-05-17 00:24:13.050617 pdme-1.3.0/pdme/inputs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1471 2024-05-17 00:24:13.050617 pdme-1.3.0/pdme/inputs/__pycache__/dot_inputs.cpython-39.pyc
+-rw-r--r--   0        0        0      688 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/inputs/dot_inputs.py
+-rw-r--r--   0        0        0      536 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/measurement/__init__.py
+-rw-r--r--   0        0        0      642 2024-05-17 00:24:13.086618 pdme-1.3.0/pdme/measurement/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1642 2024-05-17 00:24:13.090618 pdme-1.3.0/pdme/measurement/__pycache__/dot_measure.cpython-39.pyc
+-rw-r--r--   0        0        0     1864 2024-05-17 00:24:13.090618 pdme-1.3.0/pdme/measurement/__pycache__/dot_pair_measure.cpython-39.pyc
+-rw-r--r--   0        0        0     1818 2024-05-17 00:24:13.098619 pdme-1.3.0/pdme/measurement/__pycache__/input_types.cpython-39.pyc
+-rw-r--r--   0        0        0     9719 2024-05-17 00:24:13.094619 pdme-1.3.0/pdme/measurement/__pycache__/oscillating_dipole.cpython-39.pyc
+-rw-r--r--   0        0        0      984 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/measurement/dot_measure.py
+-rw-r--r--   0        0        0     1224 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/measurement/dot_pair_measure.py
+-rw-r--r--   0        0        0     1131 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/measurement/input_types.py
+-rw-r--r--   0        0        0     6903 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/measurement/oscillating_dipole.py
+-rw-r--r--   0        0        0       70 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/meta.py
+-rw-r--r--   0        0        0     1066 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/model/__init__.py
+-rw-r--r--   0        0        0      988 2024-05-17 00:24:13.126620 pdme-1.3.0/pdme/model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2740 2024-05-17 00:24:13.142621 pdme-1.3.0/pdme/model/__pycache__/fixed_magnitude_model.cpython-39.pyc
+-rw-r--r--   0        0        0     5039 2024-05-17 00:24:13.162622 pdme-1.3.0/pdme/model/__pycache__/log_spaced_random_choice_fixed_orientation_model.cpython-39.pyc
+-rw-r--r--   0        0        0     5083 2024-05-17 00:24:13.154622 pdme-1.3.0/pdme/model/__pycache__/log_spaced_random_choice_model.cpython-39.pyc
+-rw-r--r--   0        0        0     4757 2024-05-17 00:24:13.158622 pdme-1.3.0/pdme/model/__pycache__/log_spaced_random_choice_xy_model.cpython-39.pyc
+-rw-r--r--   0        0        0     3850 2024-05-17 00:24:13.130621 pdme-1.3.0/pdme/model/__pycache__/model.cpython-39.pyc
+-rw-r--r--   0        0        0     2928 2024-05-17 00:24:13.146621 pdme-1.3.0/pdme/model/__pycache__/multidipole_fixed_magnitude_model.cpython-39.pyc
+-rw-r--r--   0        0        0     3362 2024-05-17 00:24:13.150622 pdme-1.3.0/pdme/model/__pycache__/random_count_multidipole_fixed_magnitude_model.cpython-39.pyc
+-rw-r--r--   0        0        0     2367 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/model/fixed_magnitude_model.py
+-rw-r--r--   0        0        0     5158 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/model/log_spaced_random_choice_fixed_orientation_model.py
+-rw-r--r--   0        0        0     5332 2024-05-17 00:23:46.157294 pdme-1.3.0/pdme/model/log_spaced_random_choice_model.py
+-rw-r--r--   0        0        0     4699 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/model/log_spaced_random_choice_xy_model.py
+-rw-r--r--   0        0        0     3594 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/model/model.py
+-rw-r--r--   0        0        0     2560 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/model/multidipole_fixed_magnitude_model.py
+-rw-r--r--   0        0        0     3076 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/model/random_count_multidipole_fixed_magnitude_model.py
+-rw-r--r--   0        0        0        0 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/py.typed
+-rw-r--r--   0        0        0     1875 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/subspace_simulation/__init__.py
+-rw-r--r--   0        0        0     2807 2024-05-17 00:24:13.130621 pdme-1.3.0/pdme/subspace_simulation/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      842 2024-05-17 00:24:13.134621 pdme-1.3.0/pdme/subspace_simulation/__pycache__/mcmc_costs.cpython-39.pyc
+-rw-r--r--   0        0        0      575 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/subspace_simulation/mcmc_costs.py
+-rw-r--r--   0        0        0        0 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/util/__init__.py
+-rw-r--r--   0        0        0      167 2024-05-17 00:24:13.134621 pdme-1.3.0/pdme/util/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4170 2024-05-17 00:24:13.414635 pdme-1.3.0/pdme/util/__pycache__/fast_nonlocal_spectrum.cpython-39.pyc
+-rw-r--r--   0        0        0     5553 2024-05-17 00:24:13.138621 pdme-1.3.0/pdme/util/__pycache__/fast_v_calc.cpython-39.pyc
+-rw-r--r--   0        0        0     9670 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/util/fast_nonlocal_spectrum.py
+-rw-r--r--   0        0        0     7195 2024-05-17 00:23:46.161294 pdme-1.3.0/pdme/util/fast_v_calc.py
+-rw-r--r--   0        0        0      965 2024-05-17 00:23:46.161294 pdme-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 pdme-1.3.0/PKG-INFO
```

### Comparing `pdme-1.2.0/README.md` & `pdme-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/calculations/__init__.py` & `pdme-1.3.0/pdme/calculations/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/calculations/__pycache__/__init__.cpython-39.pyc` & `pdme-1.3.0/pdme/calculations/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 1578 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 2a06 0000  a........D4f*...
+00000000: 610d 0d0a 0000 0000 92a3 4666 2a06 0000  a.........Ff*...
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
-000003f0: 655f 312e 322e 302f 7064 6d65 2f63 616c  e_1.2.0/pdme/cal
+000003f0: 655f 312e 332e 302f 7064 6d65 2f63 616c  e_1.3.0/pdme/cal
 00000400: 6375 6c61 7469 6f6e 732f 5f5f 696e 6974  culations/__init
 00000410: 5f5f 2e70 79da 0e74 656c 6567 7261 7068  __.py..telegraph
 00000420: 5f62 6574 6108 0000 0073 0200 0000 000a  _beta....s......
 00000430: 720a 0000 0029 04da 0170 da01 73da 0172  r....)...p..s..r
 00000440: 7204 0000 0063 0300 0000 0000 0000 0000  r....c..........
 00000450: 0000 0400 0000 0400 0000 4300 0000 7326  ..........C...s&
 00000460: 0000 007c 027c 0118 007d 037c 00a0 007c  ...|.|...}.|...|
```

### Comparing `pdme-1.2.0/pdme/inputs/__pycache__/dot_inputs.cpython-39.pyc` & `pdme-1.3.0/pdme/inputs/__pycache__/dot_inputs.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 688 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 b002 0000  a........D4f....
+00000000: 610d 0d0a 0000 0000 92a3 4666 b002 0000  a.........Ff....
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
-000001f0: 646d 655f 312e 322e 302f 7064 6d65 2f69  dme_1.2.0/pdme/i
+000001f0: 646d 655f 312e 332e 302f 7064 6d65 2f69  dme_1.3.0/pdme/i
 00000200: 6e70 7574 732f 646f 745f 696e 7075 7473  nputs/dot_inputs
 00000210: 2e70 79da 0a3c 6c69 7374 636f 6d70 3e0a  .py..<listcomp>.
 00000220: 0000 00f3 0000 0000 7a3a 696e 7075 7473  ........z:inputs
 00000230: 5f77 6974 685f 6672 6571 7565 6e63 795f  _with_frequency_
 00000240: 7261 6e67 652e 3c6c 6f63 616c 733e 2e3c  range.<locals>.<
 00000250: 6c69 7374 636f 6d70 3e2e 3c6c 6973 7463  listcomp>.<listc
 00000260: 6f6d 703e 7207 0000 00a9 0172 0900 0000  omp>r......r....
```

### Comparing `pdme-1.2.0/pdme/inputs/dot_inputs.py` & `pdme-1.3.0/pdme/inputs/dot_inputs.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/measurement/__init__.py` & `pdme-1.3.0/pdme/measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/measurement/__pycache__/__init__.cpython-39.pyc` & `pdme-1.3.0/pdme/measurement/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 536 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 1802 0000  a........D4f....
+00000000: 610d 0d0a 0000 0000 92a3 4666 1802 0000  a.........Ff....
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
-00000240: 7064 6d65 5f31 2e32 2e30 2f70 646d 652f  pdme_1.2.0/pdme/
+00000240: 7064 6d65 5f31 2e33 2e30 2f70 646d 652f  pdme_1.3.0/pdme/
 00000250: 6d65 6173 7572 656d 656e 742f 5f5f 696e  measurement/__in
 00000260: 6974 5f5f 2e70 79da 083c 6d6f 6475 6c65  it__.py..<module
 00000270: 3e01 0000 0073 0800 0000 1001 1004 1004  >....s..........
 00000280: 1003                                     ..
```

### Comparing `pdme-1.2.0/pdme/measurement/__pycache__/dot_measure.cpython-39.pyc` & `pdme-1.3.0/pdme/measurement/__pycache__/dot_measure.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 984 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 d803 0000  a........D4f....
+00000000: 610d 0d0a 0000 0000 92a3 4666 d803 0000  a.........Ff....
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
-00000260: 735f 7064 6d65 5f31 2e32 2e30 2f70 646d  s_pdme_1.2.0/pdm
+00000260: 735f 7064 6d65 5f31 2e33 2e30 2f70 646d  s_pdme_1.3.0/pdm
 00000270: 652f 6d65 6173 7572 656d 656e 742f 646f  e/measurement/do
 00000280: 745f 6d65 6173 7572 652e 7079 da0d 5f5f  t_measure.py..__
 00000290: 706f 7374 5f69 6e69 745f 5f1b 0000 0073  post_init__....s
 000002a0: 0200 0000 0001 7a1c 446f 744d 6561 7375  ......z.DotMeasu
 000002b0: 7265 6d65 6e74 2e5f 5f70 6f73 745f 696e  rement.__post_in
 000002c0: 6974 5f5f a909 da08 5f5f 6e61 6d65 5f5f  it__....__name__
 000002d0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
```

### Comparing `pdme-1.2.0/pdme/measurement/__pycache__/dot_pair_measure.cpython-39.pyc` & `pdme-1.3.0/pdme/measurement/__pycache__/dot_pair_measure.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 1224 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 c804 0000  a........D4f....
+00000000: 610d 0d0a 0000 0000 92a3 4666 c804 0000  a.........Ff....
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
-000002c0: 7068 7973 6963 735f 7064 6d65 5f31 2e32  physics_pdme_1.2
+000002c0: 7068 7973 6963 735f 7064 6d65 5f31 2e33  physics_pdme_1.3
 000002d0: 2e30 2f70 646d 652f 6d65 6173 7572 656d  .0/pdme/measurem
 000002e0: 656e 742f 646f 745f 7061 6972 5f6d 6561  ent/dot_pair_mea
 000002f0: 7375 7265 2e70 79da 0d5f 5f70 6f73 745f  sure.py..__post_
 00000300: 696e 6974 5f5f 1f00 0000 7304 0000 0000  init__....s.....
 00000310: 010e 017a 2044 6f74 5061 6972 4d65 6173  ...z DotPairMeas
 00000320: 7572 656d 656e 742e 5f5f 706f 7374 5f69  urement.__post_i
 00000330: 6e69 745f 5fa9 09da 085f 5f6e 616d 655f  nit__....__name_
```

### Comparing `pdme-1.2.0/pdme/measurement/__pycache__/input_types.cpython-39.pyc` & `pdme-1.3.0/pdme/measurement/__pycache__/input_types.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 1131 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 6b04 0000  a........D4fk...
+00000000: 610d 0d0a 0000 0000 92a3 4666 6b04 0000  a.........Ffk...
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
-00000230: 655f 312e 322e 302f 7064 6d65 2f6d 6561  e_1.2.0/pdme/mea
+00000230: 655f 312e 332e 302f 7064 6d65 2f6d 6561  e_1.3.0/pdme/mea
 00000240: 7375 7265 6d65 6e74 2f69 6e70 7574 5f74  surement/input_t
 00000250: 7970 6573 2e70 79da 0a3c 6c69 7374 636f  ypes.py..<listco
 00000260: 6d70 3e0d 0000 00f3 0000 0000 7a27 646f  mp>.........z'do
 00000270: 745f 696e 7075 7473 5f74 6f5f 6172 7261  t_inputs_to_arra
 00000280: 792e 3c6c 6f63 616c 733e 2e3c 6c69 7374  y.<locals>.<list
 00000290: 636f 6d70 3ea9 0272 0b00 0000 720d 0000  comp>..r....r...
 000002a0: 0029 0172 0700 0000 7211 0000 0072 1100  .).r....r....r..
```

### Comparing `pdme-1.2.0/pdme/measurement/__pycache__/oscillating_dipole.cpython-39.pyc` & `pdme-1.3.0/pdme/measurement/__pycache__/oscillating_dipole.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 6903 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 f71a 0000  a........D4f....
+00000000: 610d 0d0a 0000 0000 92a3 4666 f71a 0000  a.........Ff....
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
-00000440: 6d65 5f31 2e32 2e30 2f70 646d 652f 6d65  me_1.2.0/pdme/me
+00000440: 6d65 5f31 2e33 2e30 2f70 646d 652f 6d65  me_1.3.0/pdme/me
 00000450: 6173 7572 656d 656e 742f 6f73 6369 6c6c  asurement/oscill
 00000460: 6174 696e 675f 6469 706f 6c65 2e70 79da  ating_dipole.py.
 00000470: 0d5f 5f70 6f73 745f 696e 6974 5f5f 2300  .__post_init__#.
 00000480: 0000 7304 0000 0000 040e 017a 1f4f 7363  ..s........z.Osc
 00000490: 696c 6c61 7469 6e67 4469 706f 6c65 2e5f  illatingDipole._
 000004a0: 5f70 6f73 745f 696e 6974 5f5f 2902 da01  _post_init__)...
 000004b0: 7272 1000 0000 6302 0000 0000 0000 0000  rr....c.........
```

### Comparing `pdme-1.2.0/pdme/measurement/dot_measure.py` & `pdme-1.3.0/pdme/measurement/dot_measure.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/measurement/dot_pair_measure.py` & `pdme-1.3.0/pdme/measurement/dot_pair_measure.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/measurement/input_types.py` & `pdme-1.3.0/pdme/measurement/input_types.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/measurement/oscillating_dipole.py` & `pdme-1.3.0/pdme/measurement/oscillating_dipole.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/model/__init__.py` & `pdme-1.3.0/pdme/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/model/__pycache__/__init__.cpython-39.pyc` & `pdme-1.3.0/pdme/model/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 1066 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 2a04 0000  a........D4f*...
+00000000: 610d 0d0a 0000 0000 92a3 4666 2a04 0000  a.........Ff*...
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
-000003a0: 2e32 2e30 2f70 646d 652f 6d6f 6465 6c2f  .2.0/pdme/model/
+000003a0: 2e33 2e30 2f70 646d 652f 6d6f 6465 6c2f  .3.0/pdme/model/
 000003b0: 5f5f 696e 6974 5f5f 2e70 79da 083c 6d6f  __init__.py..<mo
 000003c0: 6475 6c65 3e01 0000 0073 0e00 0000 0c01  dule>....s......
 000003d0: 0c01 0c03 0c04 0c04 0c04 0c04            ............
```

### Comparing `pdme-1.2.0/pdme/model/__pycache__/fixed_magnitude_model.cpython-39.pyc` & `pdme-1.3.0/pdme/model/__pycache__/fixed_magnitude_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 2367 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 3f09 0000  a........D4f?...
+00000000: 610d 0d0a 0000 0000 92a3 4666 3f09 0000  a.........Ff?...
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
-00000330: 7068 7973 6963 735f 7064 6d65 5f31 2e32  physics_pdme_1.2
+00000330: 7068 7973 6963 735f 7064 6d65 5f31 2e33  physics_pdme_1.3
 00000340: 2e30 2f70 646d 652f 6d6f 6465 6c2f 6669  .0/pdme/model/fi
 00000350: 7865 645f 6d61 676e 6974 7564 655f 6d6f  xed_magnitude_mo
 00000360: 6465 6c2e 7079 da08 5f5f 696e 6974 5f5f  del.py..__init__
 00000370: 1400 0000 7310 0000 0000 0a06 0106 0106  ....s...........
 00000380: 0106 0106 0106 0106 017a 2853 696e 676c  .........z(Singl
 00000390: 6544 6970 6f6c 6546 6978 6564 4d61 676e  eDipoleFixedMagn
 000003a0: 6974 7564 654d 6f64 656c 2e5f 5f69 6e69  itudeModel.__ini
```

### Comparing `pdme-1.2.0/pdme/model/__pycache__/log_spaced_random_choice_fixed_orientation_model.cpython-39.pyc` & `pdme-1.3.0/pdme/model/__pycache__/log_spaced_random_choice_fixed_orientation_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 5158 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 2614 0000  a........D4f&...
+00000000: 610d 0d0a 0000 0000 92a3 4666 2614 0000  a.........Ff&...
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
-00000710: 6373 5f70 646d 655f 312e 322e 302f 7064  cs_pdme_1.2.0/pd
+00000710: 6373 5f70 646d 655f 312e 332e 302f 7064  cs_pdme_1.3.0/pd
 00000720: 6d65 2f6d 6f64 656c 2f6c 6f67 5f73 7061  me/model/log_spa
 00000730: 6365 645f 7261 6e64 6f6d 5f63 686f 6963  ced_random_choic
 00000740: 655f 6669 7865 645f 6f72 6965 6e74 6174  e_fixed_orientat
 00000750: 696f 6e5f 6d6f 6465 6c2e 7079 da08 5f5f  ion_model.py..__
 00000760: 696e 6974 5f5f 2d00 0000 732c 0000 0000  init__-...s,....
 00000770: 1006 0106 0106 0106 0106 0106 0106 0106  ................
 00000780: 0106 0106 0106 010c 0106 021e 011e 0112  ................
```

### Comparing `pdme-1.2.0/pdme/model/__pycache__/log_spaced_random_choice_model.cpython-39.pyc` & `pdme-1.3.0/pdme/model/__pycache__/log_spaced_random_choice_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 5332 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 d414 0000  a........D4f....
+00000000: 610d 0d0a 0000 0000 92a3 4666 d414 0000  a.........Ff....
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
-00000570: 6879 7369 6373 5f70 646d 655f 312e 322e  hysics_pdme_1.2.
+00000570: 6879 7369 6373 5f70 646d 655f 312e 332e  hysics_pdme_1.3.
 00000580: 302f 7064 6d65 2f6d 6f64 656c 2f6c 6f67  0/pdme/model/log
 00000590: 5f73 7061 6365 645f 7261 6e64 6f6d 5f63  _spaced_random_c
 000005a0: 686f 6963 655f 6d6f 6465 6c2e 7079 da08  hoice_model.py..
 000005b0: 5f5f 696e 6974 5f5f 2000 0000 7320 0000  __init__ ...s ..
 000005c0: 0000 0e06 0106 0106 0106 0106 0106 0106  ................
 000005d0: 0106 0106 010c 0106 0110 0102 0108 ff04  ................
 000005e0: 037a 3e4c 6f67 5370 6163 6564 5261 6e64  .z>LogSpacedRand
```

### Comparing `pdme-1.2.0/pdme/model/__pycache__/log_spaced_random_choice_xy_model.cpython-39.pyc` & `pdme-1.3.0/pdme/model/__pycache__/log_spaced_random_choice_xy_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 4699 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 5b12 0000  a........D4f[...
+00000000: 610d 0d0a 0000 0000 92a3 4666 5b12 0000  a.........Ff[...
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
-00000580: 7369 6373 5f70 646d 655f 312e 322e 302f  sics_pdme_1.2.0/
+00000580: 7369 6373 5f70 646d 655f 312e 332e 302f  sics_pdme_1.3.0/
 00000590: 7064 6d65 2f6d 6f64 656c 2f6c 6f67 5f73  pdme/model/log_s
 000005a0: 7061 6365 645f 7261 6e64 6f6d 5f63 686f  paced_random_cho
 000005b0: 6963 655f 7879 5f6d 6f64 656c 2e70 79da  ice_xy_model.py.
 000005c0: 085f 5f69 6e69 745f 5f20 0000 0073 2000  .__init__ ...s .
 000005d0: 0000 000e 0601 0601 0601 0601 0601 0601  ................
 000005e0: 0601 0601 0601 0c01 0601 1001 0201 08ff  ................
 000005f0: 0403 7a40 4c6f 6753 7061 6365 6452 616e  ..z@LogSpacedRan
```

### Comparing `pdme-1.2.0/pdme/model/__pycache__/model.cpython-39.pyc` & `pdme-1.3.0/pdme/model/__pycache__/model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 3594 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 0a0e 0000  a........D4f....
+00000000: 610d 0d0a 0000 0000 92a3 4666 0a0e 0000  a.........Ff....
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
-00000410: 655f 312e 322e 302f 7064 6d65 2f6d 6f64  e_1.2.0/pdme/mod
+00000410: 655f 312e 332e 302f 7064 6d65 2f6d 6f64  e_1.3.0/pdme/mod
 00000420: 656c 2f6d 6f64 656c 2e70 79da 0b67 6574  el/model.py..get
 00000430: 5f64 6970 6f6c 6573 1300 0000 7302 0000  _dipoles....s...
 00000440: 0000 087a 1744 6970 6f6c 654d 6f64 656c  ...z.DipoleModel
 00000450: 2e67 6574 5f64 6970 6f6c 6573 2904 da01  .get_dipoles)...
 00000460: 6e72 0700 0000 7208 0000 0072 0900 0000  nr....r....r....
 00000470: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
 00000480: 0001 0000 0043 0000 0073 0800 0000 7400  .....C...s....t.
```

### Comparing `pdme-1.2.0/pdme/model/__pycache__/multidipole_fixed_magnitude_model.cpython-39.pyc` & `pdme-1.3.0/pdme/model/__pycache__/multidipole_fixed_magnitude_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 2560 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 000a 0000  a........D4f....
+00000000: 610d 0d0a 0000 0000 92a3 4666 000a 0000  a.........Ff....
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
-00000370: 6963 735f 7064 6d65 5f31 2e32 2e30 2f70  ics_pdme_1.2.0/p
+00000370: 6963 735f 7064 6d65 5f31 2e33 2e30 2f70  ics_pdme_1.3.0/p
 00000380: 646d 652f 6d6f 6465 6c2f 6d75 6c74 6964  dme/model/multid
 00000390: 6970 6f6c 655f 6669 7865 645f 6d61 676e  ipole_fixed_magn
 000003a0: 6974 7564 655f 6d6f 6465 6c2e 7079 da08  itude_model.py..
 000003b0: 5f5f 696e 6974 5f5f 1700 0000 7312 0000  __init__....s...
 000003c0: 0000 0b06 0106 0106 0106 0106 0106 0106  ................
 000003d0: 010c 017a 2a4d 756c 7469 706c 6544 6970  ...z*MultipleDip
 000003e0: 6f6c 6546 6978 6564 4d61 676e 6974 7564  oleFixedMagnitud
```

### Comparing `pdme-1.2.0/pdme/model/__pycache__/random_count_multidipole_fixed_magnitude_model.cpython-39.pyc` & `pdme-1.3.0/pdme/model/__pycache__/random_count_multidipole_fixed_magnitude_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 3076 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 040c 0000  a........D4f....
+00000000: 610d 0d0a 0000 0000 92a3 4666 040c 0000  a.........Ff....
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
-00000470: 7064 6d65 5f31 2e32 2e30 2f70 646d 652f  pdme_1.2.0/pdme/
+00000470: 7064 6d65 5f31 2e33 2e30 2f70 646d 652f  pdme_1.3.0/pdme/
 00000480: 6d6f 6465 6c2f 7261 6e64 6f6d 5f63 6f75  model/random_cou
 00000490: 6e74 5f6d 756c 7469 6469 706f 6c65 5f66  nt_multidipole_f
 000004a0: 6978 6564 5f6d 6167 6e69 7475 6465 5f6d  ixed_magnitude_m
 000004b0: 6f64 656c 2e70 79da 085f 5f69 6e69 745f  odel.py..__init_
 000004c0: 5f1a 0000 0073 1c00 0000 000c 0601 0601  _....s..........
 000004d0: 0601 0601 0601 0601 0601 0c01 0601 1001  ................
 000004e0: 0201 08ff 0403 7a35 5261 6e64 6f6d 436f  ......z5RandomCo
```

### Comparing `pdme-1.2.0/pdme/model/fixed_magnitude_model.py` & `pdme-1.3.0/pdme/model/fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/model/log_spaced_random_choice_fixed_orientation_model.py` & `pdme-1.3.0/pdme/model/log_spaced_random_choice_fixed_orientation_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/model/log_spaced_random_choice_model.py` & `pdme-1.3.0/pdme/model/log_spaced_random_choice_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/model/log_spaced_random_choice_xy_model.py` & `pdme-1.3.0/pdme/model/log_spaced_random_choice_xy_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/model/model.py` & `pdme-1.3.0/pdme/model/model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/model/multidipole_fixed_magnitude_model.py` & `pdme-1.3.0/pdme/model/multidipole_fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/model/random_count_multidipole_fixed_magnitude_model.py` & `pdme-1.3.0/pdme/model/random_count_multidipole_fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/subspace_simulation/__init__.py` & `pdme-1.3.0/pdme/subspace_simulation/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,19 +37,38 @@
 
 
 def sort_array_of_dipoles_by_frequency(configuration) -> numpy.ndarray:
 	"""
 	Say we have a situation of 2 dipoles, and we've created 8 samples. Then we'll have an (8, 2, 7) numpy array.
 	For each of the 8 samples, we want the 2 dipoles to be in order of frequency.
 
+	This just sorts each sample, the 2x7 array.
+
 	Utility function.
 	"""
 	return numpy.array(sorted(configuration, key=lambda l: l[6]))
 
 
+def sort_array_of_dipoleses_by_frequency(configurations) -> numpy.ndarray:
+	"""
+	Say we have a situation of 2 dipoles, and we've created 8 samples. Then we'll have an (8, 2, 7) numpy array.
+	For each of the 8 samples, we want the 2 dipoles to be in order of frequency.
+
+	This is the wrapper that sorts everything.
+
+	Utility function.
+	"""
+	return numpy.array(
+		[
+			sort_array_of_dipoles_by_frequency(configuration)
+			for configuration in configurations
+		]
+	)
+
+
 __all__ = [
 	"DipoleStandardDeviation",
 	"MCMCStandardDeviation",
 	"sort_array_of_dipoles_by_frequency",
 	"proportional_cost",
 	"proportional_costs_vs_actual_measurement",
 ]
```

### Comparing `pdme-1.2.0/pdme/subspace_simulation/__pycache__/__init__.cpython-39.pyc` & `pdme-1.3.0/pdme/subspace_simulation/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 1364 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,134 +1,176 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 5405 0000  a........D4fT...
+00000000: 610d 0d0a 0000 0000 92a3 4666 5307 0000  a.........FfS...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
+00000020: 0004 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a04 6400  m.Z...d.d.l.Z.d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6501  d.l.m.Z.m.Z...e.
 00000060: 4700 6405 6406 8400 6406 8302 8301 5a08  G.d.d...d.....Z.
 00000070: 4700 6407 6408 8400 6408 8302 5a09 6504  G.d.d...d...Z.e.
-00000080: 6a0a 6409 9c01 640a 640b 8404 5a0b 6700  j.d...d.d...Z.g.
-00000090: 640c a201 5a0c 6403 5300 290d e900 0000  d...Z.d.S.).....
-000000a0: 0029 01da 0964 6174 6163 6c61 7373 2901  .)...dataclass).
-000000b0: da08 5365 7175 656e 6365 4e29 02da 1170  ..SequenceN)...p
-000000c0: 726f 706f 7274 696f 6e61 6c5f 636f 7374  roportional_cost
-000000d0: da28 7072 6f70 6f72 7469 6f6e 616c 5f63  .(proportional_c
-000000e0: 6f73 7473 5f76 735f 6163 7475 616c 5f6d  osts_vs_actual_m
-000000f0: 6561 7375 7265 6d65 6e74 6300 0000 0000  easurementc.....
-00000100: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00000110: 0000 0073 4200 0000 6500 5a01 6400 5a02  ...sB...e.Z.d.Z.
-00000120: 5500 6401 5a03 6504 6505 6402 3c00 6504  U.d.Z.e.e.d.<.e.
-00000130: 6505 6403 3c00 6504 6505 6404 3c00 6504  e.d.<.e.e.d.<.e.
-00000140: 6505 6405 3c00 6504 6505 6406 3c00 6504  e.d.<.e.e.d.<.e.
-00000150: 6505 6407 3c00 6408 5300 2909 da17 4469  e.d.<.d.S.)...Di
-00000160: 706f 6c65 5374 616e 6461 7264 4465 7669  poleStandardDevi
-00000170: 6174 696f 6e7a 5f0a 0963 6f6e 7461 696e  ationz_..contain
-00000180: 7320 7468 6520 6469 706f 6c65 2073 7461  s the dipole sta
-00000190: 6e64 6172 6420 6465 7669 6174 696f 6e20  ndard deviation 
-000001a0: 746f 2062 6520 7573 6564 2069 6e20 706f  to be used in po
-000001b0: 7270 6f73 616c 7320 666f 7220 6d61 726b  rposals for mark
-000001c0: 6f76 2063 6861 696e 206d 6f6e 7465 2063  ov chain monte c
-000001d0: 6172 6c6f 0a09 5a0a 705f 7068 695f 7374  arlo..Z.p_phi_st
-000001e0: 6570 5a0c 705f 7468 6574 615f 7374 6570  epZ.p_theta_step
-000001f0: 5a07 7278 5f73 7465 705a 0772 795f 7374  Z.rx_stepZ.ry_st
-00000200: 6570 5a07 727a 5f73 7465 705a 0a77 5f6c  epZ.rz_stepZ.w_l
-00000210: 6f67 5f73 7465 704e 2906 da08 5f5f 6e61  og_stepN)...__na
-00000220: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000230: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00000240: 5f5f 646f 635f 5fda 0566 6c6f 6174 da0f  __doc__..float..
-00000250: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5fa9  __annotations__.
-00000260: 0072 0d00 0000 720d 0000 00fa 5b2f 686f  .r....r.....[/ho
-00000270: 6d65 2f6a 656e 6b69 6e73 2f61 6765 6e74  me/jenkins/agent
-00000280: 2f77 6f72 6b73 7061 6365 2f67 6974 6561  /workspace/gitea
-00000290: 2d70 6879 7369 6373 5f70 646d 655f 312e  -physics_pdme_1.
-000002a0: 322e 302f 7064 6d65 2f73 7562 7370 6163  2.0/pdme/subspac
-000002b0: 655f 7369 6d75 6c61 7469 6f6e 2f5f 5f69  e_simulation/__i
-000002c0: 6e69 745f 5f2e 7079 7206 0000 000a 0000  nit__.pyr.......
-000002d0: 0073 0e00 0000 0a02 0404 0801 0801 0801  .s..............
-000002e0: 0801 0801 7206 0000 0063 0000 0000 0000  ....r....c......
-000002f0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00000300: 0000 732a 0000 0065 005a 0164 005a 0264  ..s*...e.Z.d.Z.d
-00000310: 015a 0365 0465 0519 0064 029c 0164 0364  .Z.e.e...d...d.d
-00000320: 0484 045a 0664 0564 0684 005a 0764 0753  ...Z.d.d...Z.d.S
-00000330: 0029 08da 154d 434d 4353 7461 6e64 6172  .)...MCMCStandar
-00000340: 6444 6576 6961 7469 6f6e 7a4e 0a09 7772  dDeviationzN..wr
-00000350: 6170 7065 7220 666f 7220 6d75 6c74 6970  apper for multip
-00000360: 6c65 2073 7461 6e64 6172 6420 6465 7669  le standard devi
-00000370: 6174 696f 6e73 2c20 616c 6c6f 7773 2066  ations, allows f
-00000380: 6f72 2066 6c65 7869 626c 6520 6c65 6e67  or flexible leng
-00000390: 7468 2073 7475 6666 0a09 2901 da06 7374  th stuff..)...st
-000003a0: 6465 7673 6302 0000 0000 0000 0000 0000  devsc...........
-000003b0: 0002 0000 0004 0000 0043 0000 0073 2600  .........C...s&.
-000003c0: 0000 7c01 7c00 5f00 7401 7c01 8301 6401  ..|.|._.t.|...d.
-000003d0: 6b00 7222 7402 6402 7c01 9b00 6403 9d03  k.r"t.d.|...d...
-000003e0: 8301 8201 6400 5300 2904 4ee9 0100 0000  ....d.S.).N.....
-000003f0: 7a0c 476f 7420 7374 6465 7673 3a20 7a16  z.Got stdevs: z.
-00000400: 2c20 6d75 7374 2068 6176 6520 6c65 6e67  , must have leng
-00000410: 7468 203e 2031 2903 7210 0000 00da 036c  th > 1).r......l
-00000420: 656e da0a 5661 6c75 6545 7272 6f72 2902  en..ValueError).
-00000430: da04 7365 6c66 7210 0000 0072 0d00 0000  ..selfr....r....
-00000440: 720d 0000 0072 0e00 0000 da08 5f5f 696e  r....r......__in
-00000450: 6974 5f5f 1d00 0000 7306 0000 0000 0106  it__....s.......
-00000460: 010c 017a 1e4d 434d 4353 7461 6e64 6172  ...z.MCMCStandar
-00000470: 6444 6576 6961 7469 6f6e 2e5f 5f69 6e69  dDeviation.__ini
-00000480: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
-00000490: 0300 0000 0300 0000 4300 0000 7318 0000  ........C...s...
-000004a0: 007c 0174 007c 006a 0183 0116 007d 027c  .|.t.|.j.....}.|
-000004b0: 006a 017c 0219 0053 0029 014e 2902 7212  .j.|...S.).N).r.
-000004c0: 0000 0072 1000 0000 2903 7214 0000 00da  ...r....).r.....
-000004d0: 036b 6579 5a06 6e65 776b 6579 720d 0000  .keyZ.newkeyr...
-000004e0: 0072 0d00 0000 720e 0000 00da 0b5f 5f67  .r....r......__g
-000004f0: 6574 6974 656d 5f5f 2200 0000 7304 0000  etitem__"...s...
-00000500: 0000 010e 017a 214d 434d 4353 7461 6e64  .....z!MCMCStand
-00000510: 6172 6444 6576 6961 7469 6f6e 2e5f 5f67  ardDeviation.__g
-00000520: 6574 6974 656d 5f5f 4e29 0872 0700 0000  etitem__N).r....
-00000530: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-00000540: 0300 0000 7206 0000 0072 1500 0000 7217  ....r....r....r.
-00000550: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
-00000560: 0000 720e 0000 0072 0f00 0000 1800 0000  ..r....r........
-00000570: 7306 0000 0008 0104 0412 0572 0f00 0000  s..........r....
-00000580: 2901 da06 7265 7475 726e 6301 0000 0000  )...returnc.....
-00000590: 0000 0000 0000 0001 0000 0006 0000 0043  ...............C
-000005a0: 0000 0073 1600 0000 7400 a001 7402 7c00  ...s....t...t.|.
-000005b0: 6401 6402 8400 6403 8d02 a101 5300 2904  d.d...d.....S.).
-000005c0: 7ad3 0a09 5361 7920 7765 2068 6176 6520  z...Say we have 
-000005d0: 6120 7369 7475 6174 696f 6e20 6f66 2032  a situation of 2
-000005e0: 2064 6970 6f6c 6573 2c20 616e 6420 7765   dipoles, and we
-000005f0: 2776 6520 6372 6561 7465 6420 3820 7361  've created 8 sa
-00000600: 6d70 6c65 732e 2054 6865 6e20 7765 276c  mples. Then we'l
-00000610: 6c20 6861 7665 2061 6e20 2838 2c20 322c  l have an (8, 2,
-00000620: 2037 2920 6e75 6d70 7920 6172 7261 792e   7) numpy array.
-00000630: 0a09 466f 7220 6561 6368 206f 6620 7468  ..For each of th
-00000640: 6520 3820 7361 6d70 6c65 732c 2077 6520  e 8 samples, we 
-00000650: 7761 6e74 2074 6865 2032 2064 6970 6f6c  want the 2 dipol
-00000660: 6573 2074 6f20 6265 2069 6e20 6f72 6465  es to be in orde
-00000670: 7220 6f66 2066 7265 7175 656e 6379 2e0a  r of frequency..
-00000680: 0a09 5574 696c 6974 7920 6675 6e63 7469  ..Utility functi
-00000690: 6f6e 2e0a 0963 0100 0000 0000 0000 0000  on...c..........
-000006a0: 0000 0100 0000 0200 0000 5300 0000 7308  ..........S...s.
-000006b0: 0000 007c 0064 0119 0053 0029 024e e906  ...|.d...S.).N..
-000006c0: 0000 0072 0d00 0000 2901 da01 6c72 0d00  ...r....)...lr..
-000006d0: 0000 720d 0000 0072 0e00 0000 da08 3c6c  ..r....r......<l
-000006e0: 616d 6264 613e 2e00 0000 f300 0000 007a  ambda>.........z
-000006f0: 3473 6f72 745f 6172 7261 795f 6f66 5f64  4sort_array_of_d
-00000700: 6970 6f6c 6573 5f62 795f 6672 6571 7565  ipoles_by_freque
-00000710: 6e63 792e 3c6c 6f63 616c 733e 2e3c 6c61  ncy.<locals>.<la
-00000720: 6d62 6461 3e29 0172 1600 0000 2903 da05  mbda>).r....)...
-00000730: 6e75 6d70 79da 0561 7272 6179 da06 736f  numpy..array..so
-00000740: 7274 6564 2901 5a0d 636f 6e66 6967 7572  rted).Z.configur
-00000750: 6174 696f 6e72 0d00 0000 720d 0000 0072  ationr....r....r
-00000760: 0e00 0000 da22 736f 7274 5f61 7272 6179  ....."sort_array
-00000770: 5f6f 665f 6469 706f 6c65 735f 6279 5f66  _of_dipoles_by_f
-00000780: 7265 7175 656e 6379 2700 0000 7302 0000  requency'...s...
-00000790: 0000 0772 2000 0000 2905 7206 0000 0072  ...r ...).r....r
-000007a0: 0f00 0000 7220 0000 0072 0400 0000 7205  ....r ...r....r.
-000007b0: 0000 0029 0dda 0b64 6174 6163 6c61 7373  ...)...dataclass
-000007c0: 6573 7202 0000 00da 0674 7970 696e 6772  esr......typingr
-000007d0: 0300 0000 721d 0000 005a 2370 646d 652e  ....r....Z#pdme.
-000007e0: 7375 6273 7061 6365 5f73 696d 756c 6174  subspace_simulat
-000007f0: 696f 6e2e 6d63 6d63 5f63 6f73 7473 7204  ion.mcmc_costsr.
-00000800: 0000 0072 0500 0000 7206 0000 0072 0f00  ...r....r....r..
-00000810: 0000 da07 6e64 6172 7261 7972 2000 0000  ....ndarrayr ...
-00000820: da07 5f5f 616c 6c5f 5f72 0d00 0000 720d  ..__all__r....r.
-00000830: 0000 0072 0d00 0000 720e 0000 00da 083c  ...r....r......<
-00000840: 6d6f 6475 6c65 3e01 0000 0073 1000 0000  module>....s....
-00000850: 0c01 0c01 0801 1006 0201 100d 0e0f 100a  ................
+00000080: 6a0a 6409 9c01 640a 640b 8404 5a0b 6504  j.d...d.d...Z.e.
+00000090: 6a0a 6409 9c01 640c 640d 8404 5a0c 6700  j.d...d.d...Z.g.
+000000a0: 640e a201 5a0d 6403 5300 290f e900 0000  d...Z.d.S.).....
+000000b0: 0029 01da 0964 6174 6163 6c61 7373 2901  .)...dataclass).
+000000c0: da08 5365 7175 656e 6365 4e29 02da 1170  ..SequenceN)...p
+000000d0: 726f 706f 7274 696f 6e61 6c5f 636f 7374  roportional_cost
+000000e0: da28 7072 6f70 6f72 7469 6f6e 616c 5f63  .(proportional_c
+000000f0: 6f73 7473 5f76 735f 6163 7475 616c 5f6d  osts_vs_actual_m
+00000100: 6561 7375 7265 6d65 6e74 6300 0000 0000  easurementc.....
+00000110: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00000120: 0000 0073 4200 0000 6500 5a01 6400 5a02  ...sB...e.Z.d.Z.
+00000130: 5500 6401 5a03 6504 6505 6402 3c00 6504  U.d.Z.e.e.d.<.e.
+00000140: 6505 6403 3c00 6504 6505 6404 3c00 6504  e.d.<.e.e.d.<.e.
+00000150: 6505 6405 3c00 6504 6505 6406 3c00 6504  e.d.<.e.e.d.<.e.
+00000160: 6505 6407 3c00 6408 5300 2909 da17 4469  e.d.<.d.S.)...Di
+00000170: 706f 6c65 5374 616e 6461 7264 4465 7669  poleStandardDevi
+00000180: 6174 696f 6e7a 5f0a 0963 6f6e 7461 696e  ationz_..contain
+00000190: 7320 7468 6520 6469 706f 6c65 2073 7461  s the dipole sta
+000001a0: 6e64 6172 6420 6465 7669 6174 696f 6e20  ndard deviation 
+000001b0: 746f 2062 6520 7573 6564 2069 6e20 706f  to be used in po
+000001c0: 7270 6f73 616c 7320 666f 7220 6d61 726b  rposals for mark
+000001d0: 6f76 2063 6861 696e 206d 6f6e 7465 2063  ov chain monte c
+000001e0: 6172 6c6f 0a09 5a0a 705f 7068 695f 7374  arlo..Z.p_phi_st
+000001f0: 6570 5a0c 705f 7468 6574 615f 7374 6570  epZ.p_theta_step
+00000200: 5a07 7278 5f73 7465 705a 0772 795f 7374  Z.rx_stepZ.ry_st
+00000210: 6570 5a07 727a 5f73 7465 705a 0a77 5f6c  epZ.rz_stepZ.w_l
+00000220: 6f67 5f73 7465 704e 2906 da08 5f5f 6e61  og_stepN)...__na
+00000230: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000240: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
+00000250: 5f5f 646f 635f 5fda 0566 6c6f 6174 da0f  __doc__..float..
+00000260: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5fa9  __annotations__.
+00000270: 0072 0d00 0000 720d 0000 00fa 5b2f 686f  .r....r.....[/ho
+00000280: 6d65 2f6a 656e 6b69 6e73 2f61 6765 6e74  me/jenkins/agent
+00000290: 2f77 6f72 6b73 7061 6365 2f67 6974 6561  /workspace/gitea
+000002a0: 2d70 6879 7369 6373 5f70 646d 655f 312e  -physics_pdme_1.
+000002b0: 332e 302f 7064 6d65 2f73 7562 7370 6163  3.0/pdme/subspac
+000002c0: 655f 7369 6d75 6c61 7469 6f6e 2f5f 5f69  e_simulation/__i
+000002d0: 6e69 745f 5f2e 7079 7206 0000 000a 0000  nit__.pyr.......
+000002e0: 0073 0e00 0000 0a02 0404 0801 0801 0801  .s..............
+000002f0: 0801 0801 7206 0000 0063 0000 0000 0000  ....r....c......
+00000300: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
+00000310: 0000 732a 0000 0065 005a 0164 005a 0264  ..s*...e.Z.d.Z.d
+00000320: 015a 0365 0465 0519 0064 029c 0164 0364  .Z.e.e...d...d.d
+00000330: 0484 045a 0664 0564 0684 005a 0764 0753  ...Z.d.d...Z.d.S
+00000340: 0029 08da 154d 434d 4353 7461 6e64 6172  .)...MCMCStandar
+00000350: 6444 6576 6961 7469 6f6e 7a4e 0a09 7772  dDeviationzN..wr
+00000360: 6170 7065 7220 666f 7220 6d75 6c74 6970  apper for multip
+00000370: 6c65 2073 7461 6e64 6172 6420 6465 7669  le standard devi
+00000380: 6174 696f 6e73 2c20 616c 6c6f 7773 2066  ations, allows f
+00000390: 6f72 2066 6c65 7869 626c 6520 6c65 6e67  or flexible leng
+000003a0: 7468 2073 7475 6666 0a09 2901 da06 7374  th stuff..)...st
+000003b0: 6465 7673 6302 0000 0000 0000 0000 0000  devsc...........
+000003c0: 0002 0000 0004 0000 0043 0000 0073 2600  .........C...s&.
+000003d0: 0000 7c01 7c00 5f00 7401 7c01 8301 6401  ..|.|._.t.|...d.
+000003e0: 6b00 7222 7402 6402 7c01 9b00 6403 9d03  k.r"t.d.|...d...
+000003f0: 8301 8201 6400 5300 2904 4ee9 0100 0000  ....d.S.).N.....
+00000400: 7a0c 476f 7420 7374 6465 7673 3a20 7a16  z.Got stdevs: z.
+00000410: 2c20 6d75 7374 2068 6176 6520 6c65 6e67  , must have leng
+00000420: 7468 203e 2031 2903 7210 0000 00da 036c  th > 1).r......l
+00000430: 656e da0a 5661 6c75 6545 7272 6f72 2902  en..ValueError).
+00000440: da04 7365 6c66 7210 0000 0072 0d00 0000  ..selfr....r....
+00000450: 720d 0000 0072 0e00 0000 da08 5f5f 696e  r....r......__in
+00000460: 6974 5f5f 1d00 0000 7306 0000 0000 0106  it__....s.......
+00000470: 010c 017a 1e4d 434d 4353 7461 6e64 6172  ...z.MCMCStandar
+00000480: 6444 6576 6961 7469 6f6e 2e5f 5f69 6e69  dDeviation.__ini
+00000490: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
+000004a0: 0300 0000 0300 0000 4300 0000 7318 0000  ........C...s...
+000004b0: 007c 0174 007c 006a 0183 0116 007d 027c  .|.t.|.j.....}.|
+000004c0: 006a 017c 0219 0053 0029 014e 2902 7212  .j.|...S.).N).r.
+000004d0: 0000 0072 1000 0000 2903 7214 0000 00da  ...r....).r.....
+000004e0: 036b 6579 5a06 6e65 776b 6579 720d 0000  .keyZ.newkeyr...
+000004f0: 0072 0d00 0000 720e 0000 00da 0b5f 5f67  .r....r......__g
+00000500: 6574 6974 656d 5f5f 2200 0000 7304 0000  etitem__"...s...
+00000510: 0000 010e 017a 214d 434d 4353 7461 6e64  .....z!MCMCStand
+00000520: 6172 6444 6576 6961 7469 6f6e 2e5f 5f67  ardDeviation.__g
+00000530: 6574 6974 656d 5f5f 4e29 0872 0700 0000  etitem__N).r....
+00000540: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00000550: 0300 0000 7206 0000 0072 1500 0000 7217  ....r....r....r.
+00000560: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
+00000570: 0000 720e 0000 0072 0f00 0000 1800 0000  ..r....r........
+00000580: 7306 0000 0008 0104 0412 0572 0f00 0000  s..........r....
+00000590: 2901 da06 7265 7475 726e 6301 0000 0000  )...returnc.....
+000005a0: 0000 0000 0000 0001 0000 0006 0000 0043  ...............C
+000005b0: 0000 0073 1600 0000 7400 a001 7402 7c00  ...s....t...t.|.
+000005c0: 6401 6402 8400 6403 8d02 a101 5300 2904  d.d...d.....S.).
+000005d0: 6101 0100 000a 0953 6179 2077 6520 6861  a......Say we ha
+000005e0: 7665 2061 2073 6974 7561 7469 6f6e 206f  ve a situation o
+000005f0: 6620 3220 6469 706f 6c65 732c 2061 6e64  f 2 dipoles, and
+00000600: 2077 6527 7665 2063 7265 6174 6564 2038   we've created 8
+00000610: 2073 616d 706c 6573 2e20 5468 656e 2077   samples. Then w
+00000620: 6527 6c6c 2068 6176 6520 616e 2028 382c  e'll have an (8,
+00000630: 2032 2c20 3729 206e 756d 7079 2061 7272   2, 7) numpy arr
+00000640: 6179 2e0a 0946 6f72 2065 6163 6820 6f66  ay...For each of
+00000650: 2074 6865 2038 2073 616d 706c 6573 2c20   the 8 samples, 
+00000660: 7765 2077 616e 7420 7468 6520 3220 6469  we want the 2 di
+00000670: 706f 6c65 7320 746f 2062 6520 696e 206f  poles to be in o
+00000680: 7264 6572 206f 6620 6672 6571 7565 6e63  rder of frequenc
+00000690: 792e 0a0a 0954 6869 7320 6a75 7374 2073  y....This just s
+000006a0: 6f72 7473 2065 6163 6820 7361 6d70 6c65  orts each sample
+000006b0: 2c20 7468 6520 3278 3720 6172 7261 792e  , the 2x7 array.
+000006c0: 0a0a 0955 7469 6c69 7479 2066 756e 6374  ...Utility funct
+000006d0: 696f 6e2e 0a09 6301 0000 0000 0000 0000  ion...c.........
+000006e0: 0000 0001 0000 0002 0000 0053 0000 0073  ...........S...s
+000006f0: 0800 0000 7c00 6401 1900 5300 2902 4ee9  ....|.d...S.).N.
+00000700: 0600 0000 720d 0000 0029 01da 016c 720d  ....r....)...lr.
+00000710: 0000 0072 0d00 0000 720e 0000 00da 083c  ...r....r......<
+00000720: 6c61 6d62 6461 3e30 0000 00f3 0000 0000  lambda>0........
+00000730: 7a34 736f 7274 5f61 7272 6179 5f6f 665f  z4sort_array_of_
+00000740: 6469 706f 6c65 735f 6279 5f66 7265 7175  dipoles_by_frequ
+00000750: 656e 6379 2e3c 6c6f 6361 6c73 3e2e 3c6c  ency.<locals>.<l
+00000760: 616d 6264 613e 2901 7216 0000 0029 03da  ambda>).r....)..
+00000770: 056e 756d 7079 da05 6172 7261 79da 0673  .numpy..array..s
+00000780: 6f72 7465 6429 01da 0d63 6f6e 6669 6775  orted)...configu
+00000790: 7261 7469 6f6e 720d 0000 0072 0d00 0000  rationr....r....
+000007a0: 720e 0000 00da 2273 6f72 745f 6172 7261  r....."sort_arra
+000007b0: 795f 6f66 5f64 6970 6f6c 6573 5f62 795f  y_of_dipoles_by_
+000007c0: 6672 6571 7565 6e63 7927 0000 0073 0200  frequency'...s..
+000007d0: 0000 0009 7221 0000 0063 0100 0000 0000  ....r!...c......
+000007e0: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+000007f0: 0000 7314 0000 0074 00a0 0164 0164 0284  ..s....t...d.d..
+00000800: 007c 0044 0083 01a1 0153 0029 0361 0001  .|.D.....S.).a..
+00000810: 0000 0a09 5361 7920 7765 2068 6176 6520  ....Say we have 
+00000820: 6120 7369 7475 6174 696f 6e20 6f66 2032  a situation of 2
+00000830: 2064 6970 6f6c 6573 2c20 616e 6420 7765   dipoles, and we
+00000840: 2776 6520 6372 6561 7465 6420 3820 7361  've created 8 sa
+00000850: 6d70 6c65 732e 2054 6865 6e20 7765 276c  mples. Then we'l
+00000860: 6c20 6861 7665 2061 6e20 2838 2c20 322c  l have an (8, 2,
+00000870: 2037 2920 6e75 6d70 7920 6172 7261 792e   7) numpy array.
+00000880: 0a09 466f 7220 6561 6368 206f 6620 7468  ..For each of th
+00000890: 6520 3820 7361 6d70 6c65 732c 2077 6520  e 8 samples, we 
+000008a0: 7761 6e74 2074 6865 2032 2064 6970 6f6c  want the 2 dipol
+000008b0: 6573 2074 6f20 6265 2069 6e20 6f72 6465  es to be in orde
+000008c0: 7220 6f66 2066 7265 7175 656e 6379 2e0a  r of frequency..
+000008d0: 0a09 5468 6973 2069 7320 7468 6520 7772  ..This is the wr
+000008e0: 6170 7065 7220 7468 6174 2073 6f72 7473  apper that sorts
+000008f0: 2065 7665 7279 7468 696e 672e 0a0a 0955   everything....U
+00000900: 7469 6c69 7479 2066 756e 6374 696f 6e2e  tility function.
+00000910: 0a09 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00000920: 0000 0004 0000 0053 0000 0073 1400 0000  .......S...s....
+00000930: 6700 7c00 5d0c 7d01 7400 7c01 8301 9102  g.|.].}.t.|.....
+00000940: 7104 5300 720d 0000 0029 0172 2100 0000  q.S.r....).r!...
+00000950: 2902 da02 2e30 7220 0000 0072 0d00 0000  )....0r ...r....
+00000960: 720d 0000 0072 0e00 0000 da0a 3c6c 6973  r....r......<lis
+00000970: 7463 6f6d 703e 3d00 0000 7304 0000 0006  tcomp>=...s.....
+00000980: 0202 ff7a 3873 6f72 745f 6172 7261 795f  ...z8sort_array_
+00000990: 6f66 5f64 6970 6f6c 6573 6573 5f62 795f  of_dipoleses_by_
+000009a0: 6672 6571 7565 6e63 792e 3c6c 6f63 616c  frequency.<local
+000009b0: 733e 2e3c 6c69 7374 636f 6d70 3e29 0272  s>.<listcomp>).r
+000009c0: 1d00 0000 721e 0000 0029 015a 0e63 6f6e  ....r....).Z.con
+000009d0: 6669 6775 7261 7469 6f6e 7372 0d00 0000  figurationsr....
+000009e0: 720d 0000 0072 0e00 0000 da24 736f 7274  r....r.....$sort
+000009f0: 5f61 7272 6179 5f6f 665f 6469 706f 6c65  _array_of_dipole
+00000a00: 7365 735f 6279 5f66 7265 7175 656e 6379  ses_by_frequency
+00000a10: 3300 0000 730a 0000 0000 0904 0106 0202  3...s...........
+00000a20: fe04 ff72 2400 0000 2905 7206 0000 0072  ...r$...).r....r
+00000a30: 0f00 0000 7221 0000 0072 0400 0000 7205  ....r!...r....r.
+00000a40: 0000 0029 0eda 0b64 6174 6163 6c61 7373  ...)...dataclass
+00000a50: 6573 7202 0000 00da 0674 7970 696e 6772  esr......typingr
+00000a60: 0300 0000 721d 0000 005a 2370 646d 652e  ....r....Z#pdme.
+00000a70: 7375 6273 7061 6365 5f73 696d 756c 6174  subspace_simulat
+00000a80: 696f 6e2e 6d63 6d63 5f63 6f73 7473 7204  ion.mcmc_costsr.
+00000a90: 0000 0072 0500 0000 7206 0000 0072 0f00  ...r....r....r..
+00000aa0: 0000 da07 6e64 6172 7261 7972 2100 0000  ....ndarrayr!...
+00000ab0: 7224 0000 00da 075f 5f61 6c6c 5f5f 720d  r$.....__all__r.
+00000ac0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000ad0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000ae0: 7312 0000 000c 010c 0108 0110 0602 0110  s...............
+00000af0: 0d0e 0f10 0c10 11                        .......
```

### Comparing `pdme-1.2.0/pdme/subspace_simulation/__pycache__/mcmc_costs.cpython-39.pyc` & `pdme-1.3.0/pdme/subspace_simulation/__pycache__/mcmc_costs.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 575 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 3f02 0000  a........D4f?...
+00000000: 610d 0d0a 0000 0000 92a3 4666 3f02 0000  a.........Ff?...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6500 6a04 6500 6a04 6500  d.l.Z.e.j.e.j.e.
 00000050: 6a04 6402 9c03 6403 6404 8404 5a05 6500  j.d...d.d...Z.e.
 00000060: 6a04 6500 6a04 6500 6a04 6500 6a04 6405  j.e.j.e.j.e.j.d.
 00000070: 9c04 6406 6407 8404 5a06 6401 5300 2908  ..d.d...Z.d.S.).
@@ -16,15 +16,15 @@
 000000f0: 6178 6973 2903 da05 6e75 6d70 79da 036d  axis)...numpy..m
 00000100: 6178 da07 6d61 7869 6d75 6d29 0472 0200  ax..maximum).r..
 00000110: 0000 7203 0000 005a 0474 6f70 735a 0762  ..r....Z.topsZ.b
 00000120: 6f74 746f 6d73 a900 720a 0000 00fa 5d2f  ottoms..r.....]/
 00000130: 686f 6d65 2f6a 656e 6b69 6e73 2f61 6765  home/jenkins/age
 00000140: 6e74 2f77 6f72 6b73 7061 6365 2f67 6974  nt/workspace/git
 00000150: 6561 2d70 6879 7369 6373 5f70 646d 655f  ea-physics_pdme_
-00000160: 312e 322e 302f 7064 6d65 2f73 7562 7370  1.2.0/pdme/subsp
+00000160: 312e 332e 302f 7064 6d65 2f73 7562 7370  1.3.0/pdme/subsp
 00000170: 6163 655f 7369 6d75 6c61 7469 6f6e 2f6d  ace_simulation/m
 00000180: 636d 635f 636f 7374 732e 7079 da11 7072  cmc_costs.py..pr
 00000190: 6f70 6f72 7469 6f6e 616c 5f63 6f73 7406  oportional_cost.
 000001a0: 0000 0073 0600 0000 0001 1201 1201 720c  ...s..........r.
 000001b0: 0000 0029 04da 1064 6f74 5f69 6e70 7574  ...)...dot_input
 000001c0: 735f 6172 7261 79da 1861 6374 7561 6c5f  s_array..actual_
 000001d0: 6d65 6173 7572 656d 656e 745f 6172 7261  measurement_arra
```

### Comparing `pdme-1.2.0/pdme/subspace_simulation/mcmc_costs.py` & `pdme-1.3.0/pdme/subspace_simulation/mcmc_costs.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/util/__pycache__/fast_nonlocal_spectrum.cpython-39.pyc` & `pdme-1.3.0/pdme/util/__pycache__/fast_nonlocal_spectrum.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 9670 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 c625 0000  a........D4f.%..
+00000000: 610d 0d0a 0000 0000 92a3 4666 c625 0000  a.........Ff.%..
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
-000004f0: 6373 5f70 646d 655f 312e 322e 302f 7064  cs_pdme_1.2.0/pd
+000004f0: 6373 5f70 646d 655f 312e 332e 302f 7064  cs_pdme_1.3.0/pd
 00000500: 6d65 2f75 7469 6c2f 6661 7374 5f6e 6f6e  me/util/fast_non
 00000510: 6c6f 6361 6c5f 7370 6563 7472 756d 2e70  local_spectrum.p
 00000520: 79da 0f66 6173 745f 735f 6e6f 6e6c 6f63  y..fast_s_nonloc
 00000530: 616c 0800 0000 733e 0000 0000 0614 0114  al....s>........
 00000540: 0110 0210 0110 0110 0216 0116 0112 0112  ................
 00000550: 020c 010e 0214 0114 010e 0110 0110 0214  ................
 00000560: 0114 010e 0110 0110 0212 0112 010e 0110  ................
```

### Comparing `pdme-1.2.0/pdme/util/__pycache__/fast_v_calc.cpython-39.pyc` & `pdme-1.3.0/pdme/util/__pycache__/fast_v_calc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 01:57:25 2024 UTC, .py size: 7195 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8544 3466 1b1c 0000  a........D4f....
+00000000: 610d 0d0a 0000 0000 92a3 4666 1b1c 0000  a.........Ff....
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
-00000410: 735f 7064 6d65 5f31 2e32 2e30 2f70 646d  s_pdme_1.2.0/pdm
+00000410: 735f 7064 6d65 5f31 2e33 2e30 2f70 646d  s_pdme_1.3.0/pdm
 00000420: 652f 7574 696c 2f66 6173 745f 765f 6361  e/util/fast_v_ca
 00000430: 6c63 2e70 79da 1366 6173 745f 7673 5f66  lc.py..fast_vs_f
 00000440: 6f72 5f64 6970 6f6c 6573 0800 0000 7322  or_dipoles....s"
 00000450: 0000 0000 0d14 0114 0210 0210 0110 0110  ................
 00000460: 0314 0210 0414 0210 0214 0110 0216 0110  ................
 00000470: 0436 0210 0272 2500 0000 2903 7202 0000  .6...r%...).r...
 00000480: 00da 0964 6970 6f6c 6573 6573 7204 0000  ...dipolesesr...
```

### Comparing `pdme-1.2.0/pdme/util/fast_nonlocal_spectrum.py` & `pdme-1.3.0/pdme/util/fast_nonlocal_spectrum.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pdme/util/fast_v_calc.py` & `pdme-1.3.0/pdme/util/fast_v_calc.py`

 * *Files identical despite different names*

### Comparing `pdme-1.2.0/pyproject.toml` & `pdme-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdme"
-version = "1.2.0"
+version = "1.3.0"
 description = "Python dipole model evaluator"
 authors = ["Deepak <dmallubhotla+github@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
```

### Comparing `pdme-1.2.0/PKG-INFO` & `pdme-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdme
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python dipole model evaluator
 License: GPL-3.0-only
 Author: Deepak
 Author-email: dmallubhotla+github@gmail.com
 Requires-Python: >=3.8.1,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

