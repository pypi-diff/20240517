# Comparing `tmp/prophetverse-0.1.0.tar.gz` & `tmp/prophetverse-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophetverse-0.1.0.tar", max compression
+gzip compressed data, was "prophetverse-0.1.1.tar", max compression
```

## Comparing `prophetverse-0.1.0.tar` & `prophetverse-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2024-05-13 00:11:34.893268 prophetverse-0.1.0/LICENSE
--rw-r--r--   0        0        0     4550 2024-05-13 00:11:34.893268 prophetverse-0.1.0/README.md
--rw-r--r--   0        0        0      669 2024-05-13 00:11:44.161242 prophetverse-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       61 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/__init__.py
--rw-r--r--   0        0        0      732 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/distributions.py
--rw-r--r--   0        0        0     8336 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/effects.py
--rw-r--r--   0        0        0     6688 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/engine.py
--rw-r--r--   0        0        0       59 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/logger.py
--rw-r--r--   0        0        0     7009 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/models.py
--rw-r--r--   0        0        0       72 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/sktime/__init__.py
--rw-r--r--   0        0        0     4701 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/sktime/_expand_column_per_level.py
--rw-r--r--   0        0        0    14213 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/sktime/base.py
--rw-r--r--   0        0        0    15371 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/sktime/multivariate.py
--rw-r--r--   0        0        0     2054 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/sktime/seasonality.py
--rw-r--r--   0        0        0    19480 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/sktime/univariate.py
--rw-r--r--   0        0        0       25 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/trend/__init__.py
--rw-r--r--   0        0        0     2863 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/trend/base.py
--rw-r--r--   0        0        0     1139 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/trend/flat.py
--rw-r--r--   0        0        0    16632 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/trend/piecewise.py
--rw-r--r--   0        0        0       77 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/utils/__init__.py
--rw-r--r--   0        0        0     4309 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/utils/frame_to_array.py
--rw-r--r--   0        0        0      988 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/utils/multiindex.py
--rw-r--r--   0        0        0      802 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/utils/regex.py
--rw-r--r--   0        0        0     5093 1970-01-01 00:00:00.000000 prophetverse-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-17 12:10:19.262134 prophetverse-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4550 2024-05-17 12:10:19.262134 prophetverse-0.1.1/README.md
+-rw-r--r--   0        0        0      669 2024-05-17 12:10:28.418141 prophetverse-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/__init__.py
+-rw-r--r--   0        0        0      732 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/distributions.py
+-rw-r--r--   0        0        0     8336 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/effects.py
+-rw-r--r--   0        0        0     6688 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/engine.py
+-rw-r--r--   0        0        0       59 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/logger.py
+-rw-r--r--   0        0        0     7009 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/models.py
+-rw-r--r--   0        0        0       72 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/sktime/__init__.py
+-rw-r--r--   0        0        0     4701 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/sktime/_expand_column_per_level.py
+-rw-r--r--   0        0        0    14213 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/sktime/base.py
+-rw-r--r--   0        0        0    15976 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/sktime/multivariate.py
+-rw-r--r--   0        0        0     2054 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/sktime/seasonality.py
+-rw-r--r--   0        0        0    20354 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/sktime/univariate.py
+-rw-r--r--   0        0        0       25 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/trend/__init__.py
+-rw-r--r--   0        0        0     2863 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/trend/base.py
+-rw-r--r--   0        0        0     1139 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/trend/flat.py
+-rw-r--r--   0        0        0    16279 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/trend/piecewise.py
+-rw-r--r--   0        0        0       77 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/utils/__init__.py
+-rw-r--r--   0        0        0     4309 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/utils/frame_to_array.py
+-rw-r--r--   0        0        0      988 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/utils/multiindex.py
+-rw-r--r--   0        0        0      802 2024-05-17 12:10:19.286134 prophetverse-0.1.1/src/prophetverse/utils/regex.py
+-rw-r--r--   0        0        0     5093 1970-01-01 00:00:00.000000 prophetverse-0.1.1/PKG-INFO
```

### Comparing `prophetverse-0.1.0/LICENSE` & `prophetverse-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prophetverse-0.1.0/README.md` & `prophetverse-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `prophetverse-0.1.0/pyproject.toml` & `prophetverse-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prophetverse"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Felipe Angelim <felipeangelim@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "prophetverse", from="src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
```

### Comparing `prophetverse-0.1.0/src/prophetverse/distributions.py` & `prophetverse-0.1.1/src/prophetverse/distributions.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.1.0/src/prophetverse/effects.py` & `prophetverse-0.1.1/src/prophetverse/effects.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.1.0/src/prophetverse/engine.py` & `prophetverse-0.1.1/src/prophetverse/engine.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.1.0/src/prophetverse/models.py` & `prophetverse-0.1.1/src/prophetverse/models.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.1.0/src/prophetverse/sktime/_expand_column_per_level.py` & `prophetverse-0.1.1/src/prophetverse/sktime/_expand_column_per_level.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.1.0/src/prophetverse/sktime/base.py` & `prophetverse-0.1.1/src/prophetverse/sktime/base.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.1.0/src/prophetverse/sktime/multivariate.py` & `prophetverse-0.1.1/src/prophetverse/sktime/multivariate.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     Args:
         changepoint_interval (int): The number of points between each potential changepoint.
         changepoint_range (float): Proportion of the history in which trend changepoints will be estimated.
                                    If a float between 0 and 1, the range will be that proportion of the history.
                                    If an int, the range will be that number of points. A negative int indicates number of points
                                    counting from the end of the history.
         changepoint_prior_scale (float): Parameter controlling the flexibility of the automatic changepoint selection.
+        offset_prior_scale (float): Scale parameter for the prior distribution of the offset. Default is 0.1.
         capacity_prior_scale (float): Scale parameter for the capacity prior. Defaults to 0.2.
         capacity_prior_loc (float): Location parameter for the capacity prior. Defaults to 1.1.
         trend (str): Type of trend. Either "linear" or "logistic". Defaults to "linear".
         feature_transformer (BaseTransformer or None): A transformer to preprocess the exogenous features. Defaults to None.
         exogenous_effects (List[AbstractEffect]): A list defining the exogenous effects to be used in the model.
         default_effect (AbstractEffect): The default effect to be used when no effect is specified for a variable.
         shared_features (list): List of shared features across series. Defaults to an empty list.
@@ -91,14 +92,15 @@
     }
 
     def __init__(
         self,
         changepoint_interval=25,
         changepoint_range=0.8,
         changepoint_prior_scale=0.1,
+        offset_prior_scale=0.1,
         capacity_prior_scale=0.2,
         capacity_prior_loc=1.1,
         trend="linear",
         feature_transformer: BaseTransformer = None,
         exogenous_effects=None,
         default_effect=None,
         shared_features=None,
@@ -113,14 +115,15 @@
         correlation_matrix_concentration=1.0,
         rng_key=None,
     ):
 
         self.changepoint_interval = changepoint_interval
         self.changepoint_range = changepoint_range
         self.changepoint_prior_scale = changepoint_prior_scale
+        self.offset_prior_scale = offset_prior_scale
         self.noise_scale = noise_scale
         self.capacity_prior_scale = capacity_prior_scale
         self.capacity_prior_loc = capacity_prior_loc
         self.trend = trend
         self.shared_features = shared_features
         self.feature_transformer = feature_transformer
         self.correlation_matrix_concentration = correlation_matrix_concentration
@@ -152,14 +155,20 @@
             raise ValueError("changepoint_prior_scale must be greater than 0.")
         if self.noise_scale <= 0:
             raise ValueError("noise_scale must be greater than 0.")
         if self.capacity_prior_scale <= 0:
             raise ValueError("capacity_prior_scale must be greater than 0.")
         if self.capacity_prior_loc <= 0:
             raise ValueError("capacity_prior_loc must be greater than 0.")
+        if self.offset_prior_scale <= 0:
+            raise ValueError("offset_prior_scale must be greater than 0.")
+        if self.correlation_matrix_concentration <= 0:
+            raise ValueError(
+                "correlation_matrix_concentration must be greater than 0."
+            )
 
         if self.trend not in ["linear", "logistic"]:
             raise ValueError('trend must be either "linear" or "logistic".')
 
     def _get_fit_data(self, y, X, fh):
         """
         Prepare the data for the NumPyro model.
@@ -188,22 +197,24 @@
 
         ## Changepoints and trend
         if self.trend == "linear":
             self.trend_model_ = PiecewiseLinearTrend(
                 changepoint_interval=self.changepoint_interval,
                 changepoint_range=self.changepoint_range,
                 changepoint_prior_scale=self.changepoint_prior_scale,
+                offset_prior_scale=self.offset_prior_scale,
                 squeeze_if_single_series=False,
             )
 
         elif self.trend == "logistic":
             self.trend_model_ = PiecewiseLogisticTrend(
                 changepoint_interval=self.changepoint_interval,
                 changepoint_range=self.changepoint_range,
                 changepoint_prior_scale=self.changepoint_prior_scale,
+                offset_prior_scale=self.offset_prior_scale,
                 capacity_prior=dist.TransformedDistribution(
                     dist.HalfNormal(self.capacity_prior_scale),
                     dist.transforms.AffineTransform(
                         loc=self.capacity_prior_loc, scale=1
                     ),
                 ),
                 squeeze_if_single_series=False,
```

### Comparing `prophetverse-0.1.0/src/prophetverse/sktime/seasonality.py` & `prophetverse-0.1.1/src/prophetverse/sktime/seasonality.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.1.0/src/prophetverse/sktime/univariate.py` & `prophetverse-0.1.1/src/prophetverse/sktime/univariate.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     Args:
         changepoint_interval (int): The number of points between each potential changepoint.
         changepoint_range (float): Proportion of the history in which trend changepoints will be estimated. 
                                    If a float between 0 and 1, the range will be that proportion of the history. 
                                    If an int, the range will be that number of points. A negative int indicates number of points
                                    counting from the end of the history.
         changepoint_prior_scale (float): Parameter controlling the flexibility of the automatic changepoint selection.
+        offset_prior_scale (float): Scale parameter for the prior distribution of the offset. The offset is the constant term in the piecewise trend equation. Default is 0.1.
         feature_transformer (BaseTransformer): Transformer object to generate Fourier terms, holiday or other features. Should be a sktime's Transformer
         capacity_prior_scale (float): Scale parameter for the prior distribution of the capacity.
         capacity_prior_loc (float): Location parameter for the prior distribution of the capacity.
         noise_scale (float): Scale parameter for the observation noise.
         trend (str): Type of trend to use. Can be "linear" or "logistic".
         mcmc_samples (int): Number of MCMC samples to draw.
         mcmc_warmup (int): Number of MCMC warmup steps.
@@ -75,14 +76,15 @@
     } 
 
     def __init__(
         self,
         changepoint_interval=25,
         changepoint_range=0.8,
         changepoint_prior_scale=0.001,
+        offset_prior_scale=0.1,
         feature_transformer=None,
         capacity_prior_scale=0.2,
         capacity_prior_loc=1.1,
         noise_scale=0.05,
         trend="linear",
         mcmc_samples=2000,
         mcmc_warmup=200,
@@ -98,14 +100,15 @@
         """
         Initializes the Prophet model.
         """
 
         self.changepoint_interval = changepoint_interval
         self.changepoint_range = changepoint_range
         self.changepoint_prior_scale = changepoint_prior_scale
+        self.offset_prior_scale = offset_prior_scale
         self.noise_scale = noise_scale
         self.feature_transformer = feature_transformer
         self.capacity_prior_scale = capacity_prior_scale
         self.capacity_prior_loc = capacity_prior_loc
         self.trend = trend
 
         super().__init__(
@@ -137,14 +140,16 @@
             raise ValueError("changepoint_prior_scale must be greater than 0.")
         if self.noise_scale <= 0:
             raise ValueError("noise_scale must be greater than 0.")
         if self.capacity_prior_scale <= 0:
             raise ValueError("capacity_prior_scale must be greater than 0.")
         if self.capacity_prior_loc <= 0:
             raise ValueError("capacity_prior_loc must be greater than 0.")
+        if self.offset_prior_scale <= 0:
+            raise ValueError("offset_prior_scale must be greater than 0.")
         if self.trend not in ["linear", "logistic", "flat"] and not isinstance(self.trend, TrendModel):
             raise ValueError('trend must be either "linear" or "logistic".')
 
     def _get_fit_data(self, y, X, fh):
         """
         Prepares the data for the Numpyro model.
 
@@ -249,21 +254,23 @@
 
         ## Changepoints and trend
         if self.trend == "linear":
             return PiecewiseLinearTrend(
                 changepoint_interval=self.changepoint_interval,
                 changepoint_range=self.changepoint_range,
                 changepoint_prior_scale=self.changepoint_prior_scale,
+                offset_prior_scale=self.offset_prior_scale,
             )
 
         elif self.trend == "logistic":
             return PiecewiseLogisticTrend(
                 changepoint_interval=self.changepoint_interval,
                 changepoint_range=self.changepoint_range,
                 changepoint_prior_scale=self.changepoint_prior_scale,
+                offset_prior_scale=self.offset_prior_scale,
                 capacity_prior=dist.TransformedDistribution(
                     dist.HalfNormal(self.capacity_prior_scale),
                     dist.transforms.AffineTransform(
                         loc=self.capacity_prior_loc, scale=1
                     ),
                 ),
             )
@@ -283,14 +290,15 @@
 class ProphetGamma(Prophet):
     """A subclass of Prophet that models time series data with a gamma likelihood. Useful for positive only timeseries.
 
     Args:
         changepoint_interval (int): The number of points between potential changepoints. Default is 25.
         changepoint_range (float): Proportion of history in which trend changepoints will be estimated. Default is 0.8.
         changepoint_prior_scale (float): Parameter modulating the flexibility of the automatic changepoint selection. Default is 0.001.
+        offset_prior_scale (float): Scale parameter for the prior distribution of the offset. Default is 0.1.
         feature_transformer (object): A transformer object to preprocess exogenous features. Default is None.
         capacity_prior_scale (float): Scale parameter for the capacity prior distribution. Default is 0.2.
         capacity_prior_loc (float): Location parameter for the capacity prior distribution. Default is 1.1.
         noise_scale (float): Scale parameter for the observation noise. Default is 0.05.
         trend (str): Type of trend component. Default is "logistic".
         mcmc_samples (int): Number of MCMC samples. Default is 2000.
         mcmc_warmup (int): Number of MCMC warmup steps. Default is 200.
@@ -305,14 +313,15 @@
     """
 
     def __init__(
         self,
         changepoint_interval=25,
         changepoint_range=0.8,
         changepoint_prior_scale=0.001,
+        offset_prior_scale=0.1,
         feature_transformer=None,
         capacity_prior_scale=0.2,
         capacity_prior_loc=1.1,
         noise_scale=0.05,
         trend="logistic",
         mcmc_samples=2000,
         mcmc_warmup=200,
@@ -321,19 +330,20 @@
         optimizer_name="Adam",
         optimizer_kwargs=None,
         optimizer_steps=1_000,
         exogenous_effects=None,
         default_effect=None,
         rng_key=None,
     ):
-        
+
         super().__init__(
             changepoint_interval=changepoint_interval,
             changepoint_range=changepoint_range,
             changepoint_prior_scale=changepoint_prior_scale,
+            offset_prior_scale=offset_prior_scale,
             feature_transformer=feature_transformer,
             capacity_prior_scale=capacity_prior_scale,
             capacity_prior_loc=capacity_prior_loc,
             noise_scale=noise_scale,
             trend=trend,
             mcmc_samples=mcmc_samples,
             mcmc_warmup=mcmc_warmup,
@@ -353,14 +363,15 @@
     """
     A subclass of Prophet that models time series data with a negative binomial likelihood. Useful for count data.
 
     Args:
         changepoint_interval (int): The number of points between potential changepoints. Default is 25.
         changepoint_range (float): Proportion of history in which trend changepoints will be estimated. Default is 0.8.
         changepoint_prior_scale (float): Parameter modulating the flexibility of the automatic changepoint selection. Default is 0.001.
+        offset_prior_scale (float): Scale parameter for the prior distribution of the offset. Default is 0.1.
         feature_transformer (object): A transformer object to preprocess exogenous features. Default is None.
         capacity_prior_scale (float): Scale parameter for the capacity prior distribution. Default is 0.2.
         capacity_prior_loc (float): Location parameter for the capacity prior distribution. Default is 1.1.
         noise_scale (float): Scale parameter for the observation noise. Default is 0.05.
         trend (str): Type of trend component. Default is "logistic".
         mcmc_samples (int): Number of MCMC samples. Default is 2000.
         mcmc_warmup (int): Number of MCMC warmup steps. Default is 200.
@@ -375,14 +386,15 @@
     """
 
     def __init__(
         self,
         changepoint_interval=25,
         changepoint_range=0.8,
         changepoint_prior_scale=0.001,
+        offset_prior_scale=0.1,
         feature_transformer=None,
         capacity_prior_scale=0.2,
         capacity_prior_loc=1.1,
         noise_scale=0.05,
         trend="logistic",
         mcmc_samples=2000,
         mcmc_warmup=200,
@@ -396,14 +408,15 @@
         rng_key=None,
     ):
 
         super().__init__(
             changepoint_interval=changepoint_interval,
             changepoint_range=changepoint_range,
             changepoint_prior_scale=changepoint_prior_scale,
+            offset_prior_scale=offset_prior_scale,
             feature_transformer=feature_transformer,
             capacity_prior_scale=capacity_prior_scale,
             capacity_prior_loc=capacity_prior_loc,
             noise_scale=noise_scale,
             trend=trend,
             mcmc_samples=mcmc_samples,
             mcmc_warmup=mcmc_warmup,
```

### Comparing `prophetverse-0.1.0/src/prophetverse/trend/base.py` & `prophetverse-0.1.1/src/prophetverse/trend/base.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.1.0/src/prophetverse/trend/flat.py` & `prophetverse-0.1.1/src/prophetverse/trend/flat.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.1.0/src/prophetverse/trend/piecewise.py` & `prophetverse-0.1.1/src/prophetverse/trend/piecewise.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple, Union
+from typing import Iterable, Tuple, Union
 
 import jax.numpy as jnp
 import numpy as np
 import numpyro
 import numpyro.distributions as dist
 import pandas as pd
 from sktime.transformations.series.detrend import Detrender
@@ -181,18 +181,19 @@
             None
         """
 
         if self.remove_seasonality_before_suggesting_initial_vals:
             detrender = Detrender()
             y = y - detrender.fit_transform(y)
 
-        self.global_rates, self.offset_loc = self._suggest_global_trend_and_offset(y)
+        self._global_rates, self._offset_prior_loc = self._suggest_global_trend_and_offset(y)
         self._changepoint_prior_loc, self._changepoint_prior_scale = (
-            self._get_changepoint_prior_vectors(global_rates=self.global_rates)
+            self._get_changepoint_prior_vectors(global_rates=self._global_rates)
         )
+        self._offset_prior_scale = self.offset_prior_scale
 
     def _get_changepoint_prior_vectors(
         self,
         global_rates: jnp.array,
     ) -> Tuple[jnp.array, jnp.array]:
         """
         Returns the prior vectors for the changepoint coefficients.
@@ -271,27 +272,20 @@
         Returns:
             jnp.ndarray: The computed trend.
 
         Raises:
             None
 
         """
-        
-        if isinstance(self.changepoint_prior_scale, (list, tuple)):
-            offset_scale = [x * self.offset_prior_scale for x in self.changepoint_prior_scale]
-        elif isinstance(self.changepoint_prior_scale, (int, float)):
-            offset_scale = self.changepoint_prior_scale * self.offset_prior_scale
-        else:
-            raise ValueError(f"Invalid type for changepoint_prior_scale {self.changepoint_prior_scale}")
-        
+
         offset = numpyro.sample(
             "offset",
             dist.Normal(
-                self.offset_loc,
-                offset_scale
+                self._offset_prior_loc,
+                self._offset_prior_scale
             ),
         )
 
         changepoint_coefficients = numpyro.sample(
             "changepoint_coefficients",
             dist.Laplace(self._changepoint_prior_loc, self._changepoint_prior_scale),
         )
```

### Comparing `prophetverse-0.1.0/src/prophetverse/utils/frame_to_array.py` & `prophetverse-0.1.1/src/prophetverse/utils/frame_to_array.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.1.0/src/prophetverse/utils/multiindex.py` & `prophetverse-0.1.1/src/prophetverse/utils/multiindex.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.1.0/src/prophetverse/utils/regex.py` & `prophetverse-0.1.1/src/prophetverse/utils/regex.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.1.0/PKG-INFO` & `prophetverse-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophetverse
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Felipe Angelim
 Author-email: felipeangelim@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

