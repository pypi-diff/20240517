# Comparing `tmp/paicorelib-1.1.0.tar.gz` & `tmp/paicorelib-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paicorelib-1.1.0.tar", max compression
+gzip compressed data, was "paicorelib-1.1.0rc1.tar", max compression
```

## Comparing `paicorelib-1.1.0.tar` & `paicorelib-1.1.0rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      282 2024-05-17 12:22:50.011186 paicorelib-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-05-17 12:22:50.011186 paicorelib-1.1.0/LICENSE
--rw-r--r--   0        0        0      834 2024-05-17 12:22:50.011186 paicorelib-1.1.0/README.md
--rw-r--r--   0        0        0     1775 2024-05-17 12:22:50.011186 paicorelib-1.1.0/docs/Table-of-Terms.md
--rw-r--r--   0        0        0     1188 2024-05-17 12:22:50.011186 paicorelib-1.1.0/paicorelib/__init__.py
--rw-r--r--   0        0        0    15668 2024-05-17 12:22:50.011186 paicorelib-1.1.0/paicorelib/coordinate.py
--rw-r--r--   0        0        0       81 2024-05-17 12:22:50.011186 paicorelib-1.1.0/paicorelib/framelib/__init__.py
--rw-r--r--   0        0        0     5212 2024-05-17 12:22:50.011186 paicorelib-1.1.0/paicorelib/framelib/base.py
--rw-r--r--   0        0        0     7150 2024-05-17 12:22:50.011186 paicorelib-1.1.0/paicorelib/framelib/frame_defs.py
--rw-r--r--   0        0        0     9900 2024-05-17 12:22:50.011186 paicorelib-1.1.0/paicorelib/framelib/frame_gen.py
--rw-r--r--   0        0        0    22009 2024-05-17 12:22:50.011186 paicorelib-1.1.0/paicorelib/framelib/frames.py
--rw-r--r--   0        0        0      736 2024-05-17 12:22:50.011186 paicorelib-1.1.0/paicorelib/framelib/types.py
--rw-r--r--   0        0        0     4034 2024-05-17 12:22:50.011186 paicorelib-1.1.0/paicorelib/framelib/utils.py
--rw-r--r--   0        0        0     1532 2024-05-17 12:22:50.011186 paicorelib-1.1.0/paicorelib/hw_defs.py
--rw-r--r--   0        0        0     2312 2024-05-17 12:22:50.011186 paicorelib-1.1.0/paicorelib/hw_types.py
--rw-r--r--   0        0        0     7488 2024-05-17 12:22:50.011186 paicorelib-1.1.0/paicorelib/ram_model.py
--rw-r--r--   0        0        0     2618 2024-05-17 12:22:50.011186 paicorelib-1.1.0/paicorelib/ram_types.py
--rw-r--r--   0        0        0     5861 2024-05-17 12:22:50.011186 paicorelib-1.1.0/paicorelib/reg_model.py
--rw-r--r--   0        0        0     4265 2024-05-17 12:22:50.011186 paicorelib-1.1.0/paicorelib/reg_types.py
--rw-r--r--   0        0        0     5747 2024-05-17 12:22:50.011186 paicorelib-1.1.0/paicorelib/routing_defs.py
--rw-r--r--   0        0        0     1729 2024-05-17 12:22:50.011186 paicorelib-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 paicorelib-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      163 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/LICENSE
+-rw-r--r--   0        0        0      837 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/README.md
+-rw-r--r--   0        0        0     1775 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/docs/Table-of-Terms.md
+-rw-r--r--   0        0        0     1188 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/__init__.py
+-rw-r--r--   0        0        0    15668 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/coordinate.py
+-rw-r--r--   0        0        0       81 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/framelib/__init__.py
+-rw-r--r--   0        0        0     5212 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/framelib/base.py
+-rw-r--r--   0        0        0     7150 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/framelib/frame_defs.py
+-rw-r--r--   0        0        0     9900 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/framelib/frame_gen.py
+-rw-r--r--   0        0        0    22003 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/framelib/frames.py
+-rw-r--r--   0        0        0      736 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/framelib/types.py
+-rw-r--r--   0        0        0     4034 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/framelib/utils.py
+-rw-r--r--   0        0        0     1532 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/hw_defs.py
+-rw-r--r--   0        0        0     2312 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/hw_types.py
+-rw-r--r--   0        0        0     7488 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/ram_model.py
+-rw-r--r--   0        0        0     2618 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/ram_types.py
+-rw-r--r--   0        0        0     5816 2024-05-15 07:32:44.420498 paicorelib-1.1.0rc1/paicorelib/reg_model.py
+-rw-r--r--   0        0        0     4265 2024-05-15 07:32:44.424499 paicorelib-1.1.0rc1/paicorelib/reg_types.py
+-rw-r--r--   0        0        0     5757 2024-05-15 07:32:44.424499 paicorelib-1.1.0rc1/paicorelib/routing_defs.py
+-rw-r--r--   0        0        0     1732 2024-05-15 07:32:44.424499 paicorelib-1.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 paicorelib-1.1.0rc1/PKG-INFO
```

### Comparing `paicorelib-1.1.0/LICENSE` & `paicorelib-1.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.0/README.md` & `paicorelib-1.1.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIlib/blob/master/pyproject.toml">
         <img src="https://img.shields.io/pypi/pyversions/paicorelib">
     </a>
-    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v1.1.0">
+    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v1.1.0rc1">
         <img src="https://img.shields.io/github/v/release/PAICookers/PAIlib?color=orange">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIlib">
       <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIlib/master?color=red">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIlib/master">
 	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIlib/master.svg" alt="pre-commit.ci status">
```

### Comparing `paicorelib-1.1.0/docs/Table-of-Terms.md` & `paicorelib-1.1.0rc1/docs/Table-of-Terms.md`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.0/paicorelib/__init__.py` & `paicorelib-1.1.0rc1/paicorelib/__init__.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.0/paicorelib/coordinate.py` & `paicorelib-1.1.0rc1/paicorelib/coordinate.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.0/paicorelib/framelib/base.py` & `paicorelib-1.1.0rc1/paicorelib/framelib/base.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.0/paicorelib/framelib/frame_defs.py` & `paicorelib-1.1.0rc1/paicorelib/framelib/frame_defs.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.0/paicorelib/framelib/frame_gen.py` & `paicorelib-1.1.0rc1/paicorelib/framelib/frame_gen.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.0/paicorelib/framelib/frames.py` & `paicorelib-1.1.0rc1/paicorelib/framelib/frames.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,16 +98,16 @@
         super().__init__(header, chip_coord, core_coord, rid, payload)
 
     @staticmethod
     @params_check(ParamsRegChecker)
     def _payload_reorganized(reg_dict: Dict[str, Any]) -> FrameArrayType:
         # High 8 bits & low 7 bits of tick_wait_start
         tws_high8, tws_low7 = bin_split(reg_dict["tick_wait_start"], 7, 8)
-        # High 3 bits & low 7 bits of test_chip_addr
-        tca_high3, tca_low7 = bin_split(reg_dict["test_chip_addr"].address, 7, 3)
+        # High 3 bits & low 7 bits of test_chip_addrs
+        tca_high3, tca_low7 = bin_split(reg_dict["test_chip_addr"], 7, 3)
 
         reg_frame1 = (
             (reg_dict["weight_width"] & RegF.WEIGHT_WIDTH_MASK)
             << RegF.WEIGHT_WIDTH_OFFSET
             | ((reg_dict["LCN"] & RegF.LCN_MASK) << RegF.LCN_OFFSET)
             | (
                 (reg_dict["input_width"] & RegF.INPUT_WIDTH_MASK)
@@ -567,15 +567,15 @@
         if axon > HwParams.ADDR_AXON_MAX or axon < 0:
             raise ValueError(f"Axon out of range, {axon}.")
 
         if isinstance(_data, np.ndarray) and _data.size != 1:
             raise ShapeError(f"Size of data must be 1, {_data.size}.")
 
         if _data < np.iinfo(np.int8).min or _data > np.iinfo(np.int8).max:
-            raise ValueError("Data out of range np.int8.")
+            raise ValueError(f"Data out of range np.int8.")
 
         self.data = np.uint8(_data)
         self._axon = int(axon)
         self._timeslot = int(timeslot)
 
         payload = FRAME_DTYPE(
             ((self._axon & WF1F.AXON_MASK) << WF1F.AXON_OFFSET)
```

### Comparing `paicorelib-1.1.0/paicorelib/framelib/types.py` & `paicorelib-1.1.0rc1/paicorelib/framelib/types.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.0/paicorelib/framelib/utils.py` & `paicorelib-1.1.0rc1/paicorelib/framelib/utils.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.0/paicorelib/hw_defs.py` & `paicorelib-1.1.0rc1/paicorelib/hw_defs.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.0/paicorelib/hw_types.py` & `paicorelib-1.1.0rc1/paicorelib/hw_types.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.0/paicorelib/ram_model.py` & `paicorelib-1.1.0rc1/paicorelib/ram_model.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.0/paicorelib/ram_types.py` & `paicorelib-1.1.0rc1/paicorelib/ram_types.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.0/paicorelib/reg_model.py` & `paicorelib-1.1.0rc1/paicorelib/reg_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,10 @@
 from typing import Literal
 
-from pydantic import (
-    BaseModel,
-    ConfigDict,
-    Field,
-    field_serializer,
-    field_validator,
-    model_validator,
-)
+from pydantic import BaseModel, ConfigDict, Field, field_serializer, model_validator
 from pydantic.type_adapter import TypeAdapter
 from pydantic.types import NonNegativeInt
 from typing_extensions import TypedDict  # Use `typing_extensions.TypedDict`.
 
 from .coordinate import Coord
 from .hw_defs import HwParams
 from .reg_types import *
@@ -158,16 +151,16 @@
         return snn_mode_en.value
 
     @field_serializer("target_lcn")
     def _target_lcn(self, target_lcn: LCNExtensionType) -> int:
         return target_lcn.value
 
     @field_serializer("test_chip_addr")
-    def _test_chip_addr(self, test_chip_addr: Coord) -> str:
-        return str(test_chip_addr)
+    def _test_chip_addr(self, test_chip_addr: Coord) -> int:
+        return test_chip_addr.address
 
 
 ParamsReg = CoreParams
 
 
 class _ParamsRegDict(TypedDict):
     """Typed dictionary of `ParamsReg` for typing check."""
@@ -178,11 +171,11 @@
     spike_width: int
     neuron_num: int
     pool_max: int
     tick_wait_start: int
     tick_wait_end: int
     snn_en: int
     target_LCN: int
-    test_chip_addr: Coord
+    test_chip_addr: int
 
 
 ParamsRegChecker = TypeAdapter(_ParamsRegDict)
```

### Comparing `paicorelib-1.1.0/paicorelib/reg_types.py` & `paicorelib-1.1.0rc1/paicorelib/reg_types.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.0/paicorelib/routing_defs.py` & `paicorelib-1.1.0rc1/paicorelib/routing_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     X1Y0 = (1, 0)
     X1Y1 = (1, 1)
     ANY = (-1, -1)
 
     def to_index(self) -> int:
         """Convert the direction to index in children list."""
         if self is RoutingDirection.ANY:
-            raise TypeError("The direction of routing is not specified.")
+            raise TypeError(f"The direction of routing is not specified.")
 
         x, y = self.value
 
         if HwParams.COORD_Y_PRIORITY:
             return (x << 1) + y
         else:
             return (y << 1) + x
@@ -83,16 +83,16 @@
     n_L3: int
     n_L4: int
     n_L5: int = 1
 
     def get_routing_level(self) -> RoutingLevel:
         """Return the routing cluster level. If the #N of Lx-level > 1, then we need a  \
             cluster with level Lx+1. And we need the #N of routing sub-level clusters.
-
-        XXX: At present, if #N of L5 > 1, raise exception.
+        
+        XXX: At present, if #N of L5 > 1, raise exception. 
         """
         if self.n_L5 > 1:
             raise ValueError(f"#N of L5-level node out of range, got {self.n_L5}.")
 
         for i in reversed(range(N_ROUTING_LEVEL)):
             if self[i] > 1:
                 return RoutingLevel(i + 1)
```

### Comparing `paicorelib-1.1.0/pyproject.toml` & `paicorelib-1.1.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paicorelib"
-version = "1.1.0"
+version = "1.1.0rc1"
 description = "Library of PAICORE 2.0"
 authors = ["Ziru Pan <zrpan@stu.pku.edu.cn>"]
 maintainers = [
     "Hongtu Xia <hongtux@pku.edu.cn>",
     "Siyuan Gao <siyuan-gao@outlook.com>",
     "Zhaoyang Hao <hzyang2218@gmail.com>",
     "Ziru Pan <zrpan@stu.pku.edu.cn>",
```

### Comparing `paicorelib-1.1.0/PKG-INFO` & `paicorelib-1.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paicorelib
-Version: 1.1.0
+Version: 1.1.0rc1
 Summary: Library of PAICORE 2.0
 Home-page: https://github.com/PAICookers/PAIlib
 License: GPL-3.0-or-later
 Keywords: PAICORE 2.0,PAICORE library,PAILib
 Author: Ziru Pan
 Author-email: zrpan@stu.pku.edu.cn
 Maintainer: Hongtu Xia
@@ -34,15 +34,15 @@
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIlib/blob/master/pyproject.toml">
         <img src="https://img.shields.io/pypi/pyversions/paicorelib">
     </a>
-    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v1.1.0">
+    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v1.1.0rc1">
         <img src="https://img.shields.io/github/v/release/PAICookers/PAIlib?color=orange">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIlib">
       <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIlib/master?color=red">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIlib/master">
 	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIlib/master.svg" alt="pre-commit.ci status">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: paicorelib Version: 1.1.0 Summary: Library of
+Metadata-Version: 2.1 Name: paicorelib Version: 1.1.0rc1 Summary: Library of
 PAICORE 2.0 Home-page: https://github.com/PAICookers/PAIlib License: GPL-3.0-
 or-later Keywords: PAICORE 2.0,PAICORE library,PAILib Author: Ziru Pan Author-
 email: zrpan@stu.pku.edu.cn Maintainer: Hongtu Xia Maintainer-email:
 hongtux@pku.edu.cn Requires-Python: >=3.8,<4.0 Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

