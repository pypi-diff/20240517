# Comparing `tmp/splink-4.0.0.dev3.tar.gz` & `tmp/splink-4.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splink-4.0.0.dev3.tar", max compression
+gzip compressed data, was "splink-4.0.0.dev4.tar", max compression
```

## Comparing `splink-4.0.0.dev3.tar` & `splink-4.0.0.dev4.tar`

### file list

```diff
@@ -1,126 +1,129 @@
--rw-r--r--   0        0        0     1076 2024-03-19 17:14:35.664632 splink-4.0.0.dev3/LICENSE
--rw-r--r--   0        0        0    10918 2024-03-19 17:14:35.664632 splink-4.0.0.dev3/README.md
--rw-r--r--   0        0        0     3053 2024-03-19 17:14:35.808634 splink-4.0.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     2076 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/__init__.py
--rw-r--r--   0        0        0    11964 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/accuracy.py
--rw-r--r--   0        0        0     8219 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/analyse_blocking.py
--rw-r--r--   0        0        0      350 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/athena/athena_helpers/athena_transforms.py
--rw-r--r--   0        0        0     2999 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/athena/athena_helpers/athena_utils.py
--rw-r--r--   0        0        0    22477 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/athena/linker.py
--rw-r--r--   0        0        0     2880 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/block_from_labels.py
--rw-r--r--   0        0        0    19828 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/blocking.py
--rw-r--r--   0        0        0     1565 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/blocking_rule_creator.py
--rw-r--r--   0        0        0     5812 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/blocking_rule_library.py
--rw-r--r--   0        0        0     2223 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/cache_dict_with_logging.py
--rw-r--r--   0        0        0    14670 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/charts.py
--rw-r--r--   0        0        0    13777 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/cluster_studio.py
--rw-r--r--   0        0        0     9379 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/column_expression.py
--rw-r--r--   0        0        0    16200 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/comparison.py
--rw-r--r--   0        0        0     8269 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/comparison_creator.py
--rw-r--r--   0        0        0     8940 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/comparison_helpers.py
--rw-r--r--   0        0        0    24733 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/comparison_level.py
--rw-r--r--   0        0        0     3898 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/comparison_level_composition.py
--rw-r--r--   0        0        0     5089 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/comparison_level_creator.py
--rw-r--r--   0        0        0    29471 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/comparison_level_library.py
--rw-r--r--   0        0        0     1242 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/comparison_level_sql.py
--rw-r--r--   0        0        0    24616 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/comparison_library.py
--rw-r--r--   0        0        0    24249 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/comparison_template_library.py
--rw-r--r--   0        0        0      972 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/comparison_vector_distribution.py
--rw-r--r--   0        0        0      866 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/comparison_vector_values.py
--rw-r--r--   0        0        0    16881 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/connected_components.py
--rw-r--r--   0        0        0       67 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/constants.py
--rw-r--r--   0        0        0     4621 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/cost_of_blocking_rules.py
--rw-r--r--   0        0        0    12512 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/database_api.py
--rw-r--r--   0        0        0     2487 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/databricks/enable_splink.py
--rw-r--r--   0        0        0     9695 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/datasets/__init__.py
--rw-r--r--   0        0        0      609 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/default_from_jsonschema.py
--rw-r--r--   0        0        0    15906 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/dialects.py
--rw-r--r--   0        0        0     4369 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/duckdb/database_api.py
--rw-r--r--   0        0        0     2735 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/duckdb/dataframe.py
--rw-r--r--   0        0        0     1750 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/duckdb/duckdb_helpers/duckdb_helpers.py
--rw-r--r--   0        0        0     4971 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/edge_metrics.py
--rw-r--r--   0        0        0    16240 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/em_training_session.py
--rw-r--r--   0        0        0     6689 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/estimate_u.py
--rw-r--r--   0        0        0     3179 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/exceptions.py
--rw-r--r--   0        0        0    14711 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/expectation_maximisation.py
--rw-r--r--   0        0        0   101742 2024-03-19 17:14:35.812634 splink-4.0.0.dev3/splink/files/DEPENDENCY_LICENSES.txt
--rw-r--r--   0        0        0     6779 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/accuracy_chart.json
--rw-r--r--   0        0        0     1562 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/blocking_rule_generated_comparisons.json
--rw-r--r--   0        0        0     3785 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/comparator_score_chart.json
--rw-r--r--   0        0        0     6417 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/comparator_score_threshold_chart.json
--rw-r--r--   0        0        0     2775 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/completeness.json
--rw-r--r--   0        0        0     5795 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/m_u_parameters_interactive_history.json
--rw-r--r--   0        0        0     1111 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/match_weight_histogram.json
--rw-r--r--   0        0        0     6963 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/match_weights_interactive_history.json
--rw-r--r--   0        0        0     9115 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/match_weights_waterfall.json
--rw-r--r--   0        0        0     1832 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/missingness.json
--rw-r--r--   0        0        0     2753 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/parameter_estimate_comparisons.json
--rw-r--r--   0        0        0     2660 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/phonetic_match_chart.json
--rw-r--r--   0        0        0     1654 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/precision_recall.json
--rw-r--r--   0        0        0     1125 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/probability_two_random_records_match_iteration.json
--rw-r--r--   0        0        0     2326 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/profile_data.json
--rw-r--r--   0        0        0     1805 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/roc.json
--rw-r--r--   0        0        0     9910 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/tf_adjustment_chart.json
--rw-r--r--   0        0        0    37548 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/threshold_selection_tool.json
--rw-r--r--   0        0        0     2910 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/chart_defs/unlinkables_chart_def.json
--rw-r--r--   0        0        0   279633 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/external_js/d3@7.8.5
--rw-r--r--   0        0        0    45883 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/external_js/stdlib.js@5.8.3
--rw-r--r--   0        0        0    66064 2024-03-19 17:14:35.816634 splink-4.0.0.dev3/splink/files/external_js/vega-embed@6.20.2
--rw-r--r--   0        0        0   256817 2024-03-19 17:14:35.820634 splink-4.0.0.dev3/splink/files/external_js/vega-lite@5.2.0
--rw-r--r--   0        0        0   501599 2024-03-19 17:14:35.820634 splink-4.0.0.dev3/splink/files/external_js/vega@5.21.0
--rw-r--r--   0        0        0   920157 2024-03-19 17:14:35.824634 splink-4.0.0.dev3/splink/files/labelling_tool/slt.js
--rw-r--r--   0        0        0     4104 2024-03-19 17:14:35.824634 splink-4.0.0.dev3/splink/files/labelling_tool/template.j2
--rw-r--r--   0        0        0    13833 2024-03-19 17:14:35.824634 splink-4.0.0.dev3/splink/files/settings_jsonschema.json
--rw-r--r--   0        0        0  1228220 2024-03-19 17:14:35.828634 splink-4.0.0.dev3/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
--rw-r--r--   0        0        0   944614 2024-03-19 17:14:35.836634 splink-4.0.0.dev3/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
--rw-r--r--   0        0        0   949562 2024-03-19 17:14:35.840634 splink-4.0.0.dev3/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
--rw-r--r--   0        0        0     6506 2024-03-19 17:14:35.840634 splink-4.0.0.dev3/splink/files/splink_cluster_studio/cluster_template.j2
--rw-r--r--   0        0        0     2269 2024-03-19 17:14:35.840634 splink-4.0.0.dev3/splink/files/splink_cluster_studio/custom.css
--rw-r--r--   0        0        0     2269 2024-03-19 17:14:35.840634 splink-4.0.0.dev3/splink/files/splink_comparison_viewer/custom.css
--rw-r--r--   0        0        0     4120 2024-03-19 17:14:35.840634 splink-4.0.0.dev3/splink/files/splink_comparison_viewer/template.j2
--rw-r--r--   0        0        0   321314 2024-03-19 17:14:35.840634 splink-4.0.0.dev3/splink/files/splink_vis_utils/splink_vis_utils.js
--rw-r--r--   0        0        0      404 2024-03-19 17:14:35.840634 splink-4.0.0.dev3/splink/files/templates/single_chart_template.html
--rw-r--r--   0        0        0     8692 2024-03-19 17:14:35.840634 splink-4.0.0.dev3/splink/find_brs_with_comparison_counts_below_threshold.py
--rw-r--r--   0        0        0     1313 2024-03-19 17:14:35.840634 splink-4.0.0.dev3/splink/find_matches_to_new_records.py
--rw-r--r--   0        0        0     9974 2024-03-19 17:14:35.840634 splink-4.0.0.dev3/splink/graph_metrics.py
--rw-r--r--   0        0        0    12373 2024-03-19 17:14:35.840634 splink-4.0.0.dev3/splink/input_column.py
--rw-r--r--   0        0        0     3447 2024-03-19 17:14:35.840634 splink-4.0.0.dev3/splink/labelling_tool.py
--rw-r--r--   0        0        0   153463 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/linker.py
--rw-r--r--   0        0        0      300 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/logging_messages.py
--rw-r--r--   0        0        0     3130 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/lower_id_on_lhs.py
--rw-r--r--   0        0        0     2056 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/m_from_labels.py
--rw-r--r--   0        0        0     2762 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/m_training.py
--rw-r--r--   0        0        0     2637 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/m_u_records_to_parameters.py
--rw-r--r--   0        0        0      623 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/match_key_analysis.py
--rw-r--r--   0        0        0     2028 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/match_weights_histogram.py
--rw-r--r--   0        0        0     5990 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/misc.py
--rw-r--r--   0        0        0     2820 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/missingness.py
--rw-r--r--   0        0        0     7009 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/optimise_cost_of_brs.py
--rw-r--r--   0        0        0     2201 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/parse_sql.py
--rw-r--r--   0        0        0     2696 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/pipeline.py
--rw-r--r--   0        0        0     6428 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/postgres/database_api.py
--rw-r--r--   0        0        0     2368 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/postgres/dataframe.py
--rw-r--r--   0        0        0     7479 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/predict.py
--rw-r--r--   0        0        0    11222 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/profile_data.py
--rw-r--r--   0        0        0    23912 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/settings.py
--rw-r--r--   0        0        0     5817 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/settings_creator.py
--rw-r--r--   0        0        0     9341 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/settings_validation/log_invalid_columns.py
--rw-r--r--   0        0        0     4062 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/settings_validation/settings_column_cleaner.py
--rw-r--r--   0        0        0     6373 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/settings_validation/settings_validation_log_strings.py
--rw-r--r--   0        0        0     6478 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/settings_validation/valid_types.py
--rw-r--r--   0        0        0    13235 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/spark/database_api.py
--rw-r--r--   0        0        0     2218 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/spark/dataframe.py
--rw-r--r--   0        0        0     2235 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/spark/jar_location.py
--rw-r--r--   0        0        0     1110 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/spark/spark_helpers/custom_spark_dialect.py
--rw-r--r--   0        0        0     5087 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/splink_comparison_viewer.py
--rw-r--r--   0        0        0     6745 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/splink_dataframe.py
--rw-r--r--   0        0        0     4539 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/sql_transform.py
--rw-r--r--   0        0        0     3471 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/sqlite/database_api.py
--rw-r--r--   0        0        0     2256 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/sqlite/dataframe.py
--rw-r--r--   0        0        0     9774 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/term_frequencies.py
--rw-r--r--   0        0        0     1022 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/unique_id_concat.py
--rw-r--r--   0        0        0     1673 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/unlinkables.py
--rw-r--r--   0        0        0     2383 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/validate_jsonschema.py
--rw-r--r--   0        0        0     2427 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/vertically_concatenate.py
--rw-r--r--   0        0        0     5573 2024-03-19 17:14:35.844634 splink-4.0.0.dev3/splink/waterfall_chart.py
--rw-r--r--   0        0        0    12282 1970-01-01 00:00:00.000000 splink-4.0.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-17 12:06:36.526048 splink-4.0.0.dev4/LICENSE
+-rw-r--r--   0        0        0    11224 2024-05-17 12:06:36.526048 splink-4.0.0.dev4/README.md
+-rw-r--r--   0        0        0     3738 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0     2076 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/__init__.py
+-rw-r--r--   0        0        0    19195 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/accuracy.py
+-rw-r--r--   0        0        0      350 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/athena/athena_helpers/athena_transforms.py
+-rw-r--r--   0        0        0     2999 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/athena/athena_helpers/athena_utils.py
+-rw-r--r--   0        0        0    23535 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/athena/linker.py
+-rw-r--r--   0        0        0     2932 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/block_from_labels.py
+-rw-r--r--   0        0        0    21352 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/blocking.py
+-rw-r--r--   0        0        0      416 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/blocking_analysis.py
+-rw-r--r--   0        0        0     1774 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/blocking_rule_creator.py
+-rw-r--r--   0        0        0     1398 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/blocking_rule_creator_utils.py
+-rw-r--r--   0        0        0     5992 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/blocking_rule_library.py
+-rw-r--r--   0        0        0     2371 2024-05-17 12:06:36.674049 splink-4.0.0.dev4/splink/cache_dict_with_logging.py
+-rw-r--r--   0        0        0    14938 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/charts.py
+-rw-r--r--   0        0        0    14547 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/cluster_studio.py
+-rw-r--r--   0        0        0     9629 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/column_expression.py
+-rw-r--r--   0        0        0    16520 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison.py
+-rw-r--r--   0        0        0     8440 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_creator.py
+-rw-r--r--   0        0        0     8940 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_helpers.py
+-rw-r--r--   0        0        0    26220 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_level.py
+-rw-r--r--   0        0        0     3948 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_level_composition.py
+-rw-r--r--   0        0        0     5211 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_level_creator.py
+-rw-r--r--   0        0        0    29966 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_level_library.py
+-rw-r--r--   0        0        0     1242 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_level_sql.py
+-rw-r--r--   0        0        0    24897 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_library.py
+-rw-r--r--   0        0        0    24992 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_template_library.py
+-rw-r--r--   0        0        0      979 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_vector_distribution.py
+-rw-r--r--   0        0        0      874 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/comparison_vector_values.py
+-rw-r--r--   0        0        0    17476 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/connected_components.py
+-rw-r--r--   0        0        0       67 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/constants.py
+-rw-r--r--   0        0        0     4693 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/cost_of_blocking_rules.py
+-rw-r--r--   0        0        0    13026 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/database_api.py
+-rw-r--r--   0        0        0     2487 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/databricks/enable_splink.py
+-rw-r--r--   0        0        0     9801 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/datasets/__init__.py
+-rw-r--r--   0        0        0      609 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/default_from_jsonschema.py
+-rw-r--r--   0        0        0    16429 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/dialects.py
+-rw-r--r--   0        0        0     3706 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/duckdb/database_api.py
+-rw-r--r--   0        0        0     2735 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/duckdb/dataframe.py
+-rw-r--r--   0        0        0     1762 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/duckdb/duckdb_helpers/duckdb_helpers.py
+-rw-r--r--   0        0        0     5279 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/edge_metrics.py
+-rw-r--r--   0        0        0    17045 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/em_training_session.py
+-rw-r--r--   0        0        0     7922 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/estimate_u.py
+-rw-r--r--   0        0        0     3226 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/exceptions.py
+-rw-r--r--   0        0        0    15022 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/expectation_maximisation.py
+-rw-r--r--   0        0        0      160 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/exploratory.py
+-rw-r--r--   0        0        0   101742 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/DEPENDENCY_LICENSES.txt
+-rw-r--r--   0        0        0     6779 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/accuracy_chart.json
+-rw-r--r--   0        0        0     1316 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/blocking_rule_generated_comparisons.json
+-rw-r--r--   0        0        0     3785 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/comparator_score_chart.json
+-rw-r--r--   0        0        0     6417 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/comparator_score_threshold_chart.json
+-rw-r--r--   0        0        0     2775 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/completeness.json
+-rw-r--r--   0        0        0     5795 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/m_u_parameters_interactive_history.json
+-rw-r--r--   0        0        0     1111 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/match_weight_histogram.json
+-rw-r--r--   0        0        0     6963 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/match_weights_interactive_history.json
+-rw-r--r--   0        0        0     9115 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/match_weights_waterfall.json
+-rw-r--r--   0        0        0     1832 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/missingness.json
+-rw-r--r--   0        0        0     2753 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/parameter_estimate_comparisons.json
+-rw-r--r--   0        0        0     2660 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/phonetic_match_chart.json
+-rw-r--r--   0        0        0     1654 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/precision_recall.json
+-rw-r--r--   0        0        0     1125 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/probability_two_random_records_match_iteration.json
+-rw-r--r--   0        0        0     2326 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/profile_data.json
+-rw-r--r--   0        0        0     1805 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/roc.json
+-rw-r--r--   0        0        0     9910 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/tf_adjustment_chart.json
+-rw-r--r--   0        0        0    37552 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/threshold_selection_tool.json
+-rw-r--r--   0        0        0     2910 2024-05-17 12:06:36.678048 splink-4.0.0.dev4/splink/files/chart_defs/unlinkables_chart_def.json
+-rw-r--r--   0        0        0   279633 2024-05-17 12:06:36.682048 splink-4.0.0.dev4/splink/files/external_js/d3@7.8.5
+-rw-r--r--   0        0        0    45883 2024-05-17 12:06:36.682048 splink-4.0.0.dev4/splink/files/external_js/stdlib.js@5.8.3
+-rw-r--r--   0        0        0    66064 2024-05-17 12:06:36.682048 splink-4.0.0.dev4/splink/files/external_js/vega-embed@6.20.2
+-rw-r--r--   0        0        0   256817 2024-05-17 12:06:36.682048 splink-4.0.0.dev4/splink/files/external_js/vega-lite@5.2.0
+-rw-r--r--   0        0        0   501599 2024-05-17 12:06:36.686048 splink-4.0.0.dev4/splink/files/external_js/vega@5.21.0
+-rw-r--r--   0        0        0   920157 2024-05-17 12:06:36.690049 splink-4.0.0.dev4/splink/files/labelling_tool/slt.js
+-rw-r--r--   0        0        0     4104 2024-05-17 12:06:36.690049 splink-4.0.0.dev4/splink/files/labelling_tool/template.j2
+-rw-r--r--   0        0        0    14089 2024-05-17 12:06:36.690049 splink-4.0.0.dev4/splink/files/settings_jsonschema.json
+-rw-r--r--   0        0        0  1228220 2024-05-17 12:06:36.694049 splink-4.0.0.dev4/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
+-rw-r--r--   0        0        0   944614 2024-05-17 12:06:36.702048 splink-4.0.0.dev4/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
+-rw-r--r--   0        0        0   949562 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
+-rw-r--r--   0        0        0     6506 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/files/splink_cluster_studio/cluster_template.j2
+-rw-r--r--   0        0        0     2269 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/files/splink_cluster_studio/custom.css
+-rw-r--r--   0        0        0     2269 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/files/splink_comparison_viewer/custom.css
+-rw-r--r--   0        0        0     4120 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/files/splink_comparison_viewer/template.j2
+-rw-r--r--   0        0        0   321314 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/files/splink_vis_utils/splink_vis_utils.js
+-rw-r--r--   0        0        0      404 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/files/templates/single_chart_template.html
+-rw-r--r--   0        0        0     9072 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/find_brs_with_comparison_counts_below_threshold.py
+-rw-r--r--   0        0        0     1488 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/find_matches_to_new_records.py
+-rw-r--r--   0        0        0    10088 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/graph_metrics.py
+-rw-r--r--   0        0        0    12400 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/input_column.py
+-rw-r--r--   0        0        0    23741 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/internals/blocking_analysis.py
+-rw-r--r--   0        0        0     4066 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/internals/completeness.py
+-rw-r--r--   0        0        0    11706 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/internals/profile_data.py
+-rw-r--r--   0        0        0     3763 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/labelling_tool.py
+-rw-r--r--   0        0        0   137958 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/linker.py
+-rw-r--r--   0        0        0      300 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/logging_messages.py
+-rw-r--r--   0        0        0     3191 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/lower_id_on_lhs.py
+-rw-r--r--   0        0        0     2195 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/m_from_labels.py
+-rw-r--r--   0        0        0     3238 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/m_training.py
+-rw-r--r--   0        0        0     2696 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/m_u_records_to_parameters.py
+-rw-r--r--   0        0        0      623 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/match_key_analysis.py
+-rw-r--r--   0        0        0     2162 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/match_weights_histogram.py
+-rw-r--r--   0        0        0     5482 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/misc.py
+-rw-r--r--   0        0        0     7096 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/optimise_cost_of_brs.py
+-rw-r--r--   0        0        0     2232 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/parse_sql.py
+-rw-r--r--   0        0        0     3784 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/pipeline.py
+-rw-r--r--   0        0        0     6487 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/postgres/database_api.py
+-rw-r--r--   0        0        0     2379 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/postgres/dataframe.py
+-rw-r--r--   0        0        0     7516 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/predict.py
+-rw-r--r--   0        0        0    24963 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/settings.py
+-rw-r--r--   0        0        0     5491 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/settings_creator.py
+-rw-r--r--   0        0        0     9998 2024-05-17 12:06:36.706049 splink-4.0.0.dev4/splink/settings_validation/log_invalid_columns.py
+-rw-r--r--   0        0        0     4694 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/settings_validation/settings_column_cleaner.py
+-rw-r--r--   0        0        0     6613 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/settings_validation/settings_validation_log_strings.py
+-rw-r--r--   0        0        0      797 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/settings_validation/valid_types.py
+-rw-r--r--   0        0        0    13344 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/spark/database_api.py
+-rw-r--r--   0        0        0     2224 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/spark/dataframe.py
+-rw-r--r--   0        0        0     2235 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/spark/jar_location.py
+-rw-r--r--   0        0        0     1110 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/spark/spark_helpers/custom_spark_dialect.py
+-rw-r--r--   0        0        0     5180 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/splink_comparison_viewer.py
+-rw-r--r--   0        0        0     6785 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/splink_dataframe.py
+-rw-r--r--   0        0        0     4673 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/sql_transform.py
+-rw-r--r--   0        0        0     3503 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/sqlite/database_api.py
+-rw-r--r--   0        0        0     2267 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/sqlite/dataframe.py
+-rw-r--r--   0        0        0    10265 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/term_frequencies.py
+-rw-r--r--   0        0        0     1143 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/unique_id_concat.py
+-rw-r--r--   0        0        0     1798 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/unlinkables.py
+-rw-r--r--   0        0        0     2460 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/validate_jsonschema.py
+-rw-r--r--   0        0        0     7428 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/vertically_concatenate.py
+-rw-r--r--   0        0        0     5665 2024-05-17 12:06:36.710049 splink-4.0.0.dev4/splink/waterfall_chart.py
+-rw-r--r--   0        0        0    12705 1970-01-01 00:00:00.000000 splink-4.0.0.dev4/PKG-INFO
```

### Comparing `splink-4.0.0.dev3/LICENSE` & `splink-4.0.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/README.md` & `splink-4.0.0.dev4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 <img src="https://user-images.githubusercontent.com/7570107/85285114-3969ac00-b488-11ea-88ff-5fca1b34af1f.png" alt="Splink Logo" height="150px">
 </p>
 
 [![pypi](https://img.shields.io/github/v/release/moj-analytical-services/splink?include_prereleases)](https://pypi.org/project/splink/#history)
 [![Downloads](https://static.pepy.tech/badge/splink/month)](https://pepy.tech/project/splink)
 [![Documentation](https://img.shields.io/badge/API-documentation-blue)](https://moj-analytical-services.github.io/splink/)
 
-
+> [!IMPORTANT]
+> Development has begun on Splink 4 on the `splink4_dev` branch.  Splink 3 is in maintenance mode and we are no longer accepting new features. We welcome contributions to Splink 4. Read more on our latest [blog](https://moj-analytical-services.github.io/splink/blog/2024/03/19/splink4.html).
 
 # Fast, accurate and scalable probabilistic data linkage
 
 Splink is a Python package for probabilistic record linkage (entity resolution) that allows you to deduplicate and link records from datasets that lack unique identifiers.
 
 ## Key Features
```

### Comparing `splink-4.0.0.dev3/pyproject.toml` & `splink-4.0.0.dev4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splink"
-version = "4.0.0.dev3"
+version = "4.0.0.dev4"
 description = "Fast probabilistic data linkage at scale"
 authors = ["Robin Linacre <robinlinacre@hotmail.com>", "Sam Lindsay", "Theodore Manassis", "Tom Hepworth", "Andy Bond", "Ross Kennedy"]
 license = "MIT"
 homepage = "https://github.com/moj-analytical-services/splink"
 repository = "https://github.com/moj-analytical-services/splink"
 readme = "README.md"
 
@@ -15,15 +15,25 @@
 pandas = ">1.3.5"
 duckdb = ">=0.9.2"
 sqlglot = ">=13.0.0"
 altair = "^5.0.1"
 Jinja2 = ">=3.0.3"
 phonetics = ">=1.0.5"
 
+# need to manually specify numpy versions suitable for CI
+# 1.24.4 works with python 3.8, but not 3.12
+numpy = [
+    # version is minimum valid with above listed pandas version
+    {version=">=1.17.3", python = "<3.12"},
+    {version=">=1.26.0", python = ">=3.12"},
+]
+
+
 # Optional installs
+# python >=3.12 requires pyspark >=4.0.0 - currently unreleased
 pyspark = {version=">=3.2.1", optional=true}
 
 awswrangler = [
     {version=">=3.0.0,<4.0.0", python = ">=3.8", optional=true}
 ]
 
 psycopg2-binary = {version=">=2.8.0", optional=true}
@@ -38,16 +48,15 @@
 sqlalchemy = ">=1.4.0"
 # temporarily use binary version, to avoid issues with pg_config path
 psycopg2-binary = ">=2.8.0"
 igraph = ">=0.11.2"
 
 [tool.poetry.group.linting]
 [tool.poetry.group.linting.dependencies]
-black = "22.6.0"
-ruff = "0.0.257"
+ruff = "^0.4.2"
 
 [tool.poetry.group.testing]
 [tool.poetry.group.testing.dependencies]
 # pin to reduce dependencies
 pytest = ">=7.3"
 pyarrow = ">=7.0.0"
 networkx = ">=2.5.1"
@@ -69,28 +78,28 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.ruff]
 line-length = 88
-select = [
+lint.select = [
     # Pyflakes
     "F",
     # Pycodestyle
     "E",
     "W",
     # isort
     "I001",
     # bugbear
     "B",
     # flake8-print
     "T20"
 ]
-ignore = [
+lint.ignore = [
     "B905", # `zip()` without an explicit `strict=` parameter
     "B006", # Do not use mutable data structures for argument defaults"
 ]
 
 [tool.pytest.ini_options]
 addopts = ["-m default"]
 markers = [
@@ -102,27 +111,37 @@
 # backend-specific sets
     "duckdb",
     "duckdb_only",
     "spark",
     "spark_only",
     "sqlite",
     "sqlite_only",
+    "postgres",
+    "postgres_only",
 ]
 
 [tool.mypy]
 packages = "splink"
-# temporary exclusions
-exclude = [
-    # modules with large number of errors
-    '.*comparison.*library\.py',
-    '.*linker\.py',
-    '/settings_validation/'
-]
 # for now at least allow implicit optionals
 # to cut down on noise. Easy to fix.
 implicit_optional = true
 # for now, ignore missing imports
 # can remove later and install stubs, where existent
 ignore_missing_imports = true
-# don't follow imports to modules we don't want to typecheck yet
-# eventually restore this back to the default "normal"
-follow_imports = "silent"
+
+# options for strict mode
+# too much to handle at once, so opt-in a little at a time
+# https://mypy.readthedocs.io/en/stable/existing_code.html#introduce-stricter-options
+warn_unused_configs = true
+warn_redundant_casts = true
+warn_unused_ignores = true
+strict_equality = true
+# don't worry about warning: https://github.com/python/mypy/issues/16189
+strict_concatenate = true
+check_untyped_defs = true
+disallow_subclassing_any = true
+disallow_untyped_decorators = true
+disallow_any_generics = true
+# further strict checks to add in:
+# disallow_untyped_calls = true
+disallow_incomplete_defs = true
+# disallow_untyped_defs = true
```

### Comparing `splink-4.0.0.dev3/splink/__init__.py` & `splink-4.0.0.dev4/splink/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,8 +53,8 @@
                 f"{name} cannot be imported because its dependencies are not "
                 "installed. Please `pip install` the required package(s) as "
                 "specified in the optional dependencies in pyproject.toml"
             ) from err
     raise AttributeError(f"module 'splink' has no attribute '{name}'") from None
 
 
-__version__ = "4.0.0.dev3"
+__version__ = "4.0.0.dev4"
```

### Comparing `splink-4.0.0.dev3/splink/analyse_blocking.py` & `splink-4.0.0.dev4/splink/find_brs_with_comparison_counts_below_threshold.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,251 +1,256 @@
 from __future__ import annotations
 
-from copy import deepcopy
-from typing import TYPE_CHECKING, Union
+import logging
+import string
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Set
 
 import pandas as pd
 
-from .blocking import BlockingRule, _sql_gen_where_condition, block_using_rules_sqls
-from .misc import calculate_cartesian, calculate_reduction_ratio
+from .blocking import BlockingRule
+from .blocking_rule_creator import BlockingRuleCreator
+from .blocking_rule_library import CustomRule, block_on
+from .database_api import DatabaseAPISubClass
+from .input_column import InputColumn
+from .internals.blocking_analysis import (
+    _count_comparisons_generated_from_blocking_rule,
+)
 
-# https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
     from .linker import Linker
+logger = logging.getLogger(__name__)
 
 
-def number_of_comparisons_generated_by_blocking_rule_post_filters_sql(
-    linker: Linker,
-    blocking_rule,
-) -> str:
-    settings_obj = linker._settings_obj
-
-    where_condition = _sql_gen_where_condition(
-        settings_obj._link_type,
-        settings_obj.column_info_settings.unique_id_input_columns,
-    )
-
-    sql = f"""
-    select count(*) as count_of_pairwise_comparisons_generated
-
-    from __splink__df_concat as l
-    inner join __splink__df_concat as r
-    on
-    {blocking_rule}
-    {where_condition}
+def sanitise_column_name_for_one_hot_encoding(column_name: str) -> str:
+    allowed_chars = string.ascii_letters + string.digits + "_"
+    sanitised_name = "".join(c for c in column_name if c in allowed_chars)
+    return sanitised_name
+
+
+def _generate_output_combinations_table_row(
+    blocking_columns: list[str],
+    splink_blocking_rule: BlockingRule,
+    comparison_count: int,
+    all_columns: list[str],
+) -> dict[str, Any]:
+    row: dict[str, Any] = {}
+
+    blocking_columns = [
+        sanitise_column_name_for_one_hot_encoding(c) for c in blocking_columns
+    ]
+    all_columns = [sanitise_column_name_for_one_hot_encoding(c) for c in all_columns]
+
+    row["blocking_columns_sanitised"] = blocking_columns
+    row["splink_blocking_rule"] = splink_blocking_rule
+    row["comparison_count"] = comparison_count
+    row["num_equi_joins"] = len(blocking_columns)
+
+    for col in all_columns:
+        row[f"__fixed__{col}"] = 1 if col in blocking_columns else 0
+
+    return row
+
+
+def _generate_combinations(
+    all_columns: list[str],
+    current_combination: list[str],
+    already_visited: Set[frozenset[str]],
+) -> list[list[str]]:
+    """Generate combinations of columns to visit that haven't been visited already
+    irrespective of order
     """
 
-    return sql
+    combinations = []
+    for col in all_columns:
+        if col not in current_combination:
+            next_combination = current_combination + [col]
+            if frozenset(next_combination) not in already_visited:
+                combinations.append(next_combination)
+
+    return combinations
+
+
+def _generate_blocking_rule(
+    db_api: DatabaseAPISubClass, cols_as_string: List[str]
+) -> BlockingRule:
+    """Generate a Splink blocking rule given a list of column names which
+    are provided as as string"""
 
+    if len(cols_as_string) == 0:
+        br: BlockingRuleCreator = CustomRule("1=1", db_api.sql_dialect.name)
+    else:
+        br = block_on(*cols_as_string)
 
-def cumulative_comparisons_generated_by_blocking_rules(
-    linker: Linker, blocking_rules, output_chart=True, return_dataframe=False
-):
-    # Deepcopy our original linker so we can safely adjust our settings.
-    # This is particularly important to ensure we don't overwrite our
-    # original blocking rules.
-    linker = deepcopy(linker)
-
-    settings_obj = linker._settings_obj
-    linker._settings_obj = settings_obj
-    linker._analyse_blocking_mode = True
-
-    if blocking_rules:
-        brs_as_objs = settings_obj._brs_as_objs(blocking_rules)
-        linker._settings_obj._blocking_rules_to_generate_predictions = brs_as_objs
-
-    # Turn tf off.  No need to apply term frequencies to perform these calcs
-    settings_obj._retain_matching_columns = False
-    settings_obj._retain_intermediate_calculation_columns = False
-    for cc in settings_obj.comparisons:
-        for cl in cc.comparison_levels:
-            # TODO: ComparisonLevel: manage access
-            cl._tf_adjustment_column = None
-
-    concat = linker._initialise_df_concat(materialise=True)
-
-    # Calculate the Cartesian Product
-    if output_chart:
-        # We only need the cartesian product if we want to output the chart view
+    return br.get_blocking_rule(db_api.sql_dialect.name)
 
-        if settings_obj._link_type == "dedupe_only":
-            group_by_statement = ""
-        else:
-            group_by_statement = "group by source_dataset"
 
-        sql = f"""
-            select count(*) as count
-            from {concat.physical_name}
-            {group_by_statement}
-        """
-        linker._enqueue_sql(sql, "__splink__cartesian_product")
-        cartesian_count = linker._execute_sql_pipeline([concat])
-        row_count_df = cartesian_count.as_record_dict()
-        cartesian_count.drop_table_from_database_and_remove_from_cache()
-
-        cartesian = calculate_cartesian(row_count_df, settings_obj._link_type)
-
-    # Calculate the total number of rows generated by each blocking rule
-    sql_infos = block_using_rules_sqls(linker)
-    for sql_info in sql_infos:
-        linker._enqueue_sql(sql_info["sql"], sql_info["output_table_name"])
-
-    brs_as_objs = linker._settings_obj._blocking_rules_to_generate_predictions
-
-    sql = """
-        select
-        count(*) as row_count,
-        match_key
-        from __splink__df_blocked
-        group by match_key
-        order by cast(match_key as int) asc
+def _search_tree_for_blocking_rules_below_threshold_count(
+    linker: "Linker",
+    all_columns: List[str],
+    threshold: int,
+    current_combination: List[str] = None,
+    already_visited: Set[frozenset[str]] = None,
+    results: List[Dict[str, str]] = None,
+) -> List[Dict[str, str]]:
     """
-    linker._enqueue_sql(sql, "__splink__df_count_cumulative_blocks")
-    cumulative_blocking_rule_count = linker._execute_sql_pipeline([concat])
-    br_n = cumulative_blocking_rule_count.as_pandas_dataframe()
-    # not all dialects return column names when frame is empty (e.g. sqlite, postgres)
-    if br_n.empty:
-        br_n["row_count"] = []
-        br_n["match_key"] = []
-    cumulative_blocking_rule_count.drop_table_from_database_and_remove_from_cache()
-    br_count, br_keys = list(br_n["row_count"]), list(br_n["match_key"].astype("int"))
-
-    if len(br_count) != len(brs_as_objs):
-        missing_br = [x for x in range(len(brs_as_objs)) if x not in br_keys]
-        for n in missing_br:
-            br_count.insert(n, 0)
-
-    br_comparisons = []
-    cumulative_sum = 0
-    # Wrap everything into an output dictionary
-    for row, br in zip(br_count, brs_as_objs):
-        out_dict = {
-            "row_count": row,
-            "rule": br.blocking_rule_sql,
-        }
-        if output_chart:
-            cumulative_sum += row
-            # Increase round threshold to capture more info on larger datasets
-            rr = round(calculate_reduction_ratio(cumulative_sum, cartesian), 6)
-
-            rr_text = (
-                "The rolling reduction ratio with your given blocking rule(s) "
-                f"is {rr}. This represents the reduction in the total number "
-                "of comparisons due to your rule(s)."
-            )
-
-            additional_vals = {
-                "cumulative_rows": cumulative_sum,
-                "cartesian": int(cartesian),
-                "reduction_ratio": rr_text,
-                "start": cumulative_sum - row,
-            }
-            out_dict = {**out_dict, **additional_vals}
+    Recursively search combinations of fields to find ones that result in a count less
+    than the threshold.
 
-        br_comparisons.append(out_dict.copy())
-
-    linker._analyse_blocking_mode = False
-
-    if return_dataframe:
-        return pd.DataFrame(br_comparisons)
+    Uses the new, fast counting function
+    linker._count_num_comparisons_from_blocking_rule_pre_filter_conditions
+    to count
+
+    The full tree looks like this, where c1 c2 are columns:
+    c1                    count_comparisons(c1)
+    ├── c2                count_comparisons(c1, c2)
+    │   └── c3            count_comparisons(c1, c2, c3)
+    ├── c3                count_comparisons(c1, c3)
+    │   └── c2            count_comparisons(c1, c3, c2)
+    c2                    count_comparisons(c2)
+    ├── c1                count_comparisons(c2, c1)
+    │   └── c3            count_comparisons(c2, c1, c3)
+    ├── c3                count_comparisons(c2, c3)
+    │   └── c1            count_comparisons(c2, c3, c1)
+
+    But many nodes do not need to be visited:
+        - Once the count is below the threshold, no branches from the node are explored.
+        - If a combination has alraedy been evaluated, it is not evaluated again. For
+          example, c2 -> c1 will not be evaluated because c1 -> c2 has already been
+          counted
+
+    When a count is below the threshold, create a dictionary with the relevant stats
+    like :
+    {
+        'blocking_columns_sanitised':['first_name'],
+        'splink_blocking_rule':<Custom rule>',
+        comparison_count':4827,
+        'num_equi_join':1,
+        '__fixed__first_name':1,
+        '__fixed__surname':0,
+        '__fixed__dob':0,
+        '__fixed__city':0,
+        '__fixed__email':0,
+        '__fixed__cluster':0,
+    }
+
+    Return a list of these dicts.
+
+
+    Args:
+        linker: splink.Linker
+        fields (List[str]): List of fields to combine.
+        threshold (float): The count threshold.
+        current_combination (List[str], optional): Current combination of fields.
+        already_visited (Set[frozenset], optional): Set of visited combinations.
+        results (List[Dict[str, str]], optional): List of results. Defaults to [].
+
+    Returns:
+        List[Dict]: List of results.  Each result is a dict with statistics like
+            the number of comparisons, the blocking rule etc.
+    """
+    if current_combination is None:
+        current_combination = []
+    if already_visited is None:
+        already_visited = set()
+    if results is None:
+        results = []
+
+    if len(current_combination) == len(all_columns):
+        return results  # All fields included, meaning we're at a leaf so exit recursion
+
+    br = _generate_blocking_rule(linker.db_api, current_combination)
+
+    comparison_count = _count_comparisons_generated_from_blocking_rule(
+        splink_df_dict=linker._input_tables_dict,
+        blocking_rule=br,
+        link_type=linker._settings_obj._link_type,
+        db_api=linker.db_api,
+        compute_post_filter_count=False,
+        source_dataset_column_name=linker._settings_obj.column_info_settings.source_dataset_column_name,
+        unique_id_column_name=linker._settings_obj.column_info_settings.unique_id_column_name,
+    )["number_of_comparisons_generated_pre_filter_conditions"]
+
+    already_visited.add(frozenset(current_combination))
+
+    # int just to satisfy mypy
+    comparison_count = int(comparison_count)
+    if comparison_count > threshold:
+        # Generate all valid combinations and continue the search
+        combinations = _generate_combinations(
+            all_columns, current_combination, already_visited
+        )
+        for next_combination in combinations:
+            _search_tree_for_blocking_rules_below_threshold_count(
+                linker,
+                all_columns,
+                threshold,
+                next_combination,
+                already_visited,
+                results,
+            )
     else:
-        return br_comparisons
+        row = _generate_output_combinations_table_row(
+            current_combination,
+            br,
+            comparison_count,
+            all_columns,
+        )
+        results.append(row)
 
+    return results
 
-def count_comparisons_from_blocking_rule_pre_filter_conditions_sqls(
-    linker: "Linker", blocking_rule: Union[str, "BlockingRule"]
-):
-    if isinstance(blocking_rule, str):
-        blocking_rule = BlockingRule(blocking_rule, sqlglot_dialect=linker._sql_dialect)
-
-    join_conditions = blocking_rule._equi_join_conditions
-
-    l_cols_sel = []
-    r_cols_sel = []
-    l_cols_gb = []
-    r_cols_gb = []
-    using = []
-    for (
-        i,
-        (l_key, r_key),
-    ) in enumerate(join_conditions):
-        l_cols_sel.append(f"{l_key} as key_{i}")
-        r_cols_sel.append(f"{r_key} as key_{i}")
-        l_cols_gb.append(l_key)
-        r_cols_gb.append(r_key)
-        using.append(f"key_{i}")
-
-    l_cols_sel_str = ", ".join(l_cols_sel)
-    r_cols_sel_str = ", ".join(r_cols_sel)
-    l_cols_gb_str = ", ".join(l_cols_gb)
-    r_cols_gb_str = ", ".join(r_cols_gb)
-    using_str = ", ".join(using)
-
-    sqls = []
-
-    if linker._two_dataset_link_only:
-        #    Can just use the raw input datasets
-        keys = list(linker._input_tables_dict.keys())
-        input_tablename_l = linker._input_tables_dict[keys[0]].physical_name
-        input_tablename_r = linker._input_tables_dict[keys[1]].physical_name
 
-    else:
-        input_tablename_l = "__splink__df_concat"
-        input_tablename_r = "__splink__df_concat"
+def find_blocking_rules_below_threshold_comparison_count(
+    linker: "Linker",
+    max_comparisons_per_rule: int,
+    column_expressions: Optional[Sequence[str | InputColumn]] = None,
+) -> pd.DataFrame:
+    """
+    Finds blocking rules which return a comparison count below a given threshold.
 
-    if not join_conditions:
-        if linker._two_dataset_link_only:
-            sql = f"""
-            SELECT
-                (SELECT COUNT(*) FROM {input_tablename_l})
-                *
-                (SELECT COUNT(*) FROM {input_tablename_r})
-                    AS count_of_pairwise_comparisons_generated
-            """
-        else:
-            sql = """
-            select count(*) * count(*) as count_of_pairwise_comparisons_generated
-            from __splink__df_concat
-
-            """
-        sqls.append(
-            {"sql": sql, "output_table_name": "__splink__total_of_block_counts"}
-        )
-        return sqls
+    In addition to returning blocking rules, returns the comparison count and
+    'num_equi_joins', which refers to the number of equi-joins used by the rule.
 
-    sql = f"""
-    select {l_cols_sel_str}, count(*) as count_l
-    from {input_tablename_l}
-    group by {l_cols_gb_str}
-    """
+    Also returns one-hot encoding that describes which columns are __fixed__ by the
+    blocking rule
 
-    sqls.append(
-        {"sql": sql, "output_table_name": "__splink__count_comparisons_from_blocking_l"}
-    )
+    e.g. equality on first_name and surname has num_equi_joins of 2
+
+    Args:
+        linker (Linker): The Linker object
+        max_comparisons_per_rule (int): Max comparisons allowed per blocking rule.
+        column_expressions: List[str] = Algorithm will find combinations of these
+            column expressions to use as blocking rules. If None, uses all columns used
+            by the ComparisonLevels of the Linker. Column expressions can be SQL
+            expressions, not just column names i.e. 'substr(surname, 1,1)' is a valid
+            entry in this list.
 
-    sql = f"""
-    select {r_cols_sel_str}, count(*) as count_r
-    from {input_tablename_r}
-    group by {r_cols_gb_str}
+    Returns:
+        pd.DataFrame: DataFrame with blocking rules, comparison_count and num_equi_joins
     """
 
-    sqls.append(
-        {"sql": sql, "output_table_name": "__splink__count_comparisons_from_blocking_r"}
-    )
+    if column_expressions is None:
+        column_expressions = linker._input_columns(
+            include_unique_id_col_names=False,
+            include_additional_columns_to_retain=False,
+        )
 
-    sql = f"""
-    select *, count_l, count_r, count_l * count_r as block_count
-    from __splink__count_comparisons_from_blocking_l
-    inner join __splink__count_comparisons_from_blocking_r
-    using ({using_str})
-    """
+    column_expressions_as_strings = []
 
-    sqls.append({"sql": sql, "output_table_name": "__splink__block_counts"})
+    for c in column_expressions:
+        if isinstance(c, InputColumn):
+            column_expressions_as_strings.append(c.quote().name)
+        else:
+            column_expressions_as_strings.append(c)
 
-    sql = """
-    select sum(block_count) as count_of_pairwise_comparisons_generated
-    from __splink__block_counts
-    """
+    results = _search_tree_for_blocking_rules_below_threshold_count(
+        linker, column_expressions_as_strings, max_comparisons_per_rule
+    )
 
-    sqls.append({"sql": sql, "output_table_name": "__splink__total_of_block_counts"})
+    if not results:
+        raise ValueError(
+            "No blocking rules could be found that produce a comparison count below "
+            "your chosen max_comparisons_per_rule threshold of "
+            f"{max_comparisons_per_rule}. Try increasing the threshold."
+        )
 
-    return sqls
+    return pd.DataFrame(results)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `splink-4.0.0.dev3/splink/athena/athena_helpers/athena_utils.py` & `splink-4.0.0.dev4/splink/athena/athena_helpers/athena_utils.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/athena/linker.py` & `splink-4.0.0.dev4/splink/athena/linker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,561 +1,563 @@
-from __future__ import annotations
-
-import logging
-import os
-from typing import Union
-
-import awswrangler as wr
-import boto3
-import numpy as np
-import pandas as pd
-
-from ..input_column import InputColumn
-from ..linker import Linker
-from ..logging_messages import execute_sql_logging_message_info, log_sql
-from ..misc import ensure_is_list
-from ..splink_dataframe import SplinkDataFrame
-from ..sql_transform import sqlglot_transform_sql
-from .athena_helpers.athena_transforms import cast_concat_as_varchar
-from .athena_helpers.athena_utils import (
-    _garbage_collection,
-    _verify_athena_inputs,
-)
-
-logger = logging.getLogger(__name__)
-
-
-class AthenaDataFrame(SplinkDataFrame):
-    linker: AthenaLinker
-
-    @property
-    def columns(self):
-        db, tb = self.linker.get_schema_info(self.physical_name)
-        d = wr.catalog.get_table_types(
-            database=db,
-            table=tb,
-            boto3_session=self.linker.boto3_session,
-        )
-
-        cols = list(d.keys())
-        return [InputColumn(c, sql_dialect="presto") for c in cols]
-
-    def validate(self):
-        pass
-
-    def _drop_table_from_database(
-        self, force_non_splink_table=False, delete_s3_data=True
-    ):
-        # Check folder and table set for deletion
-        self._check_drop_folder_created_by_splink(force_non_splink_table)
-        self._check_drop_table_created_by_splink(force_non_splink_table)
-
-        # Delete the table from s3 and your database
-        table_deleted = self.linker._drop_table_from_database_if_exists(
-            self.physical_name
-        )
-        if delete_s3_data and table_deleted:
-            self.linker._delete_table_from_s3(self.physical_name)
-
-    def drop_table_from_database_and_remove_from_cache(
-        self,
-        force_non_splink_table=False,
-        delete_s3_data=True,
-    ):
-        self._drop_table_from_database(
-            force_non_splink_table=force_non_splink_table, delete_s3_data=delete_s3_data
-        )
-        self.linker._remove_splinkdataframe_from_cache(self)
-
-    def _check_drop_folder_created_by_splink(self, force_non_splink_table=False):
-        filepath = self.linker.s3_output
-        filename = self.physical_name
-        # Validate that the folder is a splink generated folder...
-        files = wr.s3.list_objects(
-            path=os.path.join(filepath, filename),
-            boto3_session=self.linker.boto3_session,
-            ignore_empty=True,
-        )
-
-        if len(files) == 0:
-            if not force_non_splink_table:
-                raise ValueError(
-                    f"You've asked to drop data housed under the filepath "
-                    f"{self.linker.s3_output} from your "
-                    "s3 output bucket, which is not a folder created by "
-                    "Splink. If you really want to delete this data, you "
-                    "can do so by setting force_non_splink_table=True."
-                )
-
-        # validate that the ctas_query_info is for the given table
-        # we're interacting with
-        if (
-            self.linker.ctas_query_info[self.physical_name]["ctas_table"]
-            != self.physical_name
-        ):
-            raise ValueError(
-                f"The recorded metadata for {self.physical_name} that you're "
-                "attempting to delete does not match the recorded metadata on s3. "
-                "To prevent any tables becoming corrupted on s3, this run will be "
-                "terminated. Please retry the link/dedupe job and report the issue "
-                "if this error persists."
-            )
-
-    def as_pandas_dataframe(self, limit=None):
-        sql = f"""
-        select *
-        from {self.physical_name}
-        """
-        if limit:
-            sql += f" limit {limit}"
-
-        out_df = wr.athena.read_sql_query(
-            sql=sql,
-            database=self.linker.output_schema,
-            s3_output=self.linker.s3_output,
-            keep_files=False,
-            ctas_approach=True,
-            use_threads=True,
-            boto3_session=self.linker.boto3_session,
-        )
-        return out_df
-
-    def as_record_dict(self, limit=None):
-        out_df = self.as_pandas_dataframe(limit)
-        out_df = out_df.fillna(np.nan).replace([np.nan], [None])
-        return out_df.to_dict(orient="records")
-
-
-class AthenaLinker(Linker):
-    def __init__(
-        self,
-        input_table_or_tables,
-        boto3_session: boto3.session.Session,
-        output_database: str,
-        output_bucket: str,
-        settings_dict: dict | str = None,
-        input_table_aliases: str | list = None,
-        set_up_basic_logging=True,
-        output_filepath: str = "",
-        validate_settings: bool = True,
-    ):
-        """An athena backend for our main linker class. This funnels our generated SQL
-        through athena using awswrangler.
-        See linker.py for more information on the main linker class.
-        Attributes:
-            input_table_or_tables (Union[str, list]): Input data into the linkage model.
-                Either a single string (the name of a table in a database) for
-                deduplication jobs, or a list of strings  (the name of tables in a
-                database) for link_only or link_and_dedupe.
-            boto3_session (boto3.session.Session): A working boto3 session, which
-                should contain user credentials and region information.
-            output_database (str): The name of the database you wish to export the
-                results of the link job to. This should be created prior to performing
-                your link.
-            output_bucket (str): The name of the bucket and the filepath you wish to
-                store your outputs in on aws. The bucket should be created prior to
-                performing your link.
-            settings_dict (dict | Path, optional): A Splink settings dictionary, or
-                 a path to a json defining a settingss dictionary or pre-trained model.
-                  If not provided when the object is created, can later be added using
-                `linker.load_settings()` or `linker.load_model()` Defaults to None.
-            input_table_aliases: Aliases/custom names for your input tables, if
-                a pandas df or a list of dfs are used as inputs. None by default, which
-                saves your tables under a custom name: '__splink__input_table_{n}';
-                where n is the list index.
-            set_up_basic_logging (bool, optional): If true, sets ups up basic logging
-                so that Splink sends messages at INFO level to stdout. Defaults to True.
-            output_filepath (str, optional): Inside of your selected output bucket,
-                where to write output files to.
-                Defaults to "splink_warehouse/{unique_id}".
-            validate_settings (bool, optional): When True, check your settings
-                dictionary for any potential errors that may cause splink to fail.
-        Examples:
-            ```py
-            # Creating a database in athena and writing to it
-            import awswrangler as wr
-            wr.catalog.create_database("splink_awswrangler_test", exist_ok=True)
-            >>>
-            from splink.athena.linker import AthenaLinker
-            import boto3
-            # Create a session - please see the boto3 documentation for more info
-            my_session = boto3.Session(region_name="eu-west-1")
-            >>>
-            linker = AthenaLinker(
-                settings_dict=settings_dict,
-                input_table_or_tables="synthetic_data_all",
-                boto3_session=my_session,
-                output_bucket="alpha-splink-db-testing",
-                output_database="splink_awswrangler_test",
-            )
-            ```
-            ```py
-            # Creating a secondary database and use data on and existing db
-            import awswrangler as wr
-            wr.catalog.create_database("splink_awswrangler_test2", exist_ok=True)
-            >>>
-            from splink.athena.linker import AthenaLinker
-            import boto3
-            my_session = boto3.Session(region_name="eu-west-1")
-            >>>
-            # To read and write from separate databases, specify your secondary
-            # database as the output and enter your primary database as a schema
-            # for your input table(s)
-            linker = AthenaLinker(
-                settings_dict=settings_dict,
-                input_table_or_tables="splink_awswrangler_test.synthetic_data_all",
-                boto3_session=my_session,
-                output_bucket="alpha-splink-db-testing",
-                output_database="splink_awswrangler_test2",
-            )
-            ```
-        """
-
-        if not type(boto3_session) == boto3.session.Session:
-            raise ValueError("Please enter a valid boto3 session object.")
-
-        self._sql_dialect_ = "presto"
-
-        _verify_athena_inputs(output_database, output_bucket, boto3_session)
-        self.boto3_session = boto3_session
-        self.output_schema = output_database
-        self.output_bucket = output_bucket
-
-        # If the default folder is blank, name it `splink_warehouse`
-        if output_filepath:
-            self.output_filepath = output_filepath
-        else:
-            self.output_filepath = "splink_warehouse"
-
-        # This query info dictionary is used to circumvent the need to run
-        # `wr.catalog.get_table_location` every time we want to delete
-        # the backing data from s3.
-        self.ctas_query_info = {}
-
-        # If user has provided pandas dataframes, need to register
-        # them with the database, using user-provided aliases
-        # if provided or a created alias if not
-        input_tables = ensure_is_list(input_table_or_tables)
-
-        input_aliases = self._ensure_aliases_populated_and_is_list(
-            input_table_or_tables, input_table_aliases
-        )
-        accepted_df_dtypes = pd.DataFrame
-
-        # Run a quick check against our inputs to check if they
-        # exist in the database
-        for table in input_tables:
-            if not isinstance(table, accepted_df_dtypes):
-                db, tb = self.get_schema_info(table)
-                self.check_table_exists(db, tb)
-
-        super().__init__(
-            input_tables,
-            settings_dict,
-            accepted_df_dtypes,
-            set_up_basic_logging,
-            input_table_aliases=input_aliases,
-            validate_settings=validate_settings,
-        )
-
-    def _table_to_splink_dataframe(self, templated_name, physical_name):
-        return AthenaDataFrame(templated_name, physical_name, self)
-
-    def change_output_filepath(self, new_filepath):
-        self.output_filepath = new_filepath
-
-    def get_schema_info(self, input_table):
-        t = input_table.split(".")
-        return t if len(t) > 1 else [self.output_schema, input_table]
-
-    @property
-    def s3_output(self):
-        out_path = os.path.join(
-            "s3://",
-            self.output_bucket,
-            self.output_filepath,
-            self._cache_uid,  # added in the super() step
-        )
-        if out_path[-1] != "/":
-            out_path += "/"
-
-        return out_path
-
-    def check_table_exists(self, db, tb):
-        # A quick function to check if a table exists
-        # and spit out a warning if it is not found.
-        table_exists = wr.catalog.does_table_exist(
-            database=db,
-            table=tb,
-            boto3_session=self.boto3_session,
-        )
-        if not table_exists:
-            raise wr.exceptions.InvalidTable(
-                f"Table '{tb}' was not found within your selected "
-                f"database '{db}'. Please verify your input table "
-                "exists."
-            )
-
-    def register_data_on_s3(self, table, alias):
-        out_loc = f"{self.s3_output}{alias}"
-
-        wr.s3.to_parquet(
-            df=table,
-            path=out_loc,
-            dataset=True,
-            mode="overwrite",
-            database=self.output_schema,
-            table=alias,
-            boto3_session=self.boto3_session,
-            compression="snappy",
-            use_threads=True,
-        )
-        # Construct the ctas metadata that we require
-        ctas_metadata = {
-            "ctas_database": self.output_schema,
-            "ctas_table": alias,
-        }
-        self.ctas_query_info.update({alias: ctas_metadata})
-
-    def __sql_to_splink_dataframe(self, sql, templated_name, physical_name):
-        self.delete_table_from_database(physical_name)
-        sql = sqlglot_transform_sql(sql, cast_concat_as_varchar, dialect="presto")
-        sql = sql.replace("FLOAT", "double").replace("float", "double")
-
-        logger.debug(execute_sql_logging_message_info(templated_name, physical_name))
-        logger.log(5, log_sql(sql))
-
-        # create our table on athena and extract the metadata information
-        query_metadata = self.create_table(sql, physical_name=physical_name)
-        # append our metadata locations
-        query_metadata = self._extract_ctas_metadata(query_metadata)
-        self.ctas_query_info.update({physical_name: query_metadata})
-
-        output_obj = self._table_to_splink_dataframe(templated_name, physical_name)
-        return output_obj
-
-    def register_table(self, input, table_name, overwrite=False):
-        # If the user has provided a table name, return it as a SplinkDataframe
-        if isinstance(input, str):
-            return self._table_to_splink_dataframe(table_name, input)
-
-        # Check if table name is already in use
-        exists = self._table_exists_in_database(table_name)
-        if exists:
-            if not overwrite:
-                raise ValueError(
-                    f"Table '{table_name}' already exists in database. "
-                    "Please use the 'overwrite' argument if you wish to overwrite"
-                )
-            else:
-                self.delete_table_from_database(table_name)
-
-        self._table_registration(input, table_name)
-        return self._table_to_splink_dataframe(table_name, table_name)
-
-    def _table_registration(self, input, table_name):
-        if isinstance(input, dict):
-            input = pd.DataFrame(input)
-        elif isinstance(input, list):
-            input = pd.DataFrame.from_records(input)
-
-        # Errors if an invalid data type is passed
-        self.register_data_on_s3(input, table_name)
-
-    def _random_sample_sql(
-        self, proportion, sample_size, seed=None, table=None, unique_id=None
-    ):
-        if proportion == 1.0:
-            return ""
-        percent = proportion * 100
-        return f" TABLESAMPLE BERNOULLI ({percent})"
-
-    @property
-    def _infinity_expression(self):
-        return "infinity()"
-
-    def _table_exists_in_database(self, table_name):
-        return wr.catalog.does_table_exist(
-            database=self.output_schema,
-            table=table_name,
-            boto3_session=self.boto3_session,
-        )
-
-    def create_table(self, sql, physical_name):
-        database = self.output_schema
-        ctas_metadata = wr.athena.create_ctas_table(
-            sql=sql,
-            database=database,
-            ctas_table=physical_name,
-            storage_format="parquet",
-            write_compression="snappy",
-            boto3_session=self.boto3_session,
-            s3_output=self.s3_output,
-            wait=True,
-        )
-        return ctas_metadata
-
-    def _drop_table_from_database_if_exists(self, table):
-        return wr.catalog.delete_table_if_exists(
-            database=self.output_schema, table=table, boto3_session=self.boto3_session
-        )
-
-    def _delete_table_from_s3(self, physical_name):
-        path = f"{self.s3_output}{physical_name}/"
-        # delete our folder
-        wr.s3.delete_objects(
-            path=path,
-            use_threads=True,
-            boto3_session=self.boto3_session,
-        )
-
-        metadata = self.ctas_query_info[physical_name]
-        if "output_location" in metadata:
-            metadata_urls = [
-                # metadata output location
-                f"{metadata['output_location']}.metadata",
-                # manifest location
-                metadata["manifest_location"],
-            ]
-            # delete our metadata
-            wr.s3.delete_objects(
-                path=metadata_urls,
-                use_threads=True,
-                boto3_session=self.boto3_session,
-            )
-
-        self.ctas_query_info.pop(physical_name)
-
-    def delete_table_from_database(self, name):
-        if name in self.ctas_query_info:
-            # Use ctas metadata to delete backing data
-            self._delete_table_from_s3(name)
-        else:
-            # If the location we want to write to already exists,
-            # clean this before continuing.
-            loc = f"{self.s3_output}{name}"
-            folder_exists = wr.s3.list_directories(
-                loc,
-                boto3_session=self.boto3_session,
-            )
-            if folder_exists:
-                # This will only delete objects we are required to delete
-                wr.s3.delete_objects(
-                    path=loc,
-                    use_threads=True,
-                    boto3_session=self.boto3_session,
-                )
-
-        self._drop_table_from_database_if_exists(name)
-
-    def _extract_ctas_metadata(self, ctas_metadata):
-        query_meta = ctas_metadata.pop("ctas_query_metadata")
-        out_locs = {
-            "output_location": query_meta.output_location,
-            "manifest_location": query_meta.manifest_location,
-        }
-        ctas_metadata.update(out_locs)
-        return ctas_metadata
-
-    def drop_all_tables_created_by_splink(
-        self,
-        delete_s3_folders=True,
-        tables_to_exclude: list[Union[SplinkDataFrame, str]] = [],
-    ):
-        """Run a cleanup process for the tables created by splink and
-        currently contained in your output database.
-        Only those tables currently contained within your database
-        will be permanently deleted. Anything existing on s3 that
-        isn't connected to your database will not be removed.
-        Attributes:
-            delete_s3_folders (bool, optional): Whether to delete the
-                backing data contained on s3. If False, the tables created
-                by splink will be removed from your database, but the parquet
-                outputs will remain on s3. Defaults to True.
-            tables_to_exclude (list[SplinkDataFrame | str], optional): A list
-                of input tables you wish to add to an ignore list. These
-                will not be removed during garbage collection.
-        """
-        # Run cleanup on the cache before checking the db
-        self.drop_tables_in_current_splink_run(
-            delete_s3_folders,
-            tables_to_exclude,
-        )
-        _garbage_collection(
-            self.output_schema,
-            self.boto3_session,
-            delete_s3_folders,
-            tables_to_exclude,
-        )
-
-    def drop_splink_tables_from_database(
-        self,
-        database_name: str,
-        delete_s3_folders: bool = True,
-        tables_to_exclude: list[Union[SplinkDataFrame, str]] = [],
-    ):
-        """Run a cleanup process for the tables created by splink
-        in a specified database.
-        Only those tables currently contained within your database
-        will be permanently deleted. Anything existing on s3 that
-        isn't connected to your database will not be removed.
-        Attributes:
-            database_name (str): The name of the database to delete splink tables from.
-            delete_s3_folders (bool, optional): Whether to delete the
-                backing data contained on s3. If False, the tables created
-                by splink will be removed from your database, but the parquet
-                outputs will remain on s3. Defaults to True.
-            tables_to_exclude (list[SplinkDataFrame | str], optional): A list
-                of input tables you wish to add to an ignore list. These
-                will not be removed during garbage collection.
-        """
-        _garbage_collection(
-            database_name,
-            self.boto3_session,
-            delete_s3_folders,
-            tables_to_exclude,
-        )
-
-    def drop_tables_in_current_splink_run(
-        self,
-        delete_s3_folders: bool = True,
-        tables_to_exclude: list[Union[SplinkDataFrame, str]] = [],
-    ):
-        """Run a cleanup process for the tables created
-        by the current splink linker.
-        This leaves tables from previous runs untouched.
-        Only those tables currently contained within your database
-        will be permanently deleted. Anything existing on s3 that
-        isn't connected to your database will not be removed.
-        Attributes:
-            delete_s3_folders (bool, optional): Whether to delete the
-                backing data contained on s3. If False, the tables created
-                by splink will be removed from your database, but the parquet
-                outputs will remain on s3. Defaults to True.
-            tables_to_exclude (list[SplinkDataFrame | str], optional): A list
-                of input tables you wish to add to an ignore list. These
-                will not be removed during garbage collection.
-        """
-
-        tables_to_exclude = ensure_is_list(tables_to_exclude)
-        tables_to_exclude = {
-            df.physical_name if isinstance(df, SplinkDataFrame) else df
-            for df in tables_to_exclude
-        }
-
-        # Exclude tables that the user doesn't want to delete
-        cached_tables = self._intermediate_table_cache
-
-        # Loop through our cached tables and delete all those not in our exclusion
-        # list.
-        for splink_df in list(cached_tables.values()):
-            if (splink_df.physical_name not in tables_to_exclude) and (
-                splink_df.templated_name not in tables_to_exclude
-            ):
-                splink_df.drop_table_from_database_and_remove_from_cache(
-                    force_non_splink_table=False, delete_s3_data=delete_s3_folders
-                )
-            # As our cache contains duplicate term frequency tables and AWSwrangler
-            # run deletions asynchronously, add any previously seen tables to the
-            # list of tables to exclude from deletion.
-            # This prevents attempts to delete a table that has already been purged.
-            tables_to_exclude.add(splink_df.physical_name)
+# ruff: noqa: E501
+# ignore line-too-long while commented out
+# from __future__ import annotations
+
+# import logging
+# import os
+# from typing import Union
+
+# import awswrangler as wr
+# import boto3
+# import numpy as np
+# import pandas as pd
+
+# from ..input_column import InputColumn
+# from ..linker import Linker
+# from ..logging_messages import execute_sql_logging_message_info, log_sql
+# from ..misc import ensure_is_list
+# from ..splink_dataframe import SplinkDataFrame
+# from ..sql_transform import sqlglot_transform_sql
+# from .athena_helpers.athena_transforms import cast_concat_as_varchar
+# from .athena_helpers.athena_utils import (
+#     _garbage_collection,
+#     _verify_athena_inputs,
+# )
+
+# logger = logging.getLogger(__name__)
+
+
+# class AthenaDataFrame(SplinkDataFrame):
+#     linker: AthenaLinker
+
+#     @property
+#     def columns(self):
+#         db, tb = self.linker.get_schema_info(self.physical_name)
+#         d = wr.catalog.get_table_types(
+#             database=db,
+#             table=tb,
+#             boto3_session=self.linker.boto3_session,
+#         )
+
+#         cols = list(d.keys())
+#         return [InputColumn(c, sql_dialect="presto") for c in cols]
+
+#     def validate(self):
+#         pass
+
+#     def _drop_table_from_database(
+#         self, force_non_splink_table=False, delete_s3_data=True
+#     ):
+#         # Check folder and table set for deletion
+#         self._check_drop_folder_created_by_splink(force_non_splink_table)
+#         self._check_drop_table_created_by_splink(force_non_splink_table)
+
+#         # Delete the table from s3 and your database
+#         table_deleted = self.linker._drop_table_from_database_if_exists(
+#             self.physical_name
+#         )
+#         if delete_s3_data and table_deleted:
+#             self.linker._delete_table_from_s3(self.physical_name)
+
+#     def drop_table_from_database_and_remove_from_cache(
+#         self,
+#         force_non_splink_table=False,
+#         delete_s3_data=True,
+#     ):
+#         self._drop_table_from_database(
+#             force_non_splink_table=force_non_splink_table, delete_s3_data=delete_s3_data
+#         )
+#         self.linker._remove_splinkdataframe_from_cache(self)
+
+#     def _check_drop_folder_created_by_splink(self, force_non_splink_table=False):
+#         filepath = self.linker.s3_output
+#         filename = self.physical_name
+#         # Validate that the folder is a splink generated folder...
+#         files = wr.s3.list_objects(
+#             path=os.path.join(filepath, filename),
+#             boto3_session=self.linker.boto3_session,
+#             ignore_empty=True,
+#         )
+
+#         if len(files) == 0:
+#             if not force_non_splink_table:
+#                 raise ValueError(
+#                     f"You've asked to drop data housed under the filepath "
+#                     f"{self.linker.s3_output} from your "
+#                     "s3 output bucket, which is not a folder created by "
+#                     "Splink. If you really want to delete this data, you "
+#                     "can do so by setting force_non_splink_table=True."
+#                 )
+
+#         # validate that the ctas_query_info is for the given table
+#         # we're interacting with
+#         if (
+#             self.linker.ctas_query_info[self.physical_name]["ctas_table"]
+#             != self.physical_name
+#         ):
+#             raise ValueError(
+#                 f"The recorded metadata for {self.physical_name} that you're "
+#                 "attempting to delete does not match the recorded metadata on s3. "
+#                 "To prevent any tables becoming corrupted on s3, this run will be "
+#                 "terminated. Please retry the link/dedupe job and report the issue "
+#                 "if this error persists."
+#             )
+
+#     def as_pandas_dataframe(self, limit=None):
+#         sql = f"""
+#         select *
+#         from {self.physical_name}
+#         """
+#         if limit:
+#             sql += f" limit {limit}"
+
+#         out_df = wr.athena.read_sql_query(
+#             sql=sql,
+#             database=self.linker.output_schema,
+#             s3_output=self.linker.s3_output,
+#             keep_files=False,
+#             ctas_approach=True,
+#             use_threads=True,
+#             boto3_session=self.linker.boto3_session,
+#         )
+#         return out_df
+
+#     def as_record_dict(self, limit=None):
+#         out_df = self.as_pandas_dataframe(limit)
+#         out_df = out_df.fillna(np.nan).replace([np.nan], [None])
+#         return out_df.to_dict(orient="records")
+
+
+# class AthenaLinker(Linker):
+#     def __init__(
+#         self,
+#         input_table_or_tables,
+#         boto3_session: boto3.session.Session,
+#         output_database: str,
+#         output_bucket: str,
+#         settings_dict: dict | str = None,
+#         input_table_aliases: str | list = None,
+#         set_up_basic_logging=True,
+#         output_filepath: str = "",
+#         validate_settings: bool = True,
+#     ):
+#         """An athena backend for our main linker class. This funnels our generated SQL
+#         through athena using awswrangler.
+#         See linker.py for more information on the main linker class.
+#         Attributes:
+#             input_table_or_tables (Union[str, list]): Input data into the linkage model.
+#                 Either a single string (the name of a table in a database) for
+#                 deduplication jobs, or a list of strings  (the name of tables in a
+#                 database) for link_only or link_and_dedupe.
+#             boto3_session (boto3.session.Session): A working boto3 session, which
+#                 should contain user credentials and region information.
+#             output_database (str): The name of the database you wish to export the
+#                 results of the link job to. This should be created prior to performing
+#                 your link.
+#             output_bucket (str): The name of the bucket and the filepath you wish to
+#                 store your outputs in on aws. The bucket should be created prior to
+#                 performing your link.
+#             settings_dict (dict | Path, optional): A Splink settings dictionary, or
+#                  a path to a json defining a settingss dictionary or pre-trained model.
+#                   If not provided when the object is created, can later be added using
+#                 `linker.load_settings()` or `linker.load_model()` Defaults to None.
+#             input_table_aliases: Aliases/custom names for your input tables, if
+#                 a pandas df or a list of dfs are used as inputs. None by default, which
+#                 saves your tables under a custom name: '__splink__input_table_{n}';
+#                 where n is the list index.
+#             set_up_basic_logging (bool, optional): If true, sets ups up basic logging
+#                 so that Splink sends messages at INFO level to stdout. Defaults to True.
+#             output_filepath (str, optional): Inside of your selected output bucket,
+#                 where to write output files to.
+#                 Defaults to "splink_warehouse/{unique_id}".
+#             validate_settings (bool, optional): When True, check your settings
+#                 dictionary for any potential errors that may cause splink to fail.
+#         Examples:
+#             ```py
+#             # Creating a database in athena and writing to it
+#             import awswrangler as wr
+#             wr.catalog.create_database("splink_awswrangler_test", exist_ok=True)
+#             >>>
+#             from splink.athena.linker import AthenaLinker
+#             import boto3
+#             # Create a session - please see the boto3 documentation for more info
+#             my_session = boto3.Session(region_name="eu-west-1")
+#             >>>
+#             linker = AthenaLinker(
+#                 settings_dict=settings_dict,
+#                 input_table_or_tables="synthetic_data_all",
+#                 boto3_session=my_session,
+#                 output_bucket="alpha-splink-db-testing",
+#                 output_database="splink_awswrangler_test",
+#             )
+#             ```
+#             ```py
+#             # Creating a secondary database and use data on and existing db
+#             import awswrangler as wr
+#             wr.catalog.create_database("splink_awswrangler_test2", exist_ok=True)
+#             >>>
+#             from splink.athena.linker import AthenaLinker
+#             import boto3
+#             my_session = boto3.Session(region_name="eu-west-1")
+#             >>>
+#             # To read and write from separate databases, specify your secondary
+#             # database as the output and enter your primary database as a schema
+#             # for your input table(s)
+#             linker = AthenaLinker(
+#                 settings_dict=settings_dict,
+#                 input_table_or_tables="splink_awswrangler_test.synthetic_data_all",
+#                 boto3_session=my_session,
+#                 output_bucket="alpha-splink-db-testing",
+#                 output_database="splink_awswrangler_test2",
+#             )
+#             ```
+#         """
+
+#         if not type(boto3_session) == boto3.session.Session:
+#             raise ValueError("Please enter a valid boto3 session object.")
+
+#         self._sql_dialect_ = "presto"
+
+#         _verify_athena_inputs(output_database, output_bucket, boto3_session)
+#         self.boto3_session = boto3_session
+#         self.output_schema = output_database
+#         self.output_bucket = output_bucket
+
+#         # If the default folder is blank, name it `splink_warehouse`
+#         if output_filepath:
+#             self.output_filepath = output_filepath
+#         else:
+#             self.output_filepath = "splink_warehouse"
+
+#         # This query info dictionary is used to circumvent the need to run
+#         # `wr.catalog.get_table_location` every time we want to delete
+#         # the backing data from s3.
+#         self.ctas_query_info = {}
+
+#         # If user has provided pandas dataframes, need to register
+#         # them with the database, using user-provided aliases
+#         # if provided or a created alias if not
+#         input_tables = ensure_is_list(input_table_or_tables)
+
+#         input_aliases = self._ensure_aliases_populated_and_is_list(
+#             input_table_or_tables, input_table_aliases
+#         )
+#         accepted_df_dtypes = pd.DataFrame
+
+#         # Run a quick check against our inputs to check if they
+#         # exist in the database
+#         for table in input_tables:
+#             if not isinstance(table, accepted_df_dtypes):
+#                 db, tb = self.get_schema_info(table)
+#                 self.check_table_exists(db, tb)
+
+#         super().__init__(
+#             input_tables,
+#             settings_dict,
+#             accepted_df_dtypes,
+#             set_up_basic_logging,
+#             input_table_aliases=input_aliases,
+#             validate_settings=validate_settings,
+#         )
+
+#     def _table_to_splink_dataframe(self, templated_name, physical_name):
+#         return AthenaDataFrame(templated_name, physical_name, self)
+
+#     def change_output_filepath(self, new_filepath):
+#         self.output_filepath = new_filepath
+
+#     def get_schema_info(self, input_table):
+#         t = input_table.split(".")
+#         return t if len(t) > 1 else [self.output_schema, input_table]
+
+#     @property
+#     def s3_output(self):
+#         out_path = os.path.join(
+#             "s3://",
+#             self.output_bucket,
+#             self.output_filepath,
+#             self._cache_uid,  # added in the super() step
+#         )
+#         if out_path[-1] != "/":
+#             out_path += "/"
+
+#         return out_path
+
+#     def check_table_exists(self, db, tb):
+#         # A quick function to check if a table exists
+#         # and spit out a warning if it is not found.
+#         table_exists = wr.catalog.does_table_exist(
+#             database=db,
+#             table=tb,
+#             boto3_session=self.boto3_session,
+#         )
+#         if not table_exists:
+#             raise wr.exceptions.InvalidTable(
+#                 f"Table '{tb}' was not found within your selected "
+#                 f"database '{db}'. Please verify your input table "
+#                 "exists."
+#             )
+
+#     def register_data_on_s3(self, table, alias):
+#         out_loc = f"{self.s3_output}{alias}"
+
+#         wr.s3.to_parquet(
+#             df=table,
+#             path=out_loc,
+#             dataset=True,
+#             mode="overwrite",
+#             database=self.output_schema,
+#             table=alias,
+#             boto3_session=self.boto3_session,
+#             compression="snappy",
+#             use_threads=True,
+#         )
+#         # Construct the ctas metadata that we require
+#         ctas_metadata = {
+#             "ctas_database": self.output_schema,
+#             "ctas_table": alias,
+#         }
+#         self.ctas_query_info.update({alias: ctas_metadata})
+
+#     def __sql_to_splink_dataframe(self, sql, templated_name, physical_name):
+#         self.delete_table_from_database(physical_name)
+#         sql = sqlglot_transform_sql(sql, cast_concat_as_varchar, dialect="presto")
+#         sql = sql.replace("FLOAT", "double").replace("float", "double")
+
+#         logger.debug(execute_sql_logging_message_info(templated_name, physical_name))
+#         logger.log(5, log_sql(sql))
+
+#         # create our table on athena and extract the metadata information
+#         query_metadata = self.create_table(sql, physical_name=physical_name)
+#         # append our metadata locations
+#         query_metadata = self._extract_ctas_metadata(query_metadata)
+#         self.ctas_query_info.update({physical_name: query_metadata})
+
+#         output_obj = self._table_to_splink_dataframe(templated_name, physical_name)
+#         return output_obj
+
+#     def register_table(self, input, table_name, overwrite=False):
+#         # If the user has provided a table name, return it as a SplinkDataframe
+#         if isinstance(input, str):
+#             return self._table_to_splink_dataframe(table_name, input)
+
+#         # Check if table name is already in use
+#         exists = self._table_exists_in_database(table_name)
+#         if exists:
+#             if not overwrite:
+#                 raise ValueError(
+#                     f"Table '{table_name}' already exists in database. "
+#                     "Please use the 'overwrite' argument if you wish to overwrite"
+#                 )
+#             else:
+#                 self.delete_table_from_database(table_name)
+
+#         self._table_registration(input, table_name)
+#         return self._table_to_splink_dataframe(table_name, table_name)
+
+#     def _table_registration(self, input, table_name):
+#         if isinstance(input, dict):
+#             input = pd.DataFrame(input)
+#         elif isinstance(input, list):
+#             input = pd.DataFrame.from_records(input)
+
+#         # Errors if an invalid data type is passed
+#         self.register_data_on_s3(input, table_name)
+
+#     def _random_sample_sql(
+#         self, proportion, sample_size, seed=None, table=None, unique_id=None
+#     ):
+#         if proportion == 1.0:
+#             return ""
+#         percent = proportion * 100
+#         return f" TABLESAMPLE BERNOULLI ({percent})"
+
+#     @property
+#     def _infinity_expression(self):
+#         return "infinity()"
+
+#     def _table_exists_in_database(self, table_name):
+#         return wr.catalog.does_table_exist(
+#             database=self.output_schema,
+#             table=table_name,
+#             boto3_session=self.boto3_session,
+#         )
+
+#     def create_table(self, sql, physical_name):
+#         database = self.output_schema
+#         ctas_metadata = wr.athena.create_ctas_table(
+#             sql=sql,
+#             database=database,
+#             ctas_table=physical_name,
+#             storage_format="parquet",
+#             write_compression="snappy",
+#             boto3_session=self.boto3_session,
+#             s3_output=self.s3_output,
+#             wait=True,
+#         )
+#         return ctas_metadata
+
+#     def _drop_table_from_database_if_exists(self, table):
+#         return wr.catalog.delete_table_if_exists(
+#             database=self.output_schema, table=table, boto3_session=self.boto3_session
+#         )
+
+#     def _delete_table_from_s3(self, physical_name):
+#         path = f"{self.s3_output}{physical_name}/"
+#         # delete our folder
+#         wr.s3.delete_objects(
+#             path=path,
+#             use_threads=True,
+#             boto3_session=self.boto3_session,
+#         )
+
+#         metadata = self.ctas_query_info[physical_name]
+#         if "output_location" in metadata:
+#             metadata_urls = [
+#                 # metadata output location
+#                 f"{metadata['output_location']}.metadata",
+#                 # manifest location
+#                 metadata["manifest_location"],
+#             ]
+#             # delete our metadata
+#             wr.s3.delete_objects(
+#                 path=metadata_urls,
+#                 use_threads=True,
+#                 boto3_session=self.boto3_session,
+#             )
+
+#         self.ctas_query_info.pop(physical_name)
+
+#     def delete_table_from_database(self, name):
+#         if name in self.ctas_query_info:
+#             # Use ctas metadata to delete backing data
+#             self._delete_table_from_s3(name)
+#         else:
+#             # If the location we want to write to already exists,
+#             # clean this before continuing.
+#             loc = f"{self.s3_output}{name}"
+#             folder_exists = wr.s3.list_directories(
+#                 loc,
+#                 boto3_session=self.boto3_session,
+#             )
+#             if folder_exists:
+#                 # This will only delete objects we are required to delete
+#                 wr.s3.delete_objects(
+#                     path=loc,
+#                     use_threads=True,
+#                     boto3_session=self.boto3_session,
+#                 )
+
+#         self._drop_table_from_database_if_exists(name)
+
+#     def _extract_ctas_metadata(self, ctas_metadata):
+#         query_meta = ctas_metadata.pop("ctas_query_metadata")
+#         out_locs = {
+#             "output_location": query_meta.output_location,
+#             "manifest_location": query_meta.manifest_location,
+#         }
+#         ctas_metadata.update(out_locs)
+#         return ctas_metadata
+
+#     def drop_all_tables_created_by_splink(
+#         self,
+#         delete_s3_folders=True,
+#         tables_to_exclude: list[Union[SplinkDataFrame, str]] = [],
+#     ):
+#         """Run a cleanup process for the tables created by splink and
+#         currently contained in your output database.
+#         Only those tables currently contained within your database
+#         will be permanently deleted. Anything existing on s3 that
+#         isn't connected to your database will not be removed.
+#         Attributes:
+#             delete_s3_folders (bool, optional): Whether to delete the
+#                 backing data contained on s3. If False, the tables created
+#                 by splink will be removed from your database, but the parquet
+#                 outputs will remain on s3. Defaults to True.
+#             tables_to_exclude (list[SplinkDataFrame | str], optional): A list
+#                 of input tables you wish to add to an ignore list. These
+#                 will not be removed during garbage collection.
+#         """
+#         # Run cleanup on the cache before checking the db
+#         self.drop_tables_in_current_splink_run(
+#             delete_s3_folders,
+#             tables_to_exclude,
+#         )
+#         _garbage_collection(
+#             self.output_schema,
+#             self.boto3_session,
+#             delete_s3_folders,
+#             tables_to_exclude,
+#         )
+
+#     def drop_splink_tables_from_database(
+#         self,
+#         database_name: str,
+#         delete_s3_folders: bool = True,
+#         tables_to_exclude: list[Union[SplinkDataFrame, str]] = [],
+#     ):
+#         """Run a cleanup process for the tables created by splink
+#         in a specified database.
+#         Only those tables currently contained within your database
+#         will be permanently deleted. Anything existing on s3 that
+#         isn't connected to your database will not be removed.
+#         Attributes:
+#             database_name (str): The name of the database to delete splink tables from.
+#             delete_s3_folders (bool, optional): Whether to delete the
+#                 backing data contained on s3. If False, the tables created
+#                 by splink will be removed from your database, but the parquet
+#                 outputs will remain on s3. Defaults to True.
+#             tables_to_exclude (list[SplinkDataFrame | str], optional): A list
+#                 of input tables you wish to add to an ignore list. These
+#                 will not be removed during garbage collection.
+#         """
+#         _garbage_collection(
+#             database_name,
+#             self.boto3_session,
+#             delete_s3_folders,
+#             tables_to_exclude,
+#         )
+
+#     def drop_tables_in_current_splink_run(
+#         self,
+#         delete_s3_folders: bool = True,
+#         tables_to_exclude: list[Union[SplinkDataFrame, str]] = [],
+#     ):
+#         """Run a cleanup process for the tables created
+#         by the current splink linker.
+#         This leaves tables from previous runs untouched.
+#         Only those tables currently contained within your database
+#         will be permanently deleted. Anything existing on s3 that
+#         isn't connected to your database will not be removed.
+#         Attributes:
+#             delete_s3_folders (bool, optional): Whether to delete the
+#                 backing data contained on s3. If False, the tables created
+#                 by splink will be removed from your database, but the parquet
+#                 outputs will remain on s3. Defaults to True.
+#             tables_to_exclude (list[SplinkDataFrame | str], optional): A list
+#                 of input tables you wish to add to an ignore list. These
+#                 will not be removed during garbage collection.
+#         """
+
+#         tables_to_exclude = ensure_is_list(tables_to_exclude)
+#         tables_to_exclude = {
+#             df.physical_name if isinstance(df, SplinkDataFrame) else df
+#             for df in tables_to_exclude
+#         }
+
+#         # Exclude tables that the user doesn't want to delete
+#         cached_tables = self._intermediate_table_cache
+
+#         # Loop through our cached tables and delete all those not in our exclusion
+#         # list.
+#         for splink_df in list(cached_tables.values()):
+#             if (splink_df.physical_name not in tables_to_exclude) and (
+#                 splink_df.templated_name not in tables_to_exclude
+#             ):
+#                 splink_df.drop_table_from_database_and_remove_from_cache(
+#                     force_non_splink_table=False, delete_s3_data=delete_s3_folders
+#                 )
+#             # As our cache contains duplicate term frequency tables and AWSwrangler
+#             # run deletions asynchronously, add any previously seen tables to the
+#             # list of tables to exclude from deletion.
+#             # This prevents attempts to delete a table that has already been purged.
+#             tables_to_exclude.add(splink_df.physical_name)
```

### Comparing `splink-4.0.0.dev3/splink/block_from_labels.py` & `splink-4.0.0.dev4/splink/block_from_labels.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
     from .linker import Linker
 
 
 def block_from_labels(
-    linker: Linker, labels_table_name: str, include_clerical_match_score=False
-):
+    linker: Linker, labels_table_name: str, include_clerical_match_score: bool = False
+) -> list[dict[str, str]]:
     """Create pairwise record comparisons corresponding to the ID pairs in a labels
     table
 
     The table of labels should be in the following format, and should be registered
     with your database:
 
     |source_dataset_l|unique_id_l|source_dataset_r|unique_id_r|clerical_match_score|
@@ -35,20 +35,20 @@
     source_dataset_col = (
         linker._settings_obj.column_info_settings.source_dataset_column_name
     )
 
     sql = lower_id_to_left_hand_side(df, source_dataset_col, unique_id_col)
 
     sqls = []
-    sql = {
+    sql_info = {
         "sql": sql,
         "output_table_name": "__splink__labels_prepared_for_joining",
     }
 
-    sqls.append(sql)
+    sqls.append(sql_info)
 
     columns_to_select = linker._settings_obj._columns_to_select_for_blocking
     sql_select_expr = ", ".join(columns_to_select)
 
     if source_dataset_col:
         join_condition_l = f"""
         l.{source_dataset_col} = df_labels.{source_dataset_col}_l and
@@ -78,15 +78,15 @@
     __splink__labels_prepared_for_joining as df_labels
     inner join __splink__df_concat_with_tf as l
     on {join_condition_l}
     inner join __splink__df_concat_with_tf as r
     on {join_condition_r}
     """
 
-    sql = {
+    sql_info = {
         "sql": sql,
         "output_table_name": "__splink__df_blocked",
     }
 
-    sqls.append(sql)
+    sqls.append(sql_info)
 
     return sqls
```

### Comparing `splink-4.0.0.dev3/splink/blocking.py` & `splink-4.0.0.dev4/splink/blocking.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 from __future__ import annotations
 
 import logging
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, Any, List, Literal, Optional
 
 from sqlglot import parse_one
-from sqlglot.expressions import Column, Join
+from sqlglot.expressions import Column, Expression, Identifier, Join
 from sqlglot.optimizer.eliminate_joins import join_condition
+from sqlglot.optimizer.optimizer import optimize
 
+from .database_api import DatabaseAPISubClass
 from .exceptions import SplinkException
 from .input_column import InputColumn
 from .misc import ensure_is_list
+from .pipeline import CTEPipeline
 from .splink_dataframe import SplinkDataFrame
 from .unique_id_concat import _composite_unique_id_from_nodes_sql
+from .vertically_concatenate import vertically_concatenate_sql
 
 logger = logging.getLogger(__name__)
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
-    from .linker import Linker
+    from .settings import LinkTypeLiteralType
 
+user_input_link_type_options = Literal["link_only", "link_and_dedupe", "dedupe_only"]
 
-def blocking_rule_to_obj(br: BlockingRule | dict | str) -> BlockingRule:
+backend_link_type_options = Literal[
+    "link_only", "link_and_dedupe", "dedupe_only", "two_dataset_link_only", "self_link"
+]
+
+
+def blocking_rule_to_obj(br: BlockingRule | dict[str, Any] | str) -> BlockingRule:
     if isinstance(br, BlockingRule):
         return br
     elif isinstance(br, dict):
         blocking_rule = br.get("blocking_rule", None)
         if blocking_rule is None:
             raise ValueError("No blocking rule submitted...")
         sqlglot_dialect = br.get("sql_dialect", None)
@@ -51,14 +61,25 @@
         return BlockingRule(blocking_rule, sqlglot_dialect)
 
     else:
         br = BlockingRule(br)
         return br
 
 
+def combine_unique_id_input_columns(
+    source_dataset_input_column: Optional[InputColumn],
+    unique_id_input_column: InputColumn,
+) -> List[InputColumn]:
+    unique_id_input_columns: List[InputColumn] = []
+    if source_dataset_input_column:
+        unique_id_input_columns.append(source_dataset_input_column)
+    unique_id_input_columns.append(unique_id_input_column)
+    return unique_id_input_columns
+
+
 class BlockingRule:
     def __init__(
         self,
         blocking_rule_sql: str,
         sqlglot_dialect: str = None,
     ):
         if sqlglot_dialect:
@@ -81,58 +102,79 @@
     def match_key(self):
         return len(self.preceding_rules)
 
     def add_preceding_rules(self, rules):
         rules = ensure_is_list(rules)
         self.preceding_rules = rules
 
-    def exclude_pairs_generated_by_this_rule_sql(self, linker: Linker):
+    def exclude_pairs_generated_by_this_rule_sql(
+        self,
+        source_dataset_input_column: Optional[InputColumn],
+        unique_id_input_column: InputColumn,
+    ) -> str:
         """A SQL string specifying how to exclude the results
         of THIS blocking rule from subseqent blocking statements,
         so that subsequent statements do not produce duplicate pairs
         """
 
         # Note the coalesce function is important here - otherwise
         # you filter out any records with nulls in the previous rules
         # meaning these comparisons get lost
         return f"coalesce(({self.blocking_rule_sql}),false)"
 
-    def exclude_pairs_generated_by_all_preceding_rules_sql(self, linker: Linker):
+    def exclude_pairs_generated_by_all_preceding_rules_sql(
+        self,
+        source_dataset_input_column: Optional[InputColumn],
+        unique_id_input_column: InputColumn,
+    ) -> str:
         """A SQL string that excludes the results of ALL previous blocking rules from
         the pairwise comparisons generated.
         """
         if not self.preceding_rules:
             return ""
         or_clauses = [
-            br.exclude_pairs_generated_by_this_rule_sql(linker)
+            br.exclude_pairs_generated_by_this_rule_sql(
+                source_dataset_input_column,
+                unique_id_input_column,
+            )
             for br in self.preceding_rules
         ]
         previous_rules = " OR ".join(or_clauses)
         return f"AND NOT ({previous_rules})"
 
-    def create_blocked_pairs_sql(self, linker: Linker, where_condition, probability):
-        columns_to_select = linker._settings_obj._columns_to_select_for_blocking
-        sql_select_expr = ", ".join(columns_to_select)
-
+    def create_blocked_pairs_sql(
+        self,
+        *,
+        source_dataset_input_column: Optional[InputColumn],
+        unique_id_input_column: InputColumn,
+        input_tablename_l: str,
+        input_tablename_r: str,
+        where_condition: str,
+        probability: str,
+        sql_select_expr: str,
+    ) -> str:
         sql = f"""
             select
             {sql_select_expr}
             , '{self.match_key}' as match_key
             {probability}
-            from {linker._input_tablename_l} as l
-            inner join {linker._input_tablename_r} as r
+            from {input_tablename_l} as l
+            inner join {input_tablename_r} as r
             on
             ({self.blocking_rule_sql})
             {where_condition}
-            {self.exclude_pairs_generated_by_all_preceding_rules_sql(linker)}
+            {self.exclude_pairs_generated_by_all_preceding_rules_sql(
+                source_dataset_input_column,
+                unique_id_input_column)
+            }
             """
         return sql
 
     @property
-    def _parsed_join_condition(self):
+    def _parsed_join_condition(self) -> Join:
         br = self.blocking_rule_sql
         return parse_one("INNER JOIN r", into=Join).on(
             br, dialect=self.sqlglot_dialect
         )  # using sqlglot==11.4.1
 
     @property
     def _equi_join_conditions(self):
@@ -140,47 +182,53 @@
         Extract the equi join conditions from the blocking rule as a tuple:
         source_keys, join_keys
 
         Returns:
             list of tuples like [(name, name), (substr(name,1,2), substr(name,2,3))]
         """
 
-        def remove_table_prefix(tree):
+        def remove_table_prefix(tree: Expression) -> Expression:
             for c in tree.find_all(Column):
                 del c.args["table"]
             return tree
 
-        j = self._parsed_join_condition
+        j: Join = self._parsed_join_condition
 
         source_keys, join_keys, _ = join_condition(j)
 
-        keys = zip(source_keys, join_keys)
+        keys_zipped = zip(source_keys, join_keys)
 
         rmtp = remove_table_prefix
 
-        keys = [(rmtp(i), rmtp(j)) for (i, j) in keys]
+        keys_de_prefixed: list[tuple[Expression, Expression]] = [
+            (rmtp(i), rmtp(j)) for (i, j) in keys_zipped
+        ]
 
-        keys = [
+        keys_strings: list[tuple[str, str]] = [
             (i.sql(dialect=self.sqlglot_dialect), j.sql(self.sqlglot_dialect))
-            for (i, j) in keys
+            for (i, j) in keys_de_prefixed
         ]
 
-        return keys
+        return keys_strings
 
     @property
     def _filter_conditions(self):
         # A more accurate term might be "non-equi-join conditions"
         # or "complex join conditions", but to capture the idea these are
         # filters that have to be applied post-creation of the pairwise record
         # comparison i've opted to call it a filter
         j = self._parsed_join_condition
         _, _, filter_condition = join_condition(j)
         if not filter_condition:
             return ""
         else:
+            filter_condition = optimize(filter_condition)
+            for i in filter_condition.find_all(Identifier):
+                i.set("quoted", False)
+
             return filter_condition.sql(self.sqlglot_dialect)
 
     def as_dict(self):
         "The minimal representation of the blocking rule"
         output = {}
 
         output["blocking_rule"] = self.blocking_rule_sql
@@ -228,213 +276,272 @@
 
     def _as_completed_dict(self):
         return self.as_dict()
 
     def _salting_condition(self, salt):
         return f"AND ceiling(l.__splink_salt * {self.salting_partitions}) = {salt + 1}"
 
-    def create_blocked_pairs_sql(self, linker: Linker, where_condition, probability):
-        columns_to_select = linker._settings_obj._columns_to_select_for_blocking
-        sql_select_expr = ", ".join(columns_to_select)
-
+    def create_blocked_pairs_sql(
+        self,
+        *,
+        source_dataset_input_column: Optional[InputColumn],
+        unique_id_input_column: InputColumn,
+        input_tablename_l: str,
+        input_tablename_r: str,
+        where_condition: str,
+        probability: str,
+        sql_select_expr: str,
+    ) -> str:
         sqls = []
+        exclude_sql = self.exclude_pairs_generated_by_all_preceding_rules_sql(
+            source_dataset_input_column, unique_id_input_column
+        )
         for salt in range(self.salting_partitions):
             salt_condition = self._salting_condition(salt)
             sql = f"""
             select
             {sql_select_expr}
             , '{self.match_key}' as match_key
             {probability}
-            from {linker._input_tablename_l} as l
-            inner join {linker._input_tablename_r} as r
+            from {input_tablename_l} as l
+            inner join {input_tablename_r} as r
             on
             ({self.blocking_rule_sql} {salt_condition})
             {where_condition}
-            {self.exclude_pairs_generated_by_all_preceding_rules_sql(linker)}
+            {exclude_sql}
             """
 
             sqls.append(sql)
         return " UNION ALL ".join(sqls)
 
 
+def _explode_arrays_sql(db_api, tbl_name, columns_to_explode, other_columns_to_retain):
+    return db_api.sql_dialect.explode_arrays_sql(
+        tbl_name, columns_to_explode, other_columns_to_retain
+    )
+
+
 class ExplodingBlockingRule(BlockingRule):
     def __init__(
         self,
-        blocking_rule: BlockingRule | dict | str,
+        blocking_rule: BlockingRule | dict[str, Any] | str,
         sqlglot_dialect: str = None,
-        array_columns_to_explode: list = [],
+        array_columns_to_explode: list[str] = [],
     ):
         if isinstance(blocking_rule, BlockingRule):
             blocking_rule_sql = blocking_rule.blocking_rule_sql
         elif isinstance(blocking_rule, dict):
             blocking_rule_sql = blocking_rule["blocking_rule_sql"]
         else:
             blocking_rule_sql = blocking_rule
         super().__init__(blocking_rule_sql, sqlglot_dialect)
         self.array_columns_to_explode: List[str] = array_columns_to_explode
         self.exploded_id_pair_table: Optional[SplinkDataFrame] = None
 
-    def marginal_exploded_id_pairs_table_sql(self, linker: Linker, br: BlockingRule):
+    def marginal_exploded_id_pairs_table_sql(
+        self,
+        source_dataset_input_column: Optional[InputColumn],
+        unique_id_input_column: InputColumn,
+        br: BlockingRule,
+        link_type: "LinkTypeLiteralType",
+    ) -> str:
         """generates a table of the marginal id pairs from the exploded blocking rule
         i.e. pairs are only created that match this blocking rule and NOT any of
         the preceding blocking rules
         """
 
-        settings_obj = linker._settings_obj
-        unique_id_col = settings_obj.column_info_settings.unique_id_column_name
-        unique_id_input_columns = (
-            settings_obj.column_info_settings.unique_id_input_columns
+        unique_id_col = unique_id_input_column
+        unique_id_input_columns = combine_unique_id_input_columns(
+            source_dataset_input_column, unique_id_input_column
         )
 
-        link_type = settings_obj._link_type
-
-        if linker._two_dataset_link_only:
-            link_type = "two_dataset_link_only"
-
-        if linker._self_link_mode:
-            link_type = "self_link"
-
         where_condition = _sql_gen_where_condition(link_type, unique_id_input_columns)
 
         id_expr_l = _composite_unique_id_from_nodes_sql(unique_id_input_columns, "l")
         id_expr_r = _composite_unique_id_from_nodes_sql(unique_id_input_columns, "r")
 
         if link_type == "two_dataset_link_only":
             where_condition = (
                 where_condition + " and l.source_dataset < r.source_dataset"
             )
 
+        exclude_sql = self.exclude_pairs_generated_by_all_preceding_rules_sql(
+            source_dataset_input_column, unique_id_input_column
+        )
         sql = f"""
             select distinct
-                {id_expr_l} as {unique_id_col}_l,
-                {id_expr_r} as {unique_id_col}_r
-            from __splink__df_concat_with_tf_unnested as l
-            inner join __splink__df_concat_with_tf_unnested as r
+                {id_expr_l} as {unique_id_col.name_l},
+                {id_expr_r} as {unique_id_col.name_r}
+            from __splink__df_concat_unnested as l
+            inner join __splink__df_concat_unnested as r
             on ({br.blocking_rule_sql})
             {where_condition}
-            {self.exclude_pairs_generated_by_all_preceding_rules_sql(linker)}
+            {exclude_sql}
             """
 
         return sql
 
     def drop_materialised_id_pairs_dataframe(self):
-        self.exploded_id_pair_table.drop_table_from_database_and_remove_from_cache()
+        if self.exploded_id_pair_table is not None:
+            self.exploded_id_pair_table.drop_table_from_database_and_remove_from_cache()
         self.exploded_id_pair_table = None
 
-    def exclude_pairs_generated_by_this_rule_sql(self, linker: Linker):
+    def exclude_pairs_generated_by_this_rule_sql(
+        self,
+        source_dataset_input_column: Optional[InputColumn],
+        unique_id_input_column: InputColumn,
+    ) -> str:
         """A SQL string specifying how to exclude the results
         of THIS blocking rule from subseqent blocking statements,
         so that subsequent statements do not produce duplicate pairs
         """
 
-        unique_id_column = (
-            linker._settings_obj.column_info_settings.unique_id_column_name
-        )
-        unique_id_input_columns = (
-            linker._settings_obj.column_info_settings.unique_id_input_columns
+        unique_id_column = unique_id_input_column
+
+        unique_id_input_columns = combine_unique_id_input_columns(
+            source_dataset_input_column, unique_id_input_column
         )
+
         if (splink_df := self.exploded_id_pair_table) is None:
             raise SplinkException(
                 "Must use `materialise_exploded_id_table(linker)` "
                 "to set `exploded_id_pair_table` before calling "
                 "exclude_pairs_generated_by_this_rule_sql()."
             )
         ids_to_compare_sql = f"select * from {splink_df.physical_name}"
 
         id_expr_l = _composite_unique_id_from_nodes_sql(unique_id_input_columns, "l")
         id_expr_r = _composite_unique_id_from_nodes_sql(unique_id_input_columns, "r")
 
         return f"""EXISTS (
             select 1 from ({ids_to_compare_sql}) as ids_to_compare
             where (
-                {id_expr_l} = ids_to_compare.{unique_id_column}_l and
-                {id_expr_r} = ids_to_compare.{unique_id_column}_r
+                {id_expr_l} = ids_to_compare.{unique_id_column.name_l} and
+                {id_expr_r} = ids_to_compare.{unique_id_column.name_r}
             )
         )
         """
 
-    def create_blocked_pairs_sql(self, linker: Linker, where_condition, probability):
-        columns_to_select = linker._settings_obj._columns_to_select_for_blocking
-        sql_select_expr = ", ".join(columns_to_select)
-
+    def create_blocked_pairs_sql(
+        self,
+        *,
+        source_dataset_input_column: Optional[InputColumn],
+        unique_id_input_column: InputColumn,
+        input_tablename_l: str,
+        input_tablename_r: str,
+        where_condition: str,
+        probability: str,
+        sql_select_expr: str,
+    ) -> str:
         if self.exploded_id_pair_table is None:
             raise ValueError(
                 "Exploding blocking rules are not supported for the function you have"
                 " called."
             )
-        settings_obj = linker._settings_obj
-        unique_id_col = settings_obj.column_info_settings.unique_id_column_name
-        unique_id_input_columns = (
-            settings_obj.column_info_settings.unique_id_input_columns
+
+        unique_id_col = unique_id_input_column
+        unique_id_input_columns = combine_unique_id_input_columns(
+            source_dataset_input_column, unique_id_input_column
         )
+
         id_expr_l = _composite_unique_id_from_nodes_sql(unique_id_input_columns, "l")
         id_expr_r = _composite_unique_id_from_nodes_sql(unique_id_input_columns, "r")
 
         exploded_id_pair_table = self.exploded_id_pair_table
         sql = f"""
             select
                 {sql_select_expr},
                 '{self.match_key}' as match_key
                 {probability}
             from {exploded_id_pair_table.physical_name} as pairs
-            left join {linker._input_tablename_l} as l
-                on pairs.{unique_id_col}_l={id_expr_l}
-            left join {linker._input_tablename_r} as r
-                on pairs.{unique_id_col}_r={id_expr_r}
+            left join {input_tablename_l} as l
+                on pairs.{unique_id_col.name_l}={id_expr_l}
+            left join {input_tablename_r} as r
+                on pairs.{unique_id_col.name_r}={id_expr_r}
         """
         return sql
 
     def as_dict(self):
         output = super().as_dict()
         output["arrays_to_explode"] = self.array_columns_to_explode
         return output
 
 
-def materialise_exploded_id_tables(linker: Linker):
-    settings_obj = linker._settings_obj
-
-    blocking_rules = settings_obj._blocking_rules_to_generate_predictions
+def materialise_exploded_id_tables(
+    link_type: "LinkTypeLiteralType",
+    blocking_rules: List[BlockingRule],
+    db_api: DatabaseAPISubClass,
+    splink_df_dict: dict[str, SplinkDataFrame],
+    source_dataset_input_column: Optional[InputColumn],
+    unique_id_input_column: InputColumn,
+) -> list[ExplodingBlockingRule]:
     exploding_blocking_rules = [
         br for br in blocking_rules if isinstance(br, ExplodingBlockingRule)
     ]
+
+    if len(exploding_blocking_rules) == 0:
+        return []
     exploded_tables = []
 
-    input_dataframe = linker._initialise_df_concat_with_tf()
-    input_colnames = {col.name for col in input_dataframe.columns}
+    pipeline = CTEPipeline()
+
+    source_dataset_column_name = (
+        source_dataset_input_column.name if source_dataset_input_column else None
+    )
+
+    sql = vertically_concatenate_sql(
+        splink_df_dict,
+        salting_required=False,
+        source_dataset_column_name=source_dataset_column_name,
+    )
+    pipeline.enqueue_sql(sql, "__splink__df_concat")
+    nodes_concat = db_api.sql_pipeline_to_splink_dataframe(pipeline)
+
+    input_colnames = {col.name for col in nodes_concat.columns}
 
     for br in exploding_blocking_rules:
+        pipeline = CTEPipeline([nodes_concat])
         arrays_to_explode_quoted = [
-            InputColumn(colname, sql_dialect=linker._sql_dialect).quote().name
+            InputColumn(colname, sql_dialect=db_api.sql_dialect.name).quote().name
             for colname in br.array_columns_to_explode
         ]
-        expl_sql = linker._explode_arrays_sql(
-            "__splink__df_concat_with_tf",
+
+        expl_sql = db_api.sql_dialect.explode_arrays_sql(
+            "__splink__df_concat",
             br.array_columns_to_explode,
             list(input_colnames.difference(arrays_to_explode_quoted)),
         )
 
-        linker._enqueue_sql(
+        pipeline.enqueue_sql(
             expl_sql,
-            "__splink__df_concat_with_tf_unnested",
+            "__splink__df_concat_unnested",
         )
 
         base_name = "__splink__marginal_exploded_ids_blocking_rule"
         table_name = f"{base_name}_mk_{br.match_key}"
 
-        sql = br.marginal_exploded_id_pairs_table_sql(linker, br)
+        sql = br.marginal_exploded_id_pairs_table_sql(
+            source_dataset_input_column=source_dataset_input_column,
+            unique_id_input_column=unique_id_input_column,
+            br=br,
+            link_type=link_type,
+        )
 
-        linker._enqueue_sql(sql, table_name)
+        pipeline.enqueue_sql(sql, table_name)
 
-        marginal_ids_table = linker._execute_sql_pipeline([input_dataframe])
+        marginal_ids_table = db_api.sql_pipeline_to_splink_dataframe(pipeline)
         br.exploded_id_pair_table = marginal_ids_table
         exploded_tables.append(marginal_ids_table)
+
     return exploding_blocking_rules
 
 
-def _sql_gen_where_condition(link_type, unique_id_cols):
+def _sql_gen_where_condition(
+    link_type: backend_link_type_options, unique_id_cols: List[InputColumn]
+) -> str:
     id_expr_l = _composite_unique_id_from_nodes_sql(unique_id_cols, "l")
     id_expr_r = _composite_unique_id_from_nodes_sql(unique_id_cols, "r")
 
     if link_type in ("two_dataset_link_only", "self_link"):
         where_condition = " where 1=1 "
     elif link_type in ["link_and_dedupe", "dedupe_only"]:
         where_condition = f"where {id_expr_l} < {id_expr_r}"
@@ -444,112 +551,67 @@
             f"where {id_expr_l} < {id_expr_r} "
             f"and l.{source_dataset_col.name} != r.{source_dataset_col.name}"
         )
 
     return where_condition
 
 
-def block_using_rules_sqls(linker: Linker, blocking_rules: List[BlockingRule] = None):
+def block_using_rules_sqls(
+    *,
+    input_tablename_l: str,
+    input_tablename_r: str,
+    blocking_rules: List[BlockingRule],
+    link_type: "LinkTypeLiteralType",
+    columns_to_select_sql: str,
+    source_dataset_input_column: Optional[InputColumn],
+    unique_id_input_column: InputColumn,
+    set_match_probability_to_one: bool = False,
+) -> list[dict[str, str]]:
     """Use the blocking rules specified in the linker's settings object to
     generate a SQL statement that will create pairwise record comparions
     according to the blocking rule(s).
 
     Where there are multiple blocking rules, the SQL statement contains logic
     so that duplicate comparisons are not generated.
     """
 
     sqls = []
 
-    # For the two dataset link only, rather than a self join of
-    # __splink__df_concat_with_tf, it's much faster to split the input
-    # into two tables, and join (because then Splink doesn't have to evaluate)
-    # intra-dataset comparisons.
-    # see https://github.com/moj-analytical-services/splink/pull/1359
-    if (
-        linker._two_dataset_link_only
-        and not linker._find_new_matches_mode
-        and not linker._compare_two_records_mode
-    ):
-        source_dataset_col = (
-            linker._settings_obj.column_info_settings.source_dataset_column_name
-        )
-        # Need df_l to be the one with the lowest id to preeserve the property
-        # that the left dataset is the one with the lowest concatenated id
-
-        # This also needs to work for training u
-        if linker._train_u_using_random_sample_mode:
-            spl_switch = "_sample"
-        else:
-            spl_switch = ""
-
-        df_concat_tf = linker._intermediate_table_cache["__splink__df_concat_with_tf"]
-
-        sql = f"""
-        select * from __splink__df_concat_with_tf{spl_switch}
-        where {source_dataset_col} =
-            (select min({source_dataset_col}) from {df_concat_tf.physical_name})
-        """
-        sqls.append(
-            {
-                "sql": sql,
-                "output_table_name": f"__splink__df_concat_with_tf{spl_switch}_left",
-            }
-        )
-
-        sql = f"""
-        select * from __splink__df_concat_with_tf{spl_switch}
-        where {source_dataset_col} =
-            (select max({source_dataset_col}) from {df_concat_tf.physical_name})
-        """
-        sqls.append(
-            {
-                "sql": sql,
-                "output_table_name": f"__splink__df_concat_with_tf{spl_switch}_right",
-            }
-        )
-
-    settings_obj = linker._settings_obj
-
-    link_type = settings_obj._link_type
-
-    if linker._two_dataset_link_only:
-        link_type = "two_dataset_link_only"
-
-    if linker._self_link_mode:
-        link_type = "self_link"
-
-    where_condition = _sql_gen_where_condition(
-        link_type, settings_obj.column_info_settings.unique_id_input_columns
+    unique_id_input_columns = combine_unique_id_input_columns(
+        source_dataset_input_column, unique_id_input_column
     )
 
-    # We could have had a single 'blocking rule'
-    # property on the settings object, and avoided this logic but I wanted to be very
-    # explicit about the difference between blocking for training
-    # and blocking for predictions
-    if blocking_rules is None:
-        blocking_rules = settings_obj._blocking_rules_to_generate_predictions
+    where_condition = _sql_gen_where_condition(link_type, unique_id_input_columns)
 
     # Cover the case where there are no blocking rules
     # This is a bit of a hack where if you do a self-join on 'true'
     # you create a cartesian product, rather than having separate code
     # that generates a cross join for the case of no blocking rules
     if not blocking_rules:
         blocking_rules = [BlockingRule("1=1")]
 
     # For Blocking rules for deterministic rules, add a match probability
     # column with all probabilities set to 1.
-    if linker._deterministic_link_mode:
+    if set_match_probability_to_one:
         probability = ", 1.00 as match_probability"
     else:
         probability = ""
 
     br_sqls = []
 
     for br in blocking_rules:
-        sql = br.create_blocked_pairs_sql(linker, where_condition, probability)
+        sql = br.create_blocked_pairs_sql(
+            unique_id_input_column=unique_id_input_column,
+            source_dataset_input_column=source_dataset_input_column,
+            input_tablename_l=input_tablename_l,
+            input_tablename_r=input_tablename_r,
+            where_condition=where_condition,
+            probability=probability,
+            sql_select_expr=columns_to_select_sql,
+        )
         br_sqls.append(sql)
 
     sql = " UNION ALL ".join(br_sqls)
 
     sqls.append({"sql": sql, "output_table_name": "__splink__df_blocked"})
 
     return sqls
```

### Comparing `splink-4.0.0.dev3/splink/blocking_rule_creator.py` & `splink-4.0.0.dev4/splink/blocking_rule_creator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
-from typing import final
+from typing import Any, Dict, Union, final
 
 from .blocking import BlockingRule, blocking_rule_to_obj
 from .dialects import SplinkDialect
 
 
 class BlockingRuleCreator(ABC):
-    def __init__(self, salting_partitions=None, arrays_to_explode=None):
+    def __init__(
+        self,
+        salting_partitions: int | None = None,
+        arrays_to_explode: list[str] | None = None,
+    ):
         self._salting_partitions = salting_partitions
         self._arrays_to_explode = arrays_to_explode
 
     # @property because merged levels need logic to determine salting partitions
     @property
     def salting_partitions(self):
         return self._salting_partitions
@@ -20,15 +26,15 @@
         return self._arrays_to_explode
 
     @abstractmethod
     def create_sql(self, sql_dialect: SplinkDialect) -> str:
         pass
 
     @final
-    def create_blocking_rule_dict(self, sql_dialect_str: str) -> dict:
+    def create_blocking_rule_dict(self, sql_dialect_str: str) -> dict[str, Any]:
         sql_dialect = SplinkDialect.from_string(sql_dialect_str)
         level_dict = {
             "blocking_rule": self.create_sql(sql_dialect),
             "sql_dialect": sql_dialect_str,
         }
 
         if self.salting_partitions and self.arrays_to_explode:
@@ -41,7 +47,10 @@
             level_dict["arrays_to_explode"] = self.arrays_to_explode
 
         return level_dict
 
     @final
     def get_blocking_rule(self, sql_dialect_str: str) -> BlockingRule:
         return blocking_rule_to_obj(self.create_blocking_rule_dict(sql_dialect_str))
+
+
+acceptable_br_creator_types = Union[BlockingRuleCreator, str, Dict[str, Any]]
```

### Comparing `splink-4.0.0.dev3/splink/blocking_rule_library.py` & `splink-4.0.0.dev4/splink/blocking_rule_library.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Union, final
+from __future__ import annotations
+
+from typing import Any, Union, final
 
 from sqlglot import TokenError, parse_one
 
 from .blocking_rule_creator import BlockingRuleCreator
 from .column_expression import ColumnExpression
 from .dialects import SplinkDialect
 
@@ -17,16 +19,16 @@
     return tree.sql(dialect=to_sqlglot_dialect)
 
 
 class ExactMatchRule(BlockingRuleCreator):
     def __init__(
         self,
         col_name_or_expr: Union[str, ColumnExpression],
-        salting_partitions=None,
-        arrays_to_explode=None,
+        salting_partitions: int = None,
+        arrays_to_explode: list[str] | None = None,
     ):
         super().__init__(
             salting_partitions=salting_partitions, arrays_to_explode=arrays_to_explode
         )
         self.col_expression = ColumnExpression.instantiate_if_str(col_name_or_expr)
 
     def create_sql(self, sql_dialect: SplinkDialect) -> str:
@@ -36,16 +38,16 @@
 
 
 class CustomRule(BlockingRuleCreator):
     def __init__(
         self,
         blocking_rule: str,
         base_dialect_str: str = None,
-        salting_partitions=None,
-        arrays_to_explode=None,
+        salting_partitions: int | None = None,
+        arrays_to_explode: list[str] | None = None,
     ):
         super().__init__(
             salting_partitions=salting_partitions, arrays_to_explode=arrays_to_explode
         )
         self.sql_condition = blocking_rule
 
         self.base_dialect_str = base_dialect_str
@@ -76,17 +78,17 @@
 
 class _Merge(BlockingRuleCreator):
     _clause = ""
 
     @final
     def __init__(
         self,
-        *blocking_rules: Union[BlockingRuleCreator, dict],
-        salting_partitions=None,
-        arrays_to_explode=None,
+        *blocking_rules: Union[BlockingRuleCreator, dict[str, Any]],
+        salting_partitions: int | None = None,
+        arrays_to_explode: list[str] | None = None,
     ):
         super().__init__(
             salting_partitions=salting_partitions, arrays_to_explode=arrays_to_explode
         )
         num_levels = len(blocking_rules)
         if num_levels == 0:
             raise ValueError(
@@ -155,16 +157,16 @@
     @final
     def create_sql(self, sql_dialect: SplinkDialect) -> str:
         return f"NOT ({self.blocking_rule_creator.create_sql(sql_dialect)})"
 
 
 def block_on(
     *col_names_or_exprs: Union[str, ColumnExpression],
-    salting_partitions=None,
-    arrays_to_explode=None,
+    salting_partitions: int | None = None,
+    arrays_to_explode: list[str] | None = None,
 ) -> BlockingRuleCreator:
     if isinstance(col_names_or_exprs[0], list):
         raise TypeError(
             "block_on no longer accepts a list as the first argument. "
             "Please pass individual column names or expressions as separate arguments"
             ' e.g. block_on("first_name", "dob") not block_on(["first_name", "dob"])'
         )
```

### Comparing `splink-4.0.0.dev3/splink/cache_dict_with_logging.py` & `splink-4.0.0.dev4/splink/cache_dict_with_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import logging
 from collections import UserDict
 from copy import copy
+from typing import TYPE_CHECKING
 
 from .splink_dataframe import SplinkDataFrame
 
 logger = logging.getLogger(__name__)
 
+if TYPE_CHECKING:
+    TypedUserDict = UserDict[str, SplinkDataFrame]
+else:
+    TypedUserDict = UserDict
 
-class CacheDictWithLogging(UserDict):
+
+class CacheDictWithLogging(TypedUserDict):
     def __init__(self):
         super().__init__()
         self.executed_queries = []
         self.queries_retrieved_from_cache = []
 
-    def __getitem__(self, key) -> SplinkDataFrame:
+    def __getitem__(self, key: str) -> SplinkDataFrame:
         splink_dataframe = super().__getitem__(key)
 
         # Return a copy so that user can modify physical or templated name
         # without modifying the version in the cache
         return copy(splink_dataframe)
 
     def __setitem__(self, key, value):
```

### Comparing `splink-4.0.0.dev3/splink/charts.py` & `splink-4.0.0.dev4/splink/charts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,33 @@
+from __future__ import annotations
+
 import json
 import math
 import os
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 import numpy as np
 import pandas as pd
 
 from .misc import read_resource
 from .waterfall_chart import records_to_waterfall_data
 
 altair_installed = True
 
 try:
     import altair as alt
 except ImportError:
     altair_installed = False
 
+if TYPE_CHECKING:
+    import altair as alt
+
+# type alias:
+ChartReturnType = Union[Dict[Any, Any], alt.core.SchemaBase]
+
 
 def load_chart_definition(filename):
     path = f"files/chart_defs/{filename}"
     return json.loads(read_resource(path))
 
 
 def _load_external_libs():
@@ -26,15 +35,17 @@
         "vega-embed": "files/external_js/vega-embed@6.20.2",
         "vega-lite": "files/external_js/vega-lite@5.2.0",
         "vega": "files/external_js/vega@5.21.0",
     }
     return {k: read_resource(v) for k, v in to_load.items()}
 
 
-def altair_or_json(chart_dict, as_dict=False):
+def altair_or_json(
+    chart_dict: dict[Any, Any], as_dict: bool = False
+) -> ChartReturnType:
     if altair_installed:
         if not as_dict:
             try:
                 return alt.Chart.from_dict(chart_dict)
 
             except ModuleNotFoundError:
                 return chart_dict
@@ -264,15 +275,15 @@
         "specificity": "Specificity (TNR)",
         "accuracy": "Accuracy",
         "npv": "NPV",
         "f1": "F1",
         "f2": "F2",
         "f0_5": "F0.5",
         "p4": "P4",
-        "phi": "\u03C6 (MCC)",
+        "phi": "\u03c6 (MCC)",
     }
     chart["transform"][2]["calculate"] = chart["transform"][2]["calculate"].replace(
         "__mapping__", str(mapping)
     )
     chart["layer"][0]["encoding"]["color"]["legend"]["labelExpr"] = chart["layer"][0][
         "encoding"
     ]["color"]["legend"]["labelExpr"].replace("__mapping__", str(mapping))
@@ -309,15 +320,15 @@
         "specificity": "Specificity (TNR)",
         "accuracy": "Accuracy",
         "npv": "NPV",
         "f1": "F1",
         "f2": "F2",
         "f0_5": "F0.5",
         "p4": "P4",
-        "phi": "\u03C6 (MCC)",
+        "phi": "\u03c6 (MCC)",
     }
     chart["hconcat"][1]["transform"][2]["calculate"] = chart["hconcat"][1]["transform"][
         2
     ]["calculate"].replace("__mapping__", str(mapping))
     chart["hconcat"][1]["layer"][0]["encoding"]["color"]["legend"]["labelExpr"] = chart[
         "hconcat"
     ][1]["layer"][0]["encoding"]["color"]["legend"]["labelExpr"].replace(
@@ -376,40 +387,40 @@
         )
 
     chart_path = "unlinkables_chart_def.json"
     unlinkables_chart_def = load_chart_definition(chart_path)
     unlinkables_chart_def["data"]["values"] = records
 
     if x_col == "match_probability":
-        unlinkables_chart_def["layer"][0]["encoding"]["x"][
-            "field"
-        ] = "match_probability"
-        unlinkables_chart_def["layer"][0]["encoding"]["x"]["axis"][
-            "title"
-        ] = "Threshold match probability"
+        unlinkables_chart_def["layer"][0]["encoding"]["x"]["field"] = (
+            "match_probability"
+        )
+        unlinkables_chart_def["layer"][0]["encoding"]["x"]["axis"]["title"] = (
+            "Threshold match probability"
+        )
         unlinkables_chart_def["layer"][0]["encoding"]["x"]["axis"]["format"] = ".2"
 
-        unlinkables_chart_def["layer"][1]["encoding"]["x"][
-            "field"
-        ] = "match_probability"
+        unlinkables_chart_def["layer"][1]["encoding"]["x"]["field"] = (
+            "match_probability"
+        )
         unlinkables_chart_def["layer"][1]["selection"]["selector112"]["fields"] = [
             "match_probability",
             "cum_prop",
         ]
 
-        unlinkables_chart_def["layer"][2]["encoding"]["x"][
-            "field"
-        ] = "match_probability"
-        unlinkables_chart_def["layer"][2]["encoding"]["x"]["axis"][
-            "title"
-        ] = "Threshold match probability"
-
-        unlinkables_chart_def["layer"][3]["encoding"]["x"][
-            "field"
-        ] = "match_probability"
+        unlinkables_chart_def["layer"][2]["encoding"]["x"]["field"] = (
+            "match_probability"
+        )
+        unlinkables_chart_def["layer"][2]["encoding"]["x"]["axis"]["title"] = (
+            "Threshold match probability"
+        )
+
+        unlinkables_chart_def["layer"][3]["encoding"]["x"]["field"] = (
+            "match_probability"
+        )
 
     if source_dataset:
         unlinkables_chart_def["title"]["text"] += f" - {source_dataset}"
 
     return altair_or_json(unlinkables_chart_def, as_dict=as_dict)
```

### Comparing `splink-4.0.0.dev3/splink/cluster_studio.py` & `splink-4.0.0.dev4/splink/cluster_studio.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,78 @@
 from __future__ import annotations
 
 import json
 import os
 import random
-from typing import TYPE_CHECKING, Any, Optional
+from typing import TYPE_CHECKING, Any, Literal, Optional
 
 from jinja2 import Template
 
 from .exceptions import SplinkException
 from .misc import EverythingEncoder, read_resource
+from .pipeline import CTEPipeline
 from .splink_dataframe import SplinkDataFrame
 from .unique_id_concat import (
     _composite_unique_id_from_edges_sql,
     _composite_unique_id_from_nodes_sql,
 )
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
     from .linker import Linker
 
+SamplingMethods = Literal[
+    "random", "by_cluster_size", "lowest_density_clusters_by_size"
+]
+
 
 def _quo_if_str(x):
     if isinstance(x, str):
         return f"'{x}'"
     else:
         return str(x)
 
 
-def _clusters_sql(df_clustered_nodes, cluster_ids: list) -> str:
+def _clusters_sql(df_clustered_nodes: SplinkDataFrame, cluster_ids: list[str]) -> str:
     cluster_ids = [_quo_if_str(x) for x in cluster_ids]
     cluster_ids_joined = ", ".join(cluster_ids)
 
     sql = f"""
     select distinct(cluster_id)
     from {df_clustered_nodes.physical_name}
     where cluster_id in ({cluster_ids_joined})
     """
 
     return sql
 
 
 def df_clusters_as_records(
-    linker: "Linker", df_clustered_nodes: SplinkDataFrame, cluster_ids: list
-) -> list[dict]:
+    linker: "Linker", df_clustered_nodes: SplinkDataFrame, cluster_ids: list[str]
+) -> list[dict[str, Any]]:
     """Retrieves distinct clusters which exist in df_clustered_nodes based on
     list of cluster IDs provided and converts them to a record dictionary.
 
     Args:
         linker: An instance of the Splink Linker class.
         df_clustered_nodes (SplinkDataFrame): Result of
         cluster_pairwise_predictions_at_threshold().
         cluster_ids (list): List of cluster IDs to filter the results.
 
     Returns:
     dict: A record dictionary of the specified cluster IDs.
     """
     sql = _clusters_sql(df_clustered_nodes, cluster_ids)
-    df_clusters = linker._sql_to_splink_dataframe_checking_cache(
-        sql, "__splink__scs_clusters"
-    )
+    pipeline = CTEPipeline()
+    pipeline.enqueue_sql(sql, "__splink__scs_clusters")
+    df_clusters = linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
+
     return df_clusters.as_record_dict()
 
 
-def _nodes_sql(df_clustered_nodes, cluster_ids) -> str:
+def _nodes_sql(df_clustered_nodes: SplinkDataFrame, cluster_ids: list[str]) -> str:
     """Generates SQL query to select all columns from df_clustered_nodes
     for list of cluster IDs provided.
 
     Args:
         df_clustered_nodes (SplinkDataFrame): result of
         cluster_pairwise_predictions_at_threshold()
         cluster_ids (list): List of cluster IDs to filter the results
@@ -81,37 +87,38 @@
     where cluster_id in ({cluster_ids_joined})
     """
 
     return sql
 
 
 def create_df_nodes(
-    linker: "Linker", df_clustered_nodes: SplinkDataFrame, cluster_ids: list
+    linker: "Linker", df_clustered_nodes: SplinkDataFrame, cluster_ids: list[str]
 ) -> SplinkDataFrame:
     """Retrieves nodes from df_clustered_nodes for list of cluster IDs provided.
 
     Args:
         linker: An instance of the Splink Linker class.
         df_clustered_nodes (SplinkDataFrame): Result of
         cluster_pairwise_predictions_at_threshold().
         cluster_ids (list): List of cluster IDs to filter the results.
 
     Returns:
         A SplinkDataFrame containing the nodes for the specified cluster IDs.
     """
+    pipeline = CTEPipeline()
     sql = _nodes_sql(df_clustered_nodes, cluster_ids)
-    df_nodes = linker._sql_to_splink_dataframe_checking_cache(
-        sql, "__splink__scs_nodes"
-    )
+    pipeline.enqueue_sql(sql, "__splink__scs_nodes")
+    df_nodes = linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
+
     return df_nodes
 
 
 def _edges_sql(
     linker: "Linker", df_predicted_edges: SplinkDataFrame, df_nodes: SplinkDataFrame
-):
+) -> str:
     unique_id_cols = linker._settings_obj.column_info_settings.unique_id_input_columns
 
     nodes_l_id_expr = _composite_unique_id_from_nodes_sql(unique_id_cols, "nodes_l")
     nodes_r_id_expr = _composite_unique_id_from_nodes_sql(unique_id_cols, "nodes_r")
     edges_l_id_expr = _composite_unique_id_from_edges_sql(
         unique_id_cols, "l", table_prefix="edges"
     )
@@ -136,32 +143,36 @@
     on {edges_r_id_expr} = {nodes_r_id_expr}
     """
     return sql
 
 
 def df_edges_as_records(
     linker: "Linker", df_predicted_edges: SplinkDataFrame, df_nodes: SplinkDataFrame
-):
+) -> list[dict[str, Any]]:
     sql = _edges_sql(linker, df_predicted_edges, df_nodes)
-    df_edges = linker._sql_to_splink_dataframe_checking_cache(
-        sql, "__splink__scs_edges"
-    )
+    pipeline = CTEPipeline()
+    pipeline.enqueue_sql(sql, "__splink__scs_edges")
+    df_edges = linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
+
     return df_edges.as_record_dict()
 
 
 def _get_random_cluster_ids(
-    linker: "Linker", connected_components: SplinkDataFrame, sample_size: int, seed=None
+    linker: "Linker",
+    connected_components: SplinkDataFrame,
+    sample_size: int,
+    seed: int | None = None,
 ) -> list[str]:
     sql = f"""
     select count(distinct cluster_id) as count
     from {connected_components.physical_name}
     """
-    df_cluster_count = linker._sql_to_splink_dataframe_checking_cache(
-        sql, "__splink__cluster_count"
-    )
+    pipeline = CTEPipeline()
+    pipeline.enqueue_sql(sql, "__splink__cluster_count")
+    df_cluster_count = linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
     cluster_count = df_cluster_count.as_record_dict()[0]["count"]
     df_cluster_count.drop_table_from_database_and_remove_from_cache()
 
     proportion = sample_size / cluster_count
 
     random_sample_sql = linker._random_sample_sql(
         proportion,
@@ -175,69 +186,71 @@
     with distinct_clusters as (
     select distinct(cluster_id)
     from {connected_components.physical_name}
     )
     select cluster_id from distinct_clusters
     {random_sample_sql}
     """
+    pipeline = CTEPipeline()
+    pipeline.enqueue_sql(sql, "__splink__df_concat_with_tf_sample")
+    df_sample = linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
-    df_sample = linker._sql_to_splink_dataframe_checking_cache(
-        sql,
-        "__splink__df_concat_with_tf_sample",
-    )
     return [r["cluster_id"] for r in df_sample.as_record_dict()]
 
 
 def _get_cluster_id_of_each_size(
     linker: "Linker", connected_components: SplinkDataFrame, rows_per_partition: int
-) -> list[dict]:
+) -> list[dict[str, Any]]:
     unique_id_col_name = linker._settings_obj.column_info_settings.unique_id_column_name
+    pipeline = CTEPipeline()
     sql = f"""
     select
         cluster_id,
         count(*) as cluster_size,
         max({unique_id_col_name}) as ordering
     from {connected_components.physical_name}
     group by cluster_id
     having count(*)>1
     """
 
-    linker._enqueue_sql(sql, "__splink__cluster_count")
+    pipeline.enqueue_sql(sql, "__splink__cluster_count")
 
     # Assign unique row number to each row in partition
     sql = """
     select
         cluster_id,
         cluster_size,
         row_number() over (partition by cluster_size order by ordering) as row_num
     from __splink__cluster_count
     """
 
-    linker._enqueue_sql(sql, "__splink__cluster_count_row_numbered")
+    pipeline.enqueue_sql(sql, "__splink__cluster_count_row_numbered")
 
     sql = f"""
     select
         cluster_id,
         cluster_size
     from __splink__cluster_count_row_numbered
     where row_num <= {rows_per_partition}
     """
 
-    linker._enqueue_sql(sql, "__splink__cluster_count_row_numbered")
-    df_cluster_sample_with_size = linker._execute_sql_pipeline()
+    pipeline.enqueue_sql(sql, "__splink__cluster_count_row_numbered")
+    df_cluster_sample_with_size = linker.db_api.sql_pipeline_to_splink_dataframe(
+        pipeline
+    )
 
     return df_cluster_sample_with_size.as_record_dict()
 
 
 def _get_lowest_density_clusters(
     linker: "Linker",
     df_cluster_metrics: SplinkDataFrame,
     rows_per_partition: int,
     min_nodes: int,
-) -> list[dict]:
+) -> list[dict[str, Any]]:
     """Returns lowest density clusters of different sizes by
     performing stratified sampling.
 
     Args:
         linker: An instance of the Splink Linker class.
         df_cluster_metrics (SplinkDataFrame): dataframe containing
         cluster metrics including density.
@@ -245,50 +258,52 @@
         min_nodes (int): minimum number of nodes a cluster must contain
         to be included in the sample.
 
     Returns:
         list: A list of record dictionaries containing cluster ids, densities
         and sizes of lowest density clusters.
     """
-
+    pipeline = CTEPipeline()
     sql = f"""
     select
         cluster_id,
         n_nodes,
         density,
         row_number() over (partition by n_nodes order by density, cluster_id) as row_num
     from {df_cluster_metrics.physical_name}
     where n_nodes >= {min_nodes}
     """
 
-    linker._enqueue_sql(sql, "__splink__partition_clusters_by_size")
+    pipeline.enqueue_sql(sql, "__splink__partition_clusters_by_size")
 
     sql = f"""
     select
         cluster_id,
         round(density, 4) as density_4dp,
         n_nodes as cluster_size
     from __splink__partition_clusters_by_size
     where row_num <= {rows_per_partition}
     """
 
-    linker._enqueue_sql(sql, "__splink__lowest_density_clusters")
-    df_lowest_density_clusters = linker._execute_sql_pipeline()
+    pipeline.enqueue_sql(sql, "__splink__lowest_density_clusters")
+    df_lowest_density_clusters = linker.db_api.sql_pipeline_to_splink_dataframe(
+        pipeline
+    )
 
     return df_lowest_density_clusters.as_record_dict()
 
 
 def _get_cluster_ids(
     linker: "Linker",
     df_clustered_nodes: SplinkDataFrame,
-    sampling_method,
-    sample_size,
-    sample_seed,
+    sampling_method: SamplingMethods,
+    sample_size: int,
+    sample_seed: int | None,
     _df_cluster_metrics: Optional[SplinkDataFrame] = None,
-) -> tuple[list, list]:
+) -> tuple[list[str], list[str]]:
     if sampling_method == "random":
         cluster_ids = _get_random_cluster_ids(
             linker, df_clustered_nodes, sample_size, sample_seed
         )
         cluster_names = []
     elif sampling_method == "by_cluster_size":
         cluster_id_infos = _get_cluster_id_of_each_size(
@@ -327,22 +342,22 @@
 
 
 def render_splink_cluster_studio_html(
     linker: "Linker",
     df_predicted_edges: SplinkDataFrame,
     df_clustered_nodes: SplinkDataFrame,
     out_path: str,
-    sampling_method="random",
-    sample_size=10,
-    sample_seed=None,
+    sampling_method: SamplingMethods = "random",
+    sample_size: int = 10,
+    sample_seed: int | None = None,
     cluster_ids: list[str] = None,
-    cluster_names: list = None,
+    cluster_names: list[str] = None,
     overwrite: bool = False,
     _df_cluster_metrics: SplinkDataFrame = None,
-):
+) -> str:
     bundle_observable_notebook = True
 
     svu_options = {
         "cluster_colname": "cluster_id",
         "prob_colname": "match_probability",
     }
     if cluster_ids is None:
```

### Comparing `splink-4.0.0.dev3/splink/column_expression.py` & `splink-4.0.0.dev4/splink/column_expression.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,33 +36,33 @@
     Note that this will typically be created without a dialect, and the dialect
     will later be populated when the ColumnExpression is passed via a comparison
     level creator into a linker.
     """
 
     def __init__(self, sql_expression: str, sql_dialect: SplinkDialect = None):
         self.raw_sql_expression = sql_expression
-        self.operations: list[Callable] = []
+        self.operations: list[Callable[..., str]] = []
         if sql_dialect is not None:
             self.sql_dialect: SplinkDialect = sql_dialect
 
-    def _clone(self):
+    def _clone(self) -> "ColumnExpression":
         clone = copy(self)
         clone.operations = [op for op in self.operations]
         return clone
 
     @staticmethod
     def instantiate_if_str(
-        str_or_column_expression: Union[str, "ColumnExpression"]
+        str_or_column_expression: Union[str, "ColumnExpression"],
     ) -> "ColumnExpression":
         if isinstance(str_or_column_expression, ColumnExpression):
             return str_or_column_expression
         elif isinstance(str_or_column_expression, str):
             return ColumnExpression(str_or_column_expression)
 
-    def parse_input_string(self, dialect: SplinkDialect):
+    def parse_input_string(self, dialect: SplinkDialect) -> str:
         """
         The input into an ColumnExpression can be
             - a column name or column reference e.g. first_name, first name
             - a sql expression e.g. UPPER(first_name), first_name || surname
 
         In the former case, we do not expect the user to have escaped the column name
         with identifier quotes (see also InputColumn).
@@ -75,84 +75,84 @@
             return self.raw_sql_expression
 
         return SqlglotColumnTreeBuilder.from_raw_column_name_or_column_reference(
             self.raw_sql_expression, dialect.sqlglot_name
         ).sql
 
     @property
-    def raw_sql_is_pure_column_or_column_reference(self):
+    def raw_sql_is_pure_column_or_column_reference(self) -> bool:
         # It's difficult (possibly impossible) to find a completely general
         # algorithm that can distinguish between the two cases (col name, or sql
         # expression), since lower(first_name) could technically be a column name
         # Here I use a heuristic:
         # If there's a () or || then assume it's a sql expression
         if re.search(r"\([^)]*\)", self.raw_sql_expression):
             return False
 
         if "||" in self.raw_sql_expression:
             return False
         return True
 
     @property
-    def is_pure_column_or_column_reference(self):
+    def is_pure_column_or_column_reference(self) -> bool:
         if len(self.operations) > 0:
             return False
 
         return self.raw_sql_is_pure_column_or_column_reference
 
-    def apply_operations(self, name: str, dialect: SplinkDialect):
+    def apply_operations(self, name: str, dialect: SplinkDialect) -> str:
         for op in self.operations:
             name = op(name=name, dialect=dialect)
         return name
 
-    def _lower_dialected(self, name, dialect):
+    def _lower_dialected(self, name: str, dialect: SplinkDialect) -> str:
         lower_sql = sqlglot.parse_one("lower(___col___)").sql(
             dialect=dialect.sqlglot_name
         )
 
         return lower_sql.replace("___col___", name)
 
-    def lower(self):
+    def lower(self) -> "ColumnExpression":
         """
         Applies a lowercase transofrom to the input expression.
         """
         clone = self._clone()
         clone.operations.append(clone._lower_dialected)
         return clone
 
     def _substr_dialected(
         self, name: str, start: int, end: int, dialect: SplinkDialect
-    ):
+    ) -> str:
         substr_sql = sqlglot.parse_one(f"substring(___col___, {start}, {end})").sql(
             dialect=dialect.sqlglot_name
         )
 
         return substr_sql.replace("___col___", name)
 
-    def substr(self, start: int, length: int):
+    def substr(self, start: int, length: int) -> "ColumnExpression":
         """
         Applies a substring transform to the input expression of a given length
         starting from a specified index.
         Args:
             start (int): The starting index of the substring.
             length (int): The length of the substring.
         """
         clone = self._clone()
         op = partial(clone._substr_dialected, start=start, end=length)
         clone.operations.append(op)
 
         return clone
 
-    def _cast_to_string_dialected(self, name: str, dialect: SplinkDialect):
+    def _cast_to_string_dialected(self, name: str, dialect: SplinkDialect) -> str:
         cast_sql = sqlglot.parse_one("cast(___col___ as string)").sql(
             dialect=dialect.sqlglot_name
         )
         return cast_sql.replace("___col___", name)
 
-    def cast_to_string(self):
+    def cast_to_string(self) -> "ColumnExpression":
         """
         Applies a cast to string transform to the input expression.
         """
         clone = self._clone()
         op = partial(clone._cast_to_string_dialected)
         clone.operations.append(op)
 
@@ -169,15 +169,15 @@
         # position (capture group) arg
         return dialect.regex_extract(
             name,
             pattern=pattern,
             capture_group=capture_group,
         )
 
-    def regex_extract(self, pattern: str, capture_group: int = 0):
+    def regex_extract(self, pattern: str, capture_group: int = 0) -> "ColumnExpression":
         """Applies a regex extract transform to the input expression.
 
         Args:
             pattern (str): The regex pattern to match.
             capture_group (int): The capture group to extract from the matched pattern.
                 Defaults to 0, meaning the full pattern is extracted
 
@@ -193,36 +193,36 @@
         return clone
 
     def _try_parse_date_dialected(
         self,
         name: str,
         dialect: SplinkDialect,
         date_format: str = None,
-    ):
+    ) -> str:
         return dialect.try_parse_date(name, date_format=date_format)
 
-    def try_parse_date(self, date_format: str = None):
+    def try_parse_date(self, date_format: str = None) -> "ColumnExpression":
         clone = self._clone()
         op = partial(
             clone._try_parse_date_dialected,
             date_format=date_format,
         )
         clone.operations.append(op)
 
         return clone
 
     def _try_parse_timestamp_dialected(
         self,
         name: str,
         dialect: SplinkDialect,
         timestamp_format: str = None,
-    ):
+    ) -> str:
         return dialect.try_parse_timestamp(name, timestamp_format=timestamp_format)
 
-    def try_parse_timestamp(self, timestamp_format: str = None):
+    def try_parse_timestamp(self, timestamp_format: str = None) -> "ColumnExpression":
         clone = self._clone()
         op = partial(
             clone._try_parse_timestamp_dialected,
             timestamp_format=timestamp_format,
         )
         clone.operations.append(op)
```

### Comparing `splink-4.0.0.dev3/splink/comparison.py` & `splink-4.0.0.dev4/splink/comparison.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, Any, List, Optional
 
 from .comparison_level import ComparisonLevel, _default_m_values, _default_u_values
 from .misc import dedupe_preserving_order, join_list_with_commas_final_and
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
     from .settings import ColumnInfoSettings
@@ -58,18 +58,17 @@
         self,
         comparison_levels: List[ComparisonLevel],
         sqlglot_dialect_name: str,
         output_column_name: str = None,
         comparison_description: str = None,
         column_info_settings: ColumnInfoSettings = None,
     ):
-
         self.comparison_levels: list[ComparisonLevel] = comparison_levels
 
-        self.column_info_settings: Optional[ColumnInfoSettings] = column_info_settings
+        self._column_info_settings: Optional[ColumnInfoSettings] = column_info_settings
 
         self.sqlglot_dialect_name = sqlglot_dialect_name
         self.output_column_name = (
             output_column_name or self._default_output_column_name()
         )
         self.comparison_description = (
             comparison_description or self._default_comparison_description()
@@ -89,29 +88,39 @@
                 level._comparison_vector_value = counter
                 if counter == num_levels - 1:
                     level._max_level = True
                 else:
                     level._max_level = False
                 counter -= 1
             level.default_m_probability = default_m_values[
-                level._comparison_vector_value
+                level.comparison_vector_value
             ]
             level.default_u_probability = default_u_values[
-                level._comparison_vector_value
+                level.comparison_vector_value
             ]
 
     @property
     def _num_levels(self):
         return len([cl for cl in self.comparison_levels if not cl.is_null_level])
 
     @property
     def _comparison_levels_excluding_null(self):
         return [cl for cl in self.comparison_levels if not cl.is_null_level]
 
     @property
+    def column_info_settings(self) -> ColumnInfoSettings:
+        if (column_info_settings := self._column_info_settings) is None:
+            raise AttributeError(f"No column_info_settings set on Comparison {self}")
+        return column_info_settings
+
+    @column_info_settings.setter
+    def column_info_settings(self, column_info_settings: ColumnInfoSettings) -> None:
+        self._column_info_settings = column_info_settings
+
+    @property
     def gamma_prefix(self):
         return self.column_info_settings.comparison_vector_value_column_prefix
 
     @property
     def _bf_column_name(self):
         bf_prefix = self.column_info_settings.bayes_factor_column_prefix
         return f"{bf_prefix}{self.output_column_name}".replace(" ", "_")
@@ -201,15 +210,17 @@
             if cl._has_tf_adjustments:
                 col = cl._tf_adjustment_input_column
                 output_cols.extend(col.tf_name_l_r)
 
         return dedupe_preserving_order(output_cols)
 
     def _columns_to_select_for_bayes_factor_parts(
-        self, retain_matching_columns, retain_intermediate_calculation_columns
+        self,
+        retain_matching_columns: bool,
+        retain_intermediate_calculation_columns: bool,
     ) -> List[str]:
         input_cols = []
         for cl in self.comparison_levels:
             input_cols.extend(cl._input_columns_used_by_sql_condition)
 
         output_cols = []
         if retain_matching_columns:
@@ -245,17 +256,17 @@
             output_cols.append(sql)
         output_cols.append(self._gamma_column_name)
 
         return dedupe_preserving_order(output_cols)
 
     def _columns_to_select_for_predict(
         self,
-        retain_matching_columns,
-        retain_intermediate_calculation_columns,
-        training_mode,
+        retain_matching_columns: bool,
+        retain_intermediate_calculation_columns: bool,
+        training_mode: bool,
     ) -> List[str]:
         input_cols = []
         for cl in self.comparison_levels:
             input_cols.extend(cl._input_columns_used_by_sql_condition)
 
         output_cols = []
         if retain_matching_columns:
@@ -279,21 +290,14 @@
     def _match_weight_columns_to_multiply(self):
         cols = []
         cols.append(self._bf_column_name)
         if self._has_tf_adjustments:
             cols.append(self._bf_tf_adj_column_name)
         return cols
 
-    @property
-    def _term_frequency_columns(self):
-        cols = set()
-        for cl in self.comparison_levels:
-            cols.add(cl.tf_adjustment_input_col_name)
-        return list(cols)
-
     def as_dict(self):
         d = {
             "output_column_name": self.output_column_name,
             "comparison_levels": [cl.as_dict() for cl in self.comparison_levels],
         }
         d["comparison_description"] = self.comparison_description
         return d
@@ -354,15 +358,15 @@
         return message
 
     @property
     def _is_trained(self):
         return self._all_m_are_trained and self._all_u_are_trained
 
     @property
-    def _as_detailed_records(self) -> list[dict]:
+    def _as_detailed_records(self) -> list[dict[str, Any]]:
         records = []
         for cl in self.comparison_levels:
             record = {}
             record["comparison_name"] = self.output_column_name
             record = {
                 **record,
                 **cl._as_detailed_record(self._num_levels, self.comparison_levels),
@@ -380,18 +384,18 @@
             for r in new_records:
                 r["comparison_name"] = self.output_column_name
             records.extend(new_records)
 
         return records
 
     def _get_comparison_level_by_comparison_vector_value(
-        self, value
+        self, value: int
     ) -> ComparisonLevel:
         for cl in self.comparison_levels:
-            if cl._comparison_vector_value == value:
+            if cl.comparison_vector_value == value:
                 return cl
         raise ValueError(f"No comparison level with comparison vector value {value}")
 
     def __repr__(self):
         return (
             f"<Comparison {self.comparison_description} with "
             f"{self._num_levels} levels at {hex(id(self))}>"
@@ -416,22 +420,22 @@
 
     @property
     def _comparison_level_description_list(self):
         cl_template = "    - '{label}' with SQL rule: {sql}\n"
 
         comp_levels = [
             cl_template.format(
-                cvv=cl._comparison_vector_value,
+                cvv=cl.comparison_vector_value,
                 label=cl.label_for_charts,
                 sql=cl.sql_condition,
             )
             for cl in self.comparison_levels
         ]
-        comp_levels = "".join(comp_levels)
-        return comp_levels
+        comp_levels_str = "".join(comp_levels)
+        return comp_levels_str
 
     @property
     def _human_readable_description_succinct(self):
         input_cols = join_list_with_commas_final_and(
             [c.name for c in self._input_columns_used_by_case_statement]
         )
```

### Comparing `splink-4.0.0.dev3/splink/comparison_creator.py` & `splink-4.0.0.dev4/splink/comparison_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
-from typing import Dict, List, Union, final
+from typing import Any, Dict, List, Optional, Union, final
 
 from .column_expression import ColumnExpression
 from .comparison import Comparison
 from .comparison_level_creator import ComparisonLevelCreator
 from .exceptions import SplinkException
 
 
@@ -108,28 +110,29 @@
         )
 
     @abstractmethod
     def create_description(self) -> str:
         pass
 
     @abstractmethod
-    def create_output_column_name(self) -> str:
+    def create_output_column_name(self) -> Optional[str]:
+        # should be str where possible, otherwise a default will be created
         pass
 
     @final
     def get_comparison(self, sql_dialect_str: str) -> Comparison:
         """sql_dialect_str is a string to make this method easier to use
         for the end user - otherwise they'd need to import a SplinkDialect"""
         return Comparison(
             **self.create_comparison_dict(sql_dialect_str),
             sqlglot_dialect_name=sql_dialect_str,
         )
 
     @final
-    def create_comparison_dict(self, sql_dialect_str: str) -> dict:
+    def create_comparison_dict(self, sql_dialect_str: str) -> dict[str, Any]:
         level_dict = {
             "comparison_description": self.create_description(),
             "output_column_name": self.create_output_column_name(),
             "comparison_levels": [
                 cl.get_comparison_level(sql_dialect_str)
                 for cl in self.get_configured_comparison_levels()
             ],
@@ -173,24 +176,24 @@
 
     @property
     def term_frequency_adjustments(self):
         return getattr(self, "_term_frequency_adjustments", False)
 
     @term_frequency_adjustments.setter
     @final
-    def term_frequency_adjustments(self, term_frequency_adjustments: bool):
+    def term_frequency_adjustments(self, term_frequency_adjustments: bool) -> None:
         self._term_frequency_adjustments = term_frequency_adjustments
 
     @property
     def m_probabilities(self):
         return getattr(self, "_m_probabilities", None)
 
     @m_probabilities.setter
     @final
-    def m_probabilities(self, m_probabilities: List[float]):
+    def m_probabilities(self, m_probabilities: List[float]) -> None:
         if m_probabilities:
             num_probs_supplied = len(m_probabilities)
             num_non_null_levels = self.num_non_null_levels
             if num_probs_supplied != self.num_non_null_levels:
                 raise ValueError(
                     f"Comparison has {num_non_null_levels} non-null levels, "
                     f"but received {num_probs_supplied} values for m_probabilities. "
@@ -200,15 +203,15 @@
 
     @property
     def u_probabilities(self):
         return getattr(self, "_u_probabilities", None)
 
     @u_probabilities.setter
     @final
-    def u_probabilities(self, u_probabilities: List[float]):
+    def u_probabilities(self, u_probabilities: List[float]) -> None:
         if u_probabilities:
             num_probs_supplied = len(u_probabilities)
             num_non_null_levels = self.num_non_null_levels
             if num_probs_supplied != self.num_non_null_levels:
                 raise ValueError(
                     f"Comparison has {num_non_null_levels} non-null levels, "
                     f"but received {num_probs_supplied} values for u_probabilities. "
```

### Comparing `splink-4.0.0.dev3/splink/comparison_helpers.py` & `splink-4.0.0.dev4/splink/comparison_helpers.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/comparison_level.py` & `splink-4.0.0.dev4/splink/comparison_level.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import logging
 import math
 import re
 from copy import copy
 from statistics import median
 from textwrap import dedent
-from typing import Any, Optional
+from typing import Any, Optional, Union, cast
 
 import sqlglot
-from sqlglot.expressions import Identifier
+from sqlglot.expressions import Column, Identifier
 from sqlglot.optimizer.normalize import normalize
 from sqlglot.optimizer.simplify import simplify
 
 from .constants import LEVEL_NOT_OBSERVED_TEXT
 from .input_column import InputColumn
 from .misc import (
     dedupe_preserving_order,
@@ -29,65 +29,58 @@
 
 def _is_exact_match(sql_syntax_tree):
     signature = sqlglot_tree_signature(sql_syntax_tree)
 
     if signature != sqlglot_tree_signature(sqlglot.parse_one("col_l = col_r")):
         return False
 
-    identifiers = []
-    for tup in sql_syntax_tree.walk():
-        subtree = tup[0]
-        if type(subtree) is Identifier:
-            identifiers.append(subtree.this[:-2])
-    if identifiers[0] == identifiers[1]:
+    cols = [s.output_name for s in sql_syntax_tree.find_all(Column)]
+    cols_truncated = [c[:-2] for c in cols]
+    if cols_truncated[0] == cols_truncated[1]:
         return True
     else:
         return False
 
 
 def _exact_match_colname(sql_syntax_tree):
     # only interested in expression directly, not context
     sql_syntax_tree.parent = None
     cols = []
 
     for identifier in sql_syntax_tree.find_all(Identifier):
         identifier.args["quoted"] = False
 
-    for tup in sql_syntax_tree.walk():
-        subtree = tup[0]
-        depth = getattr(subtree, "depth", None)
-        if depth == 2:
-            cols.append(subtree.sql())
+    cols = [id.sql() for id in sql_syntax_tree.find_all(Identifier) if id.depth == 2]
 
     cols = [c[:-2] for c in cols]  # Remove _l and _r
     cols = list(set(cols))
     if len(cols) != 1:
         raise ValueError(
             f"Expected sql condition to refer to one column but got {cols}"
         )
     return cols[0]
 
 
-def _get_and_subclauses(expr: sqlglot.Expression):
+def _get_and_subclauses(expr: sqlglot.Expression) -> list[sqlglot.Expression]:
     # get list of subclauses joined together by 'AND' at top-level
     # e.g. 'A AND B AND C' -> ['A', 'B', 'C']
     # or if no AND, return expression as a list, e.g. 'A' -> ['A']
     if isinstance(expr, sqlglot.exp.And):
         return list(expr.flatten())
     return [expr]
 
 
-def _default_m_values(num_levels):
+def _default_m_values(num_levels: int) -> list[float]:
     proportion_exact_match = 0.95
     remainder = 1 - proportion_exact_match
     split_remainder = remainder / (num_levels - 1)
     return [split_remainder] * (num_levels - 1) + [proportion_exact_match]
 
 
-def _default_u_values(num_levels):
+def _default_u_values(num_levels: int) -> list[float]:
     m_vals = _default_m_values(num_levels)
     if num_levels == 2:
         match_weights = [-5]
     else:
         match_weights = interpolate(-5, 3, num_levels - 1)
     match_weights = match_weights + [10]
 
@@ -141,38 +134,41 @@
         label_for_charts: str = None,
         is_null_level: bool = False,
         tf_adjustment_column: str = None,
         tf_adjustment_weight: float = 1.0,
         tf_minimum_u_value: float = 0.0,
         m_probability: float = None,
         u_probability: float = None,
+        disable_tf_exact_match_detection: bool = False,
     ):
         self._sqlglot_dialect_name = sqlglot_dialect_name
 
         self._sql_condition = sql_condition
         self._is_null_level = is_null_level
         self._label_for_charts = label_for_charts
 
         self._tf_adjustment_column = tf_adjustment_column
         self._tf_adjustment_weight = tf_adjustment_weight
         self._tf_minimum_u_value = tf_minimum_u_value
+        self._disable_tf_exact_match_detection = disable_tf_exact_match_detection
 
-        self._m_probability = m_probability
-        self._u_probability = u_probability
-        self.default_m_probability = None
-        self.default_u_probability = None
+        # internally these can be LEVEL_NOT_OBSERVED_TEXT, so allow for this
+        self._m_probability: float | None | str = m_probability
+        self._u_probability: float | None | str = u_probability
+        self.default_m_probability: float | None = None
+        self.default_u_probability: float | None = None
 
         # TODO: control this in comparison getter setter ?
         # These will be set when the ComparisonLevel is passed into a Comparison
         self._comparison_vector_value: Optional[int] = None
         self._max_level: Optional[bool] = None
 
         # Enable the level to 'know' when it's been trained
-        self._trained_m_probabilities: list = []
-        self._trained_u_probabilities: list = []
+        self._trained_m_probabilities: list[dict[str, Any]] = []
+        self._trained_u_probabilities: list[dict[str, Any]] = []
         # controls warnings from model training - ensures we only send once
         self._m_warning_sent = False
         self._u_warning_sent = False
 
         self._validate()
 
     def copy(self):
@@ -185,14 +181,18 @@
         return self._sqlglot_dialect_name
 
     @property
     def is_null_level(self) -> bool:
         return self._is_null_level
 
     @property
+    def disable_tf_exact_match_detection(self) -> bool:
+        return self._disable_tf_exact_match_detection
+
+    @property
     def sql_condition(self) -> str:
         return self._sql_condition
 
     @property
     def _tf_adjustment_input_column(self):
         val = self._tf_adjustment_column
         if val:
@@ -203,42 +203,44 @@
     @property
     def _tf_adjustment_input_column_name(self):
         input_column = self._tf_adjustment_input_column
         if input_column:
             return input_column.unquote().name
 
     @property
-    def m_probability(self):
+    def m_probability(self) -> float | None:
         if self.is_null_level:
-            return None
+            raise ValueError("Null levels have no m-probability")
         if self._m_probability == LEVEL_NOT_OBSERVED_TEXT:
             return 1e-6
-        if self._m_probability is None and self.default_m_probability is not None:
+        m_probability = cast(Union[float, None], self._m_probability)
+        if m_probability is None and self.default_m_probability is not None:
             return self.default_m_probability
-        return self._m_probability
+        return m_probability
 
     @m_probability.setter
-    def m_probability(self, value):
+    def m_probability(self, value: float) -> None:
         if self.is_null_level:
             raise AttributeError("Cannot set m_probability when is_null_level is true")
 
         self._m_probability = value
 
     @property
-    def u_probability(self):
+    def u_probability(self) -> float | None:
         if self.is_null_level:
-            return None
+            raise ValueError("Null levels have no u-probability")
         if self._u_probability == LEVEL_NOT_OBSERVED_TEXT:
             return 1e-6
-        if self._u_probability is None and self.default_m_probability is not None:
+        u_probability = cast(Union[float, None], self._u_probability)
+        if u_probability is None and self.default_u_probability is not None:
             return self.default_u_probability
-        return self._u_probability
+        return u_probability
 
     @u_probability.setter
-    def u_probability(self, value):
+    def u_probability(self, value: float) -> None:
         if self.is_null_level:
             raise AttributeError("Cannot set u_probability when is_null_level is true")
         self._u_probability = value
 
     @property
     def _m_probability_description(self):
         if self.m_probability is not None:
@@ -359,38 +361,47 @@
             return f"{text} {self._bayes_factor:,.2f} times more likely to be a match"
         else:
             mult = 1 / self._bayes_factor
             return f"{text}  {mult:,.2f} times less likely to be a match"
 
     @property
     def label_for_charts(self):
-        return self._label_for_charts or str(self._comparison_vector_value)
+        return self._label_for_charts or str(self.comparison_vector_value)
 
     def _label_for_charts_no_duplicates(
         self, comparison_levels: list[ComparisonLevel] = None
-    ):
+    ) -> str:
         if comparison_levels is not None:
             labels = []
             for cl in comparison_levels:
                 labels.append(cl.label_for_charts)
 
         if len(labels) == len(set(labels)):
             return self.label_for_charts
 
         # Make label unique
-        cvv = str(self._comparison_vector_value)
+        cvv = str(self.comparison_vector_value)
         label = self.label_for_charts
         return f"{cvv}. {label}"
 
     @property
     def _is_else_level(self):
         if self.sql_condition.strip().upper() == "ELSE":
             return True
 
     @property
+    def comparison_vector_value(self) -> int:
+        if (cvv := self._comparison_vector_value) is not None:
+            return cvv
+        raise ValueError(
+            "To access a `comparison_vector_value`, a `ComparisonLevel` must "
+            "belong to a `Comparison`"
+        )
+
+    @property
     def _has_tf_adjustments(self):
         col = self._tf_adjustment_column
         return col is not None
 
     def _validate_sql(self):
         sql = self.sql_condition
         if self._is_else_level:
@@ -447,17 +458,17 @@
             raise ValueError(
                 "Cannot get the 'when .. then ...' sql expression because "
                 "this comparison level does not belong to a parent Comparison. "
                 "The comparison_vector_value is only defined in the "
                 "context of a list of ComparisonLevels within a Comparison."
             )
         if self._is_else_level:
-            return f"{self.sql_condition} {self._comparison_vector_value}"
+            return f"{self.sql_condition} {self.comparison_vector_value}"
         else:
-            return f"WHEN {self.sql_condition} THEN {self._comparison_vector_value}"
+            return f"WHEN {self.sql_condition} THEN {self.comparison_vector_value}"
 
     @property
     def _is_exact_match(self):
         if self._is_else_level:
             return False
 
         sql_syntax_tree = sqlglot.parse_one(
@@ -489,53 +500,59 @@
         for expr in exprs:
             col = _exact_match_colname(expr)
             cols.append(col)
         return cols
 
     def _u_probability_corresponding_to_exact_match(
         self, comparison_levels: list[ComparisonLevel]
-    ):
+    ) -> float | None:
+        if self.disable_tf_exact_match_detection:
+            return self.u_probability
+
+        # otherwise, default to looking for an appropriate exact match level:
+
         # Find a level with a single exact match colname
         # which is equal to the tf adjustment input colname
 
         for level in comparison_levels:
             if not level._is_exact_match:
                 continue
             colnames = level._exact_match_colnames
             if len(colnames) != 1:
                 continue
             if colnames[0] == self._tf_adjustment_input_column_name.lower():
                 return level.u_probability
+
         raise ValueError(
             "Could not find an exact match level for "
             f"{self._tf_adjustment_input_column_name}."
             "\nAn exact match level is required to make a term frequency adjustment "
             "on a comparison level that is not an exact match."
         )
 
-    def _bayes_factor_sql(self, gamma_column_name: str):
+    def _bayes_factor_sql(self, gamma_column_name: str) -> str:
         bayes_factor = (
             self._bayes_factor if self._bayes_factor != math.inf else "'Infinity'"
         )
         sql = f"""
         WHEN
-        {gamma_column_name} = {self._comparison_vector_value}
+        {gamma_column_name} = {self.comparison_vector_value}
         THEN cast({bayes_factor} as float8)
         """
         return dedent(sql)
 
     def _tf_adjustment_sql(
         self, gamma_column_name: str, comparison_levels: list[ComparisonLevel]
-    ):
+    ) -> str:
         gamma_colname_value_is_this_level = (
-            f"{gamma_column_name} = {self._comparison_vector_value}"
+            f"{gamma_column_name} = {self.comparison_vector_value}"
         )
 
         # A tf adjustment of 1D is a multiplier of 1.0, i.e. no adjustment
-        if self._comparison_vector_value == -1:
+        if self.comparison_vector_value == -1:
             sql = f"WHEN  {gamma_colname_value_is_this_level} then cast(1 as float8)"
         elif not self._has_tf_adjustments:
             sql = f"WHEN  {gamma_colname_value_is_this_level} then cast(1 as float8)"
         elif self._tf_adjustment_weight == 0:
             sql = f"WHEN  {gamma_colname_value_is_this_level} then cast(1 as float8)"
         elif self._is_else_level:
             sql = f"WHEN  {gamma_colname_value_is_this_level} then cast(1 as float8)"
@@ -590,77 +607,83 @@
                 ELSE cast(1 as float8)
                 END)
             """
         return dedent(sql).strip()
 
     def as_dict(self):
         "The minimal representation of this level to use as an input to Splink"
-        output = {}
+        output: dict[str, Any] = {}
 
         output["sql_condition"] = self.sql_condition
 
         if self.label_for_charts:
             output["label_for_charts"] = self.label_for_charts
 
         if self._m_probability and self._m_is_trained:
             output["m_probability"] = self.m_probability
 
         if self._u_probability and self._u_is_trained:
             output["u_probability"] = self.u_probability
 
         if self._has_tf_adjustments:
             output["tf_adjustment_column"] = self._tf_adjustment_input_column.input_name
+            if self._tf_minimum_u_value != 0:
+                output["tf_minimum_u_value"] = self._tf_minimum_u_value
             if self._tf_adjustment_weight != 0:
                 output["tf_adjustment_weight"] = self._tf_adjustment_weight
 
         if self.is_null_level:
             output["is_null_level"] = True
 
+        if self._disable_tf_exact_match_detection:
+            output["disable_tf_exact_match_detection"] = True
+
         return output
 
     def _as_completed_dict(self):
         comp_dict = self.as_dict()
-        comp_dict["comparison_vector_value"] = self._comparison_vector_value
+        comp_dict["comparison_vector_value"] = self.comparison_vector_value
         return comp_dict
 
     def _as_detailed_record(
         self, comparison_num_levels: int, comparison_levels: list[ComparisonLevel]
-    ):
+    ) -> dict[str, Any]:
         "A detailed representation of this level to describe it in charting outputs"
         output: dict[str, Any] = {}
         output["sql_condition"] = self.sql_condition
         output["label_for_charts"] = self._label_for_charts_no_duplicates(
             comparison_levels
         )
 
-        output["m_probability"] = self.m_probability
-        output["u_probability"] = self.u_probability
+        if not self._is_null_level:
+            output["m_probability"] = self.m_probability
+            output["u_probability"] = self.u_probability
 
-        output["m_probability_description"] = self._m_probability_description
-        output["u_probability_description"] = self._u_probability_description
+            output["m_probability_description"] = self._m_probability_description
+            output["u_probability_description"] = self._u_probability_description
 
         output["has_tf_adjustments"] = self._has_tf_adjustments
         if self._has_tf_adjustments:
             output["tf_adjustment_column"] = self._tf_adjustment_input_column.input_name
         else:
             output["tf_adjustment_column"] = None
         output["tf_adjustment_weight"] = self._tf_adjustment_weight
 
         output["is_null_level"] = self.is_null_level
         output["bayes_factor"] = self._bayes_factor
         output["log2_bayes_factor"] = self._log2_bayes_factor
-        output["comparison_vector_value"] = self._comparison_vector_value
+        output["comparison_vector_value"] = self.comparison_vector_value
         output["max_comparison_vector_value"] = comparison_num_levels - 1
         output["bayes_factor_description"] = self._bayes_factor_description
 
         return output
 
     def _parameter_estimates_as_records(
         self, comparison_num_levels: int, comparison_levels: list[ComparisonLevel]
-    ):
+    ) -> list[dict[str, Any]]:
         output_records = []
 
         cl_record = self._as_detailed_record(comparison_num_levels, comparison_levels)
         trained_values = self._trained_u_probabilities + self._trained_m_probabilities
         for trained_value in trained_values:
             record = {}
             record["m_or_u"] = trained_value["m_or_u"]
```

### Comparing `splink-4.0.0.dev3/splink/comparison_level_composition.py` & `splink-4.0.0.dev4/splink/comparison_level_composition.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
-from typing import Iterable, Union, final
+from typing import Any, Iterable, Union, final
 
 from .blocking import BlockingRule
 from .comparison_creator import ComparisonLevelCreator
 from .comparison_level import ComparisonLevel
 from .dialects import SplinkDialect
 
 
 def _ensure_is_comparison_level_creator(
-    cl: Union[ComparisonLevelCreator, dict]
+    cl: Union[ComparisonLevelCreator, dict[str, Any]],
 ) -> ComparisonLevelCreator:
     if isinstance(cl, dict):
         from .comparison_level_library import CustomLevel
 
         # TODO: proper dict => level method
         return CustomLevel(**cl)
     if isinstance(cl, ComparisonLevelCreator):
@@ -24,15 +24,17 @@
     )
 
 
 class _Merge(ComparisonLevelCreator):
     _clause: str = ""
 
     @final
-    def __init__(self, *comparison_levels: Union[ComparisonLevelCreator, dict]):
+    def __init__(
+        self, *comparison_levels: Union[ComparisonLevelCreator, dict[str, Any]]
+    ):
         num_levels = len(comparison_levels)
         if num_levels == 0:
             raise ValueError(f"Must provide at least one level to {type(self)}()")
         self.comparison_levels = [
             _ensure_is_comparison_level_creator(cl) for cl in comparison_levels
         ]
         self.is_null_level = all(cl.is_null_level for cl in self.comparison_levels)
@@ -88,15 +90,15 @@
     but with SQL conditions negated with logical "NOY".
 
     Args:
         *comparison_level (ComparisonLevelCreator | dict): This represents the
             comparison level you wish to negate with 'NOT'
     """
 
-    def __init__(self, comparison_level: Union[ComparisonLevelCreator, dict]):
+    def __init__(self, comparison_level: Union[ComparisonLevelCreator, dict[str, Any]]):
         self.comparison_level = _ensure_is_comparison_level_creator(comparison_level)
         # turn null levels into non-null levels, otherwise do nothing
         if self.comparison_level.is_null_level:
             self.is_null_level = False
 
     def create_sql(self, sql_dialect: SplinkDialect) -> str:
         return f"NOT ({self.comparison_level.create_sql(sql_dialect)})"
```

### Comparing `splink-4.0.0.dev3/splink/comparison_level_creator.py` & `splink-4.0.0.dev4/splink/comparison_level_creator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from inspect import signature
-from typing import final
+from typing import Any, final
 
 from .column_expression import ColumnExpression
 from .comparison_level import ComparisonLevel
 from .dialects import SplinkDialect
 
 
 class ComparisonLevelCreator(ABC):
@@ -26,15 +28,15 @@
         sql_dialect = SplinkDialect.from_string(sql_dialect_str)
         return ComparisonLevel(
             sqlglot_dialect_name=sql_dialect.sqlglot_name,
             **self.create_level_dict(sql_dialect_str),
         )
 
     @final
-    def create_level_dict(self, sql_dialect_str: str) -> dict:
+    def create_level_dict(self, sql_dialect_str: str) -> dict[str, Any]:
         sql_dialect = SplinkDialect.from_string(sql_dialect_str)
         level_dict = {
             "sql_condition": self.create_sql(sql_dialect),
             "label_for_charts": self.create_label_for_charts(),
         }
 
         # additional config options get passed only if created via .configure()
@@ -56,14 +58,15 @@
         m_probability: float = None,
         u_probability: float = None,
         tf_adjustment_column: str = None,
         tf_adjustment_weight: float = None,
         tf_minimum_u_value: float = None,
         is_null_level: bool = None,
         label_for_charts: str = None,
+        disable_tf_exact_match_detection: bool = None,
     ) -> "ComparisonLevelCreator":
         """
         Configure the comparison level with options which are common to all
         comparison levels.  The options align to the keys in the json
         specification of a comparison level.  These options are usually not
         needed, but are available for advanced users.
 
@@ -104,24 +107,24 @@
 
     @property
     def is_null_level(self) -> bool:
         return getattr(self, "_is_null_level", False)
 
     @is_null_level.setter
     @final
-    def is_null_level(self, is_null_level: bool):
+    def is_null_level(self, is_null_level: bool) -> None:
         self._is_null_level = is_null_level
 
     @property
     def is_exact_match_level(self) -> bool:
         return getattr(self, "_is_exact_match_level", False)
 
     @is_exact_match_level.setter
     @final
-    def is_exact_match_level(self, is_exact_match_level: bool):
+    def is_exact_match_level(self, is_exact_match_level: bool) -> None:
         self._is_exact_match_level = is_exact_match_level
 
     def __repr__(self) -> str:
         return (
             f"Comparison level generator for {self.create_label_for_charts()}. "
             "Call .get_comparison_level(sql_dialect_str) to instantiate "
             "a ComparisonLevel"
```

### Comparing `splink-4.0.0.dev3/splink/comparison_level_library.py` & `splink-4.0.0.dev4/splink/comparison_level_library.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 from __future__ import annotations
 
-from typing import List, Literal, Union
+from functools import wraps
+from typing import Callable, List, Literal, TypeVar, Union
 
 from sqlglot import TokenError, parse_one
 
 from .column_expression import ColumnExpression
 
 # import composition functions for export
 from .comparison_level_composition import And, Not, Or  # NOQA: F401
 from .comparison_level_creator import ComparisonLevelCreator
 from .comparison_level_sql import great_circle_distance_km_sql
 from .dialects import SplinkDialect
 
+# type aliases:
+T = TypeVar("T", bound=ComparisonLevelCreator)
+CreateSQLFunctionType = Callable[[T, SplinkDialect], str]
 
-def unsupported_splink_dialects(unsupported_dialects: List[str]):
-    def decorator(func):
-        def wrapper(self, splink_dialect: SplinkDialect, *args, **kwargs):
+
+def unsupported_splink_dialects(
+    unsupported_dialects: List[str],
+) -> Callable[[CreateSQLFunctionType[T]], CreateSQLFunctionType[T]]:
+    def decorator(func: CreateSQLFunctionType[T]) -> CreateSQLFunctionType[T]:
+        @wraps(func)
+        def wrapper(self: T, splink_dialect: SplinkDialect) -> str:
             if splink_dialect.name in unsupported_dialects:
                 raise ValueError(
                     f"Dialect {splink_dialect.name} is not supported "
                     f"for {self.__class__.__name__}"
                 )
-            return func(self, splink_dialect, *args, **kwargs)
+            return func(self, splink_dialect)
 
         return wrapper
 
     return decorator
 
 
 def _translate_sql_string(
@@ -181,18 +189,19 @@
         """
         self.col_expression = ColumnExpression.instantiate_if_str(col_name)
         self.term_frequency_adjustments = term_frequency_adjustments
         self.is_exact_match_level = True
 
     @property
     def term_frequency_adjustments(self):
-        return self.tf_adjustment_column is not None
+        # mypy doesn't know about attribute as we use magic in .configure()
+        return self.tf_adjustment_column is not None  # type: ignore [attr-defined]
 
     @term_frequency_adjustments.setter
-    def term_frequency_adjustments(self, term_frequency_adjustments: bool):
+    def term_frequency_adjustments(self, term_frequency_adjustments: bool) -> None:
         if term_frequency_adjustments:
             if not self.col_expression.is_pure_column_or_column_reference:
                 raise ValueError(
                     "The boolean term_frequency_adjustments argument"
                     " can only be used if the column name has no "
                     "transforms applied to it such as lower(), "
                     "substr() etc."
@@ -260,14 +269,15 @@
 
         if self.side_of_comparison == "left":
             return f"{col.name_l} = {dialected}"
         elif self.side_of_comparison == "right":
             return f"{col.name_r} = {dialected}"
         elif self.side_of_comparison == "both":
             return f"{col.name_l} = {dialected}" f" AND {col.name_r} = {dialected}"
+        raise ValueError(f"Invalid `side_of_comparison`: {self.side_of_comparison}.")
 
     def create_label_for_charts(self) -> str:
         return (
             f"{self.col_expression.label} = {self.literal_value_undialected} "
             f"on {self.side_of_comparison}"
         )
 
@@ -569,16 +579,15 @@
         self.time_threshold_seconds = self.convert_time_metric_to_seconds(
             self.time_threshold_raw, self.time_metric
         )
 
         self.datetime_format = datetime_format
         self.input_is_string = input_is_string
 
-    def convert_time_metric_to_seconds(self, threshold: int, metric: str) -> float:
-
+    def convert_time_metric_to_seconds(self, threshold: float, metric: str) -> float:
         conversion_factors = {
             "second": 1,
             "minute": 60,
             "hour": 60 * 60,
             "day": 60 * 60 * 24,
             "month": 60 * 60 * 24 * 365.25 / 12,
             "year": 60 * 60 * 24 * 365.25,
```

### Comparing `splink-4.0.0.dev3/splink/comparison_level_sql.py` & `splink-4.0.0.dev4/splink/comparison_level_sql.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/comparison_library.py` & `splink-4.0.0.dev4/splink/comparison_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from __future__ import annotations
+
 from copy import copy
-from typing import Iterable, List, Union
+from typing import Any, Iterable, List, Optional, Union
 
 from . import comparison_level_library as cll
 from .comparison_creator import ComparisonCreator
 from .comparison_level_creator import ComparisonLevelCreator
 from .comparison_level_library import CustomLevel, DateMetricType
 from .misc import ensure_is_iterable
 
 
 class CustomComparison(ComparisonCreator):
     def __init__(
         self,
-        comparison_levels: List[Union[ComparisonLevelCreator, dict]],
+        comparison_levels: List[Union[ComparisonLevelCreator, dict[str, Any]]],
         output_column_name: str = None,
         comparison_description: str = None,
     ):
         """
         Represents a comparison of the data with custom supplied levels.
 
         Args:
@@ -31,28 +33,31 @@
         self._comparison_levels = comparison_levels
         self._description = comparison_description
         # we deliberately don't call super().__init__() - all that does is set up
         # column expressions, which we do not need here as we are dealing with
         # levels directly
 
     @staticmethod
-    def _convert_to_creator(cl: Union[ComparisonLevelCreator, dict]):
+    def _convert_to_creator(
+        cl: Union[ComparisonLevelCreator, dict[str, Any]],
+    ) -> ComparisonLevelCreator:
         if isinstance(cl, ComparisonLevelCreator):
             return cl
         if isinstance(cl, dict):
             # TODO: swap this if we develop a more uniform approach to (de)serialising
             cl_dict = copy(cl)
             configurable_parameters = (
                 "is_null_level",
                 "m_probability",
                 "u_probability",
                 "tf_adjustment_column",
                 "tf_adjustment_weight",
                 "tf_minimum_u_value",
                 "label_for_charts",
+                "disable_tf_exact_match_detection",
             )
             # split dict in two depending whether or not entries are 'configurables'
             configurables = {
                 key: value
                 for key, value in cl_dict.items()
                 if key in configurable_parameters
             }
@@ -81,15 +86,16 @@
         # TODO: fleshed out default description?
         return (
             self._description
             if self._description is not None
             else f"Comparison for {self._output_column_name}"
         )
 
-    def create_output_column_name(self) -> str:
+    def create_output_column_name(self) -> Optional[str]:
+        # TODO: should default logic be here? would need column-extraction logic also
         return self._output_column_name
 
 
 class ExactMatch(ComparisonCreator):
     """
     Represents a comparison of the data in `col_name` with two levels:
         - Exact match in `col_name`
@@ -390,15 +396,15 @@
         return self.col_expression.output_column_name
 
 
 class DistanceFunctionAtThresholds(ComparisonCreator):
     def __init__(
         self,
         col_name: str,
-        distance_function_name,
+        distance_function_name: str,
         distance_threshold_or_thresholds: Union[Iterable[float], float],
         higher_is_more_similar: bool = True,
     ):
         """
         Represents a comparison of the data in `col_name` with three or more levels:
             - Exact match in `col_name`
             - Custom distance function levels at specified thresholds
@@ -463,16 +469,16 @@
         self,
         col_name: str,
         *,
         input_is_string: bool,
         metrics: Union[DateMetricType, List[DateMetricType]],
         thresholds: Union[int, float, List[Union[int, float]]],
         datetime_format: str = None,
-        term_frequency_adjustments=False,
-        invalid_dates_as_null=True,
+        term_frequency_adjustments: bool = False,
+        invalid_dates_as_null: bool = True,
     ):
         """Invalid dates as null does nothing if input is not a string"""
         time_metrics_as_iterable = ensure_is_iterable(metrics)
         # unpack it to a list so we can repeat iteration if needed
         self.time_metrics = [*time_metrics_as_iterable]
 
         time_thresholds_as_iterable = ensure_is_iterable(thresholds)
```

### Comparing `splink-4.0.0.dev3/splink/comparison_template_library.py` & `splink-4.0.0.dev4/splink/comparison_template_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,26 @@
-from typing import List, Union
+from __future__ import annotations
+
+from typing import List, Type, Union
 
 from . import comparison_level_library as cll
 from .column_expression import ColumnExpression
 from .comparison_creator import ComparisonCreator
 from .comparison_level_creator import ComparisonLevelCreator
 from .comparison_level_library import DateMetricType
 from .misc import ensure_is_iterable
 
-_fuzzy_levels = {
+# alternatively we could stick an inheritance layer in these, just for typing:
+_fuzzy_cll_type = Union[
+    Type[cll.DamerauLevenshteinLevel],
+    Type[cll.JaroLevel],
+    Type[cll.JaroWinklerLevel],
+    Type[cll.LevenshteinLevel],
+]
+_fuzzy_levels: dict[str, _fuzzy_cll_type] = {
     "damerau_levenshtein": cll.DamerauLevenshteinLevel,
     "jaro": cll.JaroLevel,
     "jaro_winkler": cll.JaroWinklerLevel,
     "levenshtein": cll.LevenshteinLevel,
 }
 # metric names single quoted and comma-separated for error messages
 _AVAILABLE_METRICS_STRING = ", ".join(map(lambda x: f"'{x}'", _fuzzy_levels.keys()))
@@ -41,15 +50,14 @@
         input_is_string: bool,
         datetime_format: str = None,
         invalid_dates_as_null: bool = False,
         include_exact_match_level: bool = True,
         separate_1st_january: bool = False,
         use_damerau_levenshtein: bool = True,
     ):
-
         date_thresholds_as_iterable = ensure_is_iterable(datetime_thresholds)
         self.datetime_thresholds = [*date_thresholds_as_iterable]
         date_metrics_as_iterable = ensure_is_iterable(datetime_metrics)
         self.datetime_metrics = [*date_metrics_as_iterable]
 
         num_metrics = len(self.datetime_metrics)
         num_thresholds = len(self.datetime_thresholds)
@@ -75,21 +83,20 @@
         super().__init__(col_name)
 
     @property
     def datetime_parse_function(self):
         return self.col_expression.try_parse_date
 
     def create_comparison_levels(self) -> List[ComparisonLevelCreator]:
-
         if self.invalid_dates_as_null:
             null_col = self.datetime_parse_function(self.datetime_format)
         else:
             null_col = self.col_expression
 
-        levels = [
+        levels: list[ComparisonLevelCreator] = [
             cll.NullLevel(null_col),
         ]
 
         if self.separate_1st_january:
             # Ensure date in isoformat:
             if self.input_is_string:
                 date_as_iso_string = self.datetime_parse_function(
@@ -140,15 +147,14 @@
                     )
                 )
 
         levels.append(cll.ElseLevel())
         return levels
 
     def create_description(self) -> str:
-
         comparison_desc = "Exact match "
         if self.separate_1st_january:
             comparison_desc += "(with separate 1st Jan) "
         comparison_desc += "vs. "
 
         if self.use_damerau_levenshtein:
             comparison_desc += "Damerau-Levenshtein distance <= 1 vs. "
@@ -204,15 +210,15 @@
     def __init__(
         self,
         col_name: Union[str, ColumnExpression],
         *,
         include_exact_match_level: bool = True,
         phonetic_col_name: Union[str, ColumnExpression] = None,
         fuzzy_metric: str = "jaro_winkler",
-        fuzzy_thresholds: Union[float, list] = [0.9, 0.8],
+        fuzzy_thresholds: Union[float, list[float]] = [0.9, 0.8],
     ):
         fuzzy_thresholds_as_iterable = ensure_is_iterable(fuzzy_thresholds)
         self.fuzzy_thresholds = [*fuzzy_thresholds_as_iterable]
 
         self.exact_match = include_exact_match_level
 
         if self.fuzzy_thresholds:
@@ -233,15 +239,15 @@
         else:
             self.phonetic_col = False
         super().__init__(cols)
 
     def create_comparison_levels(self) -> List[ComparisonLevelCreator]:
         name_col_expression = self.col_expressions["name"]
 
-        levels = [
+        levels: list[ComparisonLevelCreator] = [
             cll.NullLevel(name_col_expression),
         ]
         if self.exact_match:
             levels.append(cll.ExactMatchLevel(name_col_expression))
         if self.phonetic_col:
             phonetic_col_expression = self.col_expressions["phonetic_name"]
             levels.append(cll.ExactMatchLevel(phonetic_col_expression))
@@ -339,15 +345,15 @@
             self.phonetic_match = False
         super().__init__(cols)
 
     def create_comparison_levels(self) -> List[ComparisonLevelCreator]:
         forename_col_expression = self.col_expressions["forename"]
         surname_col_expression = self.col_expressions["surname"]
 
-        levels = [
+        levels: list[ComparisonLevelCreator] = [
             cll.And(
                 cll.NullLevel(forename_col_expression),
                 cll.NullLevel(surname_col_expression),
             )
         ]
         if self.exact_match:
             levels.append(
@@ -446,20 +452,20 @@
     DISTRICT_REGEX = "^[A-Za-z]{1,2}[0-9][A-Za-z0-9]?"
     AREA_REGEX = "^[A-Za-z]{1,2}"
 
     def __init__(
         self,
         col_name: Union[str, ColumnExpression],
         *,
-        invalid_postcodes_as_null=False,
-        valid_postcode_regex=_VALID_POSTCODE_REGEX,
-        include_full_match_level=True,
-        include_sector_match_level=True,
-        include_district_match_level=True,
-        include_area_match_level=True,
+        invalid_postcodes_as_null: bool = False,
+        valid_postcode_regex: str = _VALID_POSTCODE_REGEX,
+        include_full_match_level: bool = True,
+        include_sector_match_level: bool = True,
+        include_district_match_level: bool = True,
+        include_area_match_level: bool = True,
         lat_col: Union[str, ColumnExpression] = None,
         long_col: Union[str, ColumnExpression] = None,
         km_thresholds: Union[float, List[float]] = [],
     ):
         self.valid_postcode_regex = (
             valid_postcode_regex if invalid_postcodes_as_null else None
         )
@@ -469,25 +475,30 @@
         self.district_match = include_district_match_level
         self.area_match = include_area_match_level
 
         cols = {"postcode": col_name}
         if km_thresholds:
             km_thresholds_as_iterable = ensure_is_iterable(km_thresholds)
             self.km_thresholds = [*km_thresholds_as_iterable]
+            if lat_col is None or long_col is None:
+                raise ValueError(
+                    "If you supply `km_thresholds` you must also provide values for "
+                    "`lat_col` and `long_col`."
+                )
             cols["latitude"] = lat_col
             cols["longitude"] = long_col
         super().__init__(cols)
 
     def create_comparison_levels(self) -> List[ComparisonLevelCreator]:
         full_col_expression = self.col_expressions["postcode"]
         sector_col_expression = full_col_expression.regex_extract(self.SECTOR_REGEX)
         district_col_expression = full_col_expression.regex_extract(self.DISTRICT_REGEX)
         area_col_expression = full_col_expression.regex_extract(self.AREA_REGEX)
 
-        levels = [
+        levels: list[ComparisonLevelCreator] = [
             # Null level accept pattern if not None, otherwise will ignore
             cll.NullLevel(
                 full_col_expression, valid_string_pattern=self.valid_postcode_regex
             ),
         ]
         if self.full_match:
             levels.append(cll.ExactMatchLevel(full_col_expression))
@@ -584,15 +595,15 @@
         super().__init__(col_name)
 
     def create_comparison_levels(self) -> List[ComparisonLevelCreator]:
         full_col_expression = self.col_expression
         username_col_expression = full_col_expression.regex_extract(self.USERNAME_REGEX)
         domain_col_expression = full_col_expression.regex_extract(self.DOMAIN_REGEX)
 
-        levels = [
+        levels: list[ComparisonLevelCreator] = [
             # Null level accept pattern if not None, otherwise will ignore
             cll.NullLevel(
                 full_col_expression, valid_string_pattern=self.valid_email_regex
             ),
         ]
         if self.exact_match:
             levels.append(cll.ExactMatchLevel(full_col_expression))
```

### Comparing `splink-4.0.0.dev3/splink/comparison_vector_distribution.py` & `splink-4.0.0.dev4/splink/comparison_vector_distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import TYPE_CHECKING
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
     from ..linker import Linker
 
 
-def comparison_vector_distribution_sql(linker: Linker):
+def comparison_vector_distribution_sql(linker: Linker) -> str:
     gamma_columns = [c._gamma_column_name for c in linker._settings_obj.comparisons]
     groupby_cols = " , ".join(gamma_columns)
     gam_concat = " || ',' || ".join(gamma_columns)
 
     case_tem = "(case when {g} = -1 then 0 when {g} = 0 then -1 else {g} end)"
     sum_gam = " + ".join([case_tem.format(g=c) for c in gamma_columns])
```

### Comparing `splink-4.0.0.dev3/splink/comparison_vector_values.py` & `splink-4.0.0.dev4/splink/comparison_vector_values.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 def compute_comparison_vector_values_sql(
     columns_to_select_for_comparison_vector_values: list[str],
-    include_clerical_match_score=False,
+    include_clerical_match_score: bool = False,
 ) -> str:
     """Compute the comparison vectors from __splink__df_blocked, the
     dataframe of blocked pairwise record comparisons.
 
     See [the fastlink paper](https://imai.fas.harvard.edu/research/files/linkage.pdf)
     for more details of what is meant by comparison vectors.
     """
```

### Comparing `splink-4.0.0.dev3/splink/connected_components.py` & `splink-4.0.0.dev4/splink/connected_components.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 from __future__ import annotations
 
 import logging
 import time
 from typing import TYPE_CHECKING, Optional
 
+from .input_column import InputColumn
+from .pipeline import CTEPipeline
 from .splink_dataframe import SplinkDataFrame
 from .unique_id_concat import (
     _composite_unique_id_from_edges_sql,
     _composite_unique_id_from_nodes_sql,
 )
 
 if TYPE_CHECKING:
     from .linker import Linker
 
 logger = logging.getLogger(__name__)
 
 
-def _cc_create_nodes_table(linker: "Linker", generated_graph=False):
+def _cc_create_nodes_table(linker: "Linker", generated_graph: bool = False) -> str:
     """SQL to create our connected components nodes table.
 
     From our edges table, create a nodes table.
 
     This captures ALL nodes in our edges representation
     as a single columnar list.
 
@@ -55,15 +57,15 @@
         select {uid_concat} as node_id
         from __splink__df_concat_with_tf
         """
 
     return sql
 
 
-def _cc_generate_neighbours_representation():
+def _cc_generate_neighbours_representation() -> str:
     """SQL to generate all the 'neighbours' of each input node.
 
     The 'neighbour' of a node is any other node that is connected to the original node
     within the graph.  'Connected' means that at the threshold match probability,
     the nodes are considered to be a match (i.e. the nodes are estimated to
     be same entity)
 
@@ -93,15 +95,15 @@
     left join __splink__df_connected_components_df as e_r
         on n.node_id = e_r.unique_id_r
     """
 
     return sql
 
 
-def _cc_generate_initial_representatives_table():
+def _cc_generate_initial_representatives_table() -> str:
     """SQL to generate our initial "representatives" table.
 
     The 'representative' column will eventually become the cluster ID.
 
     As outlined in the paper quoted at the top:
 
     '...begin by choosing for each vertex (node) a representatative by picking the
@@ -123,15 +125,15 @@
     group by node_id
     order by node_id
     """
 
     return sql
 
 
-def _cc_update_neighbours_first_iter():
+def _cc_update_neighbours_first_iter() -> str:
     """SQL to update our neighbours table - first iteration only.
 
     Takes our initial neighbours table, join on the representatives table
     and recalculates the mimumum representative for each node.
 
     This works by joining on the current known representative for each node's
     neighbours.
@@ -154,15 +156,15 @@
         group by neighbours.node_id
         order by neighbours.node_id
     """
 
     return sql
 
 
-def _cc_update_representatives_first_iter():
+def _cc_update_representatives_first_iter() -> str:
     """SQL to update our representatives table - first iteration only.
 
     From here, standardised code can be used inside a while loop,
     as the representatives table no longer needs generating.
 
     This is only used for the first iteration as we
 
@@ -184,16 +186,16 @@
     on n.node_id = repr.node_id
     """
 
     return sql
 
 
 def _cc_generate_representatives_loop_cond(
-    prev_representatives,
-):
+    prev_representatives: str,
+) -> str:
     """SQL for Connected components main loop.
 
     Takes our core neighbours table (this is constant), and
     joins on the current representatives table from the
     previous iteration by joining on information about each node's
     neighbours representatives.
 
@@ -247,16 +249,16 @@
     group by source.node_id
         """
 
     return sql
 
 
 def _cc_update_representatives_loop_cond(
-    prev_representatives,
-):
+    prev_representatives: str,
+) -> str:
     """SQL to update our representatives table - while loop condition.
 
     Reorganises our representatives output generated in
     cc_generate_representatives_loop_cond() and isolates 'rep_match',
     which indicates whether all representatives have 'settled' (i.e.
     no change from previous iteration).
     """
@@ -273,15 +275,15 @@
     left join {prev_representatives} as repr
     on r.node_id = repr.node_id
         """
 
     return sql
 
 
-def _cc_assess_exit_condition(representatives_name):
+def _cc_assess_exit_condition(representatives_name: str) -> str:
     """SQL exit condition for our Connected Components algorithm.
 
     Where 'rep_match' (summarised in 'cc_update_representatives_first_iter')
     it indicates that some nodes still require updating and have not yet
     settled.
     """
 
@@ -293,17 +295,17 @@
 
     return sql
 
 
 def _cc_create_unique_id_cols(
     linker: "Linker",
     concat_with_tf: str,
-    df_predict: str,
+    df_predict: SplinkDataFrame,
     match_probability_threshold: Optional[float],
-):
+) -> SplinkDataFrame:
     """Create SQL to pull unique ID columns for connected components.
 
     Takes the output of linker.predict() and either creates unique IDs for
     our linked dataframes, if we are performing a link job, or pulls out
     the unique ID columns if deduping.
 
     Args:
@@ -318,15 +320,15 @@
 
     Returns:
         SplinkDataFrame: A dataframe containing two sets of unique IDs,
         unique_id_l and unique_id_r.
 
     """
     # Set probability threshold
-    if linker._deterministic_link_mode:
+    if "is_deterministic_link" in df_predict.metadata:
         match_probability_condition = ""
     elif match_probability_threshold is None:
         raise TypeError("Parameter 'match_probability_threshold' is missing or None")
     else:
         match_probability_condition = (
             f"where match_probability >= {match_probability_threshold}"
         )
@@ -337,56 +339,55 @@
     uid_concat_edges = _composite_unique_id_from_edges_sql(uid_cols, None)
 
     # Generate new unique IDs for our linked dataframes.
     sql = f"""
         select
         {uid_concat_edges_l} as unique_id_l,
         {uid_concat_edges_r} as unique_id_r
-        from {df_predict}
+        from {df_predict.physical_name}
         {match_probability_condition}
 
         UNION
 
         select
         {uid_concat_edges} as unique_id_l,
         {uid_concat_edges} as unique_id_r
         from {concat_with_tf}
     """
-
-    return linker._sql_to_splink_dataframe_checking_cache(
-        sql, "__splink__df_connected_components_df"
-    )
+    pipeline = CTEPipeline()
+    pipeline.enqueue_sql(sql, "__splink__df_connected_components_df")
+    return linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
 
 def _exit_query(
-    pairwise_mode=False,
-    df_predict=None,
-    representatives=None,
-    concat_with_tf=None,
-    uid_cols=None,
-    pairwise_filter=False,
-):
-    representatives = representatives.physical_name if representatives else None
-    df_predict = df_predict.physical_name if df_predict else None
-    concat_with_tf = concat_with_tf.physical_name if concat_with_tf else None
+    pairwise_mode: bool,
+    df_predict: SplinkDataFrame,
+    representatives: SplinkDataFrame,
+    concat_with_tf: SplinkDataFrame,
+    uid_cols: list[InputColumn],
+    pairwise_filter: bool,
+) -> str:
+    representatives_name = representatives.physical_name
+    concat_with_tf_name = concat_with_tf.physical_name
 
     if pairwise_mode:
+        df_predict_name = df_predict.physical_name
         uid_concat_l = _composite_unique_id_from_edges_sql(uid_cols, "l", "n")
         uid_concat_r = _composite_unique_id_from_edges_sql(uid_cols, "r", "n")
 
         filter_cond = "where cluster_id_l = cluster_id_r" if pairwise_filter else ""
 
         return f"""
             select
                 n.*,
                 repr_l.representative as cluster_id_l,
                 repr_r.representative as cluster_id_r
-            from {df_predict} as n
+            from {df_predict_name} as n
             left join
-            {representatives} as repr_l
+            {representatives_name} as repr_l
                 on {uid_concat_l} = repr_l.node_id
             left join
             {representatives} as repr_r
                 on {uid_concat_r} = repr_r.node_id
             {filter_cond}
             order by
                 cluster_id_l, cluster_id_r
@@ -394,30 +395,30 @@
 
     else:
         uid_concat = _composite_unique_id_from_nodes_sql(uid_cols, "n")
 
         return f"""
             select
                 c.representative as cluster_id, n.*
-            from {representatives} as c
+            from {representatives_name} as c
 
-            left join {concat_with_tf} as n
+            left join {concat_with_tf_name} as n
             on {uid_concat} = c.node_id
         """
 
 
 def solve_connected_components(
     linker: "Linker",
     edges_table: SplinkDataFrame,
     df_predict: SplinkDataFrame,
     concat_with_tf: SplinkDataFrame,
     pairwise_output: bool = False,
     filter_pairwise_format_for_clusters: bool = False,
     _generated_graph: bool = False,
-):
+) -> SplinkDataFrame:
     """Connected Components main algorithm.
 
     This function helps cluster your linked (or deduped) records
     into single groups, which can then be more easily visualised.
 
     Args:
         linker:
@@ -442,30 +443,33 @@
 
     input_dfs = [edges_table]
     if _generated_graph:
         edges_table.templated_name = "__splink__df_connected_components_df"
     else:
         input_dfs.append(concat_with_tf)
 
+    pipeline = CTEPipeline(input_dfs)
     # Create our initial node and neighbours tables
     sql = _cc_create_nodes_table(linker, _generated_graph)
-    linker._enqueue_sql(sql, "nodes")
+    pipeline.enqueue_sql(sql, "nodes")
     sql = _cc_generate_neighbours_representation()
-    linker._enqueue_sql(sql, "__splink__df_neighbours")
-    neighbours = linker._execute_sql_pipeline(input_dfs)
+    pipeline.enqueue_sql(sql, "__splink__df_neighbours")
+    neighbours = linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
     # Create our initial representatives table
+    pipeline = CTEPipeline([neighbours])
     sql = _cc_generate_initial_representatives_table()
-    linker._enqueue_sql(sql, "representatives")
+    pipeline.enqueue_sql(sql, "representatives")
     sql = _cc_update_neighbours_first_iter()
-    linker._enqueue_sql(sql, "neighbours_first_iter")
+    pipeline.enqueue_sql(sql, "neighbours_first_iter")
     sql = _cc_update_representatives_first_iter()
     # Execute if we have no batching, otherwise add it to our batched process
-    linker._enqueue_sql(sql, "__splink__df_representatives")
-    representatives = linker._execute_sql_pipeline([neighbours])
+    pipeline.enqueue_sql(sql, "__splink__df_representatives")
+
+    representatives = linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
     prev_representatives_table = representatives
 
     # Loop while our representative table still has unsettled nodes
     iteration, root_rows_count = 0, 1
     while root_rows_count > 0:
         start_time = time.time()
         iteration += 1
@@ -475,41 +479,46 @@
         # 1. Update our neighbours table.
         # 2. Join on the representatives table from the previous iteration
         #    to create the "rep_match" column.
         # 3. Assess if our exit condition has been met.
 
         # Generates our representatives table for the next iteration
         # by joining our previous tables onto our neighbours table.
+        pipeline = CTEPipeline([neighbours])
         sql = _cc_generate_representatives_loop_cond(
             prev_representatives_table.physical_name,
         )
-        linker._enqueue_sql(sql, "r")
+        pipeline.enqueue_sql(sql, "r")
         # Update our rep_match column in the representatives table.
         sql = _cc_update_representatives_loop_cond(
             prev_representatives_table.physical_name
         )
 
         repr_name = f"__splink__df_representatives_{iteration}"
 
-        representatives = linker._enqueue_sql(
+        pipeline.enqueue_sql(
             sql,
             repr_name,
         )
 
-        representatives = linker._execute_sql_pipeline([neighbours])
+        representatives = linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
+
+        pipeline = CTEPipeline()
         # Update table reference
         prev_representatives_table.drop_table_from_database_and_remove_from_cache()
         prev_representatives_table = representatives
 
         # Check if our exit condition has been met...
         sql = _cc_assess_exit_condition(representatives.physical_name)
 
-        linker._enqueue_sql(sql, "__splink__df_root_rows")
+        pipeline.enqueue_sql(sql, "__splink__df_root_rows")
 
-        root_rows_df = linker._execute_sql_pipeline(use_cache=False)
+        root_rows_df = linker.db_api.sql_pipeline_to_splink_dataframe(
+            pipeline, use_cache=False
+        )
 
         root_rows = root_rows_df.as_record_dict()
         root_rows_df.drop_table_from_database_and_remove_from_cache()
         root_rows_count = root_rows[0]["count"]
         logger.info(
             f"Completed iteration {iteration}, root rows count {root_rows_count}"
         )
@@ -525,14 +534,12 @@
         pairwise_mode=pairwise_output,
         df_predict=df_predict,
         representatives=representatives,
         concat_with_tf=concat_with_tf,
         uid_cols=uid_cols,
         pairwise_filter=filter_pairwise_format_for_clusters,
     )
-
-    representatives = linker._sql_to_splink_dataframe_checking_cache(
-        exit_query,
-        "__splink__df_representatives",
-    )
+    pipeline = CTEPipeline([representatives])
+    pipeline.enqueue_sql(exit_query, "__splink__df_representatives")
+    representatives = linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
     return representatives
```

### Comparing `splink-4.0.0.dev3/splink/cost_of_blocking_rules.py` & `splink-4.0.0.dev4/splink/cost_of_blocking_rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from __future__ import annotations
+
 import logging
 from typing import Dict, List, Union
 
 logger = logging.getLogger(__name__)
 
 
-def calculate_field_freedom_cost(combination_of_brs: List[Dict]) -> float:
+def calculate_field_freedom_cost(combination_of_brs: List[Dict[str, float]]) -> float:
     """
     We want a higher scores (lower cost) for combinations of blocking rules that allow
     as much variation in each field as possible
 
     e.g.  we don't like combinations of four rules
     that hold first_name and surname constant in 3 out of 4
     and only allows them to vary in one, even if that affords greater
@@ -45,21 +47,21 @@
 
         total_cost = total_cost + cost
 
     return total_cost
 
 
 def calculate_cost_of_combination_of_brs(
-    br_combination: List[Dict],
+    br_combination: List[Dict[str, float]],
     max_comparison_count: int,
     num_equi_join_weight: Union[int, float] = 1,
     field_freedom_weight: Union[int, float] = 1,
     num_brs_weight: Union[int, float] = 1,
     num_comparison_weight: Union[int, float] = 1,
-) -> dict:
+) -> dict[str, float]:
     """
     Calculates the cost for a given combination of blocking rules.
 
     The cost is a weighted sum of the number of equi joins in the rules, the count of
     rules, the number of fields that are allowed to vary, and the number of rows.
 
     Args:
```

### Comparing `splink-4.0.0.dev3/splink/database_api.py` & `splink-4.0.0.dev4/splink/database_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,41 @@
+from __future__ import annotations
+
 import hashlib
 import logging
 import random
 import time
 from abc import ABC, abstractmethod
-from typing import Dict, Generic, List, Optional, TypeVar, Union, final
+from collections.abc import Sequence
+from typing import Any, Dict, Generic, List, Optional, TypeVar, Union, final
 
 import sqlglot
+from pandas import DataFrame as PandasDataFrame
 
 from .cache_dict_with_logging import CacheDictWithLogging
 from .dialects import (
     SplinkDialect,
 )
 from .exceptions import SplinkException
 from .logging_messages import execute_sql_logging_message_info, log_sql
-from .misc import (
-    ascii_uid,
-    parse_duration,
-)
+from .misc import ascii_uid, ensure_is_list, parse_duration
+from .pipeline import CTEPipeline
 from .splink_dataframe import SplinkDataFrame
 
 logger = logging.getLogger(__name__)
 
-
+# minimal acceptable table types
+AcceptableInputTableType = Union[
+    str, PandasDataFrame, List[Dict[str, Any]], Dict[str, Any]
+]
 # a placeholder type. This will depend on the backend subclass - something
 # 'tabley' for that backend, such as duckdb.DuckDBPyRelation or spark.DataFrame
 TablishType = TypeVar("TablishType")
+# general typevar
+T = TypeVar("T")
 
 
 class DatabaseAPI(ABC, Generic[TablishType]):
     sql_dialect: SplinkDialect
     debug_mode: bool = False
     """
     DatabaseAPI class handles _all_ interactions with the database
@@ -95,15 +102,15 @@
     @final
     def _get_table_from_cache_or_db(
         self, table_name_hash: str, output_tablename_templated: str
     ) -> Union[SplinkDataFrame, None]:
         # Certain tables are put in the cache using their templated_name
         # An example is __splink__df_concat_with_tf
         # These tables are put in the cache when they are first calculated
-        # e.g. with _initialise_df_concat_with_tf()
+        # e.g. with compute_df_concat_with_tf()
         # But they can also be put in the cache manually using
         # e.g. register_table_input_nodes_concat_with_tf()
 
         # Look for these 'named' tables in the cache prior
         # to looking for the hashed version s
         if output_tablename_templated in self._intermediate_table_cache:
             return self._intermediate_table_cache.get_with_logging(
@@ -123,17 +130,17 @@
                 output_tablename_templated, table_name_hash
             )
         return None
 
     @final
     def sql_to_splink_dataframe_checking_cache(
         self,
-        sql,
-        output_tablename_templated,
-        use_cache=True,
+        sql: str,
+        output_tablename_templated: str,
+        use_cache: bool = True,
     ) -> SplinkDataFrame:
         # differences from _sql_to_splink_dataframe:
         # this _calculates_ physical name, and
         # handles debug_mode
         # TODO: also maybe caching? but maybe that is even lower down
         to_hash = (sql + self._cache_uid).encode("utf-8")
         hash = hashlib.sha256(to_hash).hexdigest()[:9]
@@ -175,75 +182,71 @@
 
         self._intermediate_table_cache[physical_name] = splink_dataframe
 
         return splink_dataframe
 
     def sql_pipeline_to_splink_dataframe(
         self,
-        pipeline,
-        input_dataframes: List[SplinkDataFrame] = [],
-        use_cache=True,
+        pipeline: CTEPipeline,
+        use_cache: bool = True,
     ) -> SplinkDataFrame:
         """
         Execute a given pipeline using input_dataframes as seeds if provided.
         self.debug_mode controls whether this is CTE or individual tables.
-        pipeline is resest upon completion
+        pipeline is set to spent after execution ensuring it cannot be
+        acidentally reused
         """
 
         if not self.debug_mode:
-            sql_gen = pipeline.generate_pipeline(input_dataframes)
+            sql_gen = pipeline.generate_cte_pipeline_sql()
             output_tablename_templated = pipeline.output_table_name
 
             splink_dataframe = self.sql_to_splink_dataframe_checking_cache(
                 sql_gen,
                 output_tablename_templated,
                 use_cache,
             )
         else:
             # In debug mode, we do not pipeline the sql and print the
             # results of each part of the pipeline
-            for task in pipeline.generate_pipeline_parts(input_dataframes):
+            for cte in pipeline.ctes_pipeline():
                 start_time = time.time()
-                output_tablename = task.output_table_name
-                sql = task.sql
+                output_tablename = cte.output_table_name
+                sql = cte.sql
                 print("------")  # noqa: T201
                 print(  # noqa: T201
                     f"--------Creating table: {output_tablename}--------"
                 )
 
                 splink_dataframe = self.sql_to_splink_dataframe_checking_cache(
                     sql,
                     output_tablename,
                     use_cache=False,
                 )
                 run_time = parse_duration(time.time() - start_time)
                 print(f"Step ran in: {run_time}")  # noqa: T201
 
         # if there is an error the pipeline will not reset, leaving caller to handle
-        pipeline.reset()
+
         return splink_dataframe
 
     @final
     def register_multiple_tables(
         self,
-        input_tables,
+        input_tables: Sequence[AcceptableInputTableType],
         input_aliases: Optional[List[str]] = None,
         overwrite: bool = False,
     ) -> Dict[str, SplinkDataFrame]:
+        input_tables = self.process_input_tables(input_tables)
 
         tables_as_splink_dataframes = {}
         existing_tables = []
 
         if not input_aliases:
-            # If any of the input_tables are strings, this means they refer
-            # to tables that already exist in the database and an alias is not needed
-            input_aliases = [
-                table if isinstance(table, str) else f"__splink__{ascii_uid(8)}"
-                for table in input_tables
-            ]
+            input_aliases = [f"__splink__{ascii_uid(8)}" for table in input_tables]
 
         for table, alias in zip(input_tables, input_aliases):
             if isinstance(table, str):
                 # already registered - this should be a table name
                 continue
             exists = self.table_exists_in_database(alias)
             # if table exists, and we are not overwriting, we have a problem!
@@ -265,82 +268,97 @@
                 self._table_registration(table, alias)
                 table = alias
             sdf = self.table_to_splink_dataframe(alias, table)
             tables_as_splink_dataframes[alias] = sdf
         return tables_as_splink_dataframes
 
     @final
-    def register_table(self, input, table_name, overwrite=False) -> SplinkDataFrame:
+    def register_table(
+        self,
+        input_table: AcceptableInputTableType,
+        table_name: str,
+        overwrite: bool = False,
+    ) -> SplinkDataFrame:
         tables_dict = self.register_multiple_tables(
-            [input], [table_name], overwrite=overwrite
+            [input_table], [table_name], overwrite=overwrite
         )
         return tables_dict[table_name]
 
     def _setup_for_execute_sql(self, sql: str, physical_name: str) -> str:
         # returns sql
         # sensible default:
         self.delete_table_from_database(physical_name)
         sql = f"CREATE TABLE {physical_name} AS {sql}"
         return sql
 
     def _cleanup_for_execute_sql(
-        self, table, templated_name: str, physical_name: str
+        self, table: TablishType, templated_name: str, physical_name: str
     ) -> SplinkDataFrame:
         # sensible default:
         output_df = self.table_to_splink_dataframe(templated_name, physical_name)
         return output_df
 
     @abstractmethod
     def _execute_sql_against_backend(self, final_sql: str) -> TablishType:
         pass
 
-    def delete_table_from_database(self, name: str):
+    def delete_table_from_database(self, name: str) -> None:
         # sensible default:
         drop_sql = f"DROP TABLE IF EXISTS {name}"
         self._execute_sql_against_backend(drop_sql)
 
     @abstractmethod
-    def _table_registration(self, input, table_name: str) -> None:
+    def _table_registration(
+        self, input: AcceptableInputTableType, table_name: str
+    ) -> None:
         """
         Actually register table with backend.
 
         Overwrite if it already exists.
         """
         pass
 
     @abstractmethod
     def table_to_splink_dataframe(
-        self, templated_name, physical_name
+        self, templated_name: str, physical_name: str
     ) -> SplinkDataFrame:
         pass
 
     @abstractmethod
     def table_exists_in_database(self, table_name: str) -> bool:
         """
         Check if table_name exists in the backend
         """
         pass
 
-    def process_input_tables(self, input_tables) -> List:
+    def process_input_tables(
+        self, input_tables: Sequence[AcceptableInputTableType]
+    ) -> Sequence[AcceptableInputTableType]:
         """
         Process list of input tables from whatever form they arrive in to that suitable
         for linker.
         Default just passes through - backends can specialise if desired
         """
+        input_tables = ensure_is_list(input_tables)
         return input_tables
 
     # should probably also be responsible for cache
     # TODO: stick this in a cache-api that lives on this
 
-    def remove_splinkdataframe_from_cache(self, splink_dataframe: SplinkDataFrame):
+    def remove_splinkdataframe_from_cache(
+        self, splink_dataframe: SplinkDataFrame
+    ) -> None:
         keys_to_delete = set()
         for key, df in self._intermediate_table_cache.items():
             if df.physical_name == splink_dataframe.physical_name:
                 keys_to_delete.add(key)
 
         for k in keys_to_delete:
             del self._intermediate_table_cache[k]
 
     def delete_tables_created_by_splink_from_db(self):
         for splink_df in list(self._intermediate_table_cache.values()):
             if splink_df.created_by_splink:
                 splink_df.drop_table_from_database_and_remove_from_cache()
+
+
+DatabaseAPISubClass = DatabaseAPI[Any]
```

### Comparing `splink-4.0.0.dev3/splink/databricks/enable_splink.py` & `splink-4.0.0.dev4/splink/databricks/enable_splink.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/datasets/__init__.py` & `splink-4.0.0.dev4/splink/datasets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import warnings
 from dataclasses import asdict, dataclass
 from math import floor
 from pathlib import Path
 from urllib.request import urlretrieve
 
@@ -159,15 +161,15 @@
                 **asdict(dataset_meta)
             )
 
         attributes["__repr__"] = lambda self: repr_text
         return super().__new__(cls, clsname, bases, attributes)
 
     @classmethod
-    def progress(cls, block_count, block_size, total_size):
+    def progress(cls, block_count: int, block_size: int, total_size: int) -> None:
         prop_done = (block_count * block_size) / total_size
         if prop_done > 1:
             prop_done = 1
         perc = round(prop_done * 100)
         display = f"\r  download progress: {perc} %\t("
         deciles_done = floor(prop_done * 10)
         for i in range(10):
@@ -218,34 +220,34 @@
     def _trim_suffix(self, filename):
         return filename.split(".")[0]
 
     def list_downloaded_datasets(self):
         """Return a list of datasets that have already been pre-downloaded"""
         return [self._trim_suffix(f) for f in self._list_downloaded_data_files()]
 
-    def list_all_datasets(self):
+    def list_all_datasets(self) -> list[str]:
         """Return a list of all available datasets, regardless of whether
         or not they have already been pre-downloaded
         """
         return [d.dataset_name for d in _datasets]
 
-    def list_all_dataset_labels(self):
+    def list_all_dataset_labels(self) -> list[str]:
         """Return a list of all available dataset labels, regardless of whether
         or not they have already been pre-downloaded
         """
         return [d.dataset_name for d in _labels]
 
-    def show_downloaded_data(self):
+    def show_downloaded_data(self) -> None:
         """Print a list of datasets that have already been pre-downloaded"""
         print(  # noqa: T201
             "Datasets already downloaded and available:\n"
             + ",\n".join(self.list_downloaded_datasets())
         )
 
-    def clear_downloaded_data(self, datasets: list = None):
+    def clear_downloaded_data(self, datasets: list[str] = None) -> None:
         """Delete any pre-downloaded data stored locally.
 
         Args:
             datasets (list): A list of dataset names (without any file suffix)
                 to delete.
                 If `None`, all datasets will be deleted. Default `None`
         """
```

### Comparing `splink-4.0.0.dev3/splink/default_from_jsonschema.py` & `splink-4.0.0.dev4/splink/default_from_jsonschema.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/dialects.py` & `splink-4.0.0.dev4/splink/dialects.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 from abc import ABC, abstractproperty
-from typing import TYPE_CHECKING, Type, final
+from typing import TYPE_CHECKING, Type, TypeVar, final
 
 if TYPE_CHECKING:
     from .comparison_level_library import (
         AbsoluteTimeDifferenceLevel,
         ArrayIntersectLevel,
     )
 
+# equivalent to typing.Self in python >= 3.11
+Self = TypeVar("Self", bound="SplinkDialect")
+
 
 class SplinkDialect(ABC):
     # Stores instances of each subclass of SplinkDialect.
     _dialect_instances: dict[Type[SplinkDialect], SplinkDialect] = {}
     # string defined by subclasses to be used in factory method from_string
     # give a dummy default value so that subclasses that fail to do this
     # don't ruin functionality for existing subclasses
@@ -31,15 +34,15 @@
         pass
 
     @property
     def sqlglot_name(self):
         return self.name
 
     @classmethod
-    def from_string(cls, dialect_name: str):
+    def from_string(cls: type[Self], dialect_name: str) -> Self:
         # list of classes which match _dialect_name_for_factory
         # should just get a single subclass, as this should be unique
         classes_from_dialect_name = [
             c
             for c in cls.__subclasses__()
             if getattr(c, "_dialect_name_for_factory", None) == dialect_name
         ]
@@ -111,42 +114,49 @@
     def _wrap_in_nullif(func):
         def nullif_wrapped_function(*args, **kwargs):
             # convert empty strings to NULL
             return f"NULLIF({func(*args, **kwargs)}, '')"
 
         return nullif_wrapped_function
 
-    def try_parse_date(self, name: str, date_format: str = None):
+    def try_parse_date(self, name: str, date_format: str = None) -> str:
         return self._try_parse_date_raw(name, date_format)
 
-    def _try_parse_date_raw(self, name: str, date_format: str = None):
+    def _try_parse_date_raw(self, name: str, date_format: str = None) -> str:
         raise NotImplementedError(
             f"Backend '{self.name}' does not have a 'try_parse_date' function"
         )
 
-    def try_parse_timestamp(self, name: str, timestamp_format: str = None):
+    def try_parse_timestamp(self, name: str, timestamp_format: str = None) -> str:
         return self._try_parse_timestamp_raw(name, timestamp_format)
 
-    def _try_parse_timestamp_raw(self, name: str, timestamp_format: str = None):
+    def _try_parse_timestamp_raw(self, name: str, timestamp_format: str = None) -> str:
         raise NotImplementedError(
             f"Backend '{self.name}' does not have a 'try_parse_timestamp' function"
         )
 
     @final
-    def regex_extract(self, name: str, pattern: str, capture_group: int = 0):
+    def regex_extract(self, name: str, pattern: str, capture_group: int = 0) -> str:
         return self._wrap_in_nullif(self._regex_extract_raw)(
             name, pattern, capture_group
         )
 
-    def _regex_extract_raw(self, name: str, pattern: str, capture_group: int = 0):
+    def _regex_extract_raw(
+        self, name: str, pattern: str, capture_group: int = 0
+    ) -> str:
         raise NotImplementedError(
             f"Backend '{self.name}' does not have a 'regex_extract' function"
         )
 
-    def explode_arrays_sql(self, tbl_name, columns_to_explode, other_columns_to_retain):
+    def explode_arrays_sql(
+        self,
+        tbl_name: str,
+        columns_to_explode: list[str],
+        other_columns_to_retain: list[str],
+    ) -> str:
         raise NotImplementedError(
             f"Unnesting blocking rules are not supported for {type(self)}"
         )
 
 
 class DuckDBDialect(SplinkDialect):
     _dialect_name_for_factory = "duckdb"
@@ -179,39 +189,41 @@
     def default_date_format(self):
         return "%Y-%m-%d"
 
     @property
     def default_timestamp_format(self):
         return "%Y-%m-%dT%H:%M:%S%Z"
 
-    def _try_parse_date_raw(self, name: str, date_format: str = None):
+    def _try_parse_date_raw(self, name: str, date_format: str = None) -> str:
         if date_format is None:
             date_format = self.default_date_format
         return f"""try_strptime({name}, '{date_format}')"""
 
-    def _try_parse_timestamp_raw(self, name: str, timestamp_format: str = None):
+    def _try_parse_timestamp_raw(self, name: str, timestamp_format: str = None) -> str:
         if timestamp_format is None:
             timestamp_format = self.default_timestamp_format
         return f"""try_strptime({name}, '{timestamp_format}')"""
 
     # TODO: this is only needed for duckdb < 0.9.0.
     # should we just ditch support for that? (only for cll - engine should still work)
-    def array_intersect(self, clc: ArrayIntersectLevel):
+    def array_intersect(self, clc: ArrayIntersectLevel) -> str:
         clc.col_expression.sql_dialect = self
         col = clc.col_expression
         threshold = clc.min_intersection
 
         # sum of individual (unique) array sizes, minus the (unique) union
         return (
             f"list_unique({col.name_l}) + list_unique({col.name_r})"
             f" - list_unique(list_concat({col.name_l}, {col.name_r}))"
             f" >= {threshold}"
         ).strip()
 
-    def _regex_extract_raw(self, name: str, pattern: str, capture_group: int = 0):
+    def _regex_extract_raw(
+        self, name: str, pattern: str, capture_group: int = 0
+    ) -> str:
         return f"regexp_extract({name}, '{pattern}', {capture_group})"
 
     # TODO: roll out to other dialects, at least for now
     @property
     def infinity_expression(self):
         return "cast('infinity' as float8)"
 
@@ -222,15 +234,20 @@
             return ""
         percent = proportion * 100
         if seed:
             return f"USING SAMPLE bernoulli({percent}%) REPEATABLE({seed})"
         else:
             return f"USING SAMPLE {percent}% (bernoulli)"
 
-    def explode_arrays_sql(self, tbl_name, columns_to_explode, other_columns_to_retain):
+    def explode_arrays_sql(
+        self,
+        tbl_name: str,
+        columns_to_explode: list[str],
+        other_columns_to_retain: list[str],
+    ) -> str:
         """Generated sql that explodes one or more columns in a table"""
         columns_to_explode = columns_to_explode.copy()
         other_columns_to_retain = other_columns_to_retain.copy()
         # base case
         if len(columns_to_explode) == 0:
             return f"select {','.join(other_columns_to_retain)} from {tbl_name}"
         else:
@@ -276,25 +293,27 @@
     def default_date_format(self):
         return "yyyy-MM-dd"
 
     @property
     def default_timestamp_format(self):
         return "yyyy-MM-dd\\'T\\'HH:mm:ssXXX"
 
-    def _try_parse_date_raw(self, name: str, date_format: str = None):
+    def _try_parse_date_raw(self, name: str, date_format: str = None) -> str:
         if date_format is None:
             date_format = self.default_date_format
         return f"""to_date({name}, '{date_format}')"""
 
-    def _try_parse_timestamp_raw(self, name: str, timestamp_format: str = None):
+    def _try_parse_timestamp_raw(self, name: str, timestamp_format: str = None) -> str:
         if timestamp_format is None:
             timestamp_format = self.default_timestamp_format
         return f"""to_timestamp({name}, '{timestamp_format}')"""
 
-    def _regex_extract_raw(self, name: str, pattern: str, capture_group: int = 0):
+    def _regex_extract_raw(
+        self, name: str, pattern: str, capture_group: int = 0
+    ) -> str:
         return f"regexp_extract({name}, '{pattern}', {capture_group})"
 
     @property
     def infinity_expression(self):
         return "'infinity'"
 
     def random_sample_sql(
@@ -304,15 +323,20 @@
             return ""
         percent = proportion * 100
         if seed:
             return f" ORDER BY rand({seed}) LIMIT {round(sample_size)}"
         else:
             return f" TABLESAMPLE ({percent} PERCENT) "
 
-    def explode_arrays_sql(self, tbl_name, columns_to_explode, other_columns_to_retain):
+    def explode_arrays_sql(
+        self,
+        tbl_name: str,
+        columns_to_explode: list[str],
+        other_columns_to_retain: list[str],
+    ) -> str:
         """Generated sql that explodes one or more columns in a table"""
         columns_to_explode = columns_to_explode.copy()
         other_columns_to_retain = other_columns_to_retain.copy()
         if len(columns_to_explode) == 0:
             return f"select {','.join(other_columns_to_retain)} from {tbl_name}"
         else:
             column_to_explode = columns_to_explode.pop()
@@ -379,27 +403,29 @@
     def name(self):
         return "postgres"
 
     @property
     def levenshtein_function_name(self):
         return "levenshtein"
 
-    def absolute_time_difference(self, clc: AbsoluteTimeDifferenceLevel):
+    def absolute_time_difference(self, clc: AbsoluteTimeDifferenceLevel) -> str:
         # need custom solution as sqlglot gets confused by 'metric', as in Spark
         # datediff _only_ works in days
         clc.col_expression.sql_dialect = self
         col = clc.col_expression
 
         return (
             f"ABS(EXTRACT(EPOCH FROM {col.name_l}) "
             f"- EXTRACT(EPOCH FROM {col.name_r}))"
             f"<= {clc.time_threshold_seconds}"
         )
 
-    def _regex_extract_raw(self, name: str, pattern: str, capture_group: int = 0):
+    def _regex_extract_raw(
+        self, name: str, pattern: str, capture_group: int = 0
+    ) -> str:
         # full match - wrap pattern in parentheses so first group is whole expression
         if capture_group == 0:
             pattern = f"({pattern})"
         if capture_group > 1:
             # currently no easy way to capture non-first groups
             raise ValueError(
                 "'postgres' backend does not currently support a capture_group greater "
@@ -411,25 +437,25 @@
     def default_date_format(self):
         return "YYYY-MM-DD"
 
     @property
     def default_timestamp_format(self):
         return "YYYY-MM-DDTHH24:MI:SS"
 
-    def try_parse_date(self, name: str, date_format: str = None):
+    def try_parse_date(self, name: str, date_format: str = None) -> str:
         if date_format is None:
             date_format = self.default_date_format
         return f"""try_cast_date({name}, '{date_format}')"""
 
-    def try_parse_timestamp(self, name: str, timestamp_format: str = None):
+    def try_parse_timestamp(self, name: str, timestamp_format: str = None) -> str:
         if timestamp_format is None:
             timestamp_format = self.default_timestamp_format
         return f"""try_cast_timestamp({name}, '{timestamp_format}')"""
 
-    def array_intersect(self, clc: ArrayIntersectLevel):
+    def array_intersect(self, clc: ArrayIntersectLevel) -> str:
         clc.col_expression.sql_dialect = self
         col = clc.col_expression
         threshold = clc.min_intersection
         return f"""
         CARDINALITY(ARRAY_INTERSECT({col.name_l}, {col.name_r})) >= {threshold}
         """.strip()
```

### Comparing `splink-4.0.0.dev3/splink/duckdb/database_api.py` & `splink-4.0.0.dev4/splink/duckdb/database_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from __future__ import annotations
+
 import logging
-from tempfile import TemporaryDirectory
-from typing import Union
+from typing import Sequence, Union
 
 import duckdb
 import pandas as pd
 
-from ..database_api import DatabaseAPI
+from ..database_api import AcceptableInputTableType, DatabaseAPI
 from ..dialects import (
     DuckDBDialect,
 )
 from .dataframe import DuckDBDataFrame
 from .duckdb_helpers.duckdb_helpers import (
     create_temporary_duckdb_connection,
     duckdb_load_from_file,
@@ -19,15 +20,15 @@
 logger = logging.getLogger(__name__)
 
 
 # alias for brevity:
 ddb_con = duckdb.DuckDBPyConnection
 
 
-class DuckDBAPI(DatabaseAPI):
+class DuckDBAPI(DatabaseAPI[duckdb.DuckDBPyRelation]):
     sql_dialect = DuckDBDialect()
 
     def __init__(
         self,
         connection: Union[str, ddb_con] = ":memory:",
         output_schema: str = None,
     ):
@@ -51,59 +52,51 @@
             self._execute_sql_against_backend(
                 f"""
                     CREATE SCHEMA IF NOT EXISTS {output_schema};
                     SET schema '{output_schema}';
                 """
             )
 
-    def delete_table_from_database(self, name: str):
+    def delete_table_from_database(self, name: str) -> None:
         # If the table is in fact a pandas dataframe that's been registered using
         # duckdb con.register() then DROP TABLE will fail with
         # Catalog Error: x is of type View
         try:
             drop_sql = f"DROP TABLE IF EXISTS {name}"
             self._execute_sql_against_backend(drop_sql)
         except duckdb.CatalogException:
             drop_sql = f"DROP VIEW IF EXISTS {name}"
             self._execute_sql_against_backend(drop_sql)
 
-    def _table_registration(self, input, table_name) -> None:
+    def _table_registration(
+        self, input: AcceptableInputTableType, table_name: str
+    ) -> None:
         if isinstance(input, dict):
             input = pd.DataFrame(input)
         elif isinstance(input, list):
             input = pd.DataFrame.from_records(input)
 
         self._con.register(table_name, input)
 
     def table_to_splink_dataframe(
-        self, templated_name, physical_name
+        self, templated_name: str, physical_name: str
     ) -> DuckDBDataFrame:
         return DuckDBDataFrame(templated_name, physical_name, self)
 
     def table_exists_in_database(self, table_name):
         sql = f"PRAGMA table_info('{table_name}');"
-
-        # From duckdb 0.5.0, duckdb will raise a CatalogException
-        # which does not exist in 0.4.0 or before
-
-        # TODO: probably we can drop this compat now?
-        try:
-            from duckdb import CatalogException
-
-            error = (RuntimeError, CatalogException)
-        except ImportError:
-            error = RuntimeError
+        from duckdb import CatalogException
 
         try:
             self._execute_sql_against_backend(sql)
-        except error:
+        except CatalogException:
             return False
         return True
 
-    def load_from_file(self, file_path: str):
+    def load_from_file(self, file_path: str) -> str:
         return duckdb_load_from_file(file_path)
 
     def _execute_sql_against_backend(self, final_sql: str) -> duckdb.DuckDBPyRelation:
         return self._con.sql(final_sql)
 
     @property
     def accepted_df_dtypes(self):
@@ -113,27 +106,14 @@
             import pyarrow as pa
 
             accepted_df_dtypes.append(pa.lib.Table)
         except ImportError:
             pass
         return accepted_df_dtypes
 
-    def process_input_tables(self, input_tables):
+    def process_input_tables(
+        self, input_tables: Sequence[AcceptableInputTableType]
+    ) -> Sequence[AcceptableInputTableType]:
+        input_tables = super().process_input_tables(input_tables)
         return [
             self.load_from_file(t) if isinstance(t, str) else t for t in input_tables
         ]
-
-    # special methods for use:
-
-    def export_to_duckdb_file(self, output_path, delete_intermediate_tables=False):
-        """
-        https://stackoverflow.com/questions/66027598/how-to-vacuum-reduce-file-size-on-duckdb
-        """
-        if delete_intermediate_tables:
-            self._delete_tables_created_by_splink_from_db()
-        with TemporaryDirectory() as tmpdir:
-            self._execute_sql_against_backend(
-                f"EXPORT DATABASE '{tmpdir}' (FORMAT PARQUET);"
-            )
-            new_con = duckdb.connect(database=output_path)
-            new_con.execute(f"IMPORT DATABASE '{tmpdir}';")
-            new_con.close()
```

### Comparing `splink-4.0.0.dev3/splink/duckdb/dataframe.py` & `splink-4.0.0.dev4/splink/duckdb/dataframe.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/duckdb/duckdb_helpers/duckdb_helpers.py` & `splink-4.0.0.dev4/splink/duckdb/duckdb_helpers/duckdb_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     self._temp_dir = tempfile.TemporaryDirectory(dir=".")
     fname = uuid.uuid4().hex[:7]
     path = os.path.join(self._temp_dir.name, f"{fname}.duckdb")
     con = duckdb.connect(database=path, read_only=False)
     return con
 
 
-def duckdb_load_from_file(path):
+def duckdb_load_from_file(path: str) -> str:
     file_functions = {
         ".csv": f"read_csv_auto('{path}')",
         ".parquet": f"read_parquet('{path}')",
     }
     file_ext = Path(path).suffix
     if file_ext in file_functions.keys():
         return file_functions[file_ext]
```

### Comparing `splink-4.0.0.dev3/splink/edge_metrics.py` & `splink-4.0.0.dev4/splink/edge_metrics.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     _basic_edge_metrics_sql,
     _bridges_from_igraph_sql,
     _edges_for_igraph_sql,
     _full_bridges_sql,
     _node_mapping_table_sql,
     _truncated_edges_sql,
 )
+from .pipeline import CTEPipeline
 from .splink_dataframe import SplinkDataFrame
 from .unique_id_concat import (
     _composite_unique_id_from_edges_sql,
 )
 
 if TYPE_CHECKING:
     from .linker import Linker
@@ -47,29 +48,30 @@
             linker, df_predict, threshold_match_probability
         )
     return df_edge_metrics
 
 
 def compute_basic_edge_metrics(
     linker: Linker, df_predict: SplinkDataFrame, threshold_match_probability: float
-):
+) -> SplinkDataFrame:
+    pipeline = CTEPipeline()
     sql_info = _truncated_edges_sql(df_predict, threshold_match_probability)
-    linker._enqueue_sql(**sql_info)
+    pipeline.enqueue_sql(**sql_info)
 
     truncated_edges_table_name = sql_info["output_table_name"]
     uid_cols = linker._settings_obj.column_info_settings.unique_id_input_columns
 
     composite_uid_edges_l = _composite_unique_id_from_edges_sql(uid_cols, "l")
     composite_uid_edges_r = _composite_unique_id_from_edges_sql(uid_cols, "r")
     sql_info = _basic_edge_metrics_sql(
         composite_uid_edges_l, composite_uid_edges_r, truncated_edges_table_name
     )
-    linker._enqueue_sql(**sql_info)
+    pipeline.enqueue_sql(**sql_info)
 
-    df_truncated_edges = linker._execute_sql_pipeline()
+    df_truncated_edges = linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
     return df_truncated_edges
 
 
 def compute_igraph_metrics(
     linker: Linker,
     df_node_metrics: SplinkDataFrame,
     df_predict: SplinkDataFrame,
@@ -84,54 +86,57 @@
             "the edge metric 'is_bridge'."
         ) from None
     uid_cols = linker._settings_obj.column_info_settings.unique_id_input_columns
     # need composite unique ids
     composite_uid_edges_l = _composite_unique_id_from_edges_sql(uid_cols, "l")
     composite_uid_edges_r = _composite_unique_id_from_edges_sql(uid_cols, "r")
 
+    pipeline = CTEPipeline()
     # firstly we (arbitrarily) map node ids to 1-indexed integers with no gaps
     # this is how igraph deals with nodes
     sql_infos = _node_mapping_table_sql(df_node_metrics)
-    for sql_info in sql_infos:
-        linker._enqueue_sql(**sql_info)
-    df_node_mappings = linker._execute_sql_pipeline()
+    pipeline.enqueue_list_of_sqls(sql_infos)
+    df_node_mappings = linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
     # we keep only edges at or above relevant threshold
+    pipeline = CTEPipeline()
     sql_info = _truncated_edges_sql(df_predict, threshold_match_probability)
-    linker._enqueue_sql(**sql_info)
-    df_truncated_edges = linker._execute_sql_pipeline()
+    pipeline.enqueue_sql(**sql_info)
+    df_truncated_edges = linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
     # we map the truncated edges to the integer encoding for nodes above,
     # keeping only the list of endpoints
+    pipeline = CTEPipeline()
     sql_info = _edges_for_igraph_sql(
         df_node_mappings,
         df_truncated_edges.physical_name,
         composite_uid_edges_l,
         composite_uid_edges_r,
     )
-    linker._enqueue_sql(**sql_info)
-    edges_for_igraph = linker._execute_sql_pipeline()
+    pipeline.enqueue_sql(**sql_info)
+    edges_for_igraph = linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
     # we will need to manually register a table, so we use the hash from this table
     igraph_edges_hash = edges_for_igraph.physical_name[-9:]
     # NB: for large data we may have to revise this and process in chunks
     df_edges_for_igraph = edges_for_igraph.as_pandas_dataframe()
     # feed our edges to igraph, get the edges which are bridges as a pandas frame,
     # and register this table with our backend
     igraph_df = ig.Graph.DataFrame(df_edges_for_igraph, directed=False)
     bridges_indices = igraph_df.bridges()
     df_bridges_pd = df_edges_for_igraph.iloc[bridges_indices, :]
     df_bridges = linker.register_table(
         df_bridges_pd, f"__splink__bridges_{igraph_edges_hash}"
     )
     # map our bridge edges back to the original node labelling
+    pipeline = CTEPipeline()
     sql_info = _bridges_from_igraph_sql(df_node_mappings, df_bridges)
-    linker._enqueue_sql(**sql_info)
+    pipeline.enqueue_sql(**sql_info)
     # and adjoin edges which are _not_ bridges, labelling them as such
     sql_info = _full_bridges_sql(
         df_truncated_edges,
         sql_info["output_table_name"],
         composite_uid_edges_l,
         composite_uid_edges_r,
     )
-    linker._enqueue_sql(**sql_info)
-    df_edge_metrics = linker._execute_sql_pipeline()
+    pipeline.enqueue_sql(**sql_info)
+    df_edge_metrics = linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
     return df_edge_metrics
```

### Comparing `splink-4.0.0.dev3/splink/em_training_session.py` & `splink-4.0.0.dev4/splink/em_training_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,45 +9,47 @@
     match_weights_interactive_history_chart,
     probability_two_random_records_match_iteration_chart,
 )
 from .comparison import Comparison
 from .comparison_level import ComparisonLevel
 from .comparison_vector_values import compute_comparison_vector_values_sql
 from .constants import LEVEL_NOT_OBSERVED_TEXT
-from .database_api import DatabaseAPI
+from .database_api import DatabaseAPISubClass
 from .exceptions import EMTrainingException
 from .expectation_maximisation import expectation_maximisation
 from .input_column import InputColumn
 from .misc import bayes_factor_to_prob, prob_to_bayes_factor
 from .parse_sql import get_columns_used_from_sql
-from .pipeline import SQLPipeline
+from .pipeline import CTEPipeline
 from .settings import (
     ComparisonAndLevelDict,
     CoreModelSettings,
     Settings,
     TrainingSettings,
 )
+from .vertically_concatenate import compute_df_concat_with_tf
 
 logger = logging.getLogger(__name__)
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
     from .linker import Linker
+    from .splink_dataframe import SplinkDataFrame
 
 
 class EMTrainingSession:
     """Manages training models using the Expectation Maximisation algorithm, and
     holds statistics on the evolution of parameter estimates.  Plots diagnostic charts
     """
 
     def __init__(
         self,
         # TODO: remove linker arg once we unpick the two places we use it
         linker: Linker,
-        db_api: DatabaseAPI,
+        db_api: DatabaseAPISubClass,
         blocking_rule_for_training: BlockingRule,
         core_model_settings: CoreModelSettings,
         training_settings: TrainingSettings,
         unique_id_input_columns: List[InputColumn],
         fix_u_probabilities: bool = False,
         fix_m_probabilities: bool = False,
         fix_probability_two_random_records_match: bool = False,
@@ -83,15 +85,15 @@
             ] = Settings._get_comparison_levels_corresponding_to_training_blocking_rule(  # noqa
                 blocking_rule_sql=blocking_rule_for_training.blocking_rule_sql,
                 sqlglot_dialect_name=self.db_api.sql_dialect.sqlglot_name,
                 comparisons=core_model_settings.comparisons,
             )
 
         # batch together fixed probabilities rather than keep hold of the bools
-        self.training_fixed_probabilities: set = {
+        self.training_fixed_probabilities: set[str] = {
             probability_type
             for (probability_type, fixed) in [
                 ("m", fix_m_probabilities),
                 ("u", fix_u_probabilities),
                 ("lambda", fix_probability_two_random_records_match),
             ]
             if fixed
@@ -110,17 +112,17 @@
                 cc_cols = cc._input_columns_used_by_case_statement
                 cc_cols = [c.input_name for c in cc_cols]
                 if set(br_cols).intersection(cc_cols):
                     comparisons_to_deactivate.append(cc)
         cc_names_to_deactivate = [
             cc.output_column_name for cc in comparisons_to_deactivate
         ]
-        self._comparisons_that_cannot_be_estimated: list[
-            Comparison
-        ] = comparisons_to_deactivate
+        self._comparisons_that_cannot_be_estimated: list[Comparison] = (
+            comparisons_to_deactivate
+        )
 
         filtered_ccs = [
             cc
             for cc in core_model_settings.comparisons
             if cc.output_column_name not in cc_names_to_deactivate
         ]
 
@@ -143,20 +145,20 @@
         # initial params get inserted in training
         self._core_model_settings_history: List[CoreModelSettings] = []
 
     def _training_log_message(self):
         not_estimated = [
             cc.output_column_name for cc in self._comparisons_that_cannot_be_estimated
         ]
-        not_estimated = "".join([f"\n    - {cc}" for cc in not_estimated])
+        not_estimated_str = "".join([f"\n    - {cc}" for cc in not_estimated])
 
         estimated = [
             cc.output_column_name for cc in self.core_model_settings.comparisons
         ]
-        estimated = "".join([f"\n    - {cc}" for cc in estimated])
+        estimated_str = "".join([f"\n    - {cc}" for cc in estimated])
 
         if {"m", "u"}.issubset(self.training_fixed_probabilities):
             raise ValueError("Can't train model if you fix both m and u probabilites")
         elif "u" in self.training_fixed_probabilities:
             mu = "m probabilities"
         elif "m" in self.training_fixed_probabilities:
             mu = "u probabilities"
@@ -165,51 +167,61 @@
 
         blocking_rule = self._blocking_rule_for_training.blocking_rule_sql
 
         logger.info(
             f"Estimating the {mu} of the model by blocking on:\n"
             f"{blocking_rule}\n\n"
             "Parameter estimates will be made for the following comparison(s):"
-            f"{estimated}\n"
+            f"{estimated_str}\n"
             "\nParameter estimates cannot be made for the following comparison(s)"
-            f" since they are used in the blocking rules: {not_estimated}"
+            f" since they are used in the blocking rules: {not_estimated_str}"
         )
 
-    def _comparison_vectors(self):
+    def _comparison_vectors(self) -> SplinkDataFrame:
         self._training_log_message()
 
-        pipeline = SQLPipeline()
-        nodes_with_tf = self._original_linker._initialise_df_concat_with_tf()
+        pipeline = CTEPipeline()
+        nodes_with_tf = compute_df_concat_with_tf(self._original_linker, pipeline)
+        pipeline = CTEPipeline([nodes_with_tf])
 
+        orig_settings = self._original_linker._settings_obj
         sqls = block_using_rules_sqls(
-            self._original_linker, [self._blocking_rule_for_training]
+            input_tablename_l="__splink__df_concat_with_tf",
+            input_tablename_r="__splink__df_concat_with_tf",
+            blocking_rules=[self._blocking_rule_for_training],
+            link_type=orig_settings._link_type,
+            columns_to_select_sql=", ".join(
+                orig_settings._columns_to_select_for_blocking
+            ),
+            source_dataset_input_column=orig_settings.column_info_settings.source_dataset_input_column,
+            unique_id_input_column=orig_settings.column_info_settings.unique_id_input_column,
         )
-        for sql in sqls:
-            pipeline.enqueue_sql(sql["sql"], sql["output_table_name"])
+        pipeline.enqueue_list_of_sqls(sqls)
 
         # repartition after blocking only exists on the SparkAPI
         repartition_after_blocking = getattr(
             self.db_api, "repartition_after_blocking", False
         )
 
         if repartition_after_blocking:
-            df_blocked = self.db_api.sql_pipeline_to_splink_dataframe(
-                pipeline, [nodes_with_tf]
+            df_blocked = self.db_api.sql_pipeline_to_splink_dataframe(pipeline)
+            nodes_with_tf = (
+                self._original_linker._intermediate_table_cache.get_with_logging(
+                    "__splink__df_concat_with_tf"
+                )
             )
-            input_dataframes = [nodes_with_tf, df_blocked]
-        else:
-            input_dataframes = [nodes_with_tf]
+            pipeline = CTEPipeline([nodes_with_tf, df_blocked])
 
         sql = compute_comparison_vector_values_sql(
             self.columns_to_select_for_comparison_vector_values
         )
         pipeline.enqueue_sql(sql, "__splink__df_comparison_vectors")
-        return self.db_api.sql_pipeline_to_splink_dataframe(pipeline, input_dataframes)
+        return self.db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
-    def _train(self, cvv=None) -> CoreModelSettings:
+    def _train(self, cvv: SplinkDataFrame = None) -> CoreModelSettings:
         if cvv is None:
             cvv = self._comparison_vectors()
 
         # check that the blocking rule actually generates _some_ record pairs,
         # if not give the user a helpful message
         if not cvv.as_record_dict(limit=1):
             br_sql = f"`{self._blocking_rule_for_training.blocking_rule_sql}`"
@@ -250,40 +262,40 @@
         # Add m and u values to original settings
         for cc in self.core_model_settings.comparisons:
             orig_cc = original_core_model_settings.get_comparison_by_output_column_name(
                 cc.output_column_name
             )
             for cl in cc._comparison_levels_excluding_null:
                 orig_cl = orig_cc._get_comparison_level_by_comparison_vector_value(
-                    cl._comparison_vector_value
+                    cl.comparison_vector_value
                 )
 
                 if "m" not in self.training_fixed_probabilities:
                     not_observed = LEVEL_NOT_OBSERVED_TEXT
                     if cl._m_probability == not_observed:
                         orig_cl._add_trained_m_probability(not_observed, training_desc)
                         logger.info(
                             f"m probability not trained for {cc.output_column_name} - "
                             f"{cl.label_for_charts} (comparison vector value: "
-                            f"{cl._comparison_vector_value}). This usually means the "
+                            f"{cl.comparison_vector_value}). This usually means the "
                             "comparison level was never observed in the training data."
                         )
                     else:
                         orig_cl._add_trained_m_probability(
                             cl.m_probability, training_desc
                         )
 
                 if "u" not in self.training_fixed_probabilities:
                     not_observed = LEVEL_NOT_OBSERVED_TEXT
                     if cl._u_probability == not_observed:
                         orig_cl._add_trained_u_probability(not_observed, training_desc)
                         logger.info(
                             f"u probability not trained for {cc.output_column_name} - "
                             f"{cl.label_for_charts} (comparison vector value: "
-                            f"{cl._comparison_vector_value}). This usually means the "
+                            f"{cl.comparison_vector_value}). This usually means the "
                             "comparison level was never observed in the training data."
                         )
                     else:
                         orig_cl._add_trained_u_probability(
                             cl.u_probability, training_desc
                         )
         return original_core_model_settings
@@ -329,17 +341,17 @@
             self._core_model_settings_history
         ):
             records = core_model_settings.parameters_as_detailed_records
 
             for r in records:
                 r["iteration"] = iteration
                 # TODO: why lambda from current settings, not history?
-                r[
-                    "probability_two_random_records_match"
-                ] = self.core_model_settings.probability_two_random_records_match
+                r["probability_two_random_records_match"] = (
+                    self.core_model_settings.probability_two_random_records_match
+                )
 
             output_records.extend(records)
         return output_records
 
     @property
     def _lambda_history_records(self):
         output_records = []
```

### Comparing `splink-4.0.0.dev3/splink/exceptions.py` & `splink-4.0.0.dev4/splink/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import List, Union
 
 
 def format_text_as_red(text):
     return f"\033[91m{text}\033[0m"
 
 
@@ -58,15 +60,15 @@
 
     @property
     def errors(self) -> str:
         """Return concatenated error messages."""
 
         return "\n\n".join([f"{e}" for e in self.error_queue])
 
-    def log_error(self, error: Union[list, str, Exception]) -> None:
+    def log_error(self, error: Union[list[Exception], str, Exception]) -> None:
         """
         Log an error or a list of errors.
 
         Args:
             error: An error message, an Exception instance, or a list
                 containing strings or exceptions.
         """
```

### Comparing `splink-4.0.0.dev3/splink/expectation_maximisation.py` & `splink-4.0.0.dev4/splink/expectation_maximisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from __future__ import annotations
 
 import logging
 import time
-from typing import Any, List
+from typing import Any, List, cast
 
 import pandas as pd
 
 from .comparison import Comparison
 from .comparison_level import ComparisonLevel
 from .constants import LEVEL_NOT_OBSERVED_TEXT
-from .database_api import DatabaseAPI
+from .database_api import DatabaseAPISubClass
 from .input_column import InputColumn
 from .m_u_records_to_parameters import m_u_records_to_lookup_dict
-from .pipeline import SQLPipeline
+from .pipeline import CTEPipeline
 from .predict import (
     predict_from_agreement_pattern_counts_sqls,
     predict_from_comparison_vectors_sqls,
 )
 from .settings import CoreModelSettings, TrainingSettings
 from .splink_dataframe import SplinkDataFrame
 
 logger = logging.getLogger(__name__)
 
 
-def count_agreement_patterns_sql(comparisons: List[Comparison]):
+def count_agreement_patterns_sql(comparisons: List[Comparison]) -> str:
     """Count how many times each realized agreement pattern
     was observed across the blocked dataset."""
     gamma_cols = [cc._gamma_column_name for cc in comparisons]
     gamma_cols_expr = ",".join(gamma_cols)
 
     sql = f"""
     select
@@ -38,15 +38,15 @@
     """
 
     return sql
 
 
 def compute_new_parameters_sql(
     estimate_without_term_frequencies: bool, comparisons: List[Comparison]
-):
+) -> str:
     """compute m and u counts from the results of predict"""
     if estimate_without_term_frequencies:
         agreement_pattern_count = "agreement_pattern_count"
     else:
         agreement_pattern_count = "1"
 
     sql_template = """
@@ -112,15 +112,17 @@
     where output_column_name = '_probability_two_random_records_match'
     order by output_column_name, comparison_vector_value asc
     """
 
     return sql
 
 
-def compute_proportions_for_new_parameters_pandas(m_u_df: pd.DataFrame) -> List[dict]:
+def compute_proportions_for_new_parameters_pandas(
+    m_u_df: pd.DataFrame,
+) -> List[dict[str, Any]]:
     data = m_u_df.copy()
     m_prob = "m_probability"
     u_prob = "u_probability"
     data.rename(columns={"m_count": m_prob, "u_count": u_prob}, inplace=True)
 
     random_records = data[
         data.output_column_name == "_probability_two_random_records_match"
@@ -141,37 +143,39 @@
     data.loc[index, u_prob] = u_probs
 
     data = pd.concat([random_records, data])
 
     return data.to_dict("records")
 
 
-def compute_proportions_for_new_parameters(m_u_df: pd.DataFrame) -> List[dict]:
+def compute_proportions_for_new_parameters(
+    m_u_df: pd.DataFrame,
+) -> List[dict[str, Any]]:
     # Execute with duckdb if installed, otherwise default to pandas
     try:
         import duckdb
 
         sql = compute_proportions_for_new_parameters_sql("m_u_df")
         return duckdb.query(sql).to_df().to_dict("records")
     except (ImportError, ModuleNotFoundError):
         return compute_proportions_for_new_parameters_pandas(m_u_df)
 
 
 def populate_m_u_from_lookup(
     training_fixed_probabilities: set[str],
     comparison_level: ComparisonLevel,
     output_column_name: str,
-    m_u_records_lookup,
+    m_u_records_lookup: dict[str, dict[int, Any]],
 ) -> None:
     cl = comparison_level
 
     if "m" not in training_fixed_probabilities:
         try:
             m_probability = m_u_records_lookup[output_column_name][
-                cl._comparison_vector_value
+                cl.comparison_vector_value
             ]["m_probability"]
 
         except KeyError:
             m_probability = LEVEL_NOT_OBSERVED_TEXT
             cc_n = output_column_name
             cl_n = cl.label_for_charts
             if not cl._m_warning_sent:
@@ -182,15 +186,15 @@
                 )
                 cl._m_warning_sent = True
         cl.m_probability = m_probability
 
     if "u" not in training_fixed_probabilities:
         try:
             u_probability = m_u_records_lookup[output_column_name][
-                cl._comparison_vector_value
+                cl.comparison_vector_value
             ]["u_probability"]
 
         except KeyError:
             u_probability = LEVEL_NOT_OBSERVED_TEXT
 
             cc_n = output_column_name
             cl_n = cl.label_for_charts
@@ -204,15 +208,15 @@
 
         cl.u_probability = u_probability
 
 
 def maximisation_step(
     training_fixed_probabilities: set[str],
     core_model_settings: CoreModelSettings,
-    param_records: List[dict],
+    param_records: List[dict[str, Any]],
 ) -> CoreModelSettings:
     core_model_settings = core_model_settings.copy()
 
     m_u_records = []
     for r in param_records:
         if r["output_column_name"] == "_probability_two_random_records_match":
             prop_record = r
@@ -234,15 +238,15 @@
                 m_u_records_lookup,
             )
 
     return core_model_settings
 
 
 def expectation_maximisation(
-    db_api: DatabaseAPI,
+    db_api: DatabaseAPISubClass,
     training_settings: TrainingSettings,
     estimate_without_term_frequencies: bool,
     core_model_settings: CoreModelSettings,
     unique_id_input_columns: List[InputColumn],
     training_fixed_probabilities: set[str],
     df_comparison_vector_values: SplinkDataFrame,
 ) -> List[CoreModelSettings]:
@@ -258,25 +262,22 @@
     sql_dialect = db_api.sql_dialect.name
     sql_infinity_expression = db_api.sql_dialect.infinity_expression
 
     max_iterations = training_settings.max_iterations
     em_convergence = training_settings.em_convergence
     logger.info("")  # newline
 
-    # pipeline to execute the SQL we need to
-    pipeline = SQLPipeline()
-
     if estimate_without_term_frequencies:
         sql = count_agreement_patterns_sql(core_model_settings.comparisons)
+        pipeline = CTEPipeline([df_comparison_vector_values])
         pipeline.enqueue_sql(sql, "__splink__agreement_pattern_counts")
-        agreement_pattern_counts = db_api.sql_pipeline_to_splink_dataframe(
-            pipeline=pipeline, input_dataframes=[df_comparison_vector_values]
-        )
+        agreement_pattern_counts = db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
     for i in range(1, max_iterations + 1):
+        pipeline = CTEPipeline()
         probability_two_random_records_match = (
             core_model_settings.probability_two_random_records_match
         )
         start_time = time.time()
 
         # Expectation step
         if estimate_without_term_frequencies:
@@ -290,30 +291,28 @@
                 unique_id_input_columns=unique_id_input_columns,
                 core_model_settings=core_model_settings,
                 training_mode=True,
                 sql_dialect=sql_dialect,
                 sql_infinity_expression=sql_infinity_expression,
             )
 
-        for sql in sqls:
-            pipeline.enqueue_sql(sql["sql"], sql["output_table_name"])
+        for sql_info in sqls:
+            pipeline.enqueue_sql(sql_info["sql"], sql_info["output_table_name"])
 
         sql = compute_new_parameters_sql(
             estimate_without_term_frequencies,
             core_model_settings.comparisons,
         )
         pipeline.enqueue_sql(sql, "__splink__m_u_counts")
         if estimate_without_term_frequencies:
-            df_params = db_api.sql_pipeline_to_splink_dataframe(
-                pipeline, [agreement_pattern_counts]
-            )
+            pipeline.append_input_dataframe(agreement_pattern_counts)
+            df_params = db_api.sql_pipeline_to_splink_dataframe(pipeline)
         else:
-            df_params = db_api.sql_pipeline_to_splink_dataframe(
-                pipeline, [df_comparison_vector_values]
-            )
+            pipeline.append_input_dataframe(df_comparison_vector_values)
+            df_params = db_api.sql_pipeline_to_splink_dataframe(pipeline)
         param_records = df_params.as_pandas_dataframe()
         param_records = compute_proportions_for_new_parameters(param_records)
 
         df_params.drop_table_from_database_and_remove_from_cache()
 
         core_model_settings = maximisation_step(
             training_fixed_probabilities=training_fixed_probabilities,
@@ -358,15 +357,15 @@
         )
 
     return message
 
 
 def _max_change_in_parameters_comparison_levels(
     core_model_settings_history: List[CoreModelSettings],
-):
+) -> dict[str, Any]:
     previous_iteration = core_model_settings_history[-2]
     this_iteration = core_model_settings_history[-1]
     max_change = -0.1
 
     max_change_levels: dict[str, Any] = {
         "previous_iteration": None,
         "this_iteration": None,
@@ -379,16 +378,22 @@
         this_cc = comparison[1]
         z_cls = zip(prev_cc.comparison_levels, this_cc.comparison_levels)
         for z_cl in z_cls:
             if z_cl[0].is_null_level:
                 continue
             prev_cl = z_cl[0]
             this_cl = z_cl[1]
-            change_m = this_cl.m_probability - prev_cl.m_probability
-            change_u = this_cl.u_probability - prev_cl.u_probability
+
+            prev_m_prob = cast(float, prev_cl.m_probability)
+            this_m_prob = cast(float, this_cl.m_probability)
+            prev_u_prob = cast(float, prev_cl.u_probability)
+            this_u_prob = cast(float, this_cl.u_probability)
+            change_m = this_m_prob - prev_m_prob
+            change_u = this_u_prob - prev_u_prob
+
             change = max(abs(change_m), abs(change_u))
             change_type = (
                 "m_probability" if abs(change_m) > abs(change_u) else "u_probability"
             )
             change_value = change_m if abs(change_m) > abs(change_u) else change_u
             if change > max_change:
                 max_change = change
@@ -405,17 +410,17 @@
     )
 
     if abs(change_probability_two_random_records_match) > max_change:
         max_change = abs(change_probability_two_random_records_match)
         max_change_levels["prev_comparison_level"] = None
         max_change_levels["current_comparison_level"] = None
         max_change_levels["max_change_type"] = "probability_two_random_records_match"
-        max_change_levels[
-            "max_change_value"
-        ] = change_probability_two_random_records_match
+        max_change_levels["max_change_value"] = (
+            change_probability_two_random_records_match
+        )
         max_change_levels["max_abs_change_value"] = abs(
             change_probability_two_random_records_match
         )
 
     max_change_levels["message"] = _max_change_message(max_change_levels)
 
     return max_change_levels
```

### Comparing `splink-4.0.0.dev3/splink/files/DEPENDENCY_LICENSES.txt` & `splink-4.0.0.dev4/splink/files/DEPENDENCY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/accuracy_chart.json` & `splink-4.0.0.dev4/splink/files/chart_defs/accuracy_chart.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/blocking_rule_generated_comparisons.json` & `splink-4.0.0.dev4/splink/files/chart_defs/blocking_rule_generated_comparisons.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9855654761904761%*

 * *Differences: {"'encoding'": "{'y': {'field': 'blocking_rule'}, 'tooltip': {0: {'field': 'blocking_rule'}, 3: "*

 * *               "{'title': 'Total comparisons in Cartesian product'}, delete: [4]}, delete: "*

 * *               "['color']}"}*

```diff
@@ -1,26 +1,19 @@
 {
     "$schema": "https://vega.github.io/schema/vega-lite/v5.9.3.json",
     "data": {
         "values": []
     },
     "encoding": {
-        "color": {
-            "field": "rule",
-            "legend": null,
-            "scale": {
-                "scheme": "category20c"
-            }
-        },
         "order": {
             "field": "cumulative_rows"
         },
         "tooltip": [
             {
-                "field": "rule",
+                "field": "blocking_rule",
                 "title": "SQL Condition",
                 "type": "nominal"
             },
             {
                 "field": "row_count",
                 "format": ",",
                 "title": "Comparisons Generated",
@@ -31,33 +24,28 @@
                 "format": ",",
                 "title": "Cumulative Comparisons",
                 "type": "quantitative"
             },
             {
                 "field": "cartesian",
                 "format": ",",
-                "title": "Cartesian Product of Input Data",
+                "title": "Total comparisons in Cartesian product",
                 "type": "quantitative"
-            },
-            {
-                "field": "reduction_ratio",
-                "title": "Reduction Ratio (cumulative rows/cartesian product)",
-                "type": "nominal"
             }
         ],
         "x": {
             "field": "start",
             "title": "Comparisons Generated by Rule(s)",
             "type": "quantitative"
         },
         "x2": {
             "field": "cumulative_rows"
         },
         "y": {
-            "field": "rule",
+            "field": "blocking_rule",
             "sort": [
                 "-x2"
             ],
             "title": "SQL Blocking Rule"
         }
     },
     "height": {
```

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/comparator_score_chart.json` & `splink-4.0.0.dev4/splink/files/chart_defs/comparator_score_chart.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/comparator_score_threshold_chart.json` & `splink-4.0.0.dev4/splink/files/chart_defs/comparator_score_threshold_chart.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/completeness.json` & `splink-4.0.0.dev4/splink/files/chart_defs/completeness.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/m_u_parameters_interactive_history.json` & `splink-4.0.0.dev4/splink/files/chart_defs/m_u_parameters_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/match_weight_histogram.json` & `splink-4.0.0.dev4/splink/files/chart_defs/match_weight_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/match_weights_interactive_history.json` & `splink-4.0.0.dev4/splink/files/chart_defs/match_weights_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/match_weights_waterfall.json` & `splink-4.0.0.dev4/splink/files/chart_defs/match_weights_waterfall.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/missingness.json` & `splink-4.0.0.dev4/splink/files/chart_defs/missingness.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/parameter_estimate_comparisons.json` & `splink-4.0.0.dev4/splink/files/chart_defs/parameter_estimate_comparisons.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/phonetic_match_chart.json` & `splink-4.0.0.dev4/splink/files/chart_defs/phonetic_match_chart.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/precision_recall.json` & `splink-4.0.0.dev4/splink/files/chart_defs/precision_recall.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/probability_two_random_records_match_iteration.json` & `splink-4.0.0.dev4/splink/files/chart_defs/probability_two_random_records_match_iteration.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/profile_data.json` & `splink-4.0.0.dev4/splink/files/chart_defs/profile_data.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/roc.json` & `splink-4.0.0.dev4/splink/files/chart_defs/roc.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/tf_adjustment_chart.json` & `splink-4.0.0.dev4/splink/files/chart_defs/tf_adjustment_chart.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/threshold_selection_tool.json` & `splink-4.0.0.dev4/splink/files/chart_defs/threshold_selection_tool.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99875%*

 * *Differences: {"'config'": "{'axisX': {'format': '+.0f'}}"}*

```diff
@@ -3,15 +3,15 @@
     "config": {
         "axis": {
             "gridWidth": 0.5,
             "labelFontSize": 12,
             "titleFontSize": 16
         },
         "axisX": {
-            "format": "+",
+            "format": "+.0f",
             "grid": false,
             "offset": 20,
             "values": {
                 "expr": "[-25,-20,-15,-10,-5,0,5,10,15,20,25]"
             }
         },
         "axisY": {
```

### Comparing `splink-4.0.0.dev3/splink/files/chart_defs/unlinkables_chart_def.json` & `splink-4.0.0.dev4/splink/files/chart_defs/unlinkables_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/external_js/d3@7.8.5` & `splink-4.0.0.dev4/splink/files/external_js/d3@7.8.5`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/external_js/stdlib.js@5.8.3` & `splink-4.0.0.dev4/splink/files/external_js/stdlib.js@5.8.3`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/external_js/vega-embed@6.20.2` & `splink-4.0.0.dev4/splink/files/external_js/vega-embed@6.20.2`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/external_js/vega-lite@5.2.0` & `splink-4.0.0.dev4/splink/files/external_js/vega-lite@5.2.0`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/external_js/vega@5.21.0` & `splink-4.0.0.dev4/splink/files/external_js/vega@5.21.0`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/labelling_tool/slt.js` & `splink-4.0.0.dev4/splink/files/labelling_tool/slt.js`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/labelling_tool/template.j2` & `splink-4.0.0.dev4/splink/files/labelling_tool/template.j2`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/settings_jsonschema.json` & `splink-4.0.0.dev4/splink/files/settings_jsonschema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999905809944%*

 * *Differences: {"'properties'": "{'comparisons': {'items': {'properties': {'comparison_levels': {'items': "*

 * *                 "{'properties': {'disable_tf_exact_match_detection': OrderedDict([('title', 'If "*

 * *                 "true, do not seek exact match u-value for TF adjustment'), ('type', 'boolean'), "*

 * *                 "('default', False)])}}}}}}}"}*

```diff
@@ -84,14 +84,19 @@
                                 "label": "else",
                                 "sql_condition": "ELSE"
                             }
                         ],
                         "items": {
                             "additionalProperties": false,
                             "properties": {
+                                "disable_tf_exact_match_detection": {
+                                    "default": false,
+                                    "title": "If true, do not seek exact match u-value for TF adjustment",
+                                    "type": "boolean"
+                                },
                                 "is_null_level": {
                                     "default": false,
                                     "title": "If true, m and u values will not be estimated and instead the match weight will be zero for this column.  See treatment of nulls here on page 356, quote '. Under this MAR assumption, we can simply ignore missing data.': https://imai.fas.harvard.edu/research/files/linkage.pdf",
                                     "type": "boolean"
                                 },
                                 "label_for_charts": {
                                     "examples": [
```

### Comparing `splink-4.0.0.dev3/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar` & `splink-4.0.0.dev4/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar` & `splink-4.0.0.dev4/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar` & `splink-4.0.0.dev4/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/splink_cluster_studio/cluster_template.j2` & `splink-4.0.0.dev4/splink/files/splink_cluster_studio/cluster_template.j2`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/splink_cluster_studio/custom.css` & `splink-4.0.0.dev4/splink/files/splink_cluster_studio/custom.css`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/splink_comparison_viewer/custom.css` & `splink-4.0.0.dev4/splink/files/splink_comparison_viewer/custom.css`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/splink_comparison_viewer/template.j2` & `splink-4.0.0.dev4/splink/files/splink_comparison_viewer/template.j2`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/files/splink_vis_utils/splink_vis_utils.js` & `splink-4.0.0.dev4/splink/files/splink_vis_utils/splink_vis_utils.js`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/find_matches_to_new_records.py` & `splink-4.0.0.dev4/splink/find_matches_to_new_records.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,42 @@
+from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 from .input_column import InputColumn
+from .pipeline import CTEPipeline
 
 if TYPE_CHECKING:
     from .linker import Linker
     from .splink_dataframe import SplinkDataFrame
 
 
 def add_unique_id_and_source_dataset_cols_if_needed(
-    linker: "Linker", new_records_df: "SplinkDataFrame"
-):
-    cols = new_records_df.columns
-    cols = [c.unquote().name for c in cols]
+    linker: "Linker", new_records_df: "SplinkDataFrame", pipeline: CTEPipeline
+) -> CTEPipeline:
+    input_cols: list[InputColumn] = new_records_df.columns
+    cols: list[str] = [c.unquote().name for c in input_cols]
 
     # Add source dataset column to new records if required and not exists
     sds_sel_sql = ""
     if sds_col := linker._settings_obj.column_info_settings.source_dataset_column_name:
-
         if sds_col not in cols:
             sds_sel_sql = f", 'new_record' as {sds_col}"
 
     # Add unique_id column to new records if not exists
     uid_sel_sql = ""
     uid_col_name = linker._settings_obj.column_info_settings.unique_id_column_name
     uid_col = InputColumn(
         uid_col_name,
         column_info_settings=linker._settings_obj.column_info_settings,
         sql_dialect=linker._settings_obj._sql_dialect,
     )
     uid_col_name = uid_col.unquote().name
     if uid_col_name not in cols:
-        uid_sel_sql = f", 'no_id_provided' as {uid_col}"
+        uid_sel_sql = f", 'no_id_provided' as {uid_col.name}"
 
     sql = f"""
         select * {sds_sel_sql} {uid_sel_sql}
         from  __splink__df_new_records_with_tf_before_uid_fix
         """
-    linker._enqueue_sql(sql, "__splink__df_new_records_with_tf")
+    pipeline.enqueue_sql(sql, "__splink__df_new_records_with_tf")
+    return pipeline
```

### Comparing `splink-4.0.0.dev3/splink/graph_metrics.py` & `splink-4.0.0.dev4/splink/graph_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
 from typing import Dict, List
 
 from splink.splink_dataframe import SplinkDataFrame
 
 
 def _truncated_edges_sql(
@@ -90,15 +92,15 @@
     sql_info = {"sql": sql, "output_table_name": "__splink__graph_metrics_nodes"}
     sqls.append(sql_info)
     return sqls
 
 
 def _node_mapping_table_sql(
     df_node_metrics: SplinkDataFrame,
-):
+) -> list[dict[str, str]]:
     """
     Generate SQL to make a table that maps composite_unique_ids to 1-indexed integers.
 
     This is the node-labelling-scheme required by igraph
     """
     nodes_table_name = df_node_metrics.physical_name
     sql_infos = []
@@ -116,15 +118,15 @@
 
 
 def _edges_for_igraph_sql(
     df_node_mappings: SplinkDataFrame,
     truncated_edges_table_name: str,
     composite_uid_edges_l: str,
     composite_uid_edges_r: str,
-):
+) -> dict[str, str]:
     """
     Generate SQL to relabel an edges table using the node relabelling as
     generated by table specified by `_node_mapping_table_sql`
     """
     node_mapping_table_name = df_node_mappings.physical_name
     sql = f"""
         SELECT
@@ -150,15 +152,15 @@
     sql_info = {"sql": sql, "output_table_name": edges_with_mapped_ids_table_name}
     return sql_info
 
 
 def _bridges_from_igraph_sql(
     df_node_mappings: SplinkDataFrame,
     df_bridges: SplinkDataFrame,
-):
+) -> dict[str, str]:
     """
     Generate SQL to relabel an edges table back to the original labelling
     using the node relabelling as generated by table specified by
     `_node_mapping_table_sql` in 'reverse'
     """
     node_mapping_table_name = df_node_mappings.physical_name
     sql = f"""
@@ -188,15 +190,15 @@
 
 
 def _full_bridges_sql(
     df_truncated_edges: SplinkDataFrame,
     bridges_only_table_name: str,
     composite_uid_edges_l: str,
     composite_uid_edges_r: str,
-):
+) -> dict[str, str]:
     """
     Generate SQL to combine a table of only bridges with the remaining (non-bridge)
     edges, and mark them as such
     """
     sql = f"""
         SELECT
             e.{composite_uid_edges_l} AS composite_unique_id_l,
```

### Comparing `splink-4.0.0.dev3/splink/input_column.py` & `splink-4.0.0.dev4/splink/input_column.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from copy import deepcopy
 from dataclasses import dataclass, replace
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Optional, Type
 
 import sqlglot
 import sqlglot.expressions as exp
 
 from .sql_transform import sqlglot_tree_signature
 
 if TYPE_CHECKING:
@@ -71,15 +71,15 @@
         if self._has_key_or_index:
             tree = self._add_key_or_index_to_tree(tree)
         if self.alias:
             return exp.alias_(tree, self.alias, quoted=self.quoted)
         return tree
 
     @property
-    def sql(self):
+    def sql(self) -> str:
         return self.as_sqlglot_tree.sql(dialect=self.sqlglot_dialect)
 
     @classmethod
     def from_raw_column_name_or_column_reference(cls, input_str, sqlglot_dialect):
         def tree_to_sqlglot_column_tree_builder_args(sqlglot_tree, sqlglot_dialect):
             args = {"sqlglot_dialect": sqlglot_dialect, "quoted": True}
             if sqlglot_tree.find(exp.Bracket):
@@ -185,15 +185,15 @@
         self.col_builder: SqlglotColumnTreeBuilder = (
             SqlglotColumnTreeBuilder.from_raw_column_name_or_column_reference(
                 raw_column_name_or_column_reference,
                 sqlglot_dialect=self.sql_dialect,
             )
         )
 
-    def register_dialect(self, sql_dialect: str | None):
+    def register_dialect(self, sql_dialect: str | None) -> None:
         if self.column_info_settings is not None:
             column_info_sql_dialect = self.column_info_settings.sql_dialect
             if sql_dialect is not None:
                 if sql_dialect != column_info_sql_dialect:
                     raise ValueError(
                         f"Mismatched dialect in `InputColumn`: {sql_dialect=}, "
                         f"but `column_info_settings` has dialect: "
@@ -230,24 +230,24 @@
     @property
     def as_base_dialect(self) -> InputColumn:
         input_column_copy = deepcopy(self)
         input_column_copy.sql_dialect = None
         return input_column_copy
 
     @property
-    def name(self):
+    def name(self) -> str:
         return self.col_builder.sql
 
     @property
-    def name_l(self):
+    def name_l(self) -> str:
         new_column_name = self.col_builder.column_name + "_l"
         return replace(self.col_builder, column_name=new_column_name).sql
 
     @property
-    def name_r(self):
+    def name_r(self) -> str:
         new_column_name = self.col_builder.column_name + "_r"
         return replace(self.col_builder, column_name=new_column_name).sql
 
     @property
     def names_l_r(self):
         return [self.name_l, self.name_r]
 
@@ -325,22 +325,22 @@
 
     However, some SQL dialects, use other identifiers e.g. ` in Spark SQL
     """
     start = end = '"'
     if dialect is None:
         return start, end
     try:
-        sqlglot_dialect = sqlglot.Dialect[dialect.lower()]
+        sqlglot_dialect: Type[sqlglot.Dialect] = sqlglot.Dialect[dialect.lower()]
     except KeyError:
         return start, end
     return _get_sqlglot_dialect_quotes(sqlglot_dialect)
 
 
-def _get_sqlglot_dialect_quotes(dialect: sqlglot.Dialect):
+def _get_sqlglot_dialect_quotes(dialect: Type[sqlglot.Dialect]) -> tuple[str, str]:
     try:
-        # For sqlglot >= 16.0.0
-        start = dialect.IDENTIFIER_START  # type: ignore [attr-defined]
-        end = dialect.IDENTIFIER_END  # type: ignore [attr-defined]
+        start = dialect.IDENTIFIER_START
+        end = dialect.IDENTIFIER_END
     except AttributeError:
+        # For sqlglot < 16.0.0
         start = dialect.identifier_start  # type: ignore [attr-defined]
         end = dialect.identifier_end  # type: ignore [attr-defined]
     return start, end
```

### Comparing `splink-4.0.0.dev3/splink/labelling_tool.py` & `splink-4.0.0.dev4/splink/labelling_tool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,41 @@
+from __future__ import annotations
+
 import json
 import logging
 import os
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 import numpy as np
 import pandas as pd
 from jinja2 import Template
 
 from .misc import EverythingEncoder, read_resource
+from .pipeline import CTEPipeline
 from .splink_dataframe import SplinkDataFrame
+from .vertically_concatenate import compute_df_concat_with_tf
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
     from .linker import Linker
 
 logger = logging.getLogger(__name__)
 
 
 def generate_labelling_tool_comparisons(
-    linker: "Linker", unique_id, source_dataset, match_weight_threshold=-4
-):
+    linker: "Linker",
+    unique_id: str,
+    source_dataset: str,
+    match_weight_threshold: float = -4,
+) -> SplinkDataFrame:
     # ensure the tf table exists
-    concat_with_tf = linker._initialise_df_concat_with_tf()
+    pipeline = CTEPipeline()
+    nodes_with_tf = compute_df_concat_with_tf(linker, pipeline)
 
+    pipeline = CTEPipeline([nodes_with_tf])
     settings = linker._settings_obj
 
     source_dataset_condition = ""
 
     if source_dataset is not None:
         sds_col = settings.column_info_settings.source_dataset_column_name
         source_dataset_condition = f"""
@@ -36,33 +45,33 @@
     sql = f"""
     select *
     from __splink__df_concat_with_tf
     where {settings.column_info_settings.unique_id_column_name} = '{unique_id}'
     {source_dataset_condition}
     """
 
-    linker._enqueue_sql(sql, "__splink__df_labelling_tool_record")
-    splink_df = linker._execute_sql_pipeline([concat_with_tf])
+    pipeline.enqueue_sql(sql, "__splink__df_labelling_tool_record")
+    splink_df = linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
     matches = linker.find_matches_to_new_records(
         splink_df.physical_name, match_weight_threshold=match_weight_threshold
     )
 
     return matches
 
 
 def render_labelling_tool_html(
     linker: "Linker",
     df_comparisons: SplinkDataFrame,
-    out_path="labelling_tool.html",
-    view_in_jupyter=False,
-    show_splink_predictions_in_interface=True,
+    out_path: str = "labelling_tool.html",
+    view_in_jupyter: bool = False,
+    show_splink_predictions_in_interface: bool = True,
     overwrite: bool = True,
-):
-    settings: dict = linker._settings_obj.as_dict()
+) -> str:
+    settings: dict[str, Any] = linker._settings_obj.as_dict()
 
     logger.warning(
         "\nWARNING:\n"
         "The Splink labelling tool is still in development, which means some "
         "features may change and there may be bugs.\nYour feedback will help us "
         "improve it. Go to\n"
         "github.com/moj-analytical-services/splink/discussions/new?category=general"
```

### Comparing `splink-4.0.0.dev3/splink/linker.py` & `splink-4.0.0.dev4/splink/linker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,133 +1,124 @@
-from __future__ import annotations  # noqa: I001
+from __future__ import annotations
 
 import json
 import logging
 import os
-import warnings
 from copy import copy, deepcopy
 from pathlib import Path
 from statistics import median
-from typing import Dict, Optional, Union
-
-
-from splink.input_column import InputColumn
-from splink.settings_validation.log_invalid_columns import (
-    InvalidColumnsLogger,
-    SettingsColumnCleaner,
-)
-from splink.settings_validation.valid_types import (
-    _validate_dialect,
-    log_comparison_errors,
-)
+from typing import Any, Dict, List, Optional, Sequence, Union
 
 from .accuracy import (
     prediction_errors_from_label_column,
     prediction_errors_from_labels_table,
     truth_space_table_from_labels_column,
     truth_space_table_from_labels_table,
 )
-from .analyse_blocking import (
-    count_comparisons_from_blocking_rule_pre_filter_conditions_sqls,
-    cumulative_comparisons_generated_by_blocking_rules,
-    number_of_comparisons_generated_by_blocking_rule_post_filters_sql,
-)
 from .blocking import (
     BlockingRule,
     SaltedBlockingRule,
     block_using_rules_sqls,
     blocking_rule_to_obj,
     materialise_exploded_id_tables,
 )
 from .blocking_rule_creator import BlockingRuleCreator
+from .blocking_rule_creator_utils import to_blocking_rule_creator
 from .cache_dict_with_logging import CacheDictWithLogging
 from .charts import (
+    ChartReturnType,
     accuracy_chart,
-    completeness_chart,
-    cumulative_blocking_rule_comparisons_generated,
     match_weights_histogram,
-    missingness_chart,
     parameter_estimate_comparisons,
     precision_recall_chart,
     roc_chart,
     threshold_selection_tool,
     unlinkables_chart,
     waterfall_chart,
 )
-from .cluster_studio import render_splink_cluster_studio_html
+from .cluster_studio import SamplingMethods, render_splink_cluster_studio_html
 from .comparison import Comparison
 from .comparison_level import ComparisonLevel
 from .comparison_vector_distribution import (
     comparison_vector_distribution_sql,
 )
 from .comparison_vector_values import compute_comparison_vector_values_sql
 from .connected_components import (
     _cc_create_unique_id_cols,
     solve_connected_components,
 )
+from .database_api import AcceptableInputTableType, DatabaseAPISubClass
+from .dialects import SplinkDialect
 from .edge_metrics import compute_edge_metrics
-
-from .database_api import DatabaseAPI
 from .em_training_session import EMTrainingSession
 from .estimate_u import estimate_u_values
-from .exceptions import SplinkDeprecated, SplinkException
+from .exceptions import SplinkException
 from .find_brs_with_comparison_counts_below_threshold import (
     find_blocking_rules_below_threshold_comparison_count,
 )
 from .find_matches_to_new_records import add_unique_id_and_source_dataset_cols_if_needed
 from .graph_metrics import (
     GraphMetricsResults,
     _node_degree_sql,
     _size_density_centralisation_sql,
 )
+from .input_column import InputColumn
+from .internals.blocking_analysis import (
+    _cumulative_comparisons_to_be_scored_from_blocking_rules,
+)
 from .labelling_tool import (
     generate_labelling_tool_comparisons,
     render_labelling_tool_html,
 )
 from .m_from_labels import estimate_m_from_pairwise_labels
 from .m_training import estimate_m_values_from_label_column
-from .match_key_analysis import (
-    count_num_comparisons_from_blocking_rules_for_prediction_sql,
-)
 from .match_weights_histogram import histogram_data
 from .misc import (
     ascii_uid,
     bayes_factor_to_prob,
+    ensure_is_iterable,
     ensure_is_list,
     prob_to_bayes_factor,
 )
-from .missingness import completeness_data, missingness_data
 from .optimise_cost_of_brs import suggest_blocking_rules
-from .pipeline import SQLPipeline
+from .pipeline import CTEPipeline
 from .predict import (
-    predict_from_comparison_vectors_sqls_using_settings,
     predict_from_comparison_vectors_sqls,
+    predict_from_comparison_vectors_sqls_using_settings,
 )
-from .profile_data import profile_columns
 from .settings_creator import SettingsCreator
+from .settings_validation.log_invalid_columns import (
+    InvalidColumnsLogger,
+    SettingsColumnCleaner,
+)
+from .settings_validation.valid_types import (
+    _validate_dialect,
+)
 from .splink_comparison_viewer import (
     comparison_viewer_table_sqls,
     render_splink_comparison_viewer_html,
 )
 from .splink_dataframe import SplinkDataFrame
 from .term_frequencies import (
-    _join_tf_to_input_df_sql,
+    _join_new_table_to_df_concat_with_tf_sql,
     colname_to_tf_tablename,
-    compute_all_term_frequencies_sqls,
-    compute_term_frequencies_from_concat_with_tf,
     term_frequencies_for_single_column_sql,
-    term_frequencies_from_concat_with_tf,
     tf_adjustment_chart,
 )
 from .unique_id_concat import (
     _composite_unique_id_from_edges_sql,
     _composite_unique_id_from_nodes_sql,
 )
 from .unlinkables import unlinkables_data
-from .vertically_concatenate import vertically_concatenate_sql
+from .vertically_concatenate import (
+    compute_df_concat_with_tf,
+    enqueue_df_concat,
+    enqueue_df_concat_with_tf,
+    split_df_concat_with_tf_into_two_tables_sqls,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class Linker:
     """The Linker object manages the data linkage process and holds the data linkage
     model.
@@ -137,22 +128,23 @@
 
     The Linker class is intended for subclassing for specific backends, e.g.
     a `DuckDBLinker`.
     """
 
     def __init__(
         self,
-        input_table_or_tables: str | list,
-        settings: SettingsCreator | dict | Path | str,
-        database_api: DatabaseAPI,
+        input_table_or_tables: str | list[str],
+        settings: SettingsCreator | dict[str, Any] | Path | str,
+        database_api: DatabaseAPISubClass,
         set_up_basic_logging: bool = True,
-        input_table_aliases: str | list = None,
+        input_table_aliases: str | list[str] | None = None,
         validate_settings: bool = True,
     ):
-        """Initialise the linker object, which manages the data linkage process and
+        """
+        Initialise the linker object, which manages the data linkage process and
         holds the data linkage model.
 
         Examples:
 
             Dedupe
             ```py
             linker = Linker(df, settings_dict, db_api)
@@ -197,15 +189,14 @@
         if set_up_basic_logging:
             logging.basicConfig(
                 format="%(message)s",
             )
             splink_logger = logging.getLogger("splink")
             splink_logger.setLevel(logging.INFO)
 
-        self._pipeline = SQLPipeline()
         self.db_api = database_api
 
         # TODO: temp hack for compat
         self._intermediate_table_cache: CacheDictWithLogging = (
             self.db_api._intermediate_table_cache
         )
 
@@ -225,39 +216,30 @@
         # by comparisons/ blocking rules etc??
         self._settings_obj = settings_creator.get_settings(
             database_api.sql_dialect.name
         )
 
         # TODO: Add test of what happens if the db_api is for a different backend
         # to the sql_dialect set in the settings dict
-        input_tables = ensure_is_list(input_table_or_tables)
-        input_tables = self.db_api.process_input_tables(input_tables)
 
         self._input_tables_dict = self._register_input_tables(
-            input_tables,
+            input_table_or_tables,
             input_table_aliases,
         )
 
         self._validate_input_dfs()
         self._validate_settings(validate_settings)
         self._em_training_sessions: list[EMTrainingSession] = []
 
-        self._find_new_matches_mode = False
-        self._train_u_using_random_sample_mode = False
-        self._compare_two_records_mode = False
-        self._self_link_mode = False
-        self._analyse_blocking_mode = False
-        self._deterministic_link_mode = False
-
         self.debug_mode = False
 
     def _input_columns(
         self,
-        include_unique_id_col_names=True,
-        include_additional_columns_to_retain=True,
+        include_unique_id_col_names: bool = True,
+        include_additional_columns_to_retain: bool = True,
     ) -> list[InputColumn]:
         """Retrieve the column names from the input dataset(s) as InputColumns
 
         Args:
             include_unique_id_col_names (bool, optional): Whether to include unique ID
                 column names. Defaults to True.
             include_additional_columns_to_retain (bool, optional): Whether to include
@@ -325,115 +307,60 @@
         return self._settings_obj._cache_uid
 
     @_cache_uid.setter
     def _cache_uid(self, value):
         self._settings_obj._cache_uid = value
 
     @property
-    def _input_tablename_l(self):
-        if self._find_new_matches_mode:
-            return "__splink__df_concat_with_tf"
-
-        if self._self_link_mode:
-            return "__splink__df_concat_with_tf"
-
-        if self._compare_two_records_mode:
-            return "__splink__compare_two_records_left_with_tf"
-
-        if self._train_u_using_random_sample_mode:
-            if self._two_dataset_link_only:
-                return "__splink__df_concat_with_tf_sample_left"
-            else:
-                return "__splink__df_concat_with_tf_sample"
-
-        if self._analyse_blocking_mode:
-            return "__splink__df_concat"
-
-        if self._two_dataset_link_only:
-            return "__splink__df_concat_with_tf_left"
-
-        return "__splink__df_concat_with_tf"
-
-    @property
-    def _input_tablename_r(self):
-        if self._find_new_matches_mode:
-            return "__splink__df_new_records_with_tf"
-
-        if self._self_link_mode:
-            return "__splink__df_concat_with_tf"
-
-        if self._compare_two_records_mode:
-            return "__splink__compare_two_records_right_with_tf"
-
-        if self._train_u_using_random_sample_mode:
-            if self._two_dataset_link_only:
-                return "__splink__df_concat_with_tf_sample_right"
-            else:
-                return "__splink__df_concat_with_tf_sample"
-
-        if self._analyse_blocking_mode:
-            return "__splink__df_concat"
-
-        if self._two_dataset_link_only:
-            return "__splink__df_concat_with_tf_right"
-        return "__splink__df_concat_with_tf"
-
-    @property
     def _two_dataset_link_only(self):
         # Two dataset link only join is a special case where an inner join of the
         # two datasets is much more efficient than self-joining the vertically
         # concatenation of all input datasets
-        if self._find_new_matches_mode:
-            return True
-
-        if self._compare_two_records_mode:
-            return True
-
-        if self._analyse_blocking_mode:
-            return False
 
         if (
             len(self._input_tables_dict) == 2
             and self._settings_obj._link_type == "link_only"
         ):
             return True
         else:
             return False
 
     # convenience wrappers:
     @property
-    def debug_mode(self):
+    def debug_mode(self) -> bool:
         return self.db_api.debug_mode
 
     @debug_mode.setter
-    def debug_mode(self, value: bool):
+    def debug_mode(self, value: bool) -> None:
         self.db_api.debug_mode = value
 
     # TODO: rename these!
     @property
-    def _sql_dialect(self):
+    def _sql_dialect(self) -> str:
         return self.db_api.sql_dialect.name
 
     @property
-    def _sql_dialect_object(self):
+    def _sql_dialect_object(self) -> SplinkDialect:
         return self.db_api.sql_dialect
 
     @property
     def _infinity_expression(self):
         return self._sql_dialect_object.infinity_expression
 
     def _random_sample_sql(
         self, proportion, sample_size, seed=None, table=None, unique_id=None
     ):
         return self._sql_dialect_object.random_sample_sql(
             proportion, sample_size, seed=seed, table=table, unique_id=unique_id
         )
 
     def _register_input_tables(
-        self, input_tables, input_aliases
+        self,
+        input_tables: Sequence[AcceptableInputTableType],
+        input_aliases: Optional[str | List[str]],
     ) -> Dict[str, SplinkDataFrame]:
         if input_aliases is None:
             input_table_aliases = [
                 f"__splink__input_table_{i}" for i, _ in enumerate(input_tables)
             ]
             overwrite = True
         else:
@@ -444,153 +371,53 @@
             input_tables, input_table_aliases, overwrite
         )
 
     def _check_for_valid_settings(self):
         # raw tables don't yet exist in db
         return hasattr(self, "_input_tables_dict")
 
-    def _validate_settings_components(self, settings_dict):
-        # Vaidate our settings after plugging them through
-        # `Settings(<settings>)`
-
-        log_comparison_errors(
-            # null if not in dict - check using value is ignored
-            settings_dict.get("comparisons", None),
-            self._sql_dialect,
-        )
-
     def _validate_settings(self, validate_settings):
-        # TODO: restore logic
-        return
         # Vaidate our settings after plugging them through
         # `Settings(<settings>)`
         if not self._check_for_valid_settings():
             return
 
-        self._validate_input_dfs()
-
         # Run miscellaneous checks on our settings dictionary.
         _validate_dialect(
             settings_dialect=self._settings_obj._sql_dialect,
             linker_dialect=self._sql_dialect,
             linker_type=self.__class__.__name__,
         )
 
         # Constructs output logs for our various settings inputs
         cleaned_settings = SettingsColumnCleaner(
             settings_object=self._settings_obj,
             input_columns=self._input_tables_dict,
         )
         InvalidColumnsLogger(cleaned_settings).construct_output_logs(validate_settings)
 
-    def _initialise_df_concat(self, materialise=False):
-        cache = self._intermediate_table_cache
-        concat_df = None
-        if "__splink__df_concat" in cache:
-            concat_df = cache.get_with_logging("__splink__df_concat")
-        elif "__splink__df_concat_with_tf" in cache:
-            concat_df = cache.get_with_logging("__splink__df_concat_with_tf")
-            concat_df.templated_name = "__splink__df_concat"
-        else:
-            if materialise:
-                # Clear the pipeline if we are materialising
-                # There's no reason not to do this, since when
-                # we execute the pipeline, it'll get cleared anyway
-                self._pipeline.reset()
-            sql = vertically_concatenate_sql(self)
-            self._enqueue_sql(sql, "__splink__df_concat")
-            if materialise:
-                concat_df = self._execute_sql_pipeline()
-                cache["__splink__df_concat"] = concat_df
-
-        return concat_df
-
-    def _initialise_df_concat_with_tf(self, materialise=True):
-        cache = self._intermediate_table_cache
-        nodes_with_tf = None
-        if "__splink__df_concat_with_tf" in cache:
-            nodes_with_tf = cache.get_with_logging("__splink__df_concat_with_tf")
-
-        else:
-            # In duckdb, calls to random() in a CTE pipeline cause problems:
-            # https://gist.github.com/RobinL/d329e7004998503ce91b68479aa41139
-            if self._settings_obj.salting_required:
-                materialise = True
-
-            if materialise:
-                # Clear the pipeline if we are materialising
-                # There's no reason not to do this, since when
-                # we execute the pipeline, it'll get cleared anyway
-                self._pipeline.reset()
-
-            sql = vertically_concatenate_sql(self)
-            self._enqueue_sql(sql, "__splink__df_concat")
-
-            sqls = compute_all_term_frequencies_sqls(self)
-            for sql in sqls:
-                self._enqueue_sql(sql["sql"], sql["output_table_name"])
-
-            if materialise:
-                nodes_with_tf = self._execute_sql_pipeline()
-                cache["__splink__df_concat_with_tf"] = nodes_with_tf
-
-        return nodes_with_tf
-
     def _table_to_splink_dataframe(
-        self, templated_name, physical_name
+        self, templated_name: str, physical_name: str
     ) -> SplinkDataFrame:
         """Create a SplinkDataframe from a table in the underlying database called
         `physical_name`.
-
         Associate a `templated_name` with this table, which signifies the purpose
         or 'meaning' of this table to splink. (e.g. `__splink__df_blocked`)
-
         Args:
             templated_name (str): The purpose of the table to Splink
             physical_name (str): The name of the table in the underlying databse
         """
         return self.db_api.table_to_splink_dataframe(templated_name, physical_name)
 
-    def _enqueue_sql(self, sql, output_table_name):
-        """Add sql to the current pipeline, but do not execute the pipeline."""
-        self._pipeline.enqueue_sql(sql, output_table_name)
-
-    def _execute_sql_pipeline(
+    def register_table(
         self,
-        input_dataframes: list[SplinkDataFrame] = [],
-        use_cache=True,
+        input_table: AcceptableInputTableType,
+        table_name: str,
+        overwrite: bool = False,
     ) -> SplinkDataFrame:
-        """Execute the SQL queued in the current pipeline as a single statement
-        e.g. `with a as (), b as , c as (), select ... from c`, then execute the
-        pipeline, returning the resultant table as a SplinkDataFrame
-
-        Args:
-            input_dataframes (List[SplinkDataFrame], optional): A 'starting point' of
-                SplinkDataFrames if needed. Defaults to [].
-            use_cache (bool, optional): If true, look at whether the SQL pipeline has
-                been executed before, and if so, use the existing result. Defaults to
-                True.
-
-        Returns:
-            SplinkDataFrame: An abstraction representing the table created by the sql
-                pipeline
-        """
-        try:
-            dataframe = self.db_api.sql_pipeline_to_splink_dataframe(
-                self._pipeline,
-                input_dataframes,
-                use_cache,
-            )
-        except Exception as e:
-            raise e
-        finally:
-            self._pipeline.reset()
-        return dataframe
-
-    def register_table(self, input, table_name, overwrite=False):
         """
         Register a table to your backend database, to be used in one of the
         splink methods, or simply to allow querying.
 
         Tables can be of type: dictionary, record level dictionary,
         pandas dataframe, pyarrow table and in the spark case, a spark df.
 
@@ -609,15 +436,15 @@
                 exists
 
         Returns:
             SplinkDataFrame: An abstraction representing the table created by the sql
                 pipeline
         """
 
-        return self.db_api.register_table(input, table_name, overwrite)
+        return self.db_api.register_table(input_table, table_name, overwrite)
 
     def query_sql(self, sql, output_type="pandas"):
         """
         Run a SQL query against your backend database and return
         the resulting output.
 
         Examples:
@@ -631,18 +458,18 @@
             sql (str): The SQL to be queried.
             output_type (str): One of splink_df/splinkdf or pandas.
                 This determines the type of table that your results are output in.
         """
 
         output_tablename_templated = "__splink__df_sql_query"
 
-        splink_dataframe = self._sql_to_splink_dataframe_checking_cache(
-            sql,
-            output_tablename_templated,
-            use_cache=False,
+        pipeline = CTEPipeline()
+        pipeline.enqueue_sql(sql, output_tablename_templated)
+        splink_dataframe = self.db_api.sql_pipeline_to_splink_dataframe(
+            pipeline, use_cache=False
         )
 
         if output_type in ("splink_df", "splinkdf"):
             return splink_dataframe
         elif output_type == "pandas":
             out = splink_dataframe.as_pandas_dataframe()
             # If pandas, drop the table to cleanup the db
@@ -650,35 +477,14 @@
             return out
         else:
             raise ValueError(
                 f"output_type '{output_type}' is not supported.",
                 "Must be one of 'splink_df'/'splinkdf' or 'pandas'",
             )
 
-    def _sql_to_splink_dataframe_checking_cache(
-        self,
-        sql,
-        output_tablename_templated,
-        use_cache=True,
-    ) -> SplinkDataFrame:
-        """Execute sql, or if identical sql has been run before, return cached results.
-
-        This function
-            - is used by _execute_sql_pipeline to to execute SQL
-            - or can be used directly if you have a single SQL statement that's
-              not in a pipeline
-
-        Return a SplinkDataFrame representing the results of the SQL
-        """
-        return self.db_api.sql_to_splink_dataframe_checking_cache(
-            sql,
-            output_tablename_templated,
-            use_cache=use_cache,
-        )
-
     def __deepcopy__(self, memo):
         """When we do EM training, we need a copy of the linker which is independent
         of the main linker e.g. setting parameters on the copy will not affect the
         main linker.  This method implements ensures linker can be deepcopied.
         """
         new_linker = copy(self)
         new_linker._em_training_sessions = []
@@ -724,17 +530,15 @@
             15,
             (
                 "---- Using training sessions to compute "
                 "probability two random records match ----"
             ),
         )
         for em_training_session in self._em_training_sessions:
-            training_lambda = (
-                em_training_session.core_model_settings.probability_two_random_records_match
-            )
+            training_lambda = em_training_session.core_model_settings.probability_two_random_records_match  # noqa: E501
             training_lambda_bf = prob_to_bayes_factor(training_lambda)
             reverse_level_infos = (
                 em_training_session._comparison_levels_to_reverse_blocking_rule
             )
 
             logger.log(
                 15,
@@ -750,15 +554,15 @@
                 # maybe they are different copies with different values?
                 reverse_level = reverse_level_info["level"]
                 cc = self._settings_obj._get_comparison_by_output_column_name(
                     reverse_level_info["comparison"].output_column_name
                 )
 
                 cl = cc._get_comparison_level_by_comparison_vector_value(
-                    reverse_level._comparison_vector_value
+                    reverse_level.comparison_vector_value
                 )
 
                 if cl._has_estimated_values:
                     bf = cl._trained_m_median / cl._trained_u_median
                 else:
                     bf = cl._bayes_factor
 
@@ -870,40 +674,23 @@
         input_col = InputColumn(
             column_name,
             column_info_settings=self._settings_obj.column_info_settings,
             sql_dialect=self._settings_obj._sql_dialect,
         )
         tf_tablename = colname_to_tf_tablename(input_col)
         cache = self._intermediate_table_cache
-        concat_tf_tables = [
-            tf_col.unquote().name
-            for tf_col in self._settings_obj._term_frequency_columns
-        ]
 
         if tf_tablename in cache:
             tf_df = cache.get_with_logging(tf_tablename)
-        elif "__splink__df_concat_with_tf" in cache and column_name in concat_tf_tables:
-            self._pipeline.reset()
-            # If our df_concat_with_tf table already exists, use backwards inference to
-            # find a given tf table
-            colname = InputColumn(column_name)
-            sql = term_frequencies_from_concat_with_tf(colname)
-            self._enqueue_sql(sql, colname_to_tf_tablename(colname))
-            tf_df = self._execute_sql_pipeline([cache["__splink__df_concat_with_tf"]])
-            self._intermediate_table_cache[tf_tablename] = tf_df
         else:
-            # Clear the pipeline if we are materialising
-            self._pipeline.reset()
-            df_concat = self._initialise_df_concat()
-            input_dfs = []
-            if df_concat:
-                input_dfs.append(df_concat)
+            pipeline = CTEPipeline()
+            pipeline = enqueue_df_concat(self, pipeline)
             sql = term_frequencies_for_single_column_sql(input_col)
-            self._enqueue_sql(sql, tf_tablename)
-            tf_df = self._execute_sql_pipeline(input_dfs)
+            pipeline.enqueue_sql(sql, tf_tablename)
+            tf_df = self.db_api.sql_pipeline_to_splink_dataframe(pipeline)
             self._intermediate_table_cache[tf_tablename] = tf_df
 
         return tf_df
 
     def deterministic_link(self) -> SplinkDataFrame:
         """Uses the blocking rules specified by
         `blocking_rules_to_generate_predictions` in the settings dictionary to
@@ -938,34 +725,74 @@
 
 
         Returns:
             SplinkDataFrame: A SplinkDataFrame of the pairwise comparisons.  This
                 represents a table materialised in the database. Methods on the
                 SplinkDataFrame allow you to access the underlying data.
         """
-
+        pipeline = CTEPipeline()
         # Allows clustering during a deterministic linkage.
         # This is used in `cluster_pairwise_predictions_at_threshold`
         # to set the cluster threshold to 1
-        self._deterministic_link_mode = True
 
-        concat_with_tf = self._initialise_df_concat_with_tf()
-        exploding_br_with_id_tables = materialise_exploded_id_tables(self)
+        df_concat_with_tf = compute_df_concat_with_tf(self, pipeline)
+        pipeline = CTEPipeline([df_concat_with_tf])
+        link_type = self._settings_obj._link_type
+
+        blocking_input_tablename_l = "__splink__df_concat_with_tf"
+        blocking_input_tablename_r = "__splink__df_concat_with_tf"
+
+        link_type = self._settings_obj._link_type
+        if (
+            len(self._input_tables_dict) == 2
+            and self._settings_obj._link_type == "link_only"
+        ):
+            sqls = split_df_concat_with_tf_into_two_tables_sqls(
+                "__splink__df_concat_with_tf",
+                self._settings_obj.column_info_settings.source_dataset_column_name,
+            )
+            pipeline.enqueue_list_of_sqls(sqls)
+
+            blocking_input_tablename_l = "__splink__df_concat_with_tf_left"
+            blocking_input_tablename_r = "__splink__df_concat_with_tf_right"
+            link_type = "two_dataset_link_only"
+
+        exploding_br_with_id_tables = materialise_exploded_id_tables(
+            link_type=link_type,
+            blocking_rules=self._settings_obj._blocking_rules_to_generate_predictions,
+            db_api=self.db_api,
+            splink_df_dict=self._input_tables_dict,
+            source_dataset_input_column=self._settings_obj.column_info_settings.source_dataset_input_column,
+            unique_id_input_column=self._settings_obj.column_info_settings.unique_id_input_column,
+        )
+
+        columns_to_select = self._settings_obj._columns_to_select_for_blocking
+        sql_select_expr = ", ".join(columns_to_select)
+
+        sqls = block_using_rules_sqls(
+            input_tablename_l=blocking_input_tablename_l,
+            input_tablename_r=blocking_input_tablename_r,
+            blocking_rules=self._settings_obj._blocking_rules_to_generate_predictions,
+            link_type=link_type,
+            columns_to_select_sql=sql_select_expr,
+            source_dataset_input_column=self._settings_obj.column_info_settings.source_dataset_input_column,
+            unique_id_input_column=self._settings_obj.column_info_settings.unique_id_input_column,
+        )
+        pipeline.enqueue_list_of_sqls(sqls)
 
-        sqls = block_using_rules_sqls(self)
-        for sql in sqls:
-            self._enqueue_sql(sql["sql"], sql["output_table_name"])
+        deterministic_link_df = self.db_api.sql_pipeline_to_splink_dataframe(pipeline)
+        deterministic_link_df.metadata["is_deterministic_link"] = True
 
-        deterministic_link_df = self._execute_sql_pipeline([concat_with_tf])
         [b.drop_materialised_id_pairs_dataframe() for b in exploding_br_with_id_tables]
+
         return deterministic_link_df
 
     def estimate_u_using_random_sampling(
-        self, max_pairs: int = None, seed: int = None, *, target_rows=None
-    ):
+        self, max_pairs: float = 1e6, seed: int = None
+    ) -> None:
         """Estimate the u parameters of the linkage model using random sampling.
 
         The u parameters represent the proportion of record comparisons that fall
         into each comparison level amongst truly non-matching records.
 
         This procedure takes a sample of the data and generates the cartesian
         product of pairwise record comparisons amongst the sampled records.
@@ -993,39 +820,28 @@
             linker.estimate_u_using_random_sampling(1e8)
             ```
 
         Returns:
             None: Updates the estimated u parameters within the linker object
             and returns nothing.
         """
-        # TODO: Remove this compatibility code in a future release once we drop
-        # support for "target_rows". Deprecation warning added in 3.7.0
-        if max_pairs is not None and target_rows is not None:
-            # user supplied both
-            raise TypeError("Just use max_pairs")
-        elif max_pairs is not None:
-            # user is doing it correctly
-            pass
-        elif target_rows is not None:
-            # user is using deprecated argument
-            warnings.warn(
-                "target_rows is deprecated; use max_pairs",
-                SplinkDeprecated,
-                stacklevel=2,
+        if max_pairs == 1e6:
+            # keep default value small so as not to take too long, but warn users
+            logger.warning(
+                "You are using the default value for `max_pairs`, "
+                "which may be too small and thus lead to inaccurate estimates for your "
+                "model's u-parameters. Consider increasing to 1e8 or 1e9, which will "
+                "result in more accurate estimates, but with a longer run time."
             )
-            max_pairs = target_rows
-        else:
-            raise TypeError("Missing argument max_pairs")
-
         estimate_u_values(self, max_pairs, seed)
         self._populate_m_u_from_trained_values()
 
         self._settings_obj._columns_without_estimated_parameters_message()
 
-    def estimate_m_from_label_column(self, label_colname: str):
+    def estimate_m_from_label_column(self, label_colname: str) -> None:
         """Estimate the m parameters of the linkage model from a label (ground truth)
         column in the input dataframe(s).
 
         The m parameters represent the proportion of record comparisons that fall
         into each comparison level amongst truly matching records.
 
         The ground truth column is used to generate pairwise record comparisons
@@ -1050,35 +866,37 @@
 
         Returns:
             Updates the estimated m parameters within the linker object
             and returns nothing.
         """
 
         # Ensure this has been run on the main linker so that it can be used by
-        # training linked when it checks the cache
-        self._initialise_df_concat_with_tf()
+        # training linker when it checks the cache
+        pipeline = CTEPipeline()
+        compute_df_concat_with_tf(self, pipeline)
+
         estimate_m_values_from_label_column(
             self,
             self._input_tables_dict,
             label_colname,
         )
         self._populate_m_u_from_trained_values()
 
         self._settings_obj._columns_without_estimated_parameters_message()
 
     def estimate_parameters_using_expectation_maximisation(
         self,
         blocking_rule: Union[str, BlockingRuleCreator],
-        comparisons_to_deactivate: list[str | Comparison] = None,
+        comparisons_to_deactivate: list[Comparison] = None,
         comparison_levels_to_reverse_blocking_rule: list[ComparisonLevel] = None,
         estimate_without_term_frequencies: bool = False,
         fix_probability_two_random_records_match: bool = False,
-        fix_m_probabilities=False,
-        fix_u_probabilities=True,
-        populate_probability_two_random_records_match_from_trained_values=False,
+        fix_m_probabilities: bool = False,
+        fix_u_probabilities: bool = True,
+        populate_probability_two_random_records_match_from_trained_values: bool = False,
     ) -> EMTrainingSession:
         """Estimate the parameters of the linkage model using expectation maximisation.
 
         By default, the m probabilities are estimated, but not the u probabilities,
         because good estimates for the u probabilities can be obtained from
         `linker.estimate_u_using_random_sampling()`.  You can change this by setting
         `fix_u_probabilities` to False.
@@ -1171,23 +989,21 @@
         Returns:
             EMTrainingSession:  An object containing information about the training
                 session such as how parameters changed during the iteration history
 
         """
         # Ensure this has been run on the main linker so that it's in the cache
         # to be used by the training linkers
-        self._initialise_df_concat_with_tf()
-        if isinstance(blocking_rule, BlockingRuleCreator):
-            blocking_rule_str_or_dict: str | dict = (
-                blocking_rule.create_blocking_rule_dict(self._sql_dialect)
-            )
-        else:
-            # we have a str
-            blocking_rule_str_or_dict = blocking_rule
-        blocking_rule_obj = blocking_rule_to_obj(blocking_rule_str_or_dict)
+        pipeline = CTEPipeline()
+        compute_df_concat_with_tf(self, pipeline)
+
+        blocking_rule_obj = to_blocking_rule_creator(blocking_rule).get_blocking_rule(
+            self._sql_dialect
+        )
+
         if type(blocking_rule_obj) not in (BlockingRule, SaltedBlockingRule):
             # TODO: seems a mismatch between message and type re: SaltedBlockingRule
             raise TypeError(
                 "EM blocking rules must be plain blocking rules, not "
                 "salted or exploding blocking rules"
             )
 
@@ -1242,15 +1058,15 @@
 
         return em_training_session
 
     def predict(
         self,
         threshold_match_probability: float = None,
         threshold_match_weight: float = None,
-        materialise_after_computing_term_frequencies=True,
+        materialise_after_computing_term_frequencies: bool = True,
     ) -> SplinkDataFrame:
         """Create a dataframe of scored pairwise comparisons using the parameters
         of the linkage model.
 
         Uses the blocking rules specified in the
         `blocking_rules_to_generate_predictions` of the settings dictionary to
         generate the pairwise comparisons.
@@ -1279,69 +1095,110 @@
         Returns:
             SplinkDataFrame: A SplinkDataFrame of the pairwise comparisons.  This
                 represents a table materialised in the database. Methods on the
                 SplinkDataFrame allow you to access the underlying data.
 
         """
 
+        pipeline = CTEPipeline()
+
         # If materialise_after_computing_term_frequencies=False and the user only
         # calls predict, it runs as a single pipeline with no materialisation
         # of anything.
 
-        # _initialise_df_concat_with_tf returns None if the table doesn't exist
-        # and only SQL is queued in this step.
-        nodes_with_tf = self._initialise_df_concat_with_tf(
-            materialise=materialise_after_computing_term_frequencies
-        )
+        # In duckdb, calls to random() in a CTE pipeline cause problems:
+        # https://gist.github.com/RobinL/d329e7004998503ce91b68479aa41139
+        if (
+            materialise_after_computing_term_frequencies
+            or self._sql_dialect == "duckdb"
+        ):
+            df_concat_with_tf = compute_df_concat_with_tf(self, pipeline)
+            pipeline = CTEPipeline([df_concat_with_tf])
+        else:
+            pipeline = enqueue_df_concat_with_tf(self, pipeline)
 
-        input_dataframes = []
-        if nodes_with_tf:
-            input_dataframes.append(nodes_with_tf)
+        blocking_input_tablename_l = "__splink__df_concat_with_tf"
+        blocking_input_tablename_r = "__splink__df_concat_with_tf"
+
+        link_type = self._settings_obj._link_type
+        if (
+            len(self._input_tables_dict) == 2
+            and self._settings_obj._link_type == "link_only"
+        ):
+            sqls = split_df_concat_with_tf_into_two_tables_sqls(
+                "__splink__df_concat_with_tf",
+                self._settings_obj.column_info_settings.source_dataset_column_name,
+            )
+            pipeline.enqueue_list_of_sqls(sqls)
+
+            blocking_input_tablename_l = "__splink__df_concat_with_tf_left"
+            blocking_input_tablename_r = "__splink__df_concat_with_tf_right"
+            link_type = "two_dataset_link_only"
 
         # If exploded blocking rules exist, we need to materialise
         # the tables of ID pairs
-        exploding_br_with_id_tables = materialise_exploded_id_tables(self)
 
-        sqls = block_using_rules_sqls(self)
-        for sql in sqls:
-            self._enqueue_sql(sql["sql"], sql["output_table_name"])
+        exploding_br_with_id_tables = materialise_exploded_id_tables(
+            link_type=link_type,
+            blocking_rules=self._settings_obj._blocking_rules_to_generate_predictions,
+            db_api=self.db_api,
+            splink_df_dict=self._input_tables_dict,
+            source_dataset_input_column=self._settings_obj.column_info_settings.source_dataset_input_column,
+            unique_id_input_column=self._settings_obj.column_info_settings.unique_id_input_column,
+        )
+
+        columns_to_select = self._settings_obj._columns_to_select_for_blocking
+        sql_select_expr = ", ".join(columns_to_select)
+
+        sqls = block_using_rules_sqls(
+            input_tablename_l=blocking_input_tablename_l,
+            input_tablename_r=blocking_input_tablename_r,
+            blocking_rules=self._settings_obj._blocking_rules_to_generate_predictions,
+            link_type=link_type,
+            columns_to_select_sql=sql_select_expr,
+            source_dataset_input_column=self._settings_obj.column_info_settings.source_dataset_input_column,
+            unique_id_input_column=self._settings_obj.column_info_settings.unique_id_input_column,
+        )
+
+        pipeline.enqueue_list_of_sqls(sqls)
 
         repartition_after_blocking = getattr(self, "repartition_after_blocking", False)
 
         # repartition after blocking only exists on the SparkLinker
         if repartition_after_blocking:
-            df_blocked = self._execute_sql_pipeline(input_dataframes)
-            input_dataframes.append(df_blocked)
+            pipeline = pipeline.break_lineage(self.db_api)
 
         sql = compute_comparison_vector_values_sql(
             self._settings_obj._columns_to_select_for_comparison_vector_values
         )
-        self._enqueue_sql(sql, "__splink__df_comparison_vectors")
+        pipeline.enqueue_sql(sql, "__splink__df_comparison_vectors")
 
         sqls = predict_from_comparison_vectors_sqls_using_settings(
             self._settings_obj,
             threshold_match_probability,
             threshold_match_weight,
             sql_infinity_expression=self._infinity_expression,
         )
-        for sql in sqls:
-            self._enqueue_sql(sql["sql"], sql["output_table_name"])
+        pipeline.enqueue_list_of_sqls(sqls)
 
-        predictions = self._execute_sql_pipeline(input_dataframes)
+        predictions = self.db_api.sql_pipeline_to_splink_dataframe(pipeline)
         self._predict_warning()
 
         [b.drop_materialised_id_pairs_dataframe() for b in exploding_br_with_id_tables]
 
         return predictions
 
     def find_matches_to_new_records(
         self,
-        records_or_tablename,
-        blocking_rules=[],
-        match_weight_threshold=-4,
+        records_or_tablename: AcceptableInputTableType | str,
+        blocking_rules: list[BlockingRuleCreator | dict[str, Any] | str]
+        | BlockingRuleCreator
+        | dict[str, Any]
+        | str = [],
+        match_weight_threshold: float = -4,
     ) -> SplinkDataFrame:
         """Given one or more records, find records in the input dataset(s) which match
         and return in order of the Splink prediction score.
 
         This effectively provides a way of searching the input datasets
         for given record(s)
 
@@ -1377,101 +1234,100 @@
         """
 
         original_blocking_rules = (
             self._settings_obj._blocking_rules_to_generate_predictions
         )
         original_link_type = self._settings_obj._link_type
 
-        blocking_rules = ensure_is_list(blocking_rules)
+        blocking_rule_list = ensure_is_list(blocking_rules)
 
         if not isinstance(records_or_tablename, str):
             uid = ascii_uid(8)
             new_records_tablename = f"__splink__df_new_records_{uid}"
             self.register_table(
                 records_or_tablename, new_records_tablename, overwrite=True
             )
 
         else:
             new_records_tablename = records_or_tablename
 
-        new_records_df = self._table_to_splink_dataframe(
+        new_records_df = self.db_api.table_to_splink_dataframe(
             "__splink__df_new_records", new_records_tablename
         )
 
-        cache = self._intermediate_table_cache
-        input_dfs = []
-        # If our df_concat_with_tf table already exists, derive the term frequency
-        # tables from df_concat_with_tf rather than computing them
-        if "__splink__df_concat_with_tf" in cache:
-            concat_with_tf = cache["__splink__df_concat_with_tf"]
-            tf_tables = compute_term_frequencies_from_concat_with_tf(self)
-            # This queues up our tf tables, rather materialising them
-            for tf in tf_tables:
-                # if tf is a SplinkDataFrame, then the table already exists
-                if isinstance(tf, SplinkDataFrame):
-                    input_dfs.append(tf)
-                else:
-                    self._enqueue_sql(tf["sql"], tf["output_table_name"])
-        else:
-            # This queues up our cols_with_tf and df_concat_with_tf tables.
-            concat_with_tf = self._initialise_df_concat_with_tf(materialise=False)
-
-        if concat_with_tf:
-            input_dfs.append(concat_with_tf)
-
-        blocking_rules = [blocking_rule_to_obj(br) for br in blocking_rules]
-        for n, br in enumerate(blocking_rules):
-            br.add_preceding_rules(blocking_rules[:n])
+        pipeline = CTEPipeline()
+        nodes_with_tf = compute_df_concat_with_tf(self, pipeline)
 
-        self._settings_obj._blocking_rules_to_generate_predictions = blocking_rules
-
-        self._find_new_matches_mode = True
-
-        sql = _join_tf_to_input_df_sql(self)
-        sql = sql.replace("__splink__df_concat", new_records_tablename)
-        self._enqueue_sql(sql, "__splink__df_new_records_with_tf_before_uid_fix")
+        pipeline = CTEPipeline([nodes_with_tf, new_records_df])
+        if len(blocking_rule_list) == 0:
+            blocking_rule_list = [BlockingRule("1=1")]
+        blocking_rule_list = [blocking_rule_to_obj(br) for br in blocking_rule_list]
+        for n, br in enumerate(blocking_rule_list):
+            br.add_preceding_rules(blocking_rule_list[:n])
+
+        self._settings_obj._blocking_rules_to_generate_predictions = blocking_rule_list
+
+        for tf_col in self._settings_obj._term_frequency_columns:
+            tf_table_name = colname_to_tf_tablename(tf_col)
+            if tf_table_name in self._intermediate_table_cache:
+                tf_table = self._intermediate_table_cache.get_with_logging(
+                    tf_table_name
+                )
+                pipeline.append_input_dataframe(tf_table)
 
-        add_unique_id_and_source_dataset_cols_if_needed(self, new_records_df)
+        sql = _join_new_table_to_df_concat_with_tf_sql(self, "__splink__df_new_records")
+        pipeline.enqueue_sql(sql, "__splink__df_new_records_with_tf_before_uid_fix")
 
-        sqls = block_using_rules_sqls(self)
-        for sql in sqls:
-            self._enqueue_sql(sql["sql"], sql["output_table_name"])
+        pipeline = add_unique_id_and_source_dataset_cols_if_needed(
+            self, new_records_df, pipeline
+        )
+        settings = self._settings_obj
+        sqls = block_using_rules_sqls(
+            input_tablename_l="__splink__df_concat_with_tf",
+            input_tablename_r="__splink__df_new_records_with_tf",
+            blocking_rules=blocking_rule_list,
+            link_type="two_dataset_link_only",
+            columns_to_select_sql=", ".join(settings._columns_to_select_for_blocking),
+            source_dataset_input_column=settings.column_info_settings.source_dataset_input_column,
+            unique_id_input_column=settings.column_info_settings.unique_id_input_column,
+        )
+        pipeline.enqueue_list_of_sqls(sqls)
 
         sql = compute_comparison_vector_values_sql(
             self._settings_obj._columns_to_select_for_comparison_vector_values
         )
-        self._enqueue_sql(sql, "__splink__df_comparison_vectors")
+        pipeline.enqueue_sql(sql, "__splink__df_comparison_vectors")
 
         sqls = predict_from_comparison_vectors_sqls_using_settings(
             self._settings_obj,
             sql_infinity_expression=self._infinity_expression,
         )
-        for sql in sqls:
-            self._enqueue_sql(sql["sql"], sql["output_table_name"])
+        pipeline.enqueue_list_of_sqls(sqls)
 
         sql = f"""
         select * from __splink__df_predict
         where match_weight > {match_weight_threshold}
         """
 
-        self._enqueue_sql(sql, "__splink__find_matches_predictions")
+        pipeline.enqueue_sql(sql, "__splink__find_matches_predictions")
 
-        predictions = self._execute_sql_pipeline(
-            input_dataframes=input_dfs, use_cache=False
+        predictions = self.db_api.sql_pipeline_to_splink_dataframe(
+            pipeline, use_cache=False
         )
 
         self._settings_obj._blocking_rules_to_generate_predictions = (
             original_blocking_rules
         )
         self._settings_obj._link_type = original_link_type
-        self._find_new_matches_mode = False
 
         return predictions
 
-    def compare_two_records(self, record_1: dict, record_2: dict):
+    def compare_two_records(
+        self, record_1: dict[str, Any], record_2: dict[str, Any]
+    ) -> SplinkDataFrame:
         """Use the linkage model to compare and score a pairwise record comparison
         based on the two input records provided
 
         Args:
             record_1 (dict): dictionary representing the first record.  Columns names
                 and data types must be the same as the columns in the settings object
             record_2 (dict): dictionary representing the second record.  Columns names
@@ -1483,135 +1339,142 @@
             linker.load_settings("saved_settings.json")
             linker.compare_two_records(record_left, record_right)
             ```
 
         Returns:
             SplinkDataFrame: Pairwise comparison with scored prediction
         """
-        original_blocking_rules = (
-            self._settings_obj._blocking_rules_to_generate_predictions
-        )
-        original_link_type = self._settings_obj._link_type
 
-        self._compare_two_records_mode = True
-        self._settings_obj._blocking_rules_to_generate_predictions = []
+        cache = self._intermediate_table_cache
 
         uid = ascii_uid(8)
         df_records_left = self.register_table(
             [record_1], f"__splink__compare_two_records_left_{uid}", overwrite=True
         )
         df_records_left.templated_name = "__splink__compare_two_records_left"
 
         df_records_right = self.register_table(
             [record_2], f"__splink__compare_two_records_right_{uid}", overwrite=True
         )
         df_records_right.templated_name = "__splink__compare_two_records_right"
 
-        sql_join_tf = _join_tf_to_input_df_sql(self)
+        pipeline = CTEPipeline([df_records_left, df_records_right])
 
-        sql_join_tf = sql_join_tf.replace(
-            "__splink__df_concat", "__splink__compare_two_records_left"
+        if "__splink__df_concat_with_tf" in cache:
+            nodes_with_tf = cache.get_with_logging("__splink__df_concat_with_tf")
+            pipeline.append_input_dataframe(nodes_with_tf)
+
+        for tf_col in self._settings_obj._term_frequency_columns:
+            tf_table_name = colname_to_tf_tablename(tf_col)
+            if tf_table_name in cache:
+                tf_table = cache.get_with_logging(tf_table_name)
+                pipeline.append_input_dataframe(tf_table)
+            else:
+                if "__splink__df_concat_with_tf" not in cache:
+                    logger.warning(
+                        f"No term frequencies found for column {tf_col.name}.\n"
+                        "To apply term frequency adjustments, you need to register"
+                        " a lookup using `linker.register_term_frequency_lookup`."
+                    )
+
+        sql_join_tf = _join_new_table_to_df_concat_with_tf_sql(
+            self, "__splink__compare_two_records_left"
         )
-        self._enqueue_sql(sql_join_tf, "__splink__compare_two_records_left_with_tf")
 
-        sql_join_tf = sql_join_tf.replace(
-            "__splink__compare_two_records_left", "__splink__compare_two_records_right"
+        pipeline.enqueue_sql(sql_join_tf, "__splink__compare_two_records_left_with_tf")
+
+        sql_join_tf = _join_new_table_to_df_concat_with_tf_sql(
+            self, "__splink__compare_two_records_right"
         )
 
-        self._enqueue_sql(sql_join_tf, "__splink__compare_two_records_right_with_tf")
+        pipeline.enqueue_sql(sql_join_tf, "__splink__compare_two_records_right_with_tf")
 
-        sqls = block_using_rules_sqls(self)
-        for sql in sqls:
-            self._enqueue_sql(sql["sql"], sql["output_table_name"])
+        sqls = block_using_rules_sqls(
+            input_tablename_l="__splink__compare_two_records_left_with_tf",
+            input_tablename_r="__splink__compare_two_records_right_with_tf",
+            blocking_rules=[BlockingRule("1=1")],
+            link_type=self._settings_obj._link_type,
+            columns_to_select_sql=", ".join(
+                self._settings_obj._columns_to_select_for_blocking
+            ),
+            source_dataset_input_column=self._settings_obj.column_info_settings.source_dataset_input_column,
+            unique_id_input_column=self._settings_obj.column_info_settings.unique_id_input_column,
+        )
+        pipeline.enqueue_list_of_sqls(sqls)
 
         sql = compute_comparison_vector_values_sql(
             self._settings_obj._columns_to_select_for_comparison_vector_values
         )
-        self._enqueue_sql(sql, "__splink__df_comparison_vectors")
+        pipeline.enqueue_sql(sql, "__splink__df_comparison_vectors")
 
         sqls = predict_from_comparison_vectors_sqls_using_settings(
             self._settings_obj,
             sql_infinity_expression=self._infinity_expression,
         )
-        for sql in sqls:
-            self._enqueue_sql(sql["sql"], sql["output_table_name"])
-
-        predictions = self._execute_sql_pipeline(
-            [df_records_left, df_records_right], use_cache=False
-        )
+        pipeline.enqueue_list_of_sqls(sqls)
 
-        self._settings_obj._blocking_rules_to_generate_predictions = (
-            original_blocking_rules
+        predictions = self.db_api.sql_pipeline_to_splink_dataframe(
+            pipeline, use_cache=False
         )
-        self._settings_obj._link_type = original_link_type
-        self._compare_two_records_mode = False
 
         return predictions
 
     def _self_link(self) -> SplinkDataFrame:
         """Use the linkage model to compare and score all records in our input df with
             themselves.
 
         Returns:
             SplinkDataFrame: Scored pairwise comparisons of the input records to
                 themselves.
         """
 
-        original_blocking_rules = (
-            self._settings_obj._blocking_rules_to_generate_predictions
-        )
-        original_link_type = self._settings_obj._link_type
-
-        # Changes our sql to allow for a self link.
-        # This is used in `_sql_gen_where_condition` in blocking.py
-        # to remove any 'where' clauses when blocking (normally when blocking
-        # we want to *remove* self links!)
-        self._self_link_mode = True
-
         # Block on uid i.e. create pairwise record comparisons where the uid matches
-        uid_cols = self._settings_obj.column_info_settings.unique_id_input_columns
+        settings = self._settings_obj
+        uid_cols = settings.column_info_settings.unique_id_input_columns
         uid_l = _composite_unique_id_from_edges_sql(uid_cols, None, "l")
         uid_r = _composite_unique_id_from_edges_sql(uid_cols, None, "r")
 
-        self._settings_obj._blocking_rules_to_generate_predictions = [
-            BlockingRule(f"{uid_l} = {uid_r}", sqlglot_dialect=self._sql_dialect)
-        ]
+        blocking_rule = BlockingRule(
+            f"{uid_l} = {uid_r}", sqlglot_dialect=self._sql_dialect
+        )
+
+        pipeline = CTEPipeline()
+        nodes_with_tf = compute_df_concat_with_tf(self, pipeline)
 
-        nodes_with_tf = self._initialise_df_concat_with_tf()
+        pipeline = CTEPipeline([nodes_with_tf])
 
-        sqls = block_using_rules_sqls(self)
-        for sql in sqls:
-            self._enqueue_sql(sql["sql"], sql["output_table_name"])
+        sqls = block_using_rules_sqls(
+            input_tablename_l="__splink__df_concat_with_tf",
+            input_tablename_r="__splink__df_concat_with_tf",
+            blocking_rules=[blocking_rule],
+            link_type="self_link",
+            columns_to_select_sql=", ".join(settings._columns_to_select_for_blocking),
+            source_dataset_input_column=settings.column_info_settings.source_dataset_input_column,
+            unique_id_input_column=settings.column_info_settings.unique_id_input_column,
+        )
+        pipeline.enqueue_list_of_sqls(sqls)
 
         sql = compute_comparison_vector_values_sql(
             self._settings_obj._columns_to_select_for_comparison_vector_values
         )
 
-        self._enqueue_sql(sql, "__splink__df_comparison_vectors")
+        pipeline.enqueue_sql(sql, "__splink__df_comparison_vectors")
 
-        sqls = predict_from_comparison_vectors_sqls(
+        sql_infos = predict_from_comparison_vectors_sqls(
             unique_id_input_columns=uid_cols,
             core_model_settings=self._settings_obj.core_model_settings,
             sql_dialect=self._sql_dialect,
             sql_infinity_expression=self._infinity_expression,
         )
-        for sql in sqls:
-            output_table_name = sql["output_table_name"]
+        for sql_info in sql_infos:
+            output_table_name = sql_info["output_table_name"]
             output_table_name = output_table_name.replace("predict", "self_link")
-            self._enqueue_sql(sql["sql"], output_table_name)
+            pipeline.enqueue_sql(sql_info["sql"], output_table_name)
 
-        predictions = self._execute_sql_pipeline(
-            input_dataframes=[nodes_with_tf], use_cache=False
-        )
-
-        self._settings_obj._blocking_rules_to_generate_predictions = (
-            original_blocking_rules
-        )
-        self._settings_obj._link_type = original_link_type
-        self._self_link_mode = False
+        predictions = self.db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
         return predictions
 
     def cluster_pairwise_predictions_at_threshold(
         self,
         df_predict: SplinkDataFrame,
         threshold_match_probability: Optional[float] = None,
@@ -1643,28 +1506,29 @@
         Returns:
             SplinkDataFrame: A SplinkDataFrame containing a list of all IDs, clustered
                 into groups based on the desired match threshold.
 
         """
 
         # Feeding in df_predict forces materiailisation, if it exists in your database
-        concat_with_tf = self._initialise_df_concat_with_tf(df_predict)
+        pipeline = CTEPipeline()
+        nodes_with_tf = compute_df_concat_with_tf(self, pipeline)
 
         edges_table = _cc_create_unique_id_cols(
             self,
-            concat_with_tf.physical_name,
-            df_predict.physical_name,
+            nodes_with_tf.physical_name,
+            df_predict,
             threshold_match_probability,
         )
 
         cc = solve_connected_components(
             self,
             edges_table,
             df_predict,
-            concat_with_tf,
+            nodes_with_tf,
             pairwise_formatting,
             filter_pairwise_format_for_clusters,
         )
         cc.metadata["threshold_match_probability"] = threshold_match_probability
 
         return cc
 
@@ -1697,31 +1561,30 @@
         """
         uid_cols = self._settings_obj.column_info_settings.unique_id_input_columns
         # need composite unique ids
         composite_uid_edges_l = _composite_unique_id_from_edges_sql(uid_cols, "l")
         composite_uid_edges_r = _composite_unique_id_from_edges_sql(uid_cols, "r")
         composite_uid_clusters = _composite_unique_id_from_nodes_sql(uid_cols)
 
+        pipeline = CTEPipeline()
         sqls = _node_degree_sql(
             df_predict,
             df_clustered,
             composite_uid_edges_l,
             composite_uid_edges_r,
             composite_uid_clusters,
             threshold_match_probability,
         )
+        pipeline.enqueue_list_of_sqls(sqls)
 
-        for sql in sqls:
-            self._enqueue_sql(sql["sql"], sql["output_table_name"])
-
-        df_node_metrics = self._execute_sql_pipeline()
+        df_node_metrics = self.db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
-        df_node_metrics.metadata[
-            "threshold_match_probability"
-        ] = threshold_match_probability
+        df_node_metrics.metadata["threshold_match_probability"] = (
+            threshold_match_probability
+        )
         return df_node_metrics
 
     def _compute_metrics_edges(
         self,
         df_node_metrics: SplinkDataFrame,
         df_predict: SplinkDataFrame,
         df_clustered: SplinkDataFrame,
@@ -1748,17 +1611,17 @@
         | s1-__-10005           | s1-__-10009             | False     |
         | s1-__-10021           | s1-__-10024             | True      |
         ...
         """
         df_edge_metrics = compute_edge_metrics(
             self, df_node_metrics, df_predict, df_clustered, threshold_match_probability
         )
-        df_edge_metrics.metadata[
-            "threshold_match_probability"
-        ] = threshold_match_probability
+        df_edge_metrics.metadata["threshold_match_probability"] = (
+            threshold_match_probability
+        )
         return df_edge_metrics
 
     def _compute_metrics_clusters(
         self,
         df_node_metrics: SplinkDataFrame,
     ) -> SplinkDataFrame:
         """
@@ -1781,26 +1644,24 @@
         | cluster_id  | n_nodes | n_edges | density | cluster_centralisation |
         |-------------|---------|---------|---------|------------------------|
         | s1-__-10006 | 4       | 4       | 0.66667 | 0.6666                 |
         | s1-__-10008 | 6       | 5       | 0.33333 | 0.4                    |
         | s1-__-10013 | 11      | 19      | 0.34545 | 0.3111                 |
         ...
         """
-
+        pipeline = CTEPipeline()
         sqls = _size_density_centralisation_sql(
             df_node_metrics,
         )
+        pipeline.enqueue_list_of_sqls(sqls)
 
-        for sql in sqls:
-            self._enqueue_sql(sql["sql"], sql["output_table_name"])
-
-        df_cluster_metrics = self._execute_sql_pipeline()
-        df_cluster_metrics.metadata[
-            "threshold_match_probability"
-        ] = df_node_metrics.metadata["threshold_match_probability"]
+        df_cluster_metrics = self.db_api.sql_pipeline_to_splink_dataframe(pipeline)
+        df_cluster_metrics.metadata["threshold_match_probability"] = (
+            df_node_metrics.metadata["threshold_match_probability"]
+        )
         return df_cluster_metrics
 
     def compute_graph_metrics(
         self,
         df_predict: SplinkDataFrame,
         df_clustered: SplinkDataFrame,
         *,
@@ -1852,71 +1713,17 @@
         # don't need edges as information is baked into node metrics
         df_cluster_metrics = self._compute_metrics_clusters(df_node_metrics)
 
         return GraphMetricsResults(
             nodes=df_node_metrics, edges=df_edge_metrics, clusters=df_cluster_metrics
         )
 
-    def profile_columns(
-        self, column_expressions: str | list[str] | None = None, top_n=10, bottom_n=10
-    ):
-        """
-        Profiles the specified columns of the dataframe initiated with the linker.
-
-        This can be computationally expensive if the dataframe is large.
-
-        For the provided columns with column_expressions (or for all columns if
-         left empty) calculate:
-        - A distribution plot that shows the count of values at each percentile.
-        - A top n chart, that produces a chart showing the count of the top n values
-        within the column
-        - A bottom n chart, that produces a chart showing the count of the bottom
-        n values within the column
-
-        This should be used to explore the dataframe, determine if columns have
-        sufficient completeness for linking, analyse the cardinality of columns, and
-        identify the need for standardisation within a given column.
-
-        Args:
-            linker (object): The initiated linker.
-            column_expressions (list, optional): A list of strings containing the
-                specified column names.
-                If left empty this will default to all columns.
-            top_n (int, optional): The number of top n values to plot.
-            bottom_n (int, optional): The number of bottom n values to plot.
-
-        Returns:
-            altair.Chart or dict: A visualization or JSON specification describing the
-            profiling charts.
-
-        Examples:
-            ```py
-            linker = Linker(df, db_api)
-            linker.profile_columns()
-            ```
-
-        Note:
-            - The `linker` object should be an instance of the initiated linker.
-            - The provided `column_expressions` can be a list of column names to
-                profile. If left empty, all columns will be profiled.
-            - The `top_n` and `bottom_n` parameters determine the number of top and
-                 bottom values to display in the respective charts.
-        """
-
-        return profile_columns(
-            list(map(lambda sdf: sdf.physical_name, self._input_tables_dict.values())),
-            self.db_api,
-            column_expressions=column_expressions,
-            top_n=top_n,
-            bottom_n=bottom_n,
-        )
-
     def _get_labels_tablename_from_input(
         self, labels_splinkdataframe_or_table_name: str | SplinkDataFrame
-    ):
+    ) -> str:
         if isinstance(labels_splinkdataframe_or_table_name, SplinkDataFrame):
             labels_tablename = labels_splinkdataframe_or_table_name.physical_name
         elif isinstance(labels_splinkdataframe_or_table_name, str):
             labels_tablename = labels_splinkdataframe_or_table_name
         else:
             raise ValueError(
                 "The 'labels_splinkdataframe_or_table_name' argument"
@@ -1957,16 +1764,16 @@
         labels_tablename = self._get_labels_tablename_from_input(
             labels_splinkdataframe_or_table_name
         )
         estimate_m_from_pairwise_labels(self, labels_tablename)
 
     def truth_space_table_from_labels_table(
         self,
-        labels_splinkdataframe_or_table_name,
-        threshold_actual=0.5,
+        labels_splinkdataframe_or_table_name: SplinkDataFrame | str,
+        threshold_actual: float = 0.5,
         match_weight_round_to_nearest: float = None,
     ) -> SplinkDataFrame:
         """Generate truth statistics (false positive etc.) for each threshold value of
         match_probability, suitable for plotting a ROC chart.
 
         The table of labels should be in the following format, and should be registered
         with your database:
@@ -2015,17 +1822,17 @@
             threshold_actual=threshold_actual,
             match_weight_round_to_nearest=match_weight_round_to_nearest,
         )
 
     def roc_chart_from_labels_table(
         self,
         labels_splinkdataframe_or_table_name: str | SplinkDataFrame,
-        threshold_actual=0.5,
+        threshold_actual: float = 0.5,
         match_weight_round_to_nearest: float = None,
-    ):
+    ) -> ChartReturnType:
         """Generate a ROC chart from labelled (ground truth) data.
 
         The table of labels should be in the following format, and should be registered
         with your database:
 
         |source_dataset_l|unique_id_l|source_dataset_r|unique_id_r|clerical_match_score|
         |----------------|-----------|----------------|-----------|--------------------|
@@ -2079,18 +1886,18 @@
             match_weight_round_to_nearest=match_weight_round_to_nearest,
         )
         recs = df_truth_space.as_record_dict()
         return roc_chart(recs)
 
     def precision_recall_chart_from_labels_table(
         self,
-        labels_splinkdataframe_or_table_name,
-        threshold_actual=0.5,
+        labels_splinkdataframe_or_table_name: SplinkDataFrame | str,
+        threshold_actual: float = 0.5,
         match_weight_round_to_nearest: float = None,
-    ):
+    ) -> ChartReturnType:
         """Generate a precision-recall chart from labelled (ground truth) data.
 
         The table of labels should be in the following format, and should be registered
         as a table with your database:
 
         |source_dataset_l|unique_id_l|source_dataset_r|unique_id_r|clerical_match_score|
         |----------------|-----------|----------------|-----------|--------------------|
@@ -2135,19 +1942,19 @@
             match_weight_round_to_nearest=match_weight_round_to_nearest,
         )
         recs = df_truth_space.as_record_dict()
         return precision_recall_chart(recs)
 
     def accuracy_chart_from_labels_table(
         self,
-        labels_splinkdataframe_or_table_name,
-        threshold_actual=0.5,
+        labels_splinkdataframe_or_table_name: SplinkDataFrame | str,
+        threshold_actual: float = 0.5,
         match_weight_round_to_nearest: float = None,
-        add_metrics: list = [],
-    ):
+        add_metrics: list[str] = [],
+    ) -> ChartReturnType:
         """Generate an accuracy measure chart from labelled (ground truth) data.
 
         The table of labels should be in the following format, and should be registered
         as a table with your database:
 
         |source_dataset_l|unique_id_l|source_dataset_r|unique_id_r|clerical_match_score|
         |----------------|-----------|----------------|-----------|--------------------|
@@ -2174,18 +1981,18 @@
             add_metrics (list(str), optional): Precision and recall metrics are always
                 included. Where provided, `add_metrics` specifies additional metrics
                 to show, with the following options:
 
                 - `"specificity"`: specificity, selectivity, true negative rate (TNR)
                 - `"npv"`: negative predictive value (NPV)
                 - `"accuracy"`: overall accuracy (TP+TN)/(P+N)
-                - `"f1"`/`"f2"`/`"f0_5"`: F-scores for \u03B2=1 (balanced), \u03B2=2
-                (emphasis on recall) and \u03B2=0.5 (emphasis on precision)
+                - `"f1"`/`"f2"`/`"f0_5"`: F-scores for \u03b2=1 (balanced), \u03b2=2
+                (emphasis on recall) and \u03b2=0.5 (emphasis on precision)
                 - `"p4"` -  an extended F1 score with specificity and NPV included
-                - `"phi"` - \u03C6 coefficient or Matthews correlation coefficient (MCC)
+                - `"phi"` - \u03c6 coefficient or Matthews correlation coefficient (MCC)
         Examples:
             === ":simple-duckdb: DuckDB"
                 ```py
                 labels = pd.read_csv("my_labels.csv")
                 linker.register_table(labels, "labels")
                 linker.accuracy_chart_from_labels_table("labels", add_metrics=["f1"])
                 ```
@@ -2222,18 +2029,18 @@
         )
         recs = df_truth_space.as_record_dict()
         return accuracy_chart(recs, add_metrics=add_metrics)
 
     def threshold_selection_tool_from_labels_table(
         self,
         labels_splinkdataframe_or_table_name: str | SplinkDataFrame,
-        threshold_actual=0.5,
+        threshold_actual: float = 0.5,
         match_weight_round_to_nearest: float = None,
-        add_metrics: list = [],
-    ):
+        add_metrics: list[str] = [],
+    ) -> ChartReturnType:
         """Generate an accuracy chart from labelled (ground truth) data.
 
         The table of labels should be in the following format, and should be registered
         as a table with your database:
 
         |source_dataset_l|unique_id_l|source_dataset_r|unique_id_r|clerical_match_score|
         |----------------|-----------|----------------|-----------|--------------------|
@@ -2260,18 +2067,18 @@
             add_metrics (list(str), optional): Precision and recall metrics are always
                 included. Where provided, `add_metrics` specifies additional metrics
                 to show, with the following options:
 
                 - `"specificity"`: specificity, selectivity, true negative rate (TNR)
                 - `"npv"`: negative predictive value (NPV)
                 - `"accuracy"`: overall accuracy (TP+TN)/(P+N)
-                - `"f1"`/`"f2"`/`"f0_5"`: F-scores for \u03B2=1 (balanced), \u03B2=2
-                (emphasis on recall) and \u03B2=0.5 (emphasis on precision)
+                - `"f1"`/`"f2"`/`"f0_5"`: F-scores for \u03b2=1 (balanced), \u03b2=2
+                (emphasis on recall) and \u03b2=0.5 (emphasis on precision)
                 - `"p4"` -  an extended F1 score with specificity and NPV included
-                - `"phi"` - \u03C6 coefficient or Matthews correlation coefficient (MCC)
+                - `"phi"` - \u03c6 coefficient or Matthews correlation coefficient (MCC)
         Examples:
             ```py
             linker.accuracy_chart_from_labels_column("ground_truth", add_metrics=["f1"])
             ```
 
         Returns:
             altair.Chart: An altair chart
@@ -2332,18 +2139,19 @@
             include_false_positives,
             include_false_negatives,
             threshold,
         )
 
     def truth_space_table_from_labels_column(
         self,
-        labels_column_name,
-        threshold_actual=0.5,
+        labels_column_name: str,
+        threshold_actual: float = 0.5,
         match_weight_round_to_nearest: float = None,
-    ):
+        positives_not_captured_by_blocking_rules_scored_as_zero: bool = True,
+    ) -> SplinkDataFrame:
         """Generate truth statistics (false positive etc.) for each threshold value of
         match_probability, suitable for plotting a ROC chart.
 
         Your labels_column_name should include the ground truth cluster (unique
         identifier) that groups entities which are the same
 
         Args:
@@ -2363,23 +2171,27 @@
             ```
 
         Returns:
             SplinkDataFrame:  Table of truth statistics
         """
 
         return truth_space_table_from_labels_column(
-            self, labels_column_name, threshold_actual, match_weight_round_to_nearest
+            self,
+            labels_column_name,
+            threshold_actual,
+            match_weight_round_to_nearest,
+            positives_not_captured_by_blocking_rules_scored_as_zero,
         )
 
     def roc_chart_from_labels_column(
         self,
-        labels_column_name,
-        threshold_actual=0.5,
+        labels_column_name: str,
+        threshold_actual: float = 0.5,
         match_weight_round_to_nearest: float = None,
-    ):
+    ) -> ChartReturnType:
         """Generate a ROC chart from ground truth data, whereby the ground truth
         is in a column in the input dataset called `labels_column_name`
 
         Args:
             labels_column_name (str): Column name containing labels in the input table
             threshold_actual (float, optional): Where the `clerical_match_score`
                 provided by the user is a probability rather than binary, this value
@@ -2406,18 +2218,18 @@
             match_weight_round_to_nearest=match_weight_round_to_nearest,
         )
         recs = df_truth_space.as_record_dict()
         return roc_chart(recs)
 
     def precision_recall_chart_from_labels_column(
         self,
-        labels_column_name,
-        threshold_actual=0.5,
+        labels_column_name: str,
+        threshold_actual: float = 0.5,
         match_weight_round_to_nearest: float = None,
-    ):
+    ) -> ChartReturnType:
         """Generate a precision-recall chart from ground truth data, whereby the ground
         truth is in a column in the input dataset called `labels_column_name`
 
         Args:
             labels_column_name (str): Column name containing labels in the input table
             threshold_actual (float, optional): Where the `clerical_match_score`
                 provided by the user is a probability rather than binary, this value
@@ -2443,19 +2255,19 @@
             match_weight_round_to_nearest=match_weight_round_to_nearest,
         )
         recs = df_truth_space.as_record_dict()
         return precision_recall_chart(recs)
 
     def accuracy_chart_from_labels_column(
         self,
-        labels_column_name,
-        threshold_actual=0.5,
+        labels_column_name: str,
+        threshold_actual: float = 0.5,
         match_weight_round_to_nearest: float = None,
-        add_metrics: list = [],
-    ):
+        add_metrics: list[str] = [],
+    ) -> ChartReturnType:
         """Generate an accuracy chart from ground truth data, whereby the ground
         truth is in a column in the input dataset called `labels_column_name`
 
         Args:
             labels_column_name (str): Column name containing labels in the input table
             threshold_actual (float, optional): Where the `clerical_match_score`
                 provided by the user is a probability rather than binary, this value
@@ -2468,18 +2280,18 @@
             add_metrics (list(str), optional): Precision and recall metrics are always
                 included. Where provided, `add_metrics` specifies additional metrics
                 to show, with the following options:
 
                 - `"specificity"`: specificity, selectivity, true negative rate (TNR)
                 - `"npv"`: negative predictive value (NPV)
                 - `"accuracy"`: overall accuracy (TP+TN)/(P+N)
-                - `"f1"`/`"f2"`/`"f0_5"`: F-scores for \u03B2=1 (balanced), \u03B2=2
-                (emphasis on recall) and \u03B2=0.5 (emphasis on precision)
+                - `"f1"`/`"f2"`/`"f0_5"`: F-scores for \u03b2=1 (balanced), \u03b2=2
+                (emphasis on recall) and \u03b2=0.5 (emphasis on precision)
                 - `"p4"` -  an extended F1 score with specificity and NPV included
-                - `"phi"` - \u03C6 coefficient or Matthews correlation coefficient (MCC)
+                - `"phi"` - \u03c6 coefficient or Matthews correlation coefficient (MCC)
         Examples:
             ```py
             linker.accuracy_chart_from_labels_column("ground_truth", add_metrics=["f1"])
             ```
 
         Returns:
             altair.Chart: An altair chart
@@ -2504,18 +2316,18 @@
         )
         recs = df_truth_space.as_record_dict()
         return accuracy_chart(recs, add_metrics=add_metrics)
 
     def threshold_selection_tool_from_labels_column(
         self,
         labels_column_name: str,
-        threshold_actual=0.5,
+        threshold_actual: float = 0.5,
         match_weight_round_to_nearest: float = None,
-        add_metrics: list = [],
-    ):
+        add_metrics: list[str] = [],
+    ) -> ChartReturnType:
         """Generate an accuracy chart from ground truth data, whereby the ground
         truth is in a column in the input dataset called `labels_column_name`
 
         Args:
             labels_column_name (str): Column name containing labels in the input table
             threshold_actual (float, optional): Where the `clerical_match_score`
                 provided by the user is a probability rather than binary, this value
@@ -2528,18 +2340,18 @@
             add_metrics (list(str), optional): Precision and recall metrics are always
                 included. Where provided, `add_metrics` specifies additional metrics
                 to show, with the following options:
 
                 - `"specificity"`: specificity, selectivity, true negative rate (TNR)
                 - `"npv"`: negative predictive value (NPV)
                 - `"accuracy"`: overall accuracy (TP+TN)/(P+N)
-                - `"f1"`/`"f2"`/`"f0_5"`: F-scores for \u03B2=1 (balanced), \u03B2=2
-                (emphasis on recall) and \u03B2=0.5 (emphasis on precision)
+                - `"f1"`/`"f2"`/`"f0_5"`: F-scores for \u03b2=1 (balanced), \u03b2=2
+                (emphasis on recall) and \u03b2=0.5 (emphasis on precision)
                 - `"p4"` -  an extended F1 score with specificity and NPV included
-                - `"phi"` - \u03C6 coefficient or Matthews correlation coefficient (MCC)
+                - `"phi"` - \u03c6 coefficient or Matthews correlation coefficient (MCC)
         Examples:
             ```py
             linker.accuracy_chart_from_labels_column("ground_truth", add_metrics=["f1"])
             ```
 
         Returns:
             altair.Chart: An altair chart
@@ -2592,16 +2404,20 @@
             label_colname,
             include_false_positives,
             include_false_negatives,
             threshold,
         )
 
     def match_weights_histogram(
-        self, df_predict: SplinkDataFrame, target_bins: int = 30, width=600, height=250
-    ):
+        self,
+        df_predict: SplinkDataFrame,
+        target_bins: int = 30,
+        width: int = 600,
+        height: int = 250,
+    ) -> ChartReturnType:
         """Generate a histogram that shows the distribution of match weights in
         `df_predict`
 
         Args:
             df_predict (SplinkDataFrame): Output of `linker.predict()`
             target_bins (int, optional): Target number of bins in histogram. Defaults to
                 30.
@@ -2614,16 +2430,19 @@
 
         """
         df = histogram_data(self, df_predict, target_bins)
         recs = df.as_record_dict()
         return match_weights_histogram(recs, width=width, height=height)
 
     def waterfall_chart(
-        self, records: list[dict], filter_nulls=True, remove_sensitive_data=False
-    ):
+        self,
+        records: list[dict[str, Any]],
+        filter_nulls: bool = True,
+        remove_sensitive_data: bool = False,
+    ) -> ChartReturnType:
         """Visualise how the final match weight is computed for the provided pairwise
         record comparisons.
 
         Records must be provided as a list of dictionaries. This would usually be
         obtained from `df.as_record_dict(limit=n)` where `df` is a SplinkDataFrame.
 
         Examples:
@@ -2652,28 +2471,28 @@
 
         return waterfall_chart(
             records, self._settings_obj, filter_nulls, remove_sensitive_data
         )
 
     def unlinkables_chart(
         self,
-        x_col="match_weight",
-        source_dataset=None,
-        as_dict=False,
-    ):
+        x_col: str = "match_weight",
+        name_of_data_in_title: str | None = None,
+        as_dict: bool = False,
+    ) -> ChartReturnType:
         """Generate an interactive chart displaying the proportion of records that
         are "unlinkable" for a given splink score threshold and model parameters.
 
         Unlinkable records are those that, even when compared with themselves, do not
         contain enough information to confirm a match.
 
         Args:
             x_col (str, optional): Column to use for the x-axis.
                 Defaults to "match_weight".
-            source_dataset (str, optional): Name of the source dataset to use for
+            name_of_data_in_title (str, optional): Name of the source dataset to use for
                 the title of the output chart.
             as_dict (bool, optional): If True, return a dict version of the chart.
 
         Examples:
             For the simplest code pipeline, load a pre-trained model
             and run this against the test data.
             ```py
@@ -2688,24 +2507,24 @@
 
         Returns:
             altair.Chart: An altair chart
         """
 
         # Link our initial df on itself and calculate the % of unlinkable entries
         records = unlinkables_data(self)
-        return unlinkables_chart(records, x_col, source_dataset, as_dict)
+        return unlinkables_chart(records, x_col, name_of_data_in_title, as_dict)
 
     def comparison_viewer_dashboard(
         self,
         df_predict: SplinkDataFrame,
         out_path: str,
-        overwrite=False,
-        num_example_rows=2,
-        return_html_as_string=False,
-    ):
+        overwrite: bool = False,
+        num_example_rows: int = 2,
+        return_html_as_string: bool = False,
+    ) -> str | None:
         """Generate an interactive html visualization of the linker's predictions and
         save to `out_path`.  For more information see
         [this video](https://www.youtube.com/watch?v=DNvCMqjipis)
 
 
         Args:
             df_predict (SplinkDataFrame): The outputs of `linker.predict()`
@@ -2727,34 +2546,36 @@
             ```py
             from IPython.display import IFrame
             IFrame(src="./scv.html", width="100%", height=1200)
             ```
 
         """
         self._raise_error_if_necessary_waterfall_columns_not_computed()
-
+        pipeline = CTEPipeline([df_predict])
         sql = comparison_vector_distribution_sql(self)
-        self._enqueue_sql(sql, "__splink__df_comparison_vector_distribution")
+        pipeline.enqueue_sql(sql, "__splink__df_comparison_vector_distribution")
 
         sqls = comparison_viewer_table_sqls(self, num_example_rows)
-        for sql in sqls:
-            self._enqueue_sql(sql["sql"], sql["output_table_name"])
+        pipeline.enqueue_list_of_sqls(sqls)
 
-        df = self._execute_sql_pipeline([df_predict])
+        df = self.db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
         rendered = render_splink_comparison_viewer_html(
             df.as_record_dict(),
             self._settings_obj._as_completed_dict(),
             out_path,
             overwrite,
         )
         if return_html_as_string:
             return rendered
+        return None
 
-    def parameter_estimate_comparisons_chart(self, include_m=True, include_u=False):
+    def parameter_estimate_comparisons_chart(
+        self, include_m: bool = True, include_u: bool = False
+    ) -> ChartReturnType:
         """Show a chart that shows how parameter estimates have differed across
         the different estimation methods you have used.
 
         For example, if you have run two EM estimation sessions, blocking on
         different variables, and both result in parameter estimates for
         first_name, this chart will enable easy comparison of the different
         estimates
@@ -2774,294 +2595,14 @@
         if include_u:
             to_retain.append("u")
 
         records = [r for r in records if r["m_or_u"] in to_retain]
 
         return parameter_estimate_comparisons(records)
 
-    def missingness_chart(self, input_dataset: str = None):
-        """Generate a summary chart of the missingness (prevalence of nulls) of
-        columns in the input datasets.  By default, missingness is assessed across
-        all input datasets
-
-        Args:
-            input_dataset (str, optional): Name of one of the input tables in the
-                database.  If provided, missingness will be computed for
-                this table alone.
-                Defaults to None.
-
-        Examples:
-            ```py
-            linker.missingness_chart()
-            ```
-            To view offline (if you don't have an internet connection):
-            ```py
-            from splink.charts import save_offline_chart
-            c = linker.missingness_chart()
-            save_offline_chart(c.to_dict(), "test_chart.html")
-            ```
-            View resultant html file in Jupyter (or just load it in your browser)
-            ```py
-            from IPython.display import IFrame
-            IFrame(src="./test_chart.html", width=1000, height=500
-            ```
-
-        Returns:
-            altair.Chart: An altair chart
-        """
-        records = missingness_data(self, input_dataset)
-        return missingness_chart(records)
-
-    def completeness_chart(self, input_dataset: str = None, cols: list[str] = None):
-        """Generate a summary chart of the completeness (proportion of non-nulls) of
-        columns in each of the input datasets. By default, completeness is assessed for
-        all column in the input data.
-
-        Args:
-            input_dataset (str, optional): Name of one of the input tables in the
-                database.  If provided, completeness will be computed for this table
-                alone. Defaults to None.
-            cols (List[str], optional): List of column names to calculate completeness.
-                Default to None.
-
-        Examples:
-            ```py
-            linker.completeness_chart()
-            ```
-            To view offline (if you don't have an internet connection):
-            ```py
-            from splink.charts import save_offline_chart
-            c = linker.completeness_chart()
-            save_offline_chart(c.to_dict(), "test_chart.html")
-            ```
-            View resultant html file in Jupyter (or just load it in your browser)
-            ```py
-            from IPython.display import IFrame
-            IFrame(src="./test_chart.html", width=1000, height=500
-            ```
-        """
-        records = completeness_data(self, input_dataset, cols)
-        return completeness_chart(records)
-
-    def count_num_comparisons_from_blocking_rule(
-        self,
-        blocking_rule: str | BlockingRule,
-    ) -> int:
-        """Compute the number of pairwise record comparisons that would be generated by
-        a blocking rule
-
-        Args:
-            blocking_rule (str | BlockingRule): The blocking rule to analyse
-            link_type (str, optional): The link type.  This is needed only if the
-                linker has not yet been provided with a settings dictionary.  Defaults
-                to None.
-            unique_id_column_name (str, optional):  This is needed only if the
-                linker has not yet been provided with a settings dictionary.  Defaults
-                to None.
-
-        Examples:
-            ```py
-            br = "l.surname = r.surname"
-            linker.count_num_comparisons_from_blocking_rule(br)
-            ```
-            > 19387
-
-            ```py
-            br = "l.name = r.name and substr(l.dob,1,4) = substr(r.dob,1,4)"
-            linker.count_num_comparisons_from_blocking_rule(br)
-            ```
-            > 394
-            Alternatively, you can use the blocking rule library functions
-            ```py
-            import splink.duckdb.blocking_rule_library as brl
-            br = brl.exact_match_rule("surname")
-            linker.count_num_comparisons_from_blocking_rule(br)
-            ```
-            > 3167
-
-        Returns:
-            int: The number of comparisons generated by the blocking rule
-        """
-
-        blocking_rule = blocking_rule_to_obj(blocking_rule).blocking_rule_sql
-
-        sql = vertically_concatenate_sql(self)
-        self._enqueue_sql(sql, "__splink__df_concat")
-
-        sql = number_of_comparisons_generated_by_blocking_rule_post_filters_sql(
-            self, blocking_rule
-        )
-        self._enqueue_sql(sql, "__splink__analyse_blocking_rule")
-        res = self._execute_sql_pipeline().as_record_dict()[0]
-        return res["count_of_pairwise_comparisons_generated"]
-
-    def _count_num_comparisons_from_blocking_rule_pre_filter_conditions(
-        self,
-        blocking_rule: BlockingRule,
-    ) -> int:
-        """Compute the number of pairwise record comparisons that would be generated by
-        a blocking rule, prior to any filters (non equi-join conditions) being applied
-        by the SQL engine.
-
-        For more information on what this means, see
-        https://github.com/moj-analytical-services/splink/discussions/1391
-
-        Args:
-            blocking_rule (str): The blocking rule to analyse
-
-        Returns:
-            int: The number of comparisons generated by the blocking rule
-        """
-
-        input_dataframes = []
-        df_concat = self._initialise_df_concat()
-
-        if df_concat:
-            input_dataframes.append(df_concat)
-
-        sqls = count_comparisons_from_blocking_rule_pre_filter_conditions_sqls(
-            self, blocking_rule
-        )
-        for sql in sqls:
-            self._enqueue_sql(sql["sql"], sql["output_table_name"])
-
-        res = self._execute_sql_pipeline(input_dataframes).as_record_dict()[0]
-        return int(res["count_of_pairwise_comparisons_generated"])
-
-    def cumulative_comparisons_from_blocking_rules_records(
-        self,
-        blocking_rules: str | BlockingRule | list | None = None,
-    ):
-        """Output the number of comparisons generated by each successive blocking rule.
-
-        This is equivalent to the output size of df_predict and details how many
-        comparisons each of your individual blocking rules will contribute to the
-        total.
-
-        Args:
-            blocking_rules (str or list): The blocking rule(s) to compute comparisons
-                for. If null, the rules set out in your settings object will be used.
-
-        Examples:
-            Generate total comparisons from Blocking Rules defined in settings
-            dictionary
-            ```py
-            linker_settings = DuckDBLinker(df, settings)
-            # Compute the cumulative number of comparisons generated by the rules
-            # in your settings object.
-            linker_settings.cumulative_comparisons_from_blocking_rules_records()
-            ```
-
-            Generate total comparisons with custom blocking rules.
-            ```py
-            blocking_rules = [
-               "l.surname = r.surname",
-               "l.first_name = r.first_name
-                and substr(l.dob,1,4) = substr(r.dob,1,4)"
-            ]
-
-            linker_settings.cumulative_comparisons_from_blocking_rules_records(
-                blocking_rules
-             )
-            ```
-
-        Returns:
-            List: A list of blocking rules and the corresponding number of
-                comparisons it is forecast to generate.
-        """
-        if blocking_rules:
-            blocking_rules = ensure_is_list(blocking_rules)
-
-        records = cumulative_comparisons_generated_by_blocking_rules(
-            self, blocking_rules, output_chart=False
-        )
-
-        return records
-
-    def cumulative_num_comparisons_from_blocking_rules_chart(
-        self,
-        blocking_rules: str | BlockingRule | list | None = None,
-    ):
-        """Display a chart with the cumulative number of comparisons generated by a
-        selection of blocking rules.
-
-        This is equivalent to the output size of df_predict and details how many
-        comparisons each of your individual blocking rules will contribute to the
-        total.
-
-        Args:
-            blocking_rules (str or list): The blocking rule(s) to compute comparisons
-                for. If null, the rules set out in your settings object will be used.
-
-        Examples:
-            ```py
-            linker_settings = DuckDBLinker(df, settings)
-            # Compute the cumulative number of comparisons generated by the rules
-            # in your settings object.
-            linker_settings.cumulative_num_comparisons_from_blocking_rules_chart()
-            >>>
-            # Generate total comparisons with custom blocking rules.
-            blocking_rules = [
-               "l.surname = r.surname",
-               "l.first_name = r.first_name
-                and substr(l.dob,1,4) = substr(r.dob,1,4)"
-            ]
-            >>>
-            linker_settings.cumulative_num_comparisons_from_blocking_rules_chart(
-                blocking_rules
-             )
-            ```
-
-        Returns:
-            altair.Chart: An altair chart
-        """
-
-        if blocking_rules:
-            blocking_rules = ensure_is_list(blocking_rules)
-
-        records = cumulative_comparisons_generated_by_blocking_rules(
-            self, blocking_rules, output_chart=True
-        )
-
-        return cumulative_blocking_rule_comparisons_generated(records)
-
-    def count_num_comparisons_from_blocking_rules_for_prediction(self, df_predict):
-        """Counts the marginal number of edges created from each of the blocking rules
-        in `blocking_rules_to_generate_predictions`
-
-        This is different to `count_num_comparisons_from_blocking_rule`
-        because it (a) analyses multiple blocking rules rather than a single rule, and
-        (b) deduplicates any comparisons that are generated, to tell you the
-        marginal effect of each entry in `blocking_rules_to_generate_predictions`
-
-        Args:
-            df_predict (SplinkDataFrame): SplinkDataFrame with match weights
-            and probabilities of rows matching
-
-        Examples:
-            ```py
-            linker = DuckDBLinker(df)
-            linker.load_model("settings.json")
-            df_predict = linker.predict(threshold_match_probability=0.95)
-            count_pairwise = linker.count_num_comparisons_from_blocking_rules_for_prediction(df_predict)
-            count_pairwise.as_pandas_dataframe(limit=5)
-            ```
-
-        Returns:
-            SplinkDataFrame: A SplinkDataFrame of the pairwise comparisons and
-                estimated pairwise comparisons generated by the blocking rules.
-        """  # noqa: E501
-        sql = count_num_comparisons_from_blocking_rules_for_prediction_sql(
-            self, df_predict
-        )
-        match_key_analysis = self._sql_to_splink_dataframe_checking_cache(
-            sql, "__splink__match_key_analysis"
-        )
-        return match_key_analysis
-
     def match_weights_chart(self):
         """Display a chart of the (partial) match weights of the linkage model
 
         Examples:
             ```py
             linker.match_weights_chart()
             ```
@@ -3083,17 +2624,17 @@
         return self._settings_obj.match_weights_chart()
 
     def tf_adjustment_chart(
         self,
         output_column_name: str,
         n_most_freq: int = 10,
         n_least_freq: int = 10,
-        vals_to_include: str | list | None = None,
+        vals_to_include: str | list[str] | None = None,
         as_dict: bool = False,
-    ):
+    ) -> ChartReturnType:
         """Display a chart showing the impact of term frequency adjustments on a
         specific comparison level.
         Each value
 
         Args:
             output_column_name (str): Name of an output column for which term frequency
                  adjustment has been applied.
@@ -3119,15 +2660,17 @@
         ]
         if output_column_name not in tf_comparisons:
             raise ValueError(
                 f"{output_column_name} is not a valid comparison column, or does not"
                 f" have term frequency adjustment activated"
             )
 
-        vals_to_include = ensure_is_list(vals_to_include)
+        vals_to_include = (
+            [] if vals_to_include is None else ensure_is_list(vals_to_include)
+        )
 
         return tf_adjustment_chart(
             self,
             output_column_name,
             n_most_freq,
             n_least_freq,
             vals_to_include,
@@ -3160,22 +2703,22 @@
         return self._settings_obj.m_u_parameters_chart()
 
     def cluster_studio_dashboard(
         self,
         df_predict: SplinkDataFrame,
         df_clustered: SplinkDataFrame,
         out_path: str,
-        sampling_method="random",
+        sampling_method: SamplingMethods = "random",
         sample_size: int = 10,
-        cluster_ids: list = None,
-        cluster_names: list = None,
+        cluster_ids: list[str] = None,
+        cluster_names: list[str] = None,
         overwrite: bool = False,
-        return_html_as_string=False,
+        return_html_as_string: bool = False,
         _df_cluster_metrics: SplinkDataFrame = None,
-    ):
+    ) -> str | None:
         """Generate an interactive html visualization of the predicted cluster and
         save to `out_path`.
 
         Args:
             df_predict (SplinkDataFrame): The outputs of `linker.predict()`
             df_clustered (SplinkDataFrame): The outputs of
                 `linker.cluster_pairwise_predictions_at_threshold()`
@@ -3222,18 +2765,19 @@
             overwrite=overwrite,
             cluster_names=cluster_names,
             _df_cluster_metrics=_df_cluster_metrics,
         )
 
         if return_html_as_string:
             return rendered
+        return None
 
     def save_model_to_json(
         self, out_path: str | None = None, overwrite: bool = False
-    ) -> dict:
+    ) -> dict[str, Any]:
         """Save the configuration and parameters of the linkage model to a `.json` file.
 
         The model can later be loaded back in using `linker.load_model()`.
         The settings dict is also returned in case you want to save it a different way.
 
         Examples:
             ```py
@@ -3254,30 +2798,20 @@
                     f"The path {out_path} already exists. Please provide a different "
                     "path or set overwrite=True"
                 )
             with open(out_path, "w", encoding="utf-8") as f:
                 json.dump(model_dict, f, indent=4)
         return model_dict
 
-    def save_settings_to_json(
-        self, out_path: str | None = None, overwrite: bool = False
-    ) -> dict:
-        """
-        This function is deprecated. Use save_model_to_json() instead.
-        """
-        warnings.warn(
-            "This function is deprecated. Use save_model_to_json() instead.",
-            SplinkDeprecated,
-            stacklevel=2,
-        )
-        return self.save_model_to_json(out_path, overwrite)
-
     def estimate_probability_two_random_records_match(
-        self, deterministic_matching_rules, recall
-    ):
+        self,
+        deterministic_matching_rules: List[Union[str, BlockingRuleCreator]],
+        recall: float,
+        max_rows_limit: int = int(1e9),
+    ) -> None:
         """Estimate the model parameter `probability_two_random_records_match` using
         a direct estimation approach.
 
         See [here](https://github.com/moj-analytical-services/splink/issues/462)
         for discussion of methodology
 
         Args:
@@ -3289,25 +2823,37 @@
                 by these deterministic rules
         """
 
         if (recall > 1) or (recall <= 0):
             raise ValueError(
                 f"Estimated recall must be greater than 0 "
                 f"and no more than 1. Supplied value {recall}."
-            )
+            ) from None
 
-        # If user, by error, provides a single rule as a string
-        if isinstance(deterministic_matching_rules, str):
-            deterministic_matching_rules = [deterministic_matching_rules]
+        deterministic_matching_rules = ensure_is_iterable(deterministic_matching_rules)
+        blocking_rules: List[BlockingRule] = []
+        for br in deterministic_matching_rules:
+            blocking_rules.append(
+                to_blocking_rule_creator(br).get_blocking_rule(
+                    self.db_api.sql_dialect.name
+                )
+            )
 
-        records = cumulative_comparisons_generated_by_blocking_rules(
-            self,
-            deterministic_matching_rules,
+        pd_df = _cumulative_comparisons_to_be_scored_from_blocking_rules(
+            splink_df_dict=self._input_tables_dict,
+            blocking_rules=blocking_rules,
+            link_type=self._settings_obj._link_type,
+            db_api=self.db_api,
+            max_rows_limit=max_rows_limit,
+            unique_id_column_name=self._settings_obj.column_info_settings.unique_id_column_name,
+            source_dataset_column_name=self._settings_obj.column_info_settings.source_dataset_column_name,
         )
 
+        records = pd_df.to_dict(orient="records")
+
         summary_record = records[-1]
         num_observed_matches = summary_record["cumulative_rows"]
         num_total_comparisons = summary_record["cartesian"]
 
         if num_observed_matches > num_total_comparisons * recall:
             raise ValueError(
                 f"Deterministic matching rules led to more "
@@ -3649,14 +3195,7 @@
                 msg = "The following EM training strategy was detected:\n"
                 msg = f"{msg}{suggestion_str}"
                 logger.info(msg)
                 suggestion = blocking_rule_suggestions[
                     "suggested_blocking_rules_as_splink_brs"
                 ].iloc[0]
                 return suggestion
-
-    def _explode_arrays_sql(
-        self, tbl_name, columns_to_explode, other_columns_to_retain
-    ):
-        return self._sql_dialect_object.explode_arrays_sql(
-            tbl_name, columns_to_explode, other_columns_to_retain
-        )
```

### Comparing `splink-4.0.0.dev3/splink/lower_id_on_lhs.py` & `splink-4.0.0.dev4/splink/lower_id_on_lhs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from pandas import DataFrame
+
+
 def _sql_expr_move_left_to_right(
-    col_name,
+    col_name: str,
     unique_id_col: str = "unique_id",
     source_dataset_col: str = "source_dataset",
-):
+) -> str:
     sds_l = f"{source_dataset_col}_l"
     uid_l = f"{unique_id_col}_l"
     sds_r = f"{source_dataset_col}_r"
     uid_r = f"{unique_id_col}_r"
     col_name_l = f"{col_name}_l"
     col_name_r = f"{col_name}_r"
 
@@ -38,18 +41,18 @@
     {move_to_right}
     """
 
     return exprs
 
 
 def lower_id_to_left_hand_side(
-    df,
+    df: DataFrame,
     source_dataset_col: str = "source_dataset",
     unique_id_col: str = "unique_id",
-):
+) -> str:
     """Take a dataframe in the format of splink record comparisons (with _l and _r suffixes)
     and return a dataframe where the _l columns correspond to the record with the lower id.
     For example:
     | source_dataset_l   |   unique_id_l | source_dataset_r   |   unique_id_r |   a_l |   a_r | other_col   |
     |:-------------------|--------------:|:-------------------|--------------:|------:|------:|:------------|
     | df                 |             0 | df                 |             1 |     0 |     1 | a           |
     | df                 |             2 | df                 |             0 |     2 |     0 | b           |
```

### Comparing `splink-4.0.0.dev3/splink/m_from_labels.py` & `splink-4.0.0.dev4/splink/m_training.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,86 @@
 import logging
+from copy import deepcopy
 
-from .block_from_labels import block_from_labels
+from .blocking import BlockingRule, block_using_rules_sqls
 from .comparison_vector_values import compute_comparison_vector_values_sql
 from .expectation_maximisation import (
     compute_new_parameters_sql,
     compute_proportions_for_new_parameters,
 )
 from .m_u_records_to_parameters import (
     append_m_probability_to_comparison_level_trained_probabilities,
     m_u_records_to_lookup_dict,
 )
+from .pipeline import CTEPipeline
+from .vertically_concatenate import compute_df_concat_with_tf
 
 logger = logging.getLogger(__name__)
 
 
-def estimate_m_from_pairwise_labels(linker, table_name):
-    concat_with_tf = linker._initialise_df_concat_with_tf()
-
-    sqls = block_from_labels(linker, table_name)
-
-    for sql in sqls:
-        linker._enqueue_sql(sql["sql"], sql["output_table_name"])
+def estimate_m_values_from_label_column(linker, df_dict, label_colname):
+    msg = f" Estimating m probabilities using from column {label_colname} "
+    logger.info(f"{msg:-^70}")
+
+    original_settings_object = linker._settings_obj
+    training_linker = deepcopy(linker)
+    settings_obj = training_linker._settings_obj
+    settings_obj._retain_matching_columns = False
+    settings_obj._retain_intermediate_calculation_columns = False
+    for cc in settings_obj.comparisons:
+        for cl in cc.comparison_levels:
+            # TODO: ComparisonLevel: manage access
+            cl._tf_adjustment_column = None
+
+    pipeline = CTEPipeline()
+    nodes_with_tf = compute_df_concat_with_tf(linker, pipeline)
+
+    pipeline = CTEPipeline([nodes_with_tf])
+
+    sqls = block_using_rules_sqls(
+        input_tablename_l="__splink__df_concat_with_tf",
+        input_tablename_r="__splink__df_concat_with_tf",
+        blocking_rules=[BlockingRule(f"l.{label_colname} = r.{label_colname}")],
+        link_type=settings_obj._link_type,
+        columns_to_select_sql=", ".join(settings_obj._columns_to_select_for_blocking),
+        source_dataset_input_column=settings_obj.column_info_settings.source_dataset_input_column,
+        unique_id_input_column=settings_obj.column_info_settings.unique_id_input_column,
+    )
+    pipeline.enqueue_list_of_sqls(sqls)
 
     sql = compute_comparison_vector_values_sql(
-        linker._settings_obj._columns_to_select_for_comparison_vector_values
+        settings_obj._columns_to_select_for_comparison_vector_values
     )
 
-    linker._enqueue_sql(sql, "__splink__df_comparison_vectors")
+    pipeline.enqueue_sql(sql, "__splink__df_comparison_vectors")
 
     sql = """
     select *, cast(1.0 as float8) as match_probability
     from __splink__df_comparison_vectors
     """
-    linker._enqueue_sql(sql, "__splink__df_predict")
+    pipeline.enqueue_sql(sql, "__splink__df_predict")
 
     sql = compute_new_parameters_sql(
         estimate_without_term_frequencies=False,
-        comparisons=linker._settings_obj.comparisons,
+        comparisons=settings_obj.comparisons,
     )
-    linker._enqueue_sql(sql, "__splink__m_u_counts")
+    pipeline.enqueue_sql(sql, "__splink__m_u_counts")
+
+    df_params = training_linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
-    df_params = linker._execute_sql_pipeline([concat_with_tf])
     param_records = df_params.as_pandas_dataframe()
     param_records = compute_proportions_for_new_parameters(param_records)
 
     m_u_records = [
         r
         for r in param_records
         if r["output_column_name"] != "_probability_two_random_records_match"
     ]
-
     m_u_records_lookup = m_u_records_to_lookup_dict(m_u_records)
-    for cc in linker._settings_obj.comparisons:
+    for cc in original_settings_object.comparisons:
         for cl in cc._comparison_levels_excluding_null:
             append_m_probability_to_comparison_level_trained_probabilities(
                 cl,
                 m_u_records_lookup,
                 cc.output_column_name,
-                "estimate m from pairwise labels",
+                "estimate m from label column",
             )
-
-    linker._populate_m_u_from_trained_values()
```

### Comparing `splink-4.0.0.dev3/splink/m_training.py` & `splink-4.0.0.dev4/splink/m_from_labels.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,66 @@
 import logging
-from copy import deepcopy
 
-from .blocking import BlockingRule, block_using_rules_sqls
+from .block_from_labels import block_from_labels
 from .comparison_vector_values import compute_comparison_vector_values_sql
 from .expectation_maximisation import (
     compute_new_parameters_sql,
     compute_proportions_for_new_parameters,
 )
 from .m_u_records_to_parameters import (
     append_m_probability_to_comparison_level_trained_probabilities,
     m_u_records_to_lookup_dict,
 )
+from .pipeline import CTEPipeline
+from .vertically_concatenate import compute_df_concat_with_tf
 
 logger = logging.getLogger(__name__)
 
 
-def estimate_m_values_from_label_column(linker, df_dict, label_colname):
-    msg = f" Estimating m probabilities using from column {label_colname} "
-    logger.info(f"{msg:-^70}")
-
-    original_settings_object = linker._settings_obj
-    training_linker = deepcopy(linker)
-    settings_obj = training_linker._settings_obj
-    settings_obj._retain_matching_columns = False
-    settings_obj._retain_intermediate_calculation_columns = False
-    for cc in settings_obj.comparisons:
-        for cl in cc.comparison_levels:
-            # TODO: ComparisonLevel: manage access
-            cl._tf_adjustment_column = None
+def estimate_m_from_pairwise_labels(linker, table_name):
+    pipeline = CTEPipeline()
+    nodes_with_tf = compute_df_concat_with_tf(linker, pipeline)
+    pipeline = CTEPipeline([nodes_with_tf])
+    sqls = block_from_labels(linker, table_name)
 
-    settings_obj._blocking_rules_to_generate_predictions = [
-        BlockingRule(f"l.{label_colname} = r.{label_colname}")
-    ]
-
-    concat_with_tf = linker._initialise_df_concat_with_tf()
-
-    sqls = block_using_rules_sqls(training_linker)
-
-    for sql in sqls:
-        training_linker._enqueue_sql(sql["sql"], sql["output_table_name"])
+    pipeline.enqueue_list_of_sqls(sqls)
 
     sql = compute_comparison_vector_values_sql(
-        settings_obj._columns_to_select_for_comparison_vector_values
+        linker._settings_obj._columns_to_select_for_comparison_vector_values
     )
 
-    training_linker._enqueue_sql(sql, "__splink__df_comparison_vectors")
+    pipeline.enqueue_sql(sql, "__splink__df_comparison_vectors")
 
     sql = """
     select *, cast(1.0 as float8) as match_probability
     from __splink__df_comparison_vectors
     """
-    training_linker._enqueue_sql(sql, "__splink__df_predict")
+    pipeline.enqueue_sql(sql, "__splink__df_predict")
 
     sql = compute_new_parameters_sql(
         estimate_without_term_frequencies=False,
-        comparisons=settings_obj.comparisons,
+        comparisons=linker._settings_obj.comparisons,
     )
-    training_linker._enqueue_sql(sql, "__splink__m_u_counts")
+    pipeline.enqueue_sql(sql, "__splink__m_u_counts")
+
+    df_params = linker.db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
-    df_params = training_linker._execute_sql_pipeline([concat_with_tf])
     param_records = df_params.as_pandas_dataframe()
     param_records = compute_proportions_for_new_parameters(param_records)
 
     m_u_records = [
         r
         for r in param_records
         if r["output_column_name"] != "_probability_two_random_records_match"
     ]
+
     m_u_records_lookup = m_u_records_to_lookup_dict(m_u_records)
-    for cc in original_settings_object.comparisons:
+    for cc in linker._settings_obj.comparisons:
         for cl in cc._comparison_levels_excluding_null:
             append_m_probability_to_comparison_level_trained_probabilities(
                 cl,
                 m_u_records_lookup,
                 cc.output_column_name,
-                "estimate m from label column",
+                "estimate m from pairwise labels",
             )
+
+    linker._populate_m_u_from_trained_values()
```

### Comparing `splink-4.0.0.dev3/splink/m_u_records_to_parameters.py` & `splink-4.0.0.dev4/splink/m_u_records_to_parameters.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 import logging
-from typing import Dict, List
+from typing import Any, Dict, List
 
 from .comparison_level import ComparisonLevel
 from .constants import LEVEL_NOT_OBSERVED_TEXT
 
 logger = logging.getLogger(__name__)
 
 
-def m_u_records_to_lookup_dict(m_u_records: List[dict]) -> Dict[str, dict]:
-    lookup: dict[str, dict] = {}
+def m_u_records_to_lookup_dict(
+    m_u_records: List[Dict[str, Any]],
+) -> Dict[str, Dict[int, Any]]:
+    lookup: Dict[str, Dict[int, Any]] = {}
     for m_u_record in m_u_records:
         comparison_name = m_u_record["output_column_name"]
         level_value = m_u_record["comparison_vector_value"]
         if comparison_name not in lookup:
             lookup[comparison_name] = {}
         if level_value not in lookup[comparison_name]:
             lookup[comparison_name][level_value] = {}
@@ -34,53 +36,53 @@
 def not_trained_message(
     comparison_level: ComparisonLevel, output_column_name: str
 ) -> str:
     cl = comparison_level
     return (
         f"not trained for {output_column_name} - "
         f"{cl.label_for_charts} (comparison vector value: "
-        f"{cl._comparison_vector_value}). This usually means the "
+        f"{cl.comparison_vector_value}). This usually means the "
         "comparison level was never observed in the training data."
     )
 
 
 def append_u_probability_to_comparison_level_trained_probabilities(
     comparison_level: ComparisonLevel,
-    m_u_records_lookup: Dict,
+    m_u_records_lookup: Dict[str, Any],
     output_column_name: str,
     training_description: str,
 ) -> None:
     cl = comparison_level
 
     try:
         u_probability = m_u_records_lookup[output_column_name][
-            cl._comparison_vector_value
+            cl.comparison_vector_value
         ]["u_probability"]
 
     except KeyError:
         u_probability = LEVEL_NOT_OBSERVED_TEXT
 
         logger.info(f"u probability {not_trained_message(cl, output_column_name)}")
     cl._add_trained_u_probability(
         u_probability,
         training_description,
     )
 
 
 def append_m_probability_to_comparison_level_trained_probabilities(
     comparison_level: ComparisonLevel,
-    m_u_records_lookup: Dict,
+    m_u_records_lookup: Dict[str, Any],
     output_column_name: str,
     training_description: str,
 ) -> None:
     cl = comparison_level
 
     try:
         m_probability = m_u_records_lookup[output_column_name][
-            cl._comparison_vector_value
+            cl.comparison_vector_value
         ]["m_probability"]
 
     except KeyError:
         m_probability = LEVEL_NOT_OBSERVED_TEXT
 
         logger.info(f"m probability {not_trained_message(cl, output_column_name)}")
     cl._add_trained_m_probability(
```

### Comparing `splink-4.0.0.dev3/splink/match_key_analysis.py` & `splink-4.0.0.dev4/splink/match_key_analysis.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/misc.py` & `splink-4.0.0.dev4/splink/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,30 +127,14 @@
 
     raise ValueError(
         "'link_type' should be either 'link_only', 'dedupe_only', "
         "or 'link_and_dedupe'"
     )
 
 
-def calculate_reduction_ratio(N, cartesian):
-    """
-    Args:
-        N (int): The number of record pairs generated by a
-            blocking rule.
-        cartesian (int): The cartesian product of your input
-            dataframe(s).
-
-    Generates the reduction ratio. This represents the % reduction
-    in the comparison space as a result of using your given blocking
-    rule. This is a measure of how much the Blocking Rule reduces
-    the total search space.
-    """
-    return 1 - (N / cartesian)
-
-
 def major_minor_version_greater_equal_than(this_version, base_comparison_version):
     this_version = this_version.split(".")[:2]
     this_version = [v.zfill(10) for v in this_version]
 
     base_version = base_comparison_version.split(".")[:2]
     base_version = [v.zfill(10) for v in base_version]
```

### Comparing `splink-4.0.0.dev3/splink/optimise_cost_of_brs.py` & `splink-4.0.0.dev4/splink/optimise_cost_of_brs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,23 @@
+from __future__ import annotations
+
 import logging
 from random import randint
+from typing import TypeVar
 
 import pandas as pd
 
 from .cost_of_blocking_rules import calculate_cost_of_combination_of_brs
 
 logger = logging.getLogger(__name__)
 
+T = TypeVar("T")
+
 
-def localised_shuffle(lst: list, window_percent: float) -> list:
+def localised_shuffle(lst: list[T], window_percent: float) -> list[T]:
     """
     Performs a localised shuffle on a list.
 
     This is used to choose semi-randomly from a list of
     sorted rows, so you tend to pick from items towards the top
 
     Args:
```

### Comparing `splink-4.0.0.dev3/splink/parse_sql.py` & `splink-4.0.0.dev4/splink/parse_sql.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import List, Optional
+from __future__ import annotations
+
+from collections.abc import Sequence
 
 import sqlglot
 import sqlglot.expressions as exp
 from sqlglot.expressions import Bracket, Column, Lambda
 
 from .sql_transform import remove_quotes_from_identifiers
 
@@ -41,30 +43,30 @@
         else:
             column_names.add(column)
 
     return list(column_names)
 
 
 def parse_columns_in_sql(
-    sql: str, sql_dialect: str, remove_quotes=True
-) -> Optional[List[sqlglot.Expression]]:
+    sql: str, sql_dialect: str, remove_quotes: bool = True
+) -> Sequence[exp.Column]:
     """Extract all columns found within a SQL expression.
 
     Args:
         sql (str): A SQL string you wish to parse.
 
     Returns:
         list[exp.Column]: A list of columns as SQLglot expressions. These can be
             unwrapped with `.sql()`. If the input string is unparseable, None will
             be returned.
     """
     try:
         syntax_tree = sqlglot.parse_one(sql, read=sql_dialect)
     except Exception:  # Consider catching a more specific exception if possible
         # If we can't parse a SQL condition, it's better to just pass.
-        return None
+        return []
 
     return [
         # Remove quotes if requested by the user
         remove_quotes_from_identifiers(col) if remove_quotes else col
         for col in syntax_tree.find_all(exp.Column)
     ]
```

### Comparing `splink-4.0.0.dev3/splink/postgres/database_api.py` & `splink-4.0.0.dev4/splink/postgres/database_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import logging
-from typing import List, Union
+from typing import Any, List, Union
 
 import duckdb
 import pandas as pd
-from sqlalchemy import text
+from sqlalchemy import CursorResult, text
 from sqlalchemy.engine import Engine
 
 from ..database_api import DatabaseAPI
 from ..dialects import (
     PostgresDialect,
 )
 from ..misc import (
     ensure_is_list,
 )
 from .dataframe import PostgresDataFrame
 
 logger = logging.getLogger(__name__)
 
 
-class PostgresAPI(DatabaseAPI):
+class PostgresAPI(DatabaseAPI[CursorResult[Any]]):
     sql_dialect = PostgresDialect()
 
     def __init__(
         self,
         engine: Engine,
         schema: str = "splink",
         other_schemas_to_search: Union[str, List[str]] = [],
@@ -87,15 +87,15 @@
         """
 
         rec = self._execute_sql_against_backend(sql).mappings().all()
         return len(rec) > 0
 
     def _execute_sql_against_backend(
         self, final_sql: str, templated_name: str = None, physical_name: str = None
-    ):
+    ) -> CursorResult[Any]:
         with self._engine.begin() as con:
             res = con.execute(text(final_sql))
         return res
 
     # postgres udf registrations:
     def _create_log2_function(self):
         sql = """
```

### Comparing `splink-4.0.0.dev3/splink/postgres/dataframe.py` & `splink-4.0.0.dev4/splink/postgres/dataframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,17 +28,17 @@
         """
         res = self.db_api._execute_sql_against_backend(sql).mappings().all()
         cols = [r["column_name"] for r in res]
 
         return [InputColumn(c, sql_dialect="postgres") for c in cols]
 
     def validate(self):
-        if type(self.physical_name) is not str:
+        if not isinstance(self.physical_name, str):
             raise ValueError(
-                f"{self.df_name} is not a string dataframe.\n"
+                f"{self.templated_name} is not a string dataframe.\n"
                 "Postgres Linker requires input data"
                 " to be a string containing the name of the"
                 " postgres table."
             )
 
         sql = f"""
         SELECT table_name
```

### Comparing `splink-4.0.0.dev3/splink/predict.py` & `splink-4.0.0.dev4/splink/predict.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 def predict_from_comparison_vectors_sqls_using_settings(
     settings_obj: Settings,
     threshold_match_probability: float = None,
     threshold_match_weight: float = None,
     include_clerical_match_score: bool = False,
     sql_infinity_expression: str = "'infinity'",
-) -> list[dict]:
+) -> list[dict[str, str]]:
     return predict_from_comparison_vectors_sqls(
         unique_id_input_columns=settings_obj.column_info_settings.unique_id_input_columns,
         core_model_settings=settings_obj.core_model_settings,
         sql_dialect=settings_obj._sql_dialect,
         threshold_match_probability=threshold_match_probability,
         threshold_match_weight=threshold_match_weight,
         retain_matching_columns=settings_obj._retain_matching_columns,
@@ -45,15 +45,15 @@
     retain_matching_columns: bool = False,
     retain_intermediate_calculation_columns: bool = False,
     training_mode: bool = False,
     additional_columns_to_retain: List[InputColumn] = [],
     needs_matchkey_column: bool = False,
     include_clerical_match_score: bool = False,
     sql_infinity_expression: str = "'infinity'",
-) -> list[dict]:
+) -> list[dict[str, str]]:
     sqls = []
 
     select_cols = Settings.columns_to_select_for_bayes_factor_parts(
         unique_id_input_columns=unique_id_input_columns,
         comparisons=core_model_settings.comparisons,
         retain_matching_columns=retain_matching_columns,
         retain_intermediate_calculation_columns=retain_intermediate_calculation_columns,
@@ -136,16 +136,16 @@
 
     return sqls
 
 
 def predict_from_agreement_pattern_counts_sqls(
     comparisons: List[Comparison],
     probability_two_random_records_match: float,
-    sql_infinity_expression="'infinity'",
-) -> list[dict]:
+    sql_infinity_expression: str = "'infinity'",
+) -> list[dict[str, str]]:
     sqls = []
 
     select_cols = []
 
     for cc in comparisons:
         cc_sqls = [
             cl._bayes_factor_sql(cc._gamma_column_name) for cl in cc.comparison_levels
```

### Comparing `splink-4.0.0.dev3/splink/profile_data.py` & `splink-4.0.0.dev4/splink/internals/profile_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import logging
 import re
 from copy import deepcopy
+from typing import List, Optional, Sequence, Union
 
-from .charts import altair_or_json, load_chart_definition
-from .misc import ensure_is_list
-from .pipeline import SQLPipeline
+from ..charts import ChartReturnType, altair_or_json, load_chart_definition
+from ..column_expression import ColumnExpression
+from ..database_api import AcceptableInputTableType, DatabaseAPISubClass
+from ..misc import ensure_is_list
+from ..pipeline import CTEPipeline
+from ..vertically_concatenate import vertically_concatenate_sql
 
 logger = logging.getLogger(__name__)
 
 
 def _group_name(cols_or_expr):
     cols_or_expr = re.sub(r"[^0-9a-zA-Z_]", " ", cols_or_expr)
     cols_or_expr = re.sub(r"\s+", "_", cols_or_expr)
@@ -47,27 +51,27 @@
     sub = (
         f"In this col, {total_rows_inc_nulls*(1-perc):,.0f} values "
         f"({1-perc:,.1%}) are null and there are "
         f"{distinct_value_count} distinct values"
     )
     sub = sub.format(**percentile_data[0])
     inner_spec["hconcat"][0]["data"]["values"] = percentile_data
-    inner_spec["hconcat"][0]["title"][
-        "text"
-    ] = f"Distribution of counts of values in column {col_name}"
+    inner_spec["hconcat"][0]["title"]["text"] = (
+        f"Distribution of counts of values in column {col_name}"
+    )
 
     inner_spec["hconcat"][0]["title"]["subtitle"] = sub
 
     inner_spec["hconcat"][1]["data"]["values"] = top_n_data
     inner_spec["hconcat"][1]["title"] = f"Top {len(top_n_data)} values by value count"
 
     inner_spec["hconcat"][2]["data"]["values"] = bottom_n_data
-    inner_spec["hconcat"][2][
-        "title"
-    ] = f"Bottom {len(bottom_n_data)} values by value count"
+    inner_spec["hconcat"][2]["title"] = (
+        f"Bottom {len(bottom_n_data)} values by value count"
+    )
 
     max_val = top_n_data[0]["value_count"]
     inner_spec["hconcat"][2]["encoding"]["y"]["scale"] = {"domain": [0, max_val]}
 
     return inner_spec
 
 
@@ -149,19 +153,19 @@
         gn = _group_name(col_or_expr)
 
         # If the supplied column string is a list of columns to be concatenated,
         # add a quick clause to filter out any instances whereby either column contains
         # a null value.
         if isinstance(raw_expr, list):
             null_exprs = [f"{c} is null" for c in raw_expr]
-            null_exprs = " OR ".join(null_exprs)
+            null_expr_str = " OR ".join(null_exprs)
 
             col_or_expr = f"""
                 case when
-                {null_exprs} then null
+                {null_expr_str} then null
                 else
                 {col_or_expr}
                 end
             """
 
         sql = f"""
         select * from
@@ -191,16 +195,20 @@
         first_row["percentile_ex_nulls"] = 1.0
 
     percentile_rows.append(first_row)
     return percentile_rows
 
 
 def profile_columns(
-    table_or_tables, db_api, column_expressions=None, top_n=10, bottom_n=10
-):
+    table_or_tables: Sequence[AcceptableInputTableType],
+    db_api: DatabaseAPISubClass,
+    column_expressions: Optional[List[Union[str, ColumnExpression]]] = None,
+    top_n: int = 10,
+    bottom_n: int = 10,
+) -> Optional[ChartReturnType]:
     """
     Profiles the specified columns of the dataframe initiated with the linker.
 
     This can be computationally expensive if the dataframe is large.
 
     For the provided columns with column_expressions (or for all columns if left empty)
     calculate:
@@ -211,15 +219,15 @@
     n values within the column
 
     This should be used to explore the dataframe, determine if columns have
     sufficient completeness for linking, analyse the cardinality of columns, and
     identify the need for standardisation within a given column.
 
     Args:
-        linker (object): The initiated linker.
+
         column_expressions (list, optional): A list of strings containing the
             specified column names.
             If left empty this will default to all columns.
         top_n (int, optional): The number of top n values to plot.
         bottom_n (int, optional): The number of bottom n values to plot.
 
     Returns:
@@ -230,73 +238,72 @@
         - The `linker` object should be an instance of the initiated linker.
         - The provided `column_expressions` can be a list of column names to profile.
             If left empty, all columns will be profiled.
         - The `top_n` and `bottom_n` parameters determine the number of top and bottom
             values to display in the respective charts.
     """
 
-    tables = ensure_is_list(table_or_tables)
+    splink_df_dict = db_api.register_multiple_tables(table_or_tables)
 
-    tables = db_api.process_input_tables(tables)
+    pipeline = CTEPipeline()
+    sql = vertically_concatenate_sql(
+        splink_df_dict, salting_required=False, source_dataset_column_name=None
+    )
+    pipeline.enqueue_sql(sql, "__splink__df_concat")
 
-    splink_df_dict = db_api.register_multiple_tables(tables)
     input_dataframes = list(splink_df_dict.values())
-    input_aliases = list(splink_df_dict.keys())
+
     input_columns = input_dataframes[0].columns_escaped
 
     if not column_expressions:
         column_expressions_raw = input_columns
     else:
         column_expressions_raw = ensure_is_list(column_expressions)
-    column_expressions = expressions_to_sql(column_expressions_raw)
-
-    pipeline = SQLPipeline()
 
-    cols_to_select = ", ".join(input_columns)
-    template = """
-    select {cols_to_select}
-    from {table_name}
-    """
-
-    sql_df_concat = " UNION ALL".join(
-        [
-            template.format(cols_to_select=cols_to_select, table_name=table_name)
-            for table_name in input_aliases
-        ]
-    )
+    # If the user has provided any ColumnExpression, convert to string
+    for i in column_expressions_raw:
+        if isinstance(i, ColumnExpression):
+            i.sql_dialect = db_api.sql_dialect
+
+    column_expressions_raw = [
+        ce.name if isinstance(ce, ColumnExpression) else ce
+        for ce in column_expressions_raw
+    ]
 
-    pipeline.enqueue_sql(sql_df_concat, "__splink__df_concat")
+    column_expressions_as_sql = expressions_to_sql(column_expressions_raw)
 
     sql = _col_or_expr_frequencies_raw_data_sql(
         column_expressions_raw, "__splink__df_concat"
     )
 
     pipeline.enqueue_sql(sql, "__splink__df_all_column_value_frequencies")
-    df_raw = db_api.sql_pipeline_to_splink_dataframe(pipeline, input_dataframes)
+    df_raw = db_api.sql_pipeline_to_splink_dataframe(pipeline)
 
+    pipeline = CTEPipeline(input_dataframes=[df_raw])
     sqls = _get_df_percentiles()
-    for sql in sqls:
-        pipeline.enqueue_sql(sql["sql"], sql["output_table_name"])
+    pipeline.enqueue_list_of_sqls(sqls)
 
-    df_percentiles = db_api.sql_pipeline_to_splink_dataframe(pipeline, [df_raw])
+    df_percentiles = db_api.sql_pipeline_to_splink_dataframe(pipeline)
     percentile_rows_all = df_percentiles.as_record_dict()
 
-    sql = _get_df_top_bottom_n(column_expressions, top_n, "desc")
+    pipeline = CTEPipeline(input_dataframes=[df_raw])
+    sql = _get_df_top_bottom_n(column_expressions_as_sql, top_n, "desc")
     pipeline.enqueue_sql(sql, "__splink__df_top_n")
-    df_top_n = db_api.sql_pipeline_to_splink_dataframe(pipeline, [df_raw])
+    df_top_n = db_api.sql_pipeline_to_splink_dataframe(pipeline)
     top_n_rows_all = df_top_n.as_record_dict()
 
-    sql = _get_df_top_bottom_n(column_expressions, bottom_n, "asc")
+    pipeline = CTEPipeline(input_dataframes=[df_raw])
+    sql = _get_df_top_bottom_n(column_expressions_as_sql, bottom_n, "asc")
     pipeline.enqueue_sql(sql, "__splink__df_bottom_n")
-    df_bottom_n = db_api.sql_pipeline_to_splink_dataframe(pipeline, [df_raw])
+    df_bottom_n = db_api.sql_pipeline_to_splink_dataframe(pipeline)
     bottom_n_rows_all = df_bottom_n.as_record_dict()
 
     inner_charts = []
 
-    for expression in column_expressions:
+    for expression in column_expressions_as_sql:
         percentile_rows = [
             p for p in percentile_rows_all if p["group_name"] == _group_name(expression)
         ]
         if percentile_rows == []:
             logger.warning(
                 "Warning: No charts produced for "
                 f"{expression}"
```

### Comparing `splink-4.0.0.dev3/splink/settings.py` & `splink-4.0.0.dev4/splink/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 from copy import deepcopy
 from dataclasses import asdict, dataclass
-from typing import List, TypedDict
+from typing import Any, List, Literal, Sequence, TypedDict
 
 from .blocking import BlockingRule, SaltedBlockingRule, blocking_rule_to_obj
 from .charts import m_u_parameters_chart, match_weights_chart
 from .comparison import Comparison
 from .comparison_level import ComparisonLevel
 from .input_column import InputColumn
 from .misc import dedupe_preserving_order, prob_to_bayes_factor, prob_to_match_weight
@@ -36,14 +36,33 @@
     def source_dataset_column_name(self):
         if self._source_dataset_column_name_is_required:
             return self._source_dataset_column_name
         else:
             return None
 
     @property
+    def source_dataset_input_column(self):
+        if self._source_dataset_column_name_is_required:
+            return InputColumn(
+                self._source_dataset_column_name,
+                column_info_settings=self,
+                sql_dialect=self.sql_dialect,
+            )
+        else:
+            return None
+
+    @property
+    def unique_id_input_column(self):
+        return InputColumn(
+            self.unique_id_column_name,
+            column_info_settings=self,
+            sql_dialect=self.sql_dialect,
+        )
+
+    @property
     def unique_id_input_columns(self) -> list[InputColumn]:
         cols = []
 
         if source_dataset_column_name := (self.source_dataset_column_name):
             col = InputColumn(
                 source_dataset_column_name,
                 column_info_settings=self,
@@ -56,31 +75,31 @@
             column_info_settings=self,
             sql_dialect=self.sql_dialect,
         )
         cols.append(col)
 
         return cols
 
-    def as_dict(self) -> dict:
+    def as_dict(self) -> dict[str, Any]:
         full_dict = self._as_full_dict()
         full_dict["source_dataset_column_name"] = self._source_dataset_column_name
         del full_dict["_source_dataset_column_name"]
         del full_dict["_source_dataset_column_name_is_required"]
         return full_dict
 
-    def _as_full_dict(self) -> dict:
+    def _as_full_dict(self) -> dict[str, Any]:
         return asdict(self)
 
 
 @dataclass(frozen=True)
 class TrainingSettings:
     em_convergence: float
     max_iterations: int
 
-    def as_dict(self) -> dict:
+    def as_dict(self) -> dict[str, float]:
         naive_dict = asdict(self)
         return naive_dict
 
 
 @dataclass
 class CoreModelSettings:
     comparisons: List[Comparison]
@@ -129,28 +148,37 @@
             "bayes_factor_description": prior_description,
             "probability_two_random_records_match": rr_match,
             "comparison_sort_order": -1,
         }
         output.insert(0, prop_record)
         return output
 
-    def get_comparison_by_output_column_name(self, name) -> Comparison:
+    def get_comparison_by_output_column_name(self, name: str) -> Comparison:
         for cc in self.comparisons:
             if cc.output_column_name == name:
                 return cc
         raise ValueError(f"No comparison column with name {name}")
 
 
+LinkTypeLiteralType = Literal[
+    "two_dataset_link_only",
+    "self_link",
+    "link_only",
+    "link_and_dedupe",
+    "dedupe_only",
+]
+
+
 class Settings:
     """The settings object contains the configuration and parameters of the data
     linking model"""
 
     def __init__(
         self,
-        link_type: str,
+        link_type: LinkTypeLiteralType,
         *,
         # TODO: make everything compulsory at this level?
         comparisons: List[Comparison] = [],
         blocking_rules_to_generate_predictions: List[BlockingRule] = [],
         probability_two_random_records_match: float = 0.0001,
         retain_matching_columns: bool = True,
         retain_intermediate_calculation_columns: bool = False,
@@ -236,23 +264,23 @@
     # TODO: unpick these four
     @property
     def comparisons(self) -> List[Comparison]:
         return self.core_model_settings.comparisons
 
     # TODO: especially factor the setters
     @comparisons.setter
-    def comparisons(self, value) -> None:
+    def comparisons(self, value: list[Comparison]) -> None:
         self.core_model_settings.comparisons = value
 
     @property
     def _probability_two_random_records_match(self) -> float:
         return self.core_model_settings.probability_two_random_records_match
 
     @_probability_two_random_records_match.setter
-    def _probability_two_random_records_match(self, value) -> None:
+    def _probability_two_random_records_match(self, value: float) -> None:
         self.core_model_settings.probability_two_random_records_match = value
 
     @property
     def _additional_column_names_to_retain(self) -> List[str]:
         cols_to_retain = []
 
         # Add any columns used in blocking rules but not model
@@ -265,17 +293,17 @@
                 )
 
             used_by_brs = [InputColumn(c) for c in used_by_brs]
 
             used_by_brs = [c.unquote().name for c in used_by_brs]
             already_used_names = self._columns_used_by_comparisons
             already_used = [InputColumn(c) for c in already_used_names]
-            already_used = [c.unquote().name for c in already_used]
+            already_used_names = [c.unquote().name for c in already_used]
 
-            new_cols = list(set(used_by_brs) - set(already_used))
+            new_cols = list(set(used_by_brs) - set(already_used_names))
             cols_to_retain.extend(new_cols)
 
         cols_to_retain.extend(self._additional_col_names_to_retain)
         return cols_to_retain
 
     @property
     def _additional_columns_to_retain(self) -> List[InputColumn]:
@@ -444,18 +472,20 @@
 
         if needs_matchkey_column:
             cols.append("match_key")
 
         cols = dedupe_preserving_order(cols)
         return cols
 
-    def _get_comparison_by_output_column_name(self, name) -> Comparison:
+    def _get_comparison_by_output_column_name(self, name: str) -> Comparison:
         return self.core_model_settings.get_comparison_by_output_column_name(name)
 
-    def _brs_as_objs(self, brs_as_strings) -> List[BlockingRule]:
+    def _brs_as_objs(
+        self, brs_as_strings: Sequence[str | BlockingRule]
+    ) -> List[BlockingRule]:
         brs_as_objs = [blocking_rule_to_obj(br) for br in brs_as_strings]
         for n, br in enumerate(brs_as_objs):
             br.add_preceding_rules(brs_as_objs[:n])
         return brs_as_objs
 
     # TODO: is this the most logical place for this to live now it's static?
     @staticmethod
@@ -523,15 +553,15 @@
         for i, cc in enumerate(self.comparisons):
             records = cc._parameter_estimates_as_records
             for r in records:
                 r["comparison_sort_order"] = i
             output.extend(records)
         return output
 
-    def _simple_dict_entries(self) -> dict:
+    def _simple_dict_entries(self) -> dict[str, Any]:
         return {
             "link_type": self._link_type,
             "probability_two_random_records_match": (
                 self._probability_two_random_records_match
             ),
             "retain_matching_columns": self._retain_matching_columns,
             "retain_intermediate_calculation_columns": (
@@ -632,22 +662,27 @@
         return messages
 
     @property
     def human_readable_description(self):
         comparison_descs = [
             c._human_readable_description_succinct for c in self.comparisons
         ]
-        comparison_descs = "\n".join(comparison_descs)
+        comparison_desc_str = "\n".join(comparison_descs)
         desc = (
             "SUMMARY OF LINKING MODEL\n"
             "------------------------\n"
             "The similarity of pairwise record comparison in your model will be "
-            f"assessed as follows:\n\n{comparison_descs}"
+            f"assessed as follows:\n\n{comparison_desc_str}"
         )
         return desc
 
     @property
     def salting_required(self):
+        # see https://github.com/duckdb/duckdb/discussions/9710
+        # in duckdb to parallelise we need salting
+        if self._sql_dialect == "duckdb":
+            return True
+
         for br in self._blocking_rules_to_generate_predictions:
             if isinstance(br, SaltedBlockingRule):
                 return True
         return False
```

### Comparing `splink-4.0.0.dev3/splink/settings_creator.py` & `splink-4.0.0.dev4/splink/settings_creator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,42 @@
 from __future__ import annotations
 
 import json
 from copy import deepcopy
 from dataclasses import asdict, dataclass, field
 from pathlib import Path
-from typing import List, Union
+from typing import Any, List, Literal, Union
 
 from .blocking_rule_creator import BlockingRuleCreator
-from .blocking_rule_library import CustomRule
+from .blocking_rule_creator_utils import to_blocking_rule_creator
 from .comparison_creator import ComparisonCreator
 from .comparison_library import CustomComparison
 from .settings import Settings
 
 
 def to_comparison_creator(comparison_creator):
     if isinstance(comparison_creator, dict):
         return CustomComparison(**comparison_creator)
     return comparison_creator
 
 
-def to_blocking_rule_creator(blocking_rule_creator):
-    if isinstance(blocking_rule_creator, dict):
-        return CustomRule(**blocking_rule_creator)
-    if isinstance(blocking_rule_creator, str):
-        return CustomRule(blocking_rule_creator)
-    return blocking_rule_creator
-
-
 @dataclass
 class SettingsCreator:
     """
     Non-dialected version of Settings.
     Responsible for authoring Settings, but not implementing anything
     """
 
-    link_type: str
+    link_type: Literal["link_only", "link_and_dedupe", "dedupe_only"]
+
     # TODO: make this compulsory once we farm more stuff out of linker
-    comparisons: List[ComparisonCreator | dict] = field(default_factory=list)
-    blocking_rules_to_generate_predictions: List[BlockingRuleCreator | dict] = field(
-        default_factory=list
-    )
+    comparisons: List[ComparisonCreator | dict[str, Any]] = field(default_factory=list)
+    blocking_rules_to_generate_predictions: List[
+        BlockingRuleCreator | dict[str, Any]
+    ] = field(default_factory=list)
 
     probability_two_random_records_match: float = 0.0001
     em_convergence: float = 0.0001
     max_iterations: int = 25
 
     retain_matching_columns: bool = True
     retain_intermediate_calculation_columns: bool = False
@@ -53,24 +46,24 @@
     source_dataset_column_name: str = "source_dataset"
     bayes_factor_column_prefix: str = "bf_"
     term_frequency_adjustment_column_prefix: str = "tf_"
     comparison_vector_value_column_prefix: str = "gamma_"
 
     linker_uid: str | None = None
 
-    def _as_naive_dict(self) -> dict:
+    def _as_naive_dict(self) -> dict[str, Any]:
         """
         Returns this class as a naive dict.
         Naive in the sense that we do not process the attributes in any way.
 
         In particular blocking rules and comparisons could be dicts _or_ creator objects
         """
         return asdict(self)
 
-    def _as_creator_dict(self) -> dict:
+    def _as_creator_dict(self) -> dict[str, Any]:
         """
         Returns class as a dict where we have converted any sub-dicts into
         'creator' types
         """
         creator_dict = self._as_naive_dict()
         # we adjust dict to ensure that comparisons + blocking rules are
         # consistently of creatore types
@@ -82,30 +75,30 @@
             to_blocking_rule_creator(blocking_rule_creator)
             for blocking_rule_creator in creator_dict[
                 "blocking_rules_to_generate_predictions"
             ]
         ]
         return creator_dict
 
-    def create_settings_dict(self, sql_dialect_str: str) -> dict:
+    def create_settings_dict(self, sql_dialect_str: str) -> dict[str, Any]:
         creator_dict = self._as_creator_dict()
         # then we process 'creator' types into dialected dicts
         creator_dict["comparisons"] = [
             comparison_creator.create_comparison_dict(sql_dialect_str)
             for comparison_creator in creator_dict["comparisons"]
         ]
         creator_dict["blocking_rules_to_generate_predictions"] = [
             blocking_rule_creator.create_blocking_rule_dict(sql_dialect_str)
             for blocking_rule_creator in creator_dict[
                 "blocking_rules_to_generate_predictions"
             ]
         ]
         return creator_dict
 
-    def get_settings(self, sql_dialect_str) -> Settings:
+    def get_settings(self, sql_dialect_str: str) -> Settings:
         creator_dict = self._as_creator_dict()
         # then we process 'creator' types into dialected concrete types
         creator_dict["comparisons"] = [
             comparison_creator.get_comparison(sql_dialect_str)
             for comparison_creator in creator_dict["comparisons"]
         ]
         creator_dict["blocking_rules_to_generate_predictions"] = [
@@ -113,20 +106,20 @@
             for blocking_rule_creator in creator_dict[
                 "blocking_rules_to_generate_predictions"
             ]
         ]
         return Settings(**creator_dict, sql_dialect=sql_dialect_str)
 
     @classmethod
-    def from_path_or_dict(cls, path_or_dict: Union[Path, str, dict]) -> SettingsCreator:
-
+    def from_path_or_dict(
+        cls, path_or_dict: Union[Path, str, dict[str, Any]]
+    ) -> SettingsCreator:
         if isinstance(path_or_dict, (str, Path)):
             settings_path = Path(path_or_dict)
             if settings_path.is_file():
-
                 settings_dict = json.loads(settings_path.read_text())
 
                 # TODO: remove this once we have sorted spec
                 for br in settings_dict["blocking_rules_to_generate_predictions"]:
                     if isinstance(br, dict):
                         if "sql_dialect" in br:
                             del br["sql_dialect"]
@@ -139,15 +132,11 @@
             settings_dict = deepcopy(path_or_dict)
         else:
             raise TypeError(
                 f"Argument {path_or_dict=} must be of type `pathlib.Path`, "
                 f"`str`, or `dict`.  Found type {type(path_or_dict)}"
             )
 
-        # TODO: need to figure out how this flows with validation
-        # for now we instantiate all the correct types before the validator sees it
-        # self._validate_settings_components(settings)
-
         # TODO: should SettingsCreator deal with the logic of sql_dialect being
         # set?
         settings_dict.pop("sql_dialect", None)
         return SettingsCreator(**settings_dict)
```

### Comparing `splink-4.0.0.dev3/splink/settings_validation/log_invalid_columns.py` & `splink-4.0.0.dev4/splink/settings_validation/log_invalid_columns.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import logging
-from typing import TYPE_CHECKING, Callable, List
+from collections.abc import Sequence
+from typing import TYPE_CHECKING, Iterable, Protocol
 
 import sqlglot
+import sqlglot.expressions
 
 from ..comparison import Comparison
 from ..parse_sql import parse_columns_in_sql
 from .settings_column_cleaner import (
     SettingsColumnCleaner,
     clean_and_find_columns_not_in_input_dfs,
     find_columns_not_in_input_dfs,
@@ -24,62 +26,69 @@
 if TYPE_CHECKING:
     from .settings_validation_log_strings import InvalidColumnsLogGenerator
 
 
 logger = logging.getLogger(__name__)
 
 
+class Validator(Protocol):
+    def __call__(
+        self, columns_to_check: Sequence[sqlglot.expressions.Column]
+    ) -> InvalidColumnsLogGenerator: ...
+
+
 def validate_table_names(
-    columns_to_check: list[sqlglot.expressions],
+    columns_to_check: Sequence[sqlglot.expressions.Column],
 ) -> InvalidColumnsLogGenerator:
     """Validate a series of table names assigned to columns extracted from
     SQL statements. We expect all columns to be assigned either a `l` or
     `r` prefix.
     """
     # list of valid columns
     invalid_columns = [c.sql() for c in columns_to_check if c.table not in ["l", "r"]]
     return InvalidTableNamesLogGenerator(set(invalid_columns))
 
 
 def validate_column_suffixes(
-    columns_to_check: list[sqlglot.expressions],
+    columns_to_check: Sequence[sqlglot.expressions.Column],
 ) -> InvalidColumnsLogGenerator:
     """Validate a series of column suffixes. We expect columns to be suffixed
     with either `_l` or `_r`. Where this is missing, flag it as an error.
     """
     # list of valid columns
     invalid_columns = [
         c.sql() for c in columns_to_check if not c.sql().endswith(("_l", "_r"))
     ]
     return InvalidColumnSuffixesLogGenerator(set(invalid_columns))
 
 
 def check_for_missing_settings_column(
     settings_id: str,
-    settings_column_to_check: set,
-    valid_input_dataframe_columns: list,
-):
+    settings_column_to_check: Iterable[str],
+    valid_input_dataframe_columns: Iterable[str],
+) -> tuple[str, InvalidColumnsLogGenerator] | None:
     """Validate simple settings columns with strings as input.
     i.e. Anything that doesn't require SQL to be parsed.
     """
     missing_columns = find_columns_not_in_input_dfs(
         valid_input_dataframe_columns, columns_to_check=settings_column_to_check
     )
 
     if missing_columns:
         # If the column is missing, return an InvalidColumnsTracker
         return settings_id, MissingColumnsLogGenerator(missing_columns)
+    return None
 
 
 def check_for_missing_or_invalid_columns_in_sql_strings(
     sql_dialect: str,
-    sql_strings: list[str],
-    valid_input_dataframe_columns: list[str],
-    additional_validation_checks: List[Callable] = [],
-) -> list[MissingColumnsLogGenerator]:
+    sql_strings: Iterable[str],
+    valid_input_dataframe_columns: Iterable[str],
+    additional_validation_checks: list[Validator] = [],
+) -> dict[str, list[InvalidColumnsLogGenerator]]:
     """Evaluate whether the column(s) supplied in a series of SQL strings
     exist in our raw data.
 
     This is used to assess whether a blocking rule or comparison level
     contains columns that exist in the underlying dataset(s) supplied.
 
     Args:
@@ -111,16 +120,16 @@
         # Check for missing columns
         missing_columns = clean_and_find_columns_not_in_input_dfs(
             valid_input_dataframe_columns=valid_input_dataframe_columns,
             sqlglot_tree_columns_to_check=identified_columns_in_sql,
             sql_dialect=sql_dialect,
         )
         if missing_columns:
-            missing_columns = MissingColumnsLogGenerator(missing_columns)
-            invalid_column_tracker.append(missing_columns)
+            missing_columns_log_gen = MissingColumnsLogGenerator(missing_columns)
+            invalid_column_tracker.append(missing_columns_log_gen)
 
         # Run any additional validations checks.
         # Skipped if no additional checks are requested
         for validation_check_to_run in additional_validation_checks:
             validated_columns = validation_check_to_run(
                 columns_to_check=identified_columns_in_sql
             )
@@ -135,17 +144,17 @@
             validation_dict[sql_string] = invalid_column_tracker
 
     return validation_dict
 
 
 def check_comparison_for_missing_or_invalid_sql_strings(
     sql_dialect: str,
-    comparisons_to_check: list[Comparison],
-    valid_input_dataframe_columns: list[str],
-) -> list[MissingColumnsLogGenerator]:
+    comparisons_to_check: Iterable[Comparison],
+    valid_input_dataframe_columns: Iterable[str],
+) -> list[tuple[str, dict[str, list[InvalidColumnsLogGenerator]]]]:
     """Split apart the comparison levels found within a comparison
     and review the SQL contained within.
 
     If any errors are identified, log them in the invalid_column_tracker.
     """
     invalid_column_tracker = []
     for comparison in comparisons_to_check:
@@ -173,44 +182,46 @@
     Construct a series of log strings indicating where columns in a settings object
     are missing from the user's input dataframe(s).
     """
 
     def __init__(self, cleaned_settings: SettingsColumnCleaner):
         self.cleaned_settings_values = cleaned_settings
 
-    def validate_uid(self):
+    def validate_uid(self) -> tuple[str, InvalidColumnsLogGenerator] | None:
         return check_for_missing_settings_column(
             settings_id="unique_id_column_name",
             settings_column_to_check=self.cleaned_settings_values.uid,
             valid_input_dataframe_columns=self.cleaned_settings_values.input_columns,
         )
 
-    def validate_cols_to_retain(self):
+    def validate_cols_to_retain(self) -> tuple[str, InvalidColumnsLogGenerator] | None:
         return check_for_missing_settings_column(
             settings_id="additional_columns_to_retain",
             settings_column_to_check=self.cleaned_settings_values.cols_to_retain,
             valid_input_dataframe_columns=self.cleaned_settings_values.input_columns,
         )
 
-    def validate_blocking_rules(self):
+    def validate_blocking_rules(self) -> dict[str, list[InvalidColumnsLogGenerator]]:
         return check_for_missing_or_invalid_columns_in_sql_strings(
             sql_dialect=self.cleaned_settings_values.sql_dialect,
             sql_strings=self.cleaned_settings_values.blocking_rules,
             valid_input_dataframe_columns=self.cleaned_settings_values.input_columns,
             additional_validation_checks=[validate_table_names],
         )
 
-    def validate_comparison_levels(self):
+    def validate_comparison_levels(
+        self,
+    ) -> list[tuple[str, dict[str, list[InvalidColumnsLogGenerator]]]]:
         return check_comparison_for_missing_or_invalid_sql_strings(
             sql_dialect=self.cleaned_settings_values.sql_dialect,
             comparisons_to_check=self.cleaned_settings_values.comparisons,
             valid_input_dataframe_columns=self.cleaned_settings_values.input_columns,
         )
 
-    def construct_output_logs(self, run_settings_validations=True):
+    def construct_output_logs(self, run_settings_validations: bool = True) -> None:
         if not run_settings_validations:
             return
 
         missing_uid = self.validate_uid()
         missing_cols_to_retain = self.validate_cols_to_retain()
         invalid_blocking_rules = self.validate_blocking_rules()
         invalid_comparison_levels = self.validate_comparison_levels()
@@ -219,23 +230,23 @@
         log_strings = (
             construct_missing_settings_column_log(missing_uid),
             construct_missing_settings_column_log(missing_cols_to_retain),
             construct_missing_column_in_blocking_rule_log(invalid_blocking_rules),
             construct_missing_column_in_comparison_level_log(invalid_comparison_levels),
         )
         # Remove anything that doesn't need validation
-        log_strings = [log_string for log_string in log_strings if log_string]
+        log_string_list = [log_string for log_string in log_strings if log_string]
 
-        if log_strings:  # if nothing needs logging, return
+        if log_string_list:  # if nothing needs logging, return
             # Initial warning for the logger
             logger.warning(
                 "SETTINGS VALIDATION: Errors were identified in your "
                 "settings dictionary. \n"
             )
 
-            for log_string in log_strings:
+            for log_string in log_string_list:
                 logger.warning(log_string)
 
             logger.warning(
                 "You may want to verify your settings dictionary has "
                 "valid inputs in all fields before continuing."
             )
```

### Comparing `splink-4.0.0.dev3/splink/settings_validation/settings_column_cleaner.py` & `splink-4.0.0.dev4/splink/settings_validation/settings_column_cleaner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 from __future__ import annotations
 
 import logging
 import re
+from collections.abc import Sequence
 from copy import deepcopy
 from functools import reduce
 from operator import and_
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING, Iterable, List, Literal, overload
 
 import sqlglot
 
 from ..input_column import InputColumn
+from ..splink_dataframe import SplinkDataFrame
 
 logger = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     from ..settings import Settings
 
 
-def remove_suffix(c):
+def remove_suffix(c: str) -> str:
     return re.sub("_[l|r]{1}$", "", c)
 
 
 def find_columns_not_in_input_dfs(
-    valid_input_dataframe_columns: list, columns_to_check: set
+    valid_input_dataframe_columns: Iterable[str], columns_to_check: Iterable[str] | str
 ) -> set[str]:
     """Identify missing columns in the input dataframe(s). This function
     does not apply any cleaning to the input column(s).
     """
     # the key to use when producing our warning logs
-    if type(columns_to_check) == str:
-        columns_to_check = [columns_to_check]
+    if isinstance(columns_to_check, str):
+        columns_to_check = {columns_to_check}
 
     return {col for col in columns_to_check if col not in valid_input_dataframe_columns}
 
 
 def clean_and_find_columns_not_in_input_dfs(
-    valid_input_dataframe_columns: list,
-    sqlglot_tree_columns_to_check: list[sqlglot.expressions],
+    valid_input_dataframe_columns: Iterable[str],
+    sqlglot_tree_columns_to_check: Sequence[sqlglot.Expression],
     sql_dialect: str,
 ) -> set[str]:
     """Clean a list of sqlglot column names to remove the prefix (l.)
     and suffix (_l) and then return any that are missing from the
     input dataframe(s).
     """
     sqlglot_tree_columns_to_check = deepcopy(sqlglot_tree_columns_to_check)
@@ -48,76 +50,96 @@
         remove_prefix_and_suffix_from_column(c, sql_dialect=sql_dialect)
         for c in sqlglot_tree_columns_to_check
     )
     return find_columns_not_in_input_dfs(valid_input_dataframe_columns, cleaned_cols)
 
 
 def remove_prefix_and_suffix_from_column(
-    col_syntax_tree: sqlglot.expressions,
+    col_syntax_tree: sqlglot.Expression,
     sql_dialect: str,
-):
+) -> str:
     """Remove the prefix and suffix from a given sqlglot syntax tree
     and return it as a string of SQL.
 
     Args:
-        col_syntax_tree (sqlglot.expressions): _description_
+        col_syntax_tree (sqlglot.Expression): _description_
 
     Returns:
         str: A column without `l.` and/or `_l`
     """
     col_syntax_tree.args["table"] = None
     return remove_suffix(col_syntax_tree.sql(sql_dialect))
 
 
-def clean_list_of_column_names(col_list: List[InputColumn]):
+def clean_list_of_column_names(col_list: List[InputColumn]) -> set[str]:
     """Clean a list of columns names by removing the quote characters
     that may exist.
 
     Args:
         col_list (list): A list of InputColumn classes.
     """
     if col_list is None:
         return ()  # needs to be a blank iterable
 
     return set((c.unquote().name for c in col_list))
 
 
-def clean_user_input_columns(input_columns: dict, return_as_single_column: bool = True):
+@overload
+def clean_user_input_columns(
+    input_columns: dict[str, SplinkDataFrame], return_as_single_column: Literal[True]
+) -> set[str]: ...
+
+
+@overload
+def clean_user_input_columns(
+    input_columns: dict[str, SplinkDataFrame], return_as_single_column: Literal[False]
+) -> dict[str, set[str]]: ...
+
+
+def clean_user_input_columns(
+    input_columns: dict[str, SplinkDataFrame], return_as_single_column: bool = True
+) -> set[str] | dict[str, set[str]]:
     """A dictionary containing all input dataframes and the columns located
     within.
 
     Returns:
         dict: A dictionary of the format `{"table_name": [col1, col2, ...]}
     """
     # For each input dataframe, grab the column names and create a dictionary
     # of the form: {table_name: [column_1, column_2, ...]}
-    input_columns = {k: clean_list_of_column_names(v.columns) for k, v in input_columns}
+    cleaned_columns = {
+        k: clean_list_of_column_names(v.columns) for k, v in input_columns.items()
+    }
 
     if return_as_single_column:
-        return reduce(and_, input_columns.values())
+        return reduce(and_, cleaned_columns.values())
     else:
-        return input_columns
+        return cleaned_columns
 
 
 class SettingsColumnCleaner:
     """
     A class that takes in a linker's settings object and spits out a series of
     cleaned up settings columns and SQL strings.
     """
 
-    def __init__(self, settings_object: Settings, input_columns: dict):
+    def __init__(
+        self, settings_object: Settings, input_columns: dict[str, SplinkDataFrame]
+    ):
         self.sql_dialect = settings_object._sql_dialect
         self._settings_obj = settings_object
         self.input_columns = clean_user_input_columns(
-            input_columns.items(), return_as_single_column=True
+            input_columns, return_as_single_column=True
         )
 
     @property
     def cols_to_retain(self):
-        return clean_list_of_column_names(self._settings_obj._additional_cols_to_retain)
+        return clean_list_of_column_names(
+            self._settings_obj._additional_columns_to_retain
+        )
 
     @property
     def uid(self):
         uid_as_tree = InputColumn(
             self._settings_obj.column_info_settings.unique_id_column_name
         )
         return clean_list_of_column_names([uid_as_tree])
```

### Comparing `splink-4.0.0.dev3/splink/settings_validation/settings_validation_log_strings.py` & `splink-4.0.0.dev4/splink/settings_validation/settings_validation_log_strings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
+
 from functools import partial
 from typing import List, NamedTuple, Tuple
 
 
-def indent_error_message(message):
+def indent_error_message(message: str) -> str:
     """Indents an error message by 4 spaces."""
     return "\n    ".join(message.splitlines())
 
 
 class InvalidColumnsLogGenerator(NamedTuple):
     """
     A simple NamedTuple to aid in the construction of
@@ -17,15 +19,15 @@
             detected. This can be one of: `invalid_cols`,
             `invalid_table_pref` or `invalid_col_suffix`.
         invalid_columns (list): A list of the invalid
             columns that have been detected.
     """
 
     invalid_type: str
-    invalid_columns: set
+    invalid_columns: set[str]
 
     @property
     def log_string_prefix(self):
         return "       - "
 
     @property
     def columns_as_text(self):
@@ -58,15 +60,17 @@
     InvalidColumnsLogGenerator, "invalid_table_name"
 )
 InvalidColumnSuffixesLogGenerator = partial(
     InvalidColumnsLogGenerator, "invalid_column_suffix"
 )
 
 
-def construct_missing_settings_column_log(constructor_dict) -> str:
+def construct_missing_settings_column_log(
+    constructor_dict: tuple[str, InvalidColumnsLogGenerator] | None,
+) -> str:
     if not constructor_dict:
         return ""
 
     settings_id, InvalidCols = constructor_dict
     output_warning = [
         "======================================",
         f"Setting: `{settings_id}`",
@@ -75,30 +79,31 @@
 
     # The blank string acts as a newline
     output_warning.extend([InvalidCols.construct_log_string(), ""])
     return "\n".join(output_warning)
 
 
 def construct_invalid_sql_log_string(
-    # invalid_sql_statements: dict[str, list[InvalidColumnsTracker]]
-    invalid_sql_statements,
+    invalid_sql_statements: dict[str, list[InvalidColumnsLogGenerator]],
 ) -> str:
     log_str = []
     for sql, invalid_cols in invalid_sql_statements.items():
         log_str.append(f"    SQL: `{sql}`")
 
         for c in invalid_cols:
             log_str.append(f"{c.construct_log_string()}")
         # Acts as a newline as we're joining at the end of the str
         log_str.append("")
 
     return "\n".join(log_str)
 
 
-def construct_missing_column_in_blocking_rule_log(invalid_brs):
+def construct_missing_column_in_blocking_rule_log(
+    invalid_brs: dict[str, list[InvalidColumnsLogGenerator]],
+) -> str:
     if not invalid_brs:
         return ""
 
     # `invalid_brs` are in the format of:
     # {
     # "blocking_rule_1": {
     #  - InvalidCols tuple for invalid columns
@@ -111,15 +116,17 @@
         "======================================\n",
     ]
 
     output_warning.append(construct_invalid_sql_log_string(invalid_brs))
     return "\n".join(output_warning)
 
 
-def construct_missing_column_in_comparison_level_log(invalid_cls) -> str:
+def construct_missing_column_in_comparison_level_log(
+    invalid_cls: list[tuple[str, dict[str, list[InvalidColumnsLogGenerator]]]],
+) -> str:
     if not invalid_cls:
         return ""
 
     # `invalid_cls` is made up of a tuple containing:
     # 1) The `output_column_name` for the level, if it exists
     # 2) A dictionary in the same format as our blocking rules
     # {sql: [InvalidCols tuples]}
@@ -141,15 +148,15 @@
         output_warning.append(construct_invalid_sql_log_string(comp_lvls))
 
     return "\n".join(output_warning)
 
 
 def create_invalid_comparison_level_log_string(
     comparison_string: str, invalid_comparison_levels: List[Tuple[str, str]]
-):
+) -> str:
     invalid_levels_str = ",\n".join(
         [
             f"- Type: {type_name}. Level: {level}"
             for level, type_name in invalid_comparison_levels
         ]
     )
 
@@ -161,41 +168,41 @@
     )
 
     return indent_error_message(log_message)
 
 
 def create_invalid_comparison_log_string(
     comparison_string: str, comparison_level: bool
-):
+) -> str:
     if comparison_level:
         type_msg = "is a comparison level"
     else:
         type_msg = "is of an invalid data type"
 
     log_message = (
         f"\n{comparison_string}\n"
         f"{type_msg} and must be nested within a comparison.\n"
         "Please only include dictionaries or objects of the `Comparison` class.\n"
     )
     return indent_error_message(log_message)
 
 
-def create_no_comparison_levels_error_log_string(comparison_string: str):
+def create_no_comparison_levels_error_log_string(comparison_string: str) -> str:
     log_message = (
         f"\n{comparison_string}\n"
         "is missing the required `comparison_levels` dictionary"
         "key. Please ensure you\ninclude this in all comparisons"
         "used in your settings object.\n"
     )
     return indent_error_message(log_message)
 
 
 def create_incorrect_dialect_import_log_string(
     comparison_string: str, comparison_dialects: List[str]
-):
+) -> str:
     log_message = (
         f"\n{comparison_string}\n"
         "contains the following invalid SQL dialect(s)"
         f"within its comparison levels - {', '.join(comparison_dialects)}.\n"
         "Please ensure that you're importing comparisons designed "
         "for your specified linker.\n"
     )
```

### Comparing `splink-4.0.0.dev3/splink/spark/database_api.py` & `splink-4.0.0.dev4/splink/spark/database_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 import pandas as pd
 import sqlglot
 from numpy import nan
 from pyspark.sql.dataframe import DataFrame as spark_df
 from pyspark.sql.utils import AnalysisException
 
-from ..database_api import DatabaseAPI
+from ..database_api import AcceptableInputTableType, DatabaseAPI
 from ..databricks.enable_splink import enable_splink
 from ..dialects import (
     SparkDialect,
 )
 from ..misc import (
     major_minor_version_greater_equal_than,
 )
 from .dataframe import SparkDataFrame
 from .jar_location import get_scala_udfs
 
 logger = logging.getLogger(__name__)
 
 
-class SparkAPI(DatabaseAPI):
+class SparkAPI(DatabaseAPI[spark_df]):
     sql_dialect = SparkDialect()
 
     def __init__(
         self,
         *,
         spark_session,
         break_lineage_method=None,
@@ -66,28 +66,30 @@
         # TODO: (ideally) set things up so databricks can inherit from this
         self.in_databricks = "DATABRICKS_RUNTIME_VERSION" in os.environ
         if self.in_databricks:
             enable_splink(self.spark)
 
         self._set_default_break_lineage_method()
 
-    def _table_registration(self, input, table_name) -> None:
+    def _table_registration(
+        self, input: AcceptableInputTableType, table_name: str
+    ) -> None:
         if isinstance(input, dict):
             input = pd.DataFrame(input)
         elif isinstance(input, list):
             input = pd.DataFrame.from_records(input)
 
         if isinstance(input, pd.DataFrame):
             input = self._clean_pandas_df(input)
             input = self.spark.createDataFrame(input)
 
         input.createOrReplaceTempView(table_name)
 
     def table_to_splink_dataframe(
-        self, templated_name, physical_name
+        self, templated_name: str, physical_name: str
     ) -> SparkDataFrame:
         return SparkDataFrame(templated_name, physical_name, self)
 
     def table_exists_in_database(self, table_name):
         query_result = self._execute_sql_against_backend(
             f"show tables from {self.splink_data_store} like '{table_name}'"
         ).collect()
@@ -111,15 +113,15 @@
 
     def _setup_for_execute_sql(self, sql: str, physical_name: str) -> str:
         sql = sqlglot.transpile(sql, read="spark", write="customspark", pretty=True)[0]
         return sql
 
     def _cleanup_for_execute_sql(
         self, table: spark_df, templated_name: str, physical_name: str
-    ):
+    ) -> SparkDataFrame:
         spark_df = self._break_lineage_and_repartition(
             table, templated_name, physical_name
         )
 
         # After blocking, want to repartition
         # if templated
         spark_df.createOrReplaceTempView(physical_name)
```

### Comparing `splink-4.0.0.dev3/splink/spark/dataframe.py` & `splink-4.0.0.dev4/splink/spark/dataframe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
+from pandas import DataFrame as PandasDataFrame
+
 from ..input_column import InputColumn
 from ..splink_dataframe import SplinkDataFrame
 from .spark_helpers.custom_spark_dialect import Dialect
 
 logger = logging.getLogger(__name__)
 
 Dialect["customspark"]
@@ -29,28 +31,24 @@
         pass
 
     def as_record_dict(self, limit=None):
         sql = f"select * from {self.physical_name}"
         if limit:
             sql += f" limit {limit}"
 
-        return (
-            self.db_api._execute_sql_against_backend(sql)
-            .toPandas()
-            .to_dict(orient="records")
-        )
+        return self.as_pandas_dataframe(limit=limit).to_dict(orient="records")
 
     def _drop_table_from_database(self, force_non_splink_table=False):
         if self.db_api.break_lineage_method == "delta_lake_table":
             self._check_drop_table_created_by_splink(force_non_splink_table)
             self.db_api.delete_table_from_database(self.physical_name)
         else:
             pass
 
-    def as_pandas_dataframe(self, limit=None):
+    def as_pandas_dataframe(self, limit: int = None) -> PandasDataFrame:
         sql = f"select * from {self.physical_name}"
         if limit:
             sql += f" limit {limit}"
 
         return self.db_api._execute_sql_against_backend(sql).toPandas()
 
     def as_spark_dataframe(self):
```

### Comparing `splink-4.0.0.dev3/splink/spark/jar_location.py` & `splink-4.0.0.dev4/splink/spark/jar_location.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/spark/spark_helpers/custom_spark_dialect.py` & `splink-4.0.0.dev4/splink/spark/spark_helpers/custom_spark_dialect.py`

 * *Files identical despite different names*

### Comparing `splink-4.0.0.dev3/splink/splink_comparison_viewer.py` & `splink-4.0.0.dev4/splink/splink_comparison_viewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 from .predict import _combine_prior_and_bfs
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
     from .linker import Linker
 
 
-def row_examples(linker: Linker, example_rows_per_category=2):
+def row_examples(
+    linker: Linker, example_rows_per_category: int = 2
+) -> list[dict[str, str]]:
     sqls = []
 
     uid_cols = linker._settings_obj.column_info_settings.unique_id_input_columns
     uid_cols_l = [uid_col.name_l for uid_col in uid_cols]
     uid_cols_r = [uid_col.name_r for uid_col in uid_cols]
     uid_col_lr_names = uid_cols_l + uid_cols_r
     uid_expr = " || '-' ||".join(uid_col_lr_names)
@@ -79,16 +81,16 @@
 
     sqls.append(sql_info)
 
     return sqls
 
 
 def comparison_viewer_table_sqls(
-    linker: Linker, example_rows_per_category=2
-) -> list[dict]:
+    linker: Linker, example_rows_per_category: int = 2
+) -> list[dict[str, str]]:
     sqls = row_examples(linker, example_rows_per_category)
 
     sql = """
     select ser.*,
            cvd.sum_gam,
            cvd.count_rows_in_comparison_vector_group,
            cvd.proportion_of_comparisons
@@ -104,19 +106,19 @@
     }
 
     sqls.append(sql_info)
     return sqls
 
 
 def render_splink_comparison_viewer_html(
-    comparison_vector_data,
-    splink_settings: dict,
+    comparison_vector_data: list[dict[str, Any]],
+    splink_settings: dict[str, Any],
     out_path: str,
     overwrite: bool = False,
-):
+) -> str:
     # When developing the package, it can be easier to point
     # ar the script live on observable using <script src=>
     # rather than bundling the whole thing into the html
     bundle_observable_notebook = True
 
     template_path = "files/splink_comparison_viewer/template.j2"
     template = Template(read_resource(template_path))
```

### Comparing `splink-4.0.0.dev3/splink/splink_dataframe.py` & `splink-4.0.0.dev4/splink/splink_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod, abstractproperty
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from .input_column import InputColumn
 
 logger = logging.getLogger(__name__)
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
@@ -21,23 +21,23 @@
     Uses methods like `as_pandas_dataframe()` and `as_record_dict()` to retrieve data
     """
 
     def __init__(
         self,
         templated_name: str,
         physical_name: str,
-        database_api: DatabaseAPI,
-        metadata: dict = None,
+        database_api: DatabaseAPI[Any],
+        metadata: dict[str, Any] = None,
     ):
         self.templated_name = templated_name
         self.physical_name = physical_name
         self.db_api = database_api
         self._target_schema = "splink"
         self.created_by_splink = False
-        self.sql_used_to_create = None
+        self.sql_used_to_create: str | None = None
         self.metadata = metadata or {}
 
     @abstractproperty
     def columns(self) -> list[InputColumn]:
         pass
 
     @property
@@ -69,15 +69,15 @@
 
     def _drop_table_from_database(self, force_non_splink_table=False):
         raise NotImplementedError(
             "_drop_table_from_database from database not " "implemented for this linker"
         )
 
     def drop_table_from_database_and_remove_from_cache(
-        self, force_non_splink_table=False
+        self, force_non_splink_table: bool = False
     ) -> None:
         """Drops the table from the underlying database, and removes it
         from the (linker) cache.
 
         By default this will fail if the table is not one created by Splink,
         but this check can be overriden
```

### Comparing `splink-4.0.0.dev3/splink/sql_transform.py` & `splink-4.0.0.dev4/splink/sql_transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from typing import TypeVar
+
 import sqlglot
 import sqlglot.expressions as exp
 
 
 def sqlglot_transform_sql(sql, func, dialect=None):
     syntax_tree = sqlglot.parse_one(sql, read=dialect)
     transformed_tree = syntax_tree.transform(func)
     return transformed_tree.sql(dialect)
 
 
-def _add_l_or_r_to_identifier(node: exp.Expression):
+def _add_l_or_r_to_identifier(node: exp.Expression) -> exp.Expression:
     if not isinstance(node, exp.Identifier):
         return node
 
     if (p := node.parent) is None:
         raise TypeError(f"Node {node} has no parent")
     if isinstance(p, (exp.Lambda, exp.Anonymous)):
         # node is the `x` in the lambda `x -> list_contains(r.name_list, x))`
@@ -31,19 +33,21 @@
 def _remove_table_prefix(node):
     if isinstance(node, exp.Column):
         n = node.sql().replace(f"{node.table}.", "")
         return sqlglot.parse_one(n)
     return node
 
 
-def move_l_r_table_prefix_to_column_suffix(blocking_rule) -> str:
-    expression_tree = sqlglot.parse_one(blocking_rule, read=None)
+def move_l_r_table_prefix_to_column_suffix(
+    blocking_rule: str, dialect: str = None
+) -> str:
+    expression_tree = sqlglot.parse_one(blocking_rule, read=dialect)
     transformed_tree = expression_tree.transform(_add_l_or_r_to_identifier)
     transformed_tree = transformed_tree.transform(_remove_table_prefix)
-    return transformed_tree.sql()
+    return transformed_tree.sql(dialect=dialect)
 
 
 def add_quotes_and_table_prefix(syntax_tree, table_name):
     """Quotes and adds a table name to your input column(s).
 
     > tree = sqlglot.parse_one("concat(first_name, surname)")
     > add_quote_and_table_prefix(tree, "l")
@@ -92,15 +96,18 @@
             return f"{sub_tree['class']}({', '.join(child_signatures)})"
         else:
             return sub_tree["class"]
 
     return _signature(sqlglot_tree.dump())
 
 
-def remove_quotes_from_identifiers(tree) -> exp.Expression:
+T = TypeVar("T", bound=exp.Expression)
+
+
+def remove_quotes_from_identifiers(tree: T) -> T:
     tree = tree.copy()
     for identifier in tree.find_all(exp.Identifier):
         identifier.args["quoted"] = False
     return tree
 
 
 def add_suffix_to_all_column_identifiers(
@@ -135,12 +142,12 @@
 
     return tree.sql(dialect=sqlglot_dialect)
 
 
 # TODO: can we get rid of add_quotes_and_table_prefix and use this everywhere instead
 def add_table_to_all_column_identifiers(
     sql_str: str, table_name: str, sqlglot_dialect: str
-):
+) -> str:
     tree = sqlglot.parse_one(sql_str, dialect=sqlglot_dialect)
     for col in tree.find_all(exp.Column):
         col.args["table"] = table_name
     return tree.sql(dialect=sqlglot_dialect)
```

### Comparing `splink-4.0.0.dev3/splink/sqlite/database_api.py` & `splink-4.0.0.dev4/splink/sqlite/database_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 )
 from ..exceptions import SplinkException
 from .dataframe import SQLiteDataFrame
 
 sql_con = sqlite3.Connection
 
 
-class SQLiteAPI(DatabaseAPI):
+class SQLiteAPI(DatabaseAPI[sqlite3.Cursor]):
     sql_dialect = SQLiteDialect()
 
     @staticmethod
     def dict_factory(cursor, row):
         d = {}
         for idx, col in enumerate(cursor.description):
             d[col[0]] = row[idx]
         return d
 
-    def _register_udfs(self, register_udfs: bool):
+    def _register_udfs(self, register_udfs: bool) -> None:
         self.con.create_function("log2", 1, math.log2)
         self.con.create_function("pow", 2, pow)
         self.con.create_function("power", 2, pow)
 
         if register_udfs:
             try:
                 from rapidfuzz.distance.DamerauLevenshtein import distance as dam_lev
@@ -59,15 +59,15 @@
             "jaro": jaro,
         }
 
         for sql_name, func in funcs_to_register.items():
             self.con.create_function(sql_name, 2, wrap_func_with_str(func))
 
     def __init__(
-        self, connection: Union[str, sql_con] = ":memory:", register_udfs=True
+        self, connection: Union[str, sql_con] = ":memory:", register_udfs: bool = True
     ):
         super().__init__()
 
         if isinstance(connection, str):
             connection = sqlite3.connect(connection)
         self.con = connection
         self.con.row_factory = self.dict_factory
```

### Comparing `splink-4.0.0.dev3/splink/sqlite/dataframe.py` & `splink-4.0.0.dev4/splink/sqlite/dataframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,17 +28,17 @@
         """
         pragma_result = self.db_api._execute_sql_against_backend(sql).fetchall()
         cols = [r["name"] for r in pragma_result]
 
         return [InputColumn(c, sql_dialect="sqlite") for c in cols]
 
     def validate(self):
-        if type(self.physical_name) is not str:
+        if not isinstance(self.physical_name, str):
             raise ValueError(
-                f"{self.df_name} is not a string dataframe.\n"
+                f"{self.templated_name} is not a string dataframe.\n"
                 "SQLite Linker requires input data"
                 " to be a string containing the name of the "
                 " sqlite table."
             )
 
         sql = f"""
         SELECT name
```

### Comparing `splink-4.0.0.dev3/splink/term_frequencies.py` & `splink-4.0.0.dev4/splink/term_frequencies.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from __future__ import annotations
 
 # For more information on where formulas came from, see
 # https://github.com/moj-analytical-services/splink/pull/107
 import logging
 import warnings
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from numpy import arange, ceil, floor, log2
 from pandas import concat, cut
 
-from .charts import altair_or_json, load_chart_definition
+from .charts import ChartReturnType, altair_or_json, load_chart_definition
 from .input_column import InputColumn
+from .pipeline import CTEPipeline
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
     from .linker import Linker
 
 logger = logging.getLogger(__name__)
 
 
-def colname_to_tf_tablename(input_column: InputColumn):
+def colname_to_tf_tablename(input_column: InputColumn) -> str:
     column_name_str = input_column.unquote().name.replace(" ", "_")
     return f"__splink__df_tf_{column_name_str}"
 
 
 def term_frequencies_for_single_column_sql(
-    input_column: InputColumn, table_name="__splink__df_concat"
-):
+    input_column: InputColumn, table_name: str = "__splink__df_concat"
+) -> str:
     col_name = input_column.name
 
     sql = f"""
     select
     {col_name}, cast(count(*) as float8) / (select
         count({col_name}) as total from {table_name})
             as {input_column.tf_name}
@@ -38,129 +39,139 @@
     where {col_name} is not null
     group by {col_name}
     """
 
     return sql
 
 
-def _join_tf_to_input_df_sql(linker: Linker):
+def _join_tf_to_df_concat_sql(linker: Linker) -> str:
     settings_obj = linker._settings_obj
     tf_cols = settings_obj._term_frequency_columns
 
     select_cols = []
 
     for col in tf_cols:
         tbl = colname_to_tf_tablename(col)
-        if tbl in linker._intermediate_table_cache:
-            tbl = linker._intermediate_table_cache[tbl].physical_name
-        tf_col = col.tf_name
-        select_cols.append(f"{tbl}.{tf_col}")
+        select_cols.append(f"{tbl}.{col.tf_name}")
 
     select_cols.insert(0, "__splink__df_concat.*")
     select_cols_str = ", ".join(select_cols)
 
     templ = "left join {tbl} on __splink__df_concat.{col} = {tbl}.{col}"
 
     left_joins = []
     for col in tf_cols:
         tbl = colname_to_tf_tablename(col)
-        if tbl in linker._intermediate_table_cache:
-            tbl = linker._intermediate_table_cache[tbl].physical_name
         sql = templ.format(tbl=tbl, col=col.name)
         left_joins.append(sql)
 
-    # left_joins = [
-    #     templ.format(tbl=colname_to_tf_tablename(col), col=col.name)
-    #     for col in tf_cols
-    # ]
     left_joins_str = " ".join(left_joins)
 
     sql = f"""
     select {select_cols_str }
     from __splink__df_concat
     {left_joins_str}
     """
 
     return sql
 
 
-def term_frequencies_from_concat_with_tf(input_column):
-    sql = f"""
-        select
-        distinct {input_column.name},
-        {input_column.tf_name}
-        from __splink__df_concat_with_tf
+def _join_new_table_to_df_concat_with_tf_sql(linker: Linker, new_tablename: str) -> str:
+    """
+    Joins any required tf columns onto new_tablename
+
+    This is needed e.g. when using linker.compare_two_records
+    or linker.find_matches_to_new_records in which the user provides
+    new records which need tf adjustments computed
     """
 
+    cache = linker._intermediate_table_cache
+    settings_obj = linker._settings_obj
+    tf_cols = settings_obj._term_frequency_columns
+
+    select_cols = [f"{new_tablename}.*"]
+
+    for col in tf_cols:
+        tbl = colname_to_tf_tablename(col)
+        if tbl in cache:
+            select_cols.append(f"{tbl}.{col.tf_name}")
+
+    template = "left join {tbl} on " + new_tablename + ".{col} = {tbl}.{col}"
+    template_with_alias = (
+        "left join ({subquery}) as {_as} on " + new_tablename + ".{col} = {_as}.{col}"
+    )
+
+    left_joins = []
+    for i, col in enumerate(tf_cols):
+        tbl = colname_to_tf_tablename(col)
+        if tbl in cache:
+            sql = template.format(tbl=tbl, col=col.name)
+            left_joins.append(sql)
+        elif "__splink__df_concat_with_tf" in cache:
+            subquery = f"""
+            select distinct {col.name}, {col.tf_name}
+            from __splink__df_concat_with_tf
+            """
+            _as = f"nodes_tf__{i}"
+            sql = template_with_alias.format(subquery=subquery, col=col.name, _as=_as)
+            select_cols.append(f"{_as}.{col.tf_name}")
+            left_joins.append(sql)
+        else:
+            select_cols.append(f"null as {col.tf_name}")
+
+    select_cols_str = ", ".join(select_cols)
+    left_joins_str = "\n".join(left_joins)
+
+    sql = f"""
+    select {select_cols_str}
+    from {new_tablename}
+    {left_joins_str}
+
+    """
     return sql
 
 
-def compute_all_term_frequencies_sqls(linker: Linker) -> list[dict]:
+def compute_all_term_frequencies_sqls(
+    linker: Linker, pipeline: CTEPipeline
+) -> list[dict[str, str]]:
     settings_obj = linker._settings_obj
     tf_cols = settings_obj._term_frequency_columns
 
     if not tf_cols:
         return [
             {
                 "sql": "select * from __splink__df_concat",
                 "output_table_name": "__splink__df_concat_with_tf",
             }
         ]
 
     sqls = []
+    cache = linker._intermediate_table_cache
     for tf_col in tf_cols:
         tf_table_name = colname_to_tf_tablename(tf_col)
 
-        if tf_table_name not in linker._intermediate_table_cache:
+        if tf_table_name in cache:
+            tf_table = cache.get_with_logging(tf_table_name)
+            pipeline.append_input_dataframe(tf_table)
+        else:
             sql = term_frequencies_for_single_column_sql(tf_col)
-            sql = {"sql": sql, "output_table_name": tf_table_name}
-            sqls.append(sql)
+            sql_info = {"sql": sql, "output_table_name": tf_table_name}
+            sqls.append(sql_info)
 
-    sql = _join_tf_to_input_df_sql(linker)
-    sql = {
+    sql = _join_tf_to_df_concat_sql(linker)
+    sql_info = {
         "sql": sql,
         "output_table_name": "__splink__df_concat_with_tf",
     }
-    sqls.append(sql)
+    sqls.append(sql_info)
 
     return sqls
 
 
-def compute_term_frequencies_from_concat_with_tf(linker: "Linker"):
-    """If __splink__df_concat_with_tf already exists in your database,
-    reverse engineer the underlying tf tables.
-
-    __splink__df_concat_with_tf is a cached table and often output by
-    users to disk, for use at a later point in time. As a result, it
-    often exists in the database or is easily accessible by the user,
-    while the underlying tf tables are not.
-    """
-
-    settings_obj = linker._settings_obj
-    tf_cols = settings_obj._term_frequency_columns
-    cache = linker._intermediate_table_cache
-
-    tf_table = []
-    for tf_col in tf_cols:
-        tf_table_name = colname_to_tf_tablename(tf_col)
-
-        if tf_table_name not in cache:
-            sql = term_frequencies_from_concat_with_tf(tf_col)
-            sql = {
-                "sql": sql,
-                "output_table_name": colname_to_tf_tablename(tf_col),
-            }
-            tf_table.append(sql)
-        else:
-            tf_table.append(cache[tf_table_name])
-
-    return tf_table
-
-
-def comparison_level_to_tf_chart_data(cl: dict) -> dict:
+def comparison_level_to_tf_chart_data(cl: dict[str, Any]) -> dict[str, Any]:
     df = cl["df_tf"]
     df.columns = ["value", "tf"]
     df = df[df.value.notnull()]
 
     del cl["df_tf"]
     df = df.assign(**cl)
 
@@ -189,16 +200,21 @@
 
     cl["df_out"] = df
 
     return cl
 
 
 def tf_adjustment_chart(
-    linker: Linker, col, n_most_freq, n_least_freq, vals_to_include, as_dict
-):
+    linker: Linker,
+    col: str,
+    n_most_freq: int,
+    n_least_freq: int,
+    vals_to_include: list[str],
+    as_dict: bool,
+) -> ChartReturnType:
     # Data for chart
     comparison = linker._settings_obj._get_comparison_by_output_column_name(col)
     comparison_records = comparison._as_detailed_records
 
     keys_to_retain = [
         "comparison_vector_value",
         "label_for_charts",
```

### Comparing `splink-4.0.0.dev3/splink/unique_id_concat.py` & `splink-4.0.0.dev4/splink/unique_id_concat.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,17 @@
+from __future__ import annotations
+
+from .input_column import InputColumn
+
 CONCAT_SEPARATOR = "-__-"
 
 
-def _composite_unique_id_from_nodes_sql(unique_id_cols, table_prefix=None):
+def _composite_unique_id_from_nodes_sql(
+    unique_id_cols: list[InputColumn], table_prefix: str | None = None
+) -> str:
     """
     Returns:
         str: e.g. 'l."source_dataset" || -__- || l."unique_id"'
     """
     if table_prefix:
         table_prefix = f"{table_prefix}."
     else:
```

### Comparing `splink-4.0.0.dev3/splink/validate_jsonschema.py` & `splink-4.0.0.dev4/splink/validate_jsonschema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from __future__ import annotations
+
 import json
 import operator
 from functools import lru_cache, reduce
+from typing import Any
 
 from jsonschema import Draft7Validator
 
 from .misc import read_resource
 
 
 @lru_cache()
@@ -40,15 +43,15 @@
     except ValueError:
         index_of_comparison = None
     if index_of_comparison is not None:
         comparison = get_from_dict(settings_dict, path[: index_of_comparison + 2])
     return comparison
 
 
-def validate_settings_against_schema(settings_dict: dict):
+def validate_settings_against_schema(settings_dict: dict[str, Any]) -> None:
     """Validate a splink settings object against its jsonschema"""
 
     schema = get_schema()
 
     v = Draft7Validator(schema)
 
     e = next(v.iter_errors(settings_dict), None)
```

### Comparing `splink-4.0.0.dev3/splink/waterfall_chart.py` & `splink-4.0.0.dev4/splink/waterfall_chart.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from __future__ import annotations
+
 import math
 from copy import deepcopy
+from typing import Any, Dict
 
 from .comparison import Comparison
 from .misc import prob_to_bayes_factor
 
 
 def _prior_record(settings_obj):
-    rec = {}
+    rec: Dict[str, Any] = {}
     rec["column_name"] = "Prior"
     rec["label_for_charts"] = "Starting match weight (prior)"
     rec["sql_condition"] = None
     bf = prob_to_bayes_factor(settings_obj._probability_two_random_records_match)
     rec["log2_bayes_factor"] = math.log2(bf)
     rec["bayes_factor"] = bf
     rec["comparison_vector_value"] = None
@@ -20,15 +23,15 @@
     rec["value_l"] = ""
     rec["value_r"] = ""
     rec["term_frequency_adjustment"] = None
     return rec
 
 
 def _final_score_record(record_as_dict):
-    rec = {}
+    rec: Dict[str, Any] = {}
     rec["column_name"] = "Final score"
     rec["label_for_charts"] = "Final score"
     rec["sql_condition"] = None
     rec["log2_bayes_factor"] = record_as_dict["match_weight"]
     rec["bayes_factor"] = 2 ** record_as_dict["match_weight"]
     rec["comparison_vector_value"] = None
     rec["m_probability"] = None
@@ -36,33 +39,42 @@
     rec["bayes_factor_description"] = None
     rec["value_l"] = ""
     rec["value_r"] = ""
     rec["term_frequency_adjustment"] = None
     return rec
 
 
-def _comparison_records(record_as_dict, comparison: Comparison, hide_details=False):
+def _comparison_records(
+    record_as_dict: dict[str, Any], comparison: Comparison, hide_details: bool = False
+) -> list[dict[str, Any]]:
     output_records = []
-    waterfall_record = {}
 
     c = comparison
     cv_value = record_as_dict[c._gamma_column_name]
 
     cl = c._get_comparison_level_by_comparison_vector_value(cv_value)
+    waterfall_record = {
+        field: value
+        for field, value in cl._as_detailed_record(
+            c._num_levels, c.comparison_levels
+        ).items()
+        if field
+        in [
+            "label_for_charts",
+            "sql_condition",
+            "log2_bayes_factor",
+            "bayes_factor",
+            "comparison_vector_value",
+            "m_probability",
+            "u_probability",
+            "bayes_factor_description",
+        ]
+    }
 
     waterfall_record["column_name"] = c.output_column_name
-    waterfall_record["label_for_charts"] = cl.label_for_charts
-
-    waterfall_record["sql_condition"] = cl.sql_condition
-    waterfall_record["log2_bayes_factor"] = cl._log2_bayes_factor
-    waterfall_record["bayes_factor"] = cl._bayes_factor
-    waterfall_record["comparison_vector_value"] = int(cv_value)
-    waterfall_record["m_probability"] = cl.m_probability
-    waterfall_record["u_probability"] = cl.u_probability
-    waterfall_record["bayes_factor_description"] = cl._bayes_factor_description
     input_cols_used = c._input_columns_used_by_case_statement
     input_cols_l = [ic.unquote().name_l for ic in input_cols_used]
     input_cols_r = [ic.unquote().name_r for ic in input_cols_used]
 
     if hide_details:
         waterfall_record["value_l"] = ""
         waterfall_record["value_r"] = ""
```

### Comparing `splink-4.0.0.dev3/PKG-INFO` & `splink-4.0.0.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splink
-Version: 4.0.0.dev3
+Version: 4.0.0.dev4
 Summary: Fast probabilistic data linkage at scale
 Home-page: https://github.com/moj-analytical-services/splink
 License: MIT
 Author: Robin Linacre
 Author-email: robinlinacre@hotmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,14 +20,16 @@
 Provides-Extra: spark
 Requires-Dist: Jinja2 (>=3.0.3)
 Requires-Dist: altair (>=5.0.1,<6.0.0)
 Requires-Dist: awswrangler (>=3.0.0,<4.0.0) ; (python_version >= "3.8") and (extra == "athena")
 Requires-Dist: duckdb (>=0.9.2)
 Requires-Dist: igraph (>=0.11.2) ; python_version >= "3.8"
 Requires-Dist: jsonschema (>=3.2)
+Requires-Dist: numpy (>=1.17.3) ; python_version < "3.12"
+Requires-Dist: numpy (>=1.26.0) ; python_version >= "3.12"
 Requires-Dist: pandas (>1.3.5)
 Requires-Dist: phonetics (>=1.0.5)
 Requires-Dist: psycopg2-binary (>=2.8.0) ; extra == "postgres"
 Requires-Dist: pyspark (>=3.2.1) ; extra == "pyspark" or extra == "spark"
 Requires-Dist: sqlglot (>=13.0.0)
 Project-URL: Repository, https://github.com/moj-analytical-services/splink
 Description-Content-Type: text/markdown
@@ -36,15 +38,16 @@
 <img src="https://user-images.githubusercontent.com/7570107/85285114-3969ac00-b488-11ea-88ff-5fca1b34af1f.png" alt="Splink Logo" height="150px">
 </p>
 
 [![pypi](https://img.shields.io/github/v/release/moj-analytical-services/splink?include_prereleases)](https://pypi.org/project/splink/#history)
 [![Downloads](https://static.pepy.tech/badge/splink/month)](https://pepy.tech/project/splink)
 [![Documentation](https://img.shields.io/badge/API-documentation-blue)](https://moj-analytical-services.github.io/splink/)
 
-
+> [!IMPORTANT]
+> Development has begun on Splink 4 on the `splink4_dev` branch.  Splink 3 is in maintenance mode and we are no longer accepting new features. We welcome contributions to Splink 4. Read more on our latest [blog](https://moj-analytical-services.github.io/splink/blog/2024/03/19/splink4.html).
 
 # Fast, accurate and scalable probabilistic data linkage
 
 Splink is a Python package for probabilistic record linkage (entity resolution) that allows you to deduplicate and link records from datasets that lack unique identifiers.
 
 ## Key Features
```

