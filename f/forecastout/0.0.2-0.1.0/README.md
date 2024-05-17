# Comparing `tmp/forecastout-0.0.2.tar.gz` & `tmp/forecastout-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecastout-0.0.2.tar", max compression
+gzip compressed data, was "forecastout-0.1.0.tar", max compression
```

## Comparing `forecastout-0.0.2.tar` & `forecastout-0.1.0.tar`

### file list

```diff
@@ -1,44 +1,5 @@
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
+-rw-r--r--   0        0        0       13 2024-03-12 15:06:56.954081 forecastout-0.1.0/README.md
+-rw-r--r--   0        0        0      336 2024-03-12 14:38:44.842875 forecastout-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-12 15:09:40.924641 forecastout-0.1.0/src/forecastout/__init__.py
+-rw-r--r--   0        0        0       86 2024-03-12 14:32:00.299108 forecastout-0.1.0/src/forecastout/function_test.py
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 forecastout-0.1.0/PKG-INFO
```

