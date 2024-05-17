# Comparing `tmp/py_pilecore-0.4.1.tar.gz` & `tmp/py_pilecore-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_pilecore-0.4.1.tar", last modified: Thu May  2 13:28:31 2024, max compression
+gzip compressed data, was "py_pilecore-0.4.2.tar", last modified: Fri May 17 10:03:14 2024, max compression
```

## Comparing `py_pilecore-0.4.1.tar` & `py_pilecore-0.4.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:28:31.184058 py_pilecore-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-02 13:28:31.184058 py_pilecore-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:28:31.184058 py_pilecore-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:28:31.172057 py_pilecore-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:28:31.180057 py_pilecore-0.4.1/src/py_pilecore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-02 13:28:31.000000 py_pilecore-0.4.1/src/py_pilecore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-02 13:28:31.000000 py_pilecore-0.4.1/src/py_pilecore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:28:31.000000 py_pilecore-0.4.1/src/py_pilecore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-02 13:28:31.000000 py_pilecore-0.4.1/src/py_pilecore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 13:28:31.000000 py_pilecore-0.4.1/src/py_pilecore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:28:31.176057 py_pilecore-0.4.1/src/pypilecore/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:28:31.176057 py_pilecore-0.4.1/src/pypilecore/input/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/input/grouper_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    19577 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/input/multi_cpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/input/pile_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/input/soil_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/plot_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:28:31.180057 py_pilecore-0.4.1/src/pypilecore/results/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30927 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/results/grouper_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/results/load_settlement.py
--rw-r--r--   0 runner    (1001) docker     (127)    25398 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/results/multi_cpt_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    28592 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/results/pile_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    22262 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/results/post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/results/single_cpt_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    20722 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/results/soil_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:28:31.180057 py_pilecore-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    25442 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/tests/test_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:03:14.489102 py_pilecore-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-17 10:03:14.489102 py_pilecore-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 10:03:14.489102 py_pilecore-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:03:14.481102 py_pilecore-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:03:14.489102 py_pilecore-0.4.2/src/py_pilecore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-17 10:03:14.000000 py_pilecore-0.4.2/src/py_pilecore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-17 10:03:14.000000 py_pilecore-0.4.2/src/py_pilecore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 10:03:14.000000 py_pilecore-0.4.2/src/py_pilecore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-17 10:03:14.000000 py_pilecore-0.4.2/src/py_pilecore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 10:03:14.000000 py_pilecore-0.4.2/src/py_pilecore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:03:14.485102 py_pilecore-0.4.2/src/pypilecore/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:03:14.485102 py_pilecore-0.4.2/src/pypilecore/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/input/grouper_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19592 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/input/multi_cpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/input/pile_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/input/soil_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/plot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:03:14.485102 py_pilecore-0.4.2/src/pypilecore/results/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30927 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/results/grouper_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/results/load_settlement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30678 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/results/multi_cpt_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28592 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/results/pile_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22262 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/results/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/results/single_cpt_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20722 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/results/soil_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/src/pypilecore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:03:14.485102 py_pilecore-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    25442 2024-05-17 10:03:10.000000 py_pilecore-0.4.2/tests/test_input.py
```

### Comparing `py_pilecore-0.4.1/LICENSE` & `py_pilecore-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/PKG-INFO` & `py_pilecore-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-pilecore
-Version: 0.4.1
+Version: 0.4.2
 Summary: Public python SDK for the CEMS PileCore web-API.
 License: MIT License
         
         Copyright (c) 2023 CEMS
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `py_pilecore-0.4.1/README.md` & `py_pilecore-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/pyproject.toml` & `py_pilecore-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-pilecore"
-version = "0.4.1"
+version = "0.4.2"
 description = "Public python SDK for the CEMS PileCore web-API."
 requires-python = ">=3.9"
 dependencies = [
     'pygef>0.8,<1',
     'numpy>1,<2',
     'pandas>2,<3',
     'cems-nuclei[client]>=0.5,<1',
```

### Comparing `py_pilecore-0.4.1/src/py_pilecore.egg-info/PKG-INFO` & `py_pilecore-0.4.2/src/py_pilecore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-pilecore
-Version: 0.4.1
+Version: 0.4.2
 Summary: Public python SDK for the CEMS PileCore web-API.
 License: MIT License
         
         Copyright (c) 2023 CEMS
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `py_pilecore-0.4.1/src/py_pilecore.egg-info/SOURCES.txt` & `py_pilecore-0.4.2/src/py_pilecore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/src/py_pilecore.egg-info/requires.txt` & `py_pilecore-0.4.2/src/py_pilecore.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/src/pypilecore/api.py` & `py_pilecore-0.4.2/src/pypilecore/api.py`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/src/pypilecore/input/__init__.py` & `py_pilecore-0.4.2/src/pypilecore/input/__init__.py`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/src/pypilecore/input/grouper_properties.py` & `py_pilecore-0.4.2/src/pypilecore/input/grouper_properties.py`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/src/pypilecore/input/multi_cpt.py` & `py_pilecore-0.4.2/src/pypilecore/input/multi_cpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,17 +309,17 @@
         excavation_depth_nap=excavation_depth_nap,
         master_ocr=ocr,
         individual_negative_friction_range_nap=individual_negative_friction_range_nap,
         individual_positive_friction_range_nap=individual_positive_friction_range_nap,
         individual_ocr=individual_ocr,
     )
     pile_properties = create_pile_properties_payload(
-        pile_type=pile_type,
-        specification=specification,
-        installation=installation,
+        pile_type=str(pile_type),
+        specification=str(specification),
+        installation=str(installation),
         pile_shape=pile_shape,
         diameter_base=diameter_base,
         diameter_shaft=diameter_shaft,
         width_base_large=width_base_large,
         width_base_small=width_base_small,
         width_shaft_large=width_shaft_large,
         width_shaft_small=width_shaft_small,
```

### Comparing `py_pilecore-0.4.1/src/pypilecore/input/pile_properties.py` & `py_pilecore-0.4.2/src/pypilecore/input/pile_properties.py`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/src/pypilecore/input/soil_properties.py` & `py_pilecore-0.4.2/src/pypilecore/input/soil_properties.py`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/src/pypilecore/plot_utils.py` & `py_pilecore-0.4.2/src/pypilecore/plot_utils.py`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/src/pypilecore/results/grouper_result.py` & `py_pilecore-0.4.2/src/pypilecore/results/grouper_result.py`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/src/pypilecore/results/load_settlement.py` & `py_pilecore-0.4.2/src/pypilecore/results/load_settlement.py`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/src/pypilecore/results/multi_cpt_results.py` & `py_pilecore-0.4.2/src/pypilecore/results/multi_cpt_results.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from functools import lru_cache
 from typing import Any, Dict, List, Sequence, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from matplotlib.axes import Axes
+from matplotlib.patches import Patch
 
 from pypilecore.exceptions import UserError
 from pypilecore.results.load_settlement import get_load_settlement_plot
 from pypilecore.results.pile_properties import (
     PileProperties,
     create_pile_properties_from_api_response,
 )
@@ -544,14 +545,174 @@
         return self.cpt_results.test_ids
 
     @property
     def group_results_table(self) -> CPTGroupResultsTable:
         """The CPTGroupResultsTable dataclass, containing the group results."""
         return self._group_results_table
 
+    def boxplot(
+        self,
+        attribute: str,
+        axes: Axes | None = None,
+        figsize: Tuple[float, float] = (6.0, 6.0),
+        show_sqrt: bool = False,
+        **kwargs: Any,
+    ) -> Axes:
+        """
+        Plot a box and whisker plot for a given attribute.
+
+
+        .. code-block:: none
+
+                     MIN      Q1   median  Q3       MAX
+                               |-----:-----|
+                      |--------|     :     |--------|
+                               |-----:-----|
+
+        Parameters
+        ----------
+        attribute:
+            result attribute to create boxplot. Please note that the attribute name must be present in
+            the `CPTResultsTable` and `CPTGroupResultsTable` class.
+        axes:
+            Optional `Axes` object where the boxplot data can be plotted on.
+            If not provided, a new `plt.Figure` will be activated and the `Axes`
+            object will be created and returned.
+        figsize:
+            Size of the activate figure, as the `plt.figure()` argument.
+        show_sqrt:
+            Add sqrt(2) bandwidth to figure
+        **kwargs:
+            All additional keyword arguments are passed to the `pyplot.subplots()` call.
+
+        Returns
+        -------
+        axes:
+            The `Axes` object where the settlement curves were plotted on
+        """
+
+        # validate attribute
+        if (
+            attribute not in self.cpt_results.results[0].table.__dict__.keys()
+            or attribute not in self.group_results_table.__dict__.keys()
+        ):
+            raise ValueError(
+                f"""
+                {attribute} is not present in CPTResultsTable or CPTGroupResultsTable class.
+                Please select on of the following attributes:
+                {
+                    set(self.cpt_results.results[0].table.__dict__.keys())
+                     & set(self.group_results_table.__dict__.keys())
+                }
+                """
+            )
+
+        # Create axes objects if not provided
+        if axes is not None:
+            if not isinstance(axes, Axes):
+                raise ValueError(
+                    "'axes' argument to boxplot() must be a `pyplot.axes.Axes` object or None."
+                )
+        else:
+            kwargs_subplot = {
+                "figsize": figsize,
+                "tight_layout": True,
+            }
+
+            kwargs_subplot.update(kwargs)
+
+            _, axes = plt.subplots(
+                1,
+                1,
+                **kwargs_subplot,
+            )
+
+            if not isinstance(axes, Axes):
+                raise ValueError(
+                    "Could not create Axes objects. This is probably due to invalid matplotlib keyword arguments. "
+                )
+
+        # Collect data from single calculation
+        data = np.array(
+            [
+                item.table.__getattribute__(attribute)
+                for item in self.cpt_results.results
+            ]
+        )
+
+        # Draw a box and whisker plot
+        axes.boxplot(
+            np.flip(data, axis=0),
+            labels=np.flip(self.group_results_table.pile_tip_level_nap),
+            whis=(0, 100),
+            autorange=True,
+            vert=False,
+            patch_artist=True,
+            showmeans=True,
+            zorder=0,
+        )
+
+        # ad additional bandwidth of sqrt(2) of the mean value
+        if show_sqrt:
+            axes.scatter(
+                np.flip(data.mean(axis=0)) * np.sqrt(2),
+                np.flip(
+                    np.arange(len(self.group_results_table.pile_tip_level_nap)) + 1
+                ),
+                marker="^",
+                color="tab:purple",
+                zorder=1,
+            )
+            axes.scatter(
+                np.flip(data.mean(axis=0)) / np.sqrt(2),
+                np.flip(
+                    np.arange(len(self.group_results_table.pile_tip_level_nap)) + 1
+                ),
+                marker="^",
+                color="tab:purple",
+                zorder=1,
+            )
+
+        # Draw group result over single result
+        axes.scatter(
+            np.flip(self.group_results_table.__getattribute__(attribute)),
+            np.flip(np.arange(len(self.group_results_table.pile_tip_level_nap)) + 1),
+            marker="o",
+            color="tab:red",
+            zorder=1,
+        )
+
+        # Draw group result over single result
+        for i, x in enumerate(data.mean(axis=0)):
+            axes.annotate(f"{x.round(2)}", xy=(x, i + 1))
+
+        # add legend to figure
+        axes.legend(
+            handles=[
+                Patch(color=clr, label=key)
+                for (key, clr) in {
+                    "Single;min:max": "black",
+                    "Single;Q25:Q75": "tab:blue",
+                    "Single;Q50": "tab:orange",
+                    "Single;mean": "tab:green",
+                    "Single;mean;sqrt": "tab:purple",
+                    "Group;normative": "tab:red",
+                }.items()
+            ],
+            loc="upper left",
+            bbox_to_anchor=(1, 1),
+            title=f"Bandwidth {attribute}",
+        )
+
+        # set label
+        axes.set_ylabel("Depth [m NAP]")
+        axes.set_xlabel(f"{attribute}")
+
+        return axes
+
     def plot_load_settlement(
         self,
         pile_tip_level_nap: float,
         axes: Axes | None = None,
         figsize: Tuple[float, float] = (6.0, 6.0),
         sb_max: float = 25,
         **kwargs: Any,
```

### Comparing `py_pilecore-0.4.1/src/pypilecore/results/pile_properties.py` & `py_pilecore-0.4.2/src/pypilecore/results/pile_properties.py`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/src/pypilecore/results/post_processing.py` & `py_pilecore-0.4.2/src/pypilecore/results/post_processing.py`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/src/pypilecore/results/single_cpt_results.py` & `py_pilecore-0.4.2/src/pypilecore/results/single_cpt_results.py`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/src/pypilecore/results/soil_properties.py` & `py_pilecore-0.4.2/src/pypilecore/results/soil_properties.py`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/src/pypilecore/utils.py` & `py_pilecore-0.4.2/src/pypilecore/utils.py`

 * *Files identical despite different names*

### Comparing `py_pilecore-0.4.1/tests/test_input.py` & `py_pilecore-0.4.2/tests/test_input.py`

 * *Files identical despite different names*

