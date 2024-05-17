# Comparing `tmp/TPOT2-0.1.6a0.tar.gz` & `tmp/TPOT2-0.1.6a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TPOT2-0.1.6a0.tar", last modified: Mon Apr 22 18:24:48 2024, max compression
+gzip compressed data, was "TPOT2-0.1.6a1.tar", last modified: Fri May 17 17:25:18 2024, max compression
```

## Comparing `TPOT2-0.1.6a0.tar` & `TPOT2-0.1.6a1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.194543 TPOT2-0.1.6a0/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-22 18:24:48.194543 TPOT2-0.1.6a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.182543 TPOT2-0.1.6a0/TPOT2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-22 18:24:48.000000 TPOT2-0.1.6a0/TPOT2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-22 18:24:48.000000 TPOT2-0.1.6a0/TPOT2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 18:24:48.000000 TPOT2-0.1.6a0/TPOT2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 18:24:48.000000 TPOT2-0.1.6a0/TPOT2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-22 18:24:48.000000 TPOT2-0.1.6a0/TPOT2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 18:24:48.000000 TPOT2-0.1.6a0/TPOT2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 18:24:48.000000 TPOT2-0.1.6a0/TPOT2.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-22 18:24:48.194543 TPOT2-0.1.6a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.182543 TPOT2-0.1.6a0/tpot2/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.186543 TPOT2-0.1.6a0/tpot2/builtin_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/builtin_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/builtin_modules/arithmetictransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/builtin_modules/column_one_hot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/builtin_modules/feature_encoding_frequency_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/builtin_modules/feature_set_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/builtin_modules/feature_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/builtin_modules/genetic_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/builtin_modules/imputer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18836 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/builtin_modules/one_hot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/builtin_modules/passthrough.py
--rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/builtin_modules/selector_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/builtin_modules/zero_count.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.186543 TPOT2-0.1.6a0/tpot2/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/config/all_single_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/config/autoqtl_builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/config/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/config/classifiers_sklearnex.py
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/config/hyperparametersuggestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/config/mdr_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17690 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/config/regressors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/config/regressors_sklearnex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/config/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/config/special_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/config/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.186543 TPOT2-0.1.6a0/tpot2/evolvers/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/evolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42407 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/evolvers/base_evolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    31097 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/evolvers/steady_state_evolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    16828 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/graphsklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.186543 TPOT2-0.1.6a0/tpot2/individual_representations/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/individual_representations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.190543 TPOT2-0.1.6a0/tpot2/individual_representations/graph_pipeline_individual/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/individual_representations/graph_pipeline_individual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.190543 TPOT2-0.1.6a0/tpot2/individual_representations/graph_pipeline_individual/graph_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/individual_representations/graph_pipeline_individual/graph_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/individual_representations/graph_pipeline_individual/graph_utils/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    49739 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/individual_representations/graph_pipeline_individual/individual.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/individual_representations/graph_pipeline_individual/optuna_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/individual_representations/graph_pipeline_individual/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.190543 TPOT2-0.1.6a0/tpot2/individual_representations/graph_pipeline_individual/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/individual_representations/graph_pipeline_individual/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/individual_representations/individual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.190543 TPOT2-0.1.6a0/tpot2/individual_representations/subset_selector/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/individual_representations/subset_selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/individual_representations/subset_selector/subsetselector.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/logbook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.190543 TPOT2-0.1.6a0/tpot2/objectives/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/objectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/objectives/average_path_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/objectives/complexity.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/objectives/number_of_leaves.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/objectives/number_of_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    20866 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/population.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.190543 TPOT2-0.1.6a0/tpot2/selectors/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/selectors/lexicase_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/selectors/max_weighted_average_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/selectors/nsgaii.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/selectors/random_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/selectors/tournament_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/selectors/tournament_selection_dominated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.194543 TPOT2-0.1.6a0/tpot2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/tests/test_built_in_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/tests/test_ea.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/tests/test_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/tests/test_full_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/tests/test_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/tests/test_population.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.194543 TPOT2-0.1.6a0/tpot2/tpot_estimator/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/tpot_estimator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/tpot_estimator/cross_val_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    59335 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/tpot_estimator/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/tpot_estimator/estimator_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    55782 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/tpot_estimator/steady_state_estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.194543 TPOT2-0.1.6a0/tpot2/tpot_estimator/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/tpot_estimator/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/tpot_estimator/templates/tpottemplates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:24:48.194543 TPOT2-0.1.6a0/tpot2/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/utils/eval_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-22 18:24:39.000000 TPOT2-0.1.6a0/tpot2/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.650774 TPOT2-0.1.6a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-17 17:25:18.650774 TPOT2-0.1.6a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.642773 TPOT2-0.1.6a1/TPOT2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-17 17:25:18.000000 TPOT2-0.1.6a1/TPOT2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-17 17:25:18.000000 TPOT2-0.1.6a1/TPOT2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 17:25:18.000000 TPOT2-0.1.6a1/TPOT2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-17 17:25:18.000000 TPOT2-0.1.6a1/TPOT2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-17 17:25:18.000000 TPOT2-0.1.6a1/TPOT2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 17:25:18.000000 TPOT2-0.1.6a1/TPOT2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 17:25:18.000000 TPOT2-0.1.6a1/TPOT2.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-17 17:25:18.650774 TPOT2-0.1.6a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.642773 TPOT2-0.1.6a1/tpot2/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.642773 TPOT2-0.1.6a1/tpot2/builtin_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/builtin_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/builtin_modules/arithmetictransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/builtin_modules/column_one_hot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/builtin_modules/feature_encoding_frequency_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/builtin_modules/feature_set_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/builtin_modules/feature_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/builtin_modules/genetic_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/builtin_modules/imputer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18836 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/builtin_modules/one_hot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/builtin_modules/passthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/builtin_modules/selector_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/builtin_modules/zero_count.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.646773 TPOT2-0.1.6a1/tpot2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/config/all_single_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/config/autoqtl_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/config/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/config/classifiers_sklearnex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/config/hyperparametersuggestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/config/mdr_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17690 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/config/regressors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/config/regressors_sklearnex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/config/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/config/special_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/config/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.646773 TPOT2-0.1.6a1/tpot2/evolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/evolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42407 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/evolvers/base_evolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31097 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/evolvers/steady_state_evolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16828 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/graphsklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.646773 TPOT2-0.1.6a1/tpot2/individual_representations/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/individual_representations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.646773 TPOT2-0.1.6a1/tpot2/individual_representations/graph_pipeline_individual/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/individual_representations/graph_pipeline_individual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.646773 TPOT2-0.1.6a1/tpot2/individual_representations/graph_pipeline_individual/graph_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/individual_representations/graph_pipeline_individual/graph_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/individual_representations/graph_pipeline_individual/graph_utils/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49739 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/individual_representations/graph_pipeline_individual/individual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/individual_representations/graph_pipeline_individual/optuna_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/individual_representations/graph_pipeline_individual/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.646773 TPOT2-0.1.6a1/tpot2/individual_representations/graph_pipeline_individual/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/individual_representations/graph_pipeline_individual/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/individual_representations/individual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.646773 TPOT2-0.1.6a1/tpot2/individual_representations/subset_selector/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/individual_representations/subset_selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/individual_representations/subset_selector/subsetselector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/logbook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.646773 TPOT2-0.1.6a1/tpot2/objectives/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/objectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/objectives/average_path_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/objectives/complexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/objectives/number_of_leaves.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/objectives/number_of_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20866 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/population.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.650774 TPOT2-0.1.6a1/tpot2/selectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/selectors/lexicase_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/selectors/max_weighted_average_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/selectors/nsgaii.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/selectors/random_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/selectors/tournament_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/selectors/tournament_selection_dominated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.650774 TPOT2-0.1.6a1/tpot2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/tests/test_built_in_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/tests/test_ea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/tests/test_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/tests/test_full_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/tests/test_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/tests/test_population.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.650774 TPOT2-0.1.6a1/tpot2/tpot_estimator/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/tpot_estimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/tpot_estimator/cross_val_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59335 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/tpot_estimator/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/tpot_estimator/estimator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55782 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/tpot_estimator/steady_state_estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.650774 TPOT2-0.1.6a1/tpot2/tpot_estimator/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/tpot_estimator/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/tpot_estimator/templates/tpottemplates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:25:18.650774 TPOT2-0.1.6a1/tpot2/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/utils/eval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-17 17:25:11.000000 TPOT2-0.1.6a1/tpot2/utils/utils.py
```

### Comparing `TPOT2-0.1.6a0/LICENSE` & `TPOT2-0.1.6a1/LICENSE`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/PKG-INFO` & `TPOT2-0.1.6a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: TPOT2
-Version: 0.1.6a0
+Version: 0.1.6a1
 Summary: Tree-based Pipeline Optimization Tool
 Home-page: https://github.com/EpistasisLab/tpot2
 Author: Pedro Ribeiro
 License: GNU/LGPLv3
 Keywords: pipeline optimization,hyperparameter optimization,data science,machine learning,genetic programming,evolutionary computation
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: <3.12
 Provides-Extra: skrebate
 Provides-Extra: mdr
 Provides-Extra: sklearnex
 License-File: LICENSE
 
 
 A Python tool that automatically creates and optimizes machine learning pipelines using genetic programming.
```

### Comparing `TPOT2-0.1.6a0/README.md` & `TPOT2-0.1.6a1/README.md`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/TPOT2.egg-info/PKG-INFO` & `TPOT2-0.1.6a1/TPOT2.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: TPOT2
-Version: 0.1.6a0
+Version: 0.1.6a1
 Summary: Tree-based Pipeline Optimization Tool
 Home-page: https://github.com/EpistasisLab/tpot2
 Author: Pedro Ribeiro
 License: GNU/LGPLv3
 Keywords: pipeline optimization,hyperparameter optimization,data science,machine learning,genetic programming,evolutionary computation
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: <3.12
 Provides-Extra: skrebate
 Provides-Extra: mdr
 Provides-Extra: sklearnex
 License-File: LICENSE
 
 
 A Python tool that automatically creates and optimizes machine learning pipelines using genetic programming.
```

### Comparing `TPOT2-0.1.6a0/TPOT2.egg-info/SOURCES.txt` & `TPOT2-0.1.6a1/TPOT2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/setup.py` & `TPOT2-0.1.6a1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,48 +10,49 @@
     return version
 
 
 package_version = calculate_version()
 
 setup(
     name='TPOT2',
+    python_requires='<3.12', #for configspace compatibility
     version=package_version,
     author='Pedro Ribeiro',
     packages=find_packages(),
     url='https://github.com/EpistasisLab/tpot2',
     license='GNU/LGPLv3', #TODO
     entry_points={'console_scripts': ['tpot2=tpot2:main', ]},
     description=('Tree-based Pipeline Optimization Tool'),
     long_description='''
 A Python tool that automatically creates and optimizes machine learning pipelines using genetic programming.
 
 
 ''',
     zip_safe=True,
-    install_requires=['numpy>=1.16.3',
+    install_requires=['numpy>=1.26.4',
                       'scipy>=1.3.1',
                       'scikit-learn>=1.3.0',
                       'update_checker>=0.16',
                       'tqdm>=4.36.1',
                       'stopit>=1.1.1',
                       'pandas>=2.2.0',
                       'joblib>=1.1.1',
                       'xgboost>=1.7.0',
                       'matplotlib>=3.6.2',
                       'traitlets>=5.8.0',
                       'lightgbm>=3.3.3',
                       'optuna>=3.0.5',
                       'baikal>=0.4.2',
-                      'jupyter>=1.0.0',
                       'networkx>=3.0',
-                      'dask>=2023.3.1',
-                      'distributed>=2023.7.0',
-                      'dask-ml>=2022.5.27',
-                      'dask-jobqueue>=0.8.1',
+                      'dask>=2024.4.2',
+                      'distributed>=2024.4.2',
+                      'dask-expr>=1.0.12',
+                      'dask-jobqueue>=0.8.5',
                       'func_timeout>=4.3.5',
+                      'configspace>=0.7.1',
                      ],
     extras_require={
         'skrebate': ['skrebate>=0.3.4'],
         'mdr': ['scikit-mdr>=0.4.4'],
         'sklearnex' : ['scikit-learn-intelex>=2023.2.1']
     },
     classifiers=[
```

### Comparing `TPOT2-0.1.6a0/tpot2/builtin_modules/__init__.py` & `TPOT2-0.1.6a1/tpot2/builtin_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/builtin_modules/arithmetictransformer.py` & `TPOT2-0.1.6a1/tpot2/builtin_modules/arithmetictransformer.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/builtin_modules/column_one_hot_encoder.py` & `TPOT2-0.1.6a1/tpot2/builtin_modules/column_one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/builtin_modules/feature_encoding_frequency_selector.py` & `TPOT2-0.1.6a1/tpot2/builtin_modules/feature_encoding_frequency_selector.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/builtin_modules/feature_set_selector.py` & `TPOT2-0.1.6a1/tpot2/builtin_modules/feature_set_selector.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/builtin_modules/feature_transformers.py` & `TPOT2-0.1.6a1/tpot2/builtin_modules/feature_transformers.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/builtin_modules/genetic_encoders.py` & `TPOT2-0.1.6a1/tpot2/builtin_modules/genetic_encoders.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/builtin_modules/imputer.py` & `TPOT2-0.1.6a1/tpot2/builtin_modules/imputer.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/builtin_modules/one_hot_encoder.py` & `TPOT2-0.1.6a1/tpot2/builtin_modules/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/builtin_modules/selector_wrappers.py` & `TPOT2-0.1.6a1/tpot2/builtin_modules/selector_wrappers.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/builtin_modules/zero_count.py` & `TPOT2-0.1.6a1/tpot2/builtin_modules/zero_count.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/config/__init__.py` & `TPOT2-0.1.6a1/tpot2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/config/autoqtl_builtins.py` & `TPOT2-0.1.6a1/tpot2/config/autoqtl_builtins.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/config/classifiers.py` & `TPOT2-0.1.6a1/tpot2/config/classifiers.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/config/classifiers_sklearnex.py` & `TPOT2-0.1.6a1/tpot2/config/classifiers_sklearnex.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/config/hyperparametersuggestor.py` & `TPOT2-0.1.6a1/tpot2/config/hyperparametersuggestor.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/config/mdr_configs.py` & `TPOT2-0.1.6a1/tpot2/config/mdr_configs.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/config/regressors.py` & `TPOT2-0.1.6a1/tpot2/config/regressors.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/config/regressors_sklearnex.py` & `TPOT2-0.1.6a1/tpot2/config/regressors_sklearnex.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/config/selectors.py` & `TPOT2-0.1.6a1/tpot2/config/selectors.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/config/special_configs.py` & `TPOT2-0.1.6a1/tpot2/config/special_configs.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/config/transformers.py` & `TPOT2-0.1.6a1/tpot2/config/transformers.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/evolvers/base_evolver.py` & `TPOT2-0.1.6a1/tpot2/evolvers/base_evolver.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/evolvers/steady_state_evolver.py` & `TPOT2-0.1.6a1/tpot2/evolvers/steady_state_evolver.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/graphsklearn.py` & `TPOT2-0.1.6a1/tpot2/graphsklearn.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/individual_representations/graph_pipeline_individual/graph_utils/graph_utils.py` & `TPOT2-0.1.6a1/tpot2/individual_representations/graph_pipeline_individual/graph_utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/individual_representations/graph_pipeline_individual/individual.py` & `TPOT2-0.1.6a1/tpot2/individual_representations/graph_pipeline_individual/individual.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/individual_representations/graph_pipeline_individual/optuna_optimize.py` & `TPOT2-0.1.6a1/tpot2/individual_representations/graph_pipeline_individual/optuna_optimize.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/individual_representations/graph_pipeline_individual/templates.py` & `TPOT2-0.1.6a1/tpot2/individual_representations/graph_pipeline_individual/templates.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/individual_representations/individual.py` & `TPOT2-0.1.6a1/tpot2/individual_representations/individual.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/individual_representations/subset_selector/subsetselector.py` & `TPOT2-0.1.6a1/tpot2/individual_representations/subset_selector/subsetselector.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/objectives/__init__.py` & `TPOT2-0.1.6a1/tpot2/objectives/__init__.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/objectives/complexity.py` & `TPOT2-0.1.6a1/tpot2/objectives/complexity.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/population.py` & `TPOT2-0.1.6a1/tpot2/population.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/selectors/__init__.py` & `TPOT2-0.1.6a1/tpot2/selectors/__init__.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/selectors/lexicase_selection.py` & `TPOT2-0.1.6a1/tpot2/selectors/lexicase_selection.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/selectors/nsgaii.py` & `TPOT2-0.1.6a1/tpot2/selectors/nsgaii.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/selectors/tournament_selection.py` & `TPOT2-0.1.6a1/tpot2/selectors/tournament_selection.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/selectors/tournament_selection_dominated.py` & `TPOT2-0.1.6a1/tpot2/selectors/tournament_selection_dominated.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/tests/test_estimators.py` & `TPOT2-0.1.6a1/tpot2/tests/test_estimators.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/tests/test_hello_world.py` & `TPOT2-0.1.6a1/tpot2/tests/test_hello_world.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/tests/test_nodes.py` & `TPOT2-0.1.6a1/tpot2/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/tpot_estimator/cross_val_utils.py` & `TPOT2-0.1.6a1/tpot2/tpot_estimator/cross_val_utils.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/tpot_estimator/estimator.py` & `TPOT2-0.1.6a1/tpot2/tpot_estimator/estimator.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/tpot_estimator/estimator_utils.py` & `TPOT2-0.1.6a1/tpot2/tpot_estimator/estimator_utils.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/tpot_estimator/steady_state_estimator.py` & `TPOT2-0.1.6a1/tpot2/tpot_estimator/steady_state_estimator.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/tpot_estimator/templates/tpottemplates.py` & `TPOT2-0.1.6a1/tpot2/tpot_estimator/templates/tpottemplates.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/utils/eval_utils.py` & `TPOT2-0.1.6a1/tpot2/utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `TPOT2-0.1.6a0/tpot2/utils/utils.py` & `TPOT2-0.1.6a1/tpot2/utils/utils.py`

 * *Files identical despite different names*

