# Comparing `tmp/game_generators-0.1.3.tar.gz` & `tmp/game_generators-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "game_generators-0.1.3.tar", max compression
+gzip compressed data, was "game_generators-0.1.4.tar", max compression
```

## Comparing `game_generators-0.1.3.tar` & `game_generators-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1069 2023-05-05 12:09:35.137241 game_generators-0.1.3/LICENSE
--rw-r--r--   0        0        0     2776 2024-02-12 15:39:26.386891 game_generators-0.1.3/README.md
--rw-r--r--   0        0        0      268 2024-02-12 15:39:48.773435 game_generators-0.1.3/game_generators/__init__.py
--rw-r--r--   0        0        0     1308 2024-02-12 15:38:16.190643 game_generators-0.1.3/game_generators/functions/__init__.py
--rw-r--r--   0        0        0     1194 2023-11-15 09:37:28.878448 game_generators-0.1.3/game_generators/functions/ces.py
--rw-r--r--   0        0        0     1269 2023-10-25 11:03:39.887926 game_generators-0.1.3/game_generators/functions/cobb_douglas.py
--rw-r--r--   0        0        0     4822 2024-05-09 12:03:53.282039 game_generators-0.1.3/game_generators/functions/concave.py
--rw-r--r--   0        0        0     1311 2024-05-09 12:03:53.282572 game_generators-0.1.3/game_generators/functions/interpolate.py
--rw-r--r--   0        0        0     1167 2023-10-23 12:01:29.305269 game_generators-0.1.3/game_generators/functions/leontief.py
--rw-r--r--   0        0        0      756 2023-11-15 12:34:36.098344 game_generators-0.1.3/game_generators/functions/linear.py
--rw-r--r--   0        0        0     9203 2024-05-09 12:03:53.283054 game_generators-0.1.3/game_generators/functions/monotonic.py
--rw-r--r--   0        0        0     1263 2023-11-15 09:37:28.878115 game_generators-0.1.3/game_generators/functions/polynomial.py
--rw-r--r--   0        0        0      124 2023-11-15 12:34:36.104940 game_generators-0.1.3/game_generators/multi_objective/__init__.py
--rw-r--r--   0        0        0     1068 2024-02-12 15:34:16.243350 game_generators-0.1.3/game_generators/multi_objective/from_nfg.py
--rw-r--r--   0        0        0     1096 2023-11-15 09:42:36.987001 game_generators-0.1.3/game_generators/multi_objective/identity.py
--rw-r--r--   0        0        0     2486 2023-11-15 12:43:17.989931 game_generators-0.1.3/game_generators/nfg/__init__.py
--rw-r--r--   0        0        0     1914 2023-11-15 12:34:36.101820 game_generators-0.1.3/game_generators/nfg/bach_stravinsky.py
--rw-r--r--   0        0        0     1927 2023-11-15 09:37:28.878672 game_generators-0.1.3/game_generators/nfg/bertrand_oligopoly.py
--rw-r--r--   0        0        0     1342 2023-11-15 12:34:36.122995 game_generators-0.1.3/game_generators/nfg/chicken.py
--rw-r--r--   0        0        0     3622 2023-11-15 09:37:28.878741 game_generators-0.1.3/game_generators/nfg/congestion.py
--rw-r--r--   0        0        0     1568 2023-11-15 09:37:28.878129 game_generators-0.1.3/game_generators/nfg/covariant.py
--rw-r--r--   0        0        0     1037 2023-11-15 09:37:28.877303 game_generators-0.1.3/game_generators/nfg/discrete_uniform.py
--rw-r--r--   0        0        0     1525 2023-11-15 12:36:26.183595 game_generators-0.1.3/game_generators/nfg/grab_the_dollar.py
--rw-r--r--   0        0        0     1368 2023-11-15 12:36:26.181681 game_generators-0.1.3/game_generators/nfg/hawk_dove.py
--rw-r--r--   0        0        0     1782 2023-11-15 09:25:46.506513 game_generators-0.1.3/game_generators/nfg/majority_voting.py
--rw-r--r--   0        0        0     3379 2023-11-15 12:36:26.177852 game_generators-0.1.3/game_generators/nfg/potential.py
--rw-r--r--   0        0        0     1011 2023-11-15 09:25:46.507233 game_generators-0.1.3/game_generators/nfg/random_uniform.py
--rw-r--r--   0        0        0     1855 2023-11-15 09:37:28.876831 game_generators-0.1.3/game_generators/nfg/war_of_attrition.py
--rw-r--r--   0        0        0     1460 2023-11-15 09:37:28.878496 game_generators-0.1.3/game_generators/nfg/zero_sum.py
--rw-r--r--   0        0        0        0 2023-02-26 16:08:20.449778 game_generators-0.1.3/game_generators/utils/__init__.py
--rw-r--r--   0        0        0     1442 2023-11-15 09:37:28.878460 game_generators-0.1.3/game_generators/utils/data.py
--rw-r--r--   0        0        0     1467 2023-11-15 09:25:46.508184 game_generators-0.1.3/game_generators/utils/generators.py
--rw-r--r--   0        0        0      585 2023-11-15 09:03:13.506605 game_generators-0.1.3/game_generators/utils/transforms.py
--rw-r--r--   0        0        0     2276 2023-11-15 12:36:26.179855 game_generators-0.1.3/game_generators/utils/visualisation.py
--rw-r--r--   0        0        0      490 2024-05-09 12:04:12.396913 game_generators-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3556 1970-01-01 00:00:00.000000 game_generators-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-05 12:09:35.137241 game_generators-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2776 2024-02-12 15:39:26.386891 game_generators-0.1.4/README.md
+-rw-r--r--   0        0        0      268 2024-02-12 15:39:48.773435 game_generators-0.1.4/game_generators/__init__.py
+-rw-r--r--   0        0        0     1308 2024-02-12 15:38:16.190643 game_generators-0.1.4/game_generators/functions/__init__.py
+-rw-r--r--   0        0        0     1194 2023-11-15 09:37:28.878448 game_generators-0.1.4/game_generators/functions/ces.py
+-rw-r--r--   0        0        0     1269 2023-10-25 11:03:39.887926 game_generators-0.1.4/game_generators/functions/cobb_douglas.py
+-rw-r--r--   0        0        0     4822 2024-05-09 12:03:53.282039 game_generators-0.1.4/game_generators/functions/concave.py
+-rw-r--r--   0        0        0     1806 2024-05-17 19:55:11.877075 game_generators-0.1.4/game_generators/functions/interpolate.py
+-rw-r--r--   0        0        0     1167 2023-10-23 12:01:29.305269 game_generators-0.1.4/game_generators/functions/leontief.py
+-rw-r--r--   0        0        0      756 2023-11-15 12:34:36.098344 game_generators-0.1.4/game_generators/functions/linear.py
+-rw-r--r--   0        0        0     9203 2024-05-09 12:03:53.283054 game_generators-0.1.4/game_generators/functions/monotonic.py
+-rw-r--r--   0        0        0     1263 2023-11-15 09:37:28.878115 game_generators-0.1.4/game_generators/functions/polynomial.py
+-rw-r--r--   0        0        0      124 2023-11-15 12:34:36.104940 game_generators-0.1.4/game_generators/multi_objective/__init__.py
+-rw-r--r--   0        0        0     1068 2024-02-12 15:34:16.243350 game_generators-0.1.4/game_generators/multi_objective/from_nfg.py
+-rw-r--r--   0        0        0     1096 2023-11-15 09:42:36.987001 game_generators-0.1.4/game_generators/multi_objective/identity.py
+-rw-r--r--   0        0        0     2486 2023-11-15 12:43:17.989931 game_generators-0.1.4/game_generators/nfg/__init__.py
+-rw-r--r--   0        0        0     1914 2023-11-15 12:34:36.101820 game_generators-0.1.4/game_generators/nfg/bach_stravinsky.py
+-rw-r--r--   0        0        0     1927 2023-11-15 09:37:28.878672 game_generators-0.1.4/game_generators/nfg/bertrand_oligopoly.py
+-rw-r--r--   0        0        0     1342 2023-11-15 12:34:36.122995 game_generators-0.1.4/game_generators/nfg/chicken.py
+-rw-r--r--   0        0        0     3622 2023-11-15 09:37:28.878741 game_generators-0.1.4/game_generators/nfg/congestion.py
+-rw-r--r--   0        0        0     1568 2023-11-15 09:37:28.878129 game_generators-0.1.4/game_generators/nfg/covariant.py
+-rw-r--r--   0        0        0     1037 2023-11-15 09:37:28.877303 game_generators-0.1.4/game_generators/nfg/discrete_uniform.py
+-rw-r--r--   0        0        0     1525 2023-11-15 12:36:26.183595 game_generators-0.1.4/game_generators/nfg/grab_the_dollar.py
+-rw-r--r--   0        0        0     1368 2023-11-15 12:36:26.181681 game_generators-0.1.4/game_generators/nfg/hawk_dove.py
+-rw-r--r--   0        0        0     1782 2023-11-15 09:25:46.506513 game_generators-0.1.4/game_generators/nfg/majority_voting.py
+-rw-r--r--   0        0        0     3379 2023-11-15 12:36:26.177852 game_generators-0.1.4/game_generators/nfg/potential.py
+-rw-r--r--   0        0        0     1011 2023-11-15 09:25:46.507233 game_generators-0.1.4/game_generators/nfg/random_uniform.py
+-rw-r--r--   0        0        0     1855 2023-11-15 09:37:28.876831 game_generators-0.1.4/game_generators/nfg/war_of_attrition.py
+-rw-r--r--   0        0        0     1460 2023-11-15 09:37:28.878496 game_generators-0.1.4/game_generators/nfg/zero_sum.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:08:20.449778 game_generators-0.1.4/game_generators/utils/__init__.py
+-rw-r--r--   0        0        0     1442 2023-11-15 09:37:28.878460 game_generators-0.1.4/game_generators/utils/data.py
+-rw-r--r--   0        0        0     1467 2023-11-15 09:25:46.508184 game_generators-0.1.4/game_generators/utils/generators.py
+-rw-r--r--   0        0        0      585 2023-11-15 09:03:13.506605 game_generators-0.1.4/game_generators/utils/transforms.py
+-rw-r--r--   0        0        0     2276 2023-11-15 12:36:26.179855 game_generators-0.1.4/game_generators/utils/visualisation.py
+-rw-r--r--   0        0        0      490 2024-05-17 19:56:08.451735 game_generators-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3556 1970-01-01 00:00:00.000000 game_generators-0.1.4/PKG-INFO
```

### Comparing `game_generators-0.1.3/LICENSE` & `game_generators-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/README.md` & `game_generators-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/functions/__init__.py` & `game_generators-0.1.4/game_generators/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/functions/ces.py` & `game_generators-0.1.4/game_generators/functions/ces.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/functions/cobb_douglas.py` & `game_generators-0.1.4/game_generators/functions/cobb_douglas.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/functions/concave.py` & `game_generators-0.1.4/game_generators/functions/concave.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/functions/interpolate.py` & `game_generators-0.1.4/game_generators/functions/interpolate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,51 @@
 import numpy as np
 from scipy.interpolate import RegularGridInterpolator
 
 
-def interpolate_table(table_function, min_vec=None, max_vec=None, batched=False, method="linear"):
+def interpolate_table(
+    table_function,
+    min_vec=None,
+    max_vec=None,
+    batched=False,
+    method="linear",
+    bounds_error=True,
+    fill_value=None,
+):
     """Interpolate a table function.
 
     Note:
         This function is a wrapper for scipy.interpolate.RegularGridInterpolator.
 
     Args:
         table_function (np.array): A table function.
         min_vec (np.array, optional): The minimum input values. Defaults to None.
         max_vec (np.array, optional): The maximum input values. Defaults to None.
         batched (bool, optional): Whether to return a batched interpolation function. Defaults to False.
         method (str, optional): The interpolation method. Defaults to 'linear'.
+        bounds_error (bool, optional): Whether to raise an error if the input is out of bounds. Defaults to True.
+        fill_value (float, optional): The fill value used for out of bounds values. Defaults to None.
 
     Returns:
 
     """
     if min_vec is None or max_vec is None:
         table_shape = table_function.shape if not batched else table_function.shape[1:]
         table_points = [np.arange(n) for n in table_shape]
     else:
         num_points = table_function.shape[-1]
         table_points = [np.linspace(min_v, max_v, num_points) for min_v, max_v in zip(min_vec, max_vec)]
 
     if not batched:
-        return RegularGridInterpolator(table_points, table_function, method=method)
+        return RegularGridInterpolator(
+            table_points, table_function, method=method, bounds_error=bounds_error, fill_value=fill_value
+        )
     else:
-        return [RegularGridInterpolator(table_points, table, method=method) for table in table_function]
+        return [
+            RegularGridInterpolator(
+                table_points,
+                table,
+                method=method,
+                bounds_error=bounds_error,
+            )
+            for table in table_function
+        ]
```

### Comparing `game_generators-0.1.3/game_generators/functions/leontief.py` & `game_generators-0.1.4/game_generators/functions/leontief.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/functions/linear.py` & `game_generators-0.1.4/game_generators/functions/linear.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/functions/monotonic.py` & `game_generators-0.1.4/game_generators/functions/monotonic.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/functions/polynomial.py` & `game_generators-0.1.4/game_generators/functions/polynomial.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/multi_objective/from_nfg.py` & `game_generators-0.1.4/game_generators/multi_objective/from_nfg.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/multi_objective/identity.py` & `game_generators-0.1.4/game_generators/multi_objective/identity.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/nfg/__init__.py` & `game_generators-0.1.4/game_generators/nfg/__init__.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/nfg/bach_stravinsky.py` & `game_generators-0.1.4/game_generators/nfg/bach_stravinsky.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/nfg/bertrand_oligopoly.py` & `game_generators-0.1.4/game_generators/nfg/bertrand_oligopoly.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/nfg/chicken.py` & `game_generators-0.1.4/game_generators/nfg/chicken.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/nfg/congestion.py` & `game_generators-0.1.4/game_generators/nfg/congestion.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/nfg/covariant.py` & `game_generators-0.1.4/game_generators/nfg/covariant.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/nfg/discrete_uniform.py` & `game_generators-0.1.4/game_generators/nfg/discrete_uniform.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/nfg/grab_the_dollar.py` & `game_generators-0.1.4/game_generators/nfg/grab_the_dollar.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/nfg/hawk_dove.py` & `game_generators-0.1.4/game_generators/nfg/hawk_dove.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/nfg/majority_voting.py` & `game_generators-0.1.4/game_generators/nfg/majority_voting.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/nfg/potential.py` & `game_generators-0.1.4/game_generators/nfg/potential.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/nfg/random_uniform.py` & `game_generators-0.1.4/game_generators/nfg/random_uniform.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/nfg/war_of_attrition.py` & `game_generators-0.1.4/game_generators/nfg/war_of_attrition.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/nfg/zero_sum.py` & `game_generators-0.1.4/game_generators/nfg/zero_sum.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/utils/data.py` & `game_generators-0.1.4/game_generators/utils/data.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/utils/generators.py` & `game_generators-0.1.4/game_generators/utils/generators.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/utils/transforms.py` & `game_generators-0.1.4/game_generators/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/game_generators/utils/visualisation.py` & `game_generators-0.1.4/game_generators/utils/visualisation.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.3/PKG-INFO` & `game_generators-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: game-generators
-Version: 0.1.3
+Version: 0.1.4
 Summary: Efficiently generate games for research and experimentation
 Home-page: https://github.com/wilrop/game-generators
 License: MIT
 Author: Willem Röpke
 Author-email: willem.ropke@vub.be
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

