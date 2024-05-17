# Comparing `tmp/vbelt-0.7.5.tar.gz` & `tmp/vbelt-0.8.1.tar.gz`

## Comparing `vbelt-0.7.5.tar` & `vbelt-0.8.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/__init__.py
--rwxr-xr-x   0        0        0     5623 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/charge_utils.py
--rwxr-xr-x   0        0        0    10595 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/coherence.py
--rwxr-xr-x   0        0        0     1421 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/forces.py
--rwxr-xr-x   0        0        0     8768 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/gencalc.py
--rwxr-xr-x   0        0        0     1197 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/incar.py
--rwxr-xr-x   0        0        0     6996 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/jobtool.py
--rwxr-xr-x   0        0        0     2416 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/kpoints.py
--rwxr-xr-x   0        0        0      144 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/logger.py
--rwxr-xr-x   0        0        0     4699 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/misc.py
--rwxr-xr-x   0        0        0     2946 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/outcar.py
--rwxr-xr-x   0        0        0     3551 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/outcar_utils.py
--rwxr-xr-x   0        0        0    11129 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/poscar.py
--rwxr-xr-x   0        0        0    17790 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/poscartool.py
--rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/potcar.py
--rwxr-xr-x   0        0        0    14455 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/script_utils.py
--rwxr-xr-x   0        0        0    13531 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/wrapper.py
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 vbelt-0.7.5/.gitignore
--rwxr-xr-x   0        0        0    14663 2020-02-02 00:00:00.000000 vbelt-0.7.5/LICENSE
--rwxr-xr-x   0        0        0     1284 2020-02-02 00:00:00.000000 vbelt-0.7.5/README.md
--rwxr-xr-x   0        0        0     1133 2020-02-02 00:00:00.000000 vbelt-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 vbelt-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/__init__.py
+-rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/charge_utils.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/chargetool.py
+-rw-r--r--   0        0        0    10595 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/coherence.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/forces.py
+-rw-r--r--   0        0        0     8768 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/gencalc.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/incar.py
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/jobtool.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/kpoints.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/logger.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/misc.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/outcar.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/outcar_utils.py
+-rw-r--r--   0        0        0    11129 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/poscar.py
+-rw-r--r--   0        0        0    17790 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/poscartool.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/potcar.py
+-rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/script_utils.py
+-rw-r--r--   0        0        0    11061 2020-02-02 00:00:00.000000 vbelt-0.8.1/vbelt/wrapper.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 vbelt-0.8.1/.gitignore
+-rw-r--r--   0        0        0    14663 2020-02-02 00:00:00.000000 vbelt-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 vbelt-0.8.1/README.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 vbelt-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 vbelt-0.8.1/PKG-INFO
```

### Comparing `vbelt-0.7.5/vbelt/charge_utils.py` & `vbelt-0.8.1/vbelt/charge_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from itertools import islice
 import numpy as np
 
 from .misc import prod, InvalidInput
 
 
 class Charge:
-    def __init__(self, poscar, chg, aug):
-        self.poscar = poscar
+    def __init__(self, raw_poscar, chg, aug):
+        self.raw_poscar = raw_poscar
         self.tot_chg = chg
         self.tot_aug = aug
         self.dif_part = None
         self.dif_nc_part = None
 
     def add_dif(self, chg, aug):
-        self.dif_part = Charge(self.poscar, chg, aug)
+        self.dif_part = Charge(self.raw_poscar, chg, aug)
 
     def add_nc_dif(self, x_dif, y_dif, z_dif):
         raise NotImplementedError("Non colinear density is not implemented yet.")
 
     @property
     def grid_shape(self):
         return self.tot_chg.shape
@@ -42,15 +42,15 @@
         if self.aug_shape and other.aug_shape:
             if self.aug_shape != other.aug_shape:
                 raise ValueError("Incompatible augmentation part shape.")
 
             for a, b in zip(self.tot_aug, other.tot_aug):
                 aug_sums.append(a + b)
 
-        chg_sum = Charge(self.poscar, self.tot_chg + other.tot_chg, aug_sums)
+        chg_sum = Charge(self.raw_poscar, self.tot_chg + other.tot_chg, aug_sums)
 
         if self.dif_part and other.dif_part:
             chg_sum.dif_part = self.dif_part + other.dif_part
         # TODO handle non colinear case
 
         return chg_sum
 
@@ -62,15 +62,15 @@
 
     def __rmul__(self, x):
         if not isinstance(x, (float, int, complex)):
             raise ValueError(
                 "Charge instance can only be multiplied by a numerical scalar."
             )
 
-        res = Charge(self.poscar, x * self.tot_chg, [x * e for e in self.tot_aug])
+        res = Charge(self.raw_poscar, x * self.tot_chg, [x * e for e in self.tot_aug])
 
         if self.dif_part:
             res.dif_part = x * self.dif_part
         # TODO handle non colinear case
 
         return res
 
@@ -82,31 +82,31 @@
 
         return (1.0 / x) * self
 
     def total_only(self):
         if self.dif_part is None and self.dif_nc_part is None:
             return self
 
-        return Charge(self.poscar, self.tot_chg, self.tot_aug)
+        return Charge(self.raw_poscar, self.tot_chg, self.tot_aug)
 
     @classmethod
-    def read_from(cls, file):
-        # Keep the poscar part in text form.
-        poscar = []
-        poscar.extend(islice(file, 6))
+    def from_file(cls, file):
+        # Keep the raw_poscar part in text form.
+        raw_poscar = []
+        raw_poscar.extend(islice(file, 6))
         head = next(file)
-        poscar.append(head)
+        raw_poscar.append(head)
 
         nlines = sum(map(int, head.split()))
 
-        poscar.extend(islice(file, nlines + 2))
+        raw_poscar.extend(islice(file, nlines + 2))
 
         (regular_sum, augmented_sum, after) = read_channel(file)
 
-        chg = cls(poscar, regular_sum, augmented_sum)
+        chg = cls(raw_poscar, regular_sum, augmented_sum)
 
         dif_data = []
 
         while after is not None:
             (regular_dif, augmented_dif, after) = read_channel(file, after)
 
             dif_data.append((regular_dif, augmented_dif))
@@ -116,22 +116,58 @@
             chg.add_dif(*dif_data[0])
         elif len(dif_data) == 3:
             # Non colinear spin
             chg.add_nc_dif(*dif_data)
 
         return chg
 
+    @classmethod
+    def from_dict(cls, data):
+        pass
+
+    def as_dict(self):
+        d = {
+            "raw_poscar": self.raw_poscar,
+            "tot_chg": self.tot_chg,
+            "tot_aug": self.tot_aug,
+        }
+
+        if self.dif_part:
+            ddif = self.dif_part.as_dict()
+
+            d.update({
+                "dif_" + k: v for k, v in ddif.items()
+            })
+        elif self.dif_nc_part:
+            raise NotImplementedError("Non colinear density is not implemented yet.")
+
+        return d
+
+    @classmethod
+    def from_npz(cls, file):
+        data = np.load(file)
+
+        return cls.from_dict(data)
+
     def write_to(self, file):
-        file.writelines(self.poscar)
+        file.writelines(self.raw_poscar)
 
         write_channel(file, self)
 
         if self.dif_part:
             write_channel(file, self.dif_part)
 
+    def write_npz(self, file, *, compress=False):
+        data = self.as_dict()
+
+        if compress:
+            np.savez_compressed(file, **data)
+        else:
+            np.savez(file, **data)
+
     def split(self):
         "Split the Charge object into a spin up and a spin down object."
         if self.dif_part is None:
             raise InvalidInput("No spin related data available.")
 
         return 0.5 * (self.total_only() + self.dif_part), 0.5 * (
             self.total_only() - self.dif_part
@@ -150,27 +186,29 @@
         if after[:24] != "augmentation occupancies":
             break
         i, n = map(int, after[24:].split())
 
         proj_data = read_block(file, (n,))
 
         augmented_part.append(proj_data)
+        after = next(file, None)
 
     while after is not None and after != head_:
         after = next(file, None)
 
     return (regular_data, augmented_part, after)
 
 
 def read_block(file, shape):
     npts = prod(shape)
     line = next(file)
     l1 = line.split()
 
-    nlines = ceil(npts / len(l1) - 1.0)
+    # -1 because the first line has already been read
+    nlines = int(ceil(npts / len(l1))) - 1
 
     # While this can seem a stupid way of writing this, it is actually
     # pretty fast because:
     # - one huge split is much faster than thousands of small ones
     # - the string->float is delegated to numpy in a single call
     block = line + " " + " ".join(islice(file, nlines))
     return np.array(block.split(), dtype=float).reshape(shape)
@@ -180,16 +218,16 @@
     fmt = " {: >4d}" * len(chg.tot_chg.shape)
     file.write(fmt.format(*chg.tot_chg.shape) + "\n")
 
     line = chg.tot_chg.reshape((-1,))
 
     write_block(file, line, " %+16.11E", 5)
 
-    for i, d in chg.tot_aug:
-        file.write(f"augmentation part {i:>3} {len(d):>3}\n")
+    for i, d in enumerate(chg.tot_aug, start=1):
+        file.write(f"augmentation occupancies {i:>3} {len(d):>3}\n")
         write_block(file, d, " %+13.7E", 5)
 
 
 def write_block(file, data, fmt, stride):
     bound = stride * (len(data) // stride)
     well_shaped = data[:bound].reshape((-1, stride))
```

### Comparing `vbelt-0.7.5/vbelt/coherence.py` & `vbelt-0.8.1/vbelt/coherence.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.7.5/vbelt/forces.py` & `vbelt-0.8.1/vbelt/forces.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.7.5/vbelt/gencalc.py` & `vbelt-0.8.1/vbelt/gencalc.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.7.5/vbelt/incar.py` & `vbelt-0.8.1/vbelt/incar.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.7.5/vbelt/jobtool.py` & `vbelt-0.8.1/vbelt/jobtool.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.7.5/vbelt/kpoints.py` & `vbelt-0.8.1/vbelt/kpoints.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.7.5/vbelt/misc.py` & `vbelt-0.8.1/vbelt/misc.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.7.5/vbelt/outcar.py` & `vbelt-0.8.1/vbelt/outcar.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.7.5/vbelt/outcar_utils.py` & `vbelt-0.8.1/vbelt/outcar_utils.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.7.5/vbelt/poscar.py` & `vbelt-0.8.1/vbelt/poscar.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.7.5/vbelt/poscartool.py` & `vbelt-0.8.1/vbelt/poscartool.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.7.5/vbelt/potcar.py` & `vbelt-0.8.1/vbelt/potcar.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.7.5/vbelt/script_utils.py` & `vbelt-0.8.1/vbelt/script_utils.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.7.5/vbelt/wrapper.py` & `vbelt-0.8.1/vbelt/wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,111 +1,24 @@
 # vbelt: The VASP user toolbelt.
 # Copyright (C) 2023  Théo Cavignac
-import sys
 import os.path
 
 from .misc import naturaldelta
 
 from .script_utils import (
     script,
-    error,
     positional,
     flag,
     optional,
     error_catch,
     PerfCounterCollec,
 )
 
 
 @script(
-    positional("CHGCAR", help="file to extract data from"),
-    flag("--split", help="split CHGCAR into up and down channels"),
-    flag("--spin", help="extract the spin density"),
-    flag("--total", help="extract the total density"),
-    flag("--timing", help="show the timing informations"),
-)
-def charge_extract(opts):
-    from .charge_utils import Charge
-
-    pc = PerfCounterCollec()
-
-    with pc.reading:
-        if opts.chgcar == "-":
-            chg = Charge.from_file(sys.stdin)
-            name = "CHGCAR"
-        else:
-            with open(opts.chgcar) as f:
-                chg = Charge.read_from(f)
-            name = opts.chgcar
-
-    out_prefix, ext = os.path.splitext(name)
-
-    if opts.split:
-        if chg.dif_part is None:
-            error("There is no spin data available in the input file.")
-
-        with pc.processing:
-            up, down = chg.split()
-
-        with pc.writing, open(out_prefix + ".up" + ext, "w") as f:
-            up.write_to(f)
-
-        with pc.writing, open(out_prefix + ".down" + ext, "w") as f:
-            down.write_to(f)
-
-    elif opts.spin:
-        if chg.dif_part is None:
-            error("There is no spin data available in the input file.")
-
-        with pc.writing, open(out_prefix + ".spin" + ext, "w") as f:
-            chg.dif_part.write_to(f)
-
-    elif opts.total:
-        with pc.writing, open(out_prefix + ".total" + ext, "w") as f:
-            chg.total_only().write_to(f)
-
-    else:
-        error("No action required.")
-
-    if opts.timing:
-        print(pc.summary())
-
-
-@script(
-    positional("COEF_A", type=float, help="coeficient for the first file"),
-    positional("CHGCAR_A", help="first file to extract data from"),
-    positional("COEF_B", type=float, help="coeficient for the second file"),
-    positional("CHGCAR_B", help="second file to extract data from"),
-)
-def charge_combine(opts):
-    from .charge_utils import Charge
-
-    if opts.chgcar_a == "-":
-        chg_a = Charge.from_file(sys.stdin)
-        name = "CHGCAR"
-    else:
-        with open(opts.chgcar_a) as f:
-            chg_a = Charge.read_from(f)
-        name = opts.chgcar_a
-
-    prefix_out = name
-
-    if opts.chgcar_b == "-":
-        chg_b = Charge.from_file(sys.stdin)
-    else:
-        with open(opts.chgcar_b) as f:
-            chg_b = Charge.read_from(f)
-
-    chg_sum = opts.coef_a * chg_a + opts.coef_b * chg_b
-
-    with open(prefix_out + ".sum", "w") as f:
-        chg_sum.write_to(f)
-
-
-@script(
     positional("OUTCAR", default="OUTCAR", type=str, help="VASP output file"),
     optional(
         "--tol",
         type=float,
         default=None,
         help="Maximum converged force ampliture (A/eV)",
     ),
```

### Comparing `vbelt-0.7.5/LICENSE` & `vbelt-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vbelt-0.7.5/README.md` & `vbelt-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `vbelt-0.7.5/pyproject.toml` & `vbelt-0.8.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -26,21 +26,20 @@
     "tc-pysh>=0.2.0",
 ]
 symmetry = [
     "pymatgen",
 ]
 
 [project.scripts]
-chgsum = "vbelt.wrapper:charge_combine"
-chgx = "vbelt.wrapper:charge_extract"
 ckcoherence = "vbelt.wrapper:check_coherence"
 ckconv = "vbelt.wrapper:check_conv"
 ckend = "vbelt.wrapper:check_end"
 ckforces = "vbelt.wrapper:check_forces"
 jobtool = "vbelt.jobtool:jobtool"
+chgtool = "vbelt.chargetool:chargetool"
 poscartool = "vbelt.poscartool:poscartool"
 report = "vbelt.wrapper:report"
 termdos = "vbelt.wrapper:termdos"
 
 [project.urls]
 Homepage = "https://git.sr.ht/~lattay/vbelt"
```

### Comparing `vbelt-0.7.5/PKG-INFO` & `vbelt-0.8.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: vbelt
-Version: 0.7.5
+Version: 0.8.1
 Summary: The VASP user's tool belt.
 Project-URL: Homepage, https://git.sr.ht/~lattay/vbelt
 Author-email: Théo Cavignac <theo.cavignac@gmail.com>
 License-Expression: EUPL-1.2
 License-File: LICENSE
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.7
```

