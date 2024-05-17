# Comparing `tmp/subsettools-1.0.4.tar.gz` & `tmp/subsettools-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subsettools-1.0.4.tar", max compression
+gzip compressed data, was "subsettools-1.0.5.tar", max compression
```

## Comparing `subsettools-1.0.4.tar` & `subsettools-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rwxr-xr-x   0        0        0     1092 2023-11-13 19:24:51.323232 subsettools-1.0.4/LICENSE
--rwxr-xr-x   0        0        0     2690 2024-04-16 17:49:13.047816 subsettools-1.0.4/README.md
--rw-r--r--   0        0        0      771 2024-05-03 17:17:58.029186 subsettools-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      511 2024-04-29 23:34:58.686225 subsettools-1.0.4/src/subsettools/__init__.py
--rw-r--r--   0        0        0     2468 2024-04-29 23:34:58.686225 subsettools-1.0.4/src/subsettools/_error_checking.py
--rw-r--r--   0        0        0     2110 2023-11-29 18:37:02.142147 subsettools-1.0.4/src/subsettools/datasets.py
--rw-r--r--   0        0        0      133 2023-11-29 18:37:02.142147 subsettools-1.0.4/src/subsettools/ref_yamls/__init__.py
--rw-r--r--   0        0        0    10637 2023-11-13 19:24:51.324232 subsettools-1.0.4/src/subsettools/ref_yamls/conus1_pf_spinup_box.yaml
--rw-r--r--   0        0        0    10190 2023-11-13 19:24:51.324232 subsettools-1.0.4/src/subsettools/ref_yamls/conus1_pf_spinup_solid.yaml
--rw-r--r--   0        0        0    10951 2023-11-13 19:24:51.324232 subsettools-1.0.4/src/subsettools/ref_yamls/conus1_pfclm_transient_box.yaml
--rw-r--r--   0        0        0    10482 2023-11-13 19:24:51.324232 subsettools-1.0.4/src/subsettools/ref_yamls/conus1_pfclm_transient_solid.yaml
--rw-r--r--   0        0        0    11495 2023-11-13 19:24:51.324232 subsettools-1.0.4/src/subsettools/ref_yamls/conus2_pf_spinup_box.yaml
--rw-r--r--   0        0        0    11047 2023-11-13 19:24:51.324232 subsettools-1.0.4/src/subsettools/ref_yamls/conus2_pf_spinup_solid.yaml
--rw-r--r--   0        0        0    11832 2023-11-13 19:24:51.324232 subsettools-1.0.4/src/subsettools/ref_yamls/conus2_pfclm_transient_box.yaml
--rw-r--r--   0        0        0    11384 2023-11-13 19:24:51.324232 subsettools-1.0.4/src/subsettools/ref_yamls/conus2_pfclm_transient_solid.yaml
--rw-r--r--   0        0        0     5886 2023-12-07 15:45:24.945374 subsettools-1.0.4/src/subsettools/subset_utils.py
--rw-r--r--   0        0        0    41926 2024-04-29 23:34:58.692225 subsettools-1.0.4/src/subsettools/subsettools.py
--rw-r--r--   0        0        0     3436 2024-05-03 17:17:58.029186 subsettools-1.0.4/src/subsettools/upstream_area.py
--rw-r--r--   0        0        0     2604 2024-04-17 16:57:39.679663 subsettools-1.0.4/src/subsettools/upstream_area.py~
--rw-r--r--   0        0        0     3344 1970-01-01 00:00:00.000000 subsettools-1.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1092 2023-11-13 19:24:51.323232 subsettools-1.0.5/LICENSE
+-rwxr-xr-x   0        0        0     2690 2024-05-16 18:38:12.864911 subsettools-1.0.5/README.md
+-rw-r--r--   0        0        0      862 2024-05-17 15:37:58.049379 subsettools-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      612 2024-05-16 18:38:12.881911 subsettools-1.0.5/src/subsettools/__init__.py
+-rw-r--r--   0        0        0      661 2024-05-16 18:38:12.881911 subsettools-1.0.5/src/subsettools/_common.py
+-rw-r--r--   0        0        0      154 2024-05-16 18:38:12.881911 subsettools-1.0.5/src/subsettools/_constants.py
+-rw-r--r--   0        0        0      820 2024-05-16 18:38:12.881911 subsettools-1.0.5/src/subsettools/_dev_utils.py
+-rw-r--r--   0        0        0     2928 2024-05-16 18:38:12.881911 subsettools-1.0.5/src/subsettools/_error_checking.py
+-rw-r--r--   0        0        0     9261 2024-05-16 18:38:12.881911 subsettools-1.0.5/src/subsettools/clm.py
+-rw-r--r--   0        0        0    19445 2024-05-16 18:38:12.881911 subsettools-1.0.5/src/subsettools/domain.py
+-rw-r--r--   0        0        0    14479 2024-05-16 18:38:12.881911 subsettools-1.0.5/src/subsettools/parflow_run.py
+-rw-r--r--   0        0        0    15122 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/subsetting.py
+-rw-r--r--   0        0        0      147 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/__init__.py
+-rw-r--r--   0        0        0    10637 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/conus1_spinup_box.yaml
+-rw-r--r--   0        0        0    10190 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/conus1_spinup_solid.yaml
+-rw-r--r--   0        0        0    10951 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/conus1_transient_box.yaml
+-rw-r--r--   0        0        0    10482 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/conus1_transient_solid.yaml
+-rw-r--r--   0        0        0    11495 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/conus2_spinup_box.yaml
+-rw-r--r--   0        0        0    11047 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/conus2_spinup_solid.yaml
+-rw-r--r--   0        0        0    11832 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/conus2_transient_box.yaml
+-rw-r--r--   0        0        0    11384 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/conus2_transient_solid.yaml
+-rw-r--r--   0        0        0     3383 1970-01-01 00:00:00.000000 subsettools-1.0.5/PKG-INFO
```

### Comparing `subsettools-1.0.4/LICENSE` & `subsettools-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.4/README.md` & `subsettools-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.4/pyproject.toml` & `subsettools-1.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 [tool.poetry]
 name = "subsettools"
-version = "1.0.4"
+version = "1.0.5"
 description = "Subsetting tools and utilities for ParFlow"
 authors = ["George Artavanis, Amanda Triplett"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 numpy = ">=1.23.0"
 pytz = ">=2020.1"
 requests = ">=2.28.2"
 pftools = ">=1.3.10"
-hf-hydrodata = ">=1.0.8"
+hf-hydrodata = ">=1.1.9"
+pylint = "^3.1.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
-pylint = "^2.17.5"
 jupyter = "^1.0.0"
 matplotlib = "^3.7.2"
 black = "^23.9.1"
 sphinx-autoapi = "^3.0.0"
 sphinx-rtd-theme = "^1.3.0"
 sphinx = "6.2.1"
 myst-nb = {git = "https://github.com/executablebooks/MyST-NB.git"}
 
+[tool.pylint.messages_control]
+generated-members = ["domain", "domaininput", "indi_input"]
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `subsettools-1.0.4/src/subsettools/_error_checking.py` & `subsettools-1.0.5/src/subsettools/_error_checking.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-"""This module contains helper functions for error-checking user-provided arguments.
-"""
+"""This module contains helper functions for error-checking user-provided arguments."""
 
-import os 
+import os
 import re
+import numpy as np
+
 
 def _validate_huc_list(huc_list):
     """Check errors for a user-provided list of HUC IDs."""
     if not isinstance(huc_list, list):
         raise TypeError("huc_list must be a list.")
     if not all(isinstance(huc, str) for huc in huc_list):
         raise TypeError("All elements of huc_list must be strings")
     if not all(huc.isdigit() for huc in huc_list):
         raise ValueError("HUC IDs must contain only digits")
     huc_len = len(huc_list[0])
     if huc_len not in [2, 4, 6, 8, 10]:
         raise ValueError("HUC IDs are 2, 4, 6, 8, or 10-digit")
-    if not all([len(huc) == huc_len for huc in huc_list]):
-        raise ValueError("All HUC IDs should have the same length")    
-    
+    if not all(len(huc) == huc_len for huc in huc_list):
+        raise ValueError("All HUC IDs should have the same length")
+
 
 def _validate_grid(grid):
     """Check errors for a user-provided grid argument."""
     if not isinstance(grid, str):
         raise TypeError("grid must be a string")
     grid = grid.lower()
     if grid not in ["conus1", "conus2"]:
@@ -29,34 +30,48 @@
 
 
 def _validate_latlon_list(latlon_pts):
     """Check errors for a user-provided list of latlon points."""
     if not isinstance(latlon_pts, list):
         raise TypeError("latlon argument must be a list of points")
     for point in latlon_pts:
-        if not (isinstance(point, list) and
-                len(point) == 2 and
-                all(isinstance(value, (int, float)) for value in point)):
-            raise ValueError("Each element of the list must be a list of two floats of the form [lat, lon]")
+        if not (
+            isinstance(point, list)
+            and len(point) == 2
+            and all(isinstance(value, (int, float)) for value in point)
+        ):
+            raise ValueError(
+                "Each element of the list must be a list of two floats of the form [lat, lon]"
+            )
+
 
-    
 def _validate_dir(dir_name):
     """Check that dir_name is a valid directory."""
     if not os.path.isdir(dir_name):
-        raise FileNotFoundError(f"{dir_name} is not a valid existing directory") 
+        raise FileNotFoundError(f"{dir_name} is not a valid existing directory")
 
 
 def _validate_grid_bounds(grid_bounds):
     if not isinstance(grid_bounds, tuple):
         raise TypeError("bounds must be a tuple.")
     if not all(isinstance(val, (int, float)) for val in grid_bounds):
         raise TypeError("bounds must contain integers or floats.")
     if not len(grid_bounds) == 4:
         raise ValueError("bounds must contain four elements (imin, imax, jmin, jmax).")
 
-    
+
 def _validate_date(date):
     if not isinstance(date, str):
         raise TypeError("date must be a string.")
-    pattern = re.compile(r'\d{4}-\d{2}-\d{2}$')
+    pattern = re.compile(r"\d{4}-\d{2}-\d{2}$")
     if not bool(pattern.match(date)):
         raise ValueError("invalid date format.")
+
+
+def _validate_mask(mask):
+    if not isinstance(mask, np.ndarray):
+        raise ValueError("mask must be a numpy array.")
+    if not np.issubdtype(mask.dtype, np.integer):
+        raise ValueError("mask elements must be integers.")
+    unique_values = np.unique(mask)
+    if len(unique_values) != 2 or (0 not in unique_values) or (1 not in unique_values):
+        raise ValueError("mask elements must be 0 or 1.")
```

### Comparing `subsettools-1.0.4/src/subsettools/ref_yamls/conus1_pf_spinup_box.yaml` & `subsettools-1.0.5/src/subsettools/template_runscripts/conus1_spinup_box.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.4/src/subsettools/ref_yamls/conus1_pf_spinup_solid.yaml` & `subsettools-1.0.5/src/subsettools/template_runscripts/conus1_spinup_solid.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.4/src/subsettools/ref_yamls/conus1_pfclm_transient_box.yaml` & `subsettools-1.0.5/src/subsettools/template_runscripts/conus1_transient_box.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.4/src/subsettools/ref_yamls/conus1_pfclm_transient_solid.yaml` & `subsettools-1.0.5/src/subsettools/template_runscripts/conus1_transient_solid.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.4/src/subsettools/ref_yamls/conus2_pf_spinup_box.yaml` & `subsettools-1.0.5/src/subsettools/template_runscripts/conus2_spinup_box.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.4/src/subsettools/ref_yamls/conus2_pf_spinup_solid.yaml` & `subsettools-1.0.5/src/subsettools/template_runscripts/conus2_spinup_solid.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.4/src/subsettools/ref_yamls/conus2_pfclm_transient_box.yaml` & `subsettools-1.0.5/src/subsettools/template_runscripts/conus2_transient_box.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.4/src/subsettools/ref_yamls/conus2_pfclm_transient_solid.yaml` & `subsettools-1.0.5/src/subsettools/template_runscripts/conus2_transient_solid.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.4/PKG-INFO` & `subsettools-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: subsettools
-Version: 1.0.4
+Version: 1.0.5
 Summary: Subsetting tools and utilities for ParFlow
 License: MIT
 Author: George Artavanis, Amanda Triplett
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hf-hydrodata (>=1.0.8)
+Requires-Dist: hf-hydrodata (>=1.1.9)
 Requires-Dist: numpy (>=1.23.0)
 Requires-Dist: pftools (>=1.3.10)
+Requires-Dist: pylint (>=3.1.0,<4.0.0)
 Requires-Dist: pytz (>=2020.1)
 Requires-Dist: requests (>=2.28.2)
 Description-Content-Type: text/markdown
 
 # SubsetTools
 
 ## Introduction
```

