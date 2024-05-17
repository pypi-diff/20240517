# Comparing `tmp/game_generators-0.1.4.tar.gz` & `tmp/game_generators-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "game_generators-0.1.4.tar", max compression
+gzip compressed data, was "game_generators-0.1.5.tar", max compression
```

## Comparing `game_generators-0.1.4.tar` & `game_generators-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1069 2023-05-05 12:09:35.137241 game_generators-0.1.4/LICENSE
--rw-r--r--   0        0        0     2776 2024-02-12 15:39:26.386891 game_generators-0.1.4/README.md
--rw-r--r--   0        0        0      268 2024-02-12 15:39:48.773435 game_generators-0.1.4/game_generators/__init__.py
--rw-r--r--   0        0        0     1308 2024-02-12 15:38:16.190643 game_generators-0.1.4/game_generators/functions/__init__.py
--rw-r--r--   0        0        0     1194 2023-11-15 09:37:28.878448 game_generators-0.1.4/game_generators/functions/ces.py
--rw-r--r--   0        0        0     1269 2023-10-25 11:03:39.887926 game_generators-0.1.4/game_generators/functions/cobb_douglas.py
--rw-r--r--   0        0        0     4822 2024-05-09 12:03:53.282039 game_generators-0.1.4/game_generators/functions/concave.py
--rw-r--r--   0        0        0     1806 2024-05-17 19:55:11.877075 game_generators-0.1.4/game_generators/functions/interpolate.py
--rw-r--r--   0        0        0     1167 2023-10-23 12:01:29.305269 game_generators-0.1.4/game_generators/functions/leontief.py
--rw-r--r--   0        0        0      756 2023-11-15 12:34:36.098344 game_generators-0.1.4/game_generators/functions/linear.py
--rw-r--r--   0        0        0     9203 2024-05-09 12:03:53.283054 game_generators-0.1.4/game_generators/functions/monotonic.py
--rw-r--r--   0        0        0     1263 2023-11-15 09:37:28.878115 game_generators-0.1.4/game_generators/functions/polynomial.py
--rw-r--r--   0        0        0      124 2023-11-15 12:34:36.104940 game_generators-0.1.4/game_generators/multi_objective/__init__.py
--rw-r--r--   0        0        0     1068 2024-02-12 15:34:16.243350 game_generators-0.1.4/game_generators/multi_objective/from_nfg.py
--rw-r--r--   0        0        0     1096 2023-11-15 09:42:36.987001 game_generators-0.1.4/game_generators/multi_objective/identity.py
--rw-r--r--   0        0        0     2486 2023-11-15 12:43:17.989931 game_generators-0.1.4/game_generators/nfg/__init__.py
--rw-r--r--   0        0        0     1914 2023-11-15 12:34:36.101820 game_generators-0.1.4/game_generators/nfg/bach_stravinsky.py
--rw-r--r--   0        0        0     1927 2023-11-15 09:37:28.878672 game_generators-0.1.4/game_generators/nfg/bertrand_oligopoly.py
--rw-r--r--   0        0        0     1342 2023-11-15 12:34:36.122995 game_generators-0.1.4/game_generators/nfg/chicken.py
--rw-r--r--   0        0        0     3622 2023-11-15 09:37:28.878741 game_generators-0.1.4/game_generators/nfg/congestion.py
--rw-r--r--   0        0        0     1568 2023-11-15 09:37:28.878129 game_generators-0.1.4/game_generators/nfg/covariant.py
--rw-r--r--   0        0        0     1037 2023-11-15 09:37:28.877303 game_generators-0.1.4/game_generators/nfg/discrete_uniform.py
--rw-r--r--   0        0        0     1525 2023-11-15 12:36:26.183595 game_generators-0.1.4/game_generators/nfg/grab_the_dollar.py
--rw-r--r--   0        0        0     1368 2023-11-15 12:36:26.181681 game_generators-0.1.4/game_generators/nfg/hawk_dove.py
--rw-r--r--   0        0        0     1782 2023-11-15 09:25:46.506513 game_generators-0.1.4/game_generators/nfg/majority_voting.py
--rw-r--r--   0        0        0     3379 2023-11-15 12:36:26.177852 game_generators-0.1.4/game_generators/nfg/potential.py
--rw-r--r--   0        0        0     1011 2023-11-15 09:25:46.507233 game_generators-0.1.4/game_generators/nfg/random_uniform.py
--rw-r--r--   0        0        0     1855 2023-11-15 09:37:28.876831 game_generators-0.1.4/game_generators/nfg/war_of_attrition.py
--rw-r--r--   0        0        0     1460 2023-11-15 09:37:28.878496 game_generators-0.1.4/game_generators/nfg/zero_sum.py
--rw-r--r--   0        0        0        0 2023-02-26 16:08:20.449778 game_generators-0.1.4/game_generators/utils/__init__.py
--rw-r--r--   0        0        0     1442 2023-11-15 09:37:28.878460 game_generators-0.1.4/game_generators/utils/data.py
--rw-r--r--   0        0        0     1467 2023-11-15 09:25:46.508184 game_generators-0.1.4/game_generators/utils/generators.py
--rw-r--r--   0        0        0      585 2023-11-15 09:03:13.506605 game_generators-0.1.4/game_generators/utils/transforms.py
--rw-r--r--   0        0        0     2276 2023-11-15 12:36:26.179855 game_generators-0.1.4/game_generators/utils/visualisation.py
--rw-r--r--   0        0        0      490 2024-05-17 19:56:08.451735 game_generators-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3556 1970-01-01 00:00:00.000000 game_generators-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-05 12:09:35.137241 game_generators-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2776 2024-02-12 15:39:26.386891 game_generators-0.1.5/README.md
+-rw-r--r--   0        0        0      268 2024-02-12 15:39:48.773435 game_generators-0.1.5/game_generators/__init__.py
+-rw-r--r--   0        0        0     1308 2024-02-12 15:38:16.190643 game_generators-0.1.5/game_generators/functions/__init__.py
+-rw-r--r--   0        0        0     1194 2023-11-15 09:37:28.878448 game_generators-0.1.5/game_generators/functions/ces.py
+-rw-r--r--   0        0        0     1269 2023-10-25 11:03:39.887926 game_generators-0.1.5/game_generators/functions/cobb_douglas.py
+-rw-r--r--   0        0        0     5232 2024-05-17 20:00:37.117606 game_generators-0.1.5/game_generators/functions/concave.py
+-rw-r--r--   0        0        0     1806 2024-05-17 19:55:11.877075 game_generators-0.1.5/game_generators/functions/interpolate.py
+-rw-r--r--   0        0        0     1167 2023-10-23 12:01:29.305269 game_generators-0.1.5/game_generators/functions/leontief.py
+-rw-r--r--   0        0        0      756 2023-11-15 12:34:36.098344 game_generators-0.1.5/game_generators/functions/linear.py
+-rw-r--r--   0        0        0     9949 2024-05-17 20:00:37.117654 game_generators-0.1.5/game_generators/functions/monotonic.py
+-rw-r--r--   0        0        0     1263 2023-11-15 09:37:28.878115 game_generators-0.1.5/game_generators/functions/polynomial.py
+-rw-r--r--   0        0        0      124 2023-11-15 12:34:36.104940 game_generators-0.1.5/game_generators/multi_objective/__init__.py
+-rw-r--r--   0        0        0     1068 2024-02-12 15:34:16.243350 game_generators-0.1.5/game_generators/multi_objective/from_nfg.py
+-rw-r--r--   0        0        0     1096 2023-11-15 09:42:36.987001 game_generators-0.1.5/game_generators/multi_objective/identity.py
+-rw-r--r--   0        0        0     2486 2023-11-15 12:43:17.989931 game_generators-0.1.5/game_generators/nfg/__init__.py
+-rw-r--r--   0        0        0     1914 2023-11-15 12:34:36.101820 game_generators-0.1.5/game_generators/nfg/bach_stravinsky.py
+-rw-r--r--   0        0        0     1927 2023-11-15 09:37:28.878672 game_generators-0.1.5/game_generators/nfg/bertrand_oligopoly.py
+-rw-r--r--   0        0        0     1342 2023-11-15 12:34:36.122995 game_generators-0.1.5/game_generators/nfg/chicken.py
+-rw-r--r--   0        0        0     3622 2023-11-15 09:37:28.878741 game_generators-0.1.5/game_generators/nfg/congestion.py
+-rw-r--r--   0        0        0     1568 2023-11-15 09:37:28.878129 game_generators-0.1.5/game_generators/nfg/covariant.py
+-rw-r--r--   0        0        0     1037 2023-11-15 09:37:28.877303 game_generators-0.1.5/game_generators/nfg/discrete_uniform.py
+-rw-r--r--   0        0        0     1525 2023-11-15 12:36:26.183595 game_generators-0.1.5/game_generators/nfg/grab_the_dollar.py
+-rw-r--r--   0        0        0     1368 2023-11-15 12:36:26.181681 game_generators-0.1.5/game_generators/nfg/hawk_dove.py
+-rw-r--r--   0        0        0     1782 2023-11-15 09:25:46.506513 game_generators-0.1.5/game_generators/nfg/majority_voting.py
+-rw-r--r--   0        0        0     3379 2023-11-15 12:36:26.177852 game_generators-0.1.5/game_generators/nfg/potential.py
+-rw-r--r--   0        0        0     1011 2023-11-15 09:25:46.507233 game_generators-0.1.5/game_generators/nfg/random_uniform.py
+-rw-r--r--   0        0        0     1855 2023-11-15 09:37:28.876831 game_generators-0.1.5/game_generators/nfg/war_of_attrition.py
+-rw-r--r--   0        0        0     1460 2023-11-15 09:37:28.878496 game_generators-0.1.5/game_generators/nfg/zero_sum.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:08:20.449778 game_generators-0.1.5/game_generators/utils/__init__.py
+-rw-r--r--   0        0        0     1442 2023-11-15 09:37:28.878460 game_generators-0.1.5/game_generators/utils/data.py
+-rw-r--r--   0        0        0     1467 2023-11-15 09:25:46.508184 game_generators-0.1.5/game_generators/utils/generators.py
+-rw-r--r--   0        0        0      585 2023-11-15 09:03:13.506605 game_generators-0.1.5/game_generators/utils/transforms.py
+-rw-r--r--   0        0        0     2276 2023-11-15 12:36:26.179855 game_generators-0.1.5/game_generators/utils/visualisation.py
+-rw-r--r--   0        0        0      490 2024-05-17 20:00:53.946557 game_generators-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3556 1970-01-01 00:00:00.000000 game_generators-0.1.5/PKG-INFO
```

### Comparing `game_generators-0.1.4/LICENSE` & `game_generators-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/README.md` & `game_generators-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/functions/__init__.py` & `game_generators-0.1.5/game_generators/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/functions/ces.py` & `game_generators-0.1.5/game_generators/functions/ces.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/functions/cobb_douglas.py` & `game_generators-0.1.5/game_generators/functions/cobb_douglas.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/functions/concave.py` & `game_generators-0.1.5/game_generators/functions/concave.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,32 +66,53 @@
     max_values = concave_table[(slice(None),) + ((-1,) * dim)].reshape(batch_size, *([1] * dim))
 
     # Scale the table to the desired range
     return scale_array(concave_table, min_values, max_values, min_y, max_y)
 
 
 def concave(
-    dim, min_vec=None, max_vec=None, min_y=0, max_y=10, batch_size=1, batched=True, num_points=10, rng=None, seed=None
+    dim,
+    min_vec=None,
+    max_vec=None,
+    min_y=0,
+    max_y=10,
+    batch_size=1,
+    batched=True,
+    num_points=10,
+    bounds_error=True,
+    fill_value=None,
+    rng=None,
+    seed=None,
 ):
     """Generate a random concave, monotonically increasing, function.
 
     Args:
         dim (int): The dimension of the function.
         min_vec (np.ndarray, optional): The minimum value for each dimension. Defaults to None.
         max_vec (np.ndarray, optional): The maximum value for each dimension. Defaults to None.
         min_y (int, optional): The minimum y value. Defaults to 0.
         max_y (int, optional): The maximum y value. Defaults to 10.
         batch_size (int, optional): The batch size. Defaults to 1.
         batched (bool, optional): Whether to return a batched function. Defaults to True.
         num_points (int, optional): The number of points. Defaults to 10.
+        bounds_error (bool, optional): Whether to raise an error if the input is out of bounds. Defaults to True.
+        fill_value (float, optional): The fill value used for out of bounds values. Defaults to None.
         rng (np.random.Generator, optional): The random number generator. Defaults to None.
         seed (int, optional): The random seed. Defaults to None.
 
     Returns:
         list | callable: A collection of of concave functions or a single concave function.
     """
     concave_t = concave_table(dim, batch_size, min_y, max_y, num_points, rng, seed)
     batched = batch_size > 1 or batched
     if not batched:
         concave_t = concave_t[0]
-    concave_f = interpolate_table(concave_t, min_vec=min_vec, max_vec=max_vec, batched=batched, method="linear")
+    concave_f = interpolate_table(
+        concave_t,
+        min_vec=min_vec,
+        max_vec=max_vec,
+        batched=batched,
+        method="linear",
+        bounds_error=bounds_error,
+        fill_value=fill_value,
+    )
     return concave_f
```

### Comparing `game_generators-0.1.4/game_generators/functions/interpolate.py` & `game_generators-0.1.5/game_generators/functions/interpolate.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/functions/leontief.py` & `game_generators-0.1.5/game_generators/functions/leontief.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/functions/linear.py` & `game_generators-0.1.5/game_generators/functions/linear.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/functions/monotonic.py` & `game_generators-0.1.5/game_generators/functions/monotonic.py`

 * *Files 7% similar despite different names*

```diff
@@ -136,14 +136,16 @@
     min_vec=None,
     max_vec=None,
     min_y=0,
     max_y=10,
     batch_size=1,
     batched=True,
     num_points=10,
+    bounds_error=True,
+    fill_value=None,
     rng=None,
     seed=None,
 ):
     """Create an increasing function.
 
     Args:
         dim (int): The dimension of the function.
@@ -153,14 +155,16 @@
         min_vec (np.array, optional): The minimum input values. Defaults to None.
         max_vec (np.array, optional): The maximum input values. Defaults to None.
         min_y (int, optional): The minimum value. Defaults to 0.
         max_y (int, optional): The maximum value. Defaults to 10.
         batch_size (int, optional): The batch size. Defaults to 1.
         batched (bool, optional): Whether the function is batched or not. Defaults to True.
         num_points (int, optional): The number of points. Defaults to 10.
+        bounds_error (bool, optional): Whether to raise an error if the input is out of bounds. Defaults to True.
+        fill_value (float, optional): The fill value used for out of bounds values. Defaults to None.
         rng (np.random.Generator, optional): The random number generator. Defaults to None.
         seed (int, optional): The random seed. Defaults to None.
 
     Returns:
         callable: An increasing function.
     """
     values = increasing_table(
@@ -173,29 +177,39 @@
         num_points=num_points,
         rng=rng,
         seed=seed,
     )
     batched = batch_size > 1 or batched
     if not batched:
         values = values[0]
-    increasing_f = interpolate_table(values, min_vec=min_vec, max_vec=max_vec, batched=batched, method="linear")
+    increasing_f = interpolate_table(
+        values,
+        min_vec=min_vec,
+        max_vec=max_vec,
+        batched=batched,
+        method="linear",
+        bounds_error=bounds_error,
+        fill_value=fill_value,
+    )
     return increasing_f
 
 
 def decreasing(
     dim,
     max_grad=5,
     method="cumsum",
     min_vec=None,
     max_vec=None,
     min_y=0,
     max_y=10,
     batch_size=1,
     batched=True,
     num_points=10,
+    bounds_error=True,
+    fill_value=None,
     rng=None,
     seed=None,
 ):
     """Create a decreasing function.
 
     Args:
         dim (int): The dimension of the function.
@@ -205,14 +219,16 @@
         min_vec (np.array, optional): The minimum input values. Defaults to None.
         max_vec (np.array, optional): The maximum input values. Defaults to None.
         min_y (int, optional): The minimum value. Defaults to 0.
         max_y (int, optional): The maximum value. Defaults to 10.
         batch_size (int, optional): The batch size. Defaults to 1.
         batched (bool, optional): Whether the function is batched or not. Defaults to True.
         num_points (int, optional): The number of points. Defaults to 10.
+        bounds_error (bool, optional): Whether to raise an error if the input is out of bounds. Defaults to True.
+        fill_value (float, optional): The fill value used for out of bounds values. Defaults to None.
         rng (np.random.Generator, optional): The random number generator. Defaults to None.
         seed (int, optional): The random seed. Defaults to None.
 
     Returns:
         callable: A decreasing function.
     """
     values = decreasing_table(
@@ -225,9 +241,17 @@
         num_points=num_points,
         rng=rng,
         seed=seed,
     )
     batched = batch_size > 1 or batched
     if not batched:
         values = values[0]
-    decreasing_f = interpolate_table(values, min_vec=min_vec, max_vec=max_vec, batched=batched, method="linear")
+    decreasing_f = interpolate_table(
+        values,
+        min_vec=min_vec,
+        max_vec=max_vec,
+        batched=batched,
+        method="linear",
+        bounds_error=bounds_error,
+        fill_value=fill_value,
+    )
     return decreasing_f
```

### Comparing `game_generators-0.1.4/game_generators/functions/polynomial.py` & `game_generators-0.1.5/game_generators/functions/polynomial.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/multi_objective/from_nfg.py` & `game_generators-0.1.5/game_generators/multi_objective/from_nfg.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/multi_objective/identity.py` & `game_generators-0.1.5/game_generators/multi_objective/identity.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/nfg/__init__.py` & `game_generators-0.1.5/game_generators/nfg/__init__.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/nfg/bach_stravinsky.py` & `game_generators-0.1.5/game_generators/nfg/bach_stravinsky.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/nfg/bertrand_oligopoly.py` & `game_generators-0.1.5/game_generators/nfg/bertrand_oligopoly.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/nfg/chicken.py` & `game_generators-0.1.5/game_generators/nfg/chicken.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/nfg/congestion.py` & `game_generators-0.1.5/game_generators/nfg/congestion.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/nfg/covariant.py` & `game_generators-0.1.5/game_generators/nfg/covariant.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/nfg/discrete_uniform.py` & `game_generators-0.1.5/game_generators/nfg/discrete_uniform.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/nfg/grab_the_dollar.py` & `game_generators-0.1.5/game_generators/nfg/grab_the_dollar.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/nfg/hawk_dove.py` & `game_generators-0.1.5/game_generators/nfg/hawk_dove.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/nfg/majority_voting.py` & `game_generators-0.1.5/game_generators/nfg/majority_voting.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/nfg/potential.py` & `game_generators-0.1.5/game_generators/nfg/potential.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/nfg/random_uniform.py` & `game_generators-0.1.5/game_generators/nfg/random_uniform.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/nfg/war_of_attrition.py` & `game_generators-0.1.5/game_generators/nfg/war_of_attrition.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/nfg/zero_sum.py` & `game_generators-0.1.5/game_generators/nfg/zero_sum.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/utils/data.py` & `game_generators-0.1.5/game_generators/utils/data.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/utils/generators.py` & `game_generators-0.1.5/game_generators/utils/generators.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/utils/transforms.py` & `game_generators-0.1.5/game_generators/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/game_generators/utils/visualisation.py` & `game_generators-0.1.5/game_generators/utils/visualisation.py`

 * *Files identical despite different names*

### Comparing `game_generators-0.1.4/PKG-INFO` & `game_generators-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: game-generators
-Version: 0.1.4
+Version: 0.1.5
 Summary: Efficiently generate games for research and experimentation
 Home-page: https://github.com/wilrop/game-generators
 License: MIT
 Author: Willem Röpke
 Author-email: willem.ropke@vub.be
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

