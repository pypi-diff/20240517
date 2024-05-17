# Comparing `tmp/flasc-1.4.2.tar.gz` & `tmp/flasc-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flasc-1.4.2.tar", last modified: Fri May 17 14:16:47 2024, max compression
+gzip compressed data, was "flasc-2.0.tar", last modified: Mon May  6 16:05:23 2024, max compression
```

## Comparing `flasc-1.4.2.tar` & `flasc-2.0.tar`

### file list

```diff
@@ -1,61 +1,55 @@
-drwxr-xr-x   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)        0 2024-05-17 14:16:47.972771 flasc-1.4.2/
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)      286 2023-10-27 16:00:00.000000 flasc-1.4.2/AUTHORS.rst
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)    11356 2024-05-17 14:14:00.000000 flasc-1.4.2/LICENSE.txt
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)      620 2024-05-17 14:14:00.000000 flasc-1.4.2/NOTICE.txt
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     1148 2024-05-17 14:16:47.972424 flasc-1.4.2/PKG-INFO
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     6660 2024-05-17 14:14:00.000000 flasc-1.4.2/README.rst
-drwxr-xr-x   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)        0 2024-05-17 14:16:47.964326 flasc-1.4.2/flasc/
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)      552 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/__init__.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     4419 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/circular_statistics.py
-drwxr-xr-x   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)        0 2024-05-17 14:16:47.966581 flasc-1.4.2/flasc/dataframe_operations/
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)      334 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/dataframe_operations/__init__.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     5914 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/dataframe_operations/dataframe_filtering.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)    37739 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/dataframe_operations/dataframe_manipulations.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     1641 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/dataframe_operations/df_reader_writer.py
-drwxr-xr-x   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)        0 2024-05-17 14:16:47.968041 flasc-1.4.2/flasc/energy_ratio/
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)      318 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/energy_ratio/__init__.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)    22354 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/energy_ratio/energy_ratio.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     4240 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/energy_ratio/energy_ratio_input.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)    22036 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/energy_ratio/energy_ratio_output.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)    23111 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/energy_ratio/energy_ratio_utilities.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)    23869 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/energy_ratio/energy_ratio_wd_bias_estimation.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)    22094 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/energy_ratio/total_uplift.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)    41476 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/floris_tools.py
-drwxr-xr-x   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)        0 2024-05-17 14:16:47.968593 flasc-1.4.2/flasc/model_estimation/
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)      317 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/model_estimation/__init__.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)    12246 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/model_estimation/floris_sensitivity_analysis.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     7926 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/model_estimation/turbulence_estimator.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)    10052 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/optimization.py
-drwxr-xr-x   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)        0 2024-05-17 14:16:47.969542 flasc-1.4.2/flasc/raw_data_handling/
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)      311 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/raw_data_handling/__init__.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     4359 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/raw_data_handling/raw_data_importing.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)    26102 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/raw_data_handling/sqldatabase_management.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)    14584 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/time_operations.py
-drwxr-xr-x   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)        0 2024-05-17 14:16:47.969943 flasc-1.4.2/flasc/timing_tests/
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)        0 2023-08-22 14:58:45.000000 flasc-1.4.2/flasc/timing_tests/__init__.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     3669 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/timing_tests/energy_ratio_timing.py
-drwxr-xr-x   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)        0 2024-05-17 14:16:47.971036 flasc-1.4.2/flasc/turbine_analysis/
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)      358 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/turbine_analysis/__init__.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     4897 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/turbine_analysis/find_sensor_faults.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     5757 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/turbine_analysis/northing_offset.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)    48914 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/turbine_analysis/ws_pow_filtering.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     7831 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/turbine_analysis/yaw_pow_fitting.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     6874 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/utilities.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     4974 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/utilities_examples.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)        5 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/version.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)    28276 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/visualization.py
-drwxr-xr-x   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)        0 2024-05-17 14:16:47.971745 flasc-1.4.2/flasc/wake_steering/
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)      316 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/wake_steering/__init__.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     5585 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/wake_steering/lookup_table_tools.py
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     9848 2024-05-17 14:14:00.000000 flasc-1.4.2/flasc/wake_steering/yaw_optimizer_visualization.py
-drwxr-xr-x   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)        0 2024-05-17 14:16:47.965722 flasc-1.4.2/flasc.egg-info/
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     1148 2024-05-17 14:16:47.000000 flasc-1.4.2/flasc.egg-info/PKG-INFO
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     1622 2024-05-17 14:16:47.000000 flasc-1.4.2/flasc.egg-info/SOURCES.txt
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)        1 2024-05-17 14:16:47.000000 flasc-1.4.2/flasc.egg-info/dependency_links.txt
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)       41 2024-05-17 14:16:47.000000 flasc-1.4.2/flasc.egg-info/entry_points.txt
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)        1 2022-09-02 22:07:12.000000 flasc-1.4.2/flasc.egg-info/not-zip-safe
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)      171 2024-05-17 14:16:47.000000 flasc-1.4.2/flasc.egg-info/requires.txt
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)        6 2024-05-17 14:16:47.000000 flasc-1.4.2/flasc.egg-info/top_level.txt
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     3547 2024-05-17 14:14:00.000000 flasc-1.4.2/pyproject.toml
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)       38 2024-05-17 14:16:47.972833 flasc-1.4.2/setup.cfg
--rw-r--r--   0 pfleming (2094687460) NREL_NT\Domain Users (18434217)     1962 2024-05-17 14:16:19.000000 flasc-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:05:23.939684 flasc-2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-06 16:05:16.000000 flasc-2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-06 16:05:23.939684 flasc-2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-06 16:05:16.000000 flasc-2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:05:23.931684 flasc-2.0/flasc/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-06 16:05:16.000000 flasc-2.0/flasc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:05:23.935684 flasc-2.0/flasc/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-06 16:05:16.000000 flasc-2.0/flasc/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21268 2024-05-06 16:05:16.000000 flasc-2.0/flasc/analysis/energy_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-06 16:05:16.000000 flasc-2.0/flasc/analysis/energy_ratio_heterogeneity_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-05-06 16:05:16.000000 flasc-2.0/flasc/analysis/energy_ratio_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23068 2024-05-06 16:05:16.000000 flasc-2.0/flasc/analysis/energy_ratio_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21504 2024-05-06 16:05:16.000000 flasc-2.0/flasc/analysis/total_uplift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:05:23.935684 flasc-2.0/flasc/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-06 16:05:16.000000 flasc-2.0/flasc/data_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41675 2024-05-06 16:05:16.000000 flasc-2.0/flasc/data_processing/dataframe_manipulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23162 2024-05-06 16:05:16.000000 flasc-2.0/flasc/data_processing/energy_ratio_wd_bias_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53611 2024-05-06 16:05:16.000000 flasc-2.0/flasc/data_processing/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-06 16:05:16.000000 flasc-2.0/flasc/data_processing/find_sensor_faults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-06 16:05:16.000000 flasc-2.0/flasc/data_processing/northing_offset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13157 2024-05-06 16:05:16.000000 flasc-2.0/flasc/data_processing/time_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-06 16:05:16.000000 flasc-2.0/flasc/logging_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:05:23.935684 flasc-2.0/flasc/model_fitting/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-06 16:05:16.000000 flasc-2.0/flasc/model_fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11555 2024-05-06 16:05:16.000000 flasc-2.0/flasc/model_fitting/floris_sensitivity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-05-06 16:05:16.000000 flasc-2.0/flasc/model_fitting/floris_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-05-06 16:05:16.000000 flasc-2.0/flasc/model_fitting/turbulence_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-06 16:05:16.000000 flasc-2.0/flasc/model_fitting/yaw_pow_fitting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:05:23.935684 flasc-2.0/flasc/timing_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:05:16.000000 flasc-2.0/flasc/timing_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-06 16:05:16.000000 flasc-2.0/flasc/timing_tests/energy_ratio_timing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:05:23.939684 flasc-2.0/flasc/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-06 16:05:16.000000 flasc-2.0/flasc/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-06 16:05:16.000000 flasc-2.0/flasc/utilities/circular_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22914 2024-05-06 16:05:16.000000 flasc-2.0/flasc/utilities/energy_ratio_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44323 2024-05-06 16:05:16.000000 flasc-2.0/flasc/utilities/floris_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-06 16:05:16.000000 flasc-2.0/flasc/utilities/lookup_table_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9407 2024-05-06 16:05:16.000000 flasc-2.0/flasc/utilities/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-06 16:05:16.000000 flasc-2.0/flasc/utilities/tuner_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-06 16:05:16.000000 flasc-2.0/flasc/utilities/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-06 16:05:16.000000 flasc-2.0/flasc/utilities/utilities_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-06 16:05:16.000000 flasc-2.0/flasc/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-05-06 16:05:16.000000 flasc-2.0/flasc/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-05-06 16:05:16.000000 flasc-2.0/flasc/yaw_optimizer_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:05:23.939684 flasc-2.0/flasc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-06 16:05:23.000000 flasc-2.0/flasc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-06 16:05:23.000000 flasc-2.0/flasc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:05:23.000000 flasc-2.0/flasc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-06 16:05:23.000000 flasc-2.0/flasc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:05:23.000000 flasc-2.0/flasc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-06 16:05:23.000000 flasc-2.0/flasc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 16:05:23.000000 flasc-2.0/flasc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-06 16:05:16.000000 flasc-2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:05:23.939684 flasc-2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-06 16:05:16.000000 flasc-2.0/setup.py
```

### Comparing `flasc-1.4.2/flasc/dataframe_operations/dataframe_manipulations.py` & `flasc-2.0/flasc/data_processing/dataframe_manipulations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,29 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-
 # import datetime
 import datetime
-import numpy as np
 import os as os
-import pandas as pd
 import warnings
+from xmlrpc.client import Boolean
 
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
 from floris.utilities import wrap_360
 
-from ..dataframe_operations import df_reader_writer as fsio
-from .. import (
-    time_operations as fsato,
-    floris_tools as ftools,
-    utilities as fsut
-)
+from flasc.logging_manager import LoggingManager
+from flasc.utilities import floris_tools as ftools, utilities as fsut
+
+logger_manager = LoggingManager()  # Instantiate LoggingManager
+logger = logger_manager.logger  # Obtain the reusable logger
 
 
 # Functions related to wind farm analysis for df
 def filter_df_by_ws(df, ws_range):
-    df = df[df['ws'] >= ws_range[0]]
-    df = df[df['ws'] < ws_range[1]]
+    df = df[df["ws"] >= ws_range[0]]
+    df = df[df["ws"] < ws_range[1]]
     return df
 
 
 def filter_df_by_wd(df, wd_range):
     lb = wd_range[0]
     ub = wd_range[1]
 
@@ -43,166 +31,196 @@
     if ub > 360.0:
         ub = wrap_360(ub)
 
     wd_array = wrap_360(df["wd"])
     if lb > ub:
         df = df[((wd_array >= lb) | (wd_array < ub))]
     else:
-        df = df[((wd_array >= lb) & (df['wd'] < ub))]
+        df = df[((wd_array >= lb) & (df["wd"] < ub))]
     return df
 
 
 def filter_df_by_ti(df, ti_range):
-    df = df[df['ti'] >= ti_range[0]]
-    df = df[df['ti'] < ti_range[1]]
+    df = df[df["ti"] >= ti_range[0]]
+    df = df[df["ti"] < ti_range[1]]
     return df
 
 
 def get_num_turbines(df):
     return fsut.get_num_turbines(df)
 
 
 # Generic functions for column operations
-def get_column_mean(df, col_prefix='pow', turbine_list=None,
-                    circular_mean=False):
+def get_column_mean(df, col_prefix="pow", turbine_list=None, circular_mean=False):
     if turbine_list is None:
         turbine_list = range(get_num_turbines(df))  # Assume all turbines
     elif isinstance(turbine_list, (int, np.integer)):
         turbine_list = [turbine_list]
 
-    col_names = [col_prefix + '_%03d' % ti for ti in turbine_list]
+    col_names = [col_prefix + "_%03d" % ti for ti in turbine_list]
     array = df[col_names].astype(float)
 
     if circular_mean:
         # Use unit vectors to calculate the mean
         warnings.simplefilter("ignore", category=RuntimeWarning)
-        dir_x = np.nanmean(np.cos(array * np.pi / 180.), axis=1)
-        dir_y = np.nanmean(np.sin(array * np.pi / 180.), axis=1)
+        dir_x = np.nanmean(np.cos(array * np.pi / 180.0), axis=1)
+        dir_y = np.nanmean(np.sin(array * np.pi / 180.0), axis=1)
 
         mean_dirs = np.arctan2(dir_y, dir_x)
-        mean_out = wrap_360(mean_dirs * 180. / np.pi)
+        mean_out = wrap_360(mean_dirs * 180.0 / np.pi)
     else:
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", category=RuntimeWarning)
             mean_out = np.nanmean(array, axis=1)
 
     return mean_out
 
 
-def _set_col_by_turbines(col_out, col_prefix, df,
-                         turbine_numbers, circular_mean):
+def _set_col_by_turbines(col_out, col_prefix, df, turbine_numbers, circular_mean):
     if isinstance(turbine_numbers, str):
-        if turbine_numbers.lower() == 'all':
+        if turbine_numbers.lower() == "all":
             turbine_numbers = range(get_num_turbines(df=df))
 
     df[col_out] = get_column_mean(
-        df=df,
-        col_prefix=col_prefix,
-        turbine_list=turbine_numbers,
-        circular_mean=circular_mean
-        )
+        df=df, col_prefix=col_prefix, turbine_list=turbine_numbers, circular_mean=circular_mean
+    )
     return df
 
 
-def _set_col_by_n_closest_upstream_turbines(col_out, col_prefix, df, N,
-    df_upstream, circular_mean, turb_no, x_turbs, y_turbs, exclude_turbs=[]):
+def _set_col_by_n_closest_upstream_turbines(
+    col_out,
+    col_prefix,
+    df,
+    N,
+    df_upstream,
+    circular_mean,
+    turb_no,
+    x_turbs,
+    y_turbs,
+    exclude_turbs=[],
+):
     # Can get df_upstream using floris_tools.get_upstream_turbs_floris()
     df.loc[df.index, col_out] = np.nan
     for i in range(df_upstream.shape[0]):
-        wd_min = df_upstream.loc[i, 'wd_min']
-        wd_max = df_upstream.loc[i, 'wd_max']
-        upstr_turbs = df_upstream.loc[i, 'turbines']
+        wd_min = df_upstream.loc[i, "wd_min"]
+        wd_max = df_upstream.loc[i, "wd_max"]
+        upstr_turbs = df_upstream.loc[i, "turbines"]
 
         # Calculate distances and get closest N upstream turbines
         upstr_turbs = [ti for ti in upstr_turbs if ti not in exclude_turbs]
         x0 = x_turbs[turb_no]
         y0 = y_turbs[turb_no]
         x_upstr = np.array(x_turbs, dtype=float)[upstr_turbs]
         y_upstr = np.array(y_turbs, dtype=float)[upstr_turbs]
         ds = np.sqrt((x_upstr - x0) ** 2.0 + (y_upstr - y0) ** 2.0)
         upstr_turbs_sorted = np.array(upstr_turbs, dtype=int)[np.argsort(ds)]
         upstr_turbs_n_closest = upstr_turbs_sorted[0:N]
 
         if wd_min > wd_max:  # Wrap around
-            ids = (df['wd'] > wd_min) | (df['wd'] <= wd_max)
+            ids = (df["wd"] > wd_min) | (df["wd"] <= wd_max)
         else:
-            ids = (df['wd'] >= wd_min) & (df['wd'] < wd_max)
+            ids = (df["wd"] >= wd_min) & (df["wd"] < wd_max)
 
         col_mean = get_column_mean(
             df.loc[ids, :],
             col_prefix=col_prefix,
             turbine_list=upstr_turbs_n_closest,
-            circular_mean=circular_mean
+            circular_mean=circular_mean,
         )
         df.loc[ids, col_out] = col_mean
 
     return df
 
 
-def _set_col_by_upstream_turbines(col_out, col_prefix, df,
-                                  df_upstream, circular_mean,
-                                  exclude_turbs=[]):
+def _set_col_by_upstream_turbines(
+    col_out, col_prefix, df, df_upstream, circular_mean, exclude_turbs=[]
+):
     # Can get df_upstream using floris_tools.get_upstream_turbs_floris()
     df.loc[df.index, col_out] = np.nan
     for i in range(df_upstream.shape[0]):
-        wd_min = df_upstream.loc[i, 'wd_min']
-        wd_max = df_upstream.loc[i, 'wd_max']
-        upstr_turbs = df_upstream.loc[i, 'turbines']
+        wd_min = df_upstream.loc[i, "wd_min"]
+        wd_max = df_upstream.loc[i, "wd_max"]
+        upstr_turbs = df_upstream.loc[i, "turbines"]
 
         # Exclude particular turbines
         upstr_turbs = [ti for ti in upstr_turbs if ti not in exclude_turbs]
 
         if wd_min > wd_max:  # Wrap around
-            ids = (df['wd'] > wd_min) | (df['wd'] <= wd_max)
+            ids = (df["wd"] > wd_min) | (df["wd"] <= wd_max)
         else:
-            ids = (df['wd'] >= wd_min) & (df['wd'] < wd_max)
+            ids = (df["wd"] >= wd_min) & (df["wd"] < wd_max)
 
-        col_mean = get_column_mean(df.loc[ids, :],
-                                   col_prefix=col_prefix,
-                                   turbine_list=upstr_turbs,
-                                   circular_mean=circular_mean)
+        col_mean = get_column_mean(
+            df.loc[ids, :],
+            col_prefix=col_prefix,
+            turbine_list=upstr_turbs,
+            circular_mean=circular_mean,
+        )
         df.loc[ids, col_out] = col_mean
 
     return df
 
 
-def _set_col_by_radius_from_turbine(col_out, col_prefix, df, turb_no,
-                                    x_turbs, y_turbs, max_radius,
-                                    circular_mean, include_itself=True):
-
+def _set_col_by_radius_from_turbine(
+    col_out,
+    col_prefix,
+    df,
+    turb_no,
+    x_turbs,
+    y_turbs,
+    max_radius,
+    circular_mean,
+    include_itself=True,
+):
     turbs_within_radius = ftools.get_turbs_in_radius(
-        x_turbs=x_turbs, y_turbs=y_turbs, turb_no=turb_no,
-        max_radius=max_radius, include_itself=include_itself)
+        x_turbs=x_turbs,
+        y_turbs=y_turbs,
+        turb_no=turb_no,
+        max_radius=max_radius,
+        include_itself=include_itself,
+    )
 
     if len(turbs_within_radius) < 1:
-        print('No turbines within proximity. Try to increase radius.')
+        logger.warn("No turbines within proximity. Try to increase radius.")
         return None
 
-    return _set_col_by_turbines(col_out=col_out, col_prefix=col_prefix, df=df,
-                                turbine_numbers=turbs_within_radius,
-                                circular_mean=circular_mean)
+    return _set_col_by_turbines(
+        col_out=col_out,
+        col_prefix=col_prefix,
+        df=df,
+        turbine_numbers=turbs_within_radius,
+        circular_mean=circular_mean,
+    )
 
 
 def _set_col_by_upstream_turbines_in_radius(
-    col_out, col_prefix, df, df_upstream, turb_no,
-    x_turbs, y_turbs, max_radius, circular_mean,
-    include_itself=True):
+    col_out,
+    col_prefix,
+    df,
+    df_upstream,
+    turb_no,
+    x_turbs,
+    y_turbs,
+    max_radius,
+    circular_mean,
+    include_itself=True,
+):
     """Add a column called [col_out] to your dataframe, which is the
     mean of the columns pow_%03d for turbines that are upstream and
     also within radius [max_radius] of the turbine of interest
     [turb_no].
 
     Args:
         df ([pd.DataFrame]): Dataframe with measurements. This dataframe
         typically consists of wd_%03d, ws_%03d, ti_%03d, pow_%03d, and
         potentially additional measurements.
         df_upstream ([pd.DataFrame]): Dataframe containing rows indicating
-        wind direction ranges and the corresponding upstream turbines for 
+        wind direction ranges and the corresponding upstream turbines for
         that wind direction range. This variable can be generated with
-        flasc.floris_tools.get_upstream_turbs_floris(...).
+        flasc.utilities.floris_tools.get_upstream_turbs_floris(...).
         turb_no ([int]): Turbine number from which the radius should be
         calculated.
         x_turbs ([list, array]): Array containing x locations of turbines.
         y_turbs ([list, array]): Array containing y locations of turbines.
         max_radius ([float]): Maximum radius for the upstream turbines
         until which they are still considered as relevant/used for the
         calculation of the averaged column quantity.
@@ -212,30 +230,35 @@
 
     Returns:
         df ([pd.DataFrame]): Dataframe which equals the inserted dataframe
         plus the additional column called [col_ref].
     """
 
     turbs_in_radius = ftools.get_turbs_in_radius(
-        x_turbs=x_turbs, y_turbs=y_turbs, turb_no=turb_no,
-        max_radius=max_radius, include_itself=include_itself)
+        x_turbs=x_turbs,
+        y_turbs=y_turbs,
+        turb_no=turb_no,
+        max_radius=max_radius,
+        include_itself=include_itself,
+    )
 
     if len(turbs_in_radius) < 1:
-        print('No turbines within proximity. Try to increase radius.')
+        logger.info("No turbines within proximity. Try to increase radius.")
         return None
 
     turbs = range(len(x_turbs))
     turbs_outside_radius = [i for i in turbs if i not in turbs_in_radius]
     return _set_col_by_upstream_turbines(
         col_out=col_out,
         col_prefix=col_prefix,
         df=df,
         df_upstream=df_upstream,
         circular_mean=circular_mean,
-        exclude_turbs=turbs_outside_radius)
+        exclude_turbs=turbs_outside_radius,
+    )
 
 
 # Helper functions
 def set_wd_by_turbines(df, turbine_numbers):
     """Add a column called 'wd' in your dataframe with value equal
     to the circular-averaged wind direction measurements of all
     the turbines in turbine_numbers.
@@ -247,15 +270,15 @@
         turbine_numbers ([list, array]): List of turbine numbers that
         should be used to calculate the column average.
 
     Returns:
         df ([pd.DataFrame]): Dataframe which equals the inserted dataframe
         plus the additional column called 'wd'.
     """
-    return _set_col_by_turbines('wd', 'wd', df, turbine_numbers, True)
+    return _set_col_by_turbines("wd", "wd", df, turbine_numbers, True)
 
 
 def set_wd_by_all_turbines(df):
     """Add a column called 'wd' in your dataframe with value equal
     to the circular-averaged wind direction measurements of all
     turbines.
 
@@ -264,29 +287,29 @@
         typically consists of wd_%03d, ws_%03d, ti_%03d, pow_%03d, and
         potentially additional measurements.
 
     Returns:
         df ([pd.DataFrame]): Dataframe which equals the inserted dataframe
         plus the additional column called 'wd'.
     """
-    return _set_col_by_turbines('wd', 'wd', df, 'all', True)
+    return _set_col_by_turbines("wd", "wd", df, "all", True)
 
 
-def set_wd_by_radius_from_turbine(df, turb_no, x_turbs, y_turbs,
-                                  max_radius, include_itself=True):
+def set_wd_by_radius_from_turbine(df, turb_no, x_turbs, y_turbs, max_radius, include_itself=True):
     return _set_col_by_radius_from_turbine(
-        col_out='wd',
-        col_prefix='wd',
+        col_out="wd",
+        col_prefix="wd",
         df=df,
         turb_no=turb_no,
         x_turbs=x_turbs,
         y_turbs=y_turbs,
         max_radius=max_radius,
         circular_mean=True,
-        include_itself=include_itself)
+        include_itself=include_itself,
+    )
 
 
 def set_ws_by_turbines(df, turbine_numbers):
     """Add a column called 'ws' in your dataframe with value equal
     to the circular-averaged wind direction measurements of all
     the turbines in turbine_numbers.
 
@@ -297,15 +320,15 @@
         turbine_numbers ([list, array]): List of turbine numbers that
         should be used to calculate the column average.
 
     Returns:
         df ([pd.DataFrame]): Dataframe which equals the inserted dataframe
         plus the additional column called 'ws'.
     """
-    return _set_col_by_turbines('ws', 'ws', df, turbine_numbers, False)
+    return _set_col_by_turbines("ws", "ws", df, turbine_numbers, False)
 
 
 def set_ws_by_all_turbines(df):
     """Add a column called 'ws' in your dataframe with value equal
     to the circular-averaged wind direction measurements of all
     turbines.
 
@@ -316,63 +339,63 @@
         turbine_numbers ([list, array]): List of turbine numbers that
         should be used to calculate the column average.
 
     Returns:
         df ([pd.DataFrame]): Dataframe which equals the inserted dataframe
         plus the additional column called 'ws'.
     """
-    return _set_col_by_turbines('ws', 'ws', df, 'all', False)
+    return _set_col_by_turbines("ws", "ws", df, "all", False)
 
 
 def set_ws_by_upstream_turbines(df, df_upstream, exclude_turbs=[]):
     """Add a column called 'ws' in your dataframe with value equal
     to the averaged wind speed measurements of all the turbines
     upstream, excluding the turbines listed in exclude_turbs.
 
     Args:
         df ([pd.DataFrame]): Dataframe with measurements. This dataframe
         typically consists of wd_%03d, ws_%03d, ti_%03d, pow_%03d, and
         potentially additional measurements.
         df_upstream ([pd.DataFrame]): Dataframe containing rows indicating
         wind direction ranges and the corresponding upstream turbines for
         that wind direction range. This variable can be generated with
-        flasc.floris_tools.get_upstream_turbs_floris(...).
+        flasc.utilities.floris_tools.get_upstream_turbs_floris(...).
         exclude_turbs ([list, array]): array-like variable containing
         turbine indices that should be excluded in determining the column
         mean quantity.
     Returns:
         df ([pd.DataFrame]): Dataframe which equals the inserted dataframe
         plus the additional column called 'ws'.
     """
     return _set_col_by_upstream_turbines(
-        col_out='ws',
-        col_prefix='ws',
+        col_out="ws",
+        col_prefix="ws",
         df=df,
         df_upstream=df_upstream,
         circular_mean=False,
-        exclude_turbs=exclude_turbs)
+        exclude_turbs=exclude_turbs,
+    )
 
 
-def set_ws_by_upstream_turbines_in_radius(df, df_upstream, turb_no,
-                                          x_turbs, y_turbs,
-                                          max_radius,
-                                          include_itself=True):
+def set_ws_by_upstream_turbines_in_radius(
+    df, df_upstream, turb_no, x_turbs, y_turbs, max_radius, include_itself=True
+):
     """Add a column called 'ws' to your dataframe, which is the
     mean of the columns pow_%03d for turbines that are upstream and
     also within radius [max_radius] of the turbine of interest
     [turb_no].
 
     Args:
         df ([pd.DataFrame]): Dataframe with measurements. This dataframe
         typically consists of wd_%03d, ws_%03d, ti_%03d, pow_%03d, and
         potentially additional measurements.
         df_upstream ([pd.DataFrame]): Dataframe containing rows indicating
         wind direction ranges and the corresponding upstream turbines for
         that wind direction range. This variable can be generated with
-        flasc.floris_tools.get_upstream_turbs_floris(...).
+        flasc.utilities.floris_tools.get_upstream_turbs_floris(...).
         turb_no ([int]): Turbine number from which the radius should be
         calculated.
         x_turbs ([list, array]): Array containing x locations of turbines.
         y_turbs ([list, array]): Array containing y locations of turbines.
         max_radius ([float]): Maximum radius for the upstream turbines
         until which they are still considered as relevant/used for the
         calculation of the averaged column quantity.
@@ -381,40 +404,42 @@
         to False.
 
     Returns:
         df ([pd.DataFrame]): Dataframe which equals the inserted dataframe
         plus the additional column called 'ws'.
     """
     return _set_col_by_upstream_turbines_in_radius(
-        col_out='ws',
-        col_prefix='ws',
+        col_out="ws",
+        col_prefix="ws",
         df=df,
         df_upstream=df_upstream,
         turb_no=turb_no,
         x_turbs=x_turbs,
         y_turbs=y_turbs,
         max_radius=max_radius,
         circular_mean=False,
-        include_itself=include_itself)
+        include_itself=include_itself,
+    )
 
 
-def set_ws_by_n_closest_upstream_turbines(df, df_upstream, turb_no,
-    x_turbs, y_turbs, exclude_turbs=[], N=5):
+def set_ws_by_n_closest_upstream_turbines(
+    df, df_upstream, turb_no, x_turbs, y_turbs, exclude_turbs=[], N=5
+):
     """Add a column called 'pow_ref' to your dataframe, which is the
     mean of the columns pow_%03d for the 5 closest turbines that are
     upstream of the turbine of interest [turb_no].
 
     Args:
         df ([pd.DataFrame]): Dataframe with measurements. This dataframe
         typically consists of wd_%03d, ws_%03d, ti_%03d, pow_%03d, and
         potentially additional measurements.
         df_upstream ([pd.DataFrame]): Dataframe containing rows indicating
-        wind direction ranges and the corresponding upstream turbines for 
+        wind direction ranges and the corresponding upstream turbines for
         that wind direction range. This variable can be generated with
-        flasc.floris_tools.get_upstream_turbs_floris(...).
+        flasc.utilities.floris_tools.get_upstream_turbs_floris(...).
         turb_no ([int]): Turbine number from which the radius should be
         calculated.
         x_turbs ([list, array]): Array containing x locations of turbines.
         y_turbs ([list, array]): Array containing y locations of turbines.
         max_radius ([float]): Maximum radius for the upstream turbines
         until which they are still considered as relevant/used for the
         calculation of the averaged column quantity.
@@ -423,24 +448,25 @@
         to False.
 
      Returns:
         df ([pd.DataFrame]): Dataframe which equals the inserted dataframe
         plus the additional column called 'pow_ref'.
     """
     return _set_col_by_n_closest_upstream_turbines(
-        col_out='ws',
-        col_prefix='ws',
+        col_out="ws",
+        col_prefix="ws",
         N=N,
         df=df,
         df_upstream=df_upstream,
         turb_no=turb_no,
         x_turbs=x_turbs,
         y_turbs=y_turbs,
         exclude_turbs=exclude_turbs,
-        circular_mean=False)
+        circular_mean=False,
+    )
 
 
 def set_ti_by_turbines(df, turbine_numbers):
     """Add a column called 'ti' in your dataframe with value equal
     to the averaged turbulence intensity measurements of all the
     turbines listed in turbine_numbers.
 
@@ -451,15 +477,15 @@
         turbine_numbers ([list, array]): List of turbine numbers that
         should be used to calculate the column average.
 
     Returns:
         df ([pd.DataFrame]): Dataframe which equals the inserted dataframe
         plus the additional column called 'ti'.
     """
-    return _set_col_by_turbines('ti', 'ti', df, turbine_numbers, False)
+    return _set_col_by_turbines("ti", "ti", df, turbine_numbers, False)
 
 
 def set_ti_by_all_turbines(df):
     """Add a column called 'ti' in your dataframe with value equal
     to the averaged turbulence intensity measurements of all
     turbines.
 
@@ -470,63 +496,63 @@
         turbine_numbers ([list, array]): List of turbine numbers that
         should be used to calculate the column average.
 
     Returns:
         df ([pd.DataFrame]): Dataframe which equals the inserted dataframe
         plus the additional column called 'ti'.
     """
-    return _set_col_by_turbines('ti', 'ti', df, 'all', False)
+    return _set_col_by_turbines("ti", "ti", df, "all", False)
 
 
 def set_ti_by_upstream_turbines(df, df_upstream, exclude_turbs=[]):
     """Add a column called 'ti' in your dataframe with value equal
     to the averaged turbulence intensity measurements of all the turbines
     upstream, excluding the turbines listed in exclude_turbs.
 
     Args:
         df ([pd.DataFrame]): Dataframe with measurements. This dataframe
         typically consists of wd_%03d, ws_%03d, ti_%03d, pow_%03d, and
         potentially additional measurements.
         df_upstream ([pd.DataFrame]): Dataframe containing rows indicating
         wind direction ranges and the corresponding upstream turbines for
         that wind direction range. This variable can be generated with
-        flasc.floris_tools.get_upstream_turbs_floris(...).
+        flasc.utilities.floris_tools.get_upstream_turbs_floris(...).
         exclude_turbs ([list, array]): array-like variable containing
         turbine indices that should be excluded in determining the column
         mean quantity.
     Returns:
         df ([pd.DataFrame]): Dataframe which equals the inserted dataframe
         plus the additional column called 'ti'.
     """
     return _set_col_by_upstream_turbines(
-        col_out='ti',
-        col_prefix='ti',
+        col_out="ti",
+        col_prefix="ti",
         df=df,
         df_upstream=df_upstream,
         circular_mean=False,
-        exclude_turbs=exclude_turbs)
+        exclude_turbs=exclude_turbs,
+    )
 
 
-def set_ti_by_upstream_turbines_in_radius(df, df_upstream, turb_no,
-                                          x_turbs, y_turbs,
-                                          max_radius,
-                                          include_itself=True):
+def set_ti_by_upstream_turbines_in_radius(
+    df, df_upstream, turb_no, x_turbs, y_turbs, max_radius, include_itself=True
+):
     """Add a column called 'ti' to your dataframe, which is the
     mean of the columns ti_%03d for turbines that are upstream and
     also within radius [max_radius] of the turbine of interest
     [turb_no].
 
     Args:
         df ([pd.DataFrame]): Dataframe with measurements. This dataframe
         typically consists of wd_%03d, ws_%03d, ti_%03d, pow_%03d, and
         potentially additional measurements.
         df_upstream ([pd.DataFrame]): Dataframe containing rows indicating
-        wind direction ranges and the corresponding upstream turbines for 
+        wind direction ranges and the corresponding upstream turbines for
         that wind direction range. This variable can be generated with
-        flasc.floris_tools.get_upstream_turbs_floris(...).
+        flasc.utilities.floris_tools.get_upstream_turbs_floris(...).
         turb_no ([int]): Turbine number from which the radius should be
         calculated.
         x_turbs ([list, array]): Array containing x locations of turbines.
         y_turbs ([list, array]): Array containing y locations of turbines.
         max_radius ([float]): Maximum radius for the upstream turbines
         until which they are still considered as relevant/used for the
         calculation of the averaged column quantity.
@@ -535,24 +561,25 @@
         to False.
 
     Returns:
         df ([pd.DataFrame]): Dataframe which equals the inserted dataframe
         plus the additional column called 'ti'.
     """
     return _set_col_by_upstream_turbines_in_radius(
-        col_out='ti',
-        col_prefix='ti',
+        col_out="ti",
+        col_prefix="ti",
         df=df,
         df_upstream=df_upstream,
         turb_no=turb_no,
         x_turbs=x_turbs,
         y_turbs=y_turbs,
         max_radius=max_radius,
         circular_mean=False,
-        include_itself=include_itself)
+        include_itself=include_itself,
+    )
 
 
 def set_pow_ref_by_turbines(df, turbine_numbers):
     """Add a column called 'pow_ref' in your dataframe with value equal
     to the averaged turbulence intensity measurements of all the
     turbines listed in turbine_numbers.
 
@@ -563,62 +590,63 @@
         turbine_numbers ([list, array]): List of turbine numbers that
         should be used to calculate the column average.
 
     Returns:
         df ([pd.DataFrame]): Dataframe which equals the inserted dataframe
         plus the additional column called 'ti'.
     """
-    return _set_col_by_turbines('pow_ref', 'pow', df, turbine_numbers, False)
+    return _set_col_by_turbines("pow_ref", "pow", df, turbine_numbers, False)
 
 
 def set_pow_ref_by_upstream_turbines(df, df_upstream, exclude_turbs=[]):
     """Add a column called 'pow_ref' in your dataframe with value equal
     to the averaged power measurements of all the turbines upstream,
     excluding the turbines listed in exclude_turbs.
 
     Args:
         df ([pd.DataFrame]): Dataframe with measurements. This dataframe
         typically consists of wd_%03d, ws_%03d, ti_%03d, pow_%03d, and
         potentially additional measurements.
         df_upstream ([pd.DataFrame]): Dataframe containing rows indicating
         wind direction ranges and the corresponding upstream turbines for
         that wind direction range. This variable can be generated with
-        flasc.floris_tools.get_upstream_turbs_floris(...).
+        flasc.utilities.floris_tools.get_upstream_turbs_floris(...).
         exclude_turbs ([list, array]): array-like variable containing
         turbine indices that should be excluded in determining the column
         mean quantity.
     Returns:
         df ([pd.DataFrame]): Dataframe which equals the inserted dataframe
         plus the additional column called 'pow_ref'.
     """
     return _set_col_by_upstream_turbines(
-        col_out='pow_ref',
-        col_prefix='pow',
+        col_out="pow_ref",
+        col_prefix="pow",
         df=df,
         df_upstream=df_upstream,
         circular_mean=False,
-        exclude_turbs=exclude_turbs)
+        exclude_turbs=exclude_turbs,
+    )
 
 
 def set_pow_ref_by_upstream_turbines_in_radius(
-    df, df_upstream, turb_no, x_turbs,
-    y_turbs, max_radius, include_itself=False):
+    df, df_upstream, turb_no, x_turbs, y_turbs, max_radius, include_itself=False
+):
     """Add a column called 'pow_ref' to your dataframe, which is the
     mean of the columns pow_%03d for turbines that are upstream and
     also within radius [max_radius] of the turbine of interest
     [turb_no].
 
     Args:
         df ([pd.DataFrame]): Dataframe with measurements. This dataframe
         typically consists of wd_%03d, ws_%03d, ti_%03d, pow_%03d, and
         potentially additional measurements.
         df_upstream ([pd.DataFrame]): Dataframe containing rows indicating
-        wind direction ranges and the corresponding upstream turbines for 
+        wind direction ranges and the corresponding upstream turbines for
         that wind direction range. This variable can be generated with
-        flasc.floris_tools.get_upstream_turbs_floris(...).
+        flasc.utilities.floris_tools.get_upstream_turbs_floris(...).
         turb_no ([int]): Turbine number from which the radius should be
         calculated.
         x_turbs ([list, array]): Array containing x locations of turbines.
         y_turbs ([list, array]): Array containing y locations of turbines.
         max_radius ([float]): Maximum radius for the upstream turbines
         until which they are still considered as relevant/used for the
         calculation of the averaged column quantity.
@@ -627,40 +655,42 @@
         to False.
 
     Returns:
         df ([pd.DataFrame]): Dataframe which equals the inserted dataframe
         plus the additional column called 'pow_ref'.
     """
     return _set_col_by_upstream_turbines_in_radius(
-        col_out='pow_ref',
-        col_prefix='pow',
+        col_out="pow_ref",
+        col_prefix="pow",
         df=df,
         df_upstream=df_upstream,
         turb_no=turb_no,
         x_turbs=x_turbs,
         y_turbs=y_turbs,
         max_radius=max_radius,
         circular_mean=False,
-        include_itself=include_itself)
+        include_itself=include_itself,
+    )
 
 
-def set_pow_ref_by_n_closest_upstream_turbines(df, df_upstream, turb_no,
-    x_turbs, y_turbs, exclude_turbs=[], N=5):
+def set_pow_ref_by_n_closest_upstream_turbines(
+    df, df_upstream, turb_no, x_turbs, y_turbs, exclude_turbs=[], N=5
+):
     """Add a column called 'pow_ref' to your dataframe, which is the
     mean of the columns pow_%03d for the 5 closest turbines that are
     upstream of the turbine of interest [turb_no].
 
     Args:
         df ([pd.DataFrame]): Dataframe with measurements. This dataframe
         typically consists of wd_%03d, ws_%03d, ti_%03d, pow_%03d, and
         potentially additional measurements.
         df_upstream ([pd.DataFrame]): Dataframe containing rows indicating
-        wind direction ranges and the corresponding upstream turbines for 
+        wind direction ranges and the corresponding upstream turbines for
         that wind direction range. This variable can be generated with
-        flasc.floris_tools.get_upstream_turbs_floris(...).
+        flasc.utilities.floris_tools.get_upstream_turbs_floris(...).
         turb_no ([int]): Turbine number from which the radius should be
         calculated.
         x_turbs ([list, array]): Array containing x locations of turbines.
         y_turbs ([list, array]): Array containing y locations of turbines.
         max_radius ([float]): Maximum radius for the upstream turbines
         until which they are still considered as relevant/used for the
         calculation of the averaged column quantity.
@@ -669,24 +699,25 @@
         to False.
 
      Returns:
         df ([pd.DataFrame]): Dataframe which equals the inserted dataframe
         plus the additional column called 'pow_ref'.
     """
     return _set_col_by_n_closest_upstream_turbines(
-        col_out='pow_ref',
-        col_prefix='pow',
+        col_out="pow_ref",
+        col_prefix="pow",
         N=N,
         df=df,
         df_upstream=df_upstream,
         turb_no=turb_no,
         x_turbs=x_turbs,
         y_turbs=y_turbs,
         exclude_turbs=exclude_turbs,
-        circular_mean=False)
+        circular_mean=False,
+    )
 
 
 def df_reduce_precision(df_in, verbose=False, allow_convert_to_integer=True):
     """Reduce the precision in dataframes from float64 to float32, or possibly
     even further to int32, int16, int8 or even bool. This operation typically
     reduces the size of the dataframe by a factor 2 without any real loss in
     precision. This can make particular operations and data storage much more
@@ -702,82 +733,83 @@
     Returns:
         df_out ([pd.DataFrame]): Reduced dataframe
     """
     list_out = []
     dtypes = df_in.dtypes
     for ii, c in enumerate(df_in.columns):
         datatype = str(dtypes[c])
-        if ((datatype == 'float64') or
-            (datatype == 'float32') or
-            (datatype == 'float')):
+        if (datatype == "float64") or (datatype == "float32") or (datatype == "float"):
             # Check if can be simplified as integer
-            if (not any(np.isnan(df_in[c])) and allow_convert_to_integer and
-                all(np.isclose(np.round(df_in[c]),
-                               df_in[c], equal_nan=True))):
+            if (
+                not any(np.isnan(df_in[c]))
+                and allow_convert_to_integer
+                and all(np.isclose(np.round(df_in[c]), df_in[c], equal_nan=True))
+            ):
                 unique_values = np.unique(df_in[c])
                 if np.array_equal(unique_values, [0, 1]):
                     var_downsampled = df_in[c].astype(bool)
                 elif np.max(df_in[c]) < np.iinfo(np.int8).max:
                     var_downsampled = df_in[c].astype(np.int8)
                 elif np.max(df_in[c]) < np.iinfo(np.int16).max:
                     var_downsampled = df_in[c].astype(np.int16)
                 elif np.max(df_in[c]) < np.iinfo(np.int32).max:
                     var_downsampled = df_in[c].astype(np.int32)
                 else:
                     var_downsampled = df_in[c].astype(np.int64)
             else:  # If not, just simplify as float32
                 var_downsampled = df_in[c].astype(np.float32)
-            max_error = np.max(np.abs(var_downsampled-df_in[c]))
+            max_error = np.max(np.abs(var_downsampled - df_in[c]))
             if verbose:
-                print("Column %s ['%s'] was downsampled to %s."
-                      % (c, datatype, var_downsampled.dtypes))
-                print( "Max error: ", max_error)
-        elif ((datatype == 'int64') or
-              (datatype == 'int32') or
-              (datatype == 'int')):
+                logger.info(
+                    "Column %s ['%s'] was downsampled to %s."
+                    % (c, datatype, var_downsampled.dtypes)
+                )
+                logger.info(f"Max error: {max_error}")
+        elif (datatype == "int64") or (datatype == "int32") or (datatype == "int"):
             if np.array_equal(np.unique(df_in[c]), [0, 1]):
                 var_downsampled = df_in[c].astype(bool)
             elif len(np.unique(df_in[c])) < 100:
                 var_downsampled = df_in[c].astype(np.int16)
             else:
                 var_downsampled = df_in[c].astype(np.int32)
-            max_error = np.max(np.abs(var_downsampled-df_in[c]))
+            max_error = np.max(np.abs(var_downsampled - df_in[c]))
             if verbose:
-                print("Column %s ['%s'] was downsampled to %s."
-                      % (c, datatype, var_downsampled.dtypes))
-                print( "Max error: ", max_error)
+                logger.info(
+                    "Column %s ['%s'] was downsampled to %s."
+                    % (c, datatype, var_downsampled.dtypes)
+                )
+                logger.info(f"Max error: {max_error}")
         else:
             if verbose:
-                print("Datatype '%s' not recognized. Not downsampling."
-                      % datatype)
+                logger.info("Datatype '%s' not recognized. Not downsampling." % datatype)
             var_downsampled = df_in[c]
 
         list_out.append(var_downsampled)
-    
+
     df_out = pd.concat(list_out, axis=1, ignore_index=False)
     return df_out
 
 
 # Functions used for dataframe processing specifically
 def df_drop_nan_rows(df, verbose=False):
     """Remove entries in dataframe where all rows (besides 'time')
     have nan values.
     """
 
     N_init = df.shape[0]
-    colnames = [c for c in df.columns if c not in ['time', 'turbid', 'index']]
-    df = df.dropna(axis=0, subset=colnames, how='all')
+    colnames = [c for c in df.columns if c not in ["time", "turbid", "index"]]
+    df = df.dropna(axis=0, subset=colnames, how="all")
 
     if verbose:
-        print("Reduced dataframe from %d to %d rows." % (N_init, df.shape[0]))
+        logger.info("Reduced dataframe from %d to %d rows." % (N_init, df.shape[0]))
 
     return df
 
 
-def df_find_and_fill_data_gaps_with_missing(df, missing_data_buffer=5.):
+def df_find_and_fill_data_gaps_with_missing(df, missing_data_buffer=5.0):
     """This function takes a pd.DataFrame object and look for large jumps in
        the 'time' column. Rather than simply interpolating these values using
        a ZOH, this rather indicates that measurements are missing. Hence,
        this function finds these time gaps and inserts an additional row
        extra 1 second after the start of the time gap with all 'nan' values.
        This way, the data gap becomes populated with 'nan' values and the data
        will be ignored in any further analysis.
@@ -789,52 +821,60 @@
         corrupted or missing. Defaults to 10.
 
     Returns:
         df ([pd.DataFrame]): The postprocessed dataframe where all data
         within large time gaps hold value 'missing'.
     """
 
-    df = df.sort_values(by='time')
+    df = df.sort_values(by="time")
 
-    time_values = df['time'].values
+    time_values = df["time"].values
     time_delta = np.diff(time_values)
 
-    print('Largest time jump in data is %s s, from %s to %s.'
-          % (max(time_delta)/np.timedelta64(1, 's'),
-                pd.to_datetime(time_values[np.where(time_delta==max(time_delta))[0][0]]),
-                pd.to_datetime(time_values[np.where(time_delta==max(time_delta))[0][0]+1])
-                )
-            )
+    logger.info(
+        "Largest time jump in data is %s s, from %s to %s."
+        % (
+            max(time_delta) / np.timedelta64(1, "s"),
+            pd.to_datetime(time_values[np.where(time_delta == max(time_delta))[0][0]]),
+            pd.to_datetime(time_values[np.where(time_delta == max(time_delta))[0][0] + 1]),
+        )
+    )
     if max(time_delta) >= np.timedelta64(datetime.timedelta(minutes=30)):
-        print('Found a gap of > 30 minutes in data.\n' +
-              ' Are you missing a data file?')
+        logger.warn("Found a gap of > 30 minutes in data.\n" + " Are you missing a data file?")
 
     dt_buffer = np.timedelta64(missing_data_buffer)
     missing_data_idx = np.where(time_delta >= dt_buffer)[0]
     N_datagaps = len(missing_data_idx)
-    td_avg = np.mean(time_delta[missing_data_idx])/np.timedelta64(datetime.timedelta(seconds=1))
-    print("  Found %d time jumps in data with an average of %.2f s. Filling datagaps with 'missing'." % (N_datagaps, td_avg))
-    times_to_insert = [pd.to_datetime(time_values[i]) + datetime.timedelta(seconds=1) for i in missing_data_idx]
+    td_avg = np.mean(time_delta[missing_data_idx]) / np.timedelta64(datetime.timedelta(seconds=1))
+    logger.info(
+        "  Found %d time jumps in data with an average of %.2f s. Filling datagaps with 'missing'."
+        % (N_datagaps, td_avg)
+    )
+    times_to_insert = [
+        pd.to_datetime(time_values[i]) + datetime.timedelta(seconds=1) for i in missing_data_idx
+    ]
 
     # Create empty dataframe and insert times_to_insert as nans
-    df_entries_missing = df[0:1].reset_index().drop(columns='index').drop(0)
-    df_entries_missing['time'] = times_to_insert
-    df_entries_missing = df_entries_missing.replace(pd.NaT, 'missing')
-
-    for mi in np.where(time_delta > np.timedelta64(30, 's'))[0]:
-        print("  Significant time jump in data of %s s has happened from %s to %s."
-              % (time_delta[mi]/np.timedelta64(1, 's'),
-                 pd.to_datetime(time_values[mi]),
-                 pd.to_datetime(time_values[mi+1])
-                 )
-              )
+    df_entries_missing = df[0:1].reset_index().drop(columns="index").drop(0)
+    df_entries_missing["time"] = times_to_insert
+    df_entries_missing = df_entries_missing.replace(pd.NaT, "missing")
+
+    for mi in np.where(time_delta > np.timedelta64(30, "s"))[0]:
+        logger.warn(
+            "  Significant time jump in data of %s s has happened from %s to %s."
+            % (
+                time_delta[mi] / np.timedelta64(1, "s"),
+                pd.to_datetime(time_values[mi]),
+                pd.to_datetime(time_values[mi + 1]),
+            )
+        )
 
     df = df.append(df_entries_missing)  # Add new row with 'missing' entries
-    df = df.sort_values(by='time')  # Sort by time
-    df = df.reset_index().drop(columns='index')  # Reset index
+    df = df.sort_values(by="time")  # Sort by time
+    df = df.reset_index().drop(columns="index")  # Reset index
 
     return df
 
 
 def df_sort_and_find_duplicates(df):
     """This function sorts the dataframe and finds rows with equal time index.
 
@@ -843,30 +883,160 @@
 
     Returns:
         df ([pd.DataFrame]): Dataframe sorted by time
         duplicate_entries_idx ([list of int]): list with indices of the former
         of two duplicate rows. The indices correspond to the time-sorted df.
     """
 
-    df = df.sort_values(axis=0, by='time', ignore_index=True)
-    time_delta = np.diff(df['time'].values)
+    df = df.sort_values(axis=0, by="time", ignore_index=True)
+    time_delta = np.diff(df["time"].values)
     duplicate_entries_idx = np.where(np.abs(np.float64(time_delta)) < 1e-3)[0]
 
     # Clean up
-    if 'index' in df.columns:
-        df = df.drop(columns='index')
+    if "index" in df.columns:
+        df = df.drop(columns="index")
 
     return df, duplicate_entries_idx
 
 
+def is_day_or_night(
+    df: pd.DataFrame,
+    latitude: float,
+    longitude: float,
+    sunrise_altitude: float = 0,
+    sunset_altitude: float = 0,
+    lag_hours: float = 0,
+    datetime_column: str = "time",
+):
+    """
+    Determine whether it's day or night for a given set of coordinates and
+    UTC timestamp in a DataFrame.
+
+    Args:
+        df (pd.DataFrame): A Pandas DataFrame containing the time in UTC and other relevant data.
+        latitude (float): The latitude of the location for which to determine day or night.
+        longitude (float): The longitude of the location for which to determine day or night.
+        sunrise_altitude (float): The altitude of the sun to denote
+            that sunrise has occurred [degress]
+        sunset_altitude (float): The altitude of the sun to denote that
+             sunset has occurred [degress]
+        lag_hours (float, optional): The number of hours to lag behind the
+            timestamp for the daylight
+        determination. Default is 0.
+        datetime_column (str, optional): The name of the DataFrame column containing
+            the timestamp in UTC. Default is 'time'.
+
+    Returns:
+        pd.DataFrame: The input DataFrame with two additional columns: 'sun_altitude'
+            (the sun's altitude at the given timestamp)
+            and 'is_day' (a boolean indicating whether it's daytime at the given timestamp).
+
+    """
+
+    import ephem  # Import here so don't use the memory if not calling this function
+
+    # Create an Observer with the given latitude and longitude
+    observer = ephem.Observer()
+
+    def sun_alt(row):
+        observer.lat = str(latitude)
+        observer.long = str(longitude)
+        observer.date = row[datetime_column] - datetime.timedelta(hours=lag_hours)
+        sun = ephem.Sun()
+        sun.compute(observer)
+        return float(sun.alt) * 180 / np.pi
+
+    # Add a new column 'sun_altitude' to the DataFrame
+    df["sun_altitude"] = df.apply(sun_alt, axis=1)
+    alt_diff = np.diff(df["sun_altitude"], prepend=0)
+    alt_diff[0] = alt_diff[1]  # Assume that the first time matches the second.
+
+    # Apply daytime criteria
+    df["is_day"] = (
+        ((df["sun_altitude"] > sunrise_altitude) & (alt_diff > 0))
+        | ((df["sun_altitude"] > sunset_altitude) & (alt_diff < 0))
+    ).astype(Boolean)
+
+    # If a lag was provided, recompute sun_altitude at the correct time
+    if lag_hours != 0:
+        lag_hours = 0
+        df["sun_altitude"] = df.apply(sun_alt, axis=1)
+
+    return df
+
+
+def plot_sun_altitude_with_day_night_color(df: pd.DataFrame, ax: plt.axis = None):
+    """
+    Plot Sun Altitude with Day-Night Color Differentiation.
+
+    This function creates a plot of Sun Altitude over time,
+    distinguishing between day and night periods
+    with different background colors. The input DataFrame 'df'
+    should contain time and sun_altitude columns,
+    as well as a boolean 'is_day' column to indicate day and night periods.
+
+    Args:
+        df (pd.DataFrame): A DataFrame containing time, sun_altitude, and is_day columns.
+        ax (plt.axis, optional): An optional Matplotlib axis to use for the plot.
+        If not provided, a new axis will be created.
+
+    Returns:
+        ax (plt.axis): The Matplotlib axis plotted on.
+    """
+    # Separate the DataFrame into day and night parts
+    day_data = df[df["is_day"]]
+    night_data = df[~df["is_day"]]
+
+    # Create a figure and axis for the plot
+    if ax is None:
+        fig, ax = plt.subplots()
+
+    # Plot day data with a blue background
+    ax.plot(
+        day_data["time"],
+        day_data["sun_altitude"],
+        color="orange",
+        label="Day",
+        marker=".",
+        ls="None",
+    )
+    # ax.fill_between(day_data['time'], day_data['sun_altitude'], color='orange', alpha=0.7)
+
+    # Plot night data with a black background
+    ax.plot(
+        night_data["time"],
+        night_data["sun_altitude"],
+        color="darkblue",
+        label="Night",
+        marker=".",
+        ls="None",
+    )
+    # ax.fill_between(night_data['time'], night_data['sun_altitude'], color='darkblue', alpha=0.7)
+
+    # Set axis labels and a legend
+    ax.set_xlabel("Time")
+    ax.set_ylabel("Sun altitude [deg]")
+    ax.legend(loc="upper right")
+
+    # Rotate x-axis labels for readability
+    fig = plt.gcf()
+    fig.autofmt_xdate(rotation=45)
+
+    # Final touches
+    ax.grid(True)
+    ax.axhline(0, color="k", lw=2)
+
+    return ax
+
+
 def make_df_wide(df):
-    df["turbid"] = df['turbid'].astype(int)
+    df["turbid"] = df["turbid"].astype(int)
     df = df.reset_index(drop=False)
-    if 'index' in df.columns:
-        df = df.drop(columns='index')
+    if "index" in df.columns:
+        df = df.drop(columns="index")
     df = df.set_index(["time", "turbid"], drop=True)
     df = df.unstack()
     df.columns = ["%s_%s" % c for c in df.columns]
     df = df.reset_index(drop=False)
     return df
 
 
@@ -887,19 +1057,19 @@
     # Check and merge any duplicate entries in the dataset
     df, duplicate_time_entries = df_sort_and_find_duplicates(df)
     while len(duplicate_time_entries) > 0:
         di = duplicate_time_entries[0]
         # df_subset = df[di:di+2].copy()
 
         # Check if any conflicting entries exist within duplicate rows
-        column_list = [c for c in df.columns if (c != 'time' and c != 'index')]
-        df_merged = df[di:di+1].copy().reset_index(drop=True)  # Start with first row
+        column_list = [c for c in df.columns if (c != "time" and c != "index")]
+        df_merged = df[di : di + 1].copy().reset_index(drop=True)  # Start with first row
         for c in column_list:
             x1 = df.loc[di, c]
-            x2 = df.loc[di+1, c]
+            x2 = df.loc[di + 1, c]
 
             # Check if either is NaN
             x1_isnan = not (x1 == x1)
             x2_isnan = not (x2 == x2)
 
             # Check if values conflict
             if x1_isnan:
@@ -912,30 +1082,29 @@
                 is_faulty = False
                 # Do nothing, keep x1
             else:
                 is_faulty = True
                 df_merged.loc[0, c] = np.nan
 
             if is_faulty:
-                import warnings
-                warnings.warn('Found conflicting data entries for timestamp: '
-                              + str(df.loc[di, 'time']) + '.')
-                print(df.loc[di:di+1, c])
-                print('Setting value to np.nan as a safety measure...')
-
-        print('Merged two rows with identical timestamp:',
-              df.loc[di, 'time'], '.')
-        print('Before merging:')
-        print(df[di:di+2])
-        print(' ')
-        print('After merging:')
+                logger.warn(
+                    "Found conflicting data entries for timestamp: " + str(df.loc[di, "time"]) + "."
+                )
+                print(df.loc[di : di + 1, c])
+                logger.info("Setting value to np.nan as a safety measure...")
+
+        logger.info(f"Merged two rows with identical timestamp:{df.loc[di, 'time']}.")
+        logger.info("Before merging:")
+        print(df[di : di + 2])
+        logger.info(" ")
+        logger.info("After merging:")
         print(df_merged)
-        print(' ')
+        logger.info(" ")
 
         # Now merge data
-        df = df.reset_index().drop([di, di+1])  # Remove dupl. rows
+        df = df.reset_index().drop([di, di + 1])  # Remove dupl. rows
         df = df.append(df_merged)  # Add merged row
 
         # Sort df by 'time' and recalculate duplicate entries
         df, duplicate_time_entries = df_sort_and_find_duplicates(df)
 
     return df
```

### Comparing `flasc-1.4.2/flasc/energy_ratio/energy_ratio.py` & `flasc-2.0/flasc/analysis/energy_ratio.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,211 +1,253 @@
-# This is a work in progress as we try to synthesize ideas from the 
-# table based methods and energy ratios back into one thing, 
+# This is a work in progress as we try to synthesize ideas from the
+# table based methods and energy ratios back into one thing,
 # some ideas we're incorporating:
 
 # Conversion from polars to pandas
 # Constructing tables (but now including tables of ratios)
 # Keeping track of frequencies is matching sized tables
 
-import warnings
-import numpy as np
 import polars as pl
 
-import flasc.energy_ratio.energy_ratio_utilities as util
+import flasc.utilities.energy_ratio_utilities as util
+from flasc.analysis.energy_ratio_input import EnergyRatioInput
+from flasc.analysis.energy_ratio_output import EnergyRatioOutput
+from flasc.data_processing.dataframe_manipulations import df_reduce_precision
+from flasc.logging_manager import LoggingManager
 
-from flasc.energy_ratio.energy_ratio_output import EnergyRatioOutput
-from flasc.energy_ratio.energy_ratio_input import EnergyRatioInput
-from flasc.dataframe_operations.dataframe_manipulations import df_reduce_precision
+logger_manager = LoggingManager()  # Instantiate LoggingManager
+logger = logger_manager.logger  # Obtain the reusable logger
 
 
 # Internal version, returns a polars dataframe
-def _compute_energy_ratio_single(df_,
-                         df_names,
-                         ref_cols,
-                         test_cols,
-                         wd_cols,
-                         ws_cols,
-                         wd_step = 2.0,
-                         wd_min = 0.0,
-                         wd_max = 360.0,
-                         ws_step = 1.0,
-                         ws_min = 0.0,
-                         ws_max = 50.0,
-                         bin_cols_in = ['wd_bin','ws_bin'],
-                         weight_by = 'min', #min, sum
-                         df_freq_pl = None,
-                         wd_bin_overlap_radius = 0.,
-                         uplift_pairs = [],
-                         uplift_names = [],
-                         uplift_absolute = False,
-                         remove_all_nulls = False
-                         ):
-
+def _compute_energy_ratio_single(
+    df_,
+    df_names,
+    ref_cols,
+    test_cols,
+    wd_cols,
+    ws_cols,
+    wd_step=2.0,
+    wd_min=0.0,
+    wd_max=360.0,
+    ws_step=1.0,
+    ws_min=0.0,
+    ws_max=50.0,
+    bin_cols_in=["wd_bin", "ws_bin"],
+    weight_by="min",  # min, sum
+    df_freq_pl=None,
+    wd_bin_overlap_radius=0.0,
+    uplift_pairs=[],
+    uplift_names=[],
+    uplift_absolute=False,
+    remove_all_nulls=False,
+):
     """
     Compute the energy ratio between two sets of turbines.
 
     Args:
         df_ (pl.DataFrame): A dataframe containing the data to use in the calculation.
-        df_names (list): A list of names to give to the dataframes. 
+        df_names (list): A list of names to give to the dataframes.
         ref_cols (list[str]): A list of columns to use as the reference turbines
         test_cols (list[str]): A list of columns to use as the test turbines
         wd_cols (list[str]): A list of columns to derive the wind directions from
         ws_cols (list[str]): A list of columns to derive the wind speeds from
         wd_step (float): The width of the wind direction bins.
         wd_min (float): The minimum wind direction to use.
         wd_max (float): The maximum wind direction to use.
         ws_step (float): The width of the wind speed bins.
         ws_min (float): The minimum wind speed to use.
         ws_max (float): The maximum wind speed to use.
-        bin_cols_in (list[str]): A list of column names to use for the wind speed and wind direction bins.
+        bin_cols_in (list[str]): A list of column names to use for
+            the wind speed and wind direction bins.
         weight_by (str): How to weight the energy ratio, options are 'min', or 'sum'.  'min' means
-            the minimum count across the dataframes is used to weight the energy ratio.   'sum' means the sum of the counts
+            the minimum count across the dataframes is used to weight the energy ratio.
+            'sum' means the sum of the counts
             across the dataframes is used to weight the energy ratio.   Defaults to 'min'.
         df_freq_pl (pl.Dataframe) Polars dataframe of pre-provided per bin weights
-        wd_bin_overlap_radius (float): The distance in degrees one wd bin overlaps into the next, must be 
+        wd_bin_overlap_radius (float): The distance in degrees one wd bin
+            overlaps into the next, must be
             less or equal to half the value of wd_step
-        uplift_pairs: (list[tuple]): List of pairs of df_names to compute uplifts for. Each element 
-            of the list should be a tuple (or list) of length 2, where the first element will be the 
-            base case in the uplift calculation and the second element will be the test case in the 
+        uplift_pairs: (list[tuple]): List of pairs of df_names to compute uplifts for. Each element
+            of the list should be a tuple (or list) of length 2, where the first element will be the
+            base case in the uplift calculation and the second element will be the test case in the
             uplift calculation. If None, no uplifts are computed.
-        uplift_names: (list[str]): Names for the uplift columns, following the order of the 
+        uplift_names: (list[str]): Names for the uplift columns, following the order of the
             pairs specified in uplift_pairs. If None, will default to "uplift_df_name1_df_name2",
-        uplift_absolute: (bool): If True, return uplift in absolute error instead of default percent change
+        uplift_absolute: (bool): If True, return uplift in
+            absolute error instead of default percent change
             defaults to False
-        remove_all_nulls: (bool): Construct reference and test by strictly requiring all data to be 
-            available. If False, a minimum one data point from ref_cols, test_cols, wd_cols, and ws_cols
+        remove_all_nulls: (bool): Construct reference and test by strictly requiring all data to be
+            available. If False, a minimum one data point from ref_cols,
+            test_cols, wd_cols, and ws_cols
             must be available to compute the bin. Defaults to False.
 
     Returns:
         pl.DataFrame: A dataframe containing the energy ratio for each wind direction bin
         pl.DataFrame: A dataframe containing the weights each wind direction and wind speed bin
     """
 
     # Get the number of dataframes
     num_df = len(df_names)
 
-    bin_cols_without_df_name = [c for c in bin_cols_in if c != 'df_name']
-
+    bin_cols_without_df_name = [c for c in bin_cols_in if c != "df_name"]
 
     # Filter df_ to remove null values
     null_filter = util.filter_all_nulls if remove_all_nulls else util.filter_any_nulls
     df_ = null_filter(df_, ref_cols, test_cols, ws_cols, wd_cols)
     if len(df_) == 0:
         raise RuntimeError("After removing nulls, no data remains for computation.")
 
     # Apply binning to dataframe and group by bin
-    df_ = util.bin_and_group_dataframe(df_, ref_cols, test_cols, wd_cols, ws_cols, wd_step, wd_min, 
-        wd_max, ws_step, ws_min, ws_max, wd_bin_overlap_radius,
-        remove_all_nulls, bin_cols_without_df_name, num_df)
-    
+    df_ = util.bin_and_group_dataframe(
+        df_,
+        ref_cols,
+        test_cols,
+        wd_cols,
+        ws_cols,
+        wd_step,
+        wd_min,
+        wd_max,
+        ws_step,
+        ws_min,
+        ws_max,
+        wd_bin_overlap_radius,
+        remove_all_nulls,
+        bin_cols_without_df_name,
+        num_df,
+    )
+
     # Determine the weighting of the ws/wd bins
     df_, df_freq_pl = util.add_bin_weights(df_, df_freq_pl, bin_cols_without_df_name, weight_by)
 
     # Calculate energy ratios
-    df_ = (df_
-        .with_columns(
+    df_ = (
+        df_.with_columns(
             [
-                pl.col('pow_ref').mul(pl.col('weight')).alias('ref_energy'), # Compute the reference energy
-                pl.col('pow_test').mul(pl.col('weight')).alias('test_energy'), # Compute the test energy
+                pl.col("pow_ref")
+                .mul(pl.col("weight"))
+                .alias("ref_energy"),  # Compute the reference energy
+                pl.col("pow_test")
+                .mul(pl.col("weight"))
+                .alias("test_energy"),  # Compute the test energy
             ]
         )
-        .group_by(['wd_bin','df_name'], maintain_order=True)
-        .agg([pl.sum("ref_energy"), pl.sum("test_energy"),pl.sum("count")])
-        .with_columns(
-            energy_ratio = pl.col('test_energy') / pl.col('ref_energy')
+        .group_by(["wd_bin", "df_name"], maintain_order=True)
+        .agg([pl.sum("ref_energy"), pl.sum("test_energy"), pl.sum("count")])
+        .with_columns(energy_ratio=pl.col("test_energy") / pl.col("ref_energy"))
+        .pivot(
+            values=["energy_ratio", "count"],
+            columns="df_name",
+            index="wd_bin",
+            aggregate_function="first",
         )
-        .pivot(values=['energy_ratio','count'], columns='df_name', index='wd_bin',aggregate_function='first')
-        .rename({f'energy_ratio_df_name_{n}' : n for n in df_names})
-        .rename({f'count_df_name_{n}' : f'count_{n}'  for n in df_names})
-        .sort('wd_bin')
+        .rename({f"energy_ratio_df_name_{n}": n for n in df_names})
+        .rename({f"count_df_name_{n}": f"count_{n}" for n in df_names})
+        .sort("wd_bin")
     )
 
     # In the case of two turbines, compute an uplift column
     for upp, upn in zip(uplift_pairs, uplift_names):
-        count_cols = ["count_"+upp[0], "count_"+upp[1]]
+        count_cols = ["count_" + upp[0], "count_" + upp[1]]
         if not uplift_absolute:
             df_ = df_.with_columns(
-                [(100 * (pl.col(upp[1]) - pl.col(upp[0])) / pl.col(upp[0])).alias(upn),
-                (pl.min_horizontal(count_cols) if weight_by == "min" else 
-                 pl.sum_horizontal(count_cols)).alias("count_"+upn)
+                [
+                    (100 * (pl.col(upp[1]) - pl.col(upp[0])) / pl.col(upp[0])).alias(upn),
+                    (
+                        pl.min_horizontal(count_cols)
+                        if weight_by == "min"
+                        else pl.sum_horizontal(count_cols)
+                    ).alias("count_" + upn),
                 ]
             )
         else:
             df_ = df_.with_columns(
-                [(pl.col(upp[1]) - pl.col(upp[0])).alias(upn),
-                (pl.min_horizontal(count_cols) if weight_by == "min" else 
-                 pl.sum_horizontal(count_cols)).alias("count_"+upn)
+                [
+                    (pl.col(upp[1]) - pl.col(upp[0])).alias(upn),
+                    (
+                        pl.min_horizontal(count_cols)
+                        if weight_by == "min"
+                        else pl.sum_horizontal(count_cols)
+                    ).alias("count_" + upn),
                 ]
             )
 
-
     # Enforce a column order
-    df_ = df_.select(['wd_bin'] + df_names + uplift_names + [f'count_{n}' for n in df_names+uplift_names])
+    df_ = df_.select(
+        ["wd_bin"] + df_names + uplift_names + [f"count_{n}" for n in df_names + uplift_names]
+    )
 
     return df_, df_freq_pl
 
+
 # Bootstrap function wraps the _compute_energy_ratio function
-def _compute_energy_ratio_bootstrap(er_in,
-                         ref_cols,
-                         test_cols,
-                         wd_cols,
-                         ws_cols,
-                         wd_step = 2.0,
-                         wd_min = 0.0,
-                         wd_max = 360.0,
-                         ws_step = 1.0,
-                         ws_min = 0.0,
-                         ws_max = 50.0,
-                         bin_cols_in = ['wd_bin','ws_bin'],
-                         weight_by = 'min', #min, sum
-                         df_freq_pl = None,
-                         wd_bin_overlap_radius = 0.,
-                         uplift_pairs = [],
-                         uplift_names = [],
-                         uplift_absolute = False,
-                         N = 1,
-                         percentiles=[5., 95.],
-                         remove_all_nulls=False,
-                         ):
-    
+def _compute_energy_ratio_bootstrap(
+    er_in,
+    ref_cols,
+    test_cols,
+    wd_cols,
+    ws_cols,
+    wd_step=2.0,
+    wd_min=0.0,
+    wd_max=360.0,
+    ws_step=1.0,
+    ws_min=0.0,
+    ws_max=50.0,
+    bin_cols_in=["wd_bin", "ws_bin"],
+    weight_by="min",  # min, sum
+    df_freq_pl=None,
+    wd_bin_overlap_radius=0.0,
+    uplift_pairs=[],
+    uplift_names=[],
+    uplift_absolute=False,
+    N=1,
+    percentiles=[5.0, 95.0],
+    remove_all_nulls=False,
+):
     """
     Compute the energy ratio between two sets of turbines with bootstrapping
 
     Args:
-        er_in (EnergyRatioInput): An EnergyRatioInput object containing the data to use in the calculation.
+        er_in (EnergyRatioInput): An EnergyRatioInput object containing
+            the data to use in the calculation.
         ref_cols (list[str]): A list of columns to use as the reference turbines
         test_cols (list[str]): A list of columns to use as the test turbines
         wd_cols (list[str]): A list of columns to derive the wind directions from
         ws_cols (list[str]): A list of columns to derive the wind speeds from
         wd_step (float): The width of the wind direction bins.
         wd_min (float): The minimum wind direction to use.
         wd_max (float): The maximum wind direction to use.
         ws_step (float): The width of the wind speed bins.
         ws_min (float): The minimum wind speed to use.
         ws_max (float): The maximum wind speed to use.
-        bin_cols_in (list[str]): A list of column names to use for the wind speed and wind direction bins.
+        bin_cols_in (list[str]): A list of column names to use for the wind
+            speed and wind direction bins.
         weight_by (str): How to weight the energy ratio, options are 'min', or 'sum'.  'min' means
-            the minimum count across the dataframes is used to weight the energy ratio. 'sum' means the sum of the counts
+            the minimum count across the dataframes is used to weight the energy ratio.
+            'sum' means the sum of the counts
             across the dataframes is used to weight the energy ratio.
         df_freq_pl (pl.Dataframe) Polars dataframe of pre-provided per bin weights
-        wd_bin_overlap_radius (float): The distance in degrees one wd bin overlaps into the next, must be 
+        wd_bin_overlap_radius (float): The distance in degrees one wd bin overlaps
+            into the next, must be
             less or equal to half the value of wd_step
-        uplift_pairs: (list[tuple]): List of pairs of df_names to compute uplifts for. Each element 
-            of the list should be a tuple (or list) of length 2, where the first element will be the 
-            base case in the uplift calculation and the second element will be the test case in the 
+        uplift_pairs: (list[tuple]): List of pairs of df_names to compute uplifts for. Each element
+            of the list should be a tuple (or list) of length 2, where the first element will be the
+            base case in the uplift calculation and the second element will be the test case in the
             uplift calculation. If None, no uplifts are computed.
-        uplift_names: (list[str]): Names for the uplift columns, following the order of the 
+        uplift_names: (list[str]): Names for the uplift columns, following the order of the
             pairs specified in uplift_pairs. If None, will default to "uplift_df_name1_df_name2"
-        uplift_absolute: (bool): If True, return uplift in absolute error instead of default percent change
+        uplift_absolute: (bool): If True, return uplift in absolute error
+            instead of default percent change
             defaults to True
         N (int): The number of bootstrap samples to use.
-        percentiles: (list or None): percentiles to use when returning energy ratio bounds. 
+        percentiles: (list or None): percentiles to use when returning energy ratio bounds.
             If specified as None with N > 1 (bootstrapping), defaults to [5, 95].
-        remove_all_nulls: (bool): Construct reference and test by strictly requiring all data to be 
-                available. If False, a minimum one data point from ref_cols, test_cols, wd_cols, and ws_cols
+        remove_all_nulls: (bool): Construct reference and test by strictly requiring all data to be
+                available. If False, a minimum one data point from
+                ref_cols, test_cols, wd_cols, and ws_cols
                 must be available to compute the bin. Defaults to False.
 
 
     Returns:
         pl.DataFrame: A dataframe containing the energy ratio between the two sets of turbines.
 
     """
@@ -228,107 +270,122 @@
             bin_cols_in,
             weight_by,
             df_freq_pl,
             wd_bin_overlap_radius,
             uplift_pairs,
             uplift_names,
             uplift_absolute,
-            remove_all_nulls
-        ) for i in range(N)
+            remove_all_nulls,
+        )
+        for i in range(N)
     ]
     df_concat = pl.concat([er_single_out[0] for er_single_out in er_single_outs])
     # First output contains the original table; use that df_freq_pl
     df_freq_pl = er_single_outs[0][1]
 
     bound_names = er_in.df_names + uplift_names
 
-    return (df_concat
-            .group_by(['wd_bin'], maintain_order=True)
-            .agg([pl.first(n) for n in bound_names] + 
-                    [pl.quantile(n, percentiles[0]/100).alias(n + "_ub") for n in bound_names] +
-                    [pl.quantile(n, percentiles[1]/100).alias(n + "_lb") for n in bound_names] + 
-                    [pl.first(f'count_{n}') for n in bound_names]
-                )
-            .sort('wd_bin')
-            ), df_freq_pl
-
-def compute_energy_ratio(er_in: EnergyRatioInput,
-                         ref_turbines = None,
-                         test_turbines = None,
-                         wd_turbines = None,
-                         ws_turbines = None,
-                         use_predefined_ref = False,
-                         use_predefined_wd = False,
-                         use_predefined_ws = False,
-                         wd_step = 2.0,
-                         wd_min = 0.0,
-                         wd_max = 360.0,
-                         ws_step = 1.0,
-                         ws_min = 0.0,
-                         ws_max = 50.0,
-                         bin_cols_in = ['wd_bin','ws_bin'],
-                         weight_by = 'min', #min or sum
-                         df_freq = None,
-                         wd_bin_overlap_radius = 0.,
-                         uplift_pairs = None,
-                         uplift_names = None,
-                         uplift_absolute = False,
-                         N = 1,
-                         percentiles = None,
-                         remove_all_nulls = False,
-                         )-> EnergyRatioOutput:
-    
+    return (
+        df_concat.group_by(["wd_bin"], maintain_order=True)
+        .agg(
+            [pl.first(n) for n in bound_names]
+            + [pl.quantile(n, percentiles[0] / 100).alias(n + "_ub") for n in bound_names]
+            + [pl.quantile(n, percentiles[1] / 100).alias(n + "_lb") for n in bound_names]
+            + [pl.first(f"count_{n}") for n in bound_names]
+        )
+        .sort("wd_bin")
+    ), df_freq_pl
+
+
+def compute_energy_ratio(
+    er_in: EnergyRatioInput,
+    ref_turbines=None,
+    test_turbines=None,
+    wd_turbines=None,
+    ws_turbines=None,
+    use_predefined_ref=False,
+    use_predefined_wd=False,
+    use_predefined_ws=False,
+    wd_step=2.0,
+    wd_min=0.0,
+    wd_max=360.0,
+    ws_step=1.0,
+    ws_min=0.0,
+    ws_max=50.0,
+    bin_cols_in=["wd_bin", "ws_bin"],
+    weight_by="min",  # min or sum
+    df_freq=None,
+    wd_bin_overlap_radius=0.0,
+    uplift_pairs=None,
+    uplift_names=None,
+    uplift_absolute=False,
+    N=1,
+    percentiles=None,
+    remove_all_nulls=False,
+) -> EnergyRatioOutput:
     """
     Compute the energy ratio between two sets of turbines with bootstrapping
 
     Args:
-        er_in (EnergyRatioInput): An EnergyRatioInput object containing the data to use in the calculation.
+        er_in (EnergyRatioInput): An EnergyRatioInput object containing
+            the data to use in the calculation.
         ref_turbines (list[int]): A list of turbine numbers to use as the reference.
         test_turbines (list[int]): A list of turbine numbers to use as the test.
         ws_turbines (list[int]): A list of turbine numbers to use for the wind speeds
         wd_turbines (list[int]): A list of turbine numbers to use for the wind directions
         use_predefined_ref (bool): If True, use the pow_ref column of df_ as the reference power.
         use_predefined_ws (bool): If True, use the ws column of df_ as the wind speed.
         use_predefined_wd (bool): If True, use the wd column of df_ as the wind direction.
         wd_step (float): The width of the wind direction bins.
         wd_min (float): The minimum wind direction to use.
         wd_max (float): The maximum wind direction to use.
         ws_step (float): The width of the wind speed bins.
         ws_min (float): The minimum wind speed to use.
         ws_max (float): The maximum wind speed to use.
-        bin_cols_in (list[str]): A list of column names to use for the wind speed and wind direction bins.
+        bin_cols_in (list[str]): A list of column names to use for the wind
+            speed and wind direction bins.
         weight_by (str): How to weight the energy ratio, options are 'min', , or 'sum'.  'min' means
-            the minimum count across the dataframes is used to weight the energy ratio.   'sum' means the sum of the counts
+            the minimum count across the dataframes is used to weight the energy ratio.
+            'sum' means the sum of the counts
             across the dataframes is used to weight the energy ratio.
-        df_freq (pd.Dataframe): A dataframe which specifies the frequency of the ws/wd bin combinations.  Provides
-            a method to use an explicit or long-term weigthing of bins.  Dataframe should include
-            columns ws, wd and freq_val.  ws and wd should correspond to the bin centers resulting from
-            the choices of the ws/wd_min / _max / _step.  In the case that df_freq has extra bins that aren't included 
-            in those given by ws/wd min, max, step, they will be ignored in the energy ratio calculation. 
-            Any bins given by ws/wd min, max, step not present in df_freq will be assigned a frequency of zero. 
+        df_freq (pd.Dataframe): A dataframe which specifies the frequency of
+            the ws/wd bin combinations.  Provides a method to use an explicit or long-term
+            weigthing of bins.  Dataframe should include
+            columns ws, wd and freq_val.  ws and wd should correspond
+            to the bin centers resulting from
+            the choices of the ws/wd_min / _max / _step.  In the case that
+            df_freq has extra bins that aren't included
+            in those given by ws/wd min, max, step, they will be
+            ignored in the energy ratio calculation.
+            Any bins given by ws/wd min, max, step not present in
+            df_freq will be assigned a frequency of zero.
             Defaults to None.
-        wd_bin_overlap_radius (float): The distance in degrees one wd bin overlaps into the next, must be 
+        wd_bin_overlap_radius (float): The distance in degrees one
+            wd bin overlaps into the next, must be
             less or equal to half the value of wd_step
-        uplift_pairs: (list[tuple]): List of pairs of df_names to compute uplifts for. Each element 
-            of the list should be a tuple (or list) of length 2, where the first element will be the 
-            base case in the uplift calculation and the second element will be the test case in the 
+        uplift_pairs: (list[tuple]): List of pairs of df_names to compute uplifts for. Each element
+            of the list should be a tuple (or list) of length 2, where the first element will be the
+            base case in the uplift calculation and the second element will be the test case in the
             uplift calculation. If None, no uplifts are computed.
-        uplift_names: (list[str]): Names for the uplift columns, following the order of the 
+        uplift_names: (list[str]): Names for the uplift columns, following the order of the
             pairs specified in uplift_pairs. If None, will default to "uplift_df_name1_df_name2"
-        uplift_absolute: (bool): If True, return uplift in absolute error instead of default percent change
+        uplift_absolute: (bool): If True, return uplift in absolute error
+            instead of default percent change
             defaults to True
         N (int): The number of bootstrap samples to use.
-        percentiles: (list or None): percentiles to use when returning energy ratio bounds. 
+        percentiles: (list or None): percentiles to use when returning energy ratio bounds.
             If specified as None with N > 1 (bootstrapping), defaults to [5, 95].
-        remove_all_nulls: (bool): Construct reference and test by strictly requiring all data to be 
-                available. If False, a minimum one data point from ref_cols, test_cols, wd_cols, and ws_cols
+        remove_all_nulls: (bool): Construct reference and test by strictly requiring all data to be
+                available. If False, a minimum one data point from
+                ref_cols, test_cols, wd_cols, and ws_cols
                 must be available to compute the bin. Defaults to False.
 
     Returns:
-        EnergyRatioOutput: An EnergyRatioOutput object containing the energy ratio between the two sets of turbines.
+        EnergyRatioOutput: An EnergyRatioOutput object containing the energy
+            ratio between the two sets of turbines.
 
     """
 
     # Get the polars dataframe from within the er_in
     df_ = er_in.get_df()
 
     # Check that inputs are valid
@@ -352,32 +409,32 @@
         df_freq,
         wd_bin_overlap_radius,
         uplift_pairs,
         uplift_names,
         uplift_absolute,
         N,
         percentiles,
-        remove_all_nulls
+        remove_all_nulls,
     )
-    
-     # Set up the column names for the reference and test power
+
+    # Set up the column names for the reference and test power
     if not use_predefined_ref:
-        ref_cols = [f'pow_{i:03d}' for i in ref_turbines]
+        ref_cols = [f"pow_{i:03d}" for i in ref_turbines]
     else:
-        ref_cols = ['pow_ref']
+        ref_cols = ["pow_ref"]
 
     if not use_predefined_ws:
-        ws_cols = [f'ws_{i:03d}' for i in ws_turbines]
+        ws_cols = [f"ws_{i:03d}" for i in ws_turbines]
     else:
-        ws_cols = ['ws']
+        ws_cols = ["ws"]
 
     if not use_predefined_wd:
-        wd_cols = [f'wd_{i:03d}' for i in wd_turbines]
+        wd_cols = [f"wd_{i:03d}" for i in wd_turbines]
     else:
-        wd_cols = ['wd']
+        wd_cols = ["wd"]
 
     # Confirm uplift pairs provided correctly
     if uplift_pairs is None:
         uplift_pairs = []
     elif isinstance(uplift_pairs[0], str) and len(uplift_pairs) == 2:
         # Single pair provided, not in list of lists
         uplift_pairs = [uplift_pairs]
@@ -385,46 +442,41 @@
         for up in uplift_pairs:
             if len(up) != 2:
                 raise ValueError("uplift_pairs should be a list of tuples of length 2.")
     if uplift_names is not None:
         if len(uplift_names) != len(uplift_pairs):
             raise ValueError("Length of uplift_names should match length of uplift_pairs")
     else:
-        uplift_names = ["uplift_"+up[1]+"/"+up[0] for up in uplift_pairs]
+        uplift_names = ["uplift_" + up[1] + "/" + up[0] for up in uplift_pairs]
 
     # Convert the numbered arrays to appropriate column names
-    test_cols = [f'pow_{i:03d}' for i in test_turbines]
+    test_cols = [f"pow_{i:03d}" for i in test_turbines]
 
     # If df_freq is provided, confirm is consistent with ws/wd min max and
     # prepare a polars table of weights
     if df_freq is not None:
-
         # Maybe not test, not sure yet
         # ws_edges = np.arange(ws_min, ws_max+ws_step,ws_step)
         # ws_labels = ws_edges[:-1] + np.diff(ws_edges)/2.0
         # wd_edges = np.arange(wd_min, wd_max+wd_step,wd_step)
         # wd_labels = wd_edges[:-1] + np.diff(wd_edges)/2.0
-        
+
         # Conver to polars dataframe
         df_freq_pl = pl.from_pandas(df_reduce_precision(df_freq, allow_convert_to_integer=False))
 
         # Rename the columns
-        df_freq_pl = df_freq_pl.rename({
-            'ws':'ws_bin',
-            'wd':'wd_bin',
-            'freq_val':'weight'
-        })
+        df_freq_pl = df_freq_pl.rename({"ws": "ws_bin", "wd": "wd_bin", "freq_val": "weight"})
 
     else:
         df_freq_pl = None
 
     # If N=1, don't use bootstrapping
     if N == 1:
         if percentiles is not None:
-            print("percentiles can only be used with bootstrapping (N > 1).")
+            logger.warn("percentiles can only be used with bootstrapping (N > 1).")
         # Compute the energy ratio
         df_res, df_freq_pl = _compute_energy_ratio_single(
             df_,
             er_in.df_names,
             ref_cols,
             test_cols,
             wd_cols,
@@ -438,22 +490,24 @@
             bin_cols_in,
             weight_by,
             df_freq_pl,
             wd_bin_overlap_radius,
             uplift_pairs,
             uplift_names,
             uplift_absolute,
-            remove_all_nulls
+            remove_all_nulls,
         )
     else:
         if percentiles is None:
             percentiles = [5, 95]
         elif not hasattr(percentiles, "__len__") or len(percentiles) != 2:
-            raise ValueError("percentiles should be a two element list of the "+\
-                "upper and lower desired percentiles.")
+            raise ValueError(
+                "percentiles should be a two element list of the "
+                + "upper and lower desired percentiles."
+            )
 
         df_res, df_freq_pl = _compute_energy_ratio_bootstrap(
             er_in,
             ref_cols,
             test_cols,
             wd_cols,
             ws_cols,
@@ -467,33 +521,35 @@
             weight_by,
             df_freq_pl,
             wd_bin_overlap_radius,
             uplift_pairs,
             uplift_names,
             uplift_absolute,
             N,
-            percentiles
+            percentiles,
         )
-    
+
     # Return the df_freqs, handle as needed.
-    
+
     # Sort df_res by df_names, ws, wd
 
     # Return the results as an EnergyRatioOutput object
-    return EnergyRatioOutput(df_res.to_pandas(), 
-                                er_in,
-                                df_freq_pl.to_pandas(),
-                                ref_cols, 
-                                test_cols, 
-                                wd_cols,
-                                ws_cols,
-                                uplift_names,
-                                wd_step,
-                                wd_min,
-                                wd_max,
-                                ws_step,
-                                ws_min,
-                                ws_max,
-                                bin_cols_in,
-                                weight_by,
-                                wd_bin_overlap_radius,
-                                N)
+    return EnergyRatioOutput(
+        df_res.to_pandas(),
+        er_in,
+        df_freq_pl.to_pandas(),
+        ref_cols,
+        test_cols,
+        wd_cols,
+        ws_cols,
+        uplift_names,
+        wd_step,
+        wd_min,
+        wd_max,
+        ws_step,
+        ws_min,
+        ws_max,
+        bin_cols_in,
+        weight_by,
+        wd_bin_overlap_radius,
+        N,
+    )
```

### Comparing `flasc-1.4.2/flasc/energy_ratio/energy_ratio_input.py` & `flasc-2.0/flasc/analysis/energy_ratio_input.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-from xmlrpc.client import Boolean
+from typing import List
+
 import numpy as np
 import pandas as pd
 import polars as pl
 
-from typing import Optional, Dict, List, Any, Tuple, Union
-
-from flasc.dataframe_operations.dataframe_manipulations import df_reduce_precision
-
+from flasc.data_processing.dataframe_manipulations import df_reduce_precision
 
-def generate_block_list(N: int, 
-                        num_blocks: int = 10):
 
+def generate_block_list(N: int, num_blocks: int = 10):
     """Generate an np.array of length N where each element is an integer between 0 and num_blocks-1
     with each value repeating N/num_blocks times.
 
     Args:
         N (int): Length of the array to generate
         num_blocks (int): Number of blocks to generate
-        
+
     """
 
     # Test than N and num_blocks are integers greater than 0
     if not isinstance(N, int) or not isinstance(num_blocks, int):
-        raise ValueError('N and num_blocks must be integers')
+        raise ValueError("N and num_blocks must be integers")
     if N <= 0 or num_blocks <= 0:
-        raise ValueError('N and num_blocks must be greater than 0')
-    
+        raise ValueError("N and num_blocks must be greater than 0")
+
     # Num blocks must be less than or equal to N
     if num_blocks > N:
-        raise ValueError('num_blocks must be less than or equal to N')
-
+        raise ValueError("num_blocks must be less than or equal to N")
 
     block_list = np.zeros(N)
     for i in range(num_blocks):
-        block_list[i*N//num_blocks:(i+1)*N//num_blocks] = i
+        block_list[i * N // num_blocks : (i + 1) * N // num_blocks] = i
     return block_list.astype(int)
 
 
 class EnergyRatioInput:
-    """  This class holds the structured inputs for calculating energy ratios
-    """
-    def __init__(self,
-                 df_list_in: List[pd.DataFrame],
-                 df_names: List[str],
-                 num_blocks: int = 10,
+    """This class holds the structured inputs for calculating energy ratios"""
+
+    def __init__(
+        self,
+        df_list_in: List[pd.DataFrame],
+        df_names: List[str],
+        num_blocks: int = 10,
     ) -> None:
         """Initialize the EnergyRatioInput class
 
         Args:
             df_list_in (List[pd.DataFrame]): A list of pandas dataframes to be concatenated
             df_names (List[str]): A list of names for the dataframes
             num_blocks (int): The number of blocks to use for the energy ratio calculation
         """
-        
+
         # Reduce precision if needed and convert to polars
-        df_list = [pl.from_pandas(df_reduce_precision(df, allow_convert_to_integer=False)) for df in df_list_in]
+        df_list = [
+            pl.from_pandas(df_reduce_precision(df, allow_convert_to_integer=False))
+            for df in df_list_in
+        ]
 
         # Get minimal set of columns for the dataframes; drop the rest
         keep_columns = df_list[0].columns
         for df in df_list:
             keep_columns = [c for c in df.columns if c in keep_columns]
         df_list = [df.select(keep_columns) for df in df_list]
 
         # If df_names not provided, give simple numbered names
         if df_names is None:
-            df_names = ['df_'+str(i) for i in range(len(df_list))]
+            df_names = ["df_" + str(i) for i in range(len(df_list))]
 
         # Add a name column to each dataframe
         for i in range(len(df_list)):
-            df_list[i] = df_list[i].with_columns([
-                pl.lit(df_names[i]).alias('df_name')
-            ])
+            df_list[i] = df_list[i].with_columns([pl.lit(df_names[i]).alias("df_name")])
 
         # Add a block column to each dataframe
         for i in range(len(df_list)):
-            df_list[i] = df_list[i].with_columns([
-                pl.Series(generate_block_list(df_list[i].shape[0], num_blocks=num_blocks)).alias('block')
-            ])
+            df_list[i] = df_list[i].with_columns(
+                [
+                    pl.Series(
+                        generate_block_list(df_list[i].shape[0], num_blocks=num_blocks)
+                    ).alias("block")
+                ]
+            )
 
         # Store the results
         self.df_pl = pl.concat(df_list, rechunk=True)
         self.df_names = df_names
         self.num_blocks = num_blocks
 
     def get_df(self) -> pl.DataFrame:
         """Get the concatenated dataframe
 
         Returns:
             pl.DataFrame: The concatenated dataframe
         """
         return self.df_pl.clone()
-    
-    def resample_energy_table(self, 
-                              perform_resample: bool=True
-                              )-> pl.DataFrame:
+
+    def resample_energy_table(self, perform_resample: bool = True) -> pl.DataFrame:
         """Use the block column of an energy table to resample the data.
 
         Args:
             df_e_ (pl.DataFrame): An energy table with a block column
             perform_resample: Boolean, if False returns original energy table
 
         Returns:
@@ -105,15 +105,11 @@
                 the same number of rows as the original
         """
 
         if perform_resample:
             # Generate a random np.array, num_blocks long, where each element is
             #  an integer between 0 and num_blocks-1
             block_list = np.random.randint(0, self.num_blocks, self.num_blocks)
-            
-            return pl.DataFrame(
-                {
-                    'block':block_list
-                }
-                ).join(self.df_pl, how='inner', on='block')
-        else: 
-            return self.get_df()
+
+            return pl.DataFrame({"block": block_list}).join(self.df_pl, how="inner", on="block")
+        else:
+            return self.get_df()
```

### Comparing `flasc-1.4.2/flasc/energy_ratio/energy_ratio_output.py` & `flasc-2.0/flasc/analysis/energy_ratio_output.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 from __future__ import annotations
+
+from typing import Any, Dict, List, Optional, Union
+
+import matplotlib.axes._axes as axes
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import polars as pl
-import matplotlib.pyplot as plt
 import seaborn as sns
 
-from typing import Optional, Dict, List, Any, Tuple, Union
-import matplotlib.axes._axes as axes
-
-from flasc.energy_ratio.energy_ratio_input import EnergyRatioInput
-
-from flasc.energy_ratio.energy_ratio_utilities import (
-    add_ws_bin,
+from flasc.analysis.energy_ratio_input import EnergyRatioInput
+from flasc.utilities.energy_ratio_utilities import (
     add_wd_bin,
+    add_ws_bin,
     filter_all_nulls,
-    filter_any_nulls
+    filter_any_nulls,
 )
 
 
 class EnergyRatioOutput:
-    """  This class is used to store the results of the energy ratio calculations
+    """This class is used to store the results of the energy ratio calculations
     and provide convenient methods for plotting and saving the results.
     """
-    def __init__(self,
-                 df_result: pd.DataFrame,
-                 er_in: EnergyRatioInput,
-                 df_freq: pd.DataFrame,
-                 ref_cols: List[str],
-                 test_cols: List[str],
-                 wd_cols: List[str],
-                 ws_cols: List[str],
-                 uplift_cols: List[str],
-                 wd_step: float,
-                 wd_min: float,
-                 wd_max: float,
-                 ws_step: float,
-                 ws_min: float,
-                 ws_max: float,
-                 bin_cols_in: List[str],
-                 weight_by: str,
-                 wd_bin_overlap_radius: float,
-                 N: int,
-                 remove_all_nulls: bool = False
-                ) -> None:
+
+    def __init__(
+        self,
+        df_result: pd.DataFrame,
+        er_in: EnergyRatioInput,
+        df_freq: pd.DataFrame,
+        ref_cols: List[str],
+        test_cols: List[str],
+        wd_cols: List[str],
+        ws_cols: List[str],
+        uplift_cols: List[str],
+        wd_step: float,
+        wd_min: float,
+        wd_max: float,
+        ws_step: float,
+        ws_min: float,
+        ws_max: float,
+        bin_cols_in: List[str],
+        weight_by: str,
+        wd_bin_overlap_radius: float,
+        N: int,
+        remove_all_nulls: bool = False,
+    ) -> None:
         """Initialize an EnergyRatioOutput object.
 
         Args:
             df_result (pd.DataFrame): The energy ratio results.
             er_in (EnergyRatioInput): The energy table used in the energy ratio calculation.
             df_freq (pd.DataFrame): Weights used for bins.
             ref_cols (List[str]): The column names of the reference turbines.
@@ -57,21 +58,25 @@
             wd_step (float): The wind direction bin size.
             wd_min (float): The minimum wind direction value.
             wd_max (float): The maximum wind direction value.
             ws_step (float): The wind speed bin size.
             ws_min (float): The minimum wind speed value.
             ws_max (float): The maximum wind speed value.
             bin_cols_in (List[str]): TBD
-            weight_by (str): How to weight the energy ratio, options are 'min', or 'sum'.  'min' means
-                the minimum count across the dataframes is used to weight the energy ratio.   'sum' means the sum of the counts
+            weight_by (str): How to weight the energy ratio, options are 'min', or 'sum'.
+                'min' means the minimum count across the dataframes
+                is used to weight the energy ratio.
+                'sum' means the sum of the counts
                 across the dataframes is used to weight the energy ratio.
             wd_bin_overlap_radius (float): The radius of overlap between wind direction bins.
             N (int): The number of bootstrap iterations used in the energy ratio calculation.
-            remove_all_nulls: (bool): Construct reference and test by strictly requiring all data to be 
-                available. If False, a minimum one data point from ref_cols, test_cols, wd_cols, and ws_cols
+            remove_all_nulls: (bool): Construct reference and test by
+                strictly requiring all data to be
+                available. If False, a minimum one data point from
+                ref_cols, test_cols, wd_cols, and ws_cols
                 must be available to compute the bin. Defaults to False.
         """
         self.df_result = df_result
         self.df_freq = df_freq
         self.df_names = er_in.df_names
         self.num_df = len(self.df_names)
         self.er_in = er_in
@@ -88,36 +93,45 @@
         self.ws_max = ws_max
         self.bin_cols_in = bin_cols_in
         self.weight_by = weight_by
         self.wd_bin_overlap_radius = wd_bin_overlap_radius
         self.N = N
         self.remove_all_nulls = remove_all_nulls
 
-    def plot_energy_ratios(self,
+    def plot_energy_ratios(
+        self,
         df_names_subset: Optional[List[str]] = None,
         labels: Optional[List[str]] = None,
         color_dict: Optional[Dict[str, Any]] = None,
         axarr: Optional[Union[axes.Axes, List[axes.Axes]]] = None,
         polar_plot: bool = False,
         show_wind_direction_distribution: bool = True,
         show_wind_speed_distribution: bool | None = None,
         overlay_frequency: bool = False,
-        _is_uplift: bool = False
+        _is_uplift: bool = False,
     ) -> Union[axes.Axes, List[axes.Axes]]:
         """Plot the energy ratios.
 
         Args:
-            df_names_subset (Optional[List[str]], optional): A subset of the dataframes used in the energy ratio calculation. Defaults to None.
-            labels (Optional[List[str]], optional): The labels for the energy ratios. Defaults to None.
-            color_dict (Optional[Dict[str, Any]], optional): A dictionary mapping labels to colors. Defaults to None.
-            axarr (Optional[Union[axes.Axes, List[axes.Axes]]], optional): The axes to plot on. Defaults to None.
-            polar_plot (bool, optional): Whether to plot the energy ratios on a polar plot. Defaults to False.
-            show_wind_direction_distribution (bool, optional): Whether to show the wind direction distribution. Defaults to True.
-            show_wind_speed_distribution (bool, optional): Whether to show the wind speed distribution. Defaults to True, unless polar_plot is True.
-            overlay_frequency (bool, optional): Whether to plot the frequency distribution used for calculation.
+            df_names_subset (Optional[List[str]], optional): A subset of the dataframes
+                used in the energy ratio calculation. Defaults to None.
+            labels (Optional[List[str]], optional): The labels for the energy ratios.
+                 Defaults to None.
+            color_dict (Optional[Dict[str, Any]], optional): A dictionary
+                mapping labels to colors. Defaults to None.
+            axarr (Optional[Union[axes.Axes, List[axes.Axes]]], optional): The axes
+                to plot on. Defaults to None.
+            polar_plot (bool, optional): Whether to plot the energy ratios
+                on a polar plot. Defaults to False.
+            show_wind_direction_distribution (bool, optional): Whether to show
+                 the wind direction distribution. Defaults to True.
+            show_wind_speed_distribution (bool, optional): Whether to show
+                the wind speed distribution. Defaults to True, unless polar_plot is True.
+            overlay_frequency (bool, optional): Whether to plot the
+                frequency distribution used for calculation.
             _is_uplift (bool, optional): Whether being called by plot_uplift(). Defaults to False.
 
         Returns:
             Union[axes.Axes, List[axes.Axes]]: The axes used for plotting.
 
         Raises:
             ValueError: If show_wind_speed_distribution is True and polar_plot is True.
@@ -126,24 +140,24 @@
             - If df_names_subset is None, all dataframes will be plotted.
             - If df_names_subset is not a list, it will be converted to a list.
             - If labels is None, the dataframe names will be used as labels.
             - If color_dict is None, a default color scheme will be used.
             - If axarr is None, a new figure will be created.
         """
         # Handle defaults for show_wind_speed_distribution
-        if show_wind_direction_distribution is None:
+        if show_wind_speed_distribution is None:
             if polar_plot:
-                show_wind_direction_distribution = False
+                show_wind_speed_distribution = False
             else:
-                show_wind_direction_distribution = True
+                show_wind_speed_distribution = True
 
         # Only allow showing the wind speed distribution if polar_plot is False
         if polar_plot and show_wind_speed_distribution:
-            raise ValueError('show_wind_speed_distribution cannot be True if polar_plot is True')
-        
+            raise ValueError("show_wind_speed_distribution cannot be True if polar_plot is True")
+
         # If df_names_subset is None, plot all the dataframes
         if df_names_subset is None:
             df_names_subset = self.df_names
 
         # If df_names_subset is not a list, convert it to a list
         if not isinstance(df_names_subset, list):
             df_names_subset = [df_names_subset]
@@ -157,73 +171,86 @@
 
         # If labels is not a list, convert it to a list
         if not isinstance(labels, list):
             labels = [labels]
 
         # Confirm that the length of labels is the same as the length of df_names_subset
         if len(labels) != N:
-            raise ValueError('Length of labels must be the same as the length of df_names_subset')
+            raise ValueError("Length of labels must be the same as the length of df_names_subset")
 
         # Generate the default colors using the seaborn color palette
-        default_colors = sns.color_palette('colorblind', N)
+        default_colors = sns.color_palette("colorblind", N)
 
         # If color_dict is None, use the default colors
         if color_dict is None:
             color_dict = {labels[i]: default_colors[i] for i in range(N)}
             color_dict["weight"] = "black"
 
         # If color_dict is not a dictionary, raise an error
         if not isinstance(color_dict, dict):
-            raise ValueError('color_dict must be a dictionary')
+            raise ValueError("color_dict must be a dictionary")
 
         # Make sure the keys of color_dict are in labels
-        if not all([label in labels+["weight"] for label in color_dict.keys()]):
-            raise ValueError('color_dict keys must be in df_names_subset')
+        if not all([label in labels + ["weight"] for label in color_dict.keys()]):
+            raise ValueError("color_dict keys must be in df_names_subset")
 
         if axarr is None:
             if polar_plot:
-                _, axarr = plt.subplots(nrows=1, ncols=2, figsize=(10, 5), subplot_kw={'projection': 'polar'})
+                _, axarr = plt.subplots(
+                    nrows=1, ncols=2, figsize=(10, 5), subplot_kw={"projection": "polar"}
+                )
             else:
                 if show_wind_direction_distribution:
                     if show_wind_speed_distribution:
-                        num_rows = 3 # Add rows to show wind speed and wind direction distribution
+                        num_rows = 3  # Add rows to show wind speed and wind direction distribution
                     else:
-                        num_rows = 2 # Add rows to show wind direction distribution
+                        num_rows = 2  # Add rows to show wind direction distribution
                 else:
                     num_rows = 1
-                _, axarr = plt.subplots(nrows=num_rows, ncols=1, sharex=True, figsize=(11, num_rows * 3))
-        else: # Confirm correct number of axes passed in
+                _, axarr = plt.subplots(
+                    nrows=num_rows, ncols=1, sharex=True, figsize=(11, num_rows * 3)
+                )
+        else:  # Confirm correct number of axes passed in
             if polar_plot:
                 if len(axarr) != 2:
-                    raise ValueError('If polar_plot is True, axarr must have length of 2')
+                    raise ValueError("If polar_plot is True, axarr must have length of 2")
             else:
                 if show_wind_direction_distribution:
                     if show_wind_speed_distribution:
                         if len(axarr) != 3:
-                            raise ValueError('If show_wind_speed_distribution and show_wind_direction_distribution are True, axarr must have length of 3')
+                            raise ValueError(
+                                "If show_wind_speed_distribution and "
+                                "show_wind_direction_distribution are"
+                                " True, axarr must have length of 3"
+                            )
                     else:
                         if len(axarr) != 2:
-                            raise ValueError('If show_wind_direction_distribution is True, and show_wind_direction is False axarr must have length of 2')
+                            raise ValueError(
+                                "If show_wind_direction_distribution is True, and"
+                                " show_wind_direction"
+                                " is False axarr must have length of 2"
+                            )
                 else:
                     # Confirm axarr is of type Axes
                     if not isinstance(axarr, plt.Axes):
-                        raise ValueError('If show_wind_direction_distribution and show_wind_speed_distribution are False, axarr be of type matplotlib.pyplot.Axes and not a list of axes')
-
-
+                        raise ValueError(
+                            "If show_wind_direction_distribution and show_wind_speed_distribution"
+                            " are False, axarr be of type matplotlib.pyplot.Axes "
+                            "and not a list of axes"
+                        )
 
         # For plotting, create a copy in case
         df = self.df_result.copy()
 
         # Get x-axis values
         x = np.array(df["wd_bin"], dtype=float)
 
         # Get xlims to add a horizontal line at 1
         xlims = np.linspace(np.min(x) - 4.0, np.max(x) + 4.0, 1000)
 
-
         if polar_plot:
             x = (90.0 - x) * np.pi / 180.0  # Convert to radians
             xlims = (90.0 - xlims) * np.pi / 180.0  # Convert to radians
 
         # Add NaNs to avoid connecting plots over gaps
         dwd = np.min(x[1::] - x[0:-1])
         jumps = np.where(np.diff(x) > dwd * 1.50)[0]
@@ -232,22 +259,22 @@
                 [
                     df,
                     pd.DataFrame(
                         {
                             "wd_bin": x[jumps] + dwd / 2.0,
                             "N_bin": [0] * len(jumps),
                         }
-                    )
+                    ),
                 ],
                 axis=0,
                 ignore_index=False,
             )
             df = df.iloc[np.argsort(df["wd_bin"])].reset_index(drop=True)
             x = np.array(df["wd_bin"], dtype=float)
-            if polar_plot: # Convert to radians
+            if polar_plot:  # Convert to radians
                 x = (90.0 - x) * np.pi / 180.0
 
         # Energy ratio plot ========================================
         if show_wind_direction_distribution:
             ax = axarr[0]
         else:
             ax = axarr
@@ -256,20 +283,18 @@
         if _is_uplift:
             ax.plot(xlims, np.zeros_like(xlims), color="black")
         else:
             ax.plot(xlims, np.ones_like(xlims), color="black")
 
         # Plot the energy ratios
         for df_name, label in zip(df_names_subset, labels):
-
             ax.plot(x, df[df_name], "-o", markersize=3.0, label=label, color=color_dict[label])
 
             # If data includes upper and lower bounds plot them
             if df_name + "_ub" in df.columns:
-
                 ax.fill_between(
                     x,
                     df[df_name + "_lb"],
                     df[df_name + "_ub"],
                     alpha=0.25,
                     color=color_dict[label],
                 )
@@ -278,229 +303,273 @@
         ax.legend()
         ax.grid(visible=True, which="major", axis="both", color="gray")
         ax.grid(visible=True, which="minor", axis="both", color="lightgray")
         ax.minorticks_on()
         ax.set_title("Energy Ratio")
         ax.set_ylabel("Energy Ratio")
 
-
         # Wind Direction Bin Plot ========================================
         if not show_wind_direction_distribution:
             ax.set_xlabel("Wind Direction (deg)")
             return axarr
-        
+
         ax = axarr[1]
 
         # Set the bar width using self.wd_step
         bar_width = (0.7 / N) * self.wd_step
         if polar_plot:
             bar_width = bar_width * np.pi / 180.0
 
         for i, (df_name, label) in enumerate(zip(df_names_subset, labels)):
-            if _is_uplift: # Special case, use the minimum or the sum
-                ax.set_title('Minimum of Points per Bin' if self.weight_by == "min" else
-                    'Sum of Points per Bin')
+            if _is_uplift:  # Special case, use the minimum or the sum
+                ax.set_title(
+                    "Minimum of Points per Bin"
+                    if self.weight_by == "min"
+                    else "Sum of Points per Bin"
+                )
             else:
-                ax.set_title('Number of Points per Bin')
-            
+                ax.set_title("Number of Points per Bin")
+
             x = np.array(self.df_result["wd_bin"], dtype=float)
-            if polar_plot: # Convert to radians
+            if polar_plot:  # Convert to radians
                 x = (90.0 - x) * np.pi / 180.0
             ax.bar(
                 x - (i - N / 2) * bar_width,
-                self.df_result["count_"+df_name],
+                self.df_result["count_" + df_name],
                 width=bar_width,
                 label=label,
-                color=color_dict[label]
+                color=color_dict[label],
             )
         if overlay_frequency:
             if "weight" in color_dict:
                 col = color_dict["weight"]
             else:
                 col = "black"
-            df_wd_weight = self.df_freq.drop(columns='ws_bin').groupby('wd_bin').sum().reset_index()
-            ax.plot(df_wd_weight['wd_bin'], df_wd_weight['weight'], color=col, label="Weight")
+            df_wd_weight = self.df_freq.drop(columns="ws_bin").groupby("wd_bin").sum().reset_index()
+            ax.plot(df_wd_weight["wd_bin"], df_wd_weight["weight"], color=col, label="Weight")
 
         ax.legend()
-        ax.set_ylabel('Number of Points')
-        
+        ax.set_ylabel("Number of Points")
+
         ax.grid(True)
 
         # Wind Speed Distribtution Plot ========================================
         if not show_wind_speed_distribution:
             ax.set_xlabel("Wind Direction (deg)")
             return axarr
 
-        ax = axarr[2]        
+        ax = axarr[2]
 
         df_bin_counts = self._compute_ws_counts()
-        sns.scatterplot(data=df_bin_counts, x='wd_bin', y='ws_bin', size='count',hue='count', ax=ax, legend=True, color='k')
-        ax.set_title('Minimum Number of Points per Bin' if self.weight_by == "min" else 
-            'Sum of Points per Bin')
-        ax.set_xlabel('Wind Direction (deg)')
-        ax.set_ylabel('Wind Speed (m/s)')
-        
+        sns.scatterplot(
+            data=df_bin_counts,
+            x="wd_bin",
+            y="ws_bin",
+            size="count",
+            hue="count",
+            ax=ax,
+            legend=True,
+            color="k",
+        )
+        ax.set_title(
+            "Minimum Number of Points per Bin"
+            if self.weight_by == "min"
+            else "Sum of Points per Bin"
+        )
+        ax.set_xlabel("Wind Direction (deg)")
+        ax.set_ylabel("Wind Speed (m/s)")
+
         ax.grid(True)
 
         return axarr
 
-
-    def plot_uplift(self,
+    def plot_uplift(
+        self,
         uplift_names_subset: Optional[List[str]] = None,
         labels: Optional[List[str]] = None,
         color_dict: Optional[Dict[str, Any]] = None,
         axarr: Optional[Union[axes.Axes, List[axes.Axes]]] = None,
         polar_plot: bool = False,
         show_wind_direction_distribution: bool = True,
         show_wind_speed_distribution: bool = True,
         overlay_frequency: bool = False,
-    )-> Union[axes.Axes, List[axes.Axes]]:
+    ) -> Union[axes.Axes, List[axes.Axes]]:
         """Plot the uplift in energy ratio
 
         Args:
-            uplift_names_subset (Optional[List[str]], optional): A subset of the uplifts computed to print. Defaults to None.
+            uplift_names_subset (Optional[List[str]], optional): A subset
+                of the uplifts computed to print. Defaults to None.
             labels (Optional[List[str]], optional): The labels for the uplifts. Defaults to None.
-            color_dict (Optional[Dict[str, Any]], optional): A dictionary mapping labels to colors. Defaults to None.
-            axarr (Optional[Union[axes.Axes, List[axes.Axes]]], optional): The axes to plot on. Defaults to None.
-            polar_plot (bool, optional): Whether to plot the uplift on a polar plot. Defaults to False.
-            show_wind_direction_distribution (bool, optional): Whether to show the wind direction distribution. Defaults to True.
-            show_wind_speed_distribution (bool, optional): Whether to show the wind speed distribution. Defaults to True, unless polar_plot is True.
-            overlay_frequency (bool, optional): Whether to plot the frequency distribution used for calculation.
+            color_dict (Optional[Dict[str, Any]], optional): A dictionary
+                mapping labels to colors. Defaults to None.
+            axarr (Optional[Union[axes.Axes, List[axes.Axes]]], optional): The axes
+                to plot on. Defaults to None.
+            polar_plot (bool, optional): Whether to plot the uplift on
+                a polar plot. Defaults to False.
+            show_wind_direction_distribution (bool, optional): Whether to
+                show the wind direction distribution. Defaults to True.
+            show_wind_speed_distribution (bool, optional): Whether to
+                show the wind speed distribution. Defaults to True, unless polar_plot is True.
+            overlay_frequency (bool, optional): Whether to
+                plot the frequency distribution used for calculation.
 
         Raises:
             ValueError: If show_wind_speed_distribution is True and polar_plot is True.
 
         Returns:
             Union[axes.Axes, List[axes.Axes]]: The axes used for plotting.
 
         Notes:
             - If axarr is None, a new figure will be created.
             - If axarr is a single axes object, it will be used to plot the uplift.
-            - If axarr is a list of axes objects, each component of the uplift will be plotted on a separate axes object.
+            - If axarr is a list of axes objects, each
+                component of the uplift will be plotted on a separate axes object.
             - If polar_plot is True, the uplift will be plotted on a polar plot.
-            - If show_wind_direction_distribution is True, the wind direction distribution will be shown.
+            - If show_wind_direction_distribution is True,
+                the wind direction distribution will be shown.
             - If show_wind_speed_distribution is True, the wind speed distribution will be shown.
         """
         # Handle defaults for show_wind_speed_distribution
         if show_wind_direction_distribution is None:
             if polar_plot:
                 show_wind_direction_distribution = False
             else:
                 show_wind_direction_distribution = True
-        
+
         # Only allow showing the wind speed distribution if polar_plot is False
         if polar_plot and show_wind_speed_distribution:
-            raise ValueError('show_wind_speed_distribution cannot be True if polar_plot is True')
-        
+            raise ValueError("show_wind_speed_distribution cannot be True if polar_plot is True")
+
         # If df_names_subset is None, plot all the dataframes
         if uplift_names_subset is None:
             uplift_names_subset = self.uplift_cols
 
         # If df_names_subset is not a list, convert it to a list
         if not isinstance(uplift_names_subset, list):
             uplift_names_subset = [uplift_names_subset]
 
         # Total number of energy ratios to plot
         N = len(uplift_names_subset)
 
         if N == 0:
-            raise ValueError("No uplifts to plot. Please specify uplifts when calling compute_energy_ratio().")
+            raise ValueError(
+                "No uplifts to plot. Please specify uplifts when calling compute_energy_ratio()."
+            )
 
         # If labels is None, use the dataframe names
         if labels is None:
             labels = uplift_names_subset
 
         # If labels is not a list, convert it to a list
         if not isinstance(labels, list):
             labels = [labels]
 
         # Confirm that the length of labels is the same as the length of df_names_subset
         if len(labels) != N:
-            raise ValueError('Length of labels must be the same as the length of uplift_names_subset')
+            raise ValueError(
+                "Length of labels must be the same as the length of uplift_names_subset"
+            )
 
         # Generate the default colors using the seaborn color palette
-        default_colors = sns.color_palette('colorblind', N)
+        default_colors = sns.color_palette("colorblind", N)
 
         # If color_dict is None, use the default colors
         if color_dict is None:
             color_dict = {labels[i]: default_colors[i] for i in range(N)}
             color_dict["weight"] = "black"
 
         # If color_dict is not a dictionary, raise an error
         if not isinstance(color_dict, dict):
-            raise ValueError('color_dict must be a dictionary')
+            raise ValueError("color_dict must be a dictionary")
 
         # Make sure the keys of color_dict are in labels
-        if not all([label in labels+["weight"] for label in color_dict.keys()]):
-            raise ValueError('color_dict keys must be in df_names_subset')
-
+        if not all([label in labels + ["weight"] for label in color_dict.keys()]):
+            raise ValueError("color_dict keys must be in df_names_subset")
 
         if axarr is None:
             if polar_plot:
-                _, axarr = plt.subplots(nrows=1, ncols=2, figsize=(10, 5), subplot_kw={'projection': 'polar'})
+                _, axarr = plt.subplots(
+                    nrows=1, ncols=2, figsize=(10, 5), subplot_kw={"projection": "polar"}
+                )
             else:
                 if show_wind_direction_distribution:
                     if show_wind_speed_distribution:
-                        num_rows = 3 # Add rows to show wind speed and wind direction distribution
+                        num_rows = 3  # Add rows to show wind speed and wind direction distribution
                     else:
-                        num_rows = 2 # Add rows to show wind direction distribution
+                        num_rows = 2  # Add rows to show wind direction distribution
                 else:
                     num_rows = 1
-                _, axarr = plt.subplots(nrows=num_rows, ncols=1, sharex=True, figsize=(11, num_rows * 3))
+                _, axarr = plt.subplots(
+                    nrows=num_rows, ncols=1, sharex=True, figsize=(11, num_rows * 3)
+                )
 
         self.plot_energy_ratios(
             df_names_subset=uplift_names_subset,
             labels=labels,
             color_dict=color_dict,
             axarr=axarr,
             polar_plot=polar_plot,
             show_wind_direction_distribution=show_wind_direction_distribution,
             show_wind_speed_distribution=show_wind_speed_distribution,
             overlay_frequency=overlay_frequency,
-            _is_uplift=True
+            _is_uplift=True,
         )
-            
 
         # Finish plots
         if not show_wind_direction_distribution:
             ax = axarr
         else:
             ax = axarr[0]
 
         # Finish Energy Ratio plot
-        ax.set_ylabel('Percent Change')
-        ax.set_title('Uplift in Energy Ratio')
+        ax.set_ylabel("Percent Change")
+        ax.set_title("Uplift in Energy Ratio")
 
         if not show_wind_direction_distribution:
             return axarr
 
         # # Finish Wind Direction Distribution plot
         # ax = axarr[1]
         # ax.set_title("Minimum Number of Points per Bin")
 
         return axarr
 
     def _compute_ws_counts(self):
-        """ Compute the of ws bin counts as previously computed but not presently
-        computed with the energy calculation. """
+        """Compute the of ws bin counts as previously computed but not presently
+        computed with the energy calculation."""
 
         # Temporary copy of energy table
         df_ = self.er_in.get_df()
 
         # Filter df_ to remove null values
         null_filter = filter_all_nulls if self.remove_all_nulls else filter_any_nulls
         df_ = null_filter(df_, self.ref_cols, self.test_cols, self.ws_cols, self.wd_cols)
 
         # Assign the wd/ws bins
-        df_ = add_ws_bin(df_, self.ws_cols, self.ws_step, self.ws_min, self.ws_max,
-            remove_all_nulls=self.remove_all_nulls)
-        df_ = add_wd_bin(df_, self.wd_cols, self.wd_step, self.wd_min, self.wd_max,
-            remove_all_nulls=self.remove_all_nulls)
+        df_ = add_ws_bin(
+            df_,
+            self.ws_cols,
+            self.ws_step,
+            self.ws_min,
+            self.ws_max,
+            remove_all_nulls=self.remove_all_nulls,
+        )
+        df_ = add_wd_bin(
+            df_,
+            self.wd_cols,
+            self.wd_step,
+            self.wd_min,
+            self.wd_max,
+            remove_all_nulls=self.remove_all_nulls,
+        )
 
         # Get the bin count by wd, ws and df_name
-        df_group = df_.groupby(['wd_bin','ws_bin','df_name']).count()
+        df_group = df_.groupby(["wd_bin", "ws_bin", "df_name"]).count()
 
         # Collect the minimum number of points per bin
-        df_return = df_group.groupby(['wd_bin','ws_bin']).min() if self.weight_by == "min" \
-            else df_group.groupby(['wd_bin','ws_bin']).sum()
+        df_return = (
+            df_group.groupby(["wd_bin", "ws_bin"]).min()
+            if self.weight_by == "min"
+            else df_group.groupby(["wd_bin", "ws_bin"]).sum()
+        )
 
-        return df_return.drop('df_name').to_pandas()
+        return df_return.drop("df_name").to_pandas()
```

### Comparing `flasc-1.4.2/flasc/energy_ratio/energy_ratio_utilities.py` & `flasc-2.0/flasc/utilities/energy_ratio_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 import warnings
-import polars as pl
-import numpy as np
+from typing import List, Optional, Union
 
-from typing import Union, List, Optional
+import numpy as np
+import polars as pl
 
 
-#TODO: Someday I think can replace with polars-native code: https://github.com/pola-rs/polars/issues/8551
-def cut(col_name: str,
-        edges: Union[np.ndarray, list],
-    ) -> pl.Expr:
+# TODO: Someday I think can replace with polars-native code: https://github.com/pola-rs/polars/issues/8551
+def cut(
+    col_name: str,
+    edges: Union[np.ndarray, list],
+) -> pl.Expr:
     """
     Bins the values in the specified column according to the given edges.
 
     Parameters:
     col_name (str): The name of the column to bin.
     edges (array-like): The edges of the bins. Values will be placed into the bin
                         whose left edge is the largest edge less than or equal to
                         the value, and whose right edge is the smallest edge
                         greater than the value.
 
     Returns:
     expression: An expression object that can be used to bin the column.
     """
     c = pl.col(col_name)
-    labels = edges[:-1] + np.diff(edges)/2.0
+    labels = edges[:-1] + np.diff(edges) / 2.0
     expr = pl.when(c < edges[0]).then(None)
     for edge, label in zip(edges[1:], labels):
         expr = expr.when(c < edge).then(label)
     expr = expr.otherwise(None)
 
     return expr
 
 
-def bin_column(df_: pl.DataFrame,
-               col_name: str,
-               bin_col_name: str, 
-               edges: Union[np.ndarray, list],
-    ) -> pl.DataFrame:
+def bin_column(
+    df_: pl.DataFrame,
+    col_name: str,
+    bin_col_name: str,
+    edges: Union[np.ndarray, list],
+) -> pl.DataFrame:
     """
     Bins the values in the specified column of a Polars DataFrame according to the given edges.
 
     Parameters:
     df_ (pl.DataFrame): The Polars DataFrame containing the column to bin.
     col_name (str): The name of the column to bin.
     bin_col_name (str): The name to give the new column containing the bin labels.
@@ -49,64 +51,58 @@
                         the value, and whose right edge is the smallest edge
                         greater than the value.
 
     Returns:
     pl.DataFrame: A new Polars DataFrame with an additional column containing the bin labels.
     """
     return df_.with_columns(
-        cut(
-            col_name=col_name,
-            edges = edges
-        ).alias(bin_col_name).cast(df_[col_name].dtype)
+        cut(col_name=col_name, edges=edges).alias(bin_col_name).cast(df_[col_name].dtype)
     )
 
-def add_ws(df_: pl.DataFrame,
-           ws_cols: List[str],
-           remove_all_nulls: bool=False
-    ) -> pl.DataFrame:
+
+def add_ws(df_: pl.DataFrame, ws_cols: List[str], remove_all_nulls: bool = False) -> pl.DataFrame:
     """
     Add the ws column to a dataframe, given which columns to average over
-    
+
 
     Parameters:
     df_ (pl.DataFrame): The Polars DataFrame containing the column to bin.
     ws_cols (list(str)): The name of the columns to average across.
     remove_all_nulls: (bool): Remove all null values in ws_cols (rather than any)
 
     Returns:
     pl.DataFrame: A new Polars DataFrame with an additional ws column
     """
 
-
-    df_with_mean_ws =  (
+    df_with_mean_ws = (
         # df_.select(pl.exclude('ws_bin')) # In case ws_bin already exists
         df_.with_columns(
             # df_.select(ws_cols).mean(axis=1).alias('ws_bin')
-            ws = pl.concat_list(ws_cols).list.mean() # Initially ws_bin is just the mean
+            ws=pl.concat_list(ws_cols).list.mean()  # Initially ws_bin is just the mean
         )
         .filter(
-            pl.all_horizontal(pl.col(ws_cols).is_not_null()) if remove_all_nulls else
-            pl.any_horizontal(pl.col(ws_cols).is_not_null())
-        ) 
-
-        .filter(
-            (pl.col('ws').is_not_null())
+            pl.all_horizontal(pl.col(ws_cols).is_not_null())
+            if remove_all_nulls
+            else pl.any_horizontal(pl.col(ws_cols).is_not_null())
         )
+        .filter((pl.col("ws").is_not_null()))
     )
 
     return df_with_mean_ws
-    
-def add_ws_bin(df_: pl.DataFrame,
-               ws_cols: List[str],
-               ws_step: float=1.0, 
-               ws_min: float=-0.5,
-               ws_max: float=50.0, 
-               edges: Optional[Union[np.ndarray, list]]=None,
-               remove_all_nulls: bool=False
-    ) -> pl.DataFrame:
+
+
+def add_ws_bin(
+    df_: pl.DataFrame,
+    ws_cols: List[str],
+    ws_step: float = 1.0,
+    ws_min: float = -0.5,
+    ws_max: float = 50.0,
+    edges: Optional[Union[np.ndarray, list]] = None,
+    remove_all_nulls: bool = False,
+) -> pl.DataFrame:
     """
     Add the ws_bin column to a dataframe, given which columns to average over
     and the step sizes to use
 
     Parameters:
     df_ (pl.DataFrame): The Polars DataFrame containing the column to bin.
     ws_cols (list(str)): The name of the columns to average across.
@@ -121,101 +117,99 @@
     remove_all_nulls: (bool): Remove all null values in ws_cols (rather than any)
 
     Returns:
     pl.DataFrame: A new Polars DataFrame with an additional ws_bin column
     """
 
     if edges is None:
-        edges = np.arange(ws_min, ws_max+ws_step,ws_step)
-    
+        edges = np.arange(ws_min, ws_max + ws_step, ws_step)
+
     # Check if edges is a list or numpy array or similar
     elif len(edges) < 2:
         raise ValueError("edges must have length of at least 2")
 
     df_with_mean_ws = add_ws(df_, ws_cols, remove_all_nulls)
 
     # Filter to min and max
     df_with_mean_ws = df_with_mean_ws.filter(
-        (pl.col('ws') >= ws_min) &  # Filter the mean wind speed
-        (pl.col('ws') < ws_max)
+        (pl.col("ws") >= ws_min)  # Filter the mean wind speed
+        & (pl.col("ws") < ws_max)
     )
 
-    return bin_column(df_with_mean_ws, 'ws', 'ws_bin', edges)
+    return bin_column(df_with_mean_ws, "ws", "ws_bin", edges)
 
-def add_wd(df_:pl.DataFrame,
-          wd_cols: List[str],
-          remove_all_nulls: bool=False
-    ) -> pl.DataFrame:
+
+def add_wd(df_: pl.DataFrame, wd_cols: List[str], remove_all_nulls: bool = False) -> pl.DataFrame:
     """
     Add the wd column to a dataframe, given which columns to average over
-    
+
 
     Parameters:
     df_ (pl.DataFrame): The Polars DataFrame containing the column to bin.
     wd_cols (list(str)): The name of the columns to average across.
     remove_all_nulls: (bool): Remove all null values in wd_cols (rather than any)
 
     Returns:
     pl.DataFrame: A new Polars DataFrame with an additional wd column
     """
 
-    
     # Gather up intermediate column names and final column names
-    wd_cols_cos = [c + '_cos' for c in wd_cols]
-    wd_cols_sin = [c + '_sin' for c in wd_cols]
+    wd_cols_cos = [c + "_cos" for c in wd_cols]
+    wd_cols_sin = [c + "_sin" for c in wd_cols]
     cols_to_return = df_.columns
-    if 'wd' not in cols_to_return:
-        cols_to_return = cols_to_return + ['wd']
-    
+    if "wd" not in cols_to_return:
+        cols_to_return = cols_to_return + ["wd"]
 
-    df_with_mean_wd =  (
+    df_with_mean_wd = (
         # df_.select(pl.exclude('wd_bin')) # In case wd_bin already exists
         df_.filter(
-            pl.all_horizontal(pl.col(wd_cols).is_not_null()) if remove_all_nulls else
-            pl.any_horizontal(pl.col(wd_cols).is_not_null())
-        ) 
+            pl.all_horizontal(pl.col(wd_cols).is_not_null())
+            if remove_all_nulls
+            else pl.any_horizontal(pl.col(wd_cols).is_not_null())
+        )
         # Add the cosine columns
         .with_columns(
-        [
-            pl.col(wd_cols).mul(np.pi/180).cos().suffix('_cos'),
-            pl.col(wd_cols).mul(np.pi/180).sin().suffix('_sin'),
-        ]
+            [
+                pl.col(wd_cols).mul(np.pi / 180).cos().suffix("_cos"),
+                pl.col(wd_cols).mul(np.pi / 180).sin().suffix("_sin"),
+            ]
         )
     )
     df_with_mean_wd = (
-        df_with_mean_wd
-        .with_columns(
-        [
-            # df_with_mean_wd.select(wd_cols_cos).mean(axis=1).alias('cos_mean'),
-            # df_with_mean_wd.select(wd_cols_sin).mean(axis=1).alias('sin_mean'),
-            pl.concat_list(wd_cols_cos).list.mean().alias('cos_mean'),
-            pl.concat_list(wd_cols_sin).list.mean().alias('sin_mean'),
-        ]
+        df_with_mean_wd.with_columns(
+            [
+                # df_with_mean_wd.select(wd_cols_cos).mean(axis=1).alias('cos_mean'),
+                # df_with_mean_wd.select(wd_cols_sin).mean(axis=1).alias('sin_mean'),
+                pl.concat_list(wd_cols_cos).list.mean().alias("cos_mean"),
+                pl.concat_list(wd_cols_sin).list.mean().alias("sin_mean"),
+            ]
         )
         .with_columns(
-            wd = np.mod(pl.reduce(np.arctan2, [pl.col('sin_mean'), pl.col('cos_mean')])
-                            .mul(180/np.pi), 360.0)
+            wd=np.mod(
+                pl.reduce(np.arctan2, [pl.col("sin_mean"), pl.col("cos_mean")]).mul(180 / np.pi),
+                360.0,
+            )
         )
-        .filter(
-            (pl.col('wd').is_not_null())
-        )
-        .select(cols_to_return) # Select for just the columns we want to return
+        .filter((pl.col("wd").is_not_null()))
+        .select(cols_to_return)  # Select for just the columns we want to return
     )
 
     return df_with_mean_wd
 
-# (df_, wd_cols, wd_step=2.0, wd_min=0.0, wd_max=360.0, edges=None):@# 
-def add_wd_bin(df_: pl.DataFrame,
-                wd_cols: List[str],
-                wd_step: float=2.0,
-                wd_min: float=0.0,
-                wd_max: float=360.0,
-                edges: Optional[Union[np.ndarray, list]]=None,
-                remove_all_nulls: bool=False
-    ):
+
+# (df_, wd_cols, wd_step=2.0, wd_min=0.0, wd_max=360.0, edges=None):@#
+def add_wd_bin(
+    df_: pl.DataFrame,
+    wd_cols: List[str],
+    wd_step: float = 2.0,
+    wd_min: float = 0.0,
+    wd_max: float = 360.0,
+    edges: Optional[Union[np.ndarray, list]] = None,
+    remove_all_nulls: bool = False,
+):
     """
     Add the wd_bin column to a dataframe, given which columns to average over
     and the step sizes to use
 
     Parameters:
     df_ (pl.DataFrame): The Polars DataFrame containing the column to bin.
     wd_cols (list(str)): The name of the columns to average across.
@@ -231,100 +225,98 @@
 
     Returns:
     pl.DataFrame: A new Polars DataFrame with an additional ws_bin column
     """
 
     if edges is None:
         edges = np.arange(wd_min, wd_max + wd_step, wd_step)
-    
+
     # If not none, edges must have lenght of at least 2
     elif len(edges) < 2:
         raise ValueError("edges must have length of at least 2")
-    
-    
 
     # Add in the mean wd column
     df_with_mean_wd = add_wd(df_, wd_cols, remove_all_nulls)
 
     # Filter to min and max
     df_with_mean_wd = df_with_mean_wd.filter(
-        (pl.col('wd') >= wd_min) &  # Filter the mean wind speed
-        (pl.col('wd') < wd_max)
+        (pl.col("wd") >= wd_min)  # Filter the mean wind speed
+        & (pl.col("wd") < wd_max)
     )
 
-    return bin_column(df_with_mean_wd, 'wd', 'wd_bin', edges)
+    return bin_column(df_with_mean_wd, "wd", "wd_bin", edges)
 
 
-def add_power_test(df_: pl.DataFrame,
-                     test_cols: List[str],
-    ) -> pl.DataFrame:
-
-    return df_.with_columns(
-        pow_test = pl.concat_list(test_cols).list.mean()
-    )
+def add_power_test(
+    df_: pl.DataFrame,
+    test_cols: List[str],
+) -> pl.DataFrame:
+    return df_.with_columns(pow_test=pl.concat_list(test_cols).list.mean())
 
 
-def add_power_ref(df_: pl.DataFrame,
-                   ref_cols: List[str]):
+def add_power_ref(df_: pl.DataFrame, ref_cols: List[str]):
+    return df_.with_columns(pow_ref=pl.concat_list(ref_cols).list.mean())
 
-    return df_.with_columns(
-        pow_ref = pl.concat_list(ref_cols).list.mean()
-    )
 
+def add_reflected_rows(df_: pl.DataFrame, edges: Union[np.ndarray, list], overlap_distance: float):
+    """
+    Adds rows to a datrame with where the wind direction is
+    reflected around the neearest edge if within overlap_distance
 
-def add_reflected_rows(df_: pl.DataFrame,
-                       edges: Union[np.ndarray, list], 
-                       overlap_distance: float):
-    """
-    Adds rows to a datrame with where the wind direction is reflected around the neearest edge if within overlap_distance
-
-    Given a wind direction DataFrame `df_`, this function adds reflected rows to the DataFrame such that each wind direction
-    in the original DataFrame has a corresponding reflected wind direction. The reflected wind direction is calculated by
-    subtracting the wind direction from the nearest edge in `edges` and then subtracting that difference again from the
-    original wind direction. The resulting wind direction is then wrapped around to the range [0, 360) degrees. The function
+    Given a wind direction DataFrame `df_`, this function adds
+    reflected rows to the DataFrame such that each wind direction
+    in the original DataFrame has a corresponding reflected wind
+    direction. The reflected wind direction is calculated by
+    subtracting the wind direction from the nearest edge in `edges`
+    and then subtracting that difference again from the
+    original wind direction. The resulting wind direction
+    is then wrapped around to the range [0, 360) degrees. The function
     returns a new DataFrame with the original rows and the added reflected rows.
 
     This function enables overlapping bins in the energy ratio functions
 
     Parameters
     ----------
     df_ : polars.DataFrame
         The DataFrame to add reflected rows to.
     edges : numpy.ndarray
-        An array of wind direction edges to use for reflection.  (Should be same as used in energy ratio)
+        An array of wind direction edges to use for reflection.
+        (Should be same as used in energy ratio)
     overlap_distance : float
-        The maximum distance between a wind direction and an edge for the wind direction to be considered overlapping.
+        The maximum distance between a wind direction and an edge
+        for the wind direction to be considered overlapping.
 
     Returns
     -------
     polars.DataFrame
         A new DataFrame with the original rows and the added reflected rows.
     """
 
     df_add = df_.clone()
-    wd = df_add['wd'].to_numpy()
-    diff_matrix = wd[:,None] - edges
+    wd = df_add["wd"].to_numpy()
+    diff_matrix = wd[:, None] - edges
     abs_diff_matrix = np.abs(diff_matrix)
     idx = np.argmin(abs_diff_matrix, axis=1)
     signed_mins = diff_matrix[np.arange(len(diff_matrix)), idx]
-    df_add = (df_add.with_columns(pl.Series(name='distances',values=signed_mins,dtype=pl.Float32))
-        .filter(pl.col('distances').abs() < overlap_distance)
-        .with_columns(np.mod((pl.col('wd') - pl.col('distances') * 2),360.0))
-        .drop('distances')
-        )
-    
+    df_add = (
+        df_add.with_columns(pl.Series(name="distances", values=signed_mins, dtype=pl.Float32))
+        .filter(pl.col("distances").abs() < overlap_distance)
+        .with_columns(np.mod((pl.col("wd") - pl.col("distances") * 2), 360.0))
+        .drop("distances")
+    )
 
     return pl.concat([df_, df_add])
 
+
 def filter_all_nulls(
-    df_: pl.DataFrame, 
+    df_: pl.DataFrame,
     ref_cols: List[str],
     test_cols: List[str],
     ws_cols: List[str],
-    wd_cols: List[str]
+    wd_cols: List[str],
 ):
     """
     Filter data by requiring ALL values of ref, test, ws, and wd to be valid
     numbers.
 
     Args:
         df_ (pl.DataFrame): Polars dataframe possibly containing Null values
@@ -333,24 +325,25 @@
         wd_cols (list[str]): A list of columns to derive the wind directions from
         ws_cols (list[str]): A list of columns to derive the wind speeds from
 
     Returns:
         pl.DataFrame: A dataframe containing the energy ratio between the two sets of turbines.
 
     """
-    return df_.filter(pl.all_horizontal(
-        pl.col(ref_cols + test_cols + ws_cols + wd_cols).is_not_null()
-    ))
+    return df_.filter(
+        pl.all_horizontal(pl.col(ref_cols + test_cols + ws_cols + wd_cols).is_not_null())
+    )
+
 
 def filter_any_nulls(
-    df_: pl.DataFrame, 
+    df_: pl.DataFrame,
     ref_cols: List[str],
     test_cols: List[str],
     ws_cols: List[str],
-    wd_cols: List[str]
+    wd_cols: List[str],
 ):
     """
     Filter data by requiring ANY of ref, ANY of test, ANY of ws, and ANY of wd
     to be a valid number.
 
     Args:
         df_ (pl.DataFrame): Polars dataframe possibly containing Null values
@@ -359,20 +352,22 @@
         wd_cols (list[str]): A list of columns to derive the wind directions from
         ws_cols (list[str]): A list of columns to derive the wind speeds from
 
     Returns:
         pl.DataFrame: A dataframe containing the energy ratio between the two sets of turbines.
 
     """
-    return (df_.filter(pl.any_horizontal(pl.col(ref_cols).is_not_null()))
-            .filter(pl.any_horizontal(pl.col(test_cols).is_not_null()))
-            .filter(pl.any_horizontal(pl.col(ws_cols).is_not_null()))
-            .filter(pl.any_horizontal(pl.col(wd_cols).is_not_null()))
+    return (
+        df_.filter(pl.any_horizontal(pl.col(ref_cols).is_not_null()))
+        .filter(pl.any_horizontal(pl.col(test_cols).is_not_null()))
+        .filter(pl.any_horizontal(pl.col(ws_cols).is_not_null()))
+        .filter(pl.any_horizontal(pl.col(wd_cols).is_not_null()))
     )
 
+
 def check_compute_energy_ratio_inputs(
     df_,
     ref_turbines,
     test_turbines,
     wd_turbines,
     ws_turbines,
     use_predefined_ref,
@@ -389,131 +384,140 @@
     df_freq,
     wd_bin_overlap_radius,
     uplift_pairs,
     uplift_names,
     uplift_absolute,
     N,
     percentiles,
-    remove_all_nulls
+    remove_all_nulls,
 ):
     """
     Check inputs to compute_energy_ratio. Inputs reflect inputs to compute_energy_ratio,
     with exception of df_, which is passed directly instead of er_in.
     """
 
     # Check that the inputs are valid
     # If use_predefined_ref is True, df_ must have a column named 'pow_ref'
     if use_predefined_ref:
-        if 'pow_ref' not in df_.columns:
-            raise ValueError('df_ must have a column named pow_ref when use_predefined_ref is True')
+        if "pow_ref" not in df_.columns:
+            raise ValueError("df_ must have a column named pow_ref when use_predefined_ref is True")
         # If ref_turbines supplied, warn user that it will be ignored
         if ref_turbines is not None:
-            warnings.warn('ref_turbines will be ignored when use_predefined_ref is True')
+            warnings.warn("ref_turbines will be ignored when use_predefined_ref is True")
     else:
         # ref_turbine must be supplied
         if ref_turbines is None:
-            raise ValueError('ref_turbines must be supplied when use_predefined_ref is False')
-        
+            raise ValueError("ref_turbines must be supplied when use_predefined_ref is False")
+
     # If use_predefined_ws is True, df_ must have a column named 'ws'
     if use_predefined_ws:
-        if 'ws' not in df_.columns:
-            raise ValueError('df_ must have a column named ws when use_predefined_ws is True')
+        if "ws" not in df_.columns:
+            raise ValueError("df_ must have a column named ws when use_predefined_ws is True")
         # If ws_turbines supplied, warn user that it will be ignored
         if ws_turbines is not None:
-            warnings.warn('ws_turbines will be ignored when use_predefined_ws is True')
+            warnings.warn("ws_turbines will be ignored when use_predefined_ws is True")
     else:
         # ws_turbine must be supplied
         if ws_turbines is None:
-            raise ValueError('ws_turbines must be supplied when use_predefined_ws is False')
+            raise ValueError("ws_turbines must be supplied when use_predefined_ws is False")
 
     # If use_predefined_wd is True, df_ must have a column named 'wd'
     if use_predefined_wd:
-        if 'wd' not in df_.columns:
-            raise ValueError('df_ must have a column named wd when use_predefined_wd is True')
+        if "wd" not in df_.columns:
+            raise ValueError("df_ must have a column named wd when use_predefined_wd is True")
         # If wd_turbines supplied, warn user that it will be ignored
         if wd_turbines is not None:
-            warnings.warn('wd_turbines will be ignored when use_predefined_wd is True')
+            warnings.warn("wd_turbines will be ignored when use_predefined_wd is True")
     else:
         # wd_turbine must be supplied
         if wd_turbines is None:
-            raise ValueError('wd_turbines must be supplied when use_predefined_wd is False')
-        
+            raise ValueError("wd_turbines must be supplied when use_predefined_wd is False")
 
     # Confirm that test_turbines is a list of ints or a numpy array of ints
     if not isinstance(test_turbines, list) and not isinstance(test_turbines, np.ndarray):
-        raise ValueError('test_turbines must be a list or numpy array of ints')
+        raise ValueError("test_turbines must be a list or numpy array of ints")
 
-    # Confirm that test_turbines is not empty  
+    # Confirm that test_turbines is not empty
     if len(test_turbines) == 0:
-        raise ValueError('test_turbines cannot be empty')
-    
+        raise ValueError("test_turbines cannot be empty")
+
     # Confirm that wd_bin_overlap_radius is less than or equal to wd_step/2
-    if wd_bin_overlap_radius > wd_step/2:
-        raise ValueError('wd_bin_overlap_radius must be less than or equal to wd_step/2')
-    
+    if wd_bin_overlap_radius > wd_step / 2:
+        raise ValueError("wd_bin_overlap_radius must be less than or equal to wd_step/2")
+
     # Confirm the weight_by argument is valid
-    if weight_by not in ['min', 'sum']:
+    if weight_by not in ["min", "sum"]:
         raise ValueError('weight_by must be one of "min", or "sum"')
-    
+
     # Confirm df_freq contains ws, wd and freq_val
     if df_freq is not None:
-        if ('ws' not in df_freq.columns) or ('wd' not in df_freq.columns) or  ('freq_val' not in df_freq.columns):
-            raise ValueError('df_freq must have columns ws, wd and freq_val')
+        if (
+            ("ws" not in df_freq.columns)
+            or ("wd" not in df_freq.columns)
+            or ("freq_val" not in df_freq.columns)
+        ):
+            raise ValueError("df_freq must have columns ws, wd and freq_val")
 
     return None
 
-def bin_and_group_dataframe(df_: pl.DataFrame,
+
+def bin_and_group_dataframe(
+    df_: pl.DataFrame,
     ref_cols: List,
     test_cols: List,
     wd_cols: List,
     ws_cols: List,
     wd_step: float = 2.0,
-    wd_min: float  = 0.0,
+    wd_min: float = 0.0,
     wd_max: float = 360.0,
     ws_step: float = 1.0,
     ws_min: float = 0.0,
     ws_max: float = 50.0,
-    wd_bin_overlap_radius: float = 0.,
+    wd_bin_overlap_radius: float = 0.0,
     remove_all_nulls: bool = False,
     bin_cols_without_df_name: List = None,
     num_df: int = 0,
 ):
-    
     """
     Bin and aggregate a DataFrame based on wind direction and wind speed parameters.
 
-    This function takes a Polars DataFrame (df_) and performs binning and aggregation operations based on
-    wind direction (wd) and wind speed (ws). It allows for optional handling of reflected rows and grouping by
-    specific columns. The resulting DataFrame contains aggregated statistics for reference and test power
+    This function takes a Polars DataFrame (df_) and performs
+    binning and aggregation operations based on
+    wind direction (wd) and wind speed (ws). It allows for optional
+    handling of reflected rows and grouping by
+    specific columns. The resulting DataFrame contains aggregated
+    statistics for reference and test power
     columns within specified bins.
 
     Args:
         df_ (DataFrame): The input Polars DataFrame to be processed.
         ref_cols (List[str]): List of columns containing reference power data.
         test_cols (List[str]): List of columns containing test power data.
         wd_cols (List[str]): List of columns containing wind direction data.
         ws_cols (List[str]): List of columns containing wind speed data.
         wd_step (float, optional): Step size for wind direction binning. Defaults to 2.0.
         wd_min (float, optional): Minimum wind direction value. Defaults to 0.0.
         wd_max (float, optional): Maximum wind direction value. Defaults to 360.0.
         ws_step (float, optional): Step size for wind speed binning. Defaults to 1.0.
         ws_min (float, optional): Minimum wind speed value. Defaults to 0.0.
         ws_max (float, optional): Maximum wind speed value. Defaults to 50.0.
-        wd_bin_overlap_radius (float, optional): Radius for overlapping wind direction bins. Defaults to 0.0.
-        remove_all_nulls (bool, optional): If True, remove rows unless all valid instead of any Defaults to False.
-        bin_cols_without_df_name (List[str], optional): List of columns used for grouping without 'df_name'.
+        wd_bin_overlap_radius (float, optional): Radius for overlapping wind direction bins.
+             Defaults to 0.0.
+        remove_all_nulls (bool, optional): If True, remove rows unless all valid instead of any.
+            Defaults to False.
+        bin_cols_without_df_name (List[str], optional): List of columns used
+            for grouping without 'df_name'.
         num_df (int, optional): Number of dataframes required for each bin combination.
 
     Returns:
         DataFrame: The resulting Polars DataFrame with aggregated statistics.
     """
 
-        # If wd_bin_overlap_radius is not zero, add reflected rows
-    if wd_bin_overlap_radius > 0.:
-
+    # If wd_bin_overlap_radius is not zero, add reflected rows
+    if wd_bin_overlap_radius > 0.0:
         # Need to obtain the wd column now rather than during binning
         df_ = add_wd(df_, wd_cols, remove_all_nulls)
 
         # Add reflected rows
         edges = np.arange(wd_min, wd_max + wd_step, wd_step)
         df_ = add_reflected_rows(df_, edges, wd_bin_overlap_radius)
 
@@ -521,77 +525,84 @@
     df_ = add_ws_bin(df_, ws_cols, ws_step, ws_min, ws_max, remove_all_nulls=remove_all_nulls)
     df_ = add_wd_bin(df_, wd_cols, wd_step, wd_min, wd_max, remove_all_nulls=remove_all_nulls)
 
     # Assign the reference and test power columns
     df_ = add_power_ref(df_, ref_cols)
     df_ = add_power_test(df_, test_cols)
 
-    bin_cols_with_df_name = bin_cols_without_df_name + ['df_name']
+    bin_cols_with_df_name = bin_cols_without_df_name + ["df_name"]
 
     # Group df_
-    df_ = (df_
-        .filter(pl.all_horizontal(pl.col(bin_cols_with_df_name).is_not_null())) # Select for all bin cols present
+    df_ = (
+        df_.filter(
+            pl.all_horizontal(pl.col(bin_cols_with_df_name).is_not_null())
+        )  # Select for all bin cols present
         .group_by(bin_cols_with_df_name, maintain_order=True)
-        .agg([pl.mean("pow_ref"), pl.mean("pow_test"),pl.count()])
+        .agg([pl.mean("pow_ref"), pl.mean("pow_test"), pl.count()])
         # Enforce that each ws/wd bin combination has to appear in all dataframes
         .filter(pl.count().over(bin_cols_without_df_name) == num_df)
     )
 
     return df_
 
-def add_bin_weights(df_: pl.DataFrame, 
+
+def add_bin_weights(
+    df_: pl.DataFrame,
     df_freq_pl: pl.DataFrame = None,
-    bin_cols_without_df_name: List =None,
-    weight_by: str = "min"
+    bin_cols_without_df_name: List = None,
+    weight_by: str = "min",
 ):
     """
-    Add weights to DataFrame bins based on either frequency counts or the provided frequency table df_freq_pl.
+    Add weights to DataFrame bins based on either frequency counts or
+    the provided frequency table df_freq_pl.
 
-    This function  assigns weights to DataFrame bins.  If 'df_freq_pl' is provided, these weights are used
-    directly.  If 'df_freq_pl' is not provided, the function calculates the weights from the input DataFrame 'df_'.
+    This function  assigns weights to DataFrame bins.  If 'df_freq_pl' is provided,
+    these weights are used directly.  If 'df_freq_pl' is not provided, the function
+    calculates the weights from the input DataFrame 'df_'.
     Weights can be determined as either the minimum ('min') or the sum ('sum') of counts.
 
     Args:
         df_ (DataFrame): The input Polars DataFrame containing bins and frequency counts.
         df_freq_pl (DataFrame, optional): A Polars DataFrame containing frequency counts for bins.
             If not provided, the function will calculate these counts from 'df_'.
-        bin_cols_without_df_name (List, optional): List of columns used for grouping bins without 'df_name'.
-        weight_by (str, optional): Weight calculation method, either 'min' (minimum count) or 'sum' (sum of counts).
+        bin_cols_without_df_name (List, optional): List of columns used for grouping
+            bins without 'df_name'.
+        weight_by (str, optional): Weight calculation method, either 'min'
+            (minimum count) or 'sum' (sum of counts).
             Defaults to 'min'.
 
     Returns:
-        Tuple[pl.DataFrame, pl.DataFrame]: A tuple containing the modified DataFrame 'df_' with added weights and the DataFrame
+        Tuple[pl.DataFrame, pl.DataFrame]: A tuple containing the modified DataFrame 'df_'
+            with added weights and the DataFrame
     'df_freq_pl' with the calculated frequency counts.
 
     Raises:
         RuntimeError: If none of the ws/wd bins in data appear in df_freq.
         UserWarning: If some bins in data are not in df_freq and will receive a weight of 0.
 
     """
     if df_freq_pl is None:
         # Determine the weights per bin as either the min or sum count
-        df_freq_pl = (df_
-            .select(bin_cols_without_df_name+['count'])
+        df_freq_pl = (
+            df_.select(bin_cols_without_df_name + ["count"])
             .group_by(bin_cols_without_df_name)
-            .agg([pl.min('count') if weight_by == 'min' else pl.sum('count')])
-            .rename({'count':'weight'})
+            .agg([pl.min("count") if weight_by == "min" else pl.sum("count")])
+            .rename({"count": "weight"})
         )
-    
-    df_ = (df_.join(df_freq_pl, on=['wd_bin','ws_bin'], how='left')
-            .with_columns(pl.col('weight'))
-    )
+
+    df_ = df_.join(df_freq_pl, on=["wd_bin", "ws_bin"], how="left").with_columns(pl.col("weight"))
 
     # Check if all the values in the weight column are null
-    if df_['weight'].is_null().all():
+    if df_["weight"].is_null().all():
         raise RuntimeError("None of the ws/wd bins in data appear in df_freq")
-    
+
     # Check if any of the values in the weight column are null
-    if df_['weight'].is_null().any():
-        warnings.warn('Some bins in data are not in df_freq and will get 0 weight')
+    if df_["weight"].is_null().any():
+        warnings.warn("Some bins in data are not in df_freq and will get 0 weight")
 
     # Fill the null values with zeros
-    df_= df_.with_columns(pl.col('weight').fill_null(strategy="zero"))
+    df_ = df_.with_columns(pl.col("weight").fill_null(strategy="zero"))
 
     # Normalize the weights
-    df_ = df_.with_columns(pl.col('weight').truediv(pl.col('weight').sum()))
+    df_ = df_.with_columns(pl.col("weight").truediv(pl.col("weight").sum()))
 
-    return df_, df_freq_pl
+    return df_, df_freq_pl
```

### Comparing `flasc-1.4.2/flasc/energy_ratio/energy_ratio_wd_bias_estimation.py` & `flasc-2.0/flasc/data_processing/energy_ratio_wd_bias_estimation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,70 +1,56 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
+import os as os
+from typing import Callable, List
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import os as os
-from scipy import optimize as opt
-from scipy import stats as spst
-
-from typing import Optional, Dict, List, Any, Tuple, Union, Callable
-
 from floris.utilities import wrap_360
+from scipy import optimize as opt, stats as spst
 
-from flasc.dataframe_operations import dataframe_manipulations as dfm
-from flasc import floris_tools as ftools
-from flasc.utilities import printnow as print
-from flasc.energy_ratio import energy_ratio as er
-from flasc.energy_ratio.energy_ratio_input import EnergyRatioInput
+from flasc.analysis import energy_ratio as er
+from flasc.analysis.energy_ratio_input import EnergyRatioInput
+from flasc.data_processing import dataframe_manipulations as dfm
+from flasc.logging_manager import LoggingManager
+from flasc.utilities import floris_tools as ftools
 
 
-class bias_estimation():
+class bias_estimation(LoggingManager):
     """This class can be used to estimate the bias (offset) in a wind
     direction measurement by comparing the energy ratios in the SCADA
     data with the predicted energy ratios from FLORIS under various
     bias correction values. Essentially, this class solves the following
     optimization problem: the argument in this optimization problem
     is the offset on the wind direction measurement and the cost is the
     Pearson correlation coefficient between two lines, namely
     1) the energy ratios of the SCADA data, and 2) the predicted energy
     ratios for the same data by FLORIS under the offset-corrected wind
     direction.
     """
+
     def __init__(
         self,
         df: pd.DataFrame,
-        df_fi_approx: pd.DataFrame,
+        df_fm_approx: pd.DataFrame,
         test_turbines_subset: List[int],
         df_ws_mapping_func: Callable,
-        df_pow_ref_mapping_func: Callable
+        df_pow_ref_mapping_func: Callable,
     ):
         """Initialize the bias estimation class.
 
         Args:
             df ([pd.DataFrame]): Dataframe with the SCADA data measurements
                 formatted in the generic format. The dataframe should contain
                 at the minimum the following columns:
                 * Reference wind direction for the test turbine, 'wd'
                 * Reference wind speed for the test turbine, 'ws'
                 * Power production of every turbine: pow_000, pow_001, ...
                 * Reference power production used to normalize the energy
                     ratio: 'pow_ref'
-            df_fi_approx ([pd.DataFrame]): Dataframe containing a large set
+            df_fm_approx ([pd.DataFrame]): Dataframe containing a large set
                 of precomputed solutions of the FLORIS model for a range of
                 wind directions, wind speeds (and optionally turbulence
                 intensities). This table can be generated using the following:
                     from flasc import floris_tools as ftls
                     df_approx = ftls.calc_floris_approx_table(...)
             test_turbines_subset ([iteratible]): List of test turbines for
                 which each the energy ratios are calculated and the Pearson
@@ -78,34 +64,34 @@
             df_ws_mapping_func ([function]): This is a function that
                 returns the reference wind speed based on an array of wind
                 directions as input.
             df_pow_ref_mapping_func ([function]): This is a function that
                 returns the reference power production based on an array of
                 wind directions as input.
         """
-        print('Initializing a bias_estimation() object...')
+        self.logger.info("Initializing a bias_estimation() object...")
 
         # Import inputs
-        self.df = df.reset_index(drop=('time' in df.columns))
+        self.df = df.reset_index(drop=("time" in df.columns))
         self.n_turbines = dfm.get_num_turbines(self.df)
-        self.df_fi_approx = df_fi_approx
+        self.df_fm_approx = df_fm_approx
         self.df_ws_mapping_func = df_ws_mapping_func
         self.df_pow_ref_mapping_func = df_pow_ref_mapping_func
         self.test_turbines = test_turbines_subset
 
     # Private methods
 
     def _load_er_input_for_wd_bias(
         self,
         wd_bias,
     ):
-        """This function initializes an instance of the EnergyRatioInput 
-        where the dataframe is shifted by wd_bias for each test turbine. 
-        This facilitates the calculation of the energy ratios under this 
-        hypothesized wind direction bias. Additionally, the FLORIS predictions 
+        """This function initializes an instance of the EnergyRatioInput
+        where the dataframe is shifted by wd_bias for each test turbine.
+        This facilitates the calculation of the energy ratios under this
+        hypothesized wind direction bias. Additionally, the FLORIS predictions
         for the shifted dataset are calculated and the energy ratios for the FLORIS
         predictions are also calculated.
 
         Args:
             wd_bias ([float]): Hypothesized wind direction bias in degrees.
             test_turbines ([iteratible]): List of test turbines for
                 which each the energy ratios are calculated and the Pearson
@@ -116,59 +102,50 @@
 
         Returns:
             et ([polars dataframe]): The energy ratio table
                 object in which the inserted dataframe has a shifted
                 wind direction measurement, offset by 'wd_bias' compared
                 to the nominal dataset.
         """
-        print('  Constructing energy table for wd_bias of %.2f deg.'
-              % wd_bias)
+        self.logger.info("  Constructing energy table for wd_bias of %.2f deg." % wd_bias)
 
         er_in_test_turbine_list_scada = []
         er_in_test_turbine_list_floris = []
 
         # Derive dataframe that covers all test_turbines
         df_cor_all = self.df.copy()
-        df_cor_all['wd'] = wrap_360(df_cor_all['wd'] - wd_bias)
+        df_cor_all["wd"] = wrap_360(df_cor_all["wd"] - wd_bias)
 
         # Set columns 'ws' and 'pow_ref' for df_subset_cor
         df_cor_all = self.df_ws_mapping_func(df_cor_all)
         df_cor_all = self.df_pow_ref_mapping_func(df_cor_all)
-        df_cor_all = df_cor_all.dropna(subset=['wd', 'ws', 'pow_ref'])
+        df_cor_all = df_cor_all.dropna(subset=["wd", "ws", "pow_ref"])
         df_cor_all = df_cor_all.reset_index(drop=True)
 
         # Get FLORIS predictions
-        print('    Interpolating FLORIS predictions for dataframe.')
+        self.logger.info("    Interpolating FLORIS predictions for dataframe.")
         ws_cols = ["ws_{:03d}".format(ti) for ti in range(self.n_turbines)]
         pow_cols = ["pow_{:03d}".format(ti) for ti in range(self.n_turbines)]
-        df_fi_all = df_cor_all[['time', 'wd', 'ws', 'ti', *ws_cols, *pow_cols]].copy()
+        df_fm_all = df_cor_all[["time", "wd", "ws", "ti", *ws_cols, *pow_cols]].copy()
 
-        df_fi_all = ftools.interpolate_floris_from_df_approx(
-            df=df_fi_all,
-            df_approx=self.df_fi_approx,
-            verbose=False,
-            mirror_nans=True
+        df_fm_all = ftools.interpolate_floris_from_df_approx(
+            df=df_fm_all, df_approx=self.df_fm_approx, verbose=False, mirror_nans=True
         )
-        df_fi_all = self.df_pow_ref_mapping_func(df_fi_all)
+        df_fm_all = self.df_pow_ref_mapping_func(df_fm_all)
 
         for ti in self.test_turbines:
-            valid_entries = (
-                (~df_cor_all["pow_{:03d}".format(ti)].isna()) &
-                (~df_fi_all["pow_{:03d}".format(ti)].isna())
+            valid_entries = (~df_cor_all["pow_{:03d}".format(ti)].isna()) & (
+                ~df_fm_all["pow_{:03d}".format(ti)].isna()
             )
             df_cor = df_cor_all[valid_entries].copy().reset_index(drop=True)
-            df_fi = df_fi_all[valid_entries].copy().reset_index(drop=True)
+            df_fm = df_fm_all[valid_entries].copy().reset_index(drop=True)
 
             # Initialize SCADA analysis class and add dataframes
-            er_in_test_turbine_list_scada.append(
-                EnergyRatioInput([df_cor], ["Measured data"])
-            )
-            er_in_test_turbine_list_floris.append(
-                EnergyRatioInput([df_fi], ["FLORIS prediction"])
-            )
+            er_in_test_turbine_list_scada.append(EnergyRatioInput([df_cor], ["Measured data"]))
+            er_in_test_turbine_list_floris.append(EnergyRatioInput([df_fm], ["FLORIS prediction"]))
 
         # Save to self
         self.er_in_test_turbine_list_scada = er_in_test_turbine_list_scada
         self.er_in_test_turbine_list_floris = er_in_test_turbine_list_floris
 
     def _get_energy_ratios_allbins(
         self,
@@ -211,30 +188,33 @@
                 not plot or save any figures of iterations. Defaults to
                 None.
         """
         er_out_test_turbine_list_scada = []
         er_out_test_turbine_list_floris = []
 
         if time_mask is not None:
-            raise NotImplementedError("time_mask not available. Please preprocess "+\
-                "your dataset to apply time masks.")
+            raise NotImplementedError(
+                "time_mask not available. Please preprocess " + "your dataset to apply time masks."
+            )
         if ti_mask is not None:
-            raise NotImplementedError("ti_mask not available. Please preprocess "+\
-                "your dataset to apply turbulence intensity masks.")
+            raise NotImplementedError(
+                "ti_mask not available. Please preprocess "
+                + "your dataset to apply turbulence intensity masks."
+            )
         if wd_mask is None:
-            wd_mask = [0., 360.]
+            wd_mask = [0.0, 360.0]
 
-        print("    Initializing energy ratio inputs.")
-        self._load_er_input_for_wd_bias(
-            wd_bias=wd_bias
-        )
+        self.logger.info("    Initializing energy ratio inputs.")
+        self._load_er_input_for_wd_bias(wd_bias=wd_bias)
 
         for ii, ti in enumerate(self.test_turbines):
-            print('    Determining energy ratios for test turbine = %03d.'
-                  % (ti) + ' WD bias: %.3f deg.' % wd_bias)
+            self.logger.info(
+                "    Determining energy ratios for test turbine = %03d." % (ti)
+                + " WD bias: %.3f deg." % wd_bias
+            )
 
             er_out_test_turbine_list_scada.append(
                 er.compute_energy_ratio(
                     self.er_in_test_turbine_list_scada[ii],
                     ref_turbines=None,
                     test_turbines=[ti],
                     use_predefined_ref=True,
@@ -242,15 +222,15 @@
                     use_predefined_ws=True,
                     wd_step=wd_step,
                     wd_min=wd_mask[0],
                     wd_max=wd_mask[1],
                     ws_step=ws_step,
                     ws_min=ws_mask[0],
                     ws_max=ws_mask[1],
-                    wd_bin_overlap_radius=(wd_bin_width-wd_step)/2,
+                    wd_bin_overlap_radius=(wd_bin_width - wd_step) / 2,
                     N=N_btstrp,
                 )
             )
 
             er_out_test_turbine_list_floris.append(
                 er.compute_energy_ratio(
                     self.er_in_test_turbine_list_floris[ii],
@@ -261,28 +241,29 @@
                     use_predefined_ws=True,
                     wd_step=wd_step,
                     wd_min=wd_mask[0],
                     wd_max=wd_mask[1],
                     ws_step=ws_step,
                     ws_min=ws_mask[0],
                     ws_max=ws_mask[1],
-                    wd_bin_overlap_radius=(wd_bin_width-wd_step)/2,
+                    wd_bin_overlap_radius=(wd_bin_width - wd_step) / 2,
                     N=N_btstrp,
                 )
             )
 
         # Debugging: plot iteration to path
         if plot_iter_path is not None:
-            print('    Plotting energy ratios and saving figures')
+            self.logger.info("    Plotting energy ratios and saving figures")
             fp = os.path.join(
                 plot_iter_path,
                 "bias%+.3f" % (self.fsc_wd_bias_list[ii]),
-                "energy_ratios_test_turbine")
-            self.plot_energy_ratios(save_path=fp, format='png', dpi=200)
-            plt.close('all')
+                "energy_ratios_test_turbine",
+            )
+            self.plot_energy_ratios(save_path=fp, format="png", dpi=200)
+            plt.close("all")
 
         # Save to self
         self.er_out_test_turbine_list_scada = er_out_test_turbine_list_scada
         self.er_out_test_turbine_list_floris = er_out_test_turbine_list_floris
 
         return None
 
@@ -303,15 +284,15 @@
         self._get_energy_ratios_allbins(
             wd_bias=0.0,
             time_mask=time_mask,
             ws_mask=ws_mask,
             wd_mask=wd_mask,
             ti_mask=ti_mask,
             wd_step=er_wd_step,
-            ws_step=er_ws_step, 
+            ws_step=er_ws_step,
             wd_bin_width=er_wd_bin_width,
             N_btstrp=er_N_btstrp,
             fast=False,
         )
 
     def estimate_wd_bias(
         self,
@@ -379,82 +360,82 @@
                 not plot or save any figures of iterations. Defaults to
                 None.
 
         Returns:
             x_opt ([float]): Optimal wind direction offset.
             J_opt ([float]): Cost function under optimal offset.
         """
-        print('Estimating the wind direction bias')
+        self.logger.info("Estimating the wind direction bias")
 
         def cost_fun(wd_bias):
             self._get_energy_ratios_allbins(
                 wd_bias=wd_bias,
                 time_mask=time_mask,
                 ws_mask=ws_mask,
                 wd_mask=wd_mask,
                 ti_mask=ti_mask,
                 wd_step=er_wd_step,
                 ws_step=er_ws_step,
                 wd_bin_width=er_wd_bin_width,
                 N_btstrp=1,
-                plot_iter_path=plot_iter_path
+                plot_iter_path=plot_iter_path,
             )
 
             # Calculate cost
             cost_array = np.full(len(self.er_out_test_turbine_list_scada), np.nan)
             for ii, _ in enumerate(self.test_turbines):
-                y_scada = np.array(self.er_out_test_turbine_list_scada[ii].df_result["Measured data"])
-                y_floris = np.array(self.er_out_test_turbine_list_floris[ii].df_result["FLORIS prediction"])
+                y_scada = np.array(
+                    self.er_out_test_turbine_list_scada[ii].df_result["Measured data"]
+                )
+                y_floris = np.array(
+                    self.er_out_test_turbine_list_floris[ii].df_result["FLORIS prediction"]
+                )
                 ids = ~np.isnan(y_scada) & ~np.isnan(y_floris)
                 if np.sum(ids) > 5:  # At least 6 valid data entries
                     r, _ = spst.pearsonr(y_scada[ids], y_floris[ids])
                 else:
                     r = np.nan
-                cost_array[ii] = -1. * r
+                cost_array[ii] = -1.0 * r
 
             cost = np.nanmean(cost_array)
             return cost
 
-        opt_finish = (
-            lambda func, x0, args=(): opt.fmin(func, x0, args,
-                                               maxfun=10,
-                                               full_output=True,
-                                               xtol=0.1, disp=True)
-        )
+        def opt_finish(func, x0, args=()):
+            return opt.fmin(func, x0, args, maxfun=10, full_output=True, xtol=0.1, disp=True)
 
         dran = opt_search_range[1] - opt_search_range[0]
         x_opt, J_opt, x, J = opt.brute(
             func=cost_fun,
             ranges=[opt_search_range],
-            Ns=int(np.ceil(dran/opt_search_brute_dx) + 1),
+            Ns=int(np.ceil(dran / opt_search_brute_dx) + 1),
             full_output=True,
             disp=True,
             finish=opt_finish,
             # workers=opt_workers,
         )
 
         wd_bias = x_opt
         self.opt_wd_bias = wd_bias
         self.opt_cost = J_opt
         self.opt_wd_grid = x
         self.opt_wd_cost = J
 
         # End with optimal results and bootstrapping
-        print('  Evaluating optimal solution with bootstrapping')
+        self.logger.info("  Evaluating optimal solution with bootstrapping")
         self._get_energy_ratios_allbins(
             wd_bias=x_opt,
             time_mask=time_mask,
             ws_mask=ws_mask,
             wd_mask=wd_mask,
             ti_mask=ti_mask,
             wd_step=er_wd_step,
             ws_step=er_ws_step,
             wd_bin_width=er_wd_bin_width,
             N_btstrp=er_N_btstrp,
-            plot_iter_path=None
+            plot_iter_path=None,
         )
 
         # Save input arguments for future use
         self._input_args = {
             "time_mask": time_mask,
             "ws_mask": ws_mask,
             "wd_mask": wd_mask,
@@ -462,31 +443,27 @@
             "opt_search_range": opt_search_range,
             "opt_search_brute_dx": opt_search_brute_dx,
             "opt_workers": opt_workers,
             "er_wd_step": er_wd_step,
             "er_ws_step": er_ws_step,
             "er_wd_bin_width": er_wd_bin_width,
             "er_N_btstrp": er_N_btstrp,
-            "plot_iter_path" : plot_iter_path,
+            "plot_iter_path": plot_iter_path,
         }
 
         return x_opt, J_opt
 
     def plot_energy_ratios(
-        self,
-        show_uncorrected_data=False,
-        save_path=None,
-        format='png',
-        dpi=200
+        self, show_uncorrected_data=False, save_path=None, format="png", dpi=200
     ):
         """Plot the energy ratios for the currently evaluated wind
         direction offset term.
 
         Args:
-            show_uncorrcted_data (bool, optional): Compute and show the 
+            show_uncorrcted_data (bool, optional): Compute and show the
                 uncorrected energy ratio (with wd_bias=0) on the plot. Defaults
                 to False.
             save_path ([str], optional): Path to save the figure to. If not
                 specified, will not save the figure. Defaults to None.
             format (str, optional): Figure format. Defaults to 'png'.
             dpi (int, optional): Figure DPI. Defaults to 200.
         """
@@ -501,50 +478,49 @@
                 time_mask=self._input_args["time_mask"],
                 ws_mask=self._input_args["ws_mask"],
                 wd_mask=self._input_args["wd_mask"],
                 ti_mask=self._input_args["ti_mask"],
                 wd_step=self._input_args["er_wd_step"],
                 ws_step=self._input_args["er_ws_step"],
                 wd_bin_width=self._input_args["er_wd_bin_width"],
-                N_btstrp=self._input_args["er_N_btstrp"], # What should go here?
-                plot_iter_path=None
+                N_btstrp=self._input_args["er_N_btstrp"],  # What should go here?
+                plot_iter_path=None,
             )
 
             er_out_test_turbine_list_scada_0bias = self.er_out_test_turbine_list_scada.copy()
 
             self.er_out_test_turbine_list_scada = er_out_test_turbine_list_scada_copy
 
         # Plot
         for ii, ti in enumerate(self.test_turbines):
             if show_uncorrected_data:
                 axarr = er_out_test_turbine_list_scada_0bias[ii].plot_energy_ratios(
                     labels=["Measured data (uncorrected)"],
-                    color_dict={"Measured data (uncorrected)":"silver"},
-                    show_wind_speed_distribution=False
+                    color_dict={"Measured data (uncorrected)": "silver"},
+                    show_wind_speed_distribution=False,
                 )
                 axarr = self.er_out_test_turbine_list_scada[ii].plot_energy_ratios(
                     labels=["Measured data (bias corrected)"],
-                    color_dict={"Measured data (bias corrected)":"C0"},
+                    color_dict={"Measured data (bias corrected)": "C0"},
                     axarr=axarr,
-                    show_wind_speed_distribution=False
+                    show_wind_speed_distribution=False,
                 )
             else:
                 axarr = self.er_out_test_turbine_list_scada[ii].plot_energy_ratios(
-                    color_dict={"Measured data":"C0"},
-                    show_wind_speed_distribution=False
+                    color_dict={"Measured data": "C0"}, show_wind_speed_distribution=False
                 )
-            
+
             axarr = self.er_out_test_turbine_list_floris[ii].plot_energy_ratios(
-                color_dict={"FLORIS prediction":"C1"},
-                axarr=axarr, 
-                show_wind_speed_distribution=False
+                color_dict={"FLORIS prediction": "C1"},
+                axarr=axarr,
+                show_wind_speed_distribution=False,
             )
-            
-            axarr[0].set_title('Turbine {:03d}'.format(ti))
+
+            axarr[0].set_title("Turbine {:03d}".format(ti))
             if save_path is not None:
                 os.makedirs(os.path.dirname(save_path), exist_ok=True)
-                plt.savefig(save_path + '_{:03d}.{:s}'.format(ti, format), dpi=dpi)
+                plt.savefig(save_path + "_{:03d}.{:s}".format(ti, format), dpi=dpi)
 
             fig_list.append(plt.gcf())
             ax_list.append(axarr)
 
         return fig_list, ax_list
```

### Comparing `flasc-1.4.2/flasc/energy_ratio/total_uplift.py` & `flasc-2.0/flasc/analysis/total_uplift.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,211 +1,249 @@
-# This is a work in progress as we try to synthesize ideas from the 
-# table based methods and energy ratios back into one thing, 
+# This is a work in progress as we try to synthesize ideas from the
+# table based methods and energy ratios back into one thing,
 # some ideas we're incorporating:
 
 # Conversion from polars to pandas
 # Constructing tables (but now including tables of ratios)
 # Keeping track of frequencies is matching sized tables
 
 import warnings
+
 import numpy as np
 import polars as pl
 
-import flasc.energy_ratio.energy_ratio_utilities as util
+import flasc.utilities.energy_ratio_utilities as util
+from flasc.analysis.energy_ratio_input import EnergyRatioInput
+from flasc.data_processing.dataframe_manipulations import df_reduce_precision
+from flasc.logging_manager import LoggingManager
 
-from flasc.energy_ratio.energy_ratio_output import EnergyRatioOutput
-from flasc.energy_ratio.energy_ratio_input import EnergyRatioInput
-from flasc.dataframe_operations.dataframe_manipulations import df_reduce_precision
+logger_manager = LoggingManager()  # Instantiate LoggingManager
+logger = logger_manager.logger  # Obtain the reusable logger
 
 
 # Internal version, returns a polars dataframe
 def _compute_total_uplift_single(
-        df_,
-        df_names,
-        ref_cols,
-        test_cols,
-        wd_cols,
-        ws_cols,
-        wd_step = 2.0,
-        wd_min = 0.0,
-        wd_max = 360.0,
-        ws_step = 1.0,
-        ws_min = 0.0,
-        ws_max = 50.0,
-        bin_cols_in = ['wd_bin','ws_bin'],
-        weight_by = 'min', #min, sum
-        df_freq_pl = None,
-        wd_bin_overlap_radius = 0.,
-        uplift_pairs = [],
-        uplift_names = [],
-        remove_all_nulls = False
-    ):
- 
+    df_,
+    df_names,
+    ref_cols,
+    test_cols,
+    wd_cols,
+    ws_cols,
+    wd_step=2.0,
+    wd_min=0.0,
+    wd_max=360.0,
+    ws_step=1.0,
+    ws_min=0.0,
+    ws_max=50.0,
+    bin_cols_in=["wd_bin", "ws_bin"],
+    weight_by="min",  # min, sum
+    df_freq_pl=None,
+    wd_bin_overlap_radius=0.0,
+    uplift_pairs=[],
+    uplift_names=[],
+    remove_all_nulls=False,
+):
     """
     Compute the total change in energy production between two sets of turbines.
 
     Args:
         df_ (pl.DataFrame): A dataframe containing the data to use in the calculation.
-        df_names (list): A list of names to give to the dataframes. 
+        df_names (list): A list of names to give to the dataframes.
         ref_cols (list[str]): A list of columns to use as the reference turbines
         test_cols (list[str]): A list of columns to use as the test turbines
         wd_cols (list[str]): A list of columns to derive the wind directions from
         ws_cols (list[str]): A list of columns to derive the wind speeds from
         wd_step (float): The width of the wind direction bins.
         wd_min (float): The minimum wind direction to use.
         wd_max (float): The maximum wind direction to use.
         ws_step (float): The width of the wind speed bins.
         ws_min (float): The minimum wind speed to use.
         ws_max (float): The maximum wind speed to use.
-        bin_cols_in (list[str]): A list of column names to use for the wind speed and wind direction bins.
+        bin_cols_in (list[str]): A list of column names
+            to use for the wind speed and wind direction bins.
         weight_by (str): How to weight the energy ratio, options are 'min', or 'sum'.  'min' means
-            the minimum count across the dataframes is used to weight the energy ratio.   'sum' means the sum of the counts
+            the minimum count across the dataframes
+            is used to weight the energy ratio.   'sum' means the sum of the counts
             across the dataframes is used to weight the energy ratio.   Defaults to 'min'.
         df_freq_pl (pl.Dataframe) Polars dataframe of pre-provided per bin weights
-        wd_bin_overlap_radius (float): The distance in degrees one wd bin overlaps into the next, must be 
+        wd_bin_overlap_radius (float): The distance
+            in degrees one wd bin overlaps into the next, must be
             less or equal to half the value of wd_step
-        uplift_pairs: (list[tuple]): List of pairs of df_names to compute uplifts for. Each element 
-            of the list should be a tuple (or list) of length 2, where the first element will be the 
-            base case in the uplift calculation and the second element will be the test case in the 
+        uplift_pairs: (list[tuple]): List of pairs of df_names to compute uplifts for. Each element
+            of the list should be a tuple (or list) of length 2, where the first element will be the
+            base case in the uplift calculation and the second element will be the test case in the
             uplift calculation. If None, no uplifts are computed.
-        uplift_names: (list[str]): Names for the uplift columns, following the order of the 
+        uplift_names: (list[str]): Names for the uplift columns, following the order of the
             pairs specified in uplift_pairs. If None, will default to "uplift_df_name1_df_name2",
-        remove_all_nulls: (bool): Construct reference and test by strictly requiring all data to be 
-            available. If False, a minimum one data point from ref_cols, test_cols, wd_cols, and ws_cols
+        remove_all_nulls: (bool): Construct reference and test by strictly requiring all data to be
+            available. If False, a minimum one data point from
+            ref_cols, test_cols, wd_cols, and ws_cols
             must be available to compute the bin. Defaults to False.
 
     Returns:
         dict: A dictionary with results indexed for each element of uplift_names
         pl.DataFrame: A dataframe containing the weights each wind direction and wind speed bin
     """
 
     # Get the number of dataframes
     num_df = len(df_names)
 
-    bin_cols_without_df_name = [c for c in bin_cols_in if c != 'df_name']
+    bin_cols_without_df_name = [c for c in bin_cols_in if c != "df_name"]
 
     # Filter df_ to remove null values
     null_filter = util.filter_all_nulls if remove_all_nulls else util.filter_any_nulls
     df_ = null_filter(df_, ref_cols, test_cols, ws_cols, wd_cols)
     if len(df_) == 0:
         raise RuntimeError("After removing nulls, no data remains for computation.")
 
     # Apply binning to dataframe and aggregate bins
-    df_ = util.bin_and_group_dataframe(df_, ref_cols, test_cols, wd_cols, ws_cols, wd_step, wd_min, 
-        wd_max, ws_step, ws_min, ws_max, wd_bin_overlap_radius,
-        remove_all_nulls, bin_cols_without_df_name, num_df)
+    df_ = util.bin_and_group_dataframe(
+        df_,
+        ref_cols,
+        test_cols,
+        wd_cols,
+        ws_cols,
+        wd_step,
+        wd_min,
+        wd_max,
+        ws_step,
+        ws_min,
+        ws_max,
+        wd_bin_overlap_radius,
+        remove_all_nulls,
+        bin_cols_without_df_name,
+        num_df,
+    )
 
     # Determine the weighting of the ws/wd bins
     df_, df_freq_pl = util.add_bin_weights(df_, df_freq_pl, bin_cols_without_df_name, weight_by)
 
     # If total uplift requested, compute at this point
-    total_uplift_result = {}        
+    total_uplift_result = {}
     for uplift_pair, uplift_name in zip(uplift_pairs, uplift_names):
-        df_total = (df_
-                    .filter(pl.col('df_name').is_in(uplift_pair))
-                    .with_columns(power_ratio = pl.col('pow_test') / pl.col('pow_ref'),
-                                    weighted_pow_ref = pl.col('pow_ref') * pl.col('count'))
-                    .with_columns(total_count_per_bin = pl.col('count').sum().over(bin_cols_without_df_name))
-                    .with_columns(weighted_pow_ref = pl.col('weighted_pow_ref') / pl.col('total_count_per_bin'))
-                    .with_columns(weighted_pow_ref = pl.col('weighted_pow_ref').sum().over(bin_cols_without_df_name))
-                    
-                    .pivot(values=['power_ratio'], 
-                        columns='df_name', 
-                        index=bin_cols_without_df_name + ['weight','weighted_pow_ref'],
-                        aggregate_function='first')
-
-                    # Renorm the weight
-                    .with_columns(pl.col('weight') / pl.col('weight').sum())
-
-                    .with_columns(delta_power_ratio = pl.col(uplift_pair[1]) - pl.col(uplift_pair[0]))
-                    .with_columns(delta_aep = pl.col('weight') * pl.col('delta_power_ratio') * pl.col('weighted_pow_ref'),
-                                    base_aep = pl.col('weight') * pl.col(uplift_pair[0]) * pl.col('weighted_pow_ref'), )
-                    .sum()
+        df_total = (
+            df_.filter(pl.col("df_name").is_in(uplift_pair))
+            .with_columns(
+                power_ratio=pl.col("pow_test") / pl.col("pow_ref"),
+                weighted_pow_ref=pl.col("pow_ref") * pl.col("count"),
+            )
+            .with_columns(total_count_per_bin=pl.col("count").sum().over(bin_cols_without_df_name))
+            .with_columns(
+                weighted_pow_ref=pl.col("weighted_pow_ref") / pl.col("total_count_per_bin")
+            )
+            .with_columns(
+                weighted_pow_ref=pl.col("weighted_pow_ref").sum().over(bin_cols_without_df_name)
+            )
+            .pivot(
+                values=["power_ratio"],
+                columns="df_name",
+                index=bin_cols_without_df_name + ["weight", "weighted_pow_ref"],
+                aggregate_function="first",
+            )
+            # Renorm the weight
+            .with_columns(pl.col("weight") / pl.col("weight").sum())
+            .with_columns(delta_power_ratio=pl.col(uplift_pair[1]) - pl.col(uplift_pair[0]))
+            .with_columns(
+                delta_aep=pl.col("weight")
+                * pl.col("delta_power_ratio")
+                * pl.col("weighted_pow_ref"),
+                base_aep=pl.col("weight") * pl.col(uplift_pair[0]) * pl.col("weighted_pow_ref"),
+            )
+            .sum()
         )
 
-        delta_aep = 8760 * df_total.select('delta_aep').item()
-        percent_delta_aep = 100 * (df_total.select('delta_aep').item() / df_total.select('base_aep').item())
+        delta_aep = 8760 * df_total.select("delta_aep").item()
+        percent_delta_aep = 100 * (
+            df_total.select("delta_aep").item() / df_total.select("base_aep").item()
+        )
 
         if np.isnan(delta_aep):
             if ws_min < 5.0:
-                warnings.warn("NaNs detected in power ratios. This can result from "\
-                    +"the reference power being 0, which can occur when wind speed is "\
-                    "very low. Try setting ws_min keyword argument to remove 0 power "\
-                    "wind speeds.")
+                warnings.warn(
+                    "NaNs detected in power ratios. This can result from "
+                    + "the reference power being 0, which can occur when wind speed is "
+                    "very low. Try setting ws_min keyword argument to remove 0 power "
+                    "wind speeds."
+                )
             else:
                 warnings.warn("NaNs detected in power ratios.")
 
         total_uplift_result[uplift_name] = {
             "energy_uplift_ctr": delta_aep,
             "energy_uplift_lb": None,
             "energy_uplift_ub": None,
             "energy_uplift_ctr_pc": percent_delta_aep,
             "energy_uplift_lb_pc": None,
-            "energy_uplift_ub_pc": None
+            "energy_uplift_ub_pc": None,
         }
 
     return total_uplift_result, df_freq_pl
 
 
 # Bootstrap function wraps the _compute_energy_ratio function
-def _compute_total_uplift_bootstrap(er_in,
-                         ref_cols,
-                         test_cols,
-                         wd_cols,
-                         ws_cols,
-                         wd_step = 2.0,
-                         wd_min = 0.0,
-                         wd_max = 360.0,
-                         ws_step = 1.0,
-                         ws_min = 0.0,
-                         ws_max = 50.0,
-                         bin_cols_in = ['wd_bin','ws_bin'],
-                         weight_by = 'min', #min, sum
-                         df_freq_pl = None,
-                         wd_bin_overlap_radius = 0.,
-                         uplift_pairs = [],
-                         uplift_names = [],
-                         N = 1,
-                         percentiles=[5., 95.],
-                         remove_all_nulls=False,
-                         ):
-    
+def _compute_total_uplift_bootstrap(
+    er_in,
+    ref_cols,
+    test_cols,
+    wd_cols,
+    ws_cols,
+    wd_step=2.0,
+    wd_min=0.0,
+    wd_max=360.0,
+    ws_step=1.0,
+    ws_min=0.0,
+    ws_max=50.0,
+    bin_cols_in=["wd_bin", "ws_bin"],
+    weight_by="min",  # min, sum
+    df_freq_pl=None,
+    wd_bin_overlap_radius=0.0,
+    uplift_pairs=[],
+    uplift_names=[],
+    N=1,
+    percentiles=[5.0, 95.0],
+    remove_all_nulls=False,
+):
     """
     Compute the total change in energy production between two sets of turbines with bootstrapping
 
     Args:
-        er_in (EnergyRatioInput): An EnergyRatioInput object containing the data to use in the calculation.
+        er_in (EnergyRatioInput): An EnergyRatioInput object
+            containing the data to use in the calculation.
         ref_cols (list[str]): A list of columns to use as the reference turbines
         test_cols (list[str]): A list of columns to use as the test turbines
         wd_cols (list[str]): A list of columns to derive the wind directions from
         ws_cols (list[str]): A list of columns to derive the wind speeds from
         wd_step (float): The width of the wind direction bins.
         wd_min (float): The minimum wind direction to use.
         wd_max (float): The maximum wind direction to use.
         ws_step (float): The width of the wind speed bins.
         ws_min (float): The minimum wind speed to use.
         ws_max (float): The maximum wind speed to use.
-        bin_cols_in (list[str]): A list of column names to use for the wind speed and wind direction bins.
+        bin_cols_in (list[str]): A list of column names to use for
+            the wind speed and wind direction bins.
         weight_by (str): How to weight the energy ratio, options are 'min', or 'sum'.  'min' means
-            the minimum count across the dataframes is used to weight the energy ratio. 'sum' means the sum of the counts
+            the minimum count across the dataframes
+            is used to weight the energy ratio. 'sum' means the sum of the counts
             across the dataframes is used to weight the energy ratio.
         df_freq_pl (pl.Dataframe) Polars dataframe of pre-provided per bin weights
-        wd_bin_overlap_radius (float): The distance in degrees one wd bin overlaps into the next, must be 
+        wd_bin_overlap_radius (float): The distance
+            in degrees one wd bin overlaps into the next, must be
             less or equal to half the value of wd_step
-        uplift_pairs: (list[tuple]): List of pairs of df_names to compute uplifts for. Each element 
-            of the list should be a tuple (or list) of length 2, where the first element will be the 
-            base case in the uplift calculation and the second element will be the test case in the 
+        uplift_pairs: (list[tuple]): List of pairs of df_names to compute uplifts for. Each element
+            of the list should be a tuple (or list) of length 2, where the first element will be the
+            base case in the uplift calculation and the second element will be the test case in the
             uplift calculation. If None, no uplifts are computed.
-        uplift_names: (list[str]): Names for the uplift columns, following the order of the 
+        uplift_names: (list[str]): Names for the uplift columns, following the order of the
             pairs specified in uplift_pairs. If None, will default to "uplift_df_name1_df_name2"
         N (int): The number of bootstrap samples to use.
-        percentiles: (list or None): percentiles to use when returning energy ratio bounds. 
+        percentiles: (list or None): percentiles to use when returning energy ratio bounds.
             If specified as None with N > 1 (bootstrapping), defaults to [5, 95].
-        remove_all_nulls: (bool): Construct reference and test by strictly requiring all data to be 
-                available. If False, a minimum one data point from ref_cols, test_cols, wd_cols, and ws_cols
+        remove_all_nulls: (bool): Construct reference and test by strictly requiring all data to be
+                available. If False, a minimum one data point
+                from ref_cols, test_cols, wd_cols, and ws_cols
                 must be available to compute the bin. Defaults to False.
 
 
     Returns:
         pl.DataFrame: A dataframe containing the energy ratio between the two sets of turbines.
 
     """
@@ -227,124 +265,135 @@
             ws_max,
             bin_cols_in,
             weight_by,
             df_freq_pl,
             wd_bin_overlap_radius,
             uplift_pairs,
             uplift_names,
-            remove_all_nulls
-        ) for i in range(N)
+            remove_all_nulls,
+        )
+        for i in range(N)
     ]
     # df_concat = pl.concat([uplift_single_out[0] for uplift_single_out in uplift_single_outs])
     # First output contains the original table; use that df_freq_pl
     df_freq_pl = uplift_single_outs[0][1]
 
-
     # Add in the statistics
     total_uplift_result = {}
 
     for uplift_name in uplift_names:
         delta_aeps = np.zeros(N)
         percent_delta_aeps = np.zeros(N)
 
         for i in range(N):
             delta_aeps[i] = uplift_single_outs[i][0][uplift_name]["energy_uplift_ctr"]
             percent_delta_aeps[i] = uplift_single_outs[i][0][uplift_name]["energy_uplift_ctr_pc"]
 
         delta_aep_central = delta_aeps[0]
-        delta_aep_lb =  np.quantile(delta_aeps, percentiles[0]/100)
-        delta_aep_ub =  np.quantile(delta_aeps, percentiles[1]/100)
+        delta_aep_lb = np.quantile(delta_aeps, percentiles[0] / 100)
+        delta_aep_ub = np.quantile(delta_aeps, percentiles[1] / 100)
 
         percent_delta_aep_central = percent_delta_aeps[0]
-        percent_delta_aep_lb =  np.quantile(percent_delta_aeps, percentiles[0]/100)
-        percent_delta_aep_ub =  np.quantile(percent_delta_aeps, percentiles[1]/100)
+        percent_delta_aep_lb = np.quantile(percent_delta_aeps, percentiles[0] / 100)
+        percent_delta_aep_ub = np.quantile(percent_delta_aeps, percentiles[1] / 100)
 
         total_uplift_result[uplift_name] = {
             "energy_uplift_ctr": delta_aep_central,
             "energy_uplift_lb": delta_aep_lb,
             "energy_uplift_ub": delta_aep_ub,
             "energy_uplift_ctr_pc": percent_delta_aep_central,
             "energy_uplift_lb_pc": percent_delta_aep_lb,
-            "energy_uplift_ub_pc": percent_delta_aep_ub
+            "energy_uplift_ub_pc": percent_delta_aep_ub,
         }
 
     return total_uplift_result, df_freq_pl
 
 
-def compute_total_uplift(er_in: EnergyRatioInput,
-                         ref_turbines = None,
-                         test_turbines = None,
-                         wd_turbines = None,
-                         ws_turbines = None,
-                         use_predefined_ref = False,
-                         use_predefined_wd = False,
-                         use_predefined_ws = False,
-                         wd_step = 2.0,
-                         wd_min = 0.0,
-                         wd_max = 360.0,
-                         ws_step = 1.0,
-                         ws_min = 0.0,
-                         ws_max = 50.0,
-                         bin_cols_in = ['wd_bin','ws_bin'],
-                         weight_by = 'min', #min or sum
-                         df_freq = None,
-                         wd_bin_overlap_radius = 0.,
-                         uplift_pairs = None,
-                         uplift_names = None,
-                         N = 1,
-                         percentiles = None,
-                         remove_all_nulls = False
-    ) -> dict: # dict output for now, may change later
-    
+def compute_total_uplift(
+    er_in: EnergyRatioInput,
+    ref_turbines=None,
+    test_turbines=None,
+    wd_turbines=None,
+    ws_turbines=None,
+    use_predefined_ref=False,
+    use_predefined_wd=False,
+    use_predefined_ws=False,
+    wd_step=2.0,
+    wd_min=0.0,
+    wd_max=360.0,
+    ws_step=1.0,
+    ws_min=0.0,
+    ws_max=50.0,
+    bin_cols_in=["wd_bin", "ws_bin"],
+    weight_by="min",  # min or sum
+    df_freq=None,
+    wd_bin_overlap_radius=0.0,
+    uplift_pairs=None,
+    uplift_names=None,
+    N=1,
+    percentiles=None,
+    remove_all_nulls=False,
+) -> dict:  # dict output for now, may change later
     """
     Compute the energy ratio between two sets of turbines with bootstrapping
 
     Args:
-        er_in (EnergyRatioInput): An EnergyRatioInput object containing the data to use in the calculation.
+        er_in (EnergyRatioInput): An EnergyRatioInput object
+            containing the data to use in the calculation.
         ref_turbines (list[int]): A list of turbine numbers to use as the reference.
         test_turbines (list[int]): A list of turbine numbers to use as the test.
         ws_turbines (list[int]): A list of turbine numbers to use for the wind speeds
         wd_turbines (list[int]): A list of turbine numbers to use for the wind directions
         use_predefined_ref (bool): If True, use the pow_ref column of df_ as the reference power.
         use_predefined_ws (bool): If True, use the ws column of df_ as the wind speed.
         use_predefined_wd (bool): If True, use the wd column of df_ as the wind direction.
         wd_step (float): The width of the wind direction bins.
         wd_min (float): The minimum wind direction to use.
         wd_max (float): The maximum wind direction to use.
         ws_step (float): The width of the wind speed bins.
         ws_min (float): The minimum wind speed to use.
         ws_max (float): The maximum wind speed to use.
-        bin_cols_in (list[str]): A list of column names to use for the wind speed and wind direction bins.
+        bin_cols_in (list[str]): A list of column names to
+            use for the wind speed and wind direction bins.
         weight_by (str): How to weight the energy ratio, options are 'min', , or 'sum'.  'min' means
-            the minimum count across the dataframes is used to weight the energy ratio.   'sum' means the sum of the counts
+            the minimum count across the dataframes is used to weight the energy ratio.
+            'sum' means the sum of the counts
             across the dataframes is used to weight the energy ratio.
-        df_freq (pd.Dataframe): A dataframe which specifies the frequency of the ws/wd bin combinations.  Provides
+        df_freq (pd.Dataframe): A dataframe which specifies the
+            frequency of the ws/wd bin combinations.  Provides
             a method to use an explicit or long-term weigthing of bins.  Dataframe should include
-            columns ws, wd and freq_val.  ws and wd should correspond to the bin centers resulting from
-            the choices of the ws/wd_min / _max / _step.  In the case that df_freq has extra bins that aren't included 
-            in those given by ws/wd min, max, step, they will be ignored in the energy ratio calculation. 
-            Any bins given by ws/wd min, max, step not present in df_freq will be assigned a frequency of zero. 
+            columns ws, wd and freq_val.  ws and wd should
+            orrespond to the bin centers resulting from
+            the choices of the ws/wd_min / _max / _step.
+            In the case that df_freq has extra bins that aren't included
+            in those given by ws/wd min, max, step, they will
+            be ignored in the energy ratio calculation.
+            Any bins given by ws/wd min, max, step not present in
+            df_freq will be assigned a frequency of zero.
             Defaults to None.
-        wd_bin_overlap_radius (float): The distance in degrees one wd bin overlaps into the next, must be 
+        wd_bin_overlap_radius (float): The distance in degrees
+            one wd bin overlaps into the next, must be
             less or equal to half the value of wd_step
-        uplift_pairs: (list[tuple]): List of pairs of df_names to compute uplifts for. Each element 
-            of the list should be a tuple (or list) of length 2, where the first element will be the 
-            base case in the uplift calculation and the second element will be the test case in the 
+        uplift_pairs: (list[tuple]): List of pairs of df_names to compute uplifts for. Each element
+            of the list should be a tuple (or list) of length 2, where the first element will be the
+            base case in the uplift calculation and the second element will be the test case in the
             uplift calculation. If None, no uplifts are computed.
-        uplift_names: (list[str]): Names for the uplift columns, following the order of the 
+        uplift_names: (list[str]): Names for the uplift columns, following the order of the
             pairs specified in uplift_pairs. If None, will default to "uplift_df_name1_df_name2"
         N (int): The number of bootstrap samples to use.
-        percentiles: (list or None): percentiles to use when returning energy ratio bounds. 
+        percentiles: (list or None): percentiles to use when returning energy ratio bounds.
             If specified as None with N > 1 (bootstrapping), defaults to [5, 95].
-        remove_all_nulls: (bool): Construct reference and test by strictly requiring all data to be 
-                available. If False, a minimum one data point from ref_cols, test_cols, wd_cols, and ws_cols
+        remove_all_nulls: (bool): Construct reference and test by strictly requiring all data to be
+                available. If False, a minimum one data point from ref_cols, test_cols, wd_cols,
+                and ws_cols
                 must be available to compute the bin. Defaults to False.
 
     Returns:
-        EnergyRatioOutput: An EnergyRatioOutput object containing the energy ratio between the two sets of turbines.
+        EnergyRatioOutput: An EnergyRatioOutput object containing the energy ratio between the
+        two sets of turbines.
 
     """
 
     # Get the polars dataframe from within the er_in
     df_ = er_in.get_df()
 
     # Check that inputs are valid
@@ -368,32 +417,32 @@
         df_freq,
         wd_bin_overlap_radius,
         uplift_pairs,
         uplift_names,
         False,
         N,
         percentiles,
-        remove_all_nulls
+        remove_all_nulls,
     )
-    
-     # Set up the column names for the reference and test power
+
+    # Set up the column names for the reference and test power
     if not use_predefined_ref:
-        ref_cols = [f'pow_{i:03d}' for i in ref_turbines]
+        ref_cols = [f"pow_{i:03d}" for i in ref_turbines]
     else:
-        ref_cols = ['pow_ref']
+        ref_cols = ["pow_ref"]
 
     if not use_predefined_ws:
-        ws_cols = [f'ws_{i:03d}' for i in ws_turbines]
+        ws_cols = [f"ws_{i:03d}" for i in ws_turbines]
     else:
-        ws_cols = ['ws']
+        ws_cols = ["ws"]
 
     if not use_predefined_wd:
-        wd_cols = [f'wd_{i:03d}' for i in wd_turbines]
+        wd_cols = [f"wd_{i:03d}" for i in wd_turbines]
     else:
-        wd_cols = ['wd']
+        wd_cols = ["wd"]
 
     # Confirm uplift pairs provided correctly
     if uplift_pairs is None:
         uplift_pairs = []
     elif isinstance(uplift_pairs[0], str) and len(uplift_pairs) == 2:
         # Single pair provided, not in list of lists
         uplift_pairs = [uplift_pairs]
@@ -401,46 +450,41 @@
         for up in uplift_pairs:
             if len(up) != 2:
                 raise ValueError("uplift_pairs should be a list of tuples of length 2.")
     if uplift_names is not None:
         if len(uplift_names) != len(uplift_pairs):
             raise ValueError("Length of uplift_names should match length of uplift_pairs")
     else:
-        uplift_names = ["uplift_"+up[1]+"/"+up[0] for up in uplift_pairs]
+        uplift_names = ["uplift_" + up[1] + "/" + up[0] for up in uplift_pairs]
 
     # Convert the numbered arrays to appropriate column names
-    test_cols = [f'pow_{i:03d}' for i in test_turbines]
+    test_cols = [f"pow_{i:03d}" for i in test_turbines]
 
     # If df_freq is provided, confirm is consistent with ws/wd min max and
     # prepare a polars table of weights
     if df_freq is not None:
-
         # Maybe not test, not sure yet
         # ws_edges = np.arange(ws_min, ws_max+ws_step,ws_step)
         # ws_labels = ws_edges[:-1] + np.diff(ws_edges)/2.0
         # wd_edges = np.arange(wd_min, wd_max+wd_step,wd_step)
         # wd_labels = wd_edges[:-1] + np.diff(wd_edges)/2.0
-        
+
         # Conver to polars dataframe
         df_freq_pl = pl.from_pandas(df_reduce_precision(df_freq, allow_convert_to_integer=False))
 
         # Rename the columns
-        df_freq_pl = df_freq_pl.rename({
-            'ws':'ws_bin',
-            'wd':'wd_bin',
-            'freq_val':'weight'
-        })
+        df_freq_pl = df_freq_pl.rename({"ws": "ws_bin", "wd": "wd_bin", "freq_val": "weight"})
 
     else:
         df_freq_pl = None
 
     # If N=1, don't use bootstrapping
     if N == 1:
         if percentiles is not None:
-            print("percentiles can only be used with bootstrapping (N > 1).")
+            logger.warn("percentiles can only be used with bootstrapping (N > 1).")
         # Compute the energy ratio
         total_uplift_result, df_freq_pl = _compute_total_uplift_single(
             df_,
             er_in.df_names,
             ref_cols,
             test_cols,
             wd_cols,
@@ -453,22 +497,24 @@
             ws_max,
             bin_cols_in,
             weight_by,
             df_freq_pl,
             wd_bin_overlap_radius,
             uplift_pairs,
             uplift_names,
-            remove_all_nulls
+            remove_all_nulls,
         )
     else:
         if percentiles is None:
             percentiles = [5, 95]
         elif not hasattr(percentiles, "__len__") or len(percentiles) != 2:
-            raise ValueError("percentiles should be a two element list of the "+\
-                "upper and lower desired percentiles.")
+            raise ValueError(
+                "percentiles should be a two element list of the "
+                + "upper and lower desired percentiles."
+            )
 
         total_uplift_result, df_freq_pl = _compute_total_uplift_bootstrap(
             er_in,
             ref_cols,
             test_cols,
             wd_cols,
             ws_cols,
@@ -481,13 +527,13 @@
             bin_cols_in,
             weight_by,
             df_freq_pl,
             wd_bin_overlap_radius,
             uplift_pairs,
             uplift_names,
             N,
-            percentiles
+            percentiles,
         )
 
-    # Do we want some kind of more complex return object? Or are we OK 
+    # Do we want some kind of more complex return object? Or are we OK
     # returning just the total_uplift_result dictionary?
-    return total_uplift_result
+    return total_uplift_result
```

### Comparing `flasc-1.4.2/flasc/floris_tools.py` & `flasc-2.0/flasc/utilities/floris_tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,99 +1,39 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
+import copy
+from time import perf_counter as timerpc
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+from floris import TimeSeries, WindTIRose
+from floris.utilities import wrap_360
 from scipy import interpolate
 from scipy.stats import norm
-import copy
 
-from floris.tools import FlorisInterface
-from floris.utilities import wrap_360
-from flasc import utilities as fsut
+from flasc.logging_manager import LoggingManager
+from flasc.utilities import utilities as fsut
 
+logger_manager = LoggingManager()  # Instantiate LoggingManager
+logger = logger_manager.logger  # Obtain the reusable logger
 
-def merge_floris_objects(fi_list, reference_wind_height=None):
-    """Merge a list of FlorisInterface objects into a single FlorisInterface object. Note that it uses
-    the very first object specified in fi_list to build upon, so it uses those wake model parameters,
-    air density, and so on.
 
-    Args:
-        fi_list (list): Array-like of FlorisInterface objects.
-        reference_wind_height (float, optional): Height in meters at which the reference wind speed is
-        assigned. If None, will assume this value is equal to the reference wind height specified in
-        the FlorisInterface objects. This only works if all objects have the same value for their
-        reference_wind_height.
-
-    Returns:
-        fi_merged (FlorisInterface): The merged FlorisInterface object, merged in the same order as fi_list.
-        The objects are merged on the turbine locations and turbine types, but not on the wake parameters
-        or general solver settings.
-    """
-
-    # Make sure the entries in fi_list are FlorisInterface objects
-    if not isinstance(fi_list[0], FlorisInterface):
-        raise UserWarning("Incompatible input specified. Please merge FlorisInterface objects before inserting them into ParallelComputingInterface and UncertaintyInterface.")
-
-    # Get the turbine locations and specifications for each subset and save as a list
-    x_list = []
-    y_list = []
-    turbine_type_list = []
-    reference_wind_heights = []
-    for fi in fi_list:
-        x_list.extend(fi.layout_x)
-        y_list.extend(fi.layout_y)
-
-        fi_turbine_type = fi.floris.farm.turbine_type
-        if len(fi_turbine_type) == 1:
-            fi_turbine_type = fi_turbine_type * len(fi.layout_x)
-        elif not len(fi_turbine_type) == len(fi.layout_x):
-            raise UserWarning("Incompatible format of turbine_type in FlorisInterface.")
-
-        turbine_type_list.extend(fi_turbine_type)
-        reference_wind_heights.append(fi.floris.flow_field.reference_wind_height)
-
-    # Derive reference wind height, if unspecified by the user
-    if reference_wind_height is None:
-        reference_wind_height = np.mean(reference_wind_heights)
-        if np.any(np.abs(np.array(reference_wind_heights) - reference_wind_height) > 1.0e-3):
-            raise UserWarning("Cannot automatically derive a fitting reference_wind_height since they substantially differ between FlorisInterface objects. Please specify 'reference_wind_height' manually.")
-
-    # Construct the merged FLORIS model based on the first entry in fi_list
-    fi_merged = fi_list[0].copy()
-    fi_merged.reinitialize(
-        layout_x=x_list,
-        layout_y=y_list,
-        turbine_type=turbine_type_list,
-        reference_wind_height=reference_wind_height
-    )
-
-    return fi_merged
+# Disable line too long for this file for csv block
+# Some comment blocks would be confusing otherwise
+# ruff: noqa: E501
 
 
 def interpolate_floris_from_df_approx(
     df,
     df_approx,
-    method='linear',
+    method="linear",
     wrap_0deg_to_360deg=True,
     extrapolate_ws=True,
     extrapolate_ti=True,
     mirror_nans=True,
-    verbose=True
+    verbose=True,
 ):
     """This function generates the FLORIS predictions for a set of historical
     data, 'df', quickly by linearly interpolating from a precalculated set of
     FLORIS solutions, 'df_approx'. We use linear interpolation to eliminate
     dependency of the computation time on the size of the dataframe/number of
     timeseries samples.
 
@@ -101,33 +41,33 @@
         df (pd.DataFrame): A Pandas DataFrame containing the timeseries for
         which the FLORIS predictions should be calculated. It should contain
         at least the columns 'wd', 'ws', and 'ti', which are respectively the
         ambient wind direction, ambient wind speed, and ambient turbulence
         intensity to be used in the FLORIS predictions. An example:
 
         df=
-                 time                    wd     ws      ti  
+                 time                    wd     ws      ti
         0       2018-01-01 00:10:00   213.1   7.81    0.08
         1       2018-01-01 00:20:00   215.6   7.65    0.08
         ...                     ...   ...      ...     ...
         52103   2018-12-31 23:30:00    15.6   11.0    0.08
         52104   2018-12-31 23:40:00    15.3   11.1    0.08
 
         df_approx (pd.DataFrame): A Pandas DataFrame containing the precalculated
         solutions of the FLORIS model for a large grid of ambient wind directions,
         wind speeds and turbulence intensities. This table is typically calculated
         using the 'calc_floris_approx_table(...)' function described below, but
         can also be generated by hand using other tools like PyWake. df_approx
         typically has the form:
 
         df_approx=
-                  wd    ws    ti    pow_000     pow_001  ...    pow_006 
+                  wd    ws    ti    pow_000     pow_001  ...    pow_006
         0        0.0   1.0    0.03      0.0         0.0  ...        0.0
         1        3.0   1.0    0.03      0.0         0.0  ...        0.0
-        ...      ...   ...   ...        ...         ...  ...        ... 
+        ...      ...   ...   ...        ...         ...  ...        ...
         32399  357.0  24.0    0.18    5.0e6       5.0e6  ...       5.0e6
         32400  360.0  24.0    0.18    5.0e6       5.0e6  ...       5.0e6
 
         method (str, optional): Interpolation method, options are 'nearest' and
         'linear'. Defaults to 'linear'.
         wrap_0deg_to_360deg (bool, optional): The precalculated set of FLORIS solutions
         are typically calculates from 0 deg to 360 deg in steps of 2.0 deg or 3.0 deg.
@@ -135,16 +75,16 @@
         at 357.0 deg or 358.0 deg. If the user uses this for interpolation, any wind
         directions in 'df' with a value between 358.0 deg and 360.0 deg cannot be
         interpolated because it falls outside the bounds. This option copies the
         precalculated table solutions from 0 deg over to 360 deg to allow interpolation
         for the entire wind rose. Recommended to set to True. Defaults to True.
         extrapolate_ws (bool, optional): The precalculated set of FLORIS solutions,
         df_approx, only covers a finite range of wind speeds, typically from 1 m/s up
-        to 25 m/s. Any wind speed values below or above this range therefore cannot 
-        be interpolated using the 'linear' method and therefore becomes a NaN. To 
+        to 25 m/s. Any wind speed values below or above this range therefore cannot
+        be interpolated using the 'linear' method and therefore becomes a NaN. To
         prevent this, we can copy over the lowest and highest wind speed value interpolated
         to finite bounds to avoid this. For example, if our lowest wind speed calculated is
         1 m/s, we copy the solutions at 1 m/s over to a wind speed of 0 m/s, implicitly
         assuming these values are equal. This allows interpolation over wind speeds below
         1 m/s. Additionally, we copy the highest wind speed solutions (e.g., 25 m/s) over
         to a wind speed of 99 m/s to allow interpolation of values up to 99 m/s.
         Defaults to True.
@@ -169,167 +109,236 @@
 
     Returns:
         df (pd.DataFrame): The Pandas Dataframe containing the timeseries 'wd', 'ws'
         and 'ti', plus the power productions (and potentially local inflow conditions)
         of the turbines interpolated from the precalculated solutions table. For example,
 
         df=
-                 time                    wd     ws      ti    pow_000     pow_001  ...    pow_006 
+                 time                    wd     ws      ti    pow_000     pow_001  ...    pow_006
         0       2018-01-01 00:10:00   213.1   7.81    0.08  1251108.2    825108.2  ...   725108.9
         1       2018-01-01 00:20:00   215.6   7.65    0.08  1202808.0    858161.8  ...   692111.2
         ...                     ...   ...      ...     ...         ...        ...  ...        ...
         52103   2018-12-31 23:30:00    15.6   11.0    0.08  4235128.7   3825108.4  ...  2725108.3
         52104   2018-12-31 23:40:00    15.3   11.1    0.08  3860281.3   3987634.7  ...  2957021.7
     """
 
     # Format dataframe and get number of turbines
     # df = df.reset_index(drop=('time' in df.columns))
     nturbs = fsut.get_num_turbines(df_approx)
 
     # Check input
     if mirror_nans:
-        if not ("pow_000" in df.columns) or not ("ws_000" in df.columns):
-            raise UserWarning("The option mirror_nans=True requires the raw data's wind speed and power measurements to be included in the dataframe 'df'.")
+        if "pow_000" not in df.columns or "ws_000" not in df.columns:
+            raise UserWarning(
+                "The option mirror_nans=True requires the raw data's wind speed and power measurements to be included in the dataframe 'df'."
+            )
+    else:
+        logger.warning(
+            "Warning: not mirroring NaNs from the raw data to the FLORIS predictions. This may skew your energy ratios."
+        )
+
+    # Check dimensionality: do we have a 2D or a 3D grid
+    N_wd = len(np.unique(df_approx["wd"]))
+    N_ws = len(np.unique(df_approx["ws"]))
+    N_ti = len(np.unique(df_approx["ti"]))
+    if (N_wd * N_ws) == df_approx.shape[0]:
+        grid_type = "2d"
+    elif (N_wd * N_ws * N_ti) == df_approx.shape[0]:
+        grid_type = "3d"
     else:
-        print("Warning: not mirroring NaNs from the raw data to the FLORIS predictions. This may skew your energy ratios.")
+        raise UserWarning("Incompatible df_approx table specified.")
+    if verbose:
+        logger.info(f"Identified the following grid type: {grid_type}.")
 
     # Check if all values in df fall within the precalculated solutions ranges
-    for col in ["wd", "ws", "ti"]:
+    if grid_type == "2d":
+        cols = ["wd", "ws", "ti"]
+    else:
+        cols = ["wd", "ws"]
+
+    for col in cols:
         # Check if all columns are defined
         if col not in df.columns:
             raise ValueError("Your SCADA dataframe is missing a column called '{:s}'.".format(col))
         if col not in df_approx.columns:
-            raise ValueError("Your precalculated solutions dataframe is missing a column called '{:s}'.".format(col))
+            raise ValueError(
+                "Your precalculated solutions dataframe is missing a column called '{:s}'.".format(
+                    col
+                )
+            )
 
         # Check if approximate solutions cover the entire problem space
-        if (
-            (df[col].min() < (df_approx[col].min() - 1.0e-6)) |
-            (df[col].max() > (df_approx[col].max() + 1.0e-6))
+        if (df[col].min() < (df_approx[col].min() - 1.0e-6)) | (
+            df[col].max() > (df_approx[col].max() + 1.0e-6)
         ):
-            print("Warning: the values in df[{:s}] exceed the range in the precalculated solutions df_fi_approx[{:s}].".format(col, col))
-            print("   minimum/maximum value in df:        ({:.3f}, {:.3f})".format(df[col].min(), df[col].max()))
-            print("   minimum/maximum value in df_approx: ({:.3f}, {:.3f})".format(df_approx[col].min(), df_approx[col].max()))
-
+            logger.warning(
+                "Warning: the values in df[{:s}] exceed the range in the precalculated solutions df_fi_approx[{:s}].".format(
+                    col, col
+                )
+            )
+            logger.info(
+                "   minimum/maximum value in df:        ({:.3f}, {:.3f})".format(
+                    df[col].min(), df[col].max()
+                )
+            )
+            logger.info(
+                "   minimum/maximum value in df:        ({:.3f}, {:.3f})".format(
+                    df[col].min(), df[col].max()
+                )
+            )
+            logger.info(
+                "   minimum/maximum value in df_approx: ({:.3f}, {:.3f})".format(
+                    df_approx[col].min(), df_approx[col].max()
+                )
+            )
 
     # Define which variables we must map from df_approx to df
-    varnames = ['pow']
-    if 'ws_000' in df_approx.columns:
-        varnames.append('ws')
-    if 'wd_000' in df_approx.columns:
-        varnames.append('wd')
-    if 'ti_000' in df_approx.columns:
-        varnames.append('ti')
+    varnames = ["pow"]
+    if "ws_000" in df_approx.columns:
+        varnames.append("ws")
+    if "wd_000" in df_approx.columns:
+        varnames.append("wd")
+    if "ti_000" in df_approx.columns:
+        varnames.append("ti")
 
     # Map individual data entries to full DataFrame
     if verbose:
-        print("Mapping the precalculated solutions " +
-              "from FLORIS to the dataframe...")
-        print("  Creating a gridded interpolant with " +
-              "interpolation method '%s'." % method)
+        logger.info("Mapping the precalculated solutions " + "from FLORIS to the dataframe...")
+        logger.info(
+            "  Creating a gridded interpolant with " + "interpolation method '%s'." % method
+        )
 
     # Make a copy from wd=0.0 deg to wd=360.0 deg for wrapping
     if wrap_0deg_to_360deg and (not (df_approx["wd"] > 359.999999).any()):
         if not np.any(df_approx["wd"] < 0.01):
-            raise UserWarning("wrap_0deg_to_360deg is set to True but no solutions at wd=0 deg in the precalculated solution table.")
+            raise UserWarning(
+                "wrap_0deg_to_360deg is set to True but no solutions at wd=0 deg in the precalculated solution table."
+            )
         df_subset = df_approx[df_approx["wd"] == 0.0].copy()
         df_subset["wd"] = 360.0
-        df_approx = pd.concat([df_approx, df_subset], axis=0).reset_index(drop=True)
+        df_approx = pd.concat([df_approx, df_subset], axis=0)
 
     # Copy TI to lower and upper bound
-    if extrapolate_ti:
-        df_ti_lb = df_approx.loc[df_approx["ti"] == df_approx['ti'].min()].copy()
-        df_ti_ub = df_approx.loc[df_approx["ti"] == df_approx['ti'].max()].copy()
+    if (grid_type == "3d") and extrapolate_ti:
+        df_ti_lb = df_approx.loc[df_approx["ti"] == df_approx["ti"].min()].copy()
+        df_ti_ub = df_approx.loc[df_approx["ti"] == df_approx["ti"].max()].copy()
         df_ti_lb["ti"] = 0.0
         df_ti_ub["ti"] = 1.0
-        df_approx = pd.concat(
-            [df_approx, df_ti_lb, df_ti_ub],
-            axis=0
-        ).reset_index(drop=True)
+        df_approx = pd.concat([df_approx, df_ti_lb, df_ti_ub], axis=0)
 
     # Copy WS to lower and upper bound
     if extrapolate_ws:
-        df_ws_lb = df_approx.loc[df_approx["ws"] == df_approx['ws'].min()].copy()
-        df_ws_ub = df_approx.loc[df_approx["ws"] == df_approx['ws'].max()].copy()
+        df_ws_lb = df_approx.loc[df_approx["ws"] == df_approx["ws"].min()].copy()
+        df_ws_ub = df_approx.loc[df_approx["ws"] == df_approx["ws"].max()].copy()
         df_ws_lb["ws"] = 0.0
         df_ws_ub["ws"] = 99.0
-        df_approx = pd.concat(
-            [df_approx, df_ws_lb, df_ws_ub],
-            axis=0
-        ).reset_index(drop=True)
+        df_approx = pd.concat([df_approx, df_ws_lb, df_ws_ub], axis=0)
 
     # Convert df_approx dataframe into a regular grid
     wd_array_approx = np.sort(df_approx["wd"].unique())
     ws_array_approx = np.sort(df_approx["ws"].unique())
-    ti_array_approx = np.sort(df_approx["ti"].unique())
-    xg, yg, zg = np.meshgrid(
-        wd_array_approx,
-        ws_array_approx,
-        ti_array_approx,
-        indexing='ij',
-    )
+
+    if grid_type == "2d":
+        xg, yg = np.meshgrid(
+            wd_array_approx,
+            ws_array_approx,
+            indexing="ij",
+        )
+    else:
+        ti_array_approx = np.sort(df_approx["ti"].unique())
+        xg, yg, zg = np.meshgrid(
+            wd_array_approx,
+            ws_array_approx,
+            ti_array_approx,
+            indexing="ij",
+        )
 
     grid_dict = dict()
     for varname in varnames:
-        colnames = ['{:s}_{:03d}'.format(varname, ti) for ti in range(nturbs)]
-        f = interpolate.NearestNDInterpolator(
-            df_approx[["wd", "ws", "ti"]],
-            df_approx[colnames]
-        )
-        grid_dict["{:s}".format(varname)] = f(xg, yg, zg)
+        colnames = ["{:s}_{:03d}".format(varname, ti) for ti in range(nturbs)]
+        if grid_type == "2d":
+            f = interpolate.NearestNDInterpolator(df_approx[["wd", "ws"]], df_approx[colnames])
+            grid_dict["{:s}".format(varname)] = f(xg, yg)
+        else:
+            f = interpolate.NearestNDInterpolator(
+                df_approx[["wd", "ws", "ti"]], df_approx[colnames]
+            )
+            grid_dict["{:s}".format(varname)] = f(xg, yg, zg)
 
     # Prepare an minimal output dataframe
     cols_to_copy = ["wd", "ws", "ti"]
     if "time" in df.columns:
         cols_to_copy.append("time")
-    df_out = df[cols_to_copy].copy()
+    df_out = df[cols_to_copy].reset_index(drop=True).copy()
 
     # Use interpolant to determine values for all turbines and variables
+    t0 = timerpc()
+    df_out_interp_list = [df_out]
     for ii, varname in enumerate(varnames):
         if verbose:
-            print('     Interpolating ' + varname + ' for all turbines...')
-        colnames = ['{:s}_{:03d}'.format(varname, ti) for ti in range(nturbs)]
+            logger.info("     Interpolating " + varname + " for all turbines...")
+        colnames = ["{:s}_{:03d}".format(varname, ti) for ti in range(nturbs)]
 
         if ii == 0:
-            f = interpolate.RegularGridInterpolator(
-                points=(wd_array_approx, ws_array_approx, ti_array_approx),
-                values=grid_dict[varname],
-                method=method,
-                bounds_error=False,
-            )
+            if grid_type == "2d":
+                f = interpolate.RegularGridInterpolator(
+                    points=(wd_array_approx, ws_array_approx),
+                    values=grid_dict[varname],
+                    method=method,
+                    bounds_error=False,
+                )
+            else:
+                f = interpolate.RegularGridInterpolator(
+                    points=(wd_array_approx, ws_array_approx, ti_array_approx),
+                    values=grid_dict[varname],
+                    method=method,
+                    bounds_error=False,
+                )
         else:
             f.values = np.array(grid_dict[varname], dtype=float)
 
-        df_out.loc[df_out.index, colnames] = f(df[['wd', 'ws', 'ti']])
+        # Interpolate values across grid
+        if grid_type == "2d":
+            out = f(df[["wd", "ws"]])
+        else:
+            out = f(df[["wd", "ws", "ti"]])
 
         if mirror_nans:
             # Copy NaNs in the raw data to the FLORIS predictions
-            for c in colnames:
+            for cii, c in enumerate(colnames):
                 if c in df.columns:
-                    df_out.loc[df[c].isna(), c] = None
-                else:
-                    df_out.loc[:, c] = None
+                    out[df[c].isna(), cii] = np.nan
+
+        df_out_interp_list.append(pd.DataFrame(out, columns=colnames))
+
+    # Add interpolated solutions to df_out
+    df_out = pd.concat(df_out_interp_list, axis=1)
+
+    if verbose:
+        dt = timerpc() - t0
+        logger.info(f"Finished interpolation in {dt:.3f} seconds.")
 
     return df_out
 
 
 def calc_floris_approx_table(
-    fi,
+    fm,
     wd_array=np.arange(0.0, 360.0, 1.0),
     ws_array=np.arange(1.0, 25.01, 1.0),
     ti_array=np.arange(0.03, 0.1801, 0.03),
     save_turbine_inflow_conditions_to_df=False,
-    ):
+):
     """This function calculates a large number of floris solutions for a rectangular grid
     of wind directions ('wd_array'), wind speeds ('ws_array'), and optionally turbulence
     intensities ('ti_array'). The variables that are saved are each turbine's power
     production, and optionally also each turbine's inflow wind direction, wind speed and
     turbulence intensity if 'save_turbine_inflow_conditions_to_df==True'.
 
     Args:
-        fi (FlorisInterface): FlorisInterface object.
+        fm (FlorisModel): FlorisModel object.
         wd_array (array, optional): Array of wind directions to evaluate in [deg]. This expands with the
           number of wind speeds and turbulence intensities. Defaults to np.arange(0.0, 360.0, 1.0).
         ws_array (array, optional): Array of wind speeds to evaluate in [m/s]. This expands with the
           number of wind directions and turbulence intensities. Defaults to np.arange(1.0, 25.01, 1.0).
         ti_array (array, optional): Array of turbulence intensities to evaluate in [-]. This expands with the
           number of wind directions and wind speeds. Defaults to np.arange(0.03, 0.1801, 0.03).
         save_turbine_inflow_conditions_to_df (bool, optional): When set to True, will also write each turbine's
@@ -345,15 +354,15 @@
         Example for a 7-turbine floris object with
             wd_array=np.arange(0.0, 360.0, 3.0)
             ws_array=np.arange(1.0, 25.001, 1.0)
             ti_array=np.arange(0.03, 0.1801, 0.03)
             save_turbine_inflow_conditions_to_df=True
 
         Yields:
-        
+
         df_approx=
                   wd    ws    ti    pow_000     ws_000  wd_000  ti_000  pow_001  ...    pow_006     ws_006  wd_006  ti_006
         0        0.0   1.0    0.03      0.0      1.0       0.0     0.03     0.0  ...        0.0      1.0       0.0     0.03
         1        3.0   1.0    0.03      0.0      1.0       3.0     0.03     0.0  ...        0.0      1.0       3.0     0.03
         2        6.0   1.0    0.03      0.0      1.0       6.0     0.03     0.0  ...        0.0      1.0       6.0     0.03
         3        9.0   1.0    0.03      0.0      1.0       9.0     0.03     0.0  ...        0.0      1.0       9.0     0.03
         4       12.0   1.0    0.03      0.0      1.0      12.0     0.03     0.0  ...        0.0      1.0      12.0     0.03
@@ -364,74 +373,76 @@
         32398  354.0  25.0    0.18      0.0  24.880772   354.0     0.18     0.0  ...        0.0  24.881165   354.0     0.18
         32399  357.0  25.0    0.18      0.0  24.880829   357.0     0.18     0.0  ...        0.0  24.881165   357.0     0.18
         32400  360.0  25.0    0.18      0.0  24.880829   360.0     0.18     0.0  ...        0.0  24.881165   360.0     0.18
     """
 
     # if ti_array is None, use the current value in the FLORIS object
     if ti_array is None:
-        ti = fi.floris.flow_field.turbulence_intensity
+        ti = fm.core.flow_field.turbulence_intensity
         ti_array = np.array([ti], dtype=float)
 
-    fi = fi.copy()  # Create independent copy that we can manipulate
-    num_turbines = len(fi.layout_x)
+    fm = fm.copy()  # Create independent copy that we can manipulate
+    num_turbines = len(fm.layout_x)
 
     # Format input arrays
     wd_array = np.sort(wd_array)
     ws_array = np.sort(ws_array)
     ti_array = np.sort(ti_array)
-    wd_mesh, ws_mesh = np.meshgrid(wd_array, ws_array, indexing='ij')
+    wd_mesh, ws_mesh = np.meshgrid(wd_array, ws_array, indexing="ij")
     N_approx = len(wd_array) * len(ws_array) * len(ti_array)
-    print(
-        'Generating a df_approx table of FLORIS solutions ' +
-        'covering a total of {:d} cases.'.format(N_approx)
+    logger.info(
+        "Generating a df_approx table of FLORIS solutions "
+        + "covering a total of {:d} cases.".format(N_approx)
     )
 
     # Create solutions, one set per turbulence intensity
-    df_list = []
-    for turb_intensity in ti_array:
-        # Calculate solutions
-        fi.reinitialize(
+    fm.set(
+        wind_data=WindTIRose(
             wind_directions=wd_array,
             wind_speeds=ws_array,
-            turbulence_intensity=turb_intensity,
+            turbulence_intensities=ti_array,
         )
-        fi.calculate_wake()
-        turbine_powers = fi.get_turbine_powers()
+    )
+    fm.run()
+    turbine_powers = fm.get_turbine_powers().reshape(-1, fm.n_turbines)  # Want flattened version
 
-        # Create a dictionary to save solutions in
-        solutions_dict = {"wd": wd_mesh.flatten(), "ws": ws_mesh.flatten()}
-        solutions_dict["ti"] = turb_intensity * np.ones(len(wd_array) * len(ws_array))
-        for turbi in range(num_turbines):
-            solutions_dict["pow_{:03d}".format(turbi)] = turbine_powers[:, :, turbi].flatten()
-            if save_turbine_inflow_conditions_to_df:
-                solutions_dict["ws_{:03d}".format(turbi)] = \
-                    fi.floris.flow_field.u.mean(axis=4).mean(axis=3)[:, :, turbi].flatten()
-                solutions_dict["wd_{:03d}".format(turbi)] = \
-                    wd_mesh.flatten()  # Uniform wind direction
-                solutions_dict["ti_{:03d}".format(turbi)] = \
-                    fi.floris.flow_field.turbulence_intensity_field[:, :, turbi].flatten()
-        df_list.append(pd.DataFrame(solutions_dict))
+    solutions_dict = {
+        "wd": fm.wind_directions,
+        "ws": fm.wind_speeds,
+        "ti": fm.turbulence_intensities,
+    }
+    for tindex in range(num_turbines):
+        solutions_dict["pow_{:03d}".format(tindex)] = turbine_powers[:, tindex]
+        if save_turbine_inflow_conditions_to_df:
+            solutions_dict["ws_{:03d}".format(tindex)] = fm.core.flow_field.u.mean(axis=(2, 3))[
+                :, tindex
+            ]
+            solutions_dict["wd_{:03d}".format(tindex)] = fm.wind_directions
+            solutions_dict[
+                "ti_{:03d}".format(tindex)
+            ] = fm.core.flow_field.turbulence_intensity_field[:, tindex]
+    df_approx = pd.DataFrame(solutions_dict)
 
-    print('Finished calculating the FLORIS solutions for the dataframe.')
-    df_approx = pd.concat(df_list, axis=0).sort_values(by=["ti", "ws", "wd"])
+    logger.info("Finished calculating the FLORIS solutions for the dataframe.")
+    df_approx = df_approx.sort_values(by=["ti", "ws", "wd"])
     df_approx = df_approx.reset_index(drop=True)
 
     return df_approx
 
 
 def add_gaussian_blending_to_floris_approx_table(df_fi_approx, wd_std=3.0, pdf_cutoff=0.995):
     """This function applies a Gaussian blending across the wind direction for the predicted
     turbine power productions from FLORIS. This is a post-processing step and achieves the
-    same result as evaluating FLORIS directly with the UncertaintyInterface module. However,
+    same result as evaluating FLORIS directly with the UncertainFlorisModel module. However,
     having this as a postprocess step allows for rapid generation of the FLORIS solutions for
     different values of wd_std without having to re-run FLORIS.
 
     Args:
         df_fi_approx (pd.DataFrame): Pandas DataFrame with precalculated FLORIS solutions,
-          typically generated using flasc.floris_tools.calc_floris_approx_table().
+          typically generated using flasc.utilities.floris_tools.calc_floris_approx_table().
         wd_std (float, optional): Standard deviation of the Gaussian blur that is applied
           across the wind direction in degrees. Defaults to 3.0.
         pdf_cutoff (float, optional): Cut-off point of the probability density function of
           the Gaussian curve. Defaults to 0.995 and thereby includes three standard
           deviations to the left and to the right of the evaluation.
 
     Returns:
@@ -450,46 +461,49 @@
     wd_unc = np.linspace(-1 * bound, bound, 2 * wd_bnd + 1)
     wd_unc_pmf = norm.pdf(wd_unc, scale=wd_std)
     wd_unc_pmf /= np.sum(wd_unc_pmf)  # normalize so sum = 1.0
 
     # Map solutions to the right shape using a NN interpolant
     F = interpolate.NearestNDInterpolator(
         x=df_fi_approx[["wd", "ws", "ti"]],
-        y=df_fi_approx[[c for c in df_fi_approx.columns if "pow_" in c]]
+        y=df_fi_approx[[c for c in df_fi_approx.columns if "pow_" in c]],
     )
-    
+
     # Create new sets to interpolate over for Gaussian kernel
     wd = df_fi_approx["wd"]
     wd = wrap_360(np.tile(wd, (len(wd_unc), 1)).T + np.tile(wd_unc, (wd.shape[0], 1)))
 
     ws = df_fi_approx["ws"]
     ws = np.tile(ws, (len(wd_unc), 1)).T
 
     ti = df_fi_approx["ti"]
     ti = np.tile(ti, (len(wd_unc), 1)).T
 
     # Interpolate power values
     turbine_powers = F(wd, ws, ti)
-    weights = np.tile(wd_unc_pmf[None, :, None], (turbine_powers.shape[0], 1, turbine_powers.shape[2]))
+    weights = np.tile(
+        wd_unc_pmf[None, :, None], (turbine_powers.shape[0], 1, turbine_powers.shape[2])
+    )
     turbine_powers_gaussian = np.sum(weights * turbine_powers, axis=1)  # Weighted sum
 
     pow_cols = [c for c in df_fi_approx.columns if c.startswith("pow_")]
     df_fi_approx_gauss = pd.concat(
         [
             df_fi_approx[["wd", "ws", "ti"]],
-            pd.DataFrame(dict(zip(pow_cols, turbine_powers_gaussian.T)))
+            pd.DataFrame(dict(zip(pow_cols, turbine_powers_gaussian.T))),
         ],
-        axis=1
+        axis=1,
     )
-    
+
     return df_fi_approx_gauss
 
 
-def get_turbs_in_radius(x_turbs, y_turbs, turb_no, max_radius,
-                        include_itself, sort_by_distance=False):
+def get_turbs_in_radius(
+    x_turbs, y_turbs, turb_no, max_radius, include_itself, sort_by_distance=False
+):
     """Determine which turbines are within a certain radius of other
     wind turbines.
 
     Args:
         x_turbs ([list, array]): Long. locations of turbines
         y_turbs ([list, array]): Lat. locations of turbines
         turb_no ([int]): Turbine number for which the distance is
@@ -502,33 +516,133 @@
         according to distance to the turbine, from closest to furthest (but
         still within radius). Defaults to False.
 
     Returns:
         turbs_within_radius ([list]): List of turbines that are within the
         prespecified distance from turbine [turb_no].
     """
-    dr_turb = np.sqrt((x_turbs - x_turbs[turb_no])**2.0 +
-                      (y_turbs - y_turbs[turb_no])**2.0)
+    dr_turb = np.sqrt((x_turbs - x_turbs[turb_no]) ** 2.0 + (y_turbs - y_turbs[turb_no]) ** 2.0)
     turbine_list = np.array(range(len(x_turbs)))
 
     if sort_by_distance:
         indices_sorted = np.argsort(dr_turb)
         dr_turb = dr_turb[indices_sorted]
         turbine_list = turbine_list[indices_sorted]
 
     turbs_within_radius = turbine_list[dr_turb <= max_radius]
     if not include_itself:
-        turbs_within_radius = [ti for ti in turbs_within_radius
-                               if not ti == turb_no]
+        turbs_within_radius = [ti for ti in turbs_within_radius if not ti == turb_no]
 
     return turbs_within_radius
 
 
-def get_upstream_turbs_floris(fi, wd_step=0.1, wake_slope=0.10,
-                              plot_lines=False):
+def get_all_impacting_turbines_geometrical(
+    fm, turbine_weights, wd_array=np.arange(0.0, 360.0, 3.0), wake_slope=0.30
+):
+    """Determine which turbines affect the turbines of interest
+    (i.e., those with a turbine_weights > 0.00001). This function
+    uses very simplified geometric functions to very quickly
+    derive which turbines are supposedly waking at least one
+    turbine in the farm of interest.
+
+    Args:
+        fm ([floris object]): FLORIS object of the farm of interest.
+        turbine_weights [list]: List of with turbine weights with length
+        equal to the number of wind turbines, and typically filled with
+        0s (neighbouring farms) and 1s (farm of interest).
+        wd_step (float, optional): Wind direction discretization step.
+        Defaults to 3.0.
+        wake_slope (float, optional): linear slope of the wake (dy/dx)
+        plot_lines (bool, optional): Enable plotting wakes/turbines.
+        Defaults to False.
+
+    Returns:
+        df_impacting_simple ([pd.DataFrame]): A Pandas Dataframe in which each row
+        contains a wind direction and a list of turbine numbers. The turbine
+        numbers are those turbines that should be modelled to accurately
+        capture the wake losses for the wind farm of interest. Turbine numbers
+        that are not in the 'impacting_turbines' can safely be removed from
+        the simulation without affecting any of the turbines that have a nonzero
+        turbine weight.
+    """
+
+    # Get farm layout
+    x = fm.layout_x
+    y = fm.layout_y
+    n_turbs = len(x)
+    D = [t["rotor_diameter"] for t in fm.core.farm.turbine_definitions]
+    D = np.array(D, dtype=float)
+
+    # Rotate farm and determine freestream/waked turbines
+    is_impacting_list = []
+    for wd in wd_array:
+        is_impacting = [None for _ in range(n_turbs)]
+
+        # Rotate according to freestream wind direction
+        x_rot = np.cos((wd - 270.0) * np.pi / 180.0) * x - np.sin((wd - 270.0) * np.pi / 180.0) * y
+        y_rot = np.sin((wd - 270.0) * np.pi / 180.0) * x + np.cos((wd - 270.0) * np.pi / 180.0) * y
+
+        # Get turbine indices of the farm turbines of interest, and find its most downstream location
+        turb_ids_of_interest = np.where(turbine_weights > 0.0001)[0]
+        x_rot_most_downstream_of_interest = np.max(x_rot[turb_ids_of_interest])
+
+        # Check for each turbine
+        for ii in range(n_turbs):
+            # Check easy skips: turbine is in farm of interest
+            if ii in turb_ids_of_interest:
+                is_impacting[ii] = True
+                continue
+
+            # Check easy skips: further downstream than last turbine
+            if x_rot[ii] >= x_rot_most_downstream_of_interest:
+                is_impacting[ii] = False
+                continue
+
+            x0 = x_rot[ii]
+            y0 = y_rot[ii]
+
+            def yw_upper(x):
+                y = (y0 + D[ii]) + (x - x0) * wake_slope
+                if isinstance(y, (float, np.float64, np.float32)):
+                    if x < (x0 + 0.01):
+                        y = -np.Inf
+                else:
+                    y[x < x0 + 0.01] = -np.Inf
+                return y
+
+            def yw_lower(x):
+                y = (y0 - D[ii]) - (x - x0) * wake_slope
+                if isinstance(y, (float, np.float64, np.float32)):
+                    if x < (x0 + 0.01):
+                        y = -np.Inf
+                else:
+                    y[x < x0 + 0.01] = -np.Inf
+                return y
+
+            def is_in_wake(xt, yt):
+                return (yt < yw_upper(xt)) & (yt > yw_lower(xt))
+
+            is_impacting[ii] = any(
+                is_in_wake(x_rot[turb_ids_of_interest], y_rot[turb_ids_of_interest])
+            )
+
+        is_impacting_list.append(np.where(is_impacting)[0])
+
+    n_turbines_reduced = [len(ids) for ids in is_impacting_list]
+    df_impacting_simple = pd.DataFrame(
+        {
+            "wd": wd_array,
+            "impacting_turbines": is_impacting_list,
+            "n_turbines_reduced": n_turbines_reduced,
+        }
+    )
+    return df_impacting_simple
+
+
+def get_upstream_turbs_floris(fm, wd_step=0.1, wake_slope=0.10, plot_lines=False):
     """Determine which turbines are operating in freestream (unwaked)
     flow, for the entire wind rose. This function will return a data-
     frame where each row will present a wind direction range and a set
     of wind turbine numbers for which those turbines are operating
     upstream. This is useful in determining the freestream conditions.
 
     Args:
@@ -552,323 +666,355 @@
         noticably affect your outcomes. Empirically, this approach has
         yielded good results with real SCADA data for determining what
         turbines are waked/unwaked and has served useful for determining
         what turbines to use as reference.
     """
 
     # Get farm layout
-    x = fi.layout_x
-    y = fi.layout_y
+    x = fm.layout_x
+    y = fm.layout_y
     n_turbs = len(x)
-    D = [t["rotor_diameter"] for t in fi.floris.farm.turbine_definitions]
+    D = [t["rotor_diameter"] for t in fm.core.farm.turbine_definitions]
     D = np.array(D, dtype=float)
 
     # Setup output list
     upstream_turbs_ids = []  # turbine numbers that are freestream
     upstream_turbs_wds = []  # lower bound of bin
 
     # Rotate farm and determine freestream/waked turbines
-    for wd in np.arange(0., 360., wd_step):
+    for wd in np.arange(0.0, 360.0, wd_step):
         is_freestream = [True for _ in range(n_turbs)]
-        x_rot = (np.cos((wd-270.) * np.pi / 180.) * x -
-                 np.sin((wd-270.) * np.pi / 180.) * y)
-        y_rot = (np.sin((wd-270.) * np.pi / 180.) * x +
-                 np.cos((wd-270.) * np.pi / 180.) * y)
+        x_rot = np.cos((wd - 270.0) * np.pi / 180.0) * x - np.sin((wd - 270.0) * np.pi / 180.0) * y
+        y_rot = np.sin((wd - 270.0) * np.pi / 180.0) * x + np.cos((wd - 270.0) * np.pi / 180.0) * y
 
         if plot_lines:
             fig, ax = plt.subplots()
             for ii in range(n_turbs):
-                ax.plot(x_rot[ii] * np.ones(2), [y_rot[ii] - D[ii] / 2, y_rot[ii] + D[ii] / 2], 'k')
+                ax.plot(x_rot[ii] * np.ones(2), [y_rot[ii] - D[ii] / 2, y_rot[ii] + D[ii] / 2], "k")
             for ii in range(n_turbs):
-                ax.text(x_rot[ii], y_rot[ii], 'T%03d' % ii)
-            ax.axis('equal')
+                ax.text(x_rot[ii], y_rot[ii], "T%03d" % ii)
+            ax.axis("equal")
 
         srt = np.argsort(x_rot)
         x_rot_srt = x_rot[srt]
         y_rot_srt = y_rot[srt]
         for ii in range(n_turbs):
             x0 = x_rot_srt[ii]
             y0 = y_rot_srt[ii]
 
             def yw_upper(x):
-                y = (y0 + D[ii]) + (x-x0) * wake_slope
+                y = (y0 + D[ii]) + (x - x0) * wake_slope
                 if isinstance(y, (float, np.float64, np.float32)):
                     if x < (x0 + 0.01):
                         y = -np.Inf
                 else:
                     y[x < x0 + 0.01] = -np.Inf
                 return y
 
             def yw_lower(x):
-                y = (y0 - D[ii]) - (x-x0) * wake_slope
+                y = (y0 - D[ii]) - (x - x0) * wake_slope
                 if isinstance(y, (float, np.float64, np.float32)):
                     if x < (x0 + 0.01):
                         y = -np.Inf
                 else:
                     y[x < x0 + 0.01] = -np.Inf
                 return y
 
-            is_in_wake = lambda xt, yt: ((yt < yw_upper(xt)) &
-                                         (yt > yw_lower(xt)))
+            def is_in_wake(xt, yt):
+                return (yt < yw_upper(xt)) & (yt > yw_lower(xt))
 
-            is_freestream = (is_freestream &
-                             ~is_in_wake(x_rot_srt, y_rot_srt + D/2.) &
-                             ~is_in_wake(x_rot_srt, y_rot_srt - D/2.))
+            is_freestream = (
+                is_freestream
+                & ~is_in_wake(x_rot_srt, y_rot_srt + D / 2.0)
+                & ~is_in_wake(x_rot_srt, y_rot_srt - D / 2.0)
+            )
 
             if plot_lines:
-                x1 = np.max(x_rot_srt) + 500.
-                ax.fill_between([x0, x1, x1, x0],
-                                [yw_upper(x0+0.02), yw_upper(x1),
-                                 yw_lower(x1), yw_lower(x0+0.02)],
-                                alpha=0.1, color='k', edgecolor=None)
+                x1 = np.max(x_rot_srt) + 500.0
+                ax.fill_between(
+                    [x0, x1, x1, x0],
+                    [yw_upper(x0 + 0.02), yw_upper(x1), yw_lower(x1), yw_lower(x0 + 0.02)],
+                    alpha=0.1,
+                    color="k",
+                    edgecolor=None,
+                )
 
         usrt = np.argsort(srt)
         is_freestream = is_freestream[usrt]
         turbs_freestream = list(np.where(is_freestream)[0])
 
         if len(upstream_turbs_wds) == 0:
             upstream_turbs_ids.append(turbs_freestream)
             upstream_turbs_wds.append(wd)
-        elif not(turbs_freestream == upstream_turbs_ids[-1]):
+        elif not (turbs_freestream == upstream_turbs_ids[-1]):
             upstream_turbs_ids.append(turbs_freestream)
             upstream_turbs_wds.append(wd)
 
         if plot_lines:
-            ax.set_title('wd = %03d' % wd)
-            ax.set_xlim([np.min(x_rot)-500., x1])
-            ax.set_ylim([np.min(y_rot)-500., np.max(y_rot)+500.])
-            ax.plot(x_rot[turbs_freestream],
-                    y_rot[turbs_freestream],
-                    'o', color='green')
+            ax.set_title("wd = %03d" % wd)
+            ax.set_xlim([np.min(x_rot) - 500.0, x1])
+            ax.set_ylim([np.min(y_rot) - 500.0, np.max(y_rot) + 500.0])
+            ax.plot(x_rot[turbs_freestream], y_rot[turbs_freestream], "o", color="green")
 
     # # Connect at 360 degrees
     # if upstream_turbs_ids[0] == upstream_turbs_ids[-1]:
     #     upstream_turbs_wds.pop(0)
     #     upstream_turbs_ids.pop(0)
 
     # Go from list to bins for upstream_turbs_wds
-    upstream_turbs_wds = [[upstream_turbs_wds[i], upstream_turbs_wds[i+1]]
-                          for i in range(len(upstream_turbs_wds)-1)]
-    upstream_turbs_wds.append([upstream_turbs_wds[-1][-1], 360.])
-
-    df_upstream = pd.DataFrame({'wd_min': [wd[0] for wd in upstream_turbs_wds],
-                                'wd_max': [wd[1] for wd in upstream_turbs_wds],
-                                'turbines': upstream_turbs_ids})
+    upstream_turbs_wds = [
+        [upstream_turbs_wds[i], upstream_turbs_wds[i + 1]]
+        for i in range(len(upstream_turbs_wds) - 1)
+    ]
+    upstream_turbs_wds.append([upstream_turbs_wds[-1][-1], 360.0])
+
+    df_upstream = pd.DataFrame(
+        {
+            "wd_min": [wd[0] for wd in upstream_turbs_wds],
+            "wd_max": [wd[1] for wd in upstream_turbs_wds],
+            "turbines": upstream_turbs_ids,
+        }
+    )
 
     return df_upstream
 
-def get_dependent_turbines_by_wd(fi_in, test_turbine, 
-    wd_array=np.arange(0., 360., 2.), change_threshold=0.001, limit_number=None, 
-    ws_test=9., return_influence_magnitudes=False):
-    """
-    Computes all turbines that depend on the operation of a specified 
-    turbine (test_turbine) for each wind direction in wd_array, using 
-    the FLORIS model specified by fi_in to detect dependencies. 
+
+def get_dependent_turbines_by_wd(
+    fm_in,
+    test_turbine,
+    wd_array=np.arange(0.0, 360.0, 2.0),
+    change_threshold=0.001,
+    limit_number=None,
+    ws_test=9.0,
+    return_influence_magnitudes=False,
+):
+    """
+    Computes all turbines that depend on the operation of a specified
+    turbine (test_turbine) for each wind direction in wd_array, using
+    the FLORIS model specified by fm_in to detect dependencies.
 
     Args:
         fi ([floris object]): FLORIS object of the farm of interest.
         test_turbine ([int]): Turbine for which dependencies are found.
-        wd_array ([np.array]): Wind directions at which to determine 
+        wd_array ([np.array]): Wind directions at which to determine
             dependencies. Defaults to [0, 2, ... , 358].
-        change_threshold (float): Fractional change in power needed 
-            to denote a dependency. Defaults to 0. (any change in power 
+        change_threshold (float): Fractional change in power needed
+            to denote a dependency. Defaults to 0. (any change in power
             is marked as a dependency)
-        limit_number (int | NoneType): Number of turbines that a 
-            turbine can have as dependencies. If None, returns all 
+        limit_number (int | NoneType): Number of turbines that a
+            turbine can have as dependencies. If None, returns all
             turbines that depend on each turbine. Defaults to None.
-        ws_test (float): Wind speed at which FLORIS model is run to 
+        ws_test (float): Wind speed at which FLORIS model is run to
             determine dependencies.  Defaults to 9. m/s.
-        return_influence_magnitudes (Bool): Flag for whether to return 
-            an array containing the magnitude of the influence of the 
+        return_influence_magnitudes (Bool): Flag for whether to return
+            an array containing the magnitude of the influence of the
             test_turbine on all turbines.
-        
+
     Returns:
-        dep_indices_by_wd (list): A 2-dimensional list. Each element of 
-            the outer level list, which represents wind direction, 
-            contains a list of the turbines that depend on test_turbine 
-            for that wind direction. The second-level list may be empty 
-            if no turbine depends on the test_turbine for that wind 
+        dep_indices_by_wd (list): A 2-dimensional list. Each element of
+            the outer level list, which represents wind direction,
+            contains a list of the turbines that depend on test_turbine
+            for that wind direction. The second-level list may be empty
+            if no turbine depends on the test_turbine for that wind
             direciton (e.g., the turbine is in the back row).
-        all_influence_magnitudes ([np.array]): 2-D numpy array of 
-            influences of test_turbine on all other turbines, with size 
+        all_influence_magnitudes ([np.array]): 2-D numpy array of
+            influences of test_turbine on all other turbines, with size
             (number of wind directions) x (number of turbines). Returned
             only if return_influence_magnitudes is True.
     """
     # Copy fi to a local to not mess with incoming
-    fi = copy.deepcopy(fi_in)
-    
+    fm = copy.deepcopy(fm_in)
+
     # Compute the base power
-    fi.reinitialize(
-        wind_speeds=[ws_test], 
-        wind_directions=wd_array
-    )
-    fi.calculate_wake()
-    base_power = fi.get_turbine_powers()[:,0,:] # remove unneeded dimension
-    
+    fm.set(
+        wind_data=TimeSeries(
+            wind_directions=wd_array, wind_speeds=ws_test, turbulence_intensities=0.06
+        )
+    )
+    fm.run()
+    base_power = fm.get_turbine_powers()
+
     # Compute the test power
-    if len(fi.floris.farm.turbine_type) > 1:
+    if len(fm.core.farm.turbine_type) > 1:
         # Remove test turbine from list
-        fi.floris.farm.turbine_type.pop(test_turbine) 
-    else: # Only a single turbine type defined for the whole farm; do nothing
+        fm.core.farm.turbine_type.pop(test_turbine)
+    else:  # Only a single turbine type defined for the whole farm; do nothing
         pass
-    fi.reinitialize(
-        layout_x=np.delete(fi.layout_x, [test_turbine]),
-        layout_y=np.delete(fi.layout_y, [test_turbine]),
-        wind_speeds=[ws_test],
-        wind_directions=wd_array
-    ) # This will reindex the turbines; undone in following steps.
-    fi.calculate_wake()
-    test_power = fi.get_turbine_powers()[:,0,:] # remove unneeded dimension
-    test_power = np.insert(test_power, test_turbine, 
-        base_power[:,test_turbine], axis=1)
+    fm.set(
+        layout_x=np.delete(fm.layout_x, [test_turbine]),
+        layout_y=np.delete(fm.layout_y, [test_turbine]),
+        wind_speeds=ws_test * np.ones_like(wd_array),
+        wind_directions=wd_array,
+    )  # This will reindex the turbines; undone in following steps.
+    fm.run()
+    test_power = fm.get_turbine_powers()
+    test_power = np.insert(test_power, test_turbine, base_power[:, test_turbine], axis=1)
 
     if return_influence_magnitudes:
         all_influence_magnitudes = np.zeros_like(test_power)
-    
+
     # Find the indices that have changed
-    dep_indices_by_wd = [None]*len(wd_array)
+    dep_indices_by_wd = [None] * len(wd_array)
     for i in range(len(wd_array)):
-        all_influences = np.abs(test_power[i,:] - base_power[i,:])/\
-                         base_power[i,:]
+        all_influences = np.abs(test_power[i, :] - base_power[i, :]) / base_power[i, :]
         # Sort with highest influence first; trim to limit_number
         influence_order = np.flip(np.argsort(all_influences))[:limit_number]
         # Mask to only those that meet the threshold
-        influence_order = influence_order[
-            all_influences[influence_order] >= change_threshold
-        ]
-        
+        influence_order = influence_order[all_influences[influence_order] >= change_threshold]
+
         # Store in output
         dep_indices_by_wd[i] = list(influence_order)
         if return_influence_magnitudes:
-            all_influence_magnitudes[i,:] = all_influences
-    
+            all_influence_magnitudes[i, :] = all_influences
 
     # Remove the turbines own indice
     if return_influence_magnitudes:
         return dep_indices_by_wd, all_influence_magnitudes
     else:
         return dep_indices_by_wd
 
-def get_all_dependent_turbines(fi_in, wd_array=np.arange(0., 360., 2.), 
-    change_threshold=0.001, limit_number=None, ws_test=9.):
+
+def get_all_dependent_turbines(
+    fm_in,
+    wd_array=np.arange(0.0, 360.0, 2.0),
+    change_threshold=0.001,
+    limit_number=None,
+    ws_test=9.0,
+):
     """
-    Wrapper for get_dependent_turbines_by_wd() that loops over all 
-    turbines in the farm and packages their dependencies as a pandas 
+    Wrapper for get_dependent_turbines_by_wd() that loops over all
+    turbines in the farm and packages their dependencies as a pandas
     dataframe.
 
     Args:
         fi ([floris object]): FLORIS object of the farm of interest.
-        wd_array ([np.array]): Wind directions at which to determine 
+        wd_array ([np.array]): Wind directions at which to determine
             dependencies. Defaults to [0, 2, ... , 358].
-        change_threshold (float): Fractional change in power needed 
-            to denote a dependency. Defaults to 0. (any change in power 
+        change_threshold (float): Fractional change in power needed
+            to denote a dependency. Defaults to 0. (any change in power
             is marked as a dependency)
-        limit_number (int | NoneType): Number of turbines that a 
-            turbine can have as dependencies. If None, returns all 
+        limit_number (int | NoneType): Number of turbines that a
+            turbine can have as dependencies. If None, returns all
             turbines that depend on each turbine. Defaults to None.
-        ws_test (float): Wind speed at which FLORIS model is run to 
+        ws_test (float): Wind speed at which FLORIS model is run to
             determine dependencies. Defaults to 9. m/s.
-        
+
     Returns:
         df_out ([pd.DataFrame]): A Pandas Dataframe in which each row
-            contains a wind direction, each column is a turbine, and 
-            each entry is the turbines that depend on the column turbine 
-            at the row wind direction. Dependencies can be extracted 
-            as: For wind direction wd, the turbines that depend on 
-            turbine T are df_out.loc[wd, T]. Dependencies are ordered, 
+            contains a wind direction, each column is a turbine, and
+            each entry is the turbines that depend on the column turbine
+            at the row wind direction. Dependencies can be extracted
+            as: For wind direction wd, the turbines that depend on
+            turbine T are df_out.loc[wd, T]. Dependencies are ordered,
             with strongest dependencies appearing first.
     """
 
     results = []
-    for t_i in range(len(fi_in.layout_x)):
+    for t_i in range(len(fm_in.layout_x)):
         results.append(
             get_dependent_turbines_by_wd(
-                fi_in, t_i, wd_array, change_threshold, limit_number, ws_test
+                fm_in, t_i, wd_array, change_threshold, limit_number, ws_test
             )
         )
-    
-    df_out = (pd.DataFrame(data=results, columns=wd_array)
-              .transpose()
-              .reset_index().rename(columns={"index":"wd"}).set_index("wd")
-             )
-    
+
+    df_out = (
+        pd.DataFrame(data=results, columns=wd_array)
+        .transpose()
+        .reset_index()
+        .rename(columns={"index": "wd"})
+        .set_index("wd")
+    )
+
     return df_out
 
-def get_all_impacting_turbines(fi_in, wd_array=np.arange(0., 360., 2.), 
-    change_threshold=0.001, limit_number=None, ws_test=9.):
+
+def get_all_impacting_turbines(
+    fm_in,
+    wd_array=np.arange(0.0, 360.0, 2.0),
+    change_threshold=0.001,
+    limit_number=None,
+    ws_test=9.0,
+):
     """
-    Calculate which turbines impact a specified turbine based on the 
-    FLORIS model. Essentially a wrapper for 
-    get_dependent_turbines_by_wd() that loops over all turbines and 
+    Calculate which turbines impact a specified turbine based on the
+    FLORIS model. Essentially a wrapper for
+    get_dependent_turbines_by_wd() that loops over all turbines and
     extracts their impact magnitudes, then sorts.
 
     Args:
         fi ([floris object]): FLORIS object of the farm of interest.
-        wd_array ([np.array]): Wind directions at which to determine 
+        wd_array ([np.array]): Wind directions at which to determine
             dependencies. Defaults to [0, 2, ... , 358].
-        change_threshold (float): Fractional change in power needed 
-            to denote a dependency. Defaults to 0. (any change in power 
+        change_threshold (float): Fractional change in power needed
+            to denote a dependency. Defaults to 0. (any change in power
             is marked as a dependency)
-        limit_number (int | NoneType): Number of turbines that a 
-            turbine can depend on. If None, returns all 
+        limit_number (int | NoneType): Number of turbines that a
+            turbine can depend on. If None, returns all
             turbines that each turbine depends on. Defaults to None.
-        ws_test (float): Wind speed at which FLORIS model is run to 
+        ws_test (float): Wind speed at which FLORIS model is run to
             determine dependencies. Defaults to 9. m/s.
 
     Returns:
         df_out ([pd.DataFrame]): A Pandas Dataframe in which each row
-            contains a wind direction, each column is a turbine, and 
-            each entry is the turbines that the column turbine depends 
-            on at the row wind direction. Dependencies can be extracted 
-            as: For wind direction wd, the turbines that impact turbine 
-            T are df_out.loc[wd, T]. Impacting turbines are simply 
+            contains a wind direction, each column is a turbine, and
+            each entry is the turbines that the column turbine depends
+            on at the row wind direction. Dependencies can be extracted
+            as: For wind direction wd, the turbines that impact turbine
+            T are df_out.loc[wd, T]. Impacting turbines are simply
             ordered by magnitude of impact.
     """
 
-    dependency_magnitudes = np.zeros(
-        (len(wd_array),len(fi_in.layout_x),len(fi_in.layout_x))
-    )
-    
-    for t_i in range(len(fi_in.layout_x)):
+    dependency_magnitudes = np.zeros((len(wd_array), len(fm_in.layout_x), len(fm_in.layout_x)))
+
+    for t_i in range(len(fm_in.layout_x)):
         _, ti_dep_mags = get_dependent_turbines_by_wd(
-                fi_in, t_i, wd_array, change_threshold, limit_number, ws_test,
-                return_influence_magnitudes=True
-            )
-        dependency_magnitudes[:,:,t_i] = ti_dep_mags
-    
+            fm_in,
+            t_i,
+            wd_array,
+            change_threshold,
+            limit_number,
+            ws_test,
+            return_influence_magnitudes=True,
+        )
+        dependency_magnitudes[:, :, t_i] = ti_dep_mags
+
     # Sort
     impact_order = np.flip(np.argsort(dependency_magnitudes, axis=2), axis=2)
 
     # Truncate to limit_number
-    impact_order = impact_order[:,:,:limit_number]
+    impact_order = impact_order[:, :, :limit_number]
 
     # Build up multi-level results list
     results = []
 
     for wd in range(len(wd_array)):
         wd_results = []
-        for t_j in range(len(fi_in.layout_x)):
+        for t_j in range(len(fm_in.layout_x)):
             impacts_on_t_j = dependency_magnitudes[wd, t_j, :]
             impact_order_t_j = impact_order[wd, t_j, :]
             impact_order_t_j = impact_order_t_j[
                 impacts_on_t_j[impact_order_t_j] >= change_threshold
             ]
             wd_results.append(list(impact_order_t_j))
         results.append(wd_results)
 
     # Convert to dataframe
-    df_out = (pd.DataFrame(data=results, index=wd_array)
-            .reset_index().rename(columns={"index":"wd"}).set_index("wd")
-            )
+    df_out = (
+        pd.DataFrame(data=results, index=wd_array)
+        .reset_index()
+        .rename(columns={"index": "wd"})
+        .set_index("wd")
+    )
 
     return df_out
 
+
 # Wrapper function to easily set new TI values
-def _fi_set_ws_wd_ti(fi, wd=None, ws=None, ti=None):
-    nturbs = len(fi.layout_x)
+def _fi_set_ws_wd_ti(fm, wd=None, ws=None, ti=None):
+    nturbs = len(fm.layout_x)
 
     # Convert scalar values to lists
     if not isinstance(wd, list):
         if isinstance(wd, np.ndarray):
             wd = list(wd)
         elif wd is not None:
             wd = list(np.repeat(wd, nturbs))
@@ -879,16 +1025,13 @@
             ws = list(np.repeat(ws, nturbs))
     if not isinstance(ti, list):
         if isinstance(ti, np.ndarray):
             ti = list(ti)
         elif ti is not None:
             ti = list(np.repeat(ti, nturbs))
 
-    wind_layout = (np.array(fi.layout_x), np.array(fi.layout_y))
+    wind_layout = (np.array(fm.layout_x), np.array(fm.layout_y))
 
-    fi.reinitialize_flow_field(
-        wind_layout=wind_layout,
-        wind_direction=wd,
-        wind_speed=ws,
-        turbulence_intensity=ti
+    fm.reinitialize_flow_field(
+        wind_layout=wind_layout, wind_direction=wd, wind_speed=ws, turbulence_intensity=ti
     )
-    return fi
+    return fm
```

### Comparing `flasc-1.4.2/flasc/model_estimation/floris_sensitivity_analysis.py` & `flasc-2.0/flasc/model_fitting/floris_sensitivity_analysis.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,253 +1,254 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-
-from SALib.sample import saltelli
+from pandas.errors import DataError
 from SALib.analyze import sobol
+from SALib.sample import saltelli
 
-from pandas.errors import DataError
+from flasc.logging_manager import LoggingManager
+from flasc.utilities import floris_tools as ftools
 
-from .. import floris_tools as ftools
+logger_manager = LoggingManager()  # Instantiate LoggingManager
+logger = logger_manager.logger  # Obtain the reusable logger
 
-class floris_sobol_analysis():
+
+class floris_sobol_analysis:
     def __init__(self, fi, problem, calc_second_order=False):
-        self.fi = fi
+        self.fm = fi
 
         # Default parameters
         self.param_dict = {
-                      'ad': 0.0,
-                      'alpha': 0.58,
-                      'bd': 0.0,
-                      'beta': 0.077,
-                      'eps_gain': 0.20,
-                      'ka': 0.38,
-                      'kb': 0.004,
-                      'ti_ai': 0.80,
-                      'ti_constant': 0.50,
-                      'ti_downstream': -0.32,
-                      'ti_initial': 0.10
-                      }
+            "ad": 0.0,
+            "alpha": 0.58,
+            "bd": 0.0,
+            "beta": 0.077,
+            "eps_gain": 0.20,
+            "ka": 0.38,
+            "kb": 0.004,
+            "ti_ai": 0.80,
+            "ti_constant": 0.50,
+            "ti_downstream": -0.32,
+            "ti_initial": 0.10,
+        }
 
         self.problem = problem
         self.Si = None
         self.calc_second_order = calc_second_order
         self.samples_x = None
         self.samples_y = None
         self.N = None
 
     def _get_model_params_dict(self, id):
         new_params_dict = {}
-        n_params = len(self.problem['names'])
+        n_params = len(self.problem["names"])
         for i in range(n_params):
-            var_name = self.problem['names'][i]
+            var_name = self.problem["names"][i]
             value = self.samples_x[id, i]
             new_params_dict[var_name] = value
 
         keys = list(new_params_dict.keys())
         values = list(new_params_dict.values())
         for i in range(len(keys)):
             self.param_dict[keys[i]] = values[i]
 
         params = {
-            "Wake Deflection Parameters":
-                {"ad": self.param_dict['ad'],
-                 "alpha": self.param_dict['alpha'],
-                 "bd": self.param_dict['bd'],
-                 "beta": self.param_dict['beta'],
-                 "eps_gain": self.param_dict['eps_gain'],
-                 "ka": self.param_dict['ka'],
-                 "kb": self.param_dict['kb'],
-                 "use_secondary_steering": True},
-            "Wake Turbulence Parameters":
-                {"ti_ai": self.param_dict['ti_ai'],
-                 "ti_constant": self.param_dict['ti_constant'],
-                 "ti_downstream": self.param_dict['ti_downstream'],
-                 "ti_initial": self.param_dict['ti_initial']},
-            "Wake Velocity Parameters":
-                {"alpha": self.param_dict['alpha'],
-                 "beta": self.param_dict['beta'],
-                 "eps_gain": self.param_dict['eps_gain'],
-                 "ka": self.param_dict['ka'],
-                 "kb": self.param_dict['kb'],
-                 "use_yaw_added_recovery": True}
+            "Wake Deflection Parameters": {
+                "ad": self.param_dict["ad"],
+                "alpha": self.param_dict["alpha"],
+                "bd": self.param_dict["bd"],
+                "beta": self.param_dict["beta"],
+                "eps_gain": self.param_dict["eps_gain"],
+                "ka": self.param_dict["ka"],
+                "kb": self.param_dict["kb"],
+                "use_secondary_steering": True,
+            },
+            "Wake Turbulence Parameters": {
+                "ti_ai": self.param_dict["ti_ai"],
+                "ti_constant": self.param_dict["ti_constant"],
+                "ti_downstream": self.param_dict["ti_downstream"],
+                "ti_initial": self.param_dict["ti_initial"],
+            },
+            "Wake Velocity Parameters": {
+                "alpha": self.param_dict["alpha"],
+                "beta": self.param_dict["beta"],
+                "eps_gain": self.param_dict["eps_gain"],
+                "ka": self.param_dict["ka"],
+                "kb": self.param_dict["kb"],
+                "use_yaw_added_recovery": True,
+            },
         }
 
         return params
-        # self.fi.set_model_parameters(params=params, verbose=False)
+        # self.fm.set_model_parameters(params=params, verbose=False)
 
     def _create_evals_dataframe(self):
         Nt = self.samples_x.shape[0]
         params_array = [[] for _ in range(Nt)]
         for id in range(Nt):
             params_array[id] = self._get_model_params_dict(id)
-        df = pd.DataFrame({'model_params_dict': params_array})
+        df = pd.DataFrame({"model_params_dict": params_array})
         self.df_eval = df
 
     # Step 1: generating samples for a particular problem
     def generate_samples(self, N, problem=None, calc_second_order=None):
         if problem is None:
             problem = self.problem
 
         if calc_second_order is None:
             calc_second_order = self.calc_second_order
         self.problem = problem
         self.calc_second_order = calc_second_order
 
         Ns = N
-        self.samples_x = saltelli.sample(
-            problem, Ns, calc_second_order=calc_second_order)
+        self.samples_x = saltelli.sample(problem, Ns, calc_second_order=calc_second_order)
 
         self.N = self.samples_x.shape[0]
         self.samples_y = np.zeros(self.N)
         self._create_evals_dataframe()
 
     def calculate_wfpower_for_samples(self, num_threads=1):
         if self.samples_x is None:
-            raise DataError('Please run generate_samples first.')
+            raise DataError("Please run generate_samples first.")
 
         # Copy and write wd and ws to dataframe
         # Nt = self.df_eval.shape[0]
         df = self.df_eval
-        df['wd'] = self.fi.floris.farm.wind_direction[0]
-        df['ws'] = self.fi.floris.farm.wind_speed[0]
+        df["wd"] = self.fm.core.farm.wind_direction[0]
+        df["ws"] = self.fm.core.farm.wind_speed[0]
 
         # Calculate floris predictions
         df_out = ftools.calc_floris(df, self.fi, num_threads=10, num_workers=2)
-        pow_cols = ['pow_%03d' % ti for ti in range(len(self.fi.layout_x))]
+        pow_cols = ["pow_%03d" % ti for ti in range(len(self.fm.layout_x))]
         self.samples_y = np.array(df_out[pow_cols].sum(axis=1), dtype=float)
 
         return self.samples_y
 
-    # def calculate_aep_for_samples(self, wd, ws, freq):
-    #     if self.samples_x is None:
-    #         raise DataError('Please run generate_samples first.')
-
-    #     print('Calculating AEP for %d samples.' % self.N)
-    #     for i in range(self.N):
-    #         self._set_fi_by_sample_id(i)
-    #         aep = self.fi.get_farm_AEP(wd=wd, ws=ws, freq=freq)
-    #         self.samples_y[i] = aep
-
-    #     return self.samples_y
-
     def get_sobol_sensitivity_indices(self, verbose=False):
-        self.Si = sobol.analyze(self.problem, self.samples_y,
-                                print_to_console=verbose,
-                                calc_second_order=self.calc_second_order)
+        self.Si = sobol.analyze(
+            self.problem,
+            self.samples_y,
+            print_to_console=verbose,
+            calc_second_order=self.calc_second_order,
+        )
         return self.Si
 
-    def plot_sobol_results(self, save_path=None, fig_format='png', fig_dpi=200):
+    def plot_sobol_results(self, save_path=None, fig_format="png", fig_dpi=200):
         if self.Si is None:
-            raise DataError('No Sobol results to show. ' +
-                            'Have you run get_sobol_sensitivity_indices()?')
+            raise DataError(
+                "No Sobol results to show. " + "Have you run get_sobol_sensitivity_indices()?"
+            )
         problem = self.problem
         if self.calc_second_order:
             fig, ax = plt.subplots(2)
         else:
             fig, ax = plt.subplots()
             ax = [ax]
         width = 0.30
-        Nv = problem['num_vars']
+        Nv = problem["num_vars"]
 
         # Plot first order sensitivity plus uncertainties
-        bar1 = ax[0].bar(np.arange(Nv) - width/2, self.Si['S1'], width=0.3,
-                         align='center', label='First order sensitivity',
-                         color='deepskyblue', edgecolor='black', hatch='//')
+        _ = ax[0].bar(
+            np.arange(Nv) - width / 2,
+            self.Si["S1"],
+            width=0.3,
+            align="center",
+            label="First order sensitivity",
+            color="deepskyblue",
+            edgecolor="black",
+            hatch="//",
+        )
         # ax[0].bar_label(bar1, padding=7, fmt='%.1e')
 
         for i in range(Nv):
-            ymean = self.Si['S1'][i]
-            ystd = self.Si['S1_conf'][i]
-            ax[0].plot(np.repeat(i - width/2, 3),
-                       ymean + np.array([-ystd, 0., ystd]),
-                       color='black')
-            ax[0].plot(i - width/2, ymean, 'o', color='black')
-            ax[0].plot([i - 0.75*width, i-0.25*width],
-                       [ymean-ystd, ymean-ystd], color='black')
-            ax[0].plot([i - 0.75*width, i-0.25*width],
-                       [ymean+ystd, ymean+ystd], color='black')
+            ymean = self.Si["S1"][i]
+            ystd = self.Si["S1_conf"][i]
+            ax[0].plot(
+                np.repeat(i - width / 2, 3), ymean + np.array([-ystd, 0.0, ystd]), color="black"
+            )
+            ax[0].plot(i - width / 2, ymean, "o", color="black")
+            ax[0].plot(
+                [i - 0.75 * width, i - 0.25 * width], [ymean - ystd, ymean - ystd], color="black"
+            )
+            ax[0].plot(
+                [i - 0.75 * width, i - 0.25 * width], [ymean + ystd, ymean + ystd], color="black"
+            )
 
         # Plot total sensitivity including uncertainties
-        bar2 = ax[0].bar(np.arange(Nv) + width/2, self.Si['ST'], width=0.3,
-                         align='center', label='Total sensitivity',
-                         color='orangered', edgecolor='black', hatch='.')
+        _ = ax[0].bar(
+            np.arange(Nv) + width / 2,
+            self.Si["ST"],
+            width=0.3,
+            align="center",
+            label="Total sensitivity",
+            color="orangered",
+            edgecolor="black",
+            hatch=".",
+        )
         # ax[0].bar_label(bar2, padding=7, fmt='%.1e')
 
         for i in range(Nv):
-            ymean = self.Si['ST'][i]
-            ystd = self.Si['ST_conf'][i]
-            ax[0].plot(np.repeat(i + width/2, 3),
-                       ymean + np.array([-ystd, 0., ystd]),
-                       color='black')
-            ax[0].plot(i + width/2, ymean, 'o', color='black')
-            ax[0].plot([i + 0.25*width, i+0.75*width],
-                       [ymean-ystd, ymean-ystd], color='black')
-            ax[0].plot([i + 0.25*width, i+0.75*width],
-                       [ymean+ystd, ymean+ystd], color='black')
+            ymean = self.Si["ST"][i]
+            ystd = self.Si["ST_conf"][i]
+            ax[0].plot(
+                np.repeat(i + width / 2, 3), ymean + np.array([-ystd, 0.0, ystd]), color="black"
+            )
+            ax[0].plot(i + width / 2, ymean, "o", color="black")
+            ax[0].plot(
+                [i + 0.25 * width, i + 0.75 * width], [ymean - ystd, ymean - ystd], color="black"
+            )
+            ax[0].plot(
+                [i + 0.25 * width, i + 0.75 * width], [ymean + ystd, ymean + ystd], color="black"
+            )
 
         # Plot settings
         ax[0].set_xticks(range(Nv))
-        ax[0].set_xticklabels(problem['names'])
-        ax[0].set_title('First order effects')
-        ax[0].set_ylabel('Sensitivity (-)')
+        ax[0].set_xticklabels(problem["names"])
+        ax[0].set_title("First order effects")
+        ax[0].set_ylabel("Sensitivity (-)")
         ax[0].legend()
-        ax[0].grid('minor')
+        ax[0].grid("minor")
         ax[0].set_ylim([0, 1.1])
 
         # Second order tabular/imshow plot, if calculated
         if self.calc_second_order:
-            im = ax[1].imshow(self.Si['S2'][:-1,:])
+            im = ax[1].imshow(self.Si["S2"][:-1, :])
             ax[1].set_xticks(range(Nv))
-            ax[1].set_yticks(range(Nv-1))
-            ax[1].set_xticklabels(self.problem['names'])
-            ax[1].set_yticklabels(self.problem['names'][:-1])
-            ax[1].set_title('Second order effects')
-            for ii in range(Nv-1):
+            ax[1].set_yticks(range(Nv - 1))
+            ax[1].set_xticklabels(self.problem["names"])
+            ax[1].set_yticklabels(self.problem["names"][:-1])
+            ax[1].set_title("Second order effects")
+            for ii in range(Nv - 1):
                 for jj in range(Nv):
-                    ax[1].text(y=ii, x=jj,
-                               s='%.3e' % self.Si['S2'][ii, jj],
-                               ha='center', color='white')
+                    ax[1].text(
+                        y=ii, x=jj, s="%.3e" % self.Si["S2"][ii, jj], ha="center", color="white"
+                    )
             plt.copper()
             plt.colorbar(im, ax=ax[1])
             fig.tight_layout()
 
             if save_path is not None:
-                plt.savefig(save_path + '/Sobol_sensitivity_indices.%s'
-                            % fig_format, dpi=fig_dpi)
+                plt.savefig(save_path + "/Sobol_sensitivity_indices.%s" % fig_format, dpi=fig_dpi)
 
         return fig, ax
 
-    def plot_convergence(self, save_path=None, fig_format='png', fig_dpi=200):
-        print('Analyzing convergence...')
+    def plot_convergence(self, save_path=None, fig_format="png", fig_dpi=200):
+        logger.info("Analyzing convergence...")
 
         # Create copies of original results
         samples_x_full = self.samples_x
         samples_y_full = self.samples_y
         Si_full = self.Si
         N = self.N
 
         # Create Sobol outputs for data subsets
         Si_list = []
         self.generate_samples(N=10)
         dN = self.samples_x.shape[0]
-        N_array = np.arange(dN, N, dN, dtype='int')
+        N_array = np.arange(dN, N, dN, dtype="int")
         if N_array[-1] < N:
             N_array = np.append(N_array, N)
 
         for n in N_array:
             self.samples_y = samples_y_full[0:n]
             self.get_sobol_sensitivity_indices(verbose=False)
             Si_list.append(self.Si)
@@ -255,56 +256,66 @@
         # Restore original results
         self.samples_x = samples_x_full
         self.samples_y = samples_y_full
         self.Si = Si_full
         self.N = N
 
         # Plot convergence for S1
-        Nv = self.problem['num_vars']
+        Nv = self.problem["num_vars"]
         fig, ax = plt.subplots(nrows=Nv, sharex=True)
         for i in range(Nv):
-            ax[i].errorbar(x=N_array, y=[S['S1'][i] for S in Si_list],
-                           yerr=[S['S1_conf'][i] for S in Si_list],
-                           label='First order sensitivity (S1)')
-            ax[i].errorbar(x=N_array, y=[S['ST'][i] for S in Si_list],
-                           yerr=[S['ST_conf'][i] for S in Si_list],
-                           label='Total sensitivity (ST)')
-            ax[i].plot([0, self.N], [self.Si['S1'][i], self.Si['S1'][i]],
-                       '--', color='gray', label=None)
-            ax[i].plot([0, self.N], [self.Si['ST'][i], self.Si['ST'][i]],
-                       '--', color='gray', label=None)
+            ax[i].errorbar(
+                x=N_array,
+                y=[S["S1"][i] for S in Si_list],
+                yerr=[S["S1_conf"][i] for S in Si_list],
+                label="First order sensitivity (S1)",
+            )
+            ax[i].errorbar(
+                x=N_array,
+                y=[S["ST"][i] for S in Si_list],
+                yerr=[S["ST_conf"][i] for S in Si_list],
+                label="Total sensitivity (ST)",
+            )
+            ax[i].plot(
+                [0, self.N], [self.Si["S1"][i], self.Si["S1"][i]], "--", color="gray", label=None
+            )
+            ax[i].plot(
+                [0, self.N], [self.Si["ST"][i], self.Si["ST"][i]], "--", color="gray", label=None
+            )
             ax[i].legend()
-            ax[i].grid('minor')
-            ax[i].set_ylabel(self.problem['names'][i])
-            ax[i].set_xlabel('Number of iterations')
+            ax[i].grid("minor")
+            ax[i].set_ylabel(self.problem["names"][i])
+            ax[i].set_xlabel("Number of iterations")
 
         if save_path is not None:
-            plt.savefig(save_path + '/Sobol_convergence_order1.%s'
-                        % fig_format, dpi=fig_dpi)
+            plt.savefig(save_path + "/Sobol_convergence_order1.%s" % fig_format, dpi=fig_dpi)
 
         if self.calc_second_order:
-            for i in range(Nv-1):
-                for j in range(i+1, Nv):
+            for i in range(Nv - 1):
+                for j in range(i + 1, Nv):
                     fig, ax = plt.subplots()
                     ax.errorbar(
                         x=N_array,
-                        y=[S['S2'][i, j] for S in Si_list],
-                        yerr=[S['S2_conf'][i, j] for S in Si_list],
-                        label=('Second order sensitivity with %s'
-                               % self.problem['names'][j])
-                        )
+                        y=[S["S2"][i, j] for S in Si_list],
+                        yerr=[S["S2_conf"][i, j] for S in Si_list],
+                        label=("Second order sensitivity with %s" % self.problem["names"][j]),
+                    )
                     ax.plot(
                         [0, self.N],
-                        [self.Si['S2'][i, j], self.Si['S2'][i, j]],
-                        '--', color='black', label=None
-                        )
+                        [self.Si["S2"][i, j], self.Si["S2"][i, j]],
+                        "--",
+                        color="black",
+                        label=None,
+                    )
                     ax.legend()
-                    ax.set_ylabel(self.problem['names'][i])
-                    ax.set_xlabel('Number of iterations')
-                    ax.grid('minor')
+                    ax.set_ylabel(self.problem["names"][i])
+                    ax.set_xlabel("Number of iterations")
+                    ax.grid("minor")
                     if save_path is not None:
                         plt.savefig(
-                            save_path + '/Sobol_convergence_order2_%s.%s'
-                            % (self.problem['names'][j], fig_format),
-                            dpi=fig_dpi)
+                            save_path
+                            + "/Sobol_convergence_order2_%s.%s"
+                            % (self.problem["names"][j], fig_format),
+                            dpi=fig_dpi,
+                        )
 
         return fig, ax
```

### Comparing `flasc-1.4.2/flasc/model_estimation/turbulence_estimator.py` & `flasc-2.0/flasc/model_fitting/turbulence_estimator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,23 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-
-import floris.tools as wfct
+import floris as wfct
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
-from .. import floris_tools as ftools, optimization as opt
+from flasc.logging_manager import LoggingManager
+from flasc.utilities import floris_tools as ftools, optimization as opt
 
+logger_manager = LoggingManager()  # Instantiate LoggingManager
+logger = logger_manager.logger  # Obtain the reusable logger
 
-class ti_estimator():
-    def __init__(self, fi):
-        self.fi = fi
-        self.num_turbs = len(fi.layout_x)
+
+class ti_estimator:
+    def __init__(self, fm):
+        self.fm = fm
+        self.num_turbs = len(fm.layout_x)
 
         self._reset_outputs()
 
     def _reset_outputs(self):
         self.opt_farm = None
         self.opt_turbines = None
         self.turbine_list_ordered = None
@@ -39,160 +30,159 @@
         if isinstance(P_measured, list):
             P_measured = np.array(P_measured)
 
         self._reset_outputs()
         self.P_measured = P_measured
 
     def get_turbine_order(self):
-        wd = (180 - self.fi.floris.farm.wind_direction[0]) * np.pi / 180.
-        rotz = np.matrix([[np.cos(wd), -np.sin(wd), 0],
-                          [np.sin(wd), np.cos(wd), 0],
-                          [0, 0, 1]])
-        x0 = np.mean(self.fi.layout_x)
-        y0 = np.mean(self.fi.layout_y)
-
-        xyz_init = np.matrix([np.array(self.fi.layout_x) - x0,
-                              np.array(self.fi.layout_y) - y0,
-                              [0. for _ in range(self.num_turbs)]])
+        wd = (180 - self.fm.core.farm.wind_direction[0]) * np.pi / 180.0
+        rotz = np.matrix([[np.cos(wd), -np.sin(wd), 0], [np.sin(wd), np.cos(wd), 0], [0, 0, 1]])
+        x0 = np.mean(self.fm.layout_x)
+        y0 = np.mean(self.fm.layout_y)
+
+        xyz_init = np.matrix(
+            [
+                np.array(self.fm.layout_x) - x0,
+                np.array(self.fm.layout_y) - y0,
+                [0.0 for _ in range(self.num_turbs)],
+            ]
+        )
 
         xyz_rot = rotz * xyz_init
         x_rot = np.array(xyz_rot[0, :])[0]
         turbine_list_ordered = np.argsort(x_rot)
 
         self.turbine_list_ordered = turbine_list_ordered
         return turbine_list_ordered
 
     def get_turbine_pairs(self, wake_loss_thrs=0.20):
-        fi = self.fi
-        fi.calculate_wake()
-        power_baseline = np.array(fi.get_turbine_power())
-        disabled_turb_cp_ct = {'wind_speed': [0., 50.],
-                               'power': [0., 0.],
-                               'thrust': [0.0001, 0.0001]}
-        regular_turb_cp_ct = fi.floris.farm.turbines[0].power_thrust_table
+        fm = self.fi
+        fm.run()
+        power_baseline = np.array(fm.get_turbine_power())
+        disabled_turb_cp_ct = {
+            "wind_speed": [0.0, 50.0],
+            "power": [0.0, 0.0],
+            "thrust_coefficient": [0.0001, 0.0001],
+        }
+        regular_turb_cp_ct = fm.core.farm.turbines[0].power_thrust_table
         df_pairs = pd.DataFrame(
-            {'turbine': pd.Series([], dtype='int'),
-             'affected_turbines': pd.Series([], dtype='int')})
+            {"turbine": pd.Series([], dtype="int"), "affected_turbines": pd.Series([], dtype="int")}
+        )
         for ti in range(self.num_turbs):
-            fi.change_turbine(
-                [ti], {"power_thrust_table": disabled_turb_cp_ct})
-            fi.calculate_wake()
-            power_excl = np.array(fi.get_turbine_power())
+            fm.change_turbine([ti], {"power_thrust_table": disabled_turb_cp_ct})
+            fm.run()
+            power_excl = np.array(fm.get_turbine_power())
             power_excl[ti] = power_baseline[ti]  # Placeholder
             wake_losses = 1 - power_baseline / power_excl
             affectedturbs = np.where(wake_losses >= wake_loss_thrs)[0]
             df_pairs = df_pairs.append(
-                {'turbine': int(ti), 'affected_turbines': affectedturbs},
-                ignore_index=True)
-            fi.change_turbine([ti], {"power_thrust_table": regular_turb_cp_ct})
+                {"turbine": int(ti), "affected_turbines": affectedturbs}, ignore_index=True
+            )
+            fm.change_turbine([ti], {"power_thrust_table": regular_turb_cp_ct})
 
         # Save to self
-        df_pairs = df_pairs.set_index('turbine', drop=True)
+        df_pairs = df_pairs.set_index("turbine", drop=True)
         self.turbine_pairs = df_pairs
         return df_pairs
 
     def plot_flowfield(self):
-        self.fi.calculate_wake()
+        self.fm.run()
         fig, ax = plt.subplots()
-        hor_plane = self.fi.get_hor_plane()
+        hor_plane = self.fm.get_hor_plane()
         wfct.visualization.visualize_cut_plane(hor_plane, ax=ax)
         return fig, ax, hor_plane
 
     def floris_set_ws_wd_ti(self, wd=None, ws=None, ti=None):
-        self.fi = ftools._fi_set_ws_wd_ti(self.fi, wd=wd, ws=ws, ti=ti)
+        self.fm = ftools._fi_set_ws_wd_ti(self.fi, wd=wd, ws=ws, ti=ti)
 
     def _check_measurements(self):
         if self.P_measured is None:
-            raise ValueError('Please specify measurements using .set_measurements(P_measured) before attempting to estimate the turbulence intensity.')
-
-    def estimate_farmaveraged_ti(self,
-                                 Ns=50,
-                                 bounds=(0.01, 0.50),
-                                 refine_with_fmin=False,
-                                 verbose=False):
-
+            raise ValueError(
+                "Please specify measurements using .set_measurements(P_measured) "
+                "before attempting to estimate the turbulence intensity."
+            )
+
+    def estimate_farmaveraged_ti(
+        self, Ns=50, bounds=(0.01, 0.50), refine_with_fmin=False, verbose=False
+    ):
         self._check_measurements()
-        out = opt.estimate_ti(fi=self.fi,
-                              P_measured=self.P_measured,
-                              Ns=Ns,
-                              bounds=bounds,
-                              turbine_upstream=range(self.num_turbs),
-                              turbines_downstream=range(self.num_turbs),
-                              refine_with_fmin=refine_with_fmin,
-                              verbose=verbose)
+        out = opt.estimate_ti(
+            fi=self.fi,
+            P_measured=self.P_measured,
+            Ns=Ns,
+            bounds=bounds,
+            turbine_upstream=range(self.num_turbs),
+            turbines_downstream=range(self.num_turbs),
+            refine_with_fmin=refine_with_fmin,
+            verbose=verbose,
+        )
 
         self.opt_farm = out
-        ti_opt = out['x_opt']
+        ti_opt = out["x_opt"]
         self.floris_set_ws_wd_ti(ti=ti_opt)
-        print('Optimal farm-averaged ti: %.3f' % ti_opt)
+        logger.info("Optimal farm-averaged ti: %.3f" % ti_opt)
 
         return ti_opt
 
-    def estimate_local_tis(self,
-                           Ns=50,
-                           bounds=(0.01, 0.50),
-                           refine_with_fmin=False,
-                           verbose=False):
-
+    def estimate_local_tis(self, Ns=50, bounds=(0.01, 0.50), refine_with_fmin=False, verbose=False):
         self._check_measurements()
         turbines_sorted = self.turbine_list_ordered
         df_turbine_pairs = self.turbine_pairs
 
         out_array = [[] for _ in range(self.num_turbs)]
-        ti_array = np.repeat(self.opt_farm['x_opt'], self.num_turbs)
+        ti_array = np.repeat(self.opt_farm["x_opt"], self.num_turbs)
         for ti in turbines_sorted:
-            turbs_aff = df_turbine_pairs.loc[ti, 'affected_turbines']
+            turbs_aff = df_turbine_pairs.loc[ti, "affected_turbines"]
             if len(turbs_aff) > 0:
-                out = opt.estimate_ti(fi=self.fi,
-                                      P_measured=self.P_measured[turbs_aff],
-                                      Ns=Ns,
-                                      bounds=bounds,
-                                      turbine_upstream=ti,
-                                      turbines_downstream=turbs_aff,
-                                      refine_with_fmin=refine_with_fmin,
-                                      verbose=verbose)
-                ti_array[ti] = out['x_opt']
+                out = opt.estimate_ti(
+                    fi=self.fi,
+                    P_measured=self.P_measured[turbs_aff],
+                    Ns=Ns,
+                    bounds=bounds,
+                    turbine_upstream=ti,
+                    turbines_downstream=turbs_aff,
+                    refine_with_fmin=refine_with_fmin,
+                    verbose=verbose,
+                )
+                ti_array[ti] = out["x_opt"]
                 self.floris_set_ws_wd_ti(ti=ti_array)
             else:
-                out = {'x_opt': self.opt_farm['x_opt'],
-                       'J_opt': np.nan, 'x': [], 'J': []}
+                out = {"x_opt": self.opt_farm["x_opt"], "J_opt": np.nan, "x": [], "J": []}
 
             out_array[ti] = out
 
         self.opt_turbines = out_array
         for ti in range(self.num_turbs):
-            print('Optimal ti for turbine %03d: %.3f' % (ti, ti_array[ti]))
+            logger.info("Optimal ti for turbine %03d: %.3f" % (ti, ti_array[ti]))
 
         return out_array
 
     def plot_cost_function_farm(self):
         fig, ax = plt.subplots()
-        ax.plot(self.opt_farm['x'], self.opt_farm['J'])
-        ax.plot(self.opt_farm['x_opt'], self.opt_farm['J_opt'], 'ro')
-        ax.set_ylabel('Cost function')
-        ax.set_xlabel('Turbulence intensity (-)')
+        ax.plot(self.opt_farm["x"], self.opt_farm["J"])
+        ax.plot(self.opt_farm["x_opt"], self.opt_farm["J_opt"], "ro")
+        ax.set_ylabel("Cost function")
+        ax.set_xlabel("Turbulence intensity (-)")
         ax.grid(True)
-        ax.set_title('Farm-wide turbulence intensity estimation: cost function J')
+        ax.set_title("Farm-wide turbulence intensity estimation: cost function J")
 
     def plot_cost_functions_turbines(self):
         for ti in range(self.num_turbs):
             fig, ax = plt.subplots()
-            ax.plot(self.opt_turbines[ti]['x'], self.opt_turbines[ti]['J'])
-            ax.plot(self.opt_turbines[ti]['x_opt'], self.opt_turbines[ti]['J_opt'], 'ro')
-            ax.set_ylabel('Cost function')
-            ax.set_xlabel('Turbulence intensity (-)')
+            ax.plot(self.opt_turbines[ti]["x"], self.opt_turbines[ti]["J"])
+            ax.plot(self.opt_turbines[ti]["x_opt"], self.opt_turbines[ti]["J_opt"], "ro")
+            ax.set_ylabel("Cost function")
+            ax.set_xlabel("Turbulence intensity (-)")
             ax.grid(True)
-            ax.set_title('Turbulence intensity estimation for turbine %03d: cost function J' % ti)
+            ax.set_title("Turbulence intensity estimation for turbine %03d: cost function J" % ti)
 
     def plot_power_bars(self):
-        fi = self.fi
-        fi.calculate_wake()
+        fm = self.fi
+        fm.run()
         fig, ax = plt.subplots()
-        ax.bar(x=np.array(range(self.num_turbs))-0.15,
-               height=fi.get_turbine_power(), width=.3)
-        ax.bar(x=np.array(range(self.num_turbs))+0.15,
-               height=self.P_measured, width=.3)
-        ax.set_title('Measurement and FLORIS comparison')
-        ax.set_ylabel('Power')
-        ax.set_xlabel('Turbine number')
-        ax.legend(['FLORIS', 'SCADA'])
+        ax.bar(x=np.array(range(self.num_turbs)) - 0.15, height=fm.get_turbine_power(), width=0.3)
+        ax.bar(x=np.array(range(self.num_turbs)) + 0.15, height=self.P_measured, width=0.3)
+        ax.set_title("Measurement and FLORIS comparison")
+        ax.set_ylabel("Power")
+        ax.set_xlabel("Turbine number")
+        ax.legend(["FLORIS", "SCADA"])
         return fig, ax
```

### Comparing `flasc-1.4.2/flasc/optimization.py` & `flasc-2.0/flasc/utilities/optimization.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,213 +1,180 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-
 import copy
 from datetime import timedelta as td
+
 import numpy as np
-from pandas.errors import DataError
 import scipy.optimize as opt
 import scipy.stats as spst
-
 from floris.utilities import wrap_180, wrap_360
+from pandas.errors import DataError
+
+from flasc.data_processing import time_operations as fsato
+from flasc.logging_manager import LoggingManager
+from flasc.utilities import circular_statistics as css, floris_tools as ftools, utilities as fsut
 
-from . import (
-    circular_statistics as css,
-    floris_tools as ftools,
-    utilities as fsut,
-    time_operations as fsato
-)
+logger_manager = LoggingManager()  # Instantiate LoggingManager
+logger = logger_manager.logger  # Obtain the reusable logger
 
 
 def find_timeshift_between_dfs(
     df1,
     df2,
     cols_df1,
     cols_df2,
     use_circular_statistics=False,
-    t_step=np.timedelta64(30*24, 'h'),
+    t_step=np.timedelta64(30 * 24, "h"),
     correct_y_shift=False,
     y_shift_range=np.arange(-180.0, 180.0, 2.0),
     opt_bounds=None,
     opt_Ns=None,
-    verbose=True
+    verbose=True,
 ):
-
     if np.any(df1["time"].diff() < td(seconds=0)):
         raise DataError("Dataframe 1 not sorted by time.")
 
     if np.any(df2["time"].diff() < td(seconds=0)):
         raise DataError("Dataframe 2 not sorted by time.")
 
     # Deal with incompatible inputs
-    if ((correct_y_shift) and (not use_circular_statistics)):
+    if (correct_y_shift) and (not use_circular_statistics):
         raise NotImplementedError("Incompatible input specified.")
 
     # Get min and max time for dataframes
-    min_time = np.datetime64(
-        np.max([df1.head(1)["time"], df2.head(1)["time"]])
-    )
-    max_time = np.datetime64(
-        np.min([df1.tail(1)["time"], df2.tail(1)["time"]])
-    )
+    min_time = np.datetime64(np.max([df1.head(1)["time"], df2.head(1)["time"]]))
+    max_time = np.datetime64(np.min([df1.tail(1)["time"], df2.tail(1)["time"]]))
 
     # Convert to arrays of a single mean quantity
-    print('Determining one column-average per dataframe to sync.')
+    logger.info("Determining one column-average per dataframe to sync.")
     if use_circular_statistics:
-        df1['y1'] = css.calc_wd_mean_radial(df1[cols_df1], axis=1)
-        df2['y2'] = css.calc_wd_mean_radial(df2[cols_df2], axis=1)
+        df1["y1"] = css.calc_wd_mean_radial(df1[cols_df1], axis=1)
+        df2["y2"] = css.calc_wd_mean_radial(df2[cols_df2], axis=1)
     else:
-        df1['y1'] = np.nanmean(df1[cols_df1], axis=1)
-        df2['y2'] = np.nanmean(df2[cols_df2], axis=1)
+        df1["y1"] = np.nanmean(df1[cols_df1], axis=1)
+        df2["y2"] = np.nanmean(df2[cols_df2], axis=1)
 
     # Cut down df1 and df2 to a minimal dataframe
-    df1 = df1[['time', 'y1']]
-    df2 = df2[['time', 'y2']]
+    df1 = df1[["time", "y1"]]
+    df2 = df2[["time", "y2"]]
 
     # Create a shared time array and sync both dfs on it
     try:
         # Try estimation of dt from first 5k entries
         dt = np.min(
-            [
-                fsut.estimate_dt(df1.iloc[0:5000]['time']),
-                fsut.estimate_dt(df2.iloc[0:5000]['time'])
-            ]
+            [fsut.estimate_dt(df1.iloc[0:5000]["time"]), fsut.estimate_dt(df2.iloc[0:5000]["time"])]
         )
-    except:
+    except (ValueError, TypeError) as e:
+        # Handle specific exception
+        logger.info(f"Error estimating dt: {e}")
         # Use full dataframe if fails somehow
-        dt = np.min(
-            [
-                fsut.estimate_dt(df1['time']),
-                fsut.estimate_dt(df2['time'])
-            ]
-        )
+        dt = np.min([fsut.estimate_dt(df1["time"]), fsut.estimate_dt(df2["time"])])
 
-    print('Resampling dataframes to a common time vector. ' +
-          'This may take a while...')
+    logger.info("Resampling dataframes to a common time vector. " + "This may take a while...")
     time_array = min_time + np.arange(0, max_time - min_time + np.timedelta64(dt), dt)
     max_gap = 1.5 * dt
     df1 = fsato.df_resample_by_interpolation(
         df1,
         time_array=time_array,
         circular_cols=use_circular_statistics,
-        interp_method='linear',
+        interp_method="linear",
         max_gap=max_gap,
     )
     df2 = fsato.df_resample_by_interpolation(
-        df2, time_array=time_array,
+        df2,
+        time_array=time_array,
         circular_cols=use_circular_statistics,
-        interp_method='linear',
+        interp_method="linear",
         max_gap=max_gap,
     )
 
     # Look at comparison per t_step
     current_time = min_time
     output_list = []
-    print('Estimating required timeshift for df1.')
+    logger.info("Estimating required timeshift for df1.")
     while current_time < max_time:
-        t0 = np.array(current_time, dtype='datetime64')
-        t1 = np.array(
-            np.datetime64(current_time) + np.timedelta64(t_step),
-            dtype='datetime64'
-        )
+        t0 = np.array(current_time, dtype="datetime64")
+        t1 = np.array(np.datetime64(current_time) + np.timedelta64(t_step), dtype="datetime64")
         id_sub = (df1.time >= t0) & (df1.time < t1)
         df1_sub = df1[id_sub]
         df2_sub = df2[id_sub]
 
         # Create x, y1 and y2 vectors
-        x = np.array(df1_sub['time'], dtype=np.datetime64)
-        x = np.array((x-x[0])/np.timedelta64(1, 's'))
-        y1 = np.array(df1_sub['y1'])
-        y2 = np.array(df2_sub['y2'])
+        x = np.array(df1_sub["time"], dtype=np.datetime64)
+        x = np.array((x - x[0]) / np.timedelta64(1, "s"))
+        y1 = np.array(df1_sub["y1"])
+        y2 = np.array(df2_sub["y2"])
 
         if verbose:
-            print('   Calculating timeshift for t0: %s, t1: %s'
-                  % (str(t0), str(t1)))
+            logger.info("   Calculating timeshift for t0: %s, t1: %s" % (str(t0), str(t1)))
 
         def cost_fun(x_shift):
             # Shift data along x-axis and then fit along y-axis, if necessary
-            y1_cor = fsut.interp_with_max_gap(x, x - x_shift, y1, max_gap=max_gap, kind='linear')
+            y1_cor = fsut.interp_with_max_gap(x, x - x_shift, y1, max_gap=max_gap, kind="linear")
 
             if correct_y_shift:
                 y_bias, J = match_y_curves_by_offset(
-                    y1_cor, y2, dy_eval=y_shift_range,
-                    angle_wrapping=use_circular_statistics
+                    y1_cor, y2, dy_eval=y_shift_range, angle_wrapping=use_circular_statistics
                 )
                 y1_cor = y1_cor - y_bias
                 if use_circular_statistics:
                     y1_cor = wrap_360(y1_cor)
 
             # Remove NaNs and infs
-            ids = (
-                (~np.isnan(y1_cor)) & (~np.isnan(y2)) &
-                (~np.isinf(y1_cor)) & (~np.isinf(y2))
-            )
+            ids = (~np.isnan(y1_cor)) & (~np.isnan(y2)) & (~np.isinf(y1_cor)) & (~np.isinf(y2))
             y2_cor = y2[ids]
             y1_cor = y1_cor[ids]
 
             # Calculate score
-            if ((len(y1_cor) < 10) | (len(y2_cor) < 10)):
+            if (len(y1_cor) < 10) | (len(y2_cor) < 10):
                 cost = np.nan
             else:
-                cost = -1. * spst.pearsonr(y1_cor, y2_cor)[0]
+                cost = -1.0 * spst.pearsonr(y1_cor, y2_cor)[0]
             return cost
 
         # Optimize using scipy.brute()
         if opt_bounds is None:
             opt_bounds = [(-td(hours=10), td(hours=10))]
         elif isinstance(opt_bounds[0], (tuple, list)):
             opt_bounds = opt_bounds  # Fine
         else:
             opt_bounds = [opt_bounds]
 
         if isinstance(opt_bounds[0][0], np.timedelta64):
-            opt_bounds[0] = (opt_bounds[0][0] / np.timedelta64(1, 's'),
-                             opt_bounds[0][1] / np.timedelta64(1, 's'))
+            opt_bounds[0] = (
+                opt_bounds[0][0] / np.timedelta64(1, "s"),
+                opt_bounds[0][1] / np.timedelta64(1, "s"),
+            )
         if isinstance(opt_bounds[0][0], td):
-            opt_bounds[0] = (opt_bounds[0][0] / td(seconds=1),
-                             opt_bounds[0][1] / td(seconds=1))
+            opt_bounds[0] = (opt_bounds[0][0] / td(seconds=1), opt_bounds[0][1] / td(seconds=1))
 
         if opt_Ns is None:
             # Explore in steps of 10 minutes
-            opt_Ns = int((opt_bounds[0][1]-opt_bounds[0][0]) / 600.)
+            opt_Ns = int((opt_bounds[0][1] - opt_bounds[0][0]) / 600.0)
 
         finish = opt.fmin  # Can also be None
         if verbose:
-            opt_disp = 'iter'
+            opt_disp = "iter"
         else:
-            opt_disp = 'final'
+            opt_disp = "final"
         x_opt, J_opt, x_all, J_all = opt.brute(
-            cost_fun,
-            ranges=opt_bounds,
-            Ns=opt_Ns,
-            finish=finish,
-            disp=opt_disp,
-            full_output=True
+            cost_fun, ranges=opt_bounds, Ns=opt_Ns, finish=finish, disp=opt_disp, full_output=True
+        )
+        logger.info(
+            "     Optimal time shift for df_1: %d s (%.2f hours)." % (x_opt[0], x_opt[0] / 3600.0)
         )
-        print('     Optimal time shift for df_1: %d s (%.2f hours).'
-              % (x_opt[0], x_opt[0]/3600.))
 
-        output_list.append({
-            't0': t0,
-            't1': t1,
-            'x_opt': td(seconds=x_opt[0]),
-            'J_opt': J_opt,
-            'x': x_all,
-            'J': J_all
-        })
+        output_list.append(
+            {
+                "t0": t0,
+                "t1": t1,
+                "x_opt": td(seconds=x_opt[0]),
+                "J_opt": J_opt,
+                "x": x_all,
+                "J": J_all,
+            }
+        )
 
         current_time = np.datetime64(current_time) + np.timedelta64(t_step)
 
     return output_list
 
 
 # def find_bias_x(x_1, y_1, x_2, y_2, search_range, search_dx):
@@ -250,18 +217,18 @@
             raise ValueError("Requires dy_eval if wrap_360==False.")
 
     J_opt = np.nan
     dwd_opt = np.nan
     for dy in dy_eval:
         if angle_wrapping:
             ytest_cor = wrap_360(ytest - dy)
-            y_error = np.abs(wrap_180(yref-ytest_cor))
+            y_error = np.abs(wrap_180(yref - ytest_cor))
         else:
             ytest_cor = ytest - dy
-            y_error = np.abs(yref-ytest_cor)
+            y_error = np.abs(yref - ytest_cor)
 
         if np.all(np.isnan(y_error)) | (len(y_error) < 1):
             J = np.nan
         else:
             J = np.nanmean(y_error**2.0)
 
         if np.isnan(J_opt):
@@ -270,46 +237,50 @@
                 dwd_opt = dy
         elif J < J_opt:
             J_opt = J
             dwd_opt = dy
     return dwd_opt, J_opt
 
 
-def estimate_ti(fi, P_measured, Ns, bounds, turbine_upstream,
-                turbines_downstream, refine_with_fmin=False,
-                verbose=False):
+def estimate_ti(
+    fi,
+    P_measured,
+    Ns,
+    bounds,
+    turbine_upstream,
+    turbines_downstream,
+    refine_with_fmin=False,
+    verbose=False,
+):
     # Make copy so that existing object is not changed
-    fi = copy.deepcopy(fi)
-    num_turbines = len(fi.layout_x)
-    ti_0 = np.mean(fi.floris.farm.turbulence_intensity)
+    fm = copy.deepcopy(fi)
+    num_turbines = len(fm.layout_x)
+    ti_0 = np.mean(fm.core.farm.turbulence_intensity)
 
     # Define a cost function
     def cost_fun(ti):
         ti_array = np.repeat(ti_0, num_turbines)
         ti_array[turbine_upstream] = ti
         ftools._fi_set_ws_wd_ti(fi, ti=ti_array)
-        fi.calculate_wake()
-        Pturbs = np.array(fi.get_turbine_power())
+        fm.run()
+        Pturbs = np.array(fm.get_turbine_power())
         Pturbs = Pturbs[turbines_downstream]
-        se = (P_measured-Pturbs)**2.0
+        se = (P_measured - Pturbs) ** 2.0
         mse = np.mean(se)
         return mse
 
     if refine_with_fmin:
         finish = opt.fmin
     else:
         finish = None
 
     # Ensure appropriate format
     if not (isinstance(bounds[0], tuple) | isinstance(bounds[0], list)):
         bounds = [bounds]
 
     # Optimize using grid search approach
-    x_opt, J_opt, x, J = opt.brute(cost_fun,
-                                   ranges=bounds,
-                                   Ns=Ns,
-                                   finish=finish,
-                                   disp=verbose,
-                                   full_output=True)
+    x_opt, J_opt, x, J = opt.brute(
+        cost_fun, ranges=bounds, Ns=Ns, finish=finish, disp=verbose, full_output=True
+    )
 
-    opt_result = {'x_opt': x_opt, 'J_opt': J_opt,  'x': x, 'J': J}
+    opt_result = {"x_opt": x_opt, "J_opt": J_opt, "x": x, "J": J}
     return opt_result
```

### Comparing `flasc-1.4.2/flasc/time_operations.py` & `flasc-2.0/flasc/data_processing/time_operations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,310 +1,282 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-
 from datetime import timedelta as td
-from itertools import product
 
 import numpy as np
 import pandas as pd
-
 from floris.utilities import wrap_360
 
-from . import utilities as fsut
+from flasc.logging_manager import LoggingManager
+from flasc.utilities import utilities as fsut
+
+logger_manager = LoggingManager()  # Instantiate LoggingManager
+logger = logger_manager.logger  # Obtain the reusable logger
 
 
 def df_movingaverage(
     df_in,
     cols_angular,
     window_width=td(seconds=60),
     min_periods=1,
     center=True,
-    calc_median_min_max_std=False
+    calc_median_min_max_std=False,
 ):
     """
-    Note that median, minimum, and maximum do not handle angular 
-    quantities and should be treated carefully. 
+    Note that median, minimum, and maximum do not handle angular
+    quantities and should be treated carefully.
     Standard deviation handles angular quantities.
     """
-    
-    df = df_in.set_index('time').copy()
-    
+
+    df = df_in.set_index("time").copy()
+
     # Find non-angular columns
     if isinstance(cols_angular, bool):
         if cols_angular:
             cols_angular = [c for c in df.columns]
         else:
             cols_angular = []
     cols_regular = [c for c in df.columns if c not in cols_angular]
-    
+
     # Save the full columns
     full_columns = df.columns
-    
+
     # Carry out the mean calculations
-    df_regular = (df
-                  [cols_regular] # Select only non-angular columns
-                  .rolling(window_width,
-                      center=center,
-                      axis=0,
-                      min_periods=min_periods
-                  )
-                  .mean()
-                 )
-
-
-    df_cos = (df
-              [cols_angular] # Select only angular columns
-              .pipe(lambda df_: np.cos(df_ * np.pi / 180.))
-              .rolling(window_width,
-                  center=center,
-                  axis=0,
-                  min_periods=min_periods
-              )
-              .mean()
-             )
-
-    df_sin = (df
-              [cols_angular] # Select only angular columns
-              .pipe(lambda df_: np.sin(df_ * np.pi / 180.))
-              .rolling(window_width,
-                  center=center,
-                  axis=0,
-                  min_periods=min_periods
-               )
-               .mean()
-             )
-    
-    dfm =  (df_regular
-            .join((np.arctan2(df_sin,df_cos) * 180. / np.pi) % 360)
-            [full_columns] # put back in order
-           )
-    
+    df_regular = (
+        df[cols_regular]  # Select only non-angular columns
+        .rolling(window_width, center=center, axis=0, min_periods=min_periods)
+        .mean()
+    )
+
+    df_cos = (
+        df[cols_angular]  # Select only angular columns
+        .pipe(lambda df_: np.cos(df_ * np.pi / 180.0))
+        .rolling(window_width, center=center, axis=0, min_periods=min_periods)
+        .mean()
+    )
+
+    df_sin = (
+        df[cols_angular]  # Select only angular columns
+        .pipe(lambda df_: np.sin(df_ * np.pi / 180.0))
+        .rolling(window_width, center=center, axis=0, min_periods=min_periods)
+        .mean()
+    )
+
+    dfm = df_regular.join((np.arctan2(df_sin, df_cos) * 180.0 / np.pi) % 360)[
+        full_columns
+    ]  # put back in order
+
     if not calc_median_min_max_std:
-        
         return dfm
-    
-    
-    if calc_median_min_max_std: # if including other statistics        
-   
-        df_regular_stats = (df
-                            .rolling(window_width,
-                                center=center,
-                                axis=0,
-                                min_periods=min_periods
-                            )
-                            .agg(["median", "min", "max", "std"])
-                            .pipe(lambda df_: flatten_cols(df_))
-                            )
-        
+
+    if calc_median_min_max_std:  # if including other statistics
+        df_regular_stats = (
+            df.rolling(window_width, center=center, axis=0, min_periods=min_periods)
+            .agg(["median", "min", "max", "std"])
+            .pipe(lambda df_: flatten_cols(df_))
+        )
+
         # Apply scipy.stats.circstd() step by step for performance reasons
-        df_angular_std = (df_sin
-                          .pow(2)
-                          .add(df_cos.pow(2))
-                          .pow(1/2) # sqrt()
-                          .apply(np.log) # log()
-                          .mul(-2)
-                          .pow(1/2) # sqrt()
-                          .mul(180/np.pi)
-                          .rename(
-                               {c: c + '_std' for c in dfm.columns},
-                               axis='columns'
-                          )
-                         )
-        
+        df_angular_std = (
+            df_sin.pow(2)
+            .add(df_cos.pow(2))
+            .pow(1 / 2)  # sqrt()
+            .apply(np.log)  # log()
+            .mul(-2)
+            .pow(1 / 2)  # sqrt()
+            .mul(180 / np.pi)
+            .rename({c: c + "_std" for c in dfm.columns}, axis="columns")
+        )
+
         # Merge the stats
-        df_stats = (df_regular_stats
-                    [[c for c in df_regular_stats.columns if \
-                        c not in df_angular_std.columns]]
-                    .join(df_angular_std)
-                   )
-                
+        df_stats = df_regular_stats[
+            [c for c in df_regular_stats.columns if c not in df_angular_std.columns]
+        ].join(df_angular_std)
+
         # Now merge in means and return
-        return (dfm
-                .rename({c: c + '_mean' for c in dfm.columns},axis='columns')
-                .join(df_stats)    
-               )
+        return dfm.rename({c: c + "_mean" for c in dfm.columns}, axis="columns").join(df_stats)
 
 
 def df_downsample(
     df_in,
     cols_angular,
     window_width=td(seconds=60),
     min_periods=1,
     center=False,
     calc_median_min_max_std=False,
-    return_index_mapping=False
+    return_index_mapping=False,
 ):
-
     # Copy and ensure dataframe is indexed by time
     df = df_in.copy()
     if "time" not in df.columns:
-        raise KeyError("\"time\" must be in df_in columns.")
+        raise KeyError('"time" must be in df_in columns.')
     df = df.set_index("time")
 
     # Find non-angular columns
     cols_regular = [c for c in df.columns if c not in cols_angular]
 
     # Now calculate cos and sin components for angular columns
     sin_cols = ["{:s}_sin".format(c) for c in cols_angular]
     cos_cols = ["{:s}_cos".format(c) for c in cols_angular]
 
     # Add in the sin/cos columns
-    df = pd.concat([df, np.sin(df[cols_angular] * np.pi / 180.0).
-                    set_axis(sin_cols, axis=1)], axis=1)
-    df = pd.concat([df, np.cos(df[cols_angular] * np.pi / 180.0).
-                    set_axis(cos_cols, axis=1)], axis=1)
+    df = pd.concat(
+        [df, np.sin(df[cols_angular] * np.pi / 180.0).set_axis(sin_cols, axis=1)], axis=1
+    )
+    df = pd.concat(
+        [df, np.cos(df[cols_angular] * np.pi / 180.0).set_axis(cos_cols, axis=1)], axis=1
+    )
 
     # Drop angular columns
     df = df.drop(columns=cols_angular)
 
     # Add _N for each variable to keep track of n.o. data points
     cols_all = df.columns
     cols_N = ["{:s}_N".format(c) for c in cols_all]
-    df = pd.concat([df, 1 - df[cols_all].isna().astype(int)\
-                            .set_axis(cols_N, axis=1)], axis=1)
-    
+    df = pd.concat([df, 1 - df[cols_all].isna().astype(int).set_axis(cols_N, axis=1)], axis=1)
+
     # Now calculate downsampled dataframe, automatically
     # mark by label on the right (i.e., "past 10 minutes").
     df_resample = df.resample(window_width, label="right", axis=0)
 
     # First calculate mean values of non-angular columns
     df_mean = df_resample[cols_regular].mean().copy()
 
     # Compute and append the angular means
-    df_mean = pd.concat([df_mean, pd.DataFrame(
-        wrap_360(np.arctan2(df_resample[sin_cols].mean().values,
-                            df_resample[cos_cols].mean().values
-            ) * 180.0 / np.pi
-        ),
-        columns=cols_angular,
-        index = df_mean.index
-        )], axis=1)
+    df_mean = pd.concat(
+        [
+            df_mean,
+            pd.DataFrame(
+                wrap_360(
+                    np.arctan2(
+                        df_resample[sin_cols].mean().values, df_resample[cos_cols].mean().values
+                    )
+                    * 180.0
+                    / np.pi
+                ),
+                columns=cols_angular,
+                index=df_mean.index,
+            ),
+        ],
+        axis=1,
+    )
 
     # Check if we have enough samples for every measurement
     if min_periods > 1:
         N_counts = df_resample[cols_N].sum()
         df_mean[N_counts < min_periods] = None  # Remove data relying on too few samples
 
     # Calculate median, min, max, std if necessary
     if calc_median_min_max_std:
-        
         df_stats = df_in.copy().set_index("time")
-        
+
         # Compute the stats for the non_angular columns
-        df_stats_regular =  (df_stats
-            [cols_regular] # Select non-angular columns
-            .resample(window_width, label="right", axis=0) # Resample to desired window
-            .agg(["median", "min", "max", "std"]) # Perform aggregations
-            .pipe(lambda df_: flatten_cols(df_)) # Flatten columns
+        df_stats_regular = (
+            df_stats[cols_regular]  # Select non-angular columns
+            .resample(window_width, label="right", axis=0)  # Resample to desired window
+            .agg(["median", "min", "max", "std"])  # Perform aggregations
+            .pipe(lambda df_: flatten_cols(df_))  # Flatten columns
         )
 
-        # Now to compute the statistics for the angular columns, which requires 
+        # Now to compute the statistics for the angular columns, which requires
         # shifting by the mean values
-        df_angular_mean_upsample = (df_mean
-            [cols_angular] # Select angular columns
-            .reindex(df_stats.index) # Go back to original time index
-            .bfill() # Back fill the points since using right indexing
-            .ffill() # Cover any stragglers at end
-        )
-        
-        df_angular_stats = (df_stats
-            [cols_angular]
-            .subtract(df_angular_mean_upsample) # Subtract the angular mean
-            .add(180) # Shift up by 180 (start of sequence for -180/180 wrap)
-            .mod(360) # Wrap by 360
-            .subtract(180) # Remove shift (end of sequence for -180/180 wrap)
-            .resample(window_width, label="right", axis=0) # Resample to desired window
+        df_angular_mean_upsample = (
+            df_mean[cols_angular]  # Select angular columns
+            .reindex(df_stats.index)  # Go back to original time index
+            .bfill()  # Back fill the points since using right indexing
+            .ffill()  # Cover any stragglers at end
+        )
+
+        df_angular_stats = (
+            df_stats[cols_angular]
+            .subtract(df_angular_mean_upsample)  # Subtract the angular mean
+            .add(180)  # Shift up by 180 (start of sequence for -180/180 wrap)
+            .mod(360)  # Wrap by 360
+            .subtract(180)  # Remove shift (end of sequence for -180/180 wrap)
+            .resample(window_width, label="right", axis=0)  # Resample to desired window
         )
-        
+
         # Now create the individual statistics
-        df_angular_median = (df_angular_stats
-            .median() # Apply the median
-            .add(df_mean[cols_angular]) # Shift back by original mean
-            .mod(360) # Wrap by 360
-            .rename({c:"%s_median" % c for c in cols_angular},axis="columns")
-        )
-        
-        df_angular_min = (df_angular_stats
-            .min() # Apply the min
-            .add(df_mean[cols_angular]) # Shift back by original mean
-            .mod(360) # Wrap by 360
-            .rename({c:"%s_min" % c for c in cols_angular},axis="columns")
-        )
-        
-        df_angular_max = (df_angular_stats
-            .max() # Apply the max
-            .add(df_mean[cols_angular]) # Shift back by original mean
-            .mod(360) # Wrap by 360
-            .rename({c:"%s_max" % c for c in cols_angular},axis="columns")
+        df_angular_median = (
+            df_angular_stats.median()  # Apply the median
+            .add(df_mean[cols_angular])  # Shift back by original mean
+            .mod(360)  # Wrap by 360
+            .rename({c: "%s_median" % c for c in cols_angular}, axis="columns")
+        )
+
+        df_angular_min = (
+            df_angular_stats.min()  # Apply the min
+            .add(df_mean[cols_angular])  # Shift back by original mean
+            .mod(360)  # Wrap by 360
+            .rename({c: "%s_min" % c for c in cols_angular}, axis="columns")
+        )
+
+        df_angular_max = (
+            df_angular_stats.max()  # Apply the max
+            .add(df_mean[cols_angular])  # Shift back by original mean
+            .mod(360)  # Wrap by 360
+            .rename({c: "%s_max" % c for c in cols_angular}, axis="columns")
         )
-        
+
         # Apply scipy.stats.circstd() step by step for performance reasons
-        df_angular_std = (df_resample
-            [sin_cols] # Get sine columns
-            .mean() # Apply mean
-            .rename({"{:s}_sin".format(c):"{:s}_std".format(c)
-                     for c in cols_angular}, axis="columns") # Rename for add()
+        df_angular_std = (
+            df_resample[sin_cols]  # Get sine columns
+            .mean()  # Apply mean
+            .rename(
+                {"{:s}_sin".format(c): "{:s}_std".format(c) for c in cols_angular}, axis="columns"
+            )  # Rename for add()
             .pow(2)
-            .add(df_resample[cos_cols].mean()
-                .rename({"{:s}_cos".format(c):"{:s}_std".format(c)
-                         for c in cols_angular},axis="columns")
+            .add(
+                df_resample[cos_cols]
+                .mean()
+                .rename(
+                    {"{:s}_cos".format(c): "{:s}_std".format(c) for c in cols_angular},
+                    axis="columns",
+                )
                 .pow(2)
-            ) # Now have mean(sin(wd))**2 + mean(cos(wd))**2
-            .pow(1/2) # sqrt()
-            .apply(np.log) # log()
+            )  # Now have mean(sin(wd))**2 + mean(cos(wd))**2
+            .pow(1 / 2)  # sqrt()
+            .apply(np.log)  # log()
             .mul(-2)
-            .pow(1/2) # sqrt()
-            .mul(180/np.pi)
+            .pow(1 / 2)  # sqrt()
+            .mul(180 / np.pi)
         )
-        
+
         # df_out is the concatination of all these matrices
-        df_out = pd.concat([df_mean.rename(
-                                {c:"%s_mean" % c for c in df_mean.columns},
-                                 axis="columns"
-                            ),
-                            df_stats_regular,
-                            df_angular_median,
-                            df_angular_min,
-                            df_angular_max,
-                            df_angular_std
-                            ], axis=1)
-        
+        df_out = pd.concat(
+            [
+                df_mean.rename({c: "%s_mean" % c for c in df_mean.columns}, axis="columns"),
+                df_stats_regular,
+                df_angular_median,
+                df_angular_min,
+                df_angular_max,
+                df_angular_std,
+            ],
+            axis=1,
+        )
+
         df_out = df_out[sorted(df_out.columns)]
-        
-    else: # if not computing stats
+
+    else:  # if not computing stats
         df_out = df_mean
-        
+
     if center:
         # Shift time column towards center of the bin
         df_out.index = df_out.index - window_width / 2.0
 
     if return_index_mapping:
-        df_tmp = (pd.DataFrame(
-            data = {"time":df.reset_index()["time"],
-                    "tmp":1}
-            )
-            .resample(window_width, on="time", label="right", axis=0)
+        df_tmp = pd.DataFrame(data={"time": df.reset_index()["time"], "tmp": 1}).resample(
+            window_width, on="time", label="right", axis=0
         )
 
         # Grab index of first and last time entry for each window
         def get_first_index(x):
             if len(x) <= 0:
                 return -1
             else:
                 return x.index[0]
+
         def get_last_index(x):
             if len(x) <= 0:
                 return -1
             else:
                 return x.index[-1]
 
         windows_min = df_tmp.apply(get_first_index)["tmp"].to_list()
@@ -313,94 +285,92 @@
         # Now create a large array that contains the array of indices, with
         # the values in each row corresponding to the indices upon which that
         # row's moving/rolling average is based. Note that we purposely create
         # a larger matrix than necessary, since some rows/windows rely on more
         # data (indices) than others. This is the case e.g., at the start of
         # the dataset, at the end, and when there are gaps in the data. We fill
         # the remaining matrix entries with "-1".
-        dn = int(np.ceil(window_width/fsut.estimate_dt(df_in["time"]))) + 5
+        dn = int(np.ceil(window_width / fsut.estimate_dt(df_in["time"]))) + 5
         data_indices = -1 * np.ones((df_out.shape[0], dn), dtype=int)
         for ii in range(len(windows_min)):
             lb = windows_min[ii]
             ub = windows_max[ii]
             if not ((lb == -1) | (ub == -1)):
                 ind = np.arange(lb, ub + 1, dtype=int)
                 data_indices[ii, ind - lb] = ind
-        
+
         return df_out.reset_index(), data_indices
     else:
-        return df_out.reset_index() # Conform to new standard that, between functions, time is a column
+        return (
+            df_out.reset_index()
+        )  # Conform to new standard that, between functions, time is a column
+
 
 def df_resample_by_interpolation(
-    df,
-    time_array,
-    circular_cols,
-    interp_method='linear',
-    max_gap=None,
-    verbose=True
+    df, time_array, circular_cols, interp_method="linear", max_gap=None, verbose=True
 ):
     # Copy with properties but no actual data
     df_res = df.head(0).copy()
 
     # Remove timezones, if any
     df = df.copy()
     time_array = [pd.to_datetime(t).tz_localize(None) for t in time_array]
-    time_array = np.array(time_array, dtype='datetime64')
+    time_array = np.array(time_array, dtype="datetime64")
     df["time"] = df["time"].dt.tz_localize(None)
 
     # Fill with np.nan values and the correct time array (without tz)
-    df_res['time'] = time_array
+    df_res["time"] = time_array
 
     t0 = time_array[0]
-    df_t = np.array(df['time'] - t0, dtype=np.timedelta64)
-    xp = df_t/np.timedelta64(1, 's')  # Convert to regular seconds
+    df_t = np.array(df["time"] - t0, dtype=np.timedelta64)
+    xp = df_t / np.timedelta64(1, "s")  # Convert to regular seconds
     xp = np.array(xp, dtype=float)
 
     # Normalize time variables
     time_array = np.array([t - t0 for t in time_array], dtype=np.timedelta64)
-    x = time_array/np.timedelta64(1, 's')
+    x = time_array / np.timedelta64(1, "s")
 
     if max_gap is None:
         max_gap = 1.5 * np.median(np.diff(x))
     else:
-        max_gap = np.timedelta64(max_gap) / np.timedelta64(1, 's')
+        max_gap = np.timedelta64(max_gap) / np.timedelta64(1, "s")
 
-    cols_to_interp = [c for c in df_res.columns if c not in ['time']]
+    cols_to_interp = [c for c in df_res.columns if c not in ["time"]]
 
     # NN interpolation: just find indices and map accordingly for all cols
     for ii, c in enumerate(cols_to_interp):
         if isinstance(circular_cols, bool):
             wrap_around_360 = circular_cols
         elif isinstance(circular_cols[0], bool):
             wrap_around_360 = circular_cols[ii]
         elif isinstance(circular_cols[0], str):
-            wrap_around_360 = (c in circular_cols)
+            wrap_around_360 = c in circular_cols
 
-        dt_raw_median = (df['time'].diff().median() / td(seconds=1))
+        dt_raw_median = df["time"].diff().median() / td(seconds=1)
         if verbose:
-            print(
-                "  Resampling column '{:s}' with median timestep {:.3f} s onto a prespecified time ".format(c, dt_raw_median) +
-                "array with kind={}, max_gap={}".format(interp_method, max_gap) +
-                "s, and wrap_around_360={}".format(wrap_around_360)
+            logger.info(
+                f"  Resampling column '{c}' with median timestep {dt_raw_median:.3f} s "
+                f"onto a prespecified time array with kind={interp_method}, max_gap={max_gap}"
+                f"s, and wrap_around_360={wrap_around_360}"
             )
 
         fp = np.array(df[c], dtype=float)
         ids = (~np.isnan(xp)) & ~(np.isnan(fp))
 
         y = fsut.interp_with_max_gap(
             x=x,
             xp=xp[ids],
             fp=fp[ids],
             max_gap=max_gap,
             kind=interp_method,
-            wrap_around_360=wrap_around_360
+            wrap_around_360=wrap_around_360,
         )
         df_res[c] = y
 
     return df_res
 
+
 # Function from "EFFECTIVE PANDAS" for flattening multi-level column names
-def flatten_cols (df):
-    cols = ['_'. join(map(str , vals ))
-    for vals in df.columns.to_flat_index ()]
+def flatten_cols(df):
+    cols = ["_".join(map(str, vals)) for vals in df.columns.to_flat_index()]
     df.columns = cols
     return df
```

### Comparing `flasc-1.4.2/flasc/turbine_analysis/find_sensor_faults.py` & `flasc-2.0/flasc/data_processing/find_sensor_faults.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,98 +1,96 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-
 import os
+
 import matplotlib.pyplot as plt
 import numpy as np
 
+from flasc.logging_manager import LoggingManager
+
+logger_manager = LoggingManager()  # Instantiate LoggingManager
+logger = logger_manager.logger  # Obtain the reusable logger
+
 
 def find_sensor_stuck_faults(
-        df,
-        columns,
-        ti,
-        stddev_threshold=0.001,
-        n_consecutive_measurements=3,
-        plot_figures=True,
-        verbose=False,
-    ):
+    df,
+    columns,
+    ti,
+    stddev_threshold=0.001,
+    n_consecutive_measurements=3,
+    plot_figures=True,
+    verbose=False,
+    return_by_column=False,
+):
     # Settings which indicate a sensor-stuck type of fault: the standard
     # deviation between the [no_consecutive_measurements] number of
     # consecutive measurements is less than [stddev_threshold].
+
+    # TODO: remove unused argument 'ti'
+
+    index_faults = {c: np.array([]) for c in columns}
     for c in columns:
         if verbose:
-            print("Processing column %s" % c)
+            logger.info("Processing column %s" % c)
         measurement_array = np.array(df[c])
 
-        index_faults = _find_sensor_stuck_single_timearray(
+        column_index_faults = _find_sensor_stuck_single_timearray(
             measurement_array=measurement_array,
             no_consecutive_measurements=n_consecutive_measurements,
             stddev_threshold=stddev_threshold,
             index_array=df.index,
         )
 
-        if (plot_figures) & (len(index_faults) > 0):
-            _plot_top_sensor_faults(df, c, index_faults)
+        if (plot_figures) & (len(column_index_faults) > 0):
+            _plot_top_sensor_faults(df, c, column_index_faults)
 
-    return index_faults
+        index_faults[c] = column_index_faults
+
+    if return_by_column:
+        return index_faults
+    else:
+        return np.unique(np.concatenate([v for v in index_faults.values()]))
 
 
 def _plot_top_sensor_faults(
     df,
     c,
     index_faults,
     N_eval_max=5,
     save_path=None,
     fig_format="png",
     dpi=300,
 ):
-
     # Extract largest fault set and plot
     diff_index_faults = np.diff(index_faults)
     diffjumps = np.where(diff_index_faults > 1)[0]
     fault_sets = []
     imin = 0
     for imax in list(diffjumps):
         if (imax - imin) > 1:
             fault_sets.append(index_faults[imin + 1 : imax])
         imin = imax
     if len(index_faults) - imin > 1:
         fault_sets.append(index_faults[imin + 1 : :])
     fault_sets_idx_sorted = np.argsort([len(i) for i in fault_sets])[::-1]
     N_eval = np.min([N_eval_max, len(fault_sets)])
-    fig, ax_array = plt.subplots(
-        nrows=N_eval, ncols=1, figsize=(5.0, 2.5 * N_eval)
-    )
+    fig, ax_array = plt.subplots(nrows=N_eval, ncols=1, figsize=(5.0, 2.5 * N_eval))
 
     if N_eval == 1:
         ax_array = [ax_array]
 
     for i in range(N_eval):
         ax = ax_array[i]
         fault_set_eval = fault_sets[fault_sets_idx_sorted[i]]
 
         indices_to_plot = range(
             fault_set_eval[0] - 4 * len(fault_set_eval),
             fault_set_eval[-1] + 4 * len(fault_set_eval),
         )
         indices_to_plot = [v for v in indices_to_plot if v in df.index]
 
-        ax.plot(
-            df.loc[indices_to_plot, "time"], df.loc[indices_to_plot, c], "o"
-        )
+        ax.plot(df.loc[indices_to_plot, "time"], df.loc[indices_to_plot, c], "o")
         ax.plot(
             df.loc[index_faults, "time"],
             df.loc[index_faults, c],
             "o",
             color="red",
         )
         ax.set_xlim(
@@ -113,20 +111,16 @@
         fig_path = os.path.join(save_path, "%s_faults.%s" % (c, fig_format))
         fig.savefig(fig_path, dpi=dpi)
 
     return fig, ax_array
 
 
 def _find_sensor_stuck_single_timearray(
-        measurement_array,
-        no_consecutive_measurements=6,
-        stddev_threshold=0.05,
-        index_array=None
+    measurement_array, no_consecutive_measurements=6, stddev_threshold=0.05, index_array=None
 ):
-
     # Create index array, if unspecified
     N = len(measurement_array)
     if index_array is None:
         index_array = np.array(range(N))
 
     # Ensure variable types
     index_array = np.array(index_array)
@@ -137,21 +131,19 @@
     measurement_array = measurement_array[~np.isnan(measurement_array)]
 
     def format_array(array_in, row_length):
         array_in = np.array(array_in)
         Nm = row_length - 1
         C = array_in[0:-Nm]
         for ii in range(1, Nm):
-            C = np.vstack([C, array_in[ii:-Nm+ii]])
+            C = np.vstack([C, array_in[ii : -Nm + ii]])
         C = np.vstack([C, array_in[Nm::]]).T
         return C
 
-    Cindex = format_array(index_array,
-                          row_length=no_consecutive_measurements)
-    Cmeas = format_array(measurement_array,
-                         row_length=no_consecutive_measurements)
+    Cindex = format_array(index_array, row_length=no_consecutive_measurements)
+    Cmeas = format_array(measurement_array, row_length=no_consecutive_measurements)
 
     # Get standard deviations and determine faults
     std_array = np.std(Cmeas, axis=1)
     indices_faulty = np.unique(Cindex[std_array < stddev_threshold, :])
 
     return indices_faulty
```

### Comparing `flasc-1.4.2/flasc/turbine_analysis/northing_offset.py` & `flasc-2.0/flasc/data_processing/northing_offset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,26 @@
-# Copyright 2021 NREL and SHELL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-
 from datetime import timedelta as td
+
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-
 from floris.utilities import wrap_360
 
-from flasc import (
-    floris_tools as ftools,
-    optimization as opt,
-)
+from flasc.logging_manager import LoggingManager
+from flasc.utilities import floris_tools as ftools, optimization as opt
+
+logger_manager = LoggingManager()  # Instantiate LoggingManager
+logger = logger_manager.logger  # Obtain the reusable logger
 
 
-def crosscheck_northing_offset_consistency(df, fi, bias_timestep=td(days=120), nan_thrshld=0.50, plot_figure=True):
+def crosscheck_northing_offset_consistency(
+    df, fm, bias_timestep=td(days=120), nan_thrshld=0.50, plot_figure=True
+):
     # Load data and extract info
-    num_turbines = len(fi.layout_x)
+    num_turbines = len(fm.layout_x)
     turbine_list = range(num_turbines)
 
     # Set up time_array and split into chunks
     time_array = np.array(df["time"])
     t = pd.to_datetime(time_array[0])
     idx_chunks = list()
     while t < pd.to_datetime(time_array[-1]):
@@ -41,120 +31,111 @@
 
     # Get reference turbines and create placeholder dataframes
     N_rt = 5  # Number of reference turbines
     turbs_ref_list = [[] for _ in turbine_list]
     bias_output_list = [[] for _ in turbine_list]
     for ti in turbine_list:
         turbs_in_radius = ftools.get_turbs_in_radius(
-            fi.layout_x,
-            fi.layout_y,
+            fm.layout_x,
+            fm.layout_y,
             ti,
             max_radius=1.0e9,
             include_itself=False,
             sort_by_distance=True,
         )
         turbs_ref_list[ti] = turbs_in_radius[0:N_rt]
         bias_output_list[ti] = pd.DataFrame(
             data=np.reshape(np.full(N_chnks * N_rt, np.nan), (N_chnks, N_rt)),
             columns=["T%03d" % ti_ref for ti_ref in turbs_ref_list[ti]],
         )
 
     for ti in turbine_list:
-        print("Matching curves for turbine %03d..." % ti)
+        logger.info("Matching curves for turbine %03d..." % ti)
         ref_turb_subset = turbs_ref_list[ti]
         ref_turb_subset = [
-            r
-            for r in ref_turb_subset
-            if all(np.isnan(bias_output_list[ti]["T%03d" % r]))
+            r for r in ref_turb_subset if all(np.isnan(bias_output_list[ti]["T%03d" % r]))
         ]
 
         for ii, idx_chunk in enumerate(idx_chunks):
             df_subset = df.loc[idx_chunk]
 
             for ti_ref in ref_turb_subset:
                 wd_ref = np.array(df_subset["wd_%03d" % (ti_ref)])
                 wd_turb = np.array(df_subset["wd_%03d" % ti])
 
                 wd_ref = wrap_360(wd_ref)
                 wd_turb = wrap_360(wd_turb)
 
                 if sum(np.isnan(wd_turb)) / len(wd_turb) < nan_thrshld:
                     dx_opt, J_opt = opt.match_y_curves_by_offset(
-                        yref=wd_ref, 
+                        yref=wd_ref,
                         ytest=wd_turb,
                         angle_wrapping=True,
                     )
-                    # fig, ax = plt.subplots()
-                    # ax.plot(wrap_360(wd_turb_sub - dx_opt), 'o')
-                    # ax.plot(wd_ref_sub, 'o')
-                    # plt.show()
+
                 else:
                     dx_opt = np.nan
                 bias_output_list[ti].loc[ii, "T%03d" % ti_ref] = dx_opt
                 if ti in turbs_ref_list[ti_ref]:
                     bias_output_list[ti_ref].loc[ii, "T%03d" % ti] = -dx_opt
-                # print('Estimated dx_opt = %.3f, J_opt = %.3f' % (dx_opt, J_opt))
-                # plt.show()
 
-        print(bias_output_list[ti])
+        logger.info(bias_output_list[ti])
 
     # Find turbines where dx barely changes (low variance)
     turb_is_clean = ["bad" for _ in turbine_list]
     for ti in turbine_list:
         df_out = bias_output_list[ti]
         for ti_ref in turbs_ref_list[ti]:
             # If synced by less than 5 degrees std, then both OK
             if np.nanstd(df_out["T%03d" % ti_ref]) < 5.0:
                 turb_is_clean[ti] = "clean"
                 turb_is_clean[ti_ref] = "clean"
             else:
-                if (turb_is_clean[ti] == "clean") & (
-                    turb_is_clean[ti_ref] == "clean"
-                ):
+                if (turb_is_clean[ti] == "clean") & (turb_is_clean[ti_ref] == "clean"):
                     turb_is_clean[ti] = "disputed"
                     turb_is_clean[ti_ref] = "disputed"
 
     for ti in turbine_list:
         if turb_is_clean[ti] == "disputed":
-            print(
+            logger.info(
                 "Turbine %03d may or may not have jumps in WD measurement calibration. [DISPUTED]"
                 % ti
             )
         elif turb_is_clean[ti] == "clean":
-            print(
+            logger.info(
                 "Turbine %03d seems to have no jumps in its WD measurement calibration. [CLEAN]"
                 % ti
             )
         elif turb_is_clean[ti] == "bad":
-            print(
-                "Turbine %03d seems to have one or multiple jumps in its WD measurement calibration. [BAD]"
-                % ti
+            logger.info(
+                "Turbine %03d seems to have one or multiple jumps in "
+                "its WD measurement calibration. [BAD]" % ti
             )
 
     if plot_figure:
         # Plot layout and colormap
         fig, ax = plt.subplots(figsize=(14, 5))
         for ti in turbine_list:
             if turb_is_clean[ti] == "clean":
                 clr = "green"
             elif turb_is_clean[ti] == "bad":
                 clr = "red"
             elif turb_is_clean[ti] == "disputed":
                 clr = "orange"
 
             ax.plot(
-                fi.layout_x[ti],
-                fi.layout_y[ti],
+                fm.layout_x[ti],
+                fm.layout_y[ti],
                 "o",
                 markersize=15,
                 markerfacecolor=clr,
                 markeredgewidth=0.0,
             )
             ax.text(
-                fi.layout_x[ti] + 100,
-                fi.layout_y[ti],
+                fm.layout_x[ti] + 100,
+                fm.layout_y[ti],
                 "T%03d (%s)" % (ti, turb_is_clean[ti]),
                 color="black",
             )
         fig.tight_layout()
 
     return turb_is_clean
```

### Comparing `flasc-1.4.2/flasc/turbine_analysis/ws_pow_filtering.py` & `flasc-2.0/flasc/data_processing/filtering.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,80 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
+import itertools
 
-import pandas as pd
 import matplotlib.pyplot as plt
 import numpy as np
-import itertools
-
-from ..turbine_analysis.find_sensor_faults import find_sensor_stuck_faults
-from .. import utilities as flascutils
-from ..dataframe_operations import dataframe_filtering as dff
-
-from bokeh.plotting import ColumnDataSource, figure
+import pandas as pd
 from bokeh.models import Legend
 from bokeh.palettes import Category20_20 as palette
+from bokeh.plotting import ColumnDataSource, figure
+from scipy.interpolate import interp1d
+
+from flasc.data_processing import dataframe_manipulations as dfm
+from flasc.data_processing.find_sensor_faults import find_sensor_stuck_faults
+from flasc.logging_manager import LoggingManager
+from flasc.utilities import utilities as flascutils
+
+logger_manager = LoggingManager()  # Instantiate LoggingManager
+logger = logger_manager.logger  # Obtain the reusable logger
+
+
+def df_get_no_faulty_measurements(df, turbine):
+    if isinstance(turbine, str):
+        turbine = int(turbine)
+    entryisnan = np.isnan(df["pow_%03d" % turbine].astype(float))
+    # cols = [s for s in df.columns if s[-4::] == ('_%03d' % turbine)]
+    # entryisnan = (np.sum(np.isnan(df[cols]),axis=1) > 0)
+    N_isnan = np.sum(entryisnan)
+    return N_isnan
+
 
+def df_mark_turbdata_as_faulty(df, cond, turbine_list, exclude_columns=[]):
+    if isinstance(turbine_list, (np.integer, int)):
+        turbine_list = [turbine_list]
 
-class ws_pw_curve_filtering:
+    for ti in turbine_list:
+        cols = [s for s in df.columns if s[-4::] == ("_%03d" % ti) and s not in exclude_columns]
+        df.loc[cond, cols] = None  # Delete measurements
+
+    return df
+
+
+class FlascFilter:
     """This class allows a user to filter turbine data based on the
     wind-speed power curve. This class includes several useful filtering
     methods:
         1. Filtering based on prespecified boxes/windows. Any data outside
            of the specified box is considered faulty.
         2. Filtering based on x-wise distance from the mean power curve. Any
            data too far off the mean curve is considered faulty.
         3. Filtering based on the standard deviation from the mean power
            curve. This is slightly different from (2) in the point that
            it allows the user to consider variations in standard deviation
            per power bin.
     """
-    def __init__(self, df):
+
+    def __init__(self, df, turbine_names=None):
         """Initializes the class.
 
         Args:
             df ([pd.DataFrame]): Dataframe containing the turbine data,
                 formatted in the generic SCADA data format. Namely, the
                 dataframe should at the very least contain the columns:
                   * Time of each measurement: time
-                  * Wind speed of each turbine: ws_000, ws_001, ... 
+                  * Wind speed of each turbine: ws_000, ws_001, ...
                   * Power production of each turbine: pow_000, pow_001, ...
         """
 
         # Write dataframe to self
         self._df_initial = df.copy()
         self.reset_filters()
 
+        # Save the turbine names
+        self.turbine_names = turbine_names
+
     # Private methods
     def _get_all_unique_flags(self):
         """Private function that grabs all the unique filter flags
         that are available in self.df_filters and returns them
         as a list of strings. This is helpful when plotting the
         various filter sources in a scatter plot, for example.
 
@@ -75,37 +92,37 @@
         return all_flags
 
     def _reset_mean_power_curves(self, ws_bins=np.arange(0.0, 25.5, 0.5)):
         # If uninitialized, create an empty dataframe with NaNs
         pw_curve_dict = dict(
             zip(
                 [f"pow_{ti:03d}" for ti in range(self.n_turbines)],
-                [np.ones(len(ws_bins) - 1) * np.nan] * self.n_turbines
+                [np.ones(len(ws_bins) - 1) * np.nan] * self.n_turbines,
             )
         )
         pw_curve_dict["ws"] = (ws_bins[1::] + ws_bins[0:-1]) / 2
         pw_curve_dict["ws_min"] = ws_bins[0:-1]
         pw_curve_dict["ws_max"] = ws_bins[1::]
         pw_curve_df = pd.DataFrame(pw_curve_dict)
-        
+
         self._pw_curve_ws_bins = ws_bins
         self.pw_curve_df = pw_curve_df
 
     def _get_mean_power_curves(self, df=None, turbine_subset=None):
         """Calculates the mean power production in bins of the wind speed,
         for all turbines in the wind farm.
 
         Args:
             ws_bins ([iteratible], optional): Wind speed bins. Defaults to
                 np.arange(0.0, 25.5, 0.5).
             df ([pd.DataFrame]): Dataframe containing the turbine data,
                 formatted in the generic SCADA data format. Namely, the
                 dataframe should at the very least contain the columns:
                   * Time of each measurement: time
-                  * Wind speed of each turbine: ws_000, ws_001, ... 
+                  * Wind speed of each turbine: ws_000, ws_001, ...
                   * Power production of each turbine: pow_000, pow_001, ...
             turbine_subset (list, optional): List of turbine indices to
                 calculate the mean power curve for. If None is specified,
                 defaults to calculating it for all turbines.
         Returns:
             pw_curve_df ([pd.DataFrame]): Dataframe containing the wind
                 speed bins and the mean power production value for every
@@ -121,61 +138,59 @@
 
         # By default, if unspecified, Calculate power curve for all turbines
         if turbine_subset is None:
             turbine_subset = list(range(self.n_turbines))
 
         # Apply binning to the wind speeds of the turbine(s)
         ws_bin_cuts_subset = [
-            pd.cut(df[f"ws_{ti:03d}"], bins=self._pw_curve_ws_bins)
-            for ti in turbine_subset
+            pd.cut(df[f"ws_{ti:03d}"], bins=self._pw_curve_ws_bins) for ti in turbine_subset
         ]
 
         # Now add the binned wind speeds to the power measurements dataframe
         df_pow_and_ws_bins_subset = pd.concat(
-            [
-                df[["pow_%03d" % ti for ti in turbine_subset]],
-                *ws_bin_cuts_subset
-            ],
-            axis=1
+            [df[["pow_%03d" % ti for ti in turbine_subset]], *ws_bin_cuts_subset], axis=1
         )
 
         # Now group power measurements by their wind speed bin and calculate the median
-        pw_curve_df_subset = pd.concat(
-            [
-            df_pow_and_ws_bins_subset.groupby(by=f"ws_{ti:03d}")[f"pow_{ti:03d}"].median()
-            for ti in turbine_subset
-            ],
-            axis=1
-        ).sort_index().reset_index(drop=True)
+        pw_curve_df_subset = (
+            pd.concat(
+                [
+                    df_pow_and_ws_bins_subset.groupby(by=f"ws_{ti:03d}")[f"pow_{ti:03d}"].median()
+                    for ti in turbine_subset
+                ],
+                axis=1,
+            )
+            .sort_index()
+            .reset_index(drop=True)
+        )
 
         # Update the median power curve for the turbines in turbine_subset
         pw_curve_df[[f"pow_{ti:03d}" for ti in turbine_subset]] = pw_curve_df_subset
 
         # Save the finalized power curve to self and return it to the user
         self.pw_curve_df = pw_curve_df
         return pw_curve_df
 
     # Public methods
     def reset_filters(self):
         """Reset all filter variables and assume all data is clean."""
-    
+
         # Copy the original, unfiltered dataframe from self
-        df = self._df_initial  
+        df = self._df_initial
         self.df = df.reset_index(drop=("time" in df.columns))
         self.n_turbines = flascutils.get_num_turbines(df)
 
         # Reset the dataframe with filter flags to mark all data as clean, initially
         all_clean_array = [
-            ["clean" for _ in range(self.n_turbines)]
-            for _ in range(self.df.shape[0])
+            ["clean" for _ in range(self.n_turbines)] for _ in range(self.df.shape[0])
         ]
         self.df_filters = pd.DataFrame(
             all_clean_array,
             index=self.df.index,
-            columns=["WTG_{:03d}".format(ti) for ti in range(self.n_turbines)]
+            columns=["WTG_{:03d}".format(ti) for ti in range(self.n_turbines)],
         )
 
         # Reset the mean power curves of the turbines
         self._reset_mean_power_curves()
 
     def filter_by_condition(
         self,
@@ -189,24 +204,24 @@
         condition, for a specific turbine or specific set of turbines. This
         provides a platform for user-specific queries to filter and then inspect
         the data with. You can call this function multiple times and the filters
         will aggregate chronologically. This filter directly cuts down the
         dataframe self.df to a filtered subset.
 
         A correct usage is, for example:
-            ws_pow_filtering.filter_by_condition(
-                condition=(ws_pow_filtering.df["pow_{:03d}".format(ti)] < -1.0e-6),
+            FlascFilter.filter_by_condition(
+                condition=(FlascFilter.df["pow_{:03d}".format(ti)] < -1.0e-6),
                 label="Power below zero",
                 ti=ti,
                 verbose=True,
             )
 
         and:
-            ws_pow_filtering.filter_by_condition(
-                condition=(ws_pow_filtering.df["is_operation_normal_{:03d}".format(ti)] == False),
+            FlascFilter.filter_by_condition(
+                condition=(FlascFilter.df["is_operation_normal_{:03d}".format(ti)] == False),
                 label="Self-flagged (is_operation_normal==False)",
                 ti=ti,
                 verbose=True,
             )
 
         Args:
             condition (iteratible): List or array-like variable with bool entries
@@ -215,15 +230,15 @@
                 high wind speeds but low power productions, or NaNs, self-flagged
                 status variables.
             label (str): Name or description of the fault/condition that is flagged.
             ti (int): Turbine indentifier, typically an integer, but may also be a
                 list. This flags the measurements of all these turbines as faulty
                 for which condition==True.
             verbose (bool, optional): Print information to console. Defaults to True.
-            apply_filters_to_df (bool, optional): Assign the flagged measurements in 
+            apply_filters_to_df (bool, optional): Assign the flagged measurements in
                 self.df directly as NaN. Defaults to True.
 
         Returns:
             df_out: The filtered dataframe. All measurements that are flagged as faulty
                 are overwritten by "None"/"NaN". If apply_filters_to_df==True, then this
                 dataframe is equal to the internally filtered dataframe 'self.df'.
         """
@@ -236,47 +251,53 @@
         df_in = self.df
 
         # Create standalone copy that we can manipulate, if apply_filters_to_df==False
         if not apply_filters_to_df:
             df_in = df_in.copy()
 
         # Mark data as faulty on the dataframe
-        N_pre = [dff.df_get_no_faulty_measurements(df_in, tii) for tii in ti]
-        df_out = dff.df_mark_turbdata_as_faulty(df=df_in, cond=condition, turbine_list=ti)
+        N_pre = [df_get_no_faulty_measurements(df_in, tii) for tii in ti]
+        df_out = df_mark_turbdata_as_faulty(df=df_in, cond=condition, turbine_list=ti)
 
         # Print the reduction in useful data to the console, if verbose
         if verbose:
             for iii, tii in enumerate(ti):
-                N_post = dff.df_get_no_faulty_measurements(df_out, tii)
-                print(
-                    "Faulty measurements for WTG {:03d} increased from {:.3f} % to {:.3f} %. Reason: '{:s}'.".format(
-                        tii, 100.0 * N_pre[iii] / df_in.shape[0], 100.0 * N_post / df_in.shape[0], label
+                N_post = df_get_no_faulty_measurements(df_out, tii)
+                logger.info(
+                    (
+                        "Faulty measurements for WTG {:03d} increased from {:.3f} % to {:.3f} "
+                        "%. Reason: '{:s}'."
+                    ).format(
+                        tii,
+                        100.0 * N_pre[iii] / df_in.shape[0],
+                        100.0 * N_post / df_in.shape[0],
+                        label,
                     )
                 )
 
         if apply_filters_to_df:
             # Update dataframe and filter labels
-            for tii in ti:  
+            for tii in ti:
                 self.df_filters.loc[condition, "WTG_{:03d}".format(tii)] = label
 
                 # Clear the mean power curves. Namely, with this new filtering application
                 # the mean power curves must be recalculated.
                 self.pw_curve_df[f"pow_{tii:03d}"] = None  # Set as Nones
 
         return df_out
 
     def filter_by_sensor_stuck_faults(
-            self,
-            columns: list,
-            ti: int,
-            n_consecutive_measurements: int = 3,
-            stddev_threshold: float = 0.001,
-            plot: bool = False,
-            verbose: bool = True
-        ):
+        self,
+        columns: list,
+        ti: int,
+        n_consecutive_measurements: int = 3,
+        stddev_threshold: float = 0.001,
+        plot: bool = False,
+        verbose: bool = True,
+    ):
         """Filter the turbine measurements for sensor-stuck type of faults. This is
         the situation where a turbine measurement reads the exact same value for
         multiple consecutive timestamps. This typically indicates a "frozen" sensor
         rather than a true physical effect. This is particularly the case for
         signals that are known to change at a high rate and are measured with high
         precision, e.g., wind speed and wind direction measurements.
 
@@ -286,20 +307,20 @@
                 which are the wind speed and wind direction for turbine 0. We can
                 safely assume that those measurements should change between every
                 10-minute measurement. Note that you may not want to include "pow_000",
                 since that measurement may be constant for longer periods of time even
                 during normal operation, e.g., when the turbine is shutdown at very
                 low wind speeds or when the turbine is operating above rated wind
                 speed. Note that if any of the signals in 'columns' is flagged as
-                frozen ("stuck"), all measurements of that turbine will be marked 
+                frozen ("stuck"), all measurements of that turbine will be marked
                 faulty.
             ti (int): The turbine identifier for which its measurements should be
                 flagged as faulty when the signals in the columns are found to be
                 frozen ("stuck"). This is typically the turbine number that corresponds
-                to the columns, e.g., if you use  columns=["ws_000", "wd_000"] then 
+                to the columns, e.g., if you use  columns=["ws_000", "wd_000"] then
                 ti=0, and if you use  ["ws_003", "wd_003"] you use ti=3.
             n_consecutive_measurements (int, optional): Number of consecutive
                 measurements that should read the same value for the measurement to be
                 considered "frozen". Defaults to 3.
             stddev_threshold (float, optional): Threshold value, typically a low number.
                 If the set of consecutive measurements do not differ by more than this
                 value, then the measurements is considered stuck. Defaults to 0.001.
@@ -397,15 +418,15 @@
         # iterative nature of the problem.
         df_initial_filtered = self.df[[f"ws_{ti:03d}", f"pow_{ti:03d}"]].copy()
 
         # Iteratively filter data and recalculate the mean power curves
         self._get_mean_power_curves(turbine_subset=[ti])
         for ii in range(no_iterations):
             # Only print final iteration
-            is_final_iteration = (ii == no_iterations - 1)
+            is_final_iteration = ii == no_iterations - 1
 
             # Create upper and lower bounds around mean curve
             df_xy = self.pw_curve_df.copy()
             x_full = np.array(df_xy["ws"], dtype=float)
             x = x_full[x_full < cutoff_ws]  # Only filter until 15 m/s
             self.pw_curve_df_bounds = pd.DataFrame({"ws": x})
 
@@ -430,23 +451,21 @@
                 lb_pow[jjj] = jjj / 1000.0
                 jjj = jjj + 1
 
             # Ensure non-decreasing for lower half of wind speeds
             id_center = np.argmin(np.abs(lb_ws - 9.0))  # Assume value is fine near 9 m/s
             lb_ws_l = lb_ws[0:id_center]
             lb_pow_l = lb_pow[0:id_center]
-            good_ids = (
-                np.hstack([(np.diff(lb_pow_l) >= 0.0), True])
-                & 
-                (~np.isnan(lb_pow[0:id_center]))
+            good_ids = np.hstack([(np.diff(lb_pow_l) >= 0.0), True]) & (
+                ~np.isnan(lb_pow[0:id_center])
             )
             good_ids[0] = True
             lb_pow_l = np.interp(lb_ws_l, lb_ws_l[good_ids], lb_pow_l[good_ids])
             lb_pow[0:id_center] = lb_pow_l
-            non_nans = (~np.isnan(lb_pow) & ~np.isnan(lb_ws))
+            non_nans = ~np.isnan(lb_pow) & ~np.isnan(lb_ws)
             lb_pow = lb_pow[non_nans]
             lb_ws = lb_ws[non_nans]
 
             # Specify right side bound and ensure monotonically increasing
             rb_ws = x * m_ws_rb + ws_deadband / 2.0
             rb_pow = y * m_pow_rb - pow_deadband / 2.0
 
@@ -456,23 +475,21 @@
                 rb_pow[jjj] = jjj / 1000.0
                 jjj = jjj + 1
 
             # Ensure non-decreasing for lower half of wind speeds
             id_center = np.argmin(np.abs(rb_ws - 9.0))  # Assume value is fine near 9 m/s
             rb_ws_l = rb_ws[0:id_center]
             rb_pow_l = rb_pow[0:id_center]
-            good_ids = (
-                np.hstack([(np.diff(rb_pow_l) >= 0.0), True])
-                & 
-                (~np.isnan(rb_pow[0:id_center]))
+            good_ids = np.hstack([(np.diff(rb_pow_l) >= 0.0), True]) & (
+                ~np.isnan(rb_pow[0:id_center])
             )
             good_ids[0] = True
             rb_pow_l = np.interp(rb_ws_l, rb_ws_l[good_ids], rb_pow_l[good_ids])
             rb_pow[0:id_center] = rb_pow_l
-            non_nans = (~np.isnan(rb_pow) & ~np.isnan(rb_ws))
+            non_nans = ~np.isnan(rb_pow) & ~np.isnan(rb_ws)
             rb_pow = rb_pow[non_nans]
             rb_ws = rb_ws[non_nans]
 
             # Finally interpolate
             ws_lb = np.interp(
                 x=pow_array,
                 xp=lb_pow,
@@ -490,15 +507,15 @@
 
             # Filter the dataframe according to hypothetical power curve
             df_iteration = self.filter_by_condition(
                 condition=(ws_array < ws_lb) | (ws_array > ws_rb),
                 label="Mean power curve outlier",
                 ti=ti,
                 verbose=is_final_iteration,  # If final iteration, be verbose
-                apply_filters_to_df=is_final_iteration,  # If final iteration, save dataframe to self
+                apply_filters_to_df=is_final_iteration,  # If final , save dataframe to self
             )
 
             # Recalculate the mean power curve based on current iteration's filtered dataframe
             self._get_mean_power_curves(df=df_iteration, turbine_subset=[ti])
             self.pw_curve_df_bounds["pow_%03d_lb" % ti] = np.interp(
                 x=x,
                 xp=lb_ws,
@@ -514,29 +531,29 @@
                 right=np.nan,
             )
 
         return self.df
 
     def filter_by_floris_power_curve(
         self,
-        fi,
+        fm,
         ti,
         m_ws_lb=0.95,
         m_pow_lb=1.01,
         m_ws_rb=1.05,
         m_pow_rb=0.99,
         ws_deadband=0.50,
         pow_deadband=20.0,
         cutoff_ws=20.0,
     ):
         """Filter the data by offset from the floris power curve in x-
         directions.
 
         Args:
-            fi (FlorisInterface): The FlorisInterface object for the farm
+            fm (FlorisModel): The FlorisModel object for the farm
             m_ws_lb (float, optional): Multiplier on the wind speed defining
             the left bound for the power curve. Any data to the left of this
             curve is considered faulty. Defaults to 0.95.
             m_pow_lb (float, optional): Multiplier on the power defining
             the left bound for the power curve. Any data to the left of this
             curve is considered faulty. Defaults to 1.01.
             m_ws_rb (float, optional): Multiplier on the wind speed defining
@@ -555,34 +572,32 @@
             power curve is calculated and the data is filtered for. You should
             make sure this variable is set to a value above the rated wind
             speed and below the cut-out wind speed. If you are experiencing
             problems with data filtering and your data points have a downward
             trend near the high wind speeds, try decreasing this variable's
             value to 15.0.
         """
-        print("Filtering data by deviations from the floris power curve...")
+        logger.info("Filtering data by deviations from the floris power curve...")
 
         # Create upper and lower bounds around floris curve
 
         # Get mean power curves first, if not yet calculated
         if self.pw_curve_df[f"pow_{ti:03d}"].isna().all():
             self._get_mean_power_curves(turbine_subset=[ti])
 
         df_xy = self.pw_curve_df.copy()
-        rho = fi.floris.flow_field.air_density
-        for ti in range(len(fi.layout_x)):
-            fi_turb = fi.floris.farm.turbine_definitions[ti]
-            Ad = 0.25 * np.pi * fi_turb["rotor_diameter"] ** 2.0
-            ws_array = np.array(fi_turb["power_thrust_table"]["wind_speed"])
-            cp_array = np.array(fi_turb["power_thrust_table"]["power"])
-            pow_array = (
-                0.5 * rho * ws_array ** 3.0 * Ad * cp_array * 1.0e-3
-            )
-            df_xy.loc[df_xy.index, "pow_{:03d}".format(ti)] = (
-                np.interp(xp=ws_array, fp=pow_array, x=df_xy["ws"])
+        rho = fm.core.flow_field.air_density
+        for ti in range(len(fm.layout_x)):
+            fm_turb = fm.core.farm.turbine_definitions[ti]
+            Ad = 0.25 * np.pi * fm_turb["rotor_diameter"] ** 2.0
+            ws_array = np.array(fm_turb["power_thrust_table"]["wind_speed"])
+            cp_array = np.array(fm_turb["power_thrust_table"]["power"])
+            pow_array = 0.5 * rho * ws_array**3.0 * Ad * cp_array * 1.0e-3
+            df_xy.loc[df_xy.index, "pow_{:03d}".format(ti)] = np.interp(
+                xp=ws_array, fp=pow_array, x=df_xy["ws"]
             )
 
         x_full = np.array(df_xy["ws"], dtype=float)
         x = x_full[x_full < cutoff_ws]
         self.pw_curve_df_bounds = pd.DataFrame({"ws": x})
 
         y = np.array(df_xy["pow_%03d" % ti], dtype=float)
@@ -606,23 +621,19 @@
             lb_pow[jjj] = jjj / 1000.0
             jjj = jjj + 1
 
         # Ensure non-decreasing for lower half of wind speeds
         id_center = np.argmin(np.abs(lb_ws - 9.0))  # Assume value is fine near 9 m/s
         lb_ws_l = lb_ws[0:id_center]
         lb_pow_l = lb_pow[0:id_center]
-        good_ids = (
-            np.hstack([(np.diff(lb_pow_l) >= 0.0), True])
-            & 
-            (~np.isnan(lb_pow[0:id_center]))
-        )
+        good_ids = np.hstack([(np.diff(lb_pow_l) >= 0.0), True]) & (~np.isnan(lb_pow[0:id_center]))
         good_ids[0] = True
         lb_pow_l = np.interp(lb_ws_l, lb_ws_l[good_ids], lb_pow_l[good_ids])
         lb_pow[0:id_center] = lb_pow_l
-        non_nans = (~np.isnan(lb_pow) & ~np.isnan(lb_ws))
+        non_nans = ~np.isnan(lb_pow) & ~np.isnan(lb_ws)
         lb_pow = lb_pow[non_nans]
         lb_ws = lb_ws[non_nans]
 
         # Specify right side bound and ensure monotonically increasing
         rb_ws = x * m_ws_rb + ws_deadband / 2.0
         rb_pow = y * m_pow_rb - pow_deadband / 2.0
 
@@ -632,23 +643,19 @@
             rb_pow[jjj] = jjj / 1000.0
             jjj = jjj + 1
 
         # Ensure non-decreasing for lower half of wind speeds
         id_center = np.argmin(np.abs(rb_ws - 9.0))  # Assume value is fine near 9 m/s
         rb_ws_l = rb_ws[0:id_center]
         rb_pow_l = rb_pow[0:id_center]
-        good_ids = (
-            np.hstack([(np.diff(rb_pow_l) >= 0.0), True])
-            & 
-            (~np.isnan(rb_pow[0:id_center]))
-        )
+        good_ids = np.hstack([(np.diff(rb_pow_l) >= 0.0), True]) & (~np.isnan(rb_pow[0:id_center]))
         good_ids[0] = True
         rb_pow_l = np.interp(rb_ws_l, rb_ws_l[good_ids], rb_pow_l[good_ids])
         rb_pow[0:id_center] = rb_pow_l
-        non_nans = (~np.isnan(rb_pow) & ~np.isnan(rb_ws))
+        non_nans = ~np.isnan(rb_pow) & ~np.isnan(rb_ws)
         rb_pow = rb_pow[non_nans]
         rb_ws = rb_ws[non_nans]
 
         # Finally interpolate
         ws_lb = np.interp(
             x=pow_array,
             xp=lb_pow,
@@ -714,34 +721,38 @@
                 turbine.
             calculate_missing (bool, optional): Calculate the median power
                 curves for the turbines for the turbines of which their
                 power curves were previously not yet calculated.
         """
         if calculate_missing and (self.pw_curve_df.isna().all(axis=0).any()):
             turbine_subset = np.where(
-                self.pw_curve_df[[f"pow_{ti:03d}" for ti in range(self.n_turbines)]].isna().all(axis=0)
+                self.pw_curve_df[[f"pow_{ti:03d}" for ti in range(self.n_turbines)]]
+                .isna()
+                .all(axis=0)
             )[0]
             self._get_mean_power_curves(turbine_subset=turbine_subset)
 
         return self.pw_curve_df
 
-    def plot_farm_mean_power_curve(self, fi=None):
+    def plot_farm_mean_power_curve(self, fm=None):
         """Plot all turbines' power curves in a single figure. Also estimate
         and plot a mean turbine power curve.
 
         Args:
-            fi (FlorisInterface): The FlorisInterface object for the farm. If
+            fm (FlorisModel): The FlorisModel object for the farm. If
               specified by the user, then the farm-average turbine power curve
               from FLORIS will be plotted on top of the SCADA-based power curves.
         """
 
         # Get mean power curves for the turbines that are not yet calculated
         if self.pw_curve_df.isna().all(axis=0).any():
             turbine_subset = np.where(
-                self.pw_curve_df[[f"pow_{ti:03d}" for ti in range(self.n_turbines)]].isna().all(axis=0)
+                self.pw_curve_df[[f"pow_{ti:03d}" for ti in range(self.n_turbines)]]
+                .isna()
+                .all(axis=0)
             )[0]
             self._get_mean_power_curves(turbine_subset=turbine_subset)
 
         # Create the figure
         fig, ax = plt.subplots()
         x = np.array(self.pw_curve_df["ws"], dtype=float)
         for ti in range(self.n_turbines):
@@ -757,39 +768,27 @@
             np.array(pow_mean_array + 2 * pow_std_array),
             color="tab:red",
             label="Uncertainty bounds (2 std. dev.)",
             alpha=0.30,
         )
         ax.plot(x, pow_mean_array, color="tab:red", label="Mean curve")
 
-        if fi is not None:
-            fi_turb = fi.floris.farm.turbine_definitions[ti]
-            Ad = 0.25 * np.pi * fi_turb["rotor_diameter"] ** 2.0
-            ws_array = np.array(fi_turb["power_thrust_table"]["wind_speed"])
-            cp_array = np.array(fi_turb["power_thrust_table"]["power"])
-            rho = fi.floris.flow_field.air_density
-            pow_array = (
-                0.5 * rho * ws_array ** 3.0 * Ad * cp_array * 1.0e-3
-            )
+        if fm is not None:
+            fm_turb = fm.core.farm.turbine_definitions[ti]
+            ws_array = np.array(fm_turb["power_thrust_table"]["wind_speed"])
+            pow_array = np.array(fm_turb["power_thrust_table"]["power"])
             ax.plot(ws_array, pow_array, "--", label="FLORIS curve")
 
         ax.legend()
         ax.set_title("Mean of all turbine power curves with UQ")
         return fig, ax
 
-
     def plot_filters_custom_scatter(
-            self,
-            ti,
-            x_col,
-            y_col,
-            xlabel="Wind speed (m/s)",
-            ylabel="Power (kW)",
-            ax=None
-        ):
+        self, ti, x_col, y_col, xlabel="Wind speed (m/s)", ylabel="Power (kW)", ax=None
+    ):
         """Plot the filtered data in a scatter plot, categorized
         by the source of their filter/fault. This is a generic
         function that allows the user to plot various numeric
         variables on the x and y axis.
 
         Args:
             ti (int): Turbine identifier. This is used to determine
@@ -816,53 +815,57 @@
         # Get filter dataframe
         df_f = self.df_filters["WTG_{:03d}".format(ti)]
         all_flags = self._get_all_unique_flags()
         N = df_f.shape[0]
 
         # For each flagging condition, plot the results
         for flag in all_flags:
-            ids = (df_f == flag)
+            ids = df_f == flag
             df_subset = self._df_initial.loc[ids]
             percentage = 100.0 * np.sum(ids) / N
             if (
-                any(ids) and
-                (not df_subset[x_col].isna().all()) and
-                (not df_subset[y_col].isna().all())
+                any(ids)
+                and (not df_subset[x_col].isna().all())
+                and (not df_subset[y_col].isna().all())
             ):
                 ax.plot(
                     df_subset[x_col],
                     df_subset[y_col],
                     ".",
                     markersize=5,
                     alpha=0.15,
                     rasterized=True,
                     label="{:s} ({:.2f} %)".format(flag, percentage),
                 )
 
         lgd = ax.legend()
-        for l in lgd.legendHandles:
-            l.set_alpha(1)  # Force alpha in legend to 1.0
+        for h in lgd.legendHandles:
+            h.set_alpha(1)  # Force alpha in legend to 1.0
+
+        if self.turbine_names is not None:
+            ax.set_title(f"WTG {self.turbine_names[ti]}, [{ti:03d}]: Filters")
+        else:
+            ax.set_title("WTG {:03d}: Filters".format(ti))
 
-        ax.set_title("WTG {:03d}: Filters".format(ti))
         ax.set_xlabel(xlabel)
         ax.set_ylabel(ylabel)
         ax.grid(True)
-    
+
         return ax
 
     def plot_filters_custom_scatter_bokeh(
-            self,
-            ti,
-            x_col,
-            y_col,
-            title="Wind-speed vs. power curve",
-            xlabel="Wind speed (m/s)",
-            ylabel="Power (kW)",
-            p=None,
-        ):
+        self,
+        ti,
+        x_col,
+        y_col,
+        title="Wind-speed vs. power curve",
+        xlabel="Wind speed (m/s)",
+        ylabel="Power (kW)",
+        p=None,
+    ):
         """Plot the filtered data in a scatter plot, categorized
         by the source of their filter/fault. This is a generic
         function that allows the user to plot various numeric
         variables on the x and y axis.
 
         Args:
             ti (int): Turbine identifier. This is used to determine
@@ -882,80 +885,82 @@
 
         Returns:
             ax: The figure axis in which the scatter plot is drawn.
         """
         # Create figure, if not specified
 
         bokeh_tooltips = [
-                ("(x,y)", "($x, $y)"),
-                ("time", "@time"),
-                ("index", "$index"),
+            ("(x,y)", "($x, $y)"),
+            ("time", "@time"),
+            ("index", "$index"),
         ]
 
         if p is None:
             p = figure(
                 title=title,
                 width=800,
                 height=550,
-                sizing_mode='stretch_width',
+                sizing_mode="stretch_width",
                 x_axis_label=xlabel,
                 y_axis_label=ylabel,
                 tooltips=bokeh_tooltips,
             )
-            p.add_layout(Legend(title="Data category"), 'right')
+            p.add_layout(Legend(title="Data category"), "right")
 
         # Get filter dataframe
         df_f = self.df_filters["WTG_{:03d}".format(ti)]
         all_flags = self._get_all_unique_flags()
         N = df_f.shape[0]
 
         # For each flagging condition, plot the results
         colors = itertools.cycle(palette)
         for flag in all_flags:
-            ids = (df_f == flag)
+            ids = df_f == flag
             df_subset = self._df_initial.loc[ids]
             percentage = 100.0 * np.sum(ids) / N
             label = "{:s} ({:.2f} %)".format(flag, percentage)
             alpha = 0.65
             size = 5
             color = next(colors)
             if (
-                any(ids) and
-                (not df_subset[x_col].isna().all()) and
-                (not df_subset[y_col].isna().all())
+                any(ids)
+                and (not df_subset[x_col].isna().all())
+                and (not df_subset[y_col].isna().all())
             ):
-                source = ColumnDataSource(data=dict(
-                    x=df_subset[x_col],
-                    y=df_subset[y_col],
-                    time=list(df_subset["time"].astype(str)),
-                ))
+                source = ColumnDataSource(
+                    data=dict(
+                        x=df_subset[x_col],
+                        y=df_subset[y_col],
+                        time=list(df_subset["time"].astype(str)),
+                    )
+                )
                 p.circle(
                     "x",
                     "y",
                     source=source,
                     fill_alpha=alpha,
                     color=color,
                     line_color=None,
                     size=size,
-                    legend_label=label
+                    legend_label=label,
                 )
-    
+
         p.legend.title = "Data category"
         p.legend.click_policy = "hide"
         p.toolbar.active_inspect = None
 
         return p
 
-    def plot_filters_in_ws_power_curve(self, ti, fi=None, ax=None):
+    def plot_filters_in_ws_power_curve(self, ti, fm=None, ax=None):
         """Plot the wind speed power curve and connect each faulty datapoint
         to the label it was classified as faulty with.
 
         Args:
             ti (int): Turbine number which should be plotted.
-            fi (FlorisInterface, optional): floris object. If not None, will
+            fm (FlorisModel, optional): floris object. If not None, will
             use this to plot the turbine power curves as implemented in floris.
             Defaults to None.
             ax (plt.Axis): Pyplot Axis object.
         """
 
         if ax is None:
             _, ax = plt.subplots(figsize=(10, 5))
@@ -972,23 +977,19 @@
         ax.plot(
             self.pw_curve_df["ws"],
             self.pw_curve_df["pow_%03d" % ti],
             "--",
             label="Approximate power curve",
         )
 
-        if fi is not None:
-            fi_turb = fi.floris.farm.turbine_definitions[ti]
-            Ad = 0.25 * np.pi * fi_turb["rotor_diameter"] ** 2.0
-            ws_array = np.array(fi_turb["power_thrust_table"]["wind_speed"])
-            cp_array = np.array(fi_turb["power_thrust_table"]["power"])
-            rho = fi.floris.flow_field.air_density
-            pow_array = (
-                0.5 * rho * ws_array ** 3.0 * Ad * cp_array * 1.0e-3
-            )
+        if fm is not None:
+            fm_turb = fm.core.farm.turbine_definitions[ti]
+            ws_array = np.array(fm_turb["power_thrust_table"]["wind_speed"])
+            pow_array = np.array(fm_turb["power_thrust_table"]["power"])
+
             ax.plot(ws_array, pow_array, "--", label="FLORIS curve")
 
         if self.pw_curve_df_bounds is not None:
             ax.plot(
                 self.pw_curve_df_bounds["ws"],
                 self.pw_curve_df_bounds["pow_%03d_lb" % ti],
                 "--",
@@ -998,31 +999,34 @@
                 self.pw_curve_df_bounds["ws"],
                 self.pw_curve_df_bounds["pow_%03d_rb" % ti],
                 "--",
                 label="Right bound for power curve",
             )
 
         lgd = ax.legend()
-        for l in lgd.legendHandles:
-            l.set_alpha(1)  # Force alpha in legend to 1.0
+        for h in lgd.legendHandles:
+            h.set_alpha(1)  # Force alpha in legend to 1.0
 
-        ax.set_title("WTG {:03d}: Filters".format(ti))
+        if self.turbine_names is not None:
+            ax.set_title(f"WTG {self.turbine_names[ti]}, [{ti:03d}]: Filters")
+        else:
+            ax.set_title("WTG {:03d}: Filters".format(ti))
         ax.set_xlabel("Wind speed (m/s)")
         ax.set_ylabel("Power (kW)")
         ax.grid(True)
 
         return ax
 
-    def plot_postprocessed_in_ws_power_curve(self, ti, fi=None, ax=None):
+    def plot_postprocessed_in_ws_power_curve(self, ti, fm=None, ax=None):
         """Plot the wind speed power curve and mark faulty data according to
         their filters.
 
         Args:
             ti (int): Turbine number which should be plotted.
-            fi (FlorisInterface, optional): floris object. If not None, will
+            fm (FlorisModel, optional): floris object. If not None, will
             use this to plot the turbine power curves as implemented in floris.
             Defaults to None.
             ax (Matplotlib.pyplot Axis, optional): Axis to plot in. If None is
                specified, creates a new figure and axis. Defaults to None.
         """
 
         if ax is None:
@@ -1049,23 +1053,19 @@
         ax.plot(
             self.pw_curve_df["ws"],
             self.pw_curve_df["pow_%03d" % ti],
             "--",
             label="Approximate power curve",
         )
 
-        if fi is not None:
-            fi_turb = fi.floris.farm.turbine_definitions[ti]
-            Ad = 0.25 * np.pi * fi_turb["rotor_diameter"] ** 2.0
-            ws_array = np.array(fi_turb["power_thrust_table"]["wind_speed"])
-            cp_array = np.array(fi_turb["power_thrust_table"]["power"])
-            rho = fi.floris.flow_field.air_density
-            pow_array = (
-                0.5 * rho * ws_array ** 3.0 * Ad * cp_array * 1.0e-3
-            )
+        if fm is not None:
+            fm_turb = fm.core.farm.turbine_definitions[ti]
+            ws_array = np.array(fm_turb["power_thrust_table"]["wind_speed"])
+            pow_array = np.array(fm_turb["power_thrust_table"]["power"])
+
             ax.plot(ws_array, pow_array, "--", label="FLORIS curve")
 
         if self.pw_curve_df_bounds is not None:
             ax.plot(
                 self.pw_curve_df_bounds["ws"],
                 self.pw_curve_df_bounds["pow_%03d_lb" % ti],
                 "--",
@@ -1075,18 +1075,21 @@
                 self.pw_curve_df_bounds["ws"],
                 self.pw_curve_df_bounds["pow_%03d_rb" % ti],
                 "--",
                 label="Right bound for power curve",
             )
 
         lgd = ax.legend()
-        for l in lgd.legendHandles:
-            l.set_alpha(1)  # Force alpha in legend to 1.0
+        for h in lgd.legendHandles:
+            h.set_alpha(1)  # Force alpha in legend to 1.0
 
-        ax.set_title("WTG {:03d}: Postprocessed dataset".format(ti))
+        if self.turbine_names is not None:
+            ax.set_title(f"WTG {self.turbine_names[ti]}, [{ti:03d}]: Postprocessed dataset")
+        else:
+            ax.set_title("WTG {:03d}: Postprocessed dataset".format(ti))
         ax.set_xlabel("Wind speed (m/s)")
         ax.set_ylabel("Power (kW)")
         ax.grid(True)
 
         return ax
 
     def plot_filters_in_time(self, ti, ax=None):
@@ -1107,22 +1110,30 @@
             _, ax = plt.subplots(figsize=(13, 7))
 
         # Get a list of all flags and then get colors correspondingly
         all_flags = self._get_all_unique_flags()
 
         # Manipulate dataframe to easily plot results
         df_f = self.df_filters["WTG_{:03d}".format(ti)]
-        df_conditional = pd.concat([pd.DataFrame({flag: np.array(df_f==flag, dtype=int)}) for flag in all_flags], axis=1)
+        df_conditional = pd.concat(
+            [pd.DataFrame({flag: np.array(df_f == flag, dtype=int)}) for flag in all_flags], axis=1
+        )
         df_merged = pd.concat([df_conditional, self.df["time"]], axis=1)
-        df_histogram = df_merged.groupby([df_merged["time"].dt.year, df_merged["time"].dt.isocalendar().week]).sum(numeric_only=True)
+        df_histogram = df_merged.groupby(
+            [df_merged["time"].dt.year, df_merged["time"].dt.isocalendar().week]
+        ).sum(numeric_only=True)
 
         # Plot the histogram information
         ax = df_histogram.plot.bar(stacked=True, ax=ax)
         ax.set_ylabel("Count (-)")
-        ax.set_title("WTG {:03d}".format(ti))
+        if self.turbine_names is not None:
+            ax.set_title(f"WTG {self.turbine_names[ti]}, [{ti:03d}]")
+        else:
+            ax.set_title("WTG {:03d}".format(ti))
+
         ax.grid(True)
 
         return ax
 
     def plot_filters_in_time_bokeh(self, ti, p=None):
         """Generate bar plot where each week of data is gathered and its
         filtering results will be shown relative to the data size of each
@@ -1139,44 +1150,152 @@
         """
 
         if p is None:
             p = figure(
                 title="Filters over time",
                 width=800,
                 height=550,
-                sizing_mode='stretch_width',
+                sizing_mode="stretch_width",
                 x_axis_label="Time (year - week)",
                 y_axis_label="Number of data points (-)",
                 # tooltips=bokeh_tooltips,
             )
-            p.add_layout(Legend(title="Data category"), 'right')
+            p.add_layout(Legend(title="Data category"), "right")
 
         # Get a list of all flags and then get colors correspondingly
         all_flags = self._get_all_unique_flags()
 
         # Manipulate dataframe to easily plot results
         df_f = self.df_filters["WTG_{:03d}".format(ti)]
-        df_conditional = pd.concat([pd.DataFrame({flag: np.array(df_f==flag, dtype=int)}) for flag in all_flags], axis=1)
+        df_conditional = pd.concat(
+            [pd.DataFrame({flag: np.array(df_f == flag, dtype=int)}) for flag in all_flags], axis=1
+        )
         df_merged = pd.concat([df_conditional, self.df["time"]], axis=1)
-        df_histogram = df_merged.groupby([df_merged["time"].dt.year, df_merged["time"].dt.isocalendar().week]).sum(numeric_only=True)
+        df_histogram = df_merged.groupby(
+            [df_merged["time"].dt.year, df_merged["time"].dt.isocalendar().week]
+        ).sum(numeric_only=True)
 
         filter_flags = list(df_histogram.columns)
         xlabels = [f"{year}-{week}" for year, week in df_histogram.index]
         x = np.arange(len(list(df_histogram.index)))
 
         heights = np.zeros(len(x), dtype=int)
         colors = itertools.cycle(palette)
         for f in filter_flags:
             y = np.array(df_histogram[f], dtype=int)
-            p.vbar(x=x, bottom=heights, top=heights+y, width=0.7, legend_label=f, color=next(colors))
+            p.vbar(
+                x=x, bottom=heights, top=heights + y, width=0.7, legend_label=f, color=next(colors)
+            )
             heights = heights + y
-        
+
         # Format x-axis
         p.xaxis.major_label_orientation = np.pi / 2.0
         p.xaxis.ticker = x
         p.xaxis.major_label_overrides = dict(zip(x, xlabels))
 
         # Format legend and allow hide/show functionality
         p.legend.title = "Filter"
         p.legend.click_policy = "hide"
 
         return p
+
+
+def filter_df_by_faulty_impacting_turbines(df, ti, df_impacting_turbines, verbose=True):
+    """Assigns a turbine's measurement to NaN for each timestamp for which any of the turbines
+      that are shedding a wake on this turbine is reporting NaN measurements.
+
+    Args:
+        df (pd.DataFrame): Dataframe with SCADA data with measurements
+        formatted according to wd_000, wd_001, wd_002, pow_000, pow_001,
+        pow_002, and so on.
+        ti (integer): Turbine number for which we are filtering the data.
+        Basically, each turbine that impacts that power production of
+        turbine 'ti' by more than 0.1% is required to be reporting a
+        non-faulty measurement. If not, we classify the measurement of
+        turbine 'ti' as faulty because we cannot sufficiently know the
+        inflow conditions of this turbine.
+        df_impacting_turbines (pd.DataFrame): A Pandas DataFrame in the
+        format of:
+
+                               0       1          2   3   4   5   6
+                wd
+                0.0       [6, 5]     [5]     [3, 5]  []  []  []  []
+                3.0          [6]     [5]     [3, 5]  []  []  []  []
+                ...          ...     ...        ...  ..  ..  ..  ..
+                354.0  [6, 5, 3]  [5, 0]     [3, 5]  []  []  []  []
+                357.0     [6, 5]     [5]  [3, 5, 4]  []  []  []  []
+
+        The columns indicate the turbine of interest, i.e., the turbine that
+        is waked, and each row shows which turbines are waking that turbine
+        for that particular wind direction ('wd'). Typically calculated using:
+
+            import flasc.utilities.floris_tools as ftools
+            df_impacting_turbines = ftools.get_all_impacting_turbines(fi)
+
+        verbose (bool, optional): Print information to the console. Defaults
+        to True.
+
+    Returns:
+        pd.DataFrame: The postprocessed dataframe for 'df', filtered for
+        inter-turbine issues like curtailment and turbine downtime.
+    """
+
+    # Get number of turbines
+    n_turbines = dfm.get_num_turbines(df)
+
+    # Drop all measurements where an upstream turbine is affecting this turbine but also has
+    # a NaN measurement itself
+    ws_cols = ["ws_{:03d}".format(ti) for ti in range(n_turbines)]
+    pow_cols = ["pow_{:03d}".format(ti) for ti in range(n_turbines)]
+
+    # Get array of which turbines affect our test turbine
+    wd_array = df["wd"]
+
+    # Create interpolant returning impacting turbines
+    xp = np.array(df_impacting_turbines[ti].index, dtype=float)
+    fp = np.arange(len(xp), dtype=int)
+
+    # Copy values over from 0 to 360 deg
+    if (np.abs(xp[0]) < 0.001) & (np.max(xp) < 360.0):
+        xp = np.hstack([xp, 360.0])
+        fp = np.hstack([fp, fp[0]])
+
+    # Get nearest neighbor indices
+    f = interp1d(x=xp, y=fp, kind="nearest")
+
+    ids = np.array(f(wd_array), dtype=int)
+    turbines_impacted = df_impacting_turbines[ti].values[ids]
+
+    # Organize as matrix for easy manipulations
+    impacting_turbines_matrix = np.zeros((len(wd_array), n_turbines), dtype=bool)
+    for ii, turbines_impacted_onewd in enumerate(turbines_impacted):
+        impacting_turbines_matrix[ii, turbines_impacted_onewd] = True
+
+    # Calculate True/False statement whether any of the turbines shedding a wake on our test_turbine
+    # has a NaN ws or pow measurement
+    test_turbine_impacted_by_nan_ws = np.any(
+        np.isnan(np.array(df[ws_cols], dtype=float)) & impacting_turbines_matrix, axis=1
+    )
+    test_turbine_impacted_by_nan_pow = np.any(
+        np.isnan(np.array(df[pow_cols], dtype=float)) & impacting_turbines_matrix, axis=1
+    )
+    test_turbine_impacted = test_turbine_impacted_by_nan_ws | test_turbine_impacted_by_nan_pow
+
+    # Assign test turbine's measurements to NaN if any turbine that is waking this turbine
+    # is reporting NaN measurements
+    N_pre = df_get_no_faulty_measurements(df, ti)
+    df_out = df_mark_turbdata_as_faulty(
+        df=df,
+        cond=test_turbine_impacted,
+        turbine_list=[ti],
+    )
+    N_post = df_get_no_faulty_measurements(df_out, ti)
+
+    if verbose:
+        logger.info(
+            "Faulty measurements for WTG {:02d} increased from {:.3f} % to {:.3f} %. Reason: "
+            "'Turbine is impacted by faulty upstream turbine'.".format(
+                ti, 100.0 * N_pre / df.shape[0], 100.0 * N_post / df.shape[0]
+            )
+        )
+
+    return df_out
```

### Comparing `flasc-1.4.2/flasc/turbine_analysis/yaw_pow_fitting.py` & `flasc-2.0/flasc/model_fitting/yaw_pow_fitting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,23 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
+import os
 
 import matplotlib.pyplot as plt
 import numpy as np
-import os
+from floris.utilities import wrap_180
 from scipy import optimize as opt
 
-from floris.utilities import wrap_180
+from flasc.logging_manager import LoggingManager
 
-from ..dataframe_operations import dataframe_manipulations as dfm
-from .. import utilities as fsut
+logger_manager = LoggingManager()  # Instantiate LoggingManager
+logger = logger_manager.logger  # Obtain the reusable logger
 
 
-class yaw_pow_fitting():
-    def __init__(self, df, df_upstream=None, ti=0):#, turbine_list='all'):
-        print('Initializing yaw power curve filtering object.')
+class yaw_pow_fitting:
+    def __init__(self, df, df_upstream=None, ti=0):  # , turbine_list='all'):
+        logger.info("Initializing yaw power curve filtering object.")
         # Assign dataframes to self
         # self.df_upstream = df_upstream
         self.set_df(df, df_upstream, ti)
 
         # # Set turbines specified by user
         # self.set_turbine_mode(turbine_list)
 
@@ -37,15 +26,15 @@
         #     raise KeyError('vane_000 not found in dataset.')
 
         # # Get true total number of turbines
         # self.num_turbines_all = fsut.get_num_turbines(df)
         # self.full_turbine_list = range(self.num_turbines_all)
 
         # Set df using only the relevant columns
-        rlvnt_cols = ['pow', 'pow_ref', 'vane', 'wd']
+        rlvnt_cols = ["pow", "pow_ref", "vane", "wd"]
         # rlvnt_cols.extend(['pow_%03d' % ti for ti in range(self.num_turbines_all)])
         # rlvnt_cols.extend(['vane_%03d' % ti for ti in range(self.num_turbines_all)])
         # rlvnt_cols = [c for c in rlvnt_cols if c in df.columns]
         df = df[rlvnt_cols]
 
         # Reset output variables
         self.bins_x = []
@@ -53,21 +42,21 @@
         self.bins_N = []
 
         self.x_opt = [(None, None)]
         self.bins_y_opt = []
 
         # Filter by upstream conditions
         if df_upstream is not None:
-            df_upstr_ti = df_upstream[[ti in tl for tl in df_upstream['turbines']]]
+            df_upstr_ti = df_upstream[[ti in tl for tl in df_upstream["turbines"]]]
             df_upstr_ti = df_upstr_ti.reset_index(drop=True)
             in_range = [False for _ in range(df.shape[0])]
             for i in range(df_upstr_ti.shape[0]):
-                wd_min = df_upstr_ti.loc[i, 'wd_min']
-                wd_max = df_upstr_ti.loc[i, 'wd_max']
-                in_range = in_range | ((df['wd'] >= wd_min) & (df['wd'] <= wd_max))
+                wd_min = df_upstr_ti.loc[i, "wd_min"]
+                wd_max = df_upstr_ti.loc[i, "wd_max"]
+                in_range = in_range | ((df["wd"] >= wd_min) & (df["wd"] <= wd_max))
             df = df.loc[in_range]
 
         self.df = df
 
     # def set_turbine_mode(self, turbine_list):
     #     if isinstance(turbine_list, str):
     #         if turbine_list == 'all':
@@ -75,105 +64,101 @@
     #             turbine_list = range(num_turbines)
     #         else:
     #             raise KeyError('Invalid turbine_list specified.')
 
     #     self.turbine_list = turbine_list
     #     self.num_turbines = len(turbine_list)
 
-    def calculate_curves(self, vane_bounds=(-15., 15.), dv=1.0, Pmin=10.0):
+    def calculate_curves(self, vane_bounds=(-15.0, 15.0), dv=1.0, Pmin=10.0):
         df = self.df
         # df_upstream = self.df_upstream
         # turbine_list = self.turbine_list
 
-        print('Determining yaw-power curve...')
-        # print('  Retrieving relevant dataframe subset...')
-        # rel_cols = ['wd', 'vane_%03d' % ti]
-        # rel_cols.extend(['pow_%03d' % ti for ti in self.full_turbine_list])
-        # rel_cols = [c for c in rel_cols if c in self.df.columns]
-        # df = self.df[rel_cols].copy()
+        logger.info("Determining yaw-power curve...")
 
-
-        # # Get reference power signals
-        # print('  Cutting down dataframe by minimum reference power')
-        # df = dfm.set_pow_ref_by_turbines(df, [])
-        # # df = dfm.set_pow_ref_by_upstream_turbines(
-        # #     df, df_upstream, exclude_turbs=[ti])
-        df = df[df['pow_ref'] > Pmin]
+        df = df[df["pow_ref"] > Pmin]
 
         # Define vane and (normalized) power measurements
-        vane = wrap_180(np.array(df['vane']))
+        vane = wrap_180(np.array(df["vane"]))
 
         # Filter for viable conditions
-        ids_good = ((vane >= vane_bounds[0]) & (vane <= vane_bounds[1]) &
-                    (df['pow'] > Pmin) & (df['pow_ref'] > Pmin))
+        ids_good = (
+            (vane >= vane_bounds[0])
+            & (vane <= vane_bounds[1])
+            & (df["pow"] > Pmin)
+            & (df["pow_ref"] > Pmin)
+        )
         vane = vane[ids_good]
-        Pnorm = df.loc[ids_good, 'pow'] / df.loc[ids_good, 'pow_ref']
-        print('  Number of useful datapoints: %d.' % len(vane))
+        Pnorm = df.loc[ids_good, "pow"] / df.loc[ids_good, "pow_ref"]
+        logger.info("  Number of useful datapoints: %d." % len(vane))
 
         # Bin data
-        print('  Binning data...')
+        logger.info("  Binning data...")
         bins_x = np.arange(vane_bounds[0], vane_bounds[1], dv)
         bins_y = np.zeros_like(bins_x)
         bins_N = np.zeros_like(bins_x)
 
         for ii, edge_x_l in enumerate(bins_x):
             edge_x_r = edge_x_l + dv
             yi = Pnorm[(vane >= edge_x_l) & (vane < edge_x_r)]
             bins_N[ii] = yi.shape[0]
             bins_y[ii] = np.nanmean(yi)
 
         # if np.any(bins_N > 0):
-        #     bins_y = np.array(bins_y) / np.nanmax(bins_y[bins_N/np.max(bins_N) > 0.10])  # Normalize to 1
+        #     bins_y = np.array(bins_y) / np.nanmax(bins_y[bins_N/np.max(bins_N) > 0.10])
 
         self.bins_x = bins_x
         self.bins_y = bins_y
         self.bins_N = bins_N
 
-    def estimate_cos_pp_fit(self,
-                            opt_yshift_range=None,
-                            opt_bias_range=(-15., 15.),
-                            opt_pp_range=(1.0, 10.0), opt_Ns=41):
-
+    def estimate_cos_pp_fit(
+        self,
+        opt_yshift_range=None,
+        opt_bias_range=(-15.0, 15.0),
+        opt_pp_range=(1.0, 10.0),
+        opt_Ns=41,
+    ):
         # for ti in self.turbine_list:
         bins_x = self.bins_x
         bins_y = self.bins_y
         bins_N = self.bins_N
 
         if len(bins_x) <= 0:
-            raise ValueError('Please calculate curves using ' +
-                                '.calculate_curves() before ' +
-                                'estimating a fit.')
+            raise ValueError(
+                "Please calculate curves using "
+                + ".calculate_curves() before "
+                + "estimating a fit."
+            )
 
         # Define an approximating function
         def approx_func(x):
-            y = x[0] * np.cos((bins_x-x[1]) * np.pi / 180.)**x[2]
+            y = x[0] * np.cos((bins_x - x[1]) * np.pi / 180.0) ** x[2]
             return y
 
         # Define a cost function
         def cost(x):
             # x[0] is the x offset, x[1] is the cos coefficient
             y_fit = approx_func(x)
-            J_fit = np.multiply(bins_N, (y_fit - bins_y)**2.)
+            J_fit = np.multiply(bins_N, (y_fit - bins_y) ** 2.0)
             J_sum = np.nanmean(J_fit)
             return J_sum
 
         if opt_yshift_range is None:
             opt_yshift_range = (np.nanmin(bins_y), np.nanmax(bins_y))
 
-        print('Fitting a cos(x-x0)^pp curve to the data...')
+        logger.info("Fitting a cos(x-x0)^pp curve to the data...")
         x_opt, J_opt, x, J = opt.brute(
             func=cost,
-            ranges=(opt_yshift_range,
-                    opt_bias_range, opt_pp_range),
+            ranges=(opt_yshift_range, opt_bias_range, opt_pp_range),
             Ns=opt_Ns,
             finish=opt.fmin,
             full_output=True,
-            disp=True
-            )
-        print('x_opt: ', x_opt)
+            disp=True,
+        )
+        logger.info(f"x_opt: {x_opt}")
         y_opt = approx_func(x_opt)
 
         self.x_opt = x_opt
         self.bins_y_opt = y_opt
 
         return x_opt
 
@@ -183,33 +168,36 @@
         bins_y = self.bins_y
         bins_N = self.bins_N
 
         x_opt = self.x_opt
         y_opt = self.bins_y_opt
 
         if len(bins_x) <= 0:
-            raise ValueError('Please calculate curves using ' +
-                                '.calculate_curves() before ' +
-                                'plotting.')
+            raise ValueError(
+                "Please calculate curves using " + ".calculate_curves() before " + "plotting."
+            )
 
         # Plot bins and averaged curve
         fig, ax = plt.subplots(nrows=2, sharex=True)
-        ax[0].plot(bins_x, bins_y, 'o-', label='Data')
+        ax[0].plot(bins_x, bins_y, "o-", label="Data")
         if len(y_opt) > 0:
-            ax[0].plot(bins_x, y_opt, '--',
-                    label=('Fit (x0=%.3f, x1=%.3f, x2=%.3f)'
-                           % (x_opt[0], x_opt[1], x_opt[2])))
-        ax[0].set_xlabel('Vane measurement (deg)')
-        ax[0].set_ylabel('Relative power production (-)')
-        ax[0].grid('minor')
+            ax[0].plot(
+                bins_x,
+                y_opt,
+                "--",
+                label=("Fit (x0=%.3f, x1=%.3f, x2=%.3f)" % (x_opt[0], x_opt[1], x_opt[2])),
+            )
+        ax[0].set_xlabel("Vane measurement (deg)")
+        ax[0].set_ylabel("Relative power production (-)")
+        ax[0].grid("minor")
         ax[0].legend()
 
         ax[1].bar(bins_x, bins_N)
-        ax[1].set_xlabel('Vane measurement (deg)')
-        ax[1].set_ylabel('Number of data points (-)')
+        ax[1].set_xlabel("Vane measurement (deg)")
+        ax[1].set_ylabel("Number of data points (-)")
 
         fig.tight_layout()
         if save_path is not None:
             os.makedirs(os.path.dirname(save_path), exist_ok=True)
             plt.savefig(save_path, dpi=fig_dpi)
 
         return fig, ax
```

### Comparing `flasc-1.4.2/flasc/utilities.py` & `flasc-2.0/flasc/utilities/utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,16 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-
 import datetime
 
 # import numba
 import numpy as np
-# import scipy.interpolate as interp
 
+# import scipy.interpolate as interp
 from floris.utilities import wrap_360
 
 
-def printnow(text, flush=True):
-    now_time = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-    print('%s: %s' % (now_time, text), flush=flush)
-
-
 def estimate_dt(time_array):
     """Automatically estimate timestep in a time_array
 
     Args:
         time_array ([list]): List or dataframe with time entries
 
     Returns:
@@ -37,37 +19,37 @@
 
     if len(time_array) < 2:
         # Assume arbitrary value
         return datetime.timedelta(seconds=0)
 
     dt = np.median(np.diff(time_array))
     if not isinstance(dt, datetime.timedelta):
-        dt = datetime.timedelta(seconds=dt.astype(float)/1e9)
+        dt = datetime.timedelta(seconds=dt.astype(float) / 1e9)
 
     # Check if data is all ascending
     if dt <= datetime.timedelta(0):
-        raise UserWarning('Please only insert time ascending data.')
+        raise UserWarning("Please only insert time ascending data.")
 
     return dt
 
 
 def get_num_turbines(df):
     nt = 0
-    while ('pow_%03d' % nt) in df.columns:
+    while ("pow_%03d" % nt) in df.columns:
         nt += 1
     return nt
 
 
 def interp_with_max_gap(x, xp, fp, max_gap, kind, wrap_around_360=False):
     if not ((kind == "linear") or (kind == "nearest")):
         raise NotImplementedError("Unknown interpolation method specified.")
 
     # Check format of max_gap: needs to be an integer/float
     if not isinstance(max_gap, (float, int)):
-        max_gap = np.timedelta64(max_gap) / np.timedelta64(1, 's')
+        max_gap = np.timedelta64(max_gap) / np.timedelta64(1, "s")
 
     if wrap_around_360:
         fp_cos = np.cos(fp * np.pi / 180.0)
         fp_sin = np.sin(fp * np.pi / 180.0)
         y_cos = _interpolate_with_max_gap(x, xp, fp_cos, max_gap, False, kind)
         y_sin = _interpolate_with_max_gap(x, xp, fp_sin, max_gap, False, kind)
         y = wrap_360(np.arctan2(y_sin, y_cos) * 180.0 / np.pi)
@@ -77,15 +59,21 @@
     return y
 
 
 # Credits to 'np8', from https://stackoverflow.com/questions/64045034/interpolate-values-and-replace-with-nans-within-a-long-gap
 # Adapted to include nearest-neighbor interpolation
 # @numba.njit()
 def _interpolate_with_max_gap(
-    x, xp, fp, max_gap, assume_sorted=False, kind="linear", extrapolate=True,
+    x,
+    xp,
+    fp,
+    max_gap,
+    assume_sorted=False,
+    kind="linear",
+    extrapolate=True,
 ):
     """
     Interpolate data linearly or using nearest-neighbor with maximum gap.
     If there is larger gap in data than `max_gap`, the gap will be filled
     with np.nan.
 
     The input values should not contain NaNs.
@@ -103,15 +91,15 @@
         The maximum allowable distance between x and `xp` for which
         interpolation is still performed. Gaps larger than
         this will be filled with np.nan in the output `target_y`.
     xp_is_sorted: boolean, default: True
         If True, the input data `xp` is assumed to be monotonically
         increasing. Some performance gain if you supply sorted input data.
     x_is_sorted: boolean, default: True
-        If True, the input data `x` is assumed to be 
+        If True, the input data `x` is assumed to be
         monotonically increasing. Some performance gain if you supply
         sorted input data.
 
     Returns
     ------
     target_y: np.array
         The interpolation results.
@@ -125,28 +113,28 @@
         # Sort x to be monotonous
         sort_array = np.argsort(x)
         inverse_sort_array = np.argsort(sort_array)  # Used to undo sort
         x = x[sort_array]
 
     if extrapolate:
         # Add points on boundaries for xp
-        xp_full = np.empty(len(xp) + 2) 
+        xp_full = np.empty(len(xp) + 2)
         xp_full[1:-1] = xp
         xp_full[0] = xp[0] - max_gap
         xp_full[-1] = xp[-1] + max_gap
 
         # Add points on boundaries for fp
-        fp_full = np.empty(len(fp) + 2) 
+        fp_full = np.empty(len(fp) + 2)
         fp_full[1:-1] = fp
         fp_full[0] = fp[0]
         fp_full[-1] = fp[-1]
     else:
         xp_full = xp
         fp_full = fp
-    
+
     # # Check if we can solve it using numpy's internal interp function
     # if ((kind=='linear') and (np.max(np.diff(xp)) <= max_gap)):
     #     target_y = np.interp(x, xp, fp, left=np.nan, right=np.nan)
     #     return target_y[inverse_sort_array]
 
     # Otherwise, process manually: initialize variables
     target_y = np.ones(x.size) * np.nan  # Fill with NaNs
@@ -159,17 +147,17 @@
 
     # Loop through all cases that fall inside xp
     exit_loop = False
     for ii in range(ij, len(x)):
         # Move left interp point, if necessary
         while x[ii] > xp_full[idx_left_interp_point + 1]:
             idx_left_interp_point += 1
-            if ((idx_left_interp_point + 1) >= len(xp_full)):
+            if (idx_left_interp_point + 1) >= len(xp_full):
                 # Exit, we are now to the right of max. point xp
-                exit_loop=True
+                exit_loop = True
                 break
 
         if exit_loop:
             break
 
         # Calculate coordinates to interpolate
         x1 = xp_full[idx_left_interp_point]
@@ -196,9 +184,9 @@
             if delta_x1 > delta_x2:
                 target_y[ii] = y2
             else:
                 target_y[ii] = y1
 
     if not assume_sorted:
         return target_y[inverse_sort_array]
-    
-    return target_y
+
+    return target_y
```

### Comparing `flasc-1.4.2/flasc/utilities_examples.py` & `flasc-2.0/flasc/utilities/utilities_examples.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,128 +1,130 @@
 import copy
 from pathlib import Path
-import matplotlib.pyplot as plt
-import numpy as np
 from time import perf_counter as timerpc
 
-from floris.tools import FlorisInterface, UncertaintyInterface
-from flasc.visualization import plot_floris_layout
+import floris.layout_visualization as layoutviz
+import matplotlib.pyplot as plt
+import numpy as np
+from floris import FlorisModel, UncertainFlorisModel
 
 
 def load_floris_smarteole(wake_model="gch", wd_std=0.0):
-    """Load a FlorisInterface object for the wind farm at hand.
+    """Load a FlorisModel object for the wind farm at hand.
 
     Args:
         wake_model (str, optional): The wake model that FLORIS should use. Common
           options are 'cc', 'gch', 'jensen', 'turbopark' and 'emgauss'
            . Defaults to "gch".
         operation_modes (array, optional): Array or list of integers denoting each
           turbine's operation mode. When None is specified, will assume each turbine
           is in its first operation mode (0). Defaults to None.
         wd_std (float, optional): Uncertainty; standard deviation in the inflow
           wind direction in degrees. Defaults to 0.0 deg meaning no uncertainty.
 
     Returns:
-        FlorisInterface: Floris object.
+        FlorisModel: Floris object.
     """
 
     # Use the local FLORIS GCH/CC model for the wake model settings
     root_path = (
-        Path(__file__).resolve().parents[1]
-        / "examples_smarteole" / "floris_input_smarteole"
+        Path(__file__).resolve().parents[2] / "examples_smarteole" / "floris_input_smarteole"
     )
     fn = root_path / "{:s}.yaml".format(wake_model)
 
     # Initialize FLORIS model and format appropriately
-    fi = FlorisInterface(fn)
+    fm = FlorisModel(fn)
 
     # Add uncertainty
     if wd_std > 0.01:
         unc_options = {
             "std_wd": wd_std,  # Standard deviation for inflow wind direction (deg)
             "pmf_res": 1.0,  # Resolution over which to calculate angles (deg)
             "pdf_cutoff": 0.995,  # Probability density function cut-off (-)
         }
-        fi = UncertaintyInterface(fi, unc_options=unc_options)
+        fm = UncertainFlorisModel(fm, unc_options=unc_options)
 
     # Add turbine weighing terms. These are typically used to distinguish
     # between turbines of interest and neighboring farms. This is particularly
     # helpful when you have information about surrounding wind farms.
-    turbine_weights = np.ones(len(fi.layout_x), dtype=float)
+    turbine_weights = np.ones(len(fm.layout_x), dtype=float)
 
-    return (fi, turbine_weights)
+    return (fm, turbine_weights)
 
 
-def load_floris_artificial(wake_model="gch", wd_std=0.0, pP=None):
-    """Load a FlorisInterface object for the wind farm at hand.
+def load_floris_artificial(wake_model="gch", wd_std=0.0, cosine_exponent=None):
+    """Load a FlorisModel object for the wind farm at hand.
 
     Args:
         wake_model (str, optional): The wake model that FLORIS should use. Common
           options are 'cc', 'gch', 'jensen',  'turbopark' and 'emgauss'
           . Defaults to "gch".
         operation_modes (array, optional): Array or list of integers denoting each
           turbine's operation mode. When None is specified, will assume each turbine
           is in its first operation mode (0). Defaults to None.
         wd_std (float, optional): Uncertainty; standard deviation in the inflow
           wind direction in degrees. Defaults to 0.0 deg meaning no uncertainty.
 
     Returns:
-        FlorisInterface: Floris object.
+        FlorisModel: Floris object.
     """
 
     # Use the local FLORIS GCH/CC model for the wake model settings
     root_path = (
-        Path(__file__).resolve().parents[1]
-        / "examples_artificial_data" / "floris_input_artificial"
+        Path(__file__).resolve().parents[2] / "examples_artificial_data" / "floris_input_artificial"
     )
     fn = root_path / "{:s}.yaml".format(wake_model)
 
     # Now assign the turbine locations and information
     layout_x = [1630.222, 1176.733, 816.389, 755.938, 0.0, 1142.24, 1553.102]
     layout_y = [0.0, 297.357, 123.431, 575.544, 647.779, 772.262, 504.711]
 
     # Initialize FLORIS model and format appropriately
-    fi = FlorisInterface(fn)
-    fi.reinitialize(
+    fm = FlorisModel(fn)
+    fm.set(
         layout_x=layout_x,
         layout_y=layout_y,
     )
 
     # Update Pp if specified
-    if pP is not None:
-        tdefs = [copy.deepcopy(t) for t in fi.floris.farm.turbine_definitions]
+    if cosine_exponent is not None:
+        tdefs = [copy.deepcopy(t) for t in fm.core.farm.turbine_definitions]
         for ii in range(len(tdefs)):
-            tdefs[ii]["pP"] = pP
+            tdefs[ii]["power_thrust_table"]["cosine_loss_exponent_yaw"] = cosine_exponent
 
-        fi.reinitialize(turbine_type=tdefs)
+        fm.set(turbine_type=tdefs)
 
     # Add uncertainty
     if wd_std > 0.01:
         unc_options = {
             "std_wd": wd_std,  # Standard deviation for inflow wind direction (deg)
             "pmf_res": 1.0,  # Resolution over which to calculate angles (deg)
             "pdf_cutoff": 0.995,  # Probability density function cut-off (-)
         }
-        fi = UncertaintyInterface(fi, unc_options=unc_options)
+        fm = UncertainFlorisModel(fm, unc_options=unc_options)
 
     # Add turbine weighing terms. These are typically used to distinguish
     # between turbines of interest and neighboring farms. This is particularly
     # helpful when you have information about surrounding wind farms.
     turbine_weights = np.ones(len(layout_x), dtype=float)
 
-    return (fi, turbine_weights)
+    return (fm, turbine_weights)
 
 
 if __name__ == "__main__":
     # Load and time the artificial FLORIS model
     t0 = timerpc()
-    fi, turbine_weights = load_floris_artificial()
+    fm, turbine_weights = load_floris_artificial()
     print("Time spent to load the FLORIS model (artificial): {:.2f} s.".format(timerpc() - t0))
-    plot_floris_layout(fi, plot_terrain=False)
+    ax = layoutviz.plot_turbine_points(fm)
+    layoutviz.plot_turbine_labels(fm, ax=ax)
+    ax.grid()
 
     # Load and time the Smarteole FLORIS model
     t0 = timerpc()
-    fi, turbine_weights = load_floris_smarteole()
+    fm, turbine_weights = load_floris_smarteole()
     print("Time spent to load the FLORIS model (smarteole): {:.2f} s.".format(timerpc() - t0))
-    plot_floris_layout(fi, plot_terrain=False)
+    ax = layoutviz.plot_turbine_points(fm)
+    layoutviz.plot_turbine_labels(fm, ax=ax)
+    ax.grid()
 
     plt.show()
```

### Comparing `flasc-1.4.2/flasc/wake_steering/lookup_table_tools.py` & `flasc-2.0/flasc/utilities/lookup_table_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,14 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-
 import numpy as np
 from scipy.interpolate import LinearNDInterpolator
 
 
-def get_yaw_angles_interpolant(df_opt, ramp_up_ws=[4, 5], ramp_down_ws=[10, 12], minimum_yaw_angle=None, maximum_yaw_angle=None):
+def get_yaw_angles_interpolant(
+    df_opt, ramp_up_ws=[4, 5], ramp_down_ws=[10, 12], minimum_yaw_angle=None, maximum_yaw_angle=None
+):
     """Create an interpolant for the optimal yaw angles from a dataframe
     'df_opt', which contains the rows 'wind_direction', 'wind_speed',
     'turbulence_intensity', and 'yaw_angles_opt'. This dataframe is typically
     produced automatically from a FLORIS yaw optimization using Serial Refine
     or SciPy. One can additionally apply a ramp-up and ramp-down region
     to transition between non-wake-steering and wake-steering operation.
 
@@ -76,19 +65,15 @@
         points_copied = np.array(points[ids_to_copy_ub, :], copy=True)
         values_copied = np.array(values[ids_to_copy_ub, :], copy=True)
         points_copied[:, col] = 999.0  # Upper bound
         points = np.vstack([points, points_copied])
         values = np.vstack([values, values_copied])
 
     # Now create a linear interpolant for the yaw angles
-    interpolant = LinearNDInterpolator(
-        points=points,
-        values=values,
-        fill_value=np.nan
-    )
+    interpolant = LinearNDInterpolator(points=points, values=values, fill_value=np.nan)
 
     # Now create a wrapper function with ramp-up and ramp-down
     def interpolant_with_ramps(wd_array, ws_array, ti_array=None):
         # Deal with missing ti_array
         if ti_array is None:
             ti_ref = float(np.median(interpolant.points[:, 2]))
             ti_array = np.ones(np.shape(wd_array), dtype=float) * ti_ref
@@ -100,23 +85,23 @@
         yaw_angles = interpolant(wd_array, ws_array, ti_array)
         yaw_angles = np.array(yaw_angles, dtype=float)
 
         # Define ramp down factor
         rampdown_factor = np.interp(
             x=ws_array,
             xp=[0.0, *ramp_up_ws, *ramp_down_ws, 999.0],
-            fp=[0.0, 0.0, 1.0, 1.0, 0.0, 0.0]
+            fp=[0.0, 0.0, 1.0, 1.0, 0.0, 0.0],
         )
 
         # Saturate yaw offsets to threshold
         axis = len(np.shape(yaw_angles)) - 1
         nturbs = np.shape(yaw_angles)[-1]
-        yaw_lb = np.expand_dims(
-            minimum_yaw_angle * rampdown_factor, axis=axis
-        ).repeat(nturbs, axis=axis)
-        yaw_ub = np.expand_dims(
-            maximum_yaw_angle * rampdown_factor, axis=axis
-        ).repeat(nturbs, axis=axis)
+        yaw_lb = np.expand_dims(minimum_yaw_angle * rampdown_factor, axis=axis).repeat(
+            nturbs, axis=axis
+        )
+        yaw_ub = np.expand_dims(maximum_yaw_angle * rampdown_factor, axis=axis).repeat(
+            nturbs, axis=axis
+        )
 
         return np.clip(yaw_angles, yaw_lb, yaw_ub)
 
     return interpolant_with_ramps
```

### Comparing `flasc-1.4.2/flasc/wake_steering/yaw_optimizer_visualization.py` & `flasc-2.0/flasc/yaw_optimizer_visualization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,99 +1,88 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
+from flasc.logging_manager import LoggingManager
+
+logger_manager = LoggingManager()  # Instantiate LoggingManager
+logger = logger_manager.logger  # Obtain the reusable logger
+
 
 def plot_uplifts_by_atmospheric_conditions(
     df_list,
     labels=None,
     ws_edges=np.arange(3.0, 17.0, 1.0),
     wd_edges=np.arange(0.0, 360.0001, 3.0),
-    ti_edges = np.arange(0.0, 0.30, 0.02),
+    ti_edges=np.arange(0.0, 0.30, 0.02),
 ):
     # Calculate bin means
-    ws_labels = (ws_edges[0:-1] + ws_edges[1::]) / 2.
-    wd_labels = (wd_edges[0:-1] + wd_edges[1::]) / 2.
-    ti_labels = (ti_edges[0:-1] + ti_edges[1::]) / 2.
+    ws_labels = (ws_edges[0:-1] + ws_edges[1::]) / 2.0
+    wd_labels = (wd_edges[0:-1] + wd_edges[1::]) / 2.0
+    ti_labels = (ti_edges[0:-1] + ti_edges[1::]) / 2.0
 
     # Format input
     if isinstance(df_list, pd.DataFrame):
         df_list = [df_list]
 
     # Clean dataframes and calculate AEP gains
     for ii, df in enumerate(df_list):
-         # Only keep cases with Pbl > 0 and non-NaNs
-        df = df.dropna(how='any', subset=['farm_power_baseline', 'farm_power_opt'])
-        df = df[df['farm_power_baseline'] > 0.01].reset_index(drop=True)
+        # Only keep cases with Pbl > 0 and non-NaNs
+        df = df.dropna(how="any", subset=["farm_power_baseline", "farm_power_opt"])
+        df = df[df["farm_power_baseline"] > 0.01].reset_index(drop=True)
 
         # Check if frequency vector exists
-        if not "farm_energy_baseline" in df.columns:
+        if "farm_energy_baseline" not in df.columns:
             if "frequency" in df.columns:
                 df["frequency"] = df["frequency"].astype(float)
             elif "freq" in df.columns:
                 df["frequency"] = df["freq"].astype(float)
             else:
                 df["frequency"] = 1.0
-                print(
-                    "No column 'freq' or 'frequency' found in dataframe." +
-                    "Assuming a uniform distribution."
+                logger.info(
+                    "No column 'freq' or 'frequency' found in dataframe."
+                    + "Assuming a uniform distribution."
                 )
 
             # Calculate wind farm energy, baseline and optimized
             df["farm_energy_baseline"] = df["farm_power_baseline"] * df["frequency"]
             df["farm_energy_opt"] = df["farm_power_opt"] * df["frequency"]
 
         # Calculate relative and absolute uplift in energy for every condition
         df["Prel"] = np.where(
-            df["farm_power_baseline"] > 0.0,
-            df["farm_power_opt"] / df["farm_power_baseline"],
-            0.0
+            df["farm_power_baseline"] > 0.0, df["farm_power_opt"] / df["farm_power_baseline"], 0.0
         )
 
-        df["Pabs"] = (
-            (df["farm_energy_opt"] - df["farm_energy_baseline"]) /
-            np.nansum(df["farm_energy_opt"] - df["farm_energy_baseline"])
+        df["Pabs"] = (df["farm_energy_opt"] - df["farm_energy_baseline"]) / np.nansum(
+            df["farm_energy_opt"] - df["farm_energy_baseline"]
         )
 
         # Bin data by wind speed, wind direction and turbulence intensity
         df["ws_bin"] = pd.cut(df["wind_speed"], ws_edges, right=False, labels=ws_labels)
         df["wd_bin"] = pd.cut(df["wind_direction"], wd_edges, right=False, labels=wd_labels)
         df["ti_bin"] = pd.cut(df["turbulence_intensity"], ti_edges, right=False, labels=ti_labels)
 
         df_list[ii] = df.copy()  # Save updated dataframe to self
 
     for yii, yq_col in enumerate(["Prel", "Pabs"]):
         if yii == 0:
             ylabel = "Relative power gain (%)"
         else:
             ylabel = "Contribution to AEP uplift (%)"
-    
+
         for xii, xq_col in enumerate(["ws_bin", "wd_bin", "ti_bin"]):
             if xii == 0:
                 xlabel = "Wind speed (m/s)"
             elif xii == 1:
                 xlabel = "Wind direction (deg)"
             elif xii == 2:
                 xlabel = "Turbulence intensity (%)"
                 if np.all([df["turbulence_intensity"].unique() <= 1 for df in df_list]):
                     # Skip TI, if only optimized and evaluated for single TI
-                    break 
+                    break
 
             # Now produce plots with dataframes: wind speed vs. relative power gain
             x = [None for _ in range(len(df_list))]
             y = [None for _ in range(len(df_list))]
             f = [None for _ in range(len(df_list))]
             for dii, df in enumerate(df_list):
                 df_group = df.groupby(xq_col)
@@ -115,159 +104,150 @@
         yn = [yn]
 
     # Get number of dataframes to plot
     nd = len(x)
 
     if labels is None:
         labels = [None for _ in range(nd)]
-    
+
     # Produce plots
     fig, ax = plt.subplots(nrows=2, sharex=True, figsize=(10, 4))
     if np.all([len(xi) <= 1 for xi in x]):
         dx = 1.0  # Default to 1.0 bin width, if only one value
     else:
         dx = np.min(np.hstack([np.diff(xi) for xi in x])) * 0.8 / nd  # Bin width
 
     for dii in range(nd):
         # Produce top subplot
         ax[0].bar(x=x[dii] + (dii - 0.5) * dx, height=y[dii], width=dx, label=labels[dii])
         ax[0].set_ylabel(ylabel)
         ax[0].grid(True)
 
         ax[1].bar(x=x[dii] + (dii - 0.5) * dx, height=yn[dii], width=dx, label=labels[dii])
-        ax[1].set_ylabel('Frequency (-)')
+        ax[1].set_ylabel("Frequency (-)")
         ax[1].set_xlabel(xlabel)
         ax[1].grid(True)
         ax[1].set_xticks(x[dii])
         if len(x[dii]) > 50:  # Too many ticks: reduce
-            xtlabels = ['' for _ in range(len(x[dii]))]
-            xtlabels[0::5] = ['%.1f' % i for i in x[dii][0::5]]
+            xtlabels = ["" for _ in range(len(x[dii]))]
+            xtlabels[0::5] = ["%.1f" % i for i in x[dii][0::5]]
         else:
-            xtlabels = ['%.1f' % i for i in x[dii]]
+            xtlabels = ["%.1f" % i for i in x[dii]]
         ax[1].set_xticklabels(xtlabels)
 
     if not np.all([a is None for a in labels]):
         ax[0].legend()
         ax[1].legend()
 
     return fig, ax
 
+
 def plot_offsets_wswd_heatmap(df_offsets, turb_id, ax=None):
     """
-    df_offsets should be a dataframe with columns: 
-       - wind_direction, 
+    df_offsets should be a dataframe with columns:
+       - wind_direction,
        - wind_speed,
        - turbine identifiers (possibly multiple)
-    
-    Produces a heat map of the offsets for all wind directions and 
-    wind speeds for turbine specified by turb_id. Dataframe is assumed 
-    to contain individual turbine offsets in distinct columns (unlike 
+
+    Produces a heat map of the offsets for all wind directions and
+    wind speeds for turbine specified by turb_id. Dataframe is assumed
+    to contain individual turbine offsets in distinct columns (unlike
     the yaw_angles_opt column from FLORIS.
 
     """
 
-    if type(turb_id) is int:
+    if isinstance(turb_id, int):
         if "yaw_angles_opt" in df_offsets.columns:
-            offsets = np.vstack(
-                df_offsets.yaw_angles_opt.to_numpy()
-            )[:,turb_id]
-            df_offsets = pd.DataFrame({
-                "wind_direction":df_offsets.wind_direction,
-                "wind_speed":df_offsets.wind_speed,
-                "yaw_offset":offsets
-            })
+            offsets = np.vstack(df_offsets.yaw_angles_opt.to_numpy())[:, turb_id]
+            df_offsets = pd.DataFrame(
+                {
+                    "wind_direction": df_offsets.wind_direction,
+                    "wind_speed": df_offsets.wind_speed,
+                    "yaw_offset": offsets,
+                }
+            )
             turb_id = "yaw_offset"
         else:
-            raise TypeError("Specify turb_id as a full string for the "+\
-                "correct dataframe column.")
+            raise TypeError(
+                "Specify turb_id as a full string for the " + "correct dataframe column."
+            )
 
     ws_array = np.unique(df_offsets.wind_speed)
     wd_array = np.unique(df_offsets.wind_direction)
 
     # Construct array of offets
     offsets_array = np.zeros((len(ws_array), len(wd_array)))
     for i, ws in enumerate(ws_array):
-        offsets_array[-i,:] = (df_offsets
-                [df_offsets.wind_speed == ws]
-                [turb_id]
-                .values
-        )
+        offsets_array[-i, :] = df_offsets[df_offsets.wind_speed == ws][turb_id].values
 
-    if ax == None:
-        fig, ax = plt.subplots(1,1)
-    d_wd = (wd_array[1]-wd_array[0])/2
-    d_ws = (ws_array[1]-ws_array[0])/2
+    if ax is None:
+        fig, ax = plt.subplots(1, 1)
+    d_wd = (wd_array[1] - wd_array[0]) / 2
+    d_ws = (ws_array[1] - ws_array[0]) / 2
     im = ax.imshow(
-        offsets_array, interpolation=None, 
-        extent=[wd_array[0]-d_wd, wd_array[-1]+d_wd, 
-                ws_array[0]-d_ws, ws_array[-1]+d_ws], 
-        aspect='auto'
+        offsets_array,
+        interpolation=None,
+        extent=[wd_array[0] - d_wd, wd_array[-1] + d_wd, ws_array[0] - d_ws, ws_array[-1] + d_ws],
+        aspect="auto",
     )
-    ax.set_xlabel('Wind direction')
-    ax.set_ylabel('Wind speed')
-    cbar = plt.colorbar(im, ax=ax, orientation='vertical')
-    cbar.set_label('Yaw offset')
+    ax.set_xlabel("Wind direction")
+    ax.set_ylabel("Wind speed")
+    cbar = plt.colorbar(im, ax=ax, orientation="vertical")
+    cbar.set_label("Yaw offset")
 
     return ax, cbar
 
 
-def plot_offsets_wd(df_offsets, turb_id, ws_plot, color="black", alpha=1.0,
-    label=None, ax=None):
+def plot_offsets_wd(df_offsets, turb_id, ws_plot, color="black", alpha=1.0, label=None, ax=None):
     """
-    df_offsets should be a dataframe with columns: 
-       - wind_direction, 
+    df_offsets should be a dataframe with columns:
+       - wind_direction,
        - wind_speed,
        - turbine identifiers (possibly multiple)
 
-    if ws_plot is scalar, only that wind speed is plotted. If ws_plot is 
+    if ws_plot is scalar, only that wind speed is plotted. If ws_plot is
     a two-element tuple or list, that range of wind speeds is plotted.
 
     label only allowed is single wind speed is given.
     """
 
-    if type(turb_id) is int:
+    if isinstance(turb_id, int):
         if "yaw_angles_opt" in df_offsets.columns:
-            offsets = np.vstack(
-                df_offsets.yaw_angles_opt.to_numpy()
-            )[:,turb_id]
-            df_offsets = pd.DataFrame({
-                "wind_direction":df_offsets.wind_direction,
-                "wind_speed":df_offsets.wind_speed,
-                "yaw_offset":offsets
-            })
+            offsets = np.vstack(df_offsets.yaw_angles_opt.to_numpy())[:, turb_id]
+            df_offsets = pd.DataFrame(
+                {
+                    "wind_direction": df_offsets.wind_direction,
+                    "wind_speed": df_offsets.wind_speed,
+                    "yaw_offset": offsets,
+                }
+            )
             turb_id = "yaw_offset"
         else:
-            raise TypeError("Specify turb_id as a full string for the "+\
-                "correct dataframe column.")
+            raise TypeError(
+                "Specify turb_id as a full string for the " + "correct dataframe column."
+            )
 
-    if hasattr(ws_plot, '__len__') and label is not None:
+    if hasattr(ws_plot, "__len__") and label is not None:
         label = None
-        print("label option can only be used for signle wind speed plot.")
-    
+        logger.warn("label option can only be used for single wind speed plot.")
+
     ws_array = np.unique(df_offsets.wind_speed)
     wd_array = np.unique(df_offsets.wind_direction)
-    
-    if hasattr(ws_plot, '__len__'):
+
+    if hasattr(ws_plot, "__len__"):
         offsets_list = []
         for ws in ws_array:
             if ws >= ws_plot[0] and ws <= ws_plot[-1]:
-                offsets_list.append(df_offsets
-                    [df_offsets.wind_speed == ws]
-                    [turb_id]
-                    .values
-                )
+                offsets_list.append(df_offsets[df_offsets.wind_speed == ws][turb_id].values)
     else:
-        offsets_list = [df_offsets
-                    [df_offsets.wind_speed == ws_plot]
-                    [turb_id]
-                    .values]
+        offsets_list = [df_offsets[df_offsets.wind_speed == ws_plot][turb_id].values]
 
-    if ax == None:
-        fig, ax = plt.subplots(1,1)
+    if ax is None:
+        fig, ax = plt.subplots(1, 1)
 
     for offsets in offsets_list:
         ax.plot(wd_array, offsets, color=color, alpha=alpha, label=label)
 
-    ax.set_xlabel('Wind direction')
-    ax.set_ylabel('Yaw offset')
-    
-    return ax               
+    ax.set_xlabel("Wind direction")
+    ax.set_ylabel("Yaw offset")
+
+    return ax
```

### Comparing `flasc-1.4.2/flasc.egg-info/SOURCES.txt` & `flasc-2.0/flasc.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,45 @@
-AUTHORS.rst
 LICENSE.txt
-NOTICE.txt
-README.rst
+README.md
 pyproject.toml
 setup.py
 flasc/__init__.py
-flasc/circular_statistics.py
-flasc/floris_tools.py
-flasc/optimization.py
-flasc/time_operations.py
-flasc/utilities.py
-flasc/utilities_examples.py
+flasc/logging_manager.py
 flasc/version.py
 flasc/visualization.py
+flasc/yaw_optimizer_visualization.py
 flasc.egg-info/PKG-INFO
 flasc.egg-info/SOURCES.txt
 flasc.egg-info/dependency_links.txt
 flasc.egg-info/entry_points.txt
 flasc.egg-info/not-zip-safe
 flasc.egg-info/requires.txt
 flasc.egg-info/top_level.txt
-flasc/dataframe_operations/__init__.py
-flasc/dataframe_operations/dataframe_filtering.py
-flasc/dataframe_operations/dataframe_manipulations.py
-flasc/dataframe_operations/df_reader_writer.py
-flasc/energy_ratio/__init__.py
-flasc/energy_ratio/energy_ratio.py
-flasc/energy_ratio/energy_ratio_input.py
-flasc/energy_ratio/energy_ratio_output.py
-flasc/energy_ratio/energy_ratio_utilities.py
-flasc/energy_ratio/energy_ratio_wd_bias_estimation.py
-flasc/energy_ratio/total_uplift.py
-flasc/model_estimation/__init__.py
-flasc/model_estimation/floris_sensitivity_analysis.py
-flasc/model_estimation/turbulence_estimator.py
-flasc/raw_data_handling/__init__.py
-flasc/raw_data_handling/raw_data_importing.py
-flasc/raw_data_handling/sqldatabase_management.py
+flasc/analysis/__init__.py
+flasc/analysis/energy_ratio.py
+flasc/analysis/energy_ratio_heterogeneity_mapper.py
+flasc/analysis/energy_ratio_input.py
+flasc/analysis/energy_ratio_output.py
+flasc/analysis/total_uplift.py
+flasc/data_processing/__init__.py
+flasc/data_processing/dataframe_manipulations.py
+flasc/data_processing/energy_ratio_wd_bias_estimation.py
+flasc/data_processing/filtering.py
+flasc/data_processing/find_sensor_faults.py
+flasc/data_processing/northing_offset.py
+flasc/data_processing/time_operations.py
+flasc/model_fitting/__init__.py
+flasc/model_fitting/floris_sensitivity_analysis.py
+flasc/model_fitting/floris_tuning.py
+flasc/model_fitting/turbulence_estimator.py
+flasc/model_fitting/yaw_pow_fitting.py
 flasc/timing_tests/__init__.py
 flasc/timing_tests/energy_ratio_timing.py
-flasc/turbine_analysis/__init__.py
-flasc/turbine_analysis/find_sensor_faults.py
-flasc/turbine_analysis/northing_offset.py
-flasc/turbine_analysis/ws_pow_filtering.py
-flasc/turbine_analysis/yaw_pow_fitting.py
-flasc/wake_steering/__init__.py
-flasc/wake_steering/lookup_table_tools.py
-flasc/wake_steering/yaw_optimizer_visualization.py
+flasc/utilities/__init__.py
+flasc/utilities/circular_statistics.py
+flasc/utilities/energy_ratio_utilities.py
+flasc/utilities/floris_tools.py
+flasc/utilities/lookup_table_tools.py
+flasc/utilities/optimization.py
+flasc/utilities/tuner_utilities.py
+flasc/utilities/utilities.py
+flasc/utilities/utilities_examples.py
```

### Comparing `flasc-1.4.2/setup.py` & `flasc-2.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,95 @@
 """The setup script."""
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
-
 # Package meta-data.
 NAME = "flasc"
-DESCRIPTION = "FLASC provides a rich suite of analysis tools for SCADA data filtering & analysis, wind farm model validation, field experiment design, and field experiment monitoring."
+DESCRIPTION = (
+    "FLASC provides a rich suite of analysis tools for SCADA data filtering & analysis, "
+    " wind farm model validation, field experiment design, and field experiment monitoring."
+)
 URL = "https://github.com/NREL/flasc"
 EMAIL = "paul.fleming@nrel.gov"
 AUTHOR = "NREL National Wind Technology Center"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    "bokeh>=3.1.1",
-    "floris>=3.4",
-    "feather-format",
-    "ipympl>=0.9.3",
-    "matplotlib>=3.6.3",
-    "numpy",
-    "pandas>=1.5",
-    "pyproj",
-    "pytest",
-    "SALib",
-    "scipy",
-    "sqlalchemy",
-    "streamlit",
-    "tkcalendar",
-    "seaborn",
-    "polars>=0.19.0",
+    "bokeh>=2, <4",
+    "floris~=4.0",
+    "feather-format~=0.0",
+    "ipympl~=0.9",
+    "matplotlib~=3.8",
+    "numpy~=1.20",
+    "pandas~=2.0",
+    "pyproj~=3.0",
+    "SALib~=1.0",
+    "scipy~=1.1",
+    "streamlit~=1.0",
+    "tkcalendar~=1.0",
+    "seaborn~=0.0",
+    "polars==0.19.5",
+    "ephem",
+    "coloredlogs~=10.0",
 ]
 
+EXTRAS = {
+    "docs": {
+        "jupyter-book",
+        "sphinx-book-theme",
+        "sphinx-autodoc-typehints",
+        "sphinxcontrib-autoyaml",
+        "sphinxcontrib.mermaid",
+    },
+    "develop": {
+        "pytest",
+        "pre-commit",
+        "ruff",
+        "isort",
+    },
+}
+
 ROOT = Path(__file__).parent
 with open(ROOT / "flasc" / "version.py") as version_file:
     VERSION = version_file.read().strip()
 
-
-with open("README.rst") as readme_file:
+with open("README.md") as readme_file:
     README = readme_file.read()
 
-with open("READMELONG.rst") as readme_file:
-    READMELONG = readme_file.read()
-
 setup_requirements = [
     # Placeholder
 ]
 
 test_requirements = [
     # Placeholder
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
-    long_description=READMELONG,
+    long_description=README,
+    long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     packages=find_packages(include=["flasc*"]),
     entry_points={"console_scripts": ["flasc=flasc.cli:main"]},
     include_package_data=True,
     install_requires=REQUIRED,
-    license="Apache Software License 2.0",
+    extras_require=EXTRAS,
+    license_files=("LICENSE.txt",),
     zip_safe=False,
     keywords="flasc",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: Apache Software License",
+        "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
     test_suite="tests",
     tests_require=test_requirements,
     setup_requires=setup_requirements,
 )
```

