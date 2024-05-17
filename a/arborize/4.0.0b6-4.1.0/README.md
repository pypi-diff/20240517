# Comparing `tmp/arborize-4.0.0b6.tar.gz` & `tmp/arborize-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arborize-4.0.0b6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "arborize-4.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `arborize-4.0.0b6.tar` & `arborize-4.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0    35149 2022-04-12 08:11:03.755436 arborize-4.0.0b6/LICENSE
--rwxr-xr-x   0        0        0      239 2022-04-14 09:20:30.614357 arborize-4.0.0b6/README.md
--rwxr-xr-x   0        0        0      823 2024-03-07 12:22:23.067398 arborize-4.0.0b6/arborize/__init__.py
--rwxr-xr-x   0        0        0     2142 2024-02-21 15:52:56.718688 arborize-4.0.0b6/arborize/_util.py
--rwxr-xr-x   0        0        0      109 2024-02-21 15:52:56.717686 arborize-4.0.0b6/arborize/builders/__init__.py
--rwxr-xr-x   0        0        0     5601 2024-02-13 15:48:13.847106 arborize-4.0.0b6/arborize/builders/_arbor.py
--rwxr-xr-x   0        0        0     4318 2024-03-07 12:20:10.575943 arborize-4.0.0b6/arborize/builders/_bluepyopt.py
--rwxr-xr-x   0        0        0     9007 2024-02-21 15:52:56.718688 arborize-4.0.0b6/arborize/builders/_neuron.py
--rwxr-xr-x   0        0        0     5978 2024-03-07 12:20:19.100544 arborize-4.0.0b6/arborize/constraints.py
--rwxr-xr-x   0        0        0    14277 2024-02-21 15:52:56.718688 arborize-4.0.0b6/arborize/definitions.py
--rwxr-xr-x   0        0        0      860 2024-02-13 15:03:39.261064 arborize-4.0.0b6/arborize/exceptions.py
--rwxr-xr-x   0        0        0      487 2024-02-13 15:03:39.261064 arborize-4.0.0b6/arborize/parameter.py
--rwxr-xr-x   0        0        0    11684 2024-02-21 15:52:56.718688 arborize-4.0.0b6/arborize/schematic.py
--rwxr-xr-x   0        0        0       68 2024-02-13 15:03:39.261064 arborize-4.0.0b6/arborize/schematics/__init__.py
--rwxr-xr-x   0        0        0     1594 2024-02-21 15:52:56.718688 arborize-4.0.0b6/arborize/schematics/_bsb.py
--rwxr-xr-x   0        0        0     3437 2024-02-21 15:52:56.718688 arborize-4.0.0b6/arborize/schematics/_file.py
--rwxr-xr-x   0        0        0     1359 2022-04-14 09:20:30.626355 arborize-4.0.0b6/arborize/synapse.py
--rwxr-xr-x   0        0        0      855 2024-03-07 12:20:47.011155 arborize-4.0.0b6/pyproject.toml
--rw-r--r--   0        0        0     1433 1970-01-01 00:00:00.000000 arborize-4.0.0b6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-08 07:44:19.561382 arborize-4.1.0/LICENSE
+-rw-r--r--   0        0        0      239 2024-05-08 07:44:19.561382 arborize-4.1.0/README.md
+-rw-r--r--   0        0        0      821 2024-05-17 09:13:58.936305 arborize-4.1.0/arborize/__init__.py
+-rw-r--r--   0        0        0     2142 2024-05-08 07:44:19.561382 arborize-4.1.0/arborize/_util.py
+-rw-r--r--   0        0        0      109 2024-05-08 07:44:19.561382 arborize-4.1.0/arborize/builders/__init__.py
+-rw-r--r--   0        0        0     5601 2024-05-08 07:44:19.561382 arborize-4.1.0/arborize/builders/_arbor.py
+-rw-r--r--   0        0        0     4318 2024-05-08 07:44:19.561382 arborize-4.1.0/arborize/builders/_bluepyopt.py
+-rw-r--r--   0        0        0     9007 2024-05-08 07:44:19.561382 arborize-4.1.0/arborize/builders/_neuron.py
+-rw-r--r--   0        0        0     5978 2024-05-08 07:44:19.561382 arborize-4.1.0/arborize/constraints.py
+-rw-r--r--   0        0        0    15188 2024-05-17 09:13:58.936305 arborize-4.1.0/arborize/definitions.py
+-rw-r--r--   0        0        0      860 2024-05-08 07:44:19.561382 arborize-4.1.0/arborize/exceptions.py
+-rw-r--r--   0        0        0      487 2024-05-08 07:44:19.561382 arborize-4.1.0/arborize/parameter.py
+-rw-r--r--   0        0        0    11684 2024-05-08 07:44:19.561382 arborize-4.1.0/arborize/schematic.py
+-rw-r--r--   0        0        0       68 2024-05-08 07:44:19.561382 arborize-4.1.0/arborize/schematics/__init__.py
+-rw-r--r--   0        0        0     1581 2024-05-08 07:44:19.561382 arborize-4.1.0/arborize/schematics/_bsb.py
+-rw-r--r--   0        0        0     3437 2024-05-08 07:44:19.561382 arborize-4.1.0/arborize/schematics/_file.py
+-rw-r--r--   0        0        0     1359 2024-05-08 07:44:19.561382 arborize-4.1.0/arborize/synapse.py
+-rw-r--r--   0        0        0     1518 2024-05-17 09:13:58.936305 arborize-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 arborize-4.1.0/PKG-INFO
```

### Comparing `arborize-4.0.0b6/LICENSE` & `arborize-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arborize-4.0.0b6/arborize/__init__.py` & `arborize-4.1.0/arborize/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     ModelDefinition,
     define_model,
     is_mech_id,
 )
 from .schematic import Schematic
 from .schematics import bsb_schematic, file_schematic
 
-__version__ = "4.0.0b6"
+__version__ = "4.1.0"
 __all__ = [
     "CableProperties",
     "CableType",
     "Ion",
     "Mechanism",
     "ModelDefinition",
     "Schematic",
```

### Comparing `arborize-4.0.0b6/arborize/_util.py` & `arborize-4.1.0/arborize/_util.py`

 * *Files identical despite different names*

### Comparing `arborize-4.0.0b6/arborize/builders/_arbor.py` & `arborize-4.1.0/arborize/builders/_arbor.py`

 * *Files identical despite different names*

### Comparing `arborize-4.0.0b6/arborize/builders/_bluepyopt.py` & `arborize-4.1.0/arborize/builders/_bluepyopt.py`

 * *Files identical despite different names*

### Comparing `arborize-4.0.0b6/arborize/builders/_neuron.py` & `arborize-4.1.0/arborize/builders/_neuron.py`

 * *Files identical despite different names*

### Comparing `arborize-4.0.0b6/arborize/constraints.py` & `arborize-4.1.0/arborize/constraints.py`

 * *Files identical despite different names*

### Comparing `arborize-4.0.0b6/arborize/definitions.py` & `arborize-4.1.0/arborize/definitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,28 +14,34 @@
 class CableProperties(Copy, Merge, Assert, Iterable):
     Ra: float = None
     cm: float = None
     """
     Axial resistivity in ohm/cm
     """
 
+    def to_dict(self) -> dict:
+        return dataclasses.asdict(self)
+
 
 CablePropertiesDict = typing.TypedDict(
     "CablePropertiesDict",
     {"Ra": float, "cm": float},
     total=False,
 )
 
 
 @dataclasses.dataclass
 class Ion(Copy, Merge, Assert, Iterable):
     rev_pot: float = None
     int_con: float = None
     ext_con: float = None
 
+    def to_dict(self) -> dict:
+        return dataclasses.asdict(self)
+
 
 IonDict = typing.TypedDict(
     "IonDict",
     {"rev_pot": float, "int_con": float, "ext_con": float},
     total=False,
 )
 
@@ -48,14 +54,17 @@
     def merge(self, other):
         for key, value in other.parameters.items():
             self.parameters[key] = value
 
     def copy(self):
         return Mechanism(self.parameters.copy())
 
+    def to_dict(self):
+        return {k: v for k, v in self.parameters.items()}
+
 
 class Synapse(Mechanism):
     mech_id: MechIdTuple
 
     def __init__(self, parameters, mech_id: MechId):
         super().__init__(parameters)
         self.mech_id = to_mech_id(mech_id)
@@ -111,14 +120,22 @@
 
     def set(self, param: "Parameter"):
         if hasattr(param, "set_cable_params"):
             param.set_cable_params(self.cable)
         if hasattr(param, "set_mech_params"):
             param.set_mech_params(self.mechs)
 
+    def to_dict(self):
+        cable_dict = {}
+        cable_dict["ions"] = {k: v.to_dict() for k, v in self.ions.items()}
+        cable_dict["cable"] = self.cable.to_dict()
+        cable_dict["mechanisms"] = {k: v.to_dict() for k, v in self.mechs.items()}
+        cable_dict["synapses"] = {k: v.to_dict() for k, v in self.synapses.items()}
+        return cable_dict
+
     @classmethod
     def anchor(
         cls,
         defs: typing.Iterable["CableType"],
         synapses: dict[MechId, Synapse] = None,
         use_defaults: bool = False,
         ion_class=Ion,
@@ -304,14 +321,20 @@
         mech_id = synapse.mech_id or to_mech_id(label)
         if not is_mech_id(mech_id):
             raise ValueError(f"'{mech_id}' is not a valid synapse mechanism.")
         if label in self._synapse_types:
             raise KeyError(f"Synapse type {label} already exists.")
         self._synapse_types[label] = synapse
 
+    def to_dict(self) -> dict:
+        cable_dict = {k: v.to_dict() for k, v in self._cable_types.items()}
+        synapse_dict = {k: v.to_dict() for k, v in self._synapse_types.items()}
+        model_dict = {"cable_types": cable_dict, "synapse_types": synapse_dict}
+        return model_dict
+
 
 class ModelDefinition(Definition[CableType, CableProperties, Ion, Mechanism, Synapse]):
     @classmethod
     @property
     def cable_type_class(cls):
         return CableType
```

### Comparing `arborize-4.0.0b6/arborize/exceptions.py` & `arborize-4.1.0/arborize/exceptions.py`

 * *Files identical despite different names*

### Comparing `arborize-4.0.0b6/arborize/schematic.py` & `arborize-4.1.0/arborize/schematic.py`

 * *Files identical despite different names*

### Comparing `arborize-4.0.0b6/arborize/schematics/_bsb.py` & `arborize-4.1.0/arborize/schematics/_bsb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import itertools
 from typing import TYPE_CHECKING, Optional
 
 from ..schematic import Schematic
 
 if TYPE_CHECKING:
-    from bsb.morphologies import Branch, Morphology
+    from bsb import Branch, Morphology
 
     from ..definitions import Definition
 
 
 def bsb_schematic(
     morphology: "Morphology", definitions: Optional["Definition"] = None
 ) -> Schematic:
```

### Comparing `arborize-4.0.0b6/arborize/schematics/_file.py` & `arborize-4.1.0/arborize/schematics/_file.py`

 * *Files identical despite different names*

### Comparing `arborize-4.0.0b6/arborize/synapse.py` & `arborize-4.1.0/arborize/synapse.py`

 * *Files identical despite different names*

### Comparing `arborize-4.0.0b6/PKG-INFO` & `arborize-4.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: arborize
-Version: 4.0.0b6
+Version: 4.1.0
 Summary: Write descriptions for NEURON cell models in an Arbor-like manner for both the Arbor and
 Author-email: Robin De Schepper <robingilbert.deschepper@unipv.it>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Dist: numpy
-Requires-Dist: errr>=1.2.0
-Requires-Dist: morphio>=3.3.6
-Requires-Dist: arbor>=0.9 ; extra == "arbor"
-Requires-Dist: nmodl-glia[arbor]>=4.0.0b6 ; extra == "arbor"
+Requires-Dist: numpy~=1.21
+Requires-Dist: errr~=1.2
+Requires-Dist: morphio>=3.3.6,<4
+Requires-Dist: arbor~=0.9 ; extra == "arbor"
+Requires-Dist: nmodl-glia[arbor]~=4.0 ; extra == "arbor"
 Requires-Dist: bluepyopt~=1.14 ; extra == "bluepyopt"
-Requires-Dist: dill~=0.3.8 ; extra == "bluepyopt"
-Requires-Dist: sphinx ; extra == "dev"
-Requires-Dist: sphinx_rtd_theme ; extra == "dev"
-Requires-Dist: black==24.1.1 ; extra == "dev"
-Requires-Dist: nrn-patch>=4.0.0b3 ; extra == "neuron"
-Requires-Dist: nmodl-glia[neuron]>=4.0.0b6 ; extra == "neuron"
-Requires-Dist: mpi4py ; extra == "parallel"
+Requires-Dist: dill>=0.3.8 ; extra == "bluepyopt"
+Requires-Dist: sphinx~=7.0 ; extra == "dev"
+Requires-Dist: sphinx-rtd-theme~=2.0 ; extra == "dev"
+Requires-Dist: black~=24.0 ; extra == "dev"
+Requires-Dist: nrn-patch~=4.0 ; extra == "neuron"
+Requires-Dist: nmodl-glia[neuron]~=4.0 ; extra == "neuron"
+Requires-Dist: mpi4py~=3.0 ; extra == "parallel"
 Requires-Dist: coverage~=7.0 ; extra == "test"
 Project-URL: Home, https://github.com/dbbs-lab/arborize
 Provides-Extra: arbor
 Provides-Extra: bluepyopt
 Provides-Extra: dev
 Provides-Extra: neuron
 Provides-Extra: parallel
```

