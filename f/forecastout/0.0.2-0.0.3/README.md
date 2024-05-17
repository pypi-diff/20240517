# Comparing `tmp/forecastout-0.0.2.tar.gz` & `tmp/forecastout-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecastout-0.0.2.tar", max compression
+gzip compressed data, was "forecastout-0.0.3.tar", max compression
```

## Comparing `forecastout-0.0.2.tar` & `forecastout-0.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1065 2024-05-17 08:39:18.665160 forecastout-0.0.2/LICENSE
--rw-r--r--   0        0        0     3279 2024-05-17 08:39:18.665160 forecastout-0.0.2/README.md
--rw-r--r--   0        0        0       68 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/__init__.py
--rw-r--r--   0        0        0     1064 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/config.yaml
--rw-r--r--   0        0        0     7613 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/core.py
--rw-r--r--   0        0        0      128 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/data_engine/__init__.py
--rw-r--r--   0        0        0     5041 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/data_engine/data_handler.py
--rw-r--r--   0        0        0     1358 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/data_engine/train_test_split.py
--rw-r--r--   0        0        0      576 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/disaggregation_engine/__init__.py
--rw-r--r--   0        0        0     1154 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/disaggregation_engine/disaggregate_monthly_to_daily_forecast.py
--rw-r--r--   0        0        0      557 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/disaggregation_engine/disaggregation_model_factory.py
--rw-r--r--   0        0        0     1678 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/disaggregation_engine/disaggregation_model_predictor.py
--rw-r--r--   0        0        0      943 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/disaggregation_engine/disaggregation_model_trainer.py
--rw-r--r--   0        0        0     1035 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/disaggregation_engine/get_daily_shares.py
--rw-r--r--   0        0        0     1537 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/disaggregation_engine/remake_monthly_forecast_current_month.py
--rw-r--r--   0        0        0        0 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/disaggregation_features/__init__.py
--rw-r--r--   0        0        0     1330 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/disaggregation_features/add_features.py
--rw-r--r--   0        0        0     3092 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/disaggregation_features/feature_creator.py
--rw-r--r--   0        0        0      641 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/disaggregation_features/feature_encoding.py
--rw-r--r--   0        0        0      594 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/disaggregation_features/feature_normalizer.py
--rw-r--r--   0        0        0        0 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/disaggregation_models/__init__.py
--rw-r--r--   0        0        0      567 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/disaggregation_models/abstract_model.py
--rw-r--r--   0        0        0     2413 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/disaggregation_models/random_forest_model.py
--rw-r--r--   0        0        0      433 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/forecast_engine/__init__.py
--rw-r--r--   0        0        0     2836 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/forecast_engine/anomaly_detector.py
--rw-r--r--   0        0        0     2447 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/forecast_engine/anomaly_fixer.py
--rw-r--r--   0        0        0     2794 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/forecast_engine/backtester.py
--rw-r--r--   0        0        0      776 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/forecast_engine/decompose_time_series.py
--rw-r--r--   0        0        0      778 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/forecast_engine/ensemble_models.py
--rw-r--r--   0        0        0     2207 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/forecast_engine/ensembler.py
--rw-r--r--   0        0        0     1390 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/forecast_engine/forecast_model_factory.py
--rw-r--r--   0        0        0      906 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/forecast_engine/model_predictor.py
--rw-r--r--   0        0        0     1155 2024-05-17 08:39:18.665160 forecastout-0.0.2/forecastout/forecast_engine/model_trainer.py
--rw-r--r--   0        0        0        0 2024-05-17 08:39:18.669160 forecastout-0.0.2/forecastout/forecast_models/__init__.py
--rw-r--r--   0        0        0      442 2024-05-17 08:39:18.669160 forecastout-0.0.2/forecastout/forecast_models/abstract_model.py
--rw-r--r--   0        0        0     1497 2024-05-17 08:39:18.669160 forecastout-0.0.2/forecastout/forecast_models/autoarima_model.py
--rw-r--r--   0        0        0     3741 2024-05-17 08:39:18.669160 forecastout-0.0.2/forecastout/forecast_models/holtwinters_model.py
--rw-r--r--   0        0        0     2294 2024-05-17 08:39:18.669160 forecastout-0.0.2/forecastout/forecast_models/naive_seasonal.py
--rw-r--r--   0        0        0     1721 2024-05-17 08:39:18.669160 forecastout-0.0.2/forecastout/forecast_models/prophet_model.py
--rw-r--r--   0        0        0      114 2024-05-17 08:39:18.669160 forecastout-0.0.2/forecastout/utils/__init__.py
--rw-r--r--   0        0        0     5520 2024-05-17 08:39:18.669160 forecastout-0.0.2/forecastout/utils/input_checker.py
--rw-r--r--   0        0        0      850 2024-05-17 08:39:18.669160 forecastout-0.0.2/forecastout/utils/update_config.py
--rw-r--r--   0        0        0      991 2024-05-17 08:39:26.873082 forecastout-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 forecastout-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-17 08:47:33.235708 forecastout-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3279 2024-05-17 08:47:33.235708 forecastout-0.0.3/README.md
+-rw-r--r--   0        0        0       68 2024-05-17 08:47:33.235708 forecastout-0.0.3/forecastout/__init__.py
+-rw-r--r--   0        0        0     1064 2024-05-17 08:47:33.235708 forecastout-0.0.3/forecastout/config.yaml
+-rw-r--r--   0        0        0     7613 2024-05-17 08:47:33.235708 forecastout-0.0.3/forecastout/core.py
+-rw-r--r--   0        0        0      128 2024-05-17 08:47:33.235708 forecastout-0.0.3/forecastout/data_engine/__init__.py
+-rw-r--r--   0        0        0     5041 2024-05-17 08:47:33.235708 forecastout-0.0.3/forecastout/data_engine/data_handler.py
+-rw-r--r--   0        0        0     1358 2024-05-17 08:47:33.235708 forecastout-0.0.3/forecastout/data_engine/train_test_split.py
+-rw-r--r--   0        0        0      576 2024-05-17 08:47:33.235708 forecastout-0.0.3/forecastout/disaggregation_engine/__init__.py
+-rw-r--r--   0        0        0     1154 2024-05-17 08:47:33.235708 forecastout-0.0.3/forecastout/disaggregation_engine/disaggregate_monthly_to_daily_forecast.py
+-rw-r--r--   0        0        0      557 2024-05-17 08:47:33.235708 forecastout-0.0.3/forecastout/disaggregation_engine/disaggregation_model_factory.py
+-rw-r--r--   0        0        0     1678 2024-05-17 08:47:33.235708 forecastout-0.0.3/forecastout/disaggregation_engine/disaggregation_model_predictor.py
+-rw-r--r--   0        0        0      943 2024-05-17 08:47:33.235708 forecastout-0.0.3/forecastout/disaggregation_engine/disaggregation_model_trainer.py
+-rw-r--r--   0        0        0     1035 2024-05-17 08:47:33.235708 forecastout-0.0.3/forecastout/disaggregation_engine/get_daily_shares.py
+-rw-r--r--   0        0        0     1537 2024-05-17 08:47:33.235708 forecastout-0.0.3/forecastout/disaggregation_engine/remake_monthly_forecast_current_month.py
+-rw-r--r--   0        0        0        0 2024-05-17 08:47:33.235708 forecastout-0.0.3/forecastout/disaggregation_features/__init__.py
+-rw-r--r--   0        0        0     1330 2024-05-17 08:47:33.235708 forecastout-0.0.3/forecastout/disaggregation_features/add_features.py
+-rw-r--r--   0        0        0     3092 2024-05-17 08:47:33.235708 forecastout-0.0.3/forecastout/disaggregation_features/feature_creator.py
+-rw-r--r--   0        0        0      641 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/disaggregation_features/feature_encoding.py
+-rw-r--r--   0        0        0      594 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/disaggregation_features/feature_normalizer.py
+-rw-r--r--   0        0        0        0 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/disaggregation_models/__init__.py
+-rw-r--r--   0        0        0      567 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/disaggregation_models/abstract_model.py
+-rw-r--r--   0        0        0     2413 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/disaggregation_models/random_forest_model.py
+-rw-r--r--   0        0        0      433 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/forecast_engine/__init__.py
+-rw-r--r--   0        0        0     2836 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/forecast_engine/anomaly_detector.py
+-rw-r--r--   0        0        0     2447 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/forecast_engine/anomaly_fixer.py
+-rw-r--r--   0        0        0     2794 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/forecast_engine/backtester.py
+-rw-r--r--   0        0        0      776 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/forecast_engine/decompose_time_series.py
+-rw-r--r--   0        0        0      778 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/forecast_engine/ensemble_models.py
+-rw-r--r--   0        0        0     2207 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/forecast_engine/ensembler.py
+-rw-r--r--   0        0        0     1390 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/forecast_engine/forecast_model_factory.py
+-rw-r--r--   0        0        0      906 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/forecast_engine/model_predictor.py
+-rw-r--r--   0        0        0     1155 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/forecast_engine/model_trainer.py
+-rw-r--r--   0        0        0        0 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/forecast_models/__init__.py
+-rw-r--r--   0        0        0      442 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/forecast_models/abstract_model.py
+-rw-r--r--   0        0        0     1497 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/forecast_models/autoarima_model.py
+-rw-r--r--   0        0        0     3741 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/forecast_models/holtwinters_model.py
+-rw-r--r--   0        0        0     2294 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/forecast_models/naive_seasonal.py
+-rw-r--r--   0        0        0     1721 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/forecast_models/prophet_model.py
+-rw-r--r--   0        0        0      114 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/utils/__init__.py
+-rw-r--r--   0        0        0     5520 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/utils/input_checker.py
+-rw-r--r--   0        0        0      850 2024-05-17 08:47:33.239708 forecastout-0.0.3/forecastout/utils/update_config.py
+-rw-r--r--   0        0        0      992 2024-05-17 08:47:42.047729 forecastout-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 forecastout-0.0.3/PKG-INFO
```

### Comparing `forecastout-0.0.2/LICENSE` & `forecastout-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/README.md` & `forecastout-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/config.yaml` & `forecastout-0.0.3/forecastout/config.yaml`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/core.py` & `forecastout-0.0.3/forecastout/core.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/data_engine/data_handler.py` & `forecastout-0.0.3/forecastout/data_engine/data_handler.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/data_engine/train_test_split.py` & `forecastout-0.0.3/forecastout/data_engine/train_test_split.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/disaggregation_engine/__init__.py` & `forecastout-0.0.3/forecastout/disaggregation_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/disaggregation_engine/disaggregate_monthly_to_daily_forecast.py` & `forecastout-0.0.3/forecastout/disaggregation_engine/disaggregate_monthly_to_daily_forecast.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/disaggregation_engine/disaggregation_model_factory.py` & `forecastout-0.0.3/forecastout/disaggregation_engine/disaggregation_model_factory.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/disaggregation_engine/disaggregation_model_predictor.py` & `forecastout-0.0.3/forecastout/disaggregation_engine/disaggregation_model_predictor.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/disaggregation_engine/disaggregation_model_trainer.py` & `forecastout-0.0.3/forecastout/disaggregation_engine/disaggregation_model_trainer.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/disaggregation_engine/get_daily_shares.py` & `forecastout-0.0.3/forecastout/disaggregation_engine/get_daily_shares.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/disaggregation_engine/remake_monthly_forecast_current_month.py` & `forecastout-0.0.3/forecastout/disaggregation_engine/remake_monthly_forecast_current_month.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/disaggregation_features/add_features.py` & `forecastout-0.0.3/forecastout/disaggregation_features/add_features.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/disaggregation_features/feature_creator.py` & `forecastout-0.0.3/forecastout/disaggregation_features/feature_creator.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/disaggregation_features/feature_encoding.py` & `forecastout-0.0.3/forecastout/disaggregation_features/feature_encoding.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/disaggregation_features/feature_normalizer.py` & `forecastout-0.0.3/forecastout/disaggregation_features/feature_normalizer.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/disaggregation_models/abstract_model.py` & `forecastout-0.0.3/forecastout/disaggregation_models/abstract_model.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/disaggregation_models/random_forest_model.py` & `forecastout-0.0.3/forecastout/disaggregation_models/random_forest_model.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/forecast_engine/anomaly_detector.py` & `forecastout-0.0.3/forecastout/forecast_engine/anomaly_detector.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/forecast_engine/anomaly_fixer.py` & `forecastout-0.0.3/forecastout/forecast_engine/anomaly_fixer.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/forecast_engine/backtester.py` & `forecastout-0.0.3/forecastout/forecast_engine/backtester.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/forecast_engine/decompose_time_series.py` & `forecastout-0.0.3/forecastout/forecast_engine/decompose_time_series.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/forecast_engine/ensemble_models.py` & `forecastout-0.0.3/forecastout/forecast_engine/ensemble_models.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/forecast_engine/ensembler.py` & `forecastout-0.0.3/forecastout/forecast_engine/ensembler.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/forecast_engine/forecast_model_factory.py` & `forecastout-0.0.3/forecastout/forecast_engine/forecast_model_factory.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/forecast_engine/model_predictor.py` & `forecastout-0.0.3/forecastout/forecast_engine/model_predictor.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/forecast_engine/model_trainer.py` & `forecastout-0.0.3/forecastout/forecast_engine/model_trainer.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/forecast_models/autoarima_model.py` & `forecastout-0.0.3/forecastout/forecast_models/autoarima_model.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/forecast_models/holtwinters_model.py` & `forecastout-0.0.3/forecastout/forecast_models/holtwinters_model.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/forecast_models/naive_seasonal.py` & `forecastout-0.0.3/forecastout/forecast_models/naive_seasonal.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/forecast_models/prophet_model.py` & `forecastout-0.0.3/forecastout/forecast_models/prophet_model.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/utils/input_checker.py` & `forecastout-0.0.3/forecastout/utils/input_checker.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/forecastout/utils/update_config.py` & `forecastout-0.0.3/forecastout/utils/update_config.py`

 * *Files identical despite different names*

### Comparing `forecastout-0.0.2/pyproject.toml` & `forecastout-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forecastout"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["alexis-vazquez <alexis.vazquez@adevinta.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.2.1"
@@ -43,9 +43,10 @@
     "feat",
     "fix",
     "perf",
     "style",
     "refactor",
     "test"
 ]
+
 minor_tags = ["feat"]
 patch_tags = ["fix", "perf"]
```

### Comparing `forecastout-0.0.2/PKG-INFO` & `forecastout-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastout
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: alexis-vazquez
 Author-email: alexis.vazquez@adevinta.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

