# Comparing `tmp/forloop_modules-1.1.1.tar.gz` & `tmp/forloop_modules-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forloop_modules-1.1.1.tar", last modified: Fri May 10 08:25:34 2024, max compression
+gzip compressed data, was "forloop_modules-1.1.2.tar", last modified: Thu May 16 23:27:30 2024, max compression
```

## Comparing `forloop_modules-1.1.1.tar` & `forloop_modules-1.1.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 08:25:34.374223 forloop_modules-1.1.1/
--rw-rw-rw-   0        0        0     1525 2024-02-22 17:34:45.000000 forloop_modules-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      658 2024-05-10 08:25:34.374223 forloop_modules-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-02-22 17:34:45.000000 forloop_modules-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 08:25:34.272640 forloop_modules-1.1.1/forloop_modules/
--rw-rw-rw-   0        0        0      179 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:25:34.277540 forloop_modules-1.1.1/forloop_modules/errors/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/errors/__init__.py
--rw-rw-rw-   0        0        0     1670 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/errors/errors.py
--rw-rw-rw-   0        0        0     9860 2024-03-12 11:46:28.000000 forloop_modules-1.1.1/forloop_modules/flog.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:25:34.344117 forloop_modules-1.1.1/forloop_modules/function_handlers/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/__init__.py
--rw-rw-rw-   0        0        0     6781 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/api_endpoint_handlers.py
--rw-rw-rw-   0        0        0    22200 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/api_handlers.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:25:34.349779 forloop_modules-1.1.1/forloop_modules/function_handlers/auxilliary/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/auxilliary/__init__.py
--rw-rw-rw-   0        0        0    17835 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py
--rw-rw-rw-   0        0        0      807 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py
--rw-rw-rw-   0        0        0     2061 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/auxilliary/data_types_validation.py
--rw-rw-rw-   0        0        0     1047 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/auxilliary/docs.py
--rw-rw-rw-   0        0        0     1940 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py
--rw-rw-rw-   0        0        0     7933 2024-05-03 13:07:28.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/auxilliary/form_dict_list.py
--rw-rw-rw-   0        0        0     2169 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py
--rw-rw-rw-   0        0        0    25173 2024-05-03 13:07:28.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/browser_handlers.py
--rw-rw-rw-   0        0        0   204411 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/cleaning_handlers.py
--rw-rw-rw-   0        0        0    12258 2024-03-21 12:02:54.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/control_flow_handlers.py
--rw-rw-rw-   0        0        0    46277 2024-03-21 12:02:54.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/data_handlers.py
--rw-rw-rw-   0        0        0    72995 2024-04-08 16:56:40.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/database_handlers.py
--rw-rw-rw-   0        0        0    30031 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/datetime_handlers.py
--rw-rw-rw-   0        0        0    14696 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/file_managment_handlers.py
--rw-rw-rw-   0        0        0    83412 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/integration_handlers.py
--rw-rw-rw-   0        0        0    27439 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/mapping_handlers.py
--rw-rw-rw-   0        0        0    14152 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/model_handlers.py
--rw-rw-rw-   0        0        0     2778 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/orchestration_handlers.py
--rw-rw-rw-   0        0        0    16250 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/rpa_handlers.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:25:34.352260 forloop_modules-1.1.1/forloop_modules/function_handlers/transformations/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/transformations/__init__.py
--rw-rw-rw-   0        0        0    14097 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/transformations/basic_transforms.py
--rw-rw-rw-   0        0        0    10448 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/transformations/imputation.py
--rw-rw-rw-   0        0        0     4092 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/transformations/outliers.py
--rw-rw-rw-   0        0        0    58900 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/variable_handlers.py
--rw-rw-rw-   0        0        0   103383 2024-05-03 13:07:28.000000 forloop_modules-1.1.1/forloop_modules/function_handlers/webscraping_handlers.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:25:34.358082 forloop_modules-1.1.1/forloop_modules/globals/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/globals/__init__.py
--rw-rw-rw-   0        0        0     5162 2024-05-03 13:07:28.000000 forloop_modules-1.1.1/forloop_modules/globals/active_entity_tracker.py
--rw-rw-rw-   0        0        0     1871 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/globals/database_utilities_handler.py
--rw-rw-rw-   0        0        0     7845 2024-05-10 08:24:41.000000 forloop_modules-1.1.1/forloop_modules/globals/db_connection.py
--rw-rw-rw-   0        0        0     8030 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/globals/dbtables_loader_popups.py
--rw-rw-rw-   0        0        0      223 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/globals/docs_categories.py
--rw-rw-rw-   0        0        0    19056 2024-05-03 13:07:28.000000 forloop_modules-1.1.1/forloop_modules/globals/local_variable_handler.py
--rw-rw-rw-   0        0        0    33335 2024-05-10 08:24:41.000000 forloop_modules-1.1.1/forloop_modules/globals/scraping_utilities_handler.py
--rw-rw-rw-   0        0        0     9133 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/globals/variable_handler.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:25:34.360335 forloop_modules-1.1.1/forloop_modules/integrations/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/integrations/__init__.py
--rw-rw-rw-   0        0        0     2082 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/integrations/slack_integration.py
--rw-rw-rw-   0        0        0     3580 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/integrations/testing_check_slack_notifications.py
--rw-rw-rw-   0        0        0    14244 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/node_detail_form.py
--rw-rw-rw-   0        0        0    10856 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/pipeline_function_handlers.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:25:34.363275 forloop_modules-1.1.1/forloop_modules/queries/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/queries/__init__.py
--rw-rw-rw-   0        0        0     2888 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/queries/context_request_backend_auxiliary_functions.py
--rw-rw-rw-   0        0        0    22040 2024-05-10 08:24:41.000000 forloop_modules-1.1.1/forloop_modules/queries/db_model_templates.py
--rw-rw-rw-   0        0        0    42399 2024-05-03 13:07:28.000000 forloop_modules-1.1.1/forloop_modules/queries/node_context_requests_backend.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:25:34.364307 forloop_modules-1.1.1/forloop_modules/redis/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/redis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:25:34.365560 forloop_modules-1.1.1/forloop_modules/redis/config/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/redis/config/__init__.py
--rw-rw-rw-   0        0        0     2108 2024-04-08 16:56:40.000000 forloop_modules-1.1.1/forloop_modules/redis/config/config.py
--rw-rw-rw-   0        0        0     6223 2024-04-08 16:56:40.000000 forloop_modules-1.1.1/forloop_modules/redis/redis_connection.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:25:34.372578 forloop_modules-1.1.1/forloop_modules/utils/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/utils/__init__.py
--rw-rw-rw-   0        0        0     5587 2024-04-08 16:56:40.000000 forloop_modules-1.1.1/forloop_modules/utils/definitions.py
--rw-rw-rw-   0        0        0     1024 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/utils/encryption.py
--rw-rw-rw-   0        0        0     3393 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/utils/pandas_operations.py
--rw-rw-rw-   0        0        0     3545 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/utils/pickle_serializer.py
--rw-rw-rw-   0        0        0     3190 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/utils/script_utils.py
--rw-rw-rw-   0        0        0     2021 2024-05-03 13:07:28.000000 forloop_modules-1.1.1/forloop_modules/utils/sse_parser.py
--rw-rw-rw-   0        0        0     1622 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/utils/str_helpers.py
--rw-rw-rw-   0        0        0      856 2024-04-08 16:56:40.000000 forloop_modules-1.1.1/forloop_modules/utils/synchronization_flags.py
--rw-rw-rw-   0        0        0     4570 2024-04-08 16:56:40.000000 forloop_modules-1.1.1/forloop_modules/utils/url_template_builder.py
--rw-rw-rw-   0        0        0     3558 2024-02-29 13:17:45.000000 forloop_modules-1.1.1/forloop_modules/utils/various.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:25:34.276554 forloop_modules-1.1.1/forloop_modules.egg-info/
--rw-rw-rw-   0        0        0      658 2024-05-10 08:25:34.000000 forloop_modules-1.1.1/forloop_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3529 2024-05-10 08:25:34.000000 forloop_modules-1.1.1/forloop_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 08:25:34.000000 forloop_modules-1.1.1/forloop_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-10 08:25:34.000000 forloop_modules-1.1.1/forloop_modules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 08:25:34.374223 forloop_modules-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      786 2024-05-10 08:19:29.000000 forloop_modules-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:25:34.373085 forloop_modules-1.1.1/tests/
--rw-rw-rw-   0        0        0        0 2024-02-22 17:34:45.000000 forloop_modules-1.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0     3316 2024-04-08 16:56:40.000000 forloop_modules-1.1.1/tests/test_url_template_builder.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:27:30.565792 forloop_modules-1.1.2/
+-rw-rw-rw-   0        0        0     1525 2024-02-22 17:34:45.000000 forloop_modules-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      658 2024-05-16 23:27:30.565792 forloop_modules-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2024-02-22 17:34:45.000000 forloop_modules-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 23:27:30.523685 forloop_modules-1.1.2/forloop_modules/
+-rw-rw-rw-   0        0        0      179 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:27:30.529685 forloop_modules-1.1.2/forloop_modules/errors/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/errors/__init__.py
+-rw-rw-rw-   0        0        0     1670 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/errors/errors.py
+-rw-rw-rw-   0        0        0     9860 2024-03-12 11:46:28.000000 forloop_modules-1.1.2/forloop_modules/flog.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:27:30.539691 forloop_modules-1.1.2/forloop_modules/function_handlers/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/__init__.py
+-rw-rw-rw-   0        0        0     6781 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/api_endpoint_handlers.py
+-rw-rw-rw-   0        0        0    22200 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/api_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:27:30.544692 forloop_modules-1.1.2/forloop_modules/function_handlers/auxilliary/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/auxilliary/__init__.py
+-rw-rw-rw-   0        0        0    17835 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py
+-rw-rw-rw-   0        0        0      807 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py
+-rw-rw-rw-   0        0        0     2061 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/auxilliary/data_types_validation.py
+-rw-rw-rw-   0        0        0     1047 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/auxilliary/docs.py
+-rw-rw-rw-   0        0        0     1940 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py
+-rw-rw-rw-   0        0        0     7933 2024-05-03 13:07:28.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/auxilliary/form_dict_list.py
+-rw-rw-rw-   0        0        0     2169 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py
+-rw-rw-rw-   0        0        0    25173 2024-05-03 13:07:28.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/browser_handlers.py
+-rw-rw-rw-   0        0        0   204411 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/cleaning_handlers.py
+-rw-rw-rw-   0        0        0    12333 2024-05-16 23:27:10.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/control_flow_handlers.py
+-rw-rw-rw-   0        0        0    46277 2024-03-21 12:02:54.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/data_handlers.py
+-rw-rw-rw-   0        0        0    72995 2024-04-08 16:56:40.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/database_handlers.py
+-rw-rw-rw-   0        0        0    30031 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/datetime_handlers.py
+-rw-rw-rw-   0        0        0    14696 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/file_managment_handlers.py
+-rw-rw-rw-   0        0        0    83412 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/integration_handlers.py
+-rw-rw-rw-   0        0        0    27439 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/mapping_handlers.py
+-rw-rw-rw-   0        0        0    14152 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/model_handlers.py
+-rw-rw-rw-   0        0        0     2778 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/orchestration_handlers.py
+-rw-rw-rw-   0        0        0    16250 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/rpa_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:27:30.546684 forloop_modules-1.1.2/forloop_modules/function_handlers/transformations/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/transformations/__init__.py
+-rw-rw-rw-   0        0        0    14097 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/transformations/basic_transforms.py
+-rw-rw-rw-   0        0        0    10448 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/transformations/imputation.py
+-rw-rw-rw-   0        0        0     4092 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/transformations/outliers.py
+-rw-rw-rw-   0        0        0    58900 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/variable_handlers.py
+-rw-rw-rw-   0        0        0   103383 2024-05-03 13:07:28.000000 forloop_modules-1.1.2/forloop_modules/function_handlers/webscraping_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:27:30.551684 forloop_modules-1.1.2/forloop_modules/globals/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/globals/__init__.py
+-rw-rw-rw-   0        0        0     5162 2024-05-03 13:07:28.000000 forloop_modules-1.1.2/forloop_modules/globals/active_entity_tracker.py
+-rw-rw-rw-   0        0        0     1871 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/globals/database_utilities_handler.py
+-rw-rw-rw-   0        0        0     7845 2024-05-10 08:26:16.000000 forloop_modules-1.1.2/forloop_modules/globals/db_connection.py
+-rw-rw-rw-   0        0        0     8030 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/globals/dbtables_loader_popups.py
+-rw-rw-rw-   0        0        0      223 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/globals/docs_categories.py
+-rw-rw-rw-   0        0        0    18806 2024-05-16 23:27:10.000000 forloop_modules-1.1.2/forloop_modules/globals/local_variable_handler.py
+-rw-rw-rw-   0        0        0    33335 2024-05-10 08:26:16.000000 forloop_modules-1.1.2/forloop_modules/globals/scraping_utilities_handler.py
+-rw-rw-rw-   0        0        0     9133 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/globals/variable_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:27:30.552684 forloop_modules-1.1.2/forloop_modules/integrations/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/integrations/__init__.py
+-rw-rw-rw-   0        0        0     2082 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/integrations/slack_integration.py
+-rw-rw-rw-   0        0        0     3580 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/integrations/testing_check_slack_notifications.py
+-rw-rw-rw-   0        0        0    14244 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/node_detail_form.py
+-rw-rw-rw-   0        0        0    10856 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/pipeline_function_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:27:30.555684 forloop_modules-1.1.2/forloop_modules/queries/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/queries/__init__.py
+-rw-rw-rw-   0        0        0     2888 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/queries/context_request_backend_auxiliary_functions.py
+-rw-rw-rw-   0        0        0    21803 2024-05-16 23:27:10.000000 forloop_modules-1.1.2/forloop_modules/queries/db_model_templates.py
+-rw-rw-rw-   0        0        0    42313 2024-05-16 23:27:10.000000 forloop_modules-1.1.2/forloop_modules/queries/node_context_requests_backend.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:27:30.556684 forloop_modules-1.1.2/forloop_modules/redis/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/redis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:27:30.557684 forloop_modules-1.1.2/forloop_modules/redis/config/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/redis/config/__init__.py
+-rw-rw-rw-   0        0        0     2070 2024-05-16 23:27:10.000000 forloop_modules-1.1.2/forloop_modules/redis/config/config.py
+-rw-rw-rw-   0        0        0     6573 2024-05-16 23:27:10.000000 forloop_modules-1.1.2/forloop_modules/redis/redis_connection.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:27:30.563684 forloop_modules-1.1.2/forloop_modules/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/utils/__init__.py
+-rw-rw-rw-   0        0        0     5587 2024-04-08 16:56:40.000000 forloop_modules-1.1.2/forloop_modules/utils/definitions.py
+-rw-rw-rw-   0        0        0     1024 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/utils/encryption.py
+-rw-rw-rw-   0        0        0     3393 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/utils/pandas_operations.py
+-rw-rw-rw-   0        0        0     3545 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/utils/pickle_serializer.py
+-rw-rw-rw-   0        0        0     3190 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/utils/script_utils.py
+-rw-rw-rw-   0        0        0     2021 2024-05-03 13:07:28.000000 forloop_modules-1.1.2/forloop_modules/utils/sse_parser.py
+-rw-rw-rw-   0        0        0     1622 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/utils/str_helpers.py
+-rw-rw-rw-   0        0        0      856 2024-04-08 16:56:40.000000 forloop_modules-1.1.2/forloop_modules/utils/synchronization_flags.py
+-rw-rw-rw-   0        0        0     4570 2024-04-08 16:56:40.000000 forloop_modules-1.1.2/forloop_modules/utils/url_template_builder.py
+-rw-rw-rw-   0        0        0     3558 2024-02-29 13:17:45.000000 forloop_modules-1.1.2/forloop_modules/utils/various.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:27:30.528685 forloop_modules-1.1.2/forloop_modules.egg-info/
+-rw-rw-rw-   0        0        0      658 2024-05-16 23:27:30.000000 forloop_modules-1.1.2/forloop_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3529 2024-05-16 23:27:30.000000 forloop_modules-1.1.2/forloop_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 23:27:30.000000 forloop_modules-1.1.2/forloop_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-16 23:27:30.000000 forloop_modules-1.1.2/forloop_modules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 23:27:30.565792 forloop_modules-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      786 2024-05-16 23:27:15.000000 forloop_modules-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:27:30.564684 forloop_modules-1.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-22 17:34:45.000000 forloop_modules-1.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     3316 2024-04-08 16:56:40.000000 forloop_modules-1.1.2/tests/test_url_template_builder.py
```

### Comparing `forloop_modules-1.1.1/LICENSE` & `forloop_modules-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/PKG-INFO` & `forloop_modules-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forloop_modules
-Version: 1.1.1
+Version: 1.1.2
 Summary: This package contains open source modules and integrations within Forloop.ai platform
 Home-page: https://github.com/ForloopAI/forloop_modules
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forloop_modules-1.1.1/forloop_modules/errors/errors.py` & `forloop_modules-1.1.2/forloop_modules/errors/errors.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/flog.py` & `forloop_modules-1.1.2/forloop_modules/flog.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/api_endpoint_handlers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/api_endpoint_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/api_handlers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/api_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/auxilliary/abstract_function_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/auxilliary/auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/auxilliary/data_types_validation.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/auxilliary/data_types_validation.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/auxilliary/docs.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/auxilliary/docs.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/auxilliary/forloop_code_eval.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/auxilliary/form_dict_list.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/auxilliary/form_dict_list.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/auxilliary/node_type_categories_manager.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/browser_handlers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/browser_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/cleaning_handlers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/cleaning_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/control_flow_handlers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/control_flow_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 
     def make_form_dict_list(self, *args, node_detail_form=None):
         
         fdl=FormDictList(docs=self.docs)
         fdl.label(self.fn_name)
         return fdl
 
+    def execute(self, node_detail_form):
+        self.direct_execute()
+
     def direct_execute(self):
         """Do nothing"""
         pass
 
     def export_code(self, node_detail_form):
         code = """
         #start pipeline
```

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/data_handlers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/data_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/database_handlers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/database_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/datetime_handlers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/datetime_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/file_managment_handlers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/file_managment_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/integration_handlers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/integration_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/mapping_handlers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/mapping_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/model_handlers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/model_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/orchestration_handlers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/orchestration_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/rpa_handlers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/rpa_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/transformations/basic_transforms.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/transformations/basic_transforms.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/transformations/imputation.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/transformations/imputation.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/transformations/outliers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/transformations/outliers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/variable_handlers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/variable_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/function_handlers/webscraping_handlers.py` & `forloop_modules-1.1.2/forloop_modules/function_handlers/webscraping_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/globals/active_entity_tracker.py` & `forloop_modules-1.1.2/forloop_modules/globals/active_entity_tracker.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/globals/database_utilities_handler.py` & `forloop_modules-1.1.2/forloop_modules/globals/database_utilities_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/globals/db_connection.py` & `forloop_modules-1.1.2/forloop_modules/globals/db_connection.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/globals/dbtables_loader_popups.py` & `forloop_modules-1.1.2/forloop_modules/globals/dbtables_loader_popups.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/globals/local_variable_handler.py` & `forloop_modules-1.1.2/forloop_modules/globals/local_variable_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 #from src.df_column_category_predictor import classify_df_column_categories, DataFrameColumnCategoryAnalysis
 
 from forloop_modules.redis.config.config import redis_config
 from forloop_modules.utils.pickle_serializer import save_data_dict_to_pickle_folder
 from forloop_modules.utils.pickle_serializer import load_data_dict_from_pickle_folder
 from forloop_modules.globals.active_entity_tracker import aet
-from forloop_modules.redis.redis_connection import kv_redis
+from forloop_modules.redis.redis_connection import kv_redis, get_variable_redis_name, get_initial_variable_redis_name
 from forloop_modules.utils.definitions import JSON_SERIALIZABLE_TYPES, JSON_SERIALIZABLE_TYPES_AS_STRINGS, REDIS_STORED_TYPES, REDIS_STORED_TYPES_AS_STRINGS
 from forloop_modules.utils.various import is_value_serializable, is_value_redis_compatible
 #import src.forloop_code_eval as fce
 import forloop_modules.queries.node_context_requests_backend as ncrb
 
 @dataclass
 class File:
@@ -58,17 +58,17 @@
         self.variables={}
         self.variable_uid_variable_dict={} #ANALOGY of dicts in GLC, new implementation - contains nodes in API -> reflecting status of server nodes via API
 
         self._handler_mode: Literal["initial_variable", "variable"] = "initial_variable"
 
     def get_variable_redis_name(self, name: str) -> str:
         if self.handler_mode == "initial_variable":
-            return redis_config.INITIAL_VARIABLE_KEY + name
+            return get_initial_variable_redis_name(name, aet.active_pipeline_uid)
         elif self.handler_mode == "variable":
-            return redis_config.VARIABLE_KEY + name
+            return get_variable_redis_name(name, aet.active_pipeline_job_uid)
         else:
             raise ValueError(f"Variable mode {self.handler_mode} is not supported.")
 
     @property
     def is_empty(self):
         return len(self.variables) == 0
 
@@ -117,15 +117,15 @@
 
         #serialization for objects
         if local_variable.typ in REDIS_STORED_TYPES_AS_STRINGS:
             value = kv_redis.get(self.get_variable_redis_name(name))
             value.attrs["name"] = local_variable.name
 
             variable = self.get_variable_by_name(name)
-            local_variable = LocalVariable(variable["uid"], variable["name"], value, variable["is_result"])  # TODO: Remove when PrototypeJobs are implemented
+            local_variable = LocalVariable(variable["uid"], variable["name"], value, variable["is_result"])
             return local_variable
         else:
             return local_variable
 
     def get_int_to_str_col_name_mapping(self, df: pd.DataFrame) -> dict[int, str]:
         """
         find columns whose name type is int and create mapping between their int name and its string form
@@ -196,48 +196,47 @@
             additional_params = {}
 
         if self.handler_mode == "initial_variable":
             ncrb_fn = ncrb.new_initial_variable
         elif self.handler_mode == "variable":
             ncrb_fn = ncrb.new_variable
 
+        optional_args = {"is_result": is_result} if is_result is not None else {}
         #serialization for objects
         # TODO: FFS FIXME:
         if is_value_serializable(value):
-            response = ncrb_fn(name=name, value=value)
+            response = ncrb_fn(name=name, value=value, **optional_args)
         else:
             if is_value_redis_compatible(value):
                 kv_redis.set(self.get_variable_redis_name(name), value, additional_params)
             else:
                 data_dict={}
                 data_dict[name]=value
                 folder=".//file_transfer"
                 save_data_dict_to_pickle_folder(data_dict,folder,clean_existing_folder=False)
             #TODO: FILE TRANSFER MISSING
 
-            optional_args = {"is_result": is_result} if is_result is not None else {}
             response = ncrb_fn(name=name, value="", type=type(value).__name__, **optional_args)
 
         result = response.json()
         self.create_local_variable(
-            result["uid"], result["name"], result["value"], result["is_result"],
-            result["type"]
-        )  # TODO: Remove when PrototypeJobs are implemented
+            result["uid"], result["name"], result["value"], result["is_result"], result["type"]
+        )
         return result
 
-    def create_local_variable(self, uid: str, name, value, is_result: bool, type=None):  # TODO: Change when PrototypeJobs are implemented
+    def create_local_variable(self, uid: str, name, value, is_result: bool, type=None):
         if type in JSON_SERIALIZABLE_TYPES_AS_STRINGS and type != "str":
             value=ast.literal_eval(str(value))
         elif type in REDIS_STORED_TYPES_AS_STRINGS:
             value = kv_redis.get(self.get_variable_redis_name(name))
 
             if isinstance(value, pd.DataFrame):
                 value = self.process_dataframe_variable_on_initialization(name, value)
 
-        variable=LocalVariable(uid, name, value, is_result) # TODO: Remove when PrototypeJobs are implemented
+        variable=LocalVariable(uid, name, value, is_result)
         self.variables[name]=variable
         return(variable)
 
     def update_variable(self, name, value, is_result: Optional[bool] = None, additional_params: dict = None, project_uid=None):
         if additional_params is None:
             additional_params = {}
 
@@ -254,15 +253,15 @@
 
         if variable is not None:
             is_result = is_result if is_result is not None else variable["is_result"]
             ncrb_fn_kwargs = {
                 "variable_uid": variable["uid"],
                 "name": name,
                 "value": value,
-                "is_result": is_result  # TODO: Remove when PrototypeJobs are implemented
+                "is_result": is_result
             }
 
             if is_value_serializable(value):
                 response = ncrb_update_by_uid_fn(**ncrb_fn_kwargs)
             else:
                 ncrb_fn_kwargs.update(value="")
 
@@ -274,15 +273,15 @@
                     folder=".//file_transfer"
                     save_data_dict_to_pickle_folder(data_dict,folder,clean_existing_folder=False)
                 response = ncrb_update_by_uid_fn(type=type(value).__name__, **ncrb_fn_kwargs)
 
             result = response.json()
             self.update_local_variable(
                 result["name"], result["value"], result["is_result"], result["type"]
-            )  # TODO: Remove when PrototypeJobs are implemented
+            )
             return result
 
 
         #else:
         #    self.variables.pop(name)
         #    self.create_variable(name, value)
 
@@ -294,15 +293,15 @@
         if type in JSON_SERIALIZABLE_TYPES_AS_STRINGS and type != "str":
             value=ast.literal_eval(str(value))
         elif type in REDIS_STORED_TYPES_AS_STRINGS:
             value = kv_redis.get(self.get_variable_redis_name(name))
 
         variable=self.variables[name]
         self.variables[name].value=value #Update
-        self.variables[name].is_result = is_result  # TODO: Remove when PrototypeJobs are implemented
+        self.variables[name].is_result = is_result
 
         return(variable)
 
     def delete_variable(self, var_name: str):
         if self.last_active_df_variable is not None and var_name == self.last_active_df_variable.name:
             self.last_active_df_variable = None
```

### Comparing `forloop_modules-1.1.1/forloop_modules/globals/scraping_utilities_handler.py` & `forloop_modules-1.1.2/forloop_modules/globals/scraping_utilities_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/globals/variable_handler.py` & `forloop_modules-1.1.2/forloop_modules/globals/variable_handler.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/integrations/slack_integration.py` & `forloop_modules-1.1.2/forloop_modules/integrations/slack_integration.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/integrations/testing_check_slack_notifications.py` & `forloop_modules-1.1.2/forloop_modules/integrations/testing_check_slack_notifications.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/node_detail_form.py` & `forloop_modules-1.1.2/forloop_modules/node_detail_form.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/pipeline_function_handlers.py` & `forloop_modules-1.1.2/forloop_modules/pipeline_function_handlers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/queries/context_request_backend_auxiliary_functions.py` & `forloop_modules-1.1.2/forloop_modules/queries/context_request_backend_auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/queries/db_model_templates.py` & `forloop_modules-1.1.2/forloop_modules/queries/db_model_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,16 +152,15 @@
 
 class APINodeJob(BaseModel):
     uid: str
     status: JobStatusEnum
     created_at: UTCDatetime
     completed_at: Optional[UTCDatetime] = None
     message: Optional[str] = None
-    pipeline_uid: str  # TODO: Remove when PrototypeJobs are implemented
-    pipeline_job_uid: Optional[str] = None # TODO: Change to required when PrototypeJobs are implemented
+    pipeline_uid: str
 
 
 class APIOperationJob(BaseModel):
     uid: str
     status: JobStatusEnum
     created_at: UTCDatetime
     completed_at: Optional[UTCDatetime] = None
@@ -395,15 +394,14 @@
 class VariableModel(BaseModel):
     uid: str = "0"
     name: str = ""
     value: Any = "" # strings, bytes, numbers, tuples, lists, dicts, sets, booleans, and None (anything evaluatable by ast.literal_eval)
     type: Optional[str] = None # Type can be enforced or autoinferred
     size: Optional[int] = None
     is_result: bool = False
-    pipeline_uid: str = "0"
     project_uid: str = "0" # TODO: Is this necessary? Node is indirectly linked to a project via pipeline
     pipeline_job_uid: str = "0"
 
     @field_validator("name", "value")
     @classmethod
     def check_for_single_quote_mark(cls, value: str) -> str:
         """
@@ -429,15 +427,15 @@
     uid : Any = Field(None, exclude=True, alias="_do_not_send_in_request")
 
 
 class InitialVariableModel(BaseModel):
     uid: str = "0"
     name: str = ""
     value: Any = "" # strings, bytes, numbers, tuples, lists, dicts, sets, booleans, and None (anything evaluatable by ast.literal_eval)
-    is_result: bool = False  # TODO: Remove when PrototypeJobs are implemented
+    is_result: bool = False
     type: Optional[str] = None # Type can be enforced or autoinferred
     size: Optional[int] = None
     pipeline_uid: str = "0"
     project_uid: str = "0" # TODO: Is this necessary? Node is indirectly linked to a project via pipeline
 
     @field_validator("name", "value")
     @classmethod
```

### Comparing `forloop_modules-1.1.1/forloop_modules/queries/node_context_requests_backend.py` & `forloop_modules-1.1.2/forloop_modules/queries/node_context_requests_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -541,16 +541,16 @@
 #     response = requests.post(url, json=payload)
 #     flog.info(f'New Variable response: {response.text}')
 #
 #     return response
 
 
 def get_variable_by_name(variable_name: str):
-    pipeline_uid = aet.active_pipeline_uid
-    url = f'{BASE_API}/variables?name={variable_name}&pipeline_uid={pipeline_uid}'
+    pipeline_job_uid = aet.active_pipeline_job_uid
+    url = f'{BASE_API}/variables?name={variable_name}&pipeline_job_uid={pipeline_job_uid}'
 
     response = requests.get(url)
     response.raise_for_status()
     flog.info(f'GET Variable by name response: {response.text}')
 
     return response
 
@@ -676,28 +676,28 @@
     pipeline_uid = aet.active_pipeline_uid
     response = requests.delete(f'{BASE_API}/pipelines/{pipeline_uid}/initial_variables')
     response.raise_for_status()
     return response
 
 
 def update_initial_variable_by_uid(
-    variable_uid: str, name: str, value: Any, is_result: bool, type=None, size: Optional[int] = None  # TODO: Remove when PrototypeJobs are implemented
+    variable_uid: str, name: str, value: Any, is_result: bool, type=None, size: Optional[int] = None
 ):
     project_uid = aet.project_uid
     pipeline_uid = aet.active_pipeline_uid
     pipeline_job_uid = aet.active_pipeline_job_uid
 
     if type is None:
         for std_type in [str, int, list, dict, float, bool]:
             if isinstance(value, std_type):
                 type = std_type.__name__
 
     payload = {
         "name": name, "value": value, "type": type, "size": size, "project_uid": project_uid,
-        "pipeline_uid": pipeline_uid, "pipeline_job_uid": pipeline_job_uid, "is_result": is_result  # TODO: Remove when PrototypeJobs are implemented
+        "pipeline_uid": pipeline_uid, "pipeline_job_uid": pipeline_job_uid, "is_result": is_result
     }
     response = requests.put(f"{BASE_API}/initial_variables/{variable_uid}", json=payload)
     response.raise_for_status()
     return response
 
 
 ############# Dbtables ###############
```

### Comparing `forloop_modules-1.1.1/forloop_modules/redis/config/config.py` & `forloop_modules-1.1.2/forloop_modules/redis/config/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 class RedisConfig(BaseSettings):
     class Config:
         env_file = '.env'
         env_file_encoding = 'utf-8'
 
     # None values for Host and Password are correct options:
     # in-memory local caching will be used instead of a Redis server
-    FORLOOP_REDIS_HOST: Optional[str] = None # "localhost" #localhost doesn't work for devs with DummyKVRedis
+    FORLOOP_REDIS_HOST: Optional[str] = 'localhost' # localhost doesn't work for devs with DummyKVRedis
     FORLOOP_REDIS_USERNAME: str = "default"
     FORLOOP_REDIS_PASSWORD: Optional[str] = None
     FORLOOP_REDIS_PORT: int = 6379
     FORLOOP_REDIS_DB: int = 0
 
-    VARIABLE_KEY: str = "stored_variable_"  # key prefix to be concatenated with variable name
-    INITIAL_VARIABLE_KEY: str = "stored_initial_variable_"  # key prefix to be concatenated with variable name
+    VARIABLE_KEY: str = "pipeline_job:{pipeline_job_uid}:variable:{variable_name}"
+    INITIAL_VARIABLE_KEY: str = "pipeline:{pipeline_uid}:initial_variable:{variable_name}"
 
     JOB_KEY: str = "jobs"
     JOB_INDEX_NAME: str = "index"
     JOB_LOCK_NAME: str = "jobs:lock"
     JOB_PRIMARY_KEY: str = "jobs:pk"
     
     LAST_ACTIVE_DF_NODE_UID_KEY_TEMPLATE: str = "project:{project_uid}:last_active_df_node_uid"
```

### Comparing `forloop_modules-1.1.1/forloop_modules/redis/redis_connection.py` & `forloop_modules-1.1.2/forloop_modules/redis/redis_connection.py`

 * *Files 16% similar despite different names*

```diff
@@ -129,7 +129,13 @@
     #         f"Discrepancy between '{redis_config.JOB_KEY}:{redis_config.JOB_INDEX_NAME}' initialization and validation rules. Could not initialize"
     #     )
 
 def create_redis_key_for_project_db_private_key(project_uid: str):
     redis_key = redis_config.PASSWORD_ENCRYPTION_KEY_TEMPLATE.format(project_uid=project_uid)
     
     return redis_key
+
+def get_variable_redis_name(name: str, pipeline_job_uid: str) -> str:
+    return redis_config.VARIABLE_KEY.format(pipeline_job_uid=pipeline_job_uid, variable_name=name)
+
+def get_initial_variable_redis_name(name: str, pipeline_uid: str) -> str:
+    return redis_config.INITIAL_VARIABLE_KEY.format(pipeline_uid=pipeline_uid, variable_name=name)
```

### Comparing `forloop_modules-1.1.1/forloop_modules/utils/definitions.py` & `forloop_modules-1.1.2/forloop_modules/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/utils/encryption.py` & `forloop_modules-1.1.2/forloop_modules/utils/encryption.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/utils/pandas_operations.py` & `forloop_modules-1.1.2/forloop_modules/utils/pandas_operations.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/utils/pickle_serializer.py` & `forloop_modules-1.1.2/forloop_modules/utils/pickle_serializer.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/utils/script_utils.py` & `forloop_modules-1.1.2/forloop_modules/utils/script_utils.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/utils/sse_parser.py` & `forloop_modules-1.1.2/forloop_modules/utils/sse_parser.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/utils/str_helpers.py` & `forloop_modules-1.1.2/forloop_modules/utils/str_helpers.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/utils/synchronization_flags.py` & `forloop_modules-1.1.2/forloop_modules/utils/synchronization_flags.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/utils/url_template_builder.py` & `forloop_modules-1.1.2/forloop_modules/utils/url_template_builder.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules/utils/various.py` & `forloop_modules-1.1.2/forloop_modules/utils/various.py`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/forloop_modules.egg-info/PKG-INFO` & `forloop_modules-1.1.2/forloop_modules.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forloop-modules
-Version: 1.1.1
+Version: 1.1.2
 Summary: This package contains open source modules and integrations within Forloop.ai platform
 Home-page: https://github.com/ForloopAI/forloop_modules
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forloop_modules-1.1.1/forloop_modules.egg-info/SOURCES.txt` & `forloop_modules-1.1.2/forloop_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forloop_modules-1.1.1/setup.py` & `forloop_modules-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='forloop_modules',
-    version='1.1.1',
+    version='1.1.2',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='This package contains open source modules and integrations within Forloop.ai platform',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ForloopAI/forloop_modules',
     packages=setuptools.find_packages(),
```

### Comparing `forloop_modules-1.1.1/tests/test_url_template_builder.py` & `forloop_modules-1.1.2/tests/test_url_template_builder.py`

 * *Files identical despite different names*

