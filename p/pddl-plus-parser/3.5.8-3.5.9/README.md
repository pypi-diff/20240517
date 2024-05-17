# Comparing `tmp/pddl-plus-parser-3.5.8.tar.gz` & `tmp/pddl-plus-parser-3.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pddl-plus-parser-3.5.8.tar", last modified: Tue Mar 19 16:48:37 2024, max compression
+gzip compressed data, was "pddl-plus-parser-3.5.9.tar", last modified: Sun Mar 24 13:50:28 2024, max compression
```

## Comparing `pddl-plus-parser-3.5.8.tar` & `pddl-plus-parser-3.5.9.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 16:48:37.107481 pddl-plus-parser-3.5.8/
--rw-rw-rw-   0        0        0    11499 2022-01-08 09:02:31.000000 pddl-plus-parser-3.5.8/LICENSE
--rw-rw-rw-   0        0        0     3764 2024-03-19 16:48:37.107481 pddl-plus-parser-3.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     3440 2024-03-19 16:46:02.000000 pddl-plus-parser-3.5.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 16:48:37.025368 pddl-plus-parser-3.5.8/pddl_plus_parser/
--rw-rw-rw-   0        0        0        0 2022-03-13 12:11:09.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 16:48:37.036458 pddl-plus-parser-3.5.8/pddl_plus_parser/exporters/
--rw-rw-rw-   0        0        0      264 2022-08-21 09:19:40.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/exporters/__init__.py
--rw-rw-rw-   0        0        0     7553 2022-08-21 12:45:31.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/exporters/domain_exporter.py
--rw-rw-rw-   0        0        0     1348 2022-06-02 13:51:41.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/exporters/enhsp_output_parser.py
--rw-rw-rw-   0        0        0     3677 2023-09-13 08:00:01.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/exporters/ff_output_parser.py
--rw-rw-rw-   0        0        0     6141 2023-03-14 07:34:52.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/exporters/numeric_trajectory_exporter.py
--rw-rw-rw-   0        0        0     4444 2024-03-19 10:35:44.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/exporters/problem_exporter.py
-drwxrwxrwx   0        0        0        0 2024-03-19 16:48:37.044458 pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/
--rw-rw-rw-   0        0        0      376 2023-06-18 20:40:16.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/__init__.py
--rw-rw-rw-   0        0        0    14713 2023-04-13 11:10:47.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/domain_parser.py
--rw-rw-rw-   0        0        0    10635 2023-04-17 10:32:20.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/effects_parser.py
--rw-rw-rw-   0        0        0     2998 2023-04-13 11:23:17.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/parsing_utils.py
--rw-rw-rw-   0        0        0      200 2022-01-09 12:51:47.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/pddl_parser_types.py
--rw-rw-rw-   0        0        0     2610 2022-12-05 08:48:42.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py
--rw-rw-rw-   0        0        0     5558 2023-04-13 11:44:39.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/preconditions_parser.py
--rw-rw-rw-   0        0        0    11961 2022-12-05 08:49:12.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/problem_parser.py
--rw-rw-rw-   0        0        0    13065 2023-06-18 20:51:11.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/trajectory_parser.py
-drwxrwxrwx   0        0        0        0 2024-03-19 16:48:37.062466 pddl-plus-parser-3.5.8/pddl_plus_parser/models/
--rw-rw-rw-   0        0        0      835 2023-05-01 08:05:47.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/__init__.py
--rw-rw-rw-   0        0        0     1296 2023-02-19 07:22:18.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/action_call.py
--rw-rw-rw-   0        0        0     1935 2023-05-01 08:11:11.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/conditional_effect.py
--rw-rw-rw-   0        0        0     6181 2023-11-20 15:42:29.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/grounded_effect.py
--rw-rw-rw-   0        0        0    13736 2023-08-09 07:43:30.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/grounded_precondition.py
--rw-rw-rw-   0        0        0     6340 2023-04-16 14:57:28.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/grounding_utils.py
--rw-rw-rw-   0        0        0     4844 2024-03-19 16:47:58.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/numeric_symbolic_operations.py
--rw-rw-rw-   0        0        0     9671 2024-02-27 09:43:57.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/numerical_expression.py
--rw-rw-rw-   0        0        0     3753 2022-12-05 08:50:29.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/observation.py
--rw-rw-rw-   0        0        0     1293 2023-04-13 13:54:50.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_action.py
--rw-rw-rw-   0        0        0     2279 2023-11-11 13:51:14.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_domain.py
--rw-rw-rw-   0        0        0     3973 2023-04-16 13:39:30.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_function.py
--rw-rw-rw-   0        0        0      460 2023-11-11 13:50:18.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_object.py
--rw-rw-rw-   0        0        0     8675 2023-05-16 11:04:11.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_operator.py
--rw-rw-rw-   0        0        0    11315 2024-03-08 14:49:21.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_precondition.py
--rw-rw-rw-   0        0        0     4737 2023-04-16 13:37:45.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_predicate.py
--rw-rw-rw-   0        0        0     1953 2022-11-18 11:18:07.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_problem.py
--rw-rw-rw-   0        0        0     4462 2023-11-25 13:38:32.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_state.py
--rw-rw-rw-   0        0        0     1221 2023-11-11 13:50:31.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_type.py
-drwxrwxrwx   0        0        0        0 2024-03-19 16:48:37.068456 pddl-plus-parser-3.5.8/pddl_plus_parser/multi_agent/
--rw-rw-rw-   0        0        0      324 2023-02-21 12:20:37.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/multi_agent/__init__.py
--rw-rw-rw-   0        0        0     2139 2023-04-17 11:31:48.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/multi_agent/common.py
--rw-rw-rw-   0        0        0     3282 2023-04-17 10:59:23.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py
--rw-rw-rw-   0        0        0     3031 2022-12-05 09:13:45.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py
--rw-rw-rw-   0        0        0     7079 2023-02-19 14:32:32.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py
--rw-rw-rw-   0        0        0    10857 2023-04-17 11:26:47.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/multi_agent/single_agent_plan_converter.py
-drwxrwxrwx   0        0        0        0 2024-03-19 16:48:37.079476 pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/
--rw-rw-rw-   0        0        0       40 2022-05-10 14:32:52.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/__init__.py
--rw-rw-rw-   0        0        0      357 2022-09-28 11:37:49.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/common.py
--rw-rw-rw-   0        0        0     3325 2022-09-28 12:05:01.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/counters_generator.py
--rw-rw-rw-   0        0        0     1856 2024-02-14 14:33:37.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/depot_generator.py
--rw-rw-rw-   0        0        0    12536 2022-05-16 08:10:09.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/depots_generator.py
--rw-rw-rw-   0        0        0     2113 2024-02-14 14:13:01.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/driverlog_generator.py
--rw-rw-rw-   0        0        0     5992 2022-09-28 12:09:35.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/farmland_generator.py
--rw-rw-rw-   0        0        0     2227 2023-08-06 09:42:00.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/minecraft_generator.py
--rw-rw-rw-   0        0        0     3756 2022-08-04 13:43:32.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/plant_watering_generator.py
--rw-rw-rw-   0        0        0     3679 2022-09-28 11:53:25.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/sailing_generator.py
--rw-rw-rw-   0        0        0    12311 2022-05-16 19:14:35.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/settlers_problem_generator.py
--rw-rw-rw-   0        0        0     8805 2022-09-28 12:16:10.000000 pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/zenotravel_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-19 16:48:37.030465 pddl-plus-parser-3.5.8/pddl_plus_parser.egg-info/
--rw-rw-rw-   0        0        0     3764 2024-03-19 16:48:36.000000 pddl-plus-parser-3.5.8/pddl_plus_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3919 2024-03-19 16:48:36.000000 pddl-plus-parser-3.5.8/pddl_plus_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 16:48:36.000000 pddl-plus-parser-3.5.8/pddl_plus_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-03-19 16:48:36.000000 pddl-plus-parser-3.5.8/pddl_plus_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 16:48:37.107481 pddl-plus-parser-3.5.8/setup.cfg
--rw-rw-rw-   0        0        0      492 2024-03-19 16:45:24.000000 pddl-plus-parser-3.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 16:48:37.022357 pddl-plus-parser-3.5.8/tests/
-drwxrwxrwx   0        0        0        0 2024-03-19 16:48:37.083467 pddl-plus-parser-3.5.8/tests/exporters_tests/
--rw-rw-rw-   0        0        0        0 2022-02-28 12:11:52.000000 pddl-plus-parser-3.5.8/tests/exporters_tests/__init__.py
--rw-rw-rw-   0        0        0     1262 2024-03-19 10:39:19.000000 pddl-plus-parser-3.5.8/tests/exporters_tests/consts.py
--rw-rw-rw-   0        0        0    10075 2024-03-19 10:37:02.000000 pddl-plus-parser-3.5.8/tests/exporters_tests/numeric_trajectory_exporter_test.py
--rw-rw-rw-   0        0        0     2784 2024-03-19 10:43:43.000000 pddl-plus-parser-3.5.8/tests/exporters_tests/problem_exporter_test.py
-drwxrwxrwx   0        0        0        0 2024-03-19 16:48:37.089483 pddl-plus-parser-3.5.8/tests/lisp_parsers_tests/
--rw-rw-rw-   0        0        0        0 2022-01-09 08:03:59.000000 pddl-plus-parser-3.5.8/tests/lisp_parsers_tests/__init__.py
--rw-rw-rw-   0        0        0     3503 2023-06-18 20:27:00.000000 pddl-plus-parser-3.5.8/tests/lisp_parsers_tests/consts.py
--rw-rw-rw-   0        0        0    40370 2024-02-24 16:19:58.000000 pddl-plus-parser-3.5.8/tests/lisp_parsers_tests/domain_parser_test.py
--rw-rw-rw-   0        0        0     3578 2024-01-23 11:15:50.000000 pddl-plus-parser-3.5.8/tests/lisp_parsers_tests/pddl_tokenizer_test.py
--rw-rw-rw-   0        0        0    17734 2022-08-21 10:17:02.000000 pddl-plus-parser-3.5.8/tests/lisp_parsers_tests/problem_parser_test.py
--rw-rw-rw-   0        0        0     7601 2023-06-18 20:45:34.000000 pddl-plus-parser-3.5.8/tests/lisp_parsers_tests/trajectory_parser_test.py
-drwxrwxrwx   0        0        0        0 2024-03-19 16:48:37.099464 pddl-plus-parser-3.5.8/tests/models_tests/
--rw-rw-rw-   0        0        0        0 2022-01-10 14:06:38.000000 pddl-plus-parser-3.5.8/tests/models_tests/__init__.py
--rw-rw-rw-   0        0        0      946 2024-01-23 11:19:09.000000 pddl-plus-parser-3.5.8/tests/models_tests/consts.py
--rw-rw-rw-   0        0        0    16596 2023-11-20 16:00:08.000000 pddl-plus-parser-3.5.8/tests/models_tests/grounded_effect_test.py
--rw-rw-rw-   0        0        0    27127 2023-05-14 10:23:35.000000 pddl-plus-parser-3.5.8/tests/models_tests/grounded_precondition_test.py
--rw-rw-rw-   0        0        0    15299 2024-03-19 16:48:12.000000 pddl-plus-parser-3.5.8/tests/models_tests/numeric_symbolic_operations_test.py
--rw-rw-rw-   0        0        0    14989 2024-02-27 09:02:26.000000 pddl-plus-parser-3.5.8/tests/models_tests/numerical_expression_test.py
--rw-rw-rw-   0        0        0    19392 2023-04-17 09:59:27.000000 pddl-plus-parser-3.5.8/tests/models_tests/operator_test.py
--rw-rw-rw-   0        0        0     1646 2022-06-21 11:55:51.000000 pddl-plus-parser-3.5.8/tests/models_tests/pddl_function_test.py
--rw-rw-rw-   0        0        0     7449 2023-08-25 14:53:40.000000 pddl-plus-parser-3.5.8/tests/models_tests/pddl_precondition_test.py
--rw-rw-rw-   0        0        0     3659 2023-11-25 13:50:20.000000 pddl-plus-parser-3.5.8/tests/models_tests/pddl_state_test.py
-drwxrwxrwx   0        0        0        0 2024-03-19 16:48:37.105471 pddl-plus-parser-3.5.8/tests/multi_agent_tests/
--rw-rw-rw-   0        0        0        0 2022-08-18 10:56:04.000000 pddl-plus-parser-3.5.8/tests/multi_agent_tests/__init__.py
--rw-rw-rw-   0        0        0     1706 2022-11-13 14:49:21.000000 pddl-plus-parser-3.5.8/tests/multi_agent_tests/consts.py
--rw-rw-rw-   0        0        0     2123 2023-04-17 11:05:34.000000 pddl-plus-parser-3.5.8/tests/multi_agent_tests/multi_agent_domain_converter_test.py
--rw-rw-rw-   0        0        0     2256 2022-10-27 12:17:55.000000 pddl-plus-parser-3.5.8/tests/multi_agent_tests/multi_agent_problem_converter_test.py
--rw-rw-rw-   0        0        0     8908 2022-12-05 15:59:59.000000 pddl-plus-parser-3.5.8/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py
--rw-rw-rw-   0        0        0     6939 2022-10-27 08:18:32.000000 pddl-plus-parser-3.5.8/tests/multi_agent_tests/single_agent_plan_converter_test.py
+drwxrwxrwx   0        0        0        0 2024-03-24 13:50:28.957942 pddl-plus-parser-3.5.9/
+-rw-rw-rw-   0        0        0    11499 2022-01-08 09:02:31.000000 pddl-plus-parser-3.5.9/LICENSE
+-rw-rw-rw-   0        0        0     3764 2024-03-24 13:50:28.956945 pddl-plus-parser-3.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3440 2024-03-19 16:46:02.000000 pddl-plus-parser-3.5.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-24 13:50:28.833535 pddl-plus-parser-3.5.9/pddl_plus_parser/
+-rw-rw-rw-   0        0        0        0 2022-03-13 12:11:09.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-24 13:50:28.847801 pddl-plus-parser-3.5.9/pddl_plus_parser/exporters/
+-rw-rw-rw-   0        0        0      264 2022-08-21 09:19:40.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/exporters/__init__.py
+-rw-rw-rw-   0        0        0     7553 2022-08-21 12:45:31.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/exporters/domain_exporter.py
+-rw-rw-rw-   0        0        0     1348 2022-06-02 13:51:41.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/exporters/enhsp_output_parser.py
+-rw-rw-rw-   0        0        0     3677 2023-09-13 08:00:01.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/exporters/ff_output_parser.py
+-rw-rw-rw-   0        0        0     6141 2023-03-14 07:34:52.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/exporters/numeric_trajectory_exporter.py
+-rw-rw-rw-   0        0        0     4444 2024-03-19 10:35:44.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/exporters/problem_exporter.py
+drwxrwxrwx   0        0        0        0 2024-03-24 13:50:28.860511 pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/
+-rw-rw-rw-   0        0        0      376 2023-06-18 20:40:16.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/__init__.py
+-rw-rw-rw-   0        0        0    14713 2023-04-13 11:10:47.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/domain_parser.py
+-rw-rw-rw-   0        0        0    10635 2023-04-17 10:32:20.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/effects_parser.py
+-rw-rw-rw-   0        0        0     2998 2023-04-13 11:23:17.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/parsing_utils.py
+-rw-rw-rw-   0        0        0      200 2022-01-09 12:51:47.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/pddl_parser_types.py
+-rw-rw-rw-   0        0        0     2610 2022-12-05 08:48:42.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py
+-rw-rw-rw-   0        0        0     5558 2023-04-13 11:44:39.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/preconditions_parser.py
+-rw-rw-rw-   0        0        0    11961 2022-12-05 08:49:12.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/problem_parser.py
+-rw-rw-rw-   0        0        0    13065 2023-06-18 20:51:11.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/trajectory_parser.py
+drwxrwxrwx   0        0        0        0 2024-03-24 13:50:28.887592 pddl-plus-parser-3.5.9/pddl_plus_parser/models/
+-rw-rw-rw-   0        0        0      835 2023-05-01 08:05:47.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/__init__.py
+-rw-rw-rw-   0        0        0     1296 2023-02-19 07:22:18.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/action_call.py
+-rw-rw-rw-   0        0        0     1935 2023-05-01 08:11:11.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/conditional_effect.py
+-rw-rw-rw-   0        0        0     6181 2023-11-20 15:42:29.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/grounded_effect.py
+-rw-rw-rw-   0        0        0    13736 2023-08-09 07:43:30.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/grounded_precondition.py
+-rw-rw-rw-   0        0        0     6340 2023-04-16 14:57:28.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/grounding_utils.py
+-rw-rw-rw-   0        0        0     5141 2024-03-24 13:49:22.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/numeric_symbolic_operations.py
+-rw-rw-rw-   0        0        0     9729 2024-03-24 13:15:41.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/numerical_expression.py
+-rw-rw-rw-   0        0        0     3753 2022-12-05 08:50:29.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/observation.py
+-rw-rw-rw-   0        0        0     1293 2023-04-13 13:54:50.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_action.py
+-rw-rw-rw-   0        0        0     2279 2023-11-11 13:51:14.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_domain.py
+-rw-rw-rw-   0        0        0     3973 2023-04-16 13:39:30.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_function.py
+-rw-rw-rw-   0        0        0      460 2023-11-11 13:50:18.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_object.py
+-rw-rw-rw-   0        0        0     8675 2023-05-16 11:04:11.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_operator.py
+-rw-rw-rw-   0        0        0    11315 2024-03-08 14:49:21.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_precondition.py
+-rw-rw-rw-   0        0        0     4737 2023-04-16 13:37:45.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_predicate.py
+-rw-rw-rw-   0        0        0     1953 2022-11-18 11:18:07.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_problem.py
+-rw-rw-rw-   0        0        0     4462 2023-11-25 13:38:32.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_state.py
+-rw-rw-rw-   0        0        0     1221 2023-11-11 13:50:31.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_type.py
+drwxrwxrwx   0        0        0        0 2024-03-24 13:50:28.896738 pddl-plus-parser-3.5.9/pddl_plus_parser/multi_agent/
+-rw-rw-rw-   0        0        0      324 2023-02-21 12:20:37.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/multi_agent/__init__.py
+-rw-rw-rw-   0        0        0     2139 2023-04-17 11:31:48.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/multi_agent/common.py
+-rw-rw-rw-   0        0        0     3282 2023-04-17 10:59:23.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py
+-rw-rw-rw-   0        0        0     3031 2022-12-05 09:13:45.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py
+-rw-rw-rw-   0        0        0     7079 2023-02-19 14:32:32.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py
+-rw-rw-rw-   0        0        0    10857 2023-04-17 11:26:47.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/multi_agent/single_agent_plan_converter.py
+drwxrwxrwx   0        0        0        0 2024-03-24 13:50:28.915776 pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/
+-rw-rw-rw-   0        0        0       40 2022-05-10 14:32:52.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/__init__.py
+-rw-rw-rw-   0        0        0      357 2022-09-28 11:37:49.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/common.py
+-rw-rw-rw-   0        0        0     3314 2024-03-20 14:59:17.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/counters_generator.py
+-rw-rw-rw-   0        0        0     1371 2024-03-20 13:39:22.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/depot_generator.py
+-rw-rw-rw-   0        0        0     1651 2024-03-20 13:44:58.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/driverlog_generator.py
+-rw-rw-rw-   0        0        0     6091 2024-03-20 15:05:16.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/farmland_generator.py
+-rw-rw-rw-   0        0        0     2227 2023-08-06 09:42:00.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/minecraft_generator.py
+-rw-rw-rw-   0        0        0     3756 2022-08-04 13:43:32.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/plant_watering_generator.py
+-rw-rw-rw-   0        0        0     3786 2024-03-20 17:17:01.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/sailing_generator.py
+-rw-rw-rw-   0        0        0     1649 2024-03-20 14:48:55.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/satellite_generator.py
+-rw-rw-rw-   0        0        0    12311 2022-05-16 19:14:35.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/settlers_problem_generator.py
+-rw-rw-rw-   0        0        0     8805 2022-09-28 12:16:10.000000 pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/zenotravel_generator.py
+drwxrwxrwx   0        0        0        0 2024-03-24 13:50:28.838536 pddl-plus-parser-3.5.9/pddl_plus_parser.egg-info/
+-rw-rw-rw-   0        0        0     3764 2024-03-24 13:50:28.000000 pddl-plus-parser-3.5.9/pddl_plus_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3922 2024-03-24 13:50:28.000000 pddl-plus-parser-3.5.9/pddl_plus_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-24 13:50:28.000000 pddl-plus-parser-3.5.9/pddl_plus_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-03-24 13:50:28.000000 pddl-plus-parser-3.5.9/pddl_plus_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-24 13:50:28.957942 pddl-plus-parser-3.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      492 2024-03-24 13:49:57.000000 pddl-plus-parser-3.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-24 13:50:28.827990 pddl-plus-parser-3.5.9/tests/
+drwxrwxrwx   0        0        0        0 2024-03-24 13:50:28.921338 pddl-plus-parser-3.5.9/tests/exporters_tests/
+-rw-rw-rw-   0        0        0        0 2022-02-28 12:11:52.000000 pddl-plus-parser-3.5.9/tests/exporters_tests/__init__.py
+-rw-rw-rw-   0        0        0     1262 2024-03-19 10:39:19.000000 pddl-plus-parser-3.5.9/tests/exporters_tests/consts.py
+-rw-rw-rw-   0        0        0    10075 2024-03-19 10:37:02.000000 pddl-plus-parser-3.5.9/tests/exporters_tests/numeric_trajectory_exporter_test.py
+-rw-rw-rw-   0        0        0     2784 2024-03-19 10:43:43.000000 pddl-plus-parser-3.5.9/tests/exporters_tests/problem_exporter_test.py
+drwxrwxrwx   0        0        0        0 2024-03-24 13:50:28.930361 pddl-plus-parser-3.5.9/tests/lisp_parsers_tests/
+-rw-rw-rw-   0        0        0        0 2022-01-09 08:03:59.000000 pddl-plus-parser-3.5.9/tests/lisp_parsers_tests/__init__.py
+-rw-rw-rw-   0        0        0     3503 2023-06-18 20:27:00.000000 pddl-plus-parser-3.5.9/tests/lisp_parsers_tests/consts.py
+-rw-rw-rw-   0        0        0    40370 2024-02-24 16:19:58.000000 pddl-plus-parser-3.5.9/tests/lisp_parsers_tests/domain_parser_test.py
+-rw-rw-rw-   0        0        0     3578 2024-01-23 11:15:50.000000 pddl-plus-parser-3.5.9/tests/lisp_parsers_tests/pddl_tokenizer_test.py
+-rw-rw-rw-   0        0        0    17734 2022-08-21 10:17:02.000000 pddl-plus-parser-3.5.9/tests/lisp_parsers_tests/problem_parser_test.py
+-rw-rw-rw-   0        0        0     7601 2023-06-18 20:45:34.000000 pddl-plus-parser-3.5.9/tests/lisp_parsers_tests/trajectory_parser_test.py
+drwxrwxrwx   0        0        0        0 2024-03-24 13:50:28.945416 pddl-plus-parser-3.5.9/tests/models_tests/
+-rw-rw-rw-   0        0        0        0 2022-01-10 14:06:38.000000 pddl-plus-parser-3.5.9/tests/models_tests/__init__.py
+-rw-rw-rw-   0        0        0      946 2024-01-23 11:19:09.000000 pddl-plus-parser-3.5.9/tests/models_tests/consts.py
+-rw-rw-rw-   0        0        0    16596 2023-11-20 16:00:08.000000 pddl-plus-parser-3.5.9/tests/models_tests/grounded_effect_test.py
+-rw-rw-rw-   0        0        0    27127 2023-05-14 10:23:35.000000 pddl-plus-parser-3.5.9/tests/models_tests/grounded_precondition_test.py
+-rw-rw-rw-   0        0        0    15299 2024-03-19 16:48:12.000000 pddl-plus-parser-3.5.9/tests/models_tests/numeric_symbolic_operations_test.py
+-rw-rw-rw-   0        0        0    14990 2024-03-24 13:15:08.000000 pddl-plus-parser-3.5.9/tests/models_tests/numerical_expression_test.py
+-rw-rw-rw-   0        0        0    19392 2023-04-17 09:59:27.000000 pddl-plus-parser-3.5.9/tests/models_tests/operator_test.py
+-rw-rw-rw-   0        0        0     1646 2022-06-21 11:55:51.000000 pddl-plus-parser-3.5.9/tests/models_tests/pddl_function_test.py
+-rw-rw-rw-   0        0        0     7449 2023-08-25 14:53:40.000000 pddl-plus-parser-3.5.9/tests/models_tests/pddl_precondition_test.py
+-rw-rw-rw-   0        0        0     3659 2023-11-25 13:50:20.000000 pddl-plus-parser-3.5.9/tests/models_tests/pddl_state_test.py
+drwxrwxrwx   0        0        0        0 2024-03-24 13:50:28.955964 pddl-plus-parser-3.5.9/tests/multi_agent_tests/
+-rw-rw-rw-   0        0        0        0 2022-08-18 10:56:04.000000 pddl-plus-parser-3.5.9/tests/multi_agent_tests/__init__.py
+-rw-rw-rw-   0        0        0     1706 2022-11-13 14:49:21.000000 pddl-plus-parser-3.5.9/tests/multi_agent_tests/consts.py
+-rw-rw-rw-   0        0        0     2123 2023-04-17 11:05:34.000000 pddl-plus-parser-3.5.9/tests/multi_agent_tests/multi_agent_domain_converter_test.py
+-rw-rw-rw-   0        0        0     2256 2022-10-27 12:17:55.000000 pddl-plus-parser-3.5.9/tests/multi_agent_tests/multi_agent_problem_converter_test.py
+-rw-rw-rw-   0        0        0     8908 2022-12-05 15:59:59.000000 pddl-plus-parser-3.5.9/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py
+-rw-rw-rw-   0        0        0     6939 2022-10-27 08:18:32.000000 pddl-plus-parser-3.5.9/tests/multi_agent_tests/single_agent_plan_converter_test.py
```

### Comparing `pddl-plus-parser-3.5.8/LICENSE` & `pddl-plus-parser-3.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/PKG-INFO` & `pddl-plus-parser-3.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pddl-plus-parser
-Version: 3.5.8
+Version: 3.5.9
 Summary: Parser of PDDL+ domains and problems for learning purposes
 Author: Argaman Mordoch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pddl-plus-parser Version: 3.5.8 Summary: Parser of
+Metadata-Version: 2.1 Name: pddl-plus-parser Version: 3.5.9 Summary: Parser of
 PDDL+ domains and problems for learning purposes Author: Argaman Mordoch
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE
                         ************ PPDDDDLL PPlluuss PPaarrsseerr ************
   _[_P_y_P_I_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_][PyPI - Status][PyPI - Implementation][PyPI -
                                 Wheel]_[_G_i_t_H_u_b_]
                           [test][lint][docs]_[_c_o_d_e_c_o_v_]
```

### Comparing `pddl-plus-parser-3.5.8/README.md` & `pddl-plus-parser-3.5.9/README.md`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/exporters/domain_exporter.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/exporters/domain_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/exporters/enhsp_output_parser.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/exporters/enhsp_output_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/exporters/ff_output_parser.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/exporters/ff_output_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/exporters/numeric_trajectory_exporter.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/exporters/numeric_trajectory_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/exporters/problem_exporter.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/exporters/problem_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/domain_parser.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/domain_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/effects_parser.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/effects_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/parsing_utils.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/preconditions_parser.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/preconditions_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/problem_parser.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/problem_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/lisp_parsers/trajectory_parser.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/lisp_parsers/trajectory_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/__init__.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/action_call.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/action_call.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/conditional_effect.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/conditional_effect.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/grounded_effect.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/grounded_effect.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/grounded_precondition.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/grounded_precondition.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/grounding_utils.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/grounding_utils.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/numeric_symbolic_operations.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/numeric_symbolic_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,17 @@
     """Converts a recursive expression to a PDDL format.
 
     :param expression: the expression to convert.
     :return: the string representing the PDDL expression.
     """
     exponent = expression.exp
     compiled_expression = f"{symbols_map[expression.base]}"
+    if exponent == -1:
+        return f"(/ 1 {compiled_expression})"
+
     for _ in range(exponent - 1):
         compiled_expression = f"(* {compiled_expression} {symbols_map[expression.base]})"
 
     return compiled_expression
 
 
 def _convert_internal_expression_to_pddl(expression: Expr, operator: str, symbols_map: dict) -> str:
@@ -69,15 +72,18 @@
     :param operator: the numeric operator of the current sympy expression.
     :param symbols_map: the map between the symbolic expression and the PDDL expression.
     :return: the string representing the PDDL expression.
     """
     if expression.is_Atom:
         return extract_atom(expression, symbols_map)
 
-    if isinstance(expression, Pow):
+    if isinstance(expression, Pow) and expression.exp == -1:
+        return f"(/ 1 {_convert_internal_expression_to_pddl(expression.base, SYMPY_OP_TO_PDDL_OP[expression.base.func], symbols_map)})"
+
+    if isinstance(expression, Pow) and expression.exp > 1:
         return _recursive_pow_expression_to_pddl(expression, symbols_map)
 
     # the expression is a binary expression with multiple arguments
     components = [_convert_internal_expression_to_pddl(
         expression.args[i], SYMPY_OP_TO_PDDL_OP[expression.args[i].func], symbols_map) for i in
         range(len(expression.args))]
```

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/numerical_expression.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/numerical_expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         :return: the PDDL string of the expression.
         """
         if node.is_leaf:
             if isinstance(node.value, PDDLFunction):
                 function: PDDLFunction = node.value
                 return function.untyped_representation
 
-            return node.value
+            return f"{node.value:.2f}" if isinstance(node.value, float) else node.value
 
         left_operand = self._convert_to_pddl(node.children[0])
         right_operand = self._convert_to_pddl(node.children[1])
         return f"({node.value} {left_operand} {right_operand})"
 
     def _convert_to_mathematical(self, node: AnyNode) -> str:
         """Recursive method that converts the expression tree to a PDDL string.
```

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/observation.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/observation.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_action.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_action.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_domain.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_domain.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_function.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_function.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_operator.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_operator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_precondition.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_precondition.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_predicate.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_predicate.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_problem.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_problem.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_state.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_state.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/models/pddl_type.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/models/pddl_type.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/multi_agent/common.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/multi_agent/common.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/multi_agent/single_agent_plan_converter.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/multi_agent/single_agent_plan_converter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/counters_generator.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/counters_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,26 +41,26 @@
     parser.add_argument("--output_path", required=True,
                         help="The path to the output folder where the problems will be saved")
     args = parser.parse_args()
     return args
 
 
 def generate_multiple_problems(
-        min_counters: int, max_counters: int, max_int: int, output_folder: Path) -> NoReturn:
+        min_counters: int, max_counters: int, max_int: int, output_folder: Path, total_num_problems: int = 100) -> NoReturn:
     """Generate multiple problems based on the input arguments.
 
     :param min_counters: the minimal number of counters possible in the problems.
     :param max_counters: the maximal number of counters possible in the problems.
     :param max_int: the maximal integer value.
     :param output_folder: the path to the output folder where the problems will be saved.
     """
-    counters_range = [i for i in range(min_counters, max_counters + 1)]
-    for num_counters in counters_range:
+    for i in range(total_num_problems):
+        num_counters = random.randint(min_counters, max_counters)
         print(f"Generating problem with {num_counters} counters")
-        with open(output_folder / f"pfile{num_counters}_{random.randint(0, 100)}.pddl", "wt") as problem_file:
+        with open(output_folder / f"pfile{i}.pddl", "wt") as problem_file:
             problem_file.write(
                 generate_instance(f"instance_{num_counters}_{max_int}", num_counters, max_int))
 
 
 def main():
     args = parse_arguments()
     generate_multiple_problems(min_counters=int(args.min_counters),
```

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/depot_generator.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/depot_generator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 import random
 import subprocess
 import sys
 from pathlib import Path
 
 
-def generate_problems(output_directory: Path, num_probs_per_difficulty: int = 20):
+def generate_problems(output_directory: Path, num_probs_per_difficulty: int = 50):
     print("generating problems for the depot domain...")
     for i in range(num_probs_per_difficulty):
         # Generate problems for the easy difficulty
-        problem_name = f"depot_easy_{i}.pddl"
+        problem_name = f"pfile{i}.pddl"
         problem_path = output_directory / problem_name
-        generate_problem_command = f"./depotgen {i} -n -w 100 -c 400 1 2 2 3 3 {random.randint(2, 30)} > {problem_path}"
+        generate_problem_command = f"./depotgen {random.randint(1, 100)} -n -w 100 -c 400 1 2 2 3 3 {random.randint(2, 15)} > {problem_path}"
         print(f"generating problem {problem_name}...")
         subprocess.check_output(generate_problem_command, shell=True)
 
     for i in range(num_probs_per_difficulty):
         # Generate problems for the medium difficulty
-        problem_name = f"depot_medium_{i}.pddl"
+        problem_name = f"pfile{num_probs_per_difficulty + i}.pddl"
         problem_path = output_directory / problem_name
-        generate_problem_command = f"./depotgen {i} -n -w 100 -c 400 3 3 2 {random.randint(6, 15)} {random.randint(6, 15)} {random.randint(2, 30)} > {problem_path}"
-        print(f"generating problem {problem_name}...")
-        subprocess.check_output(generate_problem_command, shell=True)
-
-    for i in range(num_probs_per_difficulty):
-        # Generate problems for the hard difficulty
-        problem_name = f"depot_hard_{i}.pddl"
-        problem_path = output_directory / problem_name
-        generate_problem_command = f"./depotgen {i} -n -w 100 -c 400 {random.randint(4, 8)} {random.randint(4, 8)} 2 {random.randint(6, 15)} {random.randint(6, 15)} {random.randint(2, 30)} > {problem_path}"
+        generate_problem_command = f"./depotgen {random.randint(1, 100)} -n -w 100 -c 400 3 3 2 {random.randint(6, 15)} {random.randint(6, 15)} {random.randint(2, 30)} > {problem_path}"
         print(f"generating problem {problem_name}...")
         subprocess.check_output(generate_problem_command, shell=True)
 
 
 def main():
     output_directory = sys.argv[1]
     generate_problems(Path(output_directory))
```

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/depots_generator.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/settlers_problem_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,351 +1,408 @@
 import enum
 import random
 import sys
+from collections import OrderedDict
+from queue import Queue
 
 
 class typeStatus(enum.Enum):
     OFF = 0
     ON = 1
 
 
 typing = typeStatus
+st = str()
 
-
-def rnd(limit):
-    return 1 + int(limit * random.random())
-
-
-def rnd2(limit):
-    return limit / 2 + rnd(limit / 2)
-
-
-def rnd3(locs, limit):
-    return int(locs * (1.0 + ((limit - 1) * random.random())))
-
-
-class locatable:
-    def __init__(self, locs=-1):
-        if locs == -1:
-            self.location = 0
+class probTypes(enum.Enum):
+    STRIPS = 0
+    NUMERIC = 1
+    SIMPLETIME = 2
+    TIMED = 3
+    COMPLEX = 4
+    HARDNUMERIC = 5
+
+
+probType = probTypes
+
+def rnd(limit=-1):
+    if limit == -1:
+        return float(random.random())
+    return int(limit * random.random())
+
+class ProblemObject:
+    class OutStatus(enum.Enum):
+        OBJECT = 0
+        INIT = 1
+        GOAL = 2
+    def object(self):
+        raise NotImplementedError
+    def init(self):
+        raise NotImplementedError
+    def goal(self):
+        raise NotImplementedError
+    def write(self):
+        global outStatus
+        if outStatus == ProblemObject.OutStatus.OBJECT:
+            self.object()
+        elif outStatus == ProblemObject.OutStatus.INIT:
+            self.init()
+        elif outStatus == ProblemObject.OutStatus.GOAL:
+            self.goal()
+    @classmethod
+    def Objects(self):
+        global outStatus
+        outStatus = ProblemObject.OutStatus.OBJECT
+    @classmethod
+    def Inits(self):
+        global outStatus
+        outStatus = ProblemObject.OutStatus.INIT
+    @classmethod
+    def Goals(self):
+        global outStatus
+        outStatus = ProblemObject.OutStatus.GOAL
+    
+outStatus = ProblemObject.OutStatus.OBJECT
+
+class IOManipulator(object):
+    def __init__(self, function=None):
+        self.function = function
+    def do(self, output):
+        self.function(output)
+def do_endl(stream):
+    stream.output.write('\n')
+endl = IOManipulator(do_endl)
+
+class OStream(object):
+    def __init__(self, output=None):
+        if output is None:
+            output = sys.stdout
+        self.output = output
+        self.format = '%s'
+    def __lshift__(self, thing):
+        if isinstance(thing, IOManipulator):
+            self.output.write(thing)
+            return OStream()
         else:
-            self.location = rnd(locs)
-
-
-class Truck(locatable):
-    def __init__(self, locs, maxc):
-        locatable.__init__(self, locs)
-        self.capacity = rnd2(maxc)
-        self.speed = rnd(10)
-
-
-class Pallet(locatable):
-    def __init__(self, locs):
-        locatable.__init__(self, locs)
-        self.topcrate = 0
-        self.dtopcrate = 0
-
-maxWeight = 0
-
-class Crate(locatable):
-
-    def __init__(self, ps, maxw):
-        locatable.__init__(self)
-        self.pallet = rnd(ps)
-        self.weight = rnd(maxw)
-        self.dpallet = 0
-        self.dsurface = 0
-        self.surface = int()
-        global maxWeight
-        maxWeight = self.weight if self.weight > maxWeight else maxWeight
-
-class Hoist(locatable):
-    def __init__(self, locs):
-        locatable.__init__(self, locs)
-        self.powr = rnd(10)
-
-
-class Map:
-    def __init__(self, locs):
-        self.distances = []
-        for i in range(locs):
-            self.distances.append(list())
-            for j in range(locs):
-                self.distances[i].append(rnd(10))
-
-
-class DepotDescriptor:
-    class ProblemType(enum.Enum):
-        STRIPS = 0
-        NUMERIC = 1
-        SIMPLETIMED = 2
-        TIMED = 3
-
-    def __init__(self, dps, dsts, trks, plts, hsts, crts, tp=ProblemType.STRIPS, mxwt=0, mxcp=0):
-        self.numDepots = dps
-        self.numDistributors = dsts
-        self.numTrucks = trks
-        self.numPallets = plts
-        self.numHoists = hsts
-        self.numCrates = crts
-        self.probtype = tp
-        self.maxCapacity = mxcp
-        self.maxWeight = mxwt
-
-
-class Depot:
-    def __init__(self, s, d, f):
-        self.__seed = s
-        self.__probtype = d.probtype
-        random.seed(s)
-        self.__numDepots = d.numDepots
-        self.__numDistributors = d.numDistributors
-        self.numTrucks = d.numTrucks
-        self.locs = self.__numDepots + self.__numDistributors
-        self.__m = Map(self.locs)
-        self.numPallets = max(d.numPallets, self.locs)
-        self.numHoists = max(d.numHoists, self.locs)
-        self.__trucks = []
-        self.__pallets = []
-        self.__hoists = []
-        self.__crates = []
-        self.file = f
-        for i in range(self.numTrucks):
-            t = Truck(self.locs, d.maxCapacity)
-            self.__trucks.append(t)
-        for i in range(self.numHoists):
-            h = Hoist(self.locs)
-            if i < self.locs:
-                h.location = i + 1
-            self.__hoists.append(h)
-        for i in range(self.numPallets):
-            p = Pallet(self.locs)
-            if i < self.locs:
-                p.location = i + 1
-            self.__pallets.append(p)
-        for i in range(d.numCrates):
-            c = Crate(self.numPallets, d.maxWeight)
-            c.location = self.__pallets[c.pallet - 1].location
-            c.surface = self.__pallets[c.pallet - 1].topcrate
-            self.__pallets[c.pallet - 1].topcrate = i + 1
-            self.__crates.append(c)
-        for i in range(2 * d.numCrates):
-            c = rnd(d.numCrates) - 1
-            if self.__crates[c].dpallet:
-                continue
-            self.__crates[c].dpallet = rnd(self.numPallets)
-            self.__crates[c].dsurface = self.__pallets[self.__crates[c].dpallet - 1].dtopcrate
-            self.__pallets[self.__crates[c].dpallet - 1].dtopcrate = c + 1
-
-    def __location(self, i):
-        if type(i) != int:
-            i = i.location - 1
-        if i < self.__numDepots:
-            self.file.write(f"depot{i}")
-        else:
-            self.file.write(f"distributor{i - self.__numDepots}")
-
-
-    def __del__(self):
-        del self.__m
-
-    def write(self):  
-        global maxWeight
-        self.file.write(
-            f"(define (problem depotprob{self.__seed}) (:domain Depot)\n(:objects\n\t")
-        for i in range(self.__numDepots):
-            self.file.write(f"depot{i} ")
-        if typing == typeStatus.ON:
-            self.file.write("- Depot\n\t")
-        for i in range(self.__numDistributors):
-            self.file.write(f"distributor{i} ")
-        if typing == typeStatus.ON:
-            self.file.write("- Distributor\n\t")
-        for i in range(len(self.__trucks)):
-            self.file.write(f"truck{i} ")
+            self.output.write(self.format % thing)
+            self.format = '%s'
+        return OStream()
+
+
+seaZones = [set() for _ in range(4)]
+
+id = 0
+
+class Place(ProblemObject):
+	
+    def __init__(self):
+        global id
+        self.__place = id
+        id += 1
+        self.__mountain = rnd(10) < 3
+        self.__woodland = rnd(10) < 6
+        self.__metalliferous = rnd(10) < 2
+        self.__bycoast = rnd(10) < 5
+        self.__seaZone = rnd(4)
+        global seaZones
+        if self.__bycoast: 
+            seaZones[self.__seaZone].add(self.__place)
+
+    def makeMountain(self):
+        self.__mountain = True
+    def makeWoodland(self):
+        self.__woodland = True
+    def makeMetalliferous(self):
+        self.__metalliferous = True
+
+    def object(self):
+        global typing
+        global st
+        st += f"\tlocation{self.__place}"
         if typing == typeStatus.ON:
-            self.file.write("- Truck\n\t")
-        for i in range(len(self.__pallets)):
-            self.file.write(f"pallet{i} ")
-        if typing == typeStatus.ON:
-            self.file.write("- Pallet\n\t")
-        for i in range(len(self.__crates)):
-            self.file.write(f"crate{i} ")
-        if typing == typeStatus.ON:
-            self.file.write("- Crate\n\t")
-        for i in range(len(self.__hoists)):
-            self.file.write(f"hoist{i} ")
-        if typing == typeStatus.ON:
-            self.file.write("- Hoist")
-        self.file.write(")\n(:init\n")
-        for i in range(len(self.__pallets)):
-            if typing == typeStatus.OFF:
-                self.file.write(f"\t(pallet pallet{i})\n")
-                self.file.write(f"\t(surface pallet{i})\n")
-            self.file.write(f"\t(at pallet{i} ")
-            self.__location(self.__pallets[i])
-            self.file.write(")\n\t(clear ")
-            if self.__pallets[i].topcrate:
-                self.file.write(
-                    f"crate{self.__pallets[i].topcrate - 1})\n")
-            else:
-                self.file.write(f"pallet{i})\n")
-        for i in range(len(self.__trucks)):
-            if typing == typeStatus.OFF:
-                self.file.write(f"\t(truck truck{i})\n")
-            self.file.write(f"\t(at truck{i} ")
-            self.__location(self.__trucks[i])
-            self.file.write(")\n")
-            if self.__probtype == DepotDescriptor.ProblemType.TIMED:
-                self.file.write(
-                    f"\t(= (speed truck{i}) {self.__trucks[i].speed})\n")
-            if self.__probtype == DepotDescriptor.ProblemType.NUMERIC:
-                self.file.write(
-                    f"\t(= (current_load truck{i}) 0)\n\t(= (load_limit truck{i}) ")
-                if ((2 * self.__trucks[i].capacity) < maxWeight) or i == 0:
-                    self.file.write(
-                        f"{str(self.__trucks[i].capacity + maxWeight)})\n")
-                else:
-                    self.file.write(
-                        f"{str(self.__trucks[i].capacity)})\n")
-        for i in range(len(self.__hoists)):
-            if typing == typeStatus.OFF:
-                self.file.write(f"\t(hoist hoist{i})\n")
-            self.file.write(f"\t(at hoist{i} ")
-            self.__location(self.__hoists[i])
-            self.file.write(f")\n\t(available hoist{i})\n")
-            if self.__probtype == DepotDescriptor.ProblemType.TIMED:
-                self.file.write(
-                    f"\t(= (power hoist{i}) {self.__hoists[i].powr})\n")
-        for i in range(len(self.__crates)):
-            if typing == typeStatus.OFF:
-                self.file.write(f"\t(crate crate{i})\n")
-                self.file.write(f"\t(surface crate{i})\n")
-            self.file.write(f"\t(at crate{i} ")
-            self.__location(self.__crates[i])
-            self.file.write(f")\n\t(on crate{i} ")
-            if self.__crates[i].surface:
-                self.file.write(
-                    f"crate{self.__crates[i].surface - 1})\n")
-            else:
-                self.file.write(
-                    f"pallet{self.__crates[i].pallet - 1})\n")
-            if self.__probtype == DepotDescriptor.ProblemType.NUMERIC or self.__probtype == DepotDescriptor.ProblemType.TIMED:
-                self.file.write(
-                    f"\t(= (weight crate{i}) {self.__crates[i].weight})\n")
+            st += " - place"
+        st += "\n"
+    def init(self):
+        global typing
+        global st
         if typing == typeStatus.OFF:
-            for i in range(self.__numDepots + self.__numDistributors):
-                self.file.write("\t(place ")
-                self.__location(i)
-                self.file.write(")\n")
-        if self.__probtype == DepotDescriptor.ProblemType.TIMED:
-            for i in range(len(self.__m.distances)):
-                for j in range(len(self.__m.distances[i])):
-                    self.file.write("\t(= (distance ")
-                    self.__location(i)
-                    self.file.write(" ")
-                    self.__location(j)
-                    self.file.write(") ")
-                    if j != i:
-                        self.file.write(
-                            f"{self.__m.distances[i][j]})\n")
-                    else:
-                        self.file.write("0)\n")
-
-        if self.__probtype == DepotDescriptor.ProblemType.NUMERIC:
-            self.file.write("\t(= (fuel-cost) 0)\n")
-
-        self.file.write(")\n\n(:goal (and\n")
-        for i in range(len(self.__crates)):
-            if self.__crates[i].dpallet:
-                if self.__crates[i].dsurface:
-                    self.file.write(
-                        f"\t\t(on crate{i} crate{self.__crates[i].dsurface - 1})\n")
-                else:
-                    self.file.write(
-                        f"\t\t(on crate{i} pallet{self.__crates[i].dpallet - 1})\n")
-        self.file.write("\t)\n)")
-        if self.__probtype != DepotDescriptor.ProblemType.STRIPS and self.__probtype != DepotDescriptor.ProblemType.NUMERIC:
-            self.file.write("\n\n(:metric minimize (total-time))")
-        if self.__probtype == DepotDescriptor.ProblemType.NUMERIC:
-            if rnd(10) < 4:
-                self.file.write("\n\n(:metric minimize (fuel-cost))")
-            else:
-                self.file.write("\n\n(:metric minimize (total-time))")
-        self.file.write(")\n")
-
-
-def usage():
-    print("Usage: gdep <seed> [-s|-t|-n|-w <weight>|-c <capacity>|-f <filename>]\n\t\t<#depots> <#distributors> <#trucks> <#pallets> <#hoists> <#crates>\n\n\tOptions:\n\tu: untyped\n\ts: simple-time\n\tt: time\n\tn: numeric\n\tw: provide maximum weight for crates\n\tc: maximum capacity for trucks\n\tf: optional file for output\n\n\tAll numbers are integers.\n\n")
-    exit(0)
+            st += f"\t(place location{self.__place})\n"
+        if self.__mountain:
+            st += f"\t(mountain location{self.__place})\n"
+        if self.__woodland:
+            st += f"\t(woodland location{self.__place})\n"
+        if self.__bycoast:
+            st += f"\t(by-coast location{self.__place})\n"
+        if self.__metalliferous:
+            st += f"\t(metalliferous location{self.__place})\n"
+        st += f"\t(= (housing location{self.__place}) 0)\n" + \
+            f"\t(= (available wood location{self.__place}) 0)\n" + \
+            f"\t(= (available timber location{self.__place}) 0)\n" + \
+            f"\t(= (available ore location{self.__place}) 0)\n" + \
+            f"\t(= (available stone location{self.__place}) 0)\n" + \
+            f"\t(= (available iron location{self.__place}) 0)\n" + \
+            f"\t(= (available coal location{self.__place}) 0)\n"
+    def goal(self):
+        pass
+    def __str__(self):
+        return st
 
 
-def commandLine(seed, filename, argc, argv):
-    probtype = DepotDescriptor.ProblemType.STRIPS
-    global typing
-    wgt = 1
-    cap = 1
-    nxt = 0
-    val = [0 for _ in range(6)]
-
-    if argc <= 0:
-        usage()
-
-    seed = int(argv[0])
-    argc -= 1
-    argv = argv[1:]
-
-    while argc > 0:
-        if argv[0][0] == '-':
-            o = argv[0][1]
-            if o == 't':
-                probtype = DepotDescriptor.ProblemType.TIMED
-            elif o == 's':
-                probtype = DepotDescriptor.ProblemType.SIMPLETIMED
-            elif o == 'n':
-                probtype = DepotDescriptor.ProblemType.NUMERIC
-            elif o == 'u':
-                typing = typeStatus.OFF
+class Goal(ProblemObject):
+    def __del__(self):
+        pass
+    def object(self):
+        raise NotImplementedError
+    def init(self):
+        raise NotImplementedError
+
+def random_select(s):
+    i = rnd(len(s))
+    for val in s:
+        while i > 0:
+            i-=1
+        return val
+    return val
+
+links = set()
+
+class RailLink(Goal):
+    def __init__(self, g, nlocs, length):
+        self.start = rnd(nlocs)
+        self.__locs = list()
+        self.__locs.append(self.start)
+        for i in range(length):
+            if not g[self.start]: return # graph g int -> set
+            self.start = random_select(g[self.start])
+            if self.__locs[len(self.__locs) - 1] != self.start:
+                self.__locs.append(self.start)
+    def goal(self):
+        global st
+        global links
+        for i in range(len(self.__locs) - 1):
+            if (self.__locs[i], self.__locs[i+1]) not in links:
+                st += f"\t(connected-by-rail location{self.__locs[i]} location{self.__locs[i+1]})\n"
+                links.add((self.__locs[i], self.__locs[i+1]))
+    def __repr__(self):
+        return st
+
+allBuildings = set()
+numBuildings = 3
+buildingName = ["coal-stack", "sawmill", "ironworks"]
+
+class Building(Goal):
+    def __init__(self, nlocs):
+        global allBuildings
+        global numBuildings
+        global buildingName
+        self.__building = rnd(numBuildings)
+        self.__loc = rnd(nlocs) 
+        while self.__loc < nlocs:
+            while self in allBuildings and self.__building < numBuildings:
+                self.__building+=1
+                if self.__building < numBuildings:
+                    break
+            self.__loc+=1
+            self.__building = 0
+        allBuildings.add(self)
+    def __hash__(self):
+        return hash((self.__building, self.__loc))
+    def __eq__(self, b):
+        return self.__building == b.__building and self.__loc == b.__loc
+    def __lt__(self, b):
+        return self.__loc < b.loc or (self.__loc == b.loc and self.__building < b.building)
+    def goal(self):
+        global buildingName
+        global st
+        st += f"\t(has-{buildingName[self.__building]} location{self.__loc})\n"
+    def __repr__(self):
+        return st
+
+places = set()
+
+class Housing(Goal):
+    def __init__(self, nlocs):
+        global places
+        if not places:
+            for i in range(nlocs):
+                places.add(i)
+        self.__place = random_select(places)
+        self.__quantity = rnd(2) + 1
+        places.remove(self.__place)
+    def goal(self):
+        global st
+        st += f"\t(>= (housing location{self.__place}) {self.__quantity})\n"
+    def __repr__(self):
+        return st
+
+
+class Map(ProblemObject):
+    def __explore(self, g, start, reached):
+        togo = Queue()
+        togo.put(start)
+        reached.add(start) #set
+        while not togo.empty():
+            loc = togo.get()
+            for i in g[loc]:
+                if i not in reached:
+                    togo.put(i)
+                    reached.add(i)
+
+    def __connect(self, g): 
+        reached = set()
+        start = rnd(self.__places)
+        self.__explore(g, start, reached)
+        while len(reached) != self.__places:
+            next = int()
+            for i in range(self.__places):
+                if i not in reached:
+                    next = i
+                    break
+            g[start].add(next)
+            start = next
+            self.__explore(g, start, reached)
+    def __init__(self, s, ngs): 
+        self.__places = s
+        self.__Places = list()
+        self.__road = OrderedDict()
+        self.__goals = list()
+        for _ in range(s):
+            self.__Places.append(Place())
+            for _ in range(4):
+                f = rnd(s)
+                t = rnd(s)
+                if t not in self.__road:
+                    self.__road[t] = set()
+                if f not in self.__road[t]:
+                    if f not in self.__road:
+                        self.__road[f] = set()
+                    self.__road[f].add(t)
+        self.__connect(self.__road)
+        self.__Places[rnd(self.__places)].makeMountain()
+        self.__Places[rnd(self.__places)].makeWoodland()
+        self.__Places[rnd(self.__places)].makeMetalliferous()
+
+        for _ in range(ngs):
+            if rnd(10) < 3:
+                self.__goals.append(RailLink(self.__road, self.__places, int(ngs/3)))
             else:
-                argc -= 1
-                argv = argv[1:]
-                if argc < 0:
-                    usage()
-                if o == 'w':
-                    wgt = int(argv[0])
-                elif o == 'c':
-                    cap = int(argv[0])
-                elif o == 'f':
-                    filename = argv[0]
+                if rnd(10) < 3:
+                    self.__goals.append(Housing(self.__places))
                 else:
-                    usage()
-            argc -= 1
-            argv = argv[1:]
-        else:
-            if nxt == 6:
-                usage()
-            val[nxt] = int(argv[0])
-            nxt += 1
-            argv = argv[1:]
-            argc -= 1
-    if nxt < 6:
-        usage()
-    return DepotDescriptor(val[0], val[1], val[2], val[3], val[4], val[5], probtype, wgt, cap), filename, seed
+                    self.__goals.append(Building(self.__places))
+    def __del__(self):
+        for i in self.__goals:
+            del i
 
+    def object(self):
+        global st
+        for p in self.__Places:
+            p.object()
+    def init(self):
+        global seaZones
+        global typing
+        global st
+        for p in self.__Places:
+            p.init()
+        if typing == typeStatus.OFF:
+            st += "\t(resource iron)\n\t(resource wood)\n\t(resource timber)\n\t(resource ore)\n\t(resource stone)\n\t(resource coal)\n"
+		
+        for k, v in self.__road.items():
+            for ele in v:
+                if k == ele:
+                    continue
+                if ele in self.__road:
+                    if ele in self.__road:
+                        if k in self.__road[ele]:
+                            continue
+
+                st += f"\t(connected-by-land location{k} location{ele})\n\t(connected-by-land location{ele} location{k})\n"
+        for i in range(4):
+            for idx, s in enumerate(seaZones[i]):
+                for t in [t1 for index, t1 in enumerate(seaZones[i]) if index > idx]:
+                    st += f"\t(connected-by-sea location{s} location{t})\n\t(connected-by-sea location{t} location{s})\n"
+
+    def goal(self):
+        global st
+        for i in self.__goals:
+            i.goal()
+    def __repr__(self):
+        return st
+
+ID = 0
+
+class Vehicle(ProblemObject):
+    def __init__(self):
+        global ID
+        self.__vnum = ID + 1
+        ID +=1
+    def object(self):
+        global st
+        global typing
+        st += f"\tvehicle{self.__vnum}"
+        if typing == typeStatus.ON:
+            st += " - vehicle"
+        st += "\n"
+    def init(self):
+        global typing
+        global st
+        if typing == typeStatus.OFF:
+            st += f"\t(vehicle vehicle{self.__vnum})\n"
+        st += f"\t(potential vehicle{self.__vnum})\n"
+    def goal(self):
+        pass
+    def __repr__(self):
+        return st
 
 def main(argc, argv):
     global typing
-    typing = typeStatus.ON
-    seed = int()
-    filename = ''
-    d, filename, seed = commandLine(seed, filename, argc - 1, argv[1:])
-    if filename != '':
-        f = open(filename, 'w')
-        dp = Depot(seed, d, f)
-        dp.write()
-        f.close()
+    global probType
+    typing = typeStatus.ON;
+    probType = probTypes.STRIPS;
+    global o
+    global st
+    if argc < 4:
+        print("Usage: settlers [-u] <seed> #<locations> #<goals> #<vehicles>\n\n\tThe number of vehicles is the number of \"potential\" vehicles.\n\n\t-u: Untyped\n\n")
+        exit(0)
+    argv = argv[1:]
+    argc -= 1
+    if argv[0][0] == '-':
+        if argv[0][1] == 'u': 
+            typing = typeStatus.OFF
+        argv = argv[1:]
+        argc -= 1
+    random.seed(int(argv[0]))
+    p = Map(int(argv[1]),int(argv[2]))
+    carts = list()
+    for _ in range(int(argv[3])):
+        carts.append(Vehicle())
+    print("(define (problem settlers)\n(:domain civ)\n(:objects\n",end='')
+    p.write()
+    o << st
+    st = ''
+    for c in carts:
+        c.write()
+        o << st
+        st = ''
+    print(")\n(:init\n\t(= (resource-use) 0)\n\t(= (labour) 0)\n\t(= (pollution) 0)\n",end='')
+    ProblemObject.Inits()
+    p.write()
+    o << st
+    st = ''
+    for c in carts:
+        c.write()
+        o << st
+        st = ''
+    print(")\n(:goal (and\n",end='')
+    ProblemObject.Goals()
+    p.write()
+    o << st
+    st = ''
+    print(f"\t)\n)\n\n(:metric minimize (+ (+ (* {rnd(4)} (pollution)) (* {rnd(4)} (resource-use))) (* {rnd(4)} (labour))))\n)\n",end='')
 
+o = OStream()
 
 if __name__ == '__main__':
     argv = sys.argv
     argc = len(argv)
     main(argc, argv)
+
```

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/driverlog_generator.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/driverlog_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 import random
 import subprocess
 import sys
 from pathlib import Path
 
 
-def generate_problems(output_directory: Path, num_probs_per_difficulty: int = 20):
+def generate_problems(output_directory: Path, num_probs_per_difficulty: int = 50):
     # The following code is a part of the driverlog_generator.py file
     # It is used to generate problems for the driverlog domain
     # The code is used to generate problems for learning purposes
     # It is not used in the main application
     print("generating problems for the driverlog domain...")
     for i in range(num_probs_per_difficulty):
         # Generate problems for the easy difficulty
-        problem_name = f"driverlog_easy_{i}.pddl"
+        problem_name = f"pfile{i}.pddl"
         problem_path = output_directory / problem_name
-        generate_problem_command = f"./dlgen -n {i} 3 {random.randint(2, 4)} {random.randint(2, 10)} {random.randint(2, 5)} 100 > {problem_path}"
+        generate_problem_command = f"./dlgen -n {random.randint(1, 100)} 3 {random.randint(2, 4)} {random.randint(2, 10)} {random.randint(2, 5)} 100 > {problem_path}"
         print(f"generating problem {problem_name}...")
         subprocess.check_output(generate_problem_command, shell=True)
 
     for i in range(num_probs_per_difficulty):
         # Generate problems for the medium difficulty
-        problem_name = f"driverlog_medium_{i}.pddl"
+        problem_name = f"pfile{num_probs_per_difficulty + i}.pddl"
         problem_path = output_directory / problem_name
-        generate_problem_command = f"./dlgen -n {i} {random.randint(5, 15)} {random.randint(3, 5)} {random.randint(3, 15)} {random.randint(3, 8)} 100 > {problem_path}"
-        print(f"generating problem {problem_name}...")
-        subprocess.check_output(generate_problem_command, shell=True)
-
-    for i in range(num_probs_per_difficulty):
-        # Generate problems for the hard difficulty
-        problem_name = f"driverlog_hard_{i}.pddl"
-        problem_path = output_directory / problem_name
-        generate_problem_command = f"./dlgen -n {i} {random.randint(15, 25)} {random.randint(5, 10)} {random.randint(10, 30)} {random.randint(5, 10)} 100 > {problem_path}"
+        generate_problem_command = f"./dlgen -n {random.randint(1, 100)} {random.randint(5, 15)} {random.randint(3, 5)} {random.randint(3, 15)} {random.randint(3, 8)} 100 > {problem_path}"
         print(f"generating problem {problem_name}...")
         subprocess.check_output(generate_problem_command, shell=True)
 
 
 def main():
     output_directory = sys.argv[1]
     generate_problems(Path(output_directory))
```

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/farmland_generator.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/farmland_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,29 +96,32 @@
                         help="Graph Generator between star (default) or strogatz or ladder",
                         default=GraphGeneratorTypes.star)
     return parser.parse_args()
 
 
 def generate_multiple_problems(min_farms: int, max_farms: int, min_num_units: int, max_num_units: int,
                                output_folder: Path,
-                               graph_generator: GraphGeneratorTypes = GraphGeneratorTypes.star) -> NoReturn:
+                               graph_generator: GraphGeneratorTypes = GraphGeneratorTypes.star,
+                               total_num_problems: int = 100) -> NoReturn:
     """Generate multiple problems based on the input arguments.
 
     :param min_farms: the minimal number of farms possible in a planning problem.
     :param max_farms: the maximal number of farms possible in a planning problem.
     :param min_num_units: the minimal number of units.
     :param max_num_units: the maximal number of units.
     :param output_folder: the path to the output folder where the planning problems will be saved.
     :param graph_generator: the type of graph generator to use.
     """
     farms_range = [i for i in range(min_farms, max_farms + 1)]
     units_range = [i for i in range(min_num_units, max_num_units + 1)]
-    for num_farms, num_units in itertools.product(farms_range, units_range):
+    for i in range(total_num_problems):
+        num_farms = random.choice(farms_range)
+        num_units = random.choice(units_range)
         print(f"Generating problem with {num_farms} farms and {num_units} units")
-        with open(output_folder / f"pfile{num_farms}_{num_units}.pddl", "wt") as problem_file:
+        with open(output_folder / f"pfile{i}.pddl", "wt") as problem_file:
             problem_file.write(generate_instance(f"instance_{num_farms}_{num_units}", num_farms, num_units,
                                                  graph_generator))
 
 
 def main():
     args = parse_arguments()
     generate_multiple_problems(min_farms=int(args.min_farms),
```

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/minecraft_generator.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/minecraft_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/plant_watering_generator.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/plant_watering_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/sailing_generator.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/sailing_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,43 +34,45 @@
 
     return template.substitute(template_mapping)
 
 
 def parse_arguments() -> argparse.Namespace:
     """Parses the command line arguments."""
     parser = argparse.ArgumentParser(description="Generate sailing planning instance")
-    parser.add_argument("--min_boats", required=True, help="Starting numer of boats")
-    parser.add_argument("--max_boats", required=True, help="Maximal number of boats")
-    parser.add_argument("--min_people", required=True, help="Min of people to save")
-    parser.add_argument("--max_people", required=True, help="Max of people to save")
-    parser.add_argument("--max_dist_goal", required=False, help="Max distance people to be rescued", default=500)
+    parser.add_argument("--min_boats", type=int, required=True, help="Starting numer of boats")
+    parser.add_argument("--max_boats", type=int, required=True, help="Maximal number of boats")
+    parser.add_argument("--min_people", type=int, required=True, help="Min of people to save")
+    parser.add_argument("--max_people", type=int, required=True, help="Max of people to save")
+    parser.add_argument("--max_dist_goal", type=int, required=False, help="Max distance people to be rescued", default=500)
     parser.add_argument("--output_folder", required=True,
                         help="Path to the directory containing the generated problems")
 
     args = parser.parse_args()
     return args
 
 
 def generate_multiple_problems(
         min_boats: int, max_boats: int, min_people: int, max_people: int, max_dist_goal: int,
-        output_folder: Path) -> NoReturn:
+        output_folder: Path, total_number_problems: int = 100) -> NoReturn:
     """Generates multiple sailing planning problems.
 
     :param min_boats: the minimal number of boats in the problem.
     :param max_boats: the maximal number of boats in the problem.
     :param min_people: the minimal number of people in the problem.
     :param max_people: the maximal number of people in the problem.
     :param max_dist_goal: the maximal distance between the people and the goal.
     :param output_folder: the path to the directory containing the generated problems.
     :return:
     """
     boats_range = [i for i in range(min_boats, max_boats + 1)]
     people_range = [i for i in range(min_people, max_people + 1)]
-    for num_boats, num_people in itertools.product(boats_range, people_range):
-        with open(output_folder / f"pfile{num_boats}_{num_people}_{max_dist_goal}.pddl", "wt") as problem_file:
+    for i in range(total_number_problems):
+        num_boats = random.choice(boats_range)
+        num_people = random.choice(people_range)
+        with open(output_folder / f"pfile{i}.pddl", "wt") as problem_file:
             problem_file.write(
                 generate_instance(f"instance_{num_boats}_{num_people}", num_boats, num_people, max_dist_goal))
 
 
 def main():
     args = parse_arguments()
     generate_multiple_problems(args.min_boats, args.max_boats, args.min_people, args.max_people, args.max_dist_goal,
```

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser/problem_generators/zenotravel_generator.py` & `pddl-plus-parser-3.5.9/pddl_plus_parser/problem_generators/zenotravel_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser.egg-info/PKG-INFO` & `pddl-plus-parser-3.5.9/pddl_plus_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pddl-plus-parser
-Version: 3.5.8
+Version: 3.5.9
 Summary: Parser of PDDL+ domains and problems for learning purposes
 Author: Argaman Mordoch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pddl-plus-parser Version: 3.5.8 Summary: Parser of
+Metadata-Version: 2.1 Name: pddl-plus-parser Version: 3.5.9 Summary: Parser of
 PDDL+ domains and problems for learning purposes Author: Argaman Mordoch
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE
                         ************ PPDDDDLL PPlluuss PPaarrsseerr ************
   _[_P_y_P_I_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_][PyPI - Status][PyPI - Implementation][PyPI -
                                 Wheel]_[_G_i_t_H_u_b_]
                           [test][lint][docs]_[_c_o_d_e_c_o_v_]
```

### Comparing `pddl-plus-parser-3.5.8/pddl_plus_parser.egg-info/SOURCES.txt` & `pddl-plus-parser-3.5.9/pddl_plus_parser.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -46,20 +46,20 @@
 pddl_plus_parser/multi_agent/multi_agent_problem_converter.py
 pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py
 pddl_plus_parser/multi_agent/single_agent_plan_converter.py
 pddl_plus_parser/problem_generators/__init__.py
 pddl_plus_parser/problem_generators/common.py
 pddl_plus_parser/problem_generators/counters_generator.py
 pddl_plus_parser/problem_generators/depot_generator.py
-pddl_plus_parser/problem_generators/depots_generator.py
 pddl_plus_parser/problem_generators/driverlog_generator.py
 pddl_plus_parser/problem_generators/farmland_generator.py
 pddl_plus_parser/problem_generators/minecraft_generator.py
 pddl_plus_parser/problem_generators/plant_watering_generator.py
 pddl_plus_parser/problem_generators/sailing_generator.py
+pddl_plus_parser/problem_generators/satellite_generator.py
 pddl_plus_parser/problem_generators/settlers_problem_generator.py
 pddl_plus_parser/problem_generators/zenotravel_generator.py
 tests/exporters_tests/__init__.py
 tests/exporters_tests/consts.py
 tests/exporters_tests/numeric_trajectory_exporter_test.py
 tests/exporters_tests/problem_exporter_test.py
 tests/lisp_parsers_tests/__init__.py
```

### Comparing `pddl-plus-parser-3.5.8/tests/exporters_tests/consts.py` & `pddl-plus-parser-3.5.9/tests/exporters_tests/consts.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/exporters_tests/numeric_trajectory_exporter_test.py` & `pddl-plus-parser-3.5.9/tests/exporters_tests/numeric_trajectory_exporter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/exporters_tests/problem_exporter_test.py` & `pddl-plus-parser-3.5.9/tests/exporters_tests/problem_exporter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/lisp_parsers_tests/consts.py` & `pddl-plus-parser-3.5.9/tests/lisp_parsers_tests/consts.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/lisp_parsers_tests/domain_parser_test.py` & `pddl-plus-parser-3.5.9/tests/lisp_parsers_tests/domain_parser_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/lisp_parsers_tests/pddl_tokenizer_test.py` & `pddl-plus-parser-3.5.9/tests/lisp_parsers_tests/pddl_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/lisp_parsers_tests/problem_parser_test.py` & `pddl-plus-parser-3.5.9/tests/lisp_parsers_tests/problem_parser_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/lisp_parsers_tests/trajectory_parser_test.py` & `pddl-plus-parser-3.5.9/tests/lisp_parsers_tests/trajectory_parser_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/models_tests/consts.py` & `pddl-plus-parser-3.5.9/tests/models_tests/consts.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/models_tests/grounded_effect_test.py` & `pddl-plus-parser-3.5.9/tests/models_tests/grounded_effect_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/models_tests/grounded_precondition_test.py` & `pddl-plus-parser-3.5.9/tests/models_tests/grounded_precondition_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/models_tests/numeric_symbolic_operations_test.py` & `pddl-plus-parser-3.5.9/tests/models_tests/numeric_symbolic_operations_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/models_tests/numerical_expression_test.py` & `pddl-plus-parser-3.5.9/tests/models_tests/numerical_expression_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     root = construct_expression_tree(test_expression, TEST_DOMAIN_FUNCTIONS)
     tree = NumericalExpressionTree(root)
     pddl_str = tree.to_pddl()
     assert pddl_str == "(>= (capacity ?jug2) (amount ?jug2))"
 
 
 def test_to_pddl_does_not_break_effects_format():
-    original_expression = "(assign (fuel ?z) (* (capacity ?z) 9.0))"
+    original_expression = "(assign (fuel ?z) (* (capacity ?z) 9.00))"
     expression_tokenizer = PDDLTokenizer(pddl_str=original_expression)
     tokens = expression_tokenizer.parse()
     zeno_domain = DomainParser(domain_path=ZENO_DOMAIN_PATH).parse_domain()
     root = construct_expression_tree(tokens, zeno_domain.functions)
     tree = NumericalExpressionTree(root)
     assert tree.to_pddl() == original_expression
```

### Comparing `pddl-plus-parser-3.5.8/tests/models_tests/operator_test.py` & `pddl-plus-parser-3.5.9/tests/models_tests/operator_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/models_tests/pddl_function_test.py` & `pddl-plus-parser-3.5.9/tests/models_tests/pddl_function_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/models_tests/pddl_precondition_test.py` & `pddl-plus-parser-3.5.9/tests/models_tests/pddl_precondition_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/models_tests/pddl_state_test.py` & `pddl-plus-parser-3.5.9/tests/models_tests/pddl_state_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/multi_agent_tests/consts.py` & `pddl-plus-parser-3.5.9/tests/multi_agent_tests/consts.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/multi_agent_tests/multi_agent_domain_converter_test.py` & `pddl-plus-parser-3.5.9/tests/multi_agent_tests/multi_agent_domain_converter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/multi_agent_tests/multi_agent_problem_converter_test.py` & `pddl-plus-parser-3.5.9/tests/multi_agent_tests/multi_agent_problem_converter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py` & `pddl-plus-parser-3.5.9/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.5.8/tests/multi_agent_tests/single_agent_plan_converter_test.py` & `pddl-plus-parser-3.5.9/tests/multi_agent_tests/single_agent_plan_converter_test.py`

 * *Files identical despite different names*

