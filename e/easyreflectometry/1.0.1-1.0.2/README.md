# Comparing `tmp/easyreflectometry-1.0.1.tar.gz` & `tmp/easyreflectometry-1.0.2.tar.gz`

## Comparing `easyreflectometry-1.0.1.tar` & `easyreflectometry-1.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/__version__.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/data.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/fitting.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/main.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/parameter_utils.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/plot.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/calculators/__init__.py
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/calculators/calculator_base.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/calculators/factory.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/calculators/wrapper_base.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/calculators/bornagain/calculator.py
--rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/calculators/bornagain/wrapper.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/calculators/refl1d/calculator.py
--rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/calculators/refl1d/wrapper.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/calculators/refnx/calculator.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/calculators/refnx/wrapper.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/experiment/__init__.py
--rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/experiment/model.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/experiment/model_collection.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/experiment/resolution_functions.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/measurement/data.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/__init__.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/base_core.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/base_element_collection.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/sample.py
--rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/assemblies/base_assembly.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/assemblies/gradient_layer.py
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/assemblies/multilayer.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/assemblies/repeating_multilayer.py
--rw-r--r--   0        0        0    10438 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/assemblies/surfactant_layer.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/elements/layers/layer.py
--rw-r--r--   0        0        0     9865 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/elements/layers/layer_area_per_molecule.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/elements/layers/layer_collection.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/elements/materials/material.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/elements/materials/material_collection.py
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/elements/materials/material_density.py
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/elements/materials/material_mixture.py
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/sample/elements/materials/material_solvated.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/special/calculations.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/src/easyreflectometry/special/parsing.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/.gitignore
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/AUTHORS.rst
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/LICENSE
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/README.md
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 easyreflectometry-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/__version__.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/data.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/fitting.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/main.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/parameter_utils.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/plot.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/calculators/__init__.py
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/calculators/calculator_base.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/calculators/factory.py
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/calculators/wrapper_base.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/calculators/bornagain/calculator.py
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/calculators/bornagain/wrapper.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/calculators/refl1d/calculator.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/calculators/refl1d/wrapper.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/calculators/refnx/calculator.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/calculators/refnx/wrapper.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/experiment/__init__.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/experiment/model.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/experiment/model_collection.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/experiment/resolution_functions.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/measurement/data.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/__init__.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/base_core.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/base_element_collection.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/sample.py
+-rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/assemblies/base_assembly.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/assemblies/gradient_layer.py
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/assemblies/multilayer.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/assemblies/repeating_multilayer.py
+-rw-r--r--   0        0        0    10438 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/assemblies/surfactant_layer.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/elements/layers/layer.py
+-rw-r--r--   0        0        0     9865 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/elements/layers/layer_area_per_molecule.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/elements/layers/layer_collection.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/elements/materials/material.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/elements/materials/material_collection.py
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/elements/materials/material_density.py
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/elements/materials/material_mixture.py
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/sample/elements/materials/material_solvated.py
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/special/calculations.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/src/easyreflectometry/special/parsing.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/.gitignore
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/AUTHORS.rst
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/README.md
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 easyreflectometry-1.0.2/PKG-INFO
```

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/data.py` & `easyreflectometry-1.0.2/src/easyreflectometry/data.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/fitting.py` & `easyreflectometry-1.0.2/src/easyreflectometry/fitting.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/parameter_utils.py` & `easyreflectometry-1.0.2/src/easyreflectometry/parameter_utils.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/plot.py` & `easyreflectometry-1.0.2/src/easyreflectometry/plot.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/calculators/__init__.py` & `easyreflectometry-1.0.2/src/easyreflectometry/calculators/__init__.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/calculators/calculator_base.py` & `easyreflectometry-1.0.2/src/easyreflectometry/calculators/calculator_base.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/calculators/wrapper_base.py` & `easyreflectometry-1.0.2/src/easyreflectometry/calculators/wrapper_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from abc import abstractmethod
-from typing import Callable
 
 import numpy as np
 
-from easyreflectometry.experiment import DEFAULT_RESOLUTION_FWHM_PERCENTAGE
-from easyreflectometry.experiment import percentage_fhwm_resolution_function
+from easyreflectometry.experiment import PercentageFhwm
+from easyreflectometry.experiment import ResolutionFunction
 
 
 class WrapperBase:
     def __init__(self):
         """Constructor."""
         self.storage = {
             'material': {},
             'layer': {},
             'item': {},
             'model': {},
         }
-        self._resolution_function = percentage_fhwm_resolution_function(DEFAULT_RESOLUTION_FWHM_PERCENTAGE)
+        self._resolution_function = PercentageFhwm()
 
     def reset_storage(self):
         """Reset the storage area to blank."""
         self.storage = {
             'material': {},
             'layer': {},
             'item': {},
@@ -201,13 +200,13 @@
         :param key: The given value keys
         :return: The desired value
         """
         item = self.storage['item'][name]
         item = getattr(item, key)
         return getattr(item, 'value')
 
-    def set_resolution_function(self, resolution_function: Callable[[np.array], np.array]) -> None:
+    def set_resolution_function(self, resolution_function: ResolutionFunction) -> None:
         """Set the resolution function for the calculator.
 
         :param resolution_function: The resolution function
         """
         self._resolution_function = resolution_function
```

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/calculators/bornagain/calculator.py` & `easyreflectometry-1.0.2/src/easyreflectometry/calculators/bornagain/calculator.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/calculators/bornagain/wrapper.py` & `easyreflectometry-1.0.2/src/easyreflectometry/calculators/bornagain/wrapper.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/calculators/refl1d/calculator.py` & `easyreflectometry-1.0.2/src/easyreflectometry/calculators/refl1d/calculator.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/calculators/refl1d/wrapper.py` & `easyreflectometry-1.0.2/src/easyreflectometry/calculators/refl1d/wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __author__ = 'github.com/arm61'
 
 from typing import Tuple
 
 import numpy as np
-from easyreflectometry.experiment.resolution_functions import is_percentage_fhwm_resolution_function
+from easyreflectometry.experiment.resolution_functions import PercentageFhwm
 from refl1d import model
 from refl1d import names
 
 from ..wrapper_base import WrapperBase
 
 RESOLUTION_PADDING = 3.5
 OVERSAMPLING_FACTOR = 21
@@ -141,17 +141,17 @@
         """For a given q array calculate the corresponding reflectivity.
 
         :param q_array: array of data points to be calculated
         :param model_name: the model name
         :return: reflectivity calculated at q
         """
         sample = _build_sample(self.storage, model_name)
-        dq_array = self._resolution_function(q_array)
+        dq_array = self._resolution_function.smearing(q_array)
 
-        if is_percentage_fhwm_resolution_function(self._resolution_function):
+        if isinstance(self._resolution_function, PercentageFhwm):
             # Get percentage of Q and change from sigma to FWHM
             dq_array = dq_array * q_array / 100 / (2 * np.sqrt(2 * np.log(2)))
 
         if not MAGNETISM:
             probe = _get_probe(
                 q_array=q_array,
                 dq_array=dq_array,
```

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/calculators/refnx/calculator.py` & `easyreflectometry-1.0.2/src/easyreflectometry/calculators/refnx/calculator.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/calculators/refnx/wrapper.py` & `easyreflectometry-1.0.2/src/easyreflectometry/calculators/refnx/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __author__ = 'github.com/arm61'
 
 from typing import Tuple
 
 import numpy as np
-from easyreflectometry.experiment.resolution_functions import is_percentage_fhwm_resolution_function
+from easyreflectometry.experiment.resolution_functions import PercentageFhwm
 from refnx import reflect
 
 from ..wrapper_base import WrapperBase
 
 
 class RefnxWrapper(WrapperBase):
     def create_material(self, name: str):
@@ -125,16 +125,16 @@
         model = reflect.ReflectModel(
             structure,
             scale=self.storage['model'][model_name].scale.value,
             bkg=self.storage['model'][model_name].bkg.value,
             dq_type='pointwise',
         )
 
-        dq_vector = self._resolution_function(q_array)
-        if is_percentage_fhwm_resolution_function(self._resolution_function):
+        dq_vector = self._resolution_function.smearing(q_array)
+        if isinstance(self._resolution_function, PercentageFhwm):
             # FWHM Percentage resolution is constant given as
             # For a constant resolution percentage refnx supports to pass a scalar value rather than a vector
             dq_vector = dq_vector[0]
 
         return model(x=q_array, x_err=dq_vector)
 
     def sld_profile(self, model_name: str) -> Tuple[np.ndarray, np.ndarray]:
```

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/experiment/model.py` & `easyreflectometry-1.0.2/src/easyreflectometry/experiment/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from __future__ import annotations
 
 __author__ = 'github.com/arm61'
 
 from numbers import Number
-from typing import Callable
 from typing import Union
 
 import numpy as np
 import yaml
 from easyscience.Objects.ObjectClasses import BaseObj
 from easyscience.Objects.ObjectClasses import Parameter
 
-from easyreflectometry.experiment.resolution_functions import is_percentage_fhwm_resolution_function
 from easyreflectometry.parameter_utils import get_as_parameter
 from easyreflectometry.sample import BaseAssembly
 from easyreflectometry.sample import Layer
 from easyreflectometry.sample import LayerCollection
 from easyreflectometry.sample import Sample
 
-from .resolution_functions import percentage_fhwm_resolution_function
+from .resolution_functions import PercentageFhwm
+from .resolution_functions import ResolutionFunction
 
 DEFAULTS = {
     'scale': {
         'description': 'Scaling of the reflectomety profile',
         'url': 'https://github.com/reflectivity/edu_outreach/blob/master/refl_maths/paper.tex',
         'value': 1.0,
         'min': 0,
@@ -55,45 +54,43 @@
     background: Parameter
 
     def __init__(
         self,
         sample: Union[Sample, None] = None,
         scale: Union[Parameter, Number, None] = None,
         background: Union[Parameter, Number, None] = None,
-        resolution_function: Union[Callable[[np.array], float], None] = None,
+        resolution_function: Union[ResolutionFunction, None] = None,
         name: str = 'EasyModel',
         interface=None,
     ):
         """Constructor.
 
         :param sample: The sample being modelled.
         :param scale: Scaling factor of profile.
         :param background: Linear background magnitude.
         :param name: Name of the model, defaults to 'EasyModel'.
-        :param resolution_function: Resolution function, defaults to percentage_fhwm_resolution_function.
+        :param resolution_function: Resolution function, defaults to PercentageFhwm.
         :param interface: Calculator interface, defaults to `None`.
 
         """
 
         if sample is None:
             sample = Sample(interface=interface)
         if resolution_function is None:
-            resolution_function = percentage_fhwm_resolution_function(DEFAULTS['resolution']['value'])
+            resolution_function = PercentageFhwm(DEFAULTS['resolution']['value'])
 
         scale = get_as_parameter('scale', scale, DEFAULTS)
         background = get_as_parameter('background', background, DEFAULTS)
 
         super().__init__(
             name=name,
             sample=sample,
             scale=scale,
             background=background,
         )
-        if not callable(resolution_function):
-            raise ValueError('Resolution function must be a callable.')
         self.resolution_function = resolution_function
         # Must be set after resolution function
         self.interface = interface
 
     def add_item(self, *assemblies: list[BaseAssembly]) -> None:
         """Add a layer or item to the model sample.
 
@@ -136,20 +133,20 @@
         :param idx: Index of the item to remove.
         """
         if self.interface is not None:
             self.interface().remove_item_from_model(self.sample[idx].uid, self.uid)
         del self.sample[idx]
 
     @property
-    def resolution_function(self) -> Callable[[np.array], np.array]:
+    def resolution_function(self) -> ResolutionFunction:
         """Return the resolution function."""
         return self._resolution_function
 
     @resolution_function.setter
-    def resolution_function(self, resolution_function: Callable[[np.array], np.array]) -> None:
+    def resolution_function(self, resolution_function: ResolutionFunction) -> None:
         """Set the resolution function for the model."""
         self._resolution_function = resolution_function
         if self.interface is not None:
             self.interface().set_resolution_function(self._resolution_function)
 
     @property
     def interface(self):
@@ -172,16 +169,16 @@
         """Return a UID from the borg map."""
         return self._borg.map.convert_id_to_key(self)
 
     # Representation
     @property
     def _dict_repr(self) -> dict[str, dict[str, str]]:
         """A simplified dict representation."""
-        if is_percentage_fhwm_resolution_function(self._resolution_function):
-            resolution_value = self._resolution_function([0])[0]
+        if isinstance(self._resolution_function, PercentageFhwm):
+            resolution_value = self._resolution_function.as_dict()['constant']
             resolution = f'{resolution_value} %'
         else:
             resolution = 'function of Q'
 
         return {
             self.name: {
                 'scale': self.scale.raw_value,
@@ -200,25 +197,29 @@
         The resulting dict matches the parameters in __init__
 
         :param skip: List of keys to skip, defaults to `None`.
         """
         if skip is None:
             skip = []
         this_dict = super().as_dict(skip=skip)
-        this_dict['sample'] = self.sample.as_dict()
+        this_dict['sample'] = self.sample.as_dict(skip=skip)
+        this_dict['resolution_function'] = self.resolution_function.as_dict()
         return this_dict
 
     @classmethod
-    def from_dict(cls, data: dict) -> Model:
+    def from_dict(cls, this_dict: dict) -> Model:
         """
         Create a Model from a dictionary.
 
-        :param data: dictionary of the Model
+        :param this_dict: dictionary of the Model
         :return: Model
         """
-        model = super().from_dict(data)
+        resolution_function = ResolutionFunction.from_dict(this_dict['resolution_function'])
+        del this_dict['resolution_function']
+        sample = Sample.from_dict(this_dict['sample'])
+        del this_dict['sample']
 
-        # Ensure that the sample is also converted
-        # TODO Should probably be handled in easyscience
-        model.sample = model.sample.__class__.from_dict(data['sample'])
+        model = super().from_dict(this_dict)
 
+        model.sample = sample
+        model.resolution_function = resolution_function
         return model
```

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/experiment/model_collection.py` & `easyreflectometry-1.0.2/src/easyreflectometry/experiment/model_collection.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 __author__ = 'github.com/arm61'
 
 from typing import Optional
 
 from easyreflectometry.sample.base_element_collection import SIZE_DEFAULT_COLLECTION
 from easyreflectometry.sample.base_element_collection import BaseElementCollection
 
@@ -10,20 +12,20 @@
 
 class ModelCollection(BaseElementCollection):
     # Added in super().__init__
     models: list[Model]
 
     def __init__(
         self,
-        *models: Optional[list[Model]],
+        *models: Optional[tuple[Model]],
         name: str = 'EasyModels',
         interface=None,
         **kwargs,
     ):
-        if models is None:
+        if not models:
             models = [Model(interface=interface) for _ in range(SIZE_DEFAULT_COLLECTION)]
         super().__init__(name, interface, *models, **kwargs)
         self.interface = interface
 
     def add_model(self, new_model: Model):
         """
         Add a model to the models.
@@ -35,7 +37,24 @@
     def remove_model(self, idx: int):
         """
         Remove an model from the models.
 
         :param idx: Index of the model to remove
         """
         del self[idx]
+
+    @classmethod
+    def from_dict(cls, this_dict: dict) -> ModelCollection:
+        """
+        Create an instance of a collection from a dictionary.
+
+        :param data: The dictionary for the collection
+        :return: An instance of the collection
+        """
+        collection = super().from_dict(this_dict)  # type: ModelCollection
+
+        if len(collection) != len(this_dict['data']):
+            raise ValueError(f"Expected {len(collection)} models, got {len(this_dict['data'])}")
+        for i, model_data in enumerate(this_dict['data']):
+            collection[i] = Model.from_dict(model_data)
+
+        return collection
```

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/__init__.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/base_core.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/base_core.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/base_element_collection.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/base_element_collection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from typing import Any
+from typing import List
+from typing import Optional
 
 import yaml
 from easyscience.Objects.Groups import BaseCollection
 
 SIZE_DEFAULT_COLLECTION = 2
 
 
@@ -44,14 +46,26 @@
         """
         A simplified dict representation.
 
         :return: Simple dictionary
         """
         return {self.name: [i._dict_repr for i in self]}
 
+    def as_dict(self, skip: Optional[List[str]] = None) -> dict:
+        """
+        Create a dictionary representation of the collection.
+
+        :return: A dictionary representation of the collection
+        """
+        this_dict = super().as_dict(skip=skip)
+        this_dict['data'] = []
+        for collection_element in self:
+            this_dict['data'].append(collection_element.as_dict(skip=skip))
+        return this_dict
+
     @classmethod
     def from_dict(cls, data: dict) -> Any:
         """
         Create an instance of a collection from a dictionary.
 
         :param data: The dictionary for the collection
         :return: An instance of the collection
```

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/sample.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         :param skip: List of keys to skip, defaults to `None`.
         """
         if skip is None:
             skip = []
         this_dict = super().as_dict(skip=skip)
         for i, layer in enumerate(self.data):
-            this_dict['data'][i] = layer.as_dict()
+            this_dict['data'][i] = layer.as_dict(skip=skip)
         return this_dict
 
     @classmethod
     def from_dict(cls, data: dict) -> Sample:
         """
         Create a Sample from a dictionary.
```

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/assemblies/base_assembly.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/assemblies/base_assembly.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/assemblies/gradient_layer.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/assemblies/gradient_layer.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/assemblies/multilayer.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/assemblies/multilayer.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/assemblies/repeating_multilayer.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/assemblies/repeating_multilayer.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/assemblies/surfactant_layer.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/assemblies/surfactant_layer.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/elements/layers/layer.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/elements/layers/layer.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/elements/layers/layer_area_per_molecule.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/elements/layers/layer_area_per_molecule.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/elements/layers/layer_collection.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/elements/layers/layer_collection.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/elements/materials/material.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/elements/materials/material.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/elements/materials/material_collection.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/elements/materials/material_collection.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/elements/materials/material_density.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/elements/materials/material_density.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/elements/materials/material_mixture.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/elements/materials/material_mixture.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/sample/elements/materials/material_solvated.py` & `easyreflectometry-1.0.2/src/easyreflectometry/sample/elements/materials/material_solvated.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/special/calculations.py` & `easyreflectometry-1.0.2/src/easyreflectometry/special/calculations.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/src/easyreflectometry/special/parsing.py` & `easyreflectometry-1.0.2/src/easyreflectometry/special/parsing.py`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/LICENSE` & `easyreflectometry-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/README.md` & `easyreflectometry-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `easyreflectometry-1.0.1/pyproject.toml` & `easyreflectometry-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -52,16 +52,17 @@
     "ruff",
     "toml>=0.10",
     "yapf>=0.31.0",
 ]
 docs = [
     "myst_parser",
     "nbsphinx",
-    "sphinx_book_theme",
     "sphinx_autodoc_typehints",
+    "sphinx_book_theme",
+    "sphinx-copybutton",
     "toml"
 ]
 
 [project.urls]
 homepage = "https://docs.easyreflectometry.org"
 documentation = "https://docs.easyreflectometry.org"
```

### Comparing `easyreflectometry-1.0.1/PKG-INFO` & `easyreflectometry-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyreflectometry
-Version: 1.0.1
+Version: 1.0.2
 Summary: A reflectometry python package built on the EasyScience framework.
 Project-URL: homepage, https://docs.easyreflectometry.org
 Project-URL: documentation, https://docs.easyreflectometry.org
 Author: EasyScience contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Easyscience contributors (https://github.com/EasyScience)
@@ -68,14 +68,15 @@
 Requires-Dist: toml>=0.10; extra == 'dev'
 Requires-Dist: yapf>=0.31.0; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: nbsphinx; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-book-theme; extra == 'docs'
+Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: toml; extra == 'docs'
 Description-Content-Type: text/markdown
 
 ![Logo](https://github.com/easyScience/EasyReflectometryLib/raw/master/docs/src/_static/logo.png)
 [![CI badge](https://github.com/easyScience/EasyReflectometryLib/actions/workflows/python-ci.yml/badge.svg)](https://github.com/easyScience/easyReflectometryLib/actions/workflows/python-ci.yml)
 [![PyPI badge](https://img.shields.io/pypi/v/easyreflectometry.svg)](https://pypi.python.org/pypi/easyreflectometry)
 [![Quality badge](https://www.codefactor.io/repository/github/easyscience/easyreflectometrylib/badge)](https://www.codefactor.io/repository/github/easyscience/easyreflectometrylib)
```

