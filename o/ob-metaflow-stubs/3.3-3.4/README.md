# Comparing `tmp/ob-metaflow-stubs-3.3.tar.gz` & `tmp/ob-metaflow-stubs-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ob-metaflow-stubs-3.3.tar", last modified: Mon May 13 17:42:15 2024, max compression
+gzip compressed data, was "ob-metaflow-stubs-3.4.tar", last modified: Fri May 17 19:44:45 2024, max compression
```

## Comparing `ob-metaflow-stubs-3.3.tar` & `ob-metaflow-stubs-3.4.tar`

### file list

```diff
@@ -1,166 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.075098 ob-metaflow-stubs-3.3/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 17:41:58.000000 ob-metaflow-stubs-3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-13 17:42:15.075098 ob-metaflow-stubs-3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-13 17:41:58.000000 ob-metaflow-stubs-3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.055098 ob-metaflow-stubs-3.3/metaflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)   107671 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/cli.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.059098 ob-metaflow-stubs-3.3/metaflow-stubs/client/
--rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/client/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/client/filecache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/clone_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/flowspec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/generated_for.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/includefile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.059098 ob-metaflow-stubs-3.3/metaflow-stubs/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/metadata/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/metadata/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/metaflow_config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/metaflow_current.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.059098 ob-metaflow-stubs-3.3/metaflow-stubs/mflog/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/mflog/mflog.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/multicore_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/parameters.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.059098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.063098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/airflow.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/airflow_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/airflow_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/exception.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.063098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.063098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_workflows.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.063098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/aws_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/aws_utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.063098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/batch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/batch_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.063098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.067098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.067098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/azure_credential.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/azure_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/azure_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.067098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_creator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_datastore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.067098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/basic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/card.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.071098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/components.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_resolver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/component_serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/catch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.071098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/local.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.071098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/s3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/s3util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/debug_logger.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/debug_monitor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/environment_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/events_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.071098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/frameworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/frameworks/pytorch.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.071098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/gs_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.071098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/package_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/parallel_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/perimeters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/project_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.075098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/conda_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/conda_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/pypi_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/resources_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/retry_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.075098 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/secrets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/storage_executor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/tag_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/plugins/timeout_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/procpoll.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.075098 ob-metaflow-stubs-3.3/metaflow-stubs/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/profilers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/pylint_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/metaflow-stubs/tagging_util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:42:15.075098 ob-metaflow-stubs-3.3/ob_metaflow_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/ob_metaflow_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-13 17:42:15.000000 ob-metaflow-stubs-3.3/ob_metaflow_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/ob_metaflow_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 17:42:14.000000 ob-metaflow-stubs-3.3/ob_metaflow_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:42:15.075098 ob-metaflow-stubs-3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-13 17:41:58.000000 ob-metaflow-stubs-3.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-13 17:41:58.000000 ob-metaflow-stubs-3.3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.580221 ob-metaflow-stubs-3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-17 19:44:28.000000 ob-metaflow-stubs-3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-17 19:44:45.580221 ob-metaflow-stubs-3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-17 19:44:28.000000 ob-metaflow-stubs-3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.560221 ob-metaflow-stubs-3.4/metaflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)   107671 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/cli.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.560221 ob-metaflow-stubs-3.4/metaflow-stubs/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/client/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/client/filecache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/clone_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/flowspec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/generated_for.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/includefile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.560221 ob-metaflow-stubs-3.4/metaflow-stubs/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/metadata/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/metadata/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/metaflow_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/metaflow_current.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.560221 ob-metaflow-stubs-3.4/metaflow-stubs/mflog/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/mflog/mflog.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/multicore_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/parameters.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.564221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.564221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/airflow.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/airflow_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/airflow_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/exception.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.564221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.568221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_workflows.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.568221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/aws_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/aws_utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.568221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/batch_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.568221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.568221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.572221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/azure_credential.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/azure_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/azure_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.572221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_creator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_datastore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.572221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/basic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/card.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.572221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/components.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_resolver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/component_serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/catch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.576221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/local.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.576221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/s3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/s3util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/debug_logger.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/debug_monitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/environment_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/events_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.576221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/frameworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/frameworks/pytorch.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.576221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/gs_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.576221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/logs_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/package_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/parallel_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/perimeters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/project_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.576221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/conda_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/conda_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/pypi_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/resources_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/retry_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.580221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/secrets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/storage_executor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/tag_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/timeout_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/procpoll.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.580221 ob-metaflow-stubs-3.4/metaflow-stubs/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/profilers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/pylint_wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/tagging_util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.580221 ob-metaflow-stubs-3.4/ob_metaflow_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-17 19:44:45.000000 ob-metaflow-stubs-3.4/ob_metaflow_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-05-17 19:44:45.000000 ob-metaflow-stubs-3.4/ob_metaflow_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:44:45.000000 ob-metaflow-stubs-3.4/ob_metaflow_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 19:44:45.000000 ob-metaflow-stubs-3.4/ob_metaflow_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:44:45.580221 ob-metaflow-stubs-3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-17 19:44:28.000000 ob-metaflow-stubs-3.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-17 19:44:28.000000 ob-metaflow-stubs-3.4/version.py
```

### Comparing `ob-metaflow-stubs-3.3/PKG-INFO` & `ob-metaflow-stubs-3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-metaflow-stubs
-Version: 3.3
+Version: 3.4
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/__init__.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.215304                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.623630                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
     import datetime
-    import metaflow._vendor.click.types
+    import io
+    import metaflow.events
     import metaflow.parameters
+    import typing
+    import metaflow.metaflow_current
     import metaflow.client.core
+    import metaflow._vendor.click.types
     import metaflow.plugins.datatools.s3.s3
-    import metaflow.metaflow_current
-    import metaflow.events
     import metaflow.datastore.inputs
-    import io
 FlowSpecDerived = typing.TypeVar("FlowSpecDerived", bound="FlowSpec", contravariant=False, covariant=False)
 StepFlag = typing.NewType("StepFlag", bool)
 
 CURRENT_DIRECTORY: str
 
 INFO_FILE: str
 
@@ -722,163 +722,126 @@
     -------
     Union[Callable[[FlowSpecDerived, StepFlag], None], Callable[[FlowSpecDerived, Any, StepFlag], None]]
         Function that is a Metaflow Step
     """
     ...
 
 @typing.overload
-def catch(*, var: typing.Optional[str] = None, print_exception: bool = True) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies that the step will success under all circumstances.
-    
-    The decorator will create an optional artifact, specified by `var`, which
-    contains the exception raised. You can use it to detect the presence
-    of errors, indicating that all happy-path artifacts produced by the step
-    are missing.
-    
-    Parameters
-    ----------
-    var : str, optional, default None
-        Name of the artifact in which to store the caught exception.
-        If not specified, the exception is not stored.
-    print_exception : bool, default True
-        Determines whether or not the exception is printed to
-        stdout when caught.
-    """
-    ...
-
-@typing.overload
-def catch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def catch(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def catch(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, var: typing.Optional[str] = None, print_exception: bool = True):
-    """
-    Specifies that the step will success under all circumstances.
-    
-    The decorator will create an optional artifact, specified by `var`, which
-    contains the exception raised. You can use it to detect the presence
-    of errors, indicating that all happy-path artifacts produced by the step
-    are missing.
-    
-    Parameters
-    ----------
-    var : str, optional, default None
-        Name of the artifact in which to store the caught exception.
-        If not specified, the exception is not stored.
-    print_exception : bool, default True
-        Determines whether or not the exception is printed to
-        stdout when caught.
-    """
-    ...
-
-@typing.overload
-def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def conda(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Creates a human-readable report, a Metaflow Card, after this step completes.
+    Specifies the Conda environment for the step.
     
-    Note that you may add multiple `@card` decorators in a step with different parameters.
+    Information in this decorator will augment any
+    attributes set in the `@conda_base` flow-level decorator. Hence,
+    you can use `@conda_base` to set packages required by all
+    steps and use `@conda` to specify step-specific overrides.
     
     Parameters
     ----------
-    type : str, default 'default'
-        Card type.
-    id : str, optional, default None
-        If multiple cards are present, use this id to identify this card.
-    options : Dict[str, Any], default {}
-        Options passed to the card. The contents depend on the card type.
-    timeout : int, default 45
-        Interrupt reporting if it takes more than this many seconds.
-    
-    
+    packages : Dict[str, str], default {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables @conda.
     """
     ...
 
 @typing.overload
-def card(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def conda(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def card(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def card(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45):
-    """
-    Creates a human-readable report, a Metaflow Card, after this step completes.
-    
-    Note that you may add multiple `@card` decorators in a step with different parameters.
-    
-    Parameters
-    ----------
-    type : str, default 'default'
-        Card type.
-    id : str, optional, default None
-        If multiple cards are present, use this id to identify this card.
-    options : Dict[str, Any], default {}
-        Options passed to the card. The contents depend on the card type.
-    timeout : int, default 45
-        Interrupt reporting if it takes more than this many seconds.
-    
-    
-    """
+def conda(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-@typing.overload
-def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def conda(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
     """
-    Specifies the number of times the task corresponding
-    to a step needs to be retried.
-    
-    This decorator is useful for handling transient errors, such as networking issues.
-    If your task contains operations that can't be retried safely, e.g. database updates,
-    it is advisable to annotate it with `@retry(times=0)`.
+    Specifies the Conda environment for the step.
     
-    This can be used in conjunction with the `@catch` decorator. The `@catch`
-    decorator will execute a no-op task after all retries have been exhausted,
-    ensuring that the flow execution can continue.
+    Information in this decorator will augment any
+    attributes set in the `@conda_base` flow-level decorator. Hence,
+    you can use `@conda_base` to set packages required by all
+    steps and use `@conda` to specify step-specific overrides.
     
     Parameters
     ----------
-    times : int, default 3
-        Number of times to retry this task.
-    minutes_between_retries : int, default 2
-        Number of minutes between retries.
+    packages : Dict[str, str], default {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables @conda.
     """
     ...
 
-@typing.overload
-def retry(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def retry(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def retry(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, times: int = 3, minutes_between_retries: int = 2):
+def kubernetes(*, cpu: int = 1, memory: int = 4096, disk: int = 10240, image: typing.Optional[str] = None, image_pull_policy: str = "KUBERNETES_IMAGE_PULL_POLICY", service_account: str = "METAFLOW_KUBERNETES_SERVICE_ACCOUNT", secrets: typing.Optional[typing.List[str]] = None, namespace: str = "METAFLOW_KUBERNETES_NAMESPACE", gpu: typing.Optional[int] = None, gpu_vendor: str = "KUBERNETES_GPU_VENDOR", tolerations: typing.List[str] = [], use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = "/metaflow_temp", persistent_volume_claims: typing.Optional[typing.Dict[str, str]] = None, shared_memory: typing.Optional[int] = None, port: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the number of times the task corresponding
-    to a step needs to be retried.
-    
-    This decorator is useful for handling transient errors, such as networking issues.
-    If your task contains operations that can't be retried safely, e.g. database updates,
-    it is advisable to annotate it with `@retry(times=0)`.
-    
-    This can be used in conjunction with the `@catch` decorator. The `@catch`
-    decorator will execute a no-op task after all retries have been exhausted,
-    ensuring that the flow execution can continue.
+    Specifies that this step should execute on Kubernetes.
     
     Parameters
     ----------
-    times : int, default 3
-        Number of times to retry this task.
-    minutes_between_retries : int, default 2
-        Number of minutes between retries.
+    cpu : int, default 1
+        Number of CPUs required for this step. If `@resources` is
+        also present, the maximum value from all decorators is used.
+    memory : int, default 4096
+        Memory size (in MB) required for this step. If
+        `@resources` is also present, the maximum value from all decorators is
+        used.
+    disk : int, default 10240
+        Disk size (in MB) required for this step. If
+        `@resources` is also present, the maximum value from all decorators is
+        used.
+    image : str, optional, default None
+        Docker image to use when launching on Kubernetes. If not specified, and
+        METAFLOW_KUBERNETES_CONTAINER_IMAGE is specified, that image is used. If
+        not, a default Docker image mapping to the current version of Python is used.
+    image_pull_policy: str, default KUBERNETES_IMAGE_PULL_POLICY
+        If given, the imagePullPolicy to be applied to the Docker image of the step.
+    service_account : str, default METAFLOW_KUBERNETES_SERVICE_ACCOUNT
+        Kubernetes service account to use when launching pod in Kubernetes.
+    secrets : List[str], optional, default None
+        Kubernetes secrets to use when launching pod in Kubernetes. These
+        secrets are in addition to the ones defined in `METAFLOW_KUBERNETES_SECRETS`
+        in Metaflow configuration.
+    namespace : str, default METAFLOW_KUBERNETES_NAMESPACE
+        Kubernetes namespace to use when launching pod in Kubernetes.
+    gpu : int, optional, default None
+        Number of GPUs required for this step. A value of zero implies that
+        the scheduled node should not have GPUs.
+    gpu_vendor : str, default KUBERNETES_GPU_VENDOR
+        The vendor of the GPUs to be used for this step.
+    tolerations : List[str], default []
+        The default is extracted from METAFLOW_KUBERNETES_TOLERATIONS.
+        Kubernetes tolerations to use when launching pod in Kubernetes.
+    use_tmpfs : bool, default False
+        This enables an explicit tmpfs mount for this step.
+    tmpfs_tempdir : bool, default True
+        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
+    tmpfs_size : int, optional, default: None
+        The value for the size (in MiB) of the tmpfs mount for this step.
+        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
+        memory allocated for this step.
+    tmpfs_path : str, optional, default /metaflow_temp
+        Path to tmpfs mount for this step.
+    persistent_volume_claims : Dict[str, str], optional, default None
+        A map (dictionary) of persistent volumes to be mounted to the pod for this step. The map is from persistent
+        volumes to the path to which the volume is to be mounted, e.g., `{'pvc-name': '/path/to/mount/on'}`.
+    shared_memory: int, optional
+        Shared memory size (in MiB) required for this step
+    port: int, optional
+        Port number to specify in the Kubernetes job object
     """
     ...
 
 @typing.overload
 def resources(*, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies the resources needed when executing this step.
@@ -952,118 +915,206 @@
     shared_memory : int, optional, default None
         The value for the size (in MiB) of the /dev/shm volume for this step.
         This parameter maps to the `--shm-size` option in Docker.
     """
     ...
 
 @typing.overload
-def pypi(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def batch(*, cpu: int = 1, gpu: int = 0, memory: int = 4096, image: typing.Optional[str] = None, queue: str = "METAFLOW_BATCH_JOB_QUEUE", iam_role: str = "METAFLOW_ECS_S3_ACCESS_IAM_ROLE", execution_role: str = "METAFLOW_ECS_FARGATE_EXECUTION_ROLE", shared_memory: typing.Optional[int] = None, max_swap: typing.Optional[int] = None, swappiness: typing.Optional[int] = None, use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = None, inferentia: int = 0, trainium: int = None, efa: int = 0, ephemeral_storage: int = None, log_driver: typing.Optional[str] = None, log_options: typing.Optional[typing.List[str]] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the PyPI packages for the step.
-    
-    Information in this decorator will augment any
-    attributes set in the `@pyi_base` flow-level decorator. Hence,
-    you can use `@pypi_base` to set packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
+    Specifies that this step should execute on [AWS Batch](https://aws.amazon.com/batch/).
     
     Parameters
     ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
+    cpu : int, default 1
+        Number of CPUs required for this step. If `@resources` is
+        also present, the maximum value from all decorators is used.
+    gpu : int, default 0
+        Number of GPUs required for this step. If `@resources` is
+        also present, the maximum value from all decorators is used.
+    memory : int, default 4096
+        Memory size (in MB) required for this step. If
+        `@resources` is also present, the maximum value from all decorators is
+        used.
+    image : str, optional, default None
+        Docker image to use when launching on AWS Batch. If not specified, and
+        METAFLOW_BATCH_CONTAINER_IMAGE is specified, that image is used. If
+        not, a default Docker image mapping to the current version of Python is used.
+    queue : str, default METAFLOW_BATCH_JOB_QUEUE
+        AWS Batch Job Queue to submit the job to.
+    iam_role : str, default METAFLOW_ECS_S3_ACCESS_IAM_ROLE
+        AWS IAM role that AWS Batch container uses to access AWS cloud resources.
+    execution_role : str, default METAFLOW_ECS_FARGATE_EXECUTION_ROLE
+        AWS IAM role that AWS Batch can use [to trigger AWS Fargate tasks]
+        (https://docs.aws.amazon.com/batch/latest/userguide/execution-IAM-role.html).
+    shared_memory : int, optional, default None
+        The value for the size (in MiB) of the /dev/shm volume for this step.
+        This parameter maps to the `--shm-size` option in Docker.
+    max_swap : int, optional, default None
+        The total amount of swap memory (in MiB) a container can use for this
+        step. This parameter is translated to the `--memory-swap` option in
+        Docker where the value is the sum of the container memory plus the
+        `max_swap` value.
+    swappiness : int, optional, default None
+        This allows you to tune memory swappiness behavior for this step.
+        A swappiness value of 0 causes swapping not to happen unless absolutely
+        necessary. A swappiness value of 100 causes pages to be swapped very
+        aggressively. Accepted values are whole numbers between 0 and 100.
+    use_tmpfs : bool, default False
+        This enables an explicit tmpfs mount for this step. Note that tmpfs is
+        not available on Fargate compute environments
+    tmpfs_tempdir : bool, default True
+        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
+    tmpfs_size : int, optional, default None
+        The value for the size (in MiB) of the tmpfs mount for this step.
+        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
+        memory allocated for this step.
+    tmpfs_path : str, optional, default None
+        Path to tmpfs mount for this step. Defaults to /metaflow_temp.
+    inferentia : int, default 0
+        Number of Inferentia chips required for this step.
+    trainium : int, default None
+        Alias for inferentia. Use only one of the two.
+    efa : int, default 0
+        Number of elastic fabric adapter network devices to attach to container
+    ephemeral_storage: int, default None
+        The total amount, in GiB, of ephemeral storage to set for the task (21-200)
+        This is only relevant for Fargate compute environments
+    log_driver: str, optional, default None
+        The log driver to use for the Amazon ECS container.
+    log_options: List[str], optional, default None
+        List of strings containing options for the chosen log driver. The configurable values
+        depend on the `log driver` chosen. Validation of these options is not supported yet.
+        Example usage: ["awslogs-group:aws/batch/job"]
     """
     ...
 
 @typing.overload
-def pypi(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def batch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def pypi(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def pypi(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
-    """
-    Specifies the PyPI packages for the step.
-    
-    Information in this decorator will augment any
-    attributes set in the `@pyi_base` flow-level decorator. Hence,
-    you can use `@pypi_base` to set packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
-    
-    Parameters
-    ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    """
+def batch(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def kubernetes(*, cpu: int = 1, memory: int = 4096, disk: int = 10240, image: typing.Optional[str] = None, image_pull_policy: str = "KUBERNETES_IMAGE_PULL_POLICY", service_account: str = "METAFLOW_KUBERNETES_SERVICE_ACCOUNT", secrets: typing.Optional[typing.List[str]] = None, namespace: str = "METAFLOW_KUBERNETES_NAMESPACE", gpu: typing.Optional[int] = None, gpu_vendor: str = "KUBERNETES_GPU_VENDOR", tolerations: typing.List[str] = [], use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = "/metaflow_temp", persistent_volume_claims: typing.Optional[typing.Dict[str, str]] = None, shared_memory: typing.Optional[int] = None, port: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def batch(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, cpu: int = 1, gpu: int = 0, memory: int = 4096, image: typing.Optional[str] = None, queue: str = "METAFLOW_BATCH_JOB_QUEUE", iam_role: str = "METAFLOW_ECS_S3_ACCESS_IAM_ROLE", execution_role: str = "METAFLOW_ECS_FARGATE_EXECUTION_ROLE", shared_memory: typing.Optional[int] = None, max_swap: typing.Optional[int] = None, swappiness: typing.Optional[int] = None, use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = None, inferentia: int = 0, trainium: int = None, efa: int = 0, ephemeral_storage: int = None, log_driver: typing.Optional[str] = None, log_options: typing.Optional[typing.List[str]] = None):
     """
-    Specifies that this step should execute on Kubernetes.
+    Specifies that this step should execute on [AWS Batch](https://aws.amazon.com/batch/).
     
     Parameters
     ----------
     cpu : int, default 1
         Number of CPUs required for this step. If `@resources` is
         also present, the maximum value from all decorators is used.
+    gpu : int, default 0
+        Number of GPUs required for this step. If `@resources` is
+        also present, the maximum value from all decorators is used.
     memory : int, default 4096
         Memory size (in MB) required for this step. If
         `@resources` is also present, the maximum value from all decorators is
         used.
-    disk : int, default 10240
-        Disk size (in MB) required for this step. If
-        `@resources` is also present, the maximum value from all decorators is
-        used.
     image : str, optional, default None
-        Docker image to use when launching on Kubernetes. If not specified, and
-        METAFLOW_KUBERNETES_CONTAINER_IMAGE is specified, that image is used. If
+        Docker image to use when launching on AWS Batch. If not specified, and
+        METAFLOW_BATCH_CONTAINER_IMAGE is specified, that image is used. If
         not, a default Docker image mapping to the current version of Python is used.
-    image_pull_policy: str, default KUBERNETES_IMAGE_PULL_POLICY
-        If given, the imagePullPolicy to be applied to the Docker image of the step.
-    service_account : str, default METAFLOW_KUBERNETES_SERVICE_ACCOUNT
-        Kubernetes service account to use when launching pod in Kubernetes.
-    secrets : List[str], optional, default None
-        Kubernetes secrets to use when launching pod in Kubernetes. These
-        secrets are in addition to the ones defined in `METAFLOW_KUBERNETES_SECRETS`
-        in Metaflow configuration.
-    namespace : str, default METAFLOW_KUBERNETES_NAMESPACE
-        Kubernetes namespace to use when launching pod in Kubernetes.
-    gpu : int, optional, default None
-        Number of GPUs required for this step. A value of zero implies that
-        the scheduled node should not have GPUs.
-    gpu_vendor : str, default KUBERNETES_GPU_VENDOR
-        The vendor of the GPUs to be used for this step.
-    tolerations : List[str], default []
-        The default is extracted from METAFLOW_KUBERNETES_TOLERATIONS.
-        Kubernetes tolerations to use when launching pod in Kubernetes.
+    queue : str, default METAFLOW_BATCH_JOB_QUEUE
+        AWS Batch Job Queue to submit the job to.
+    iam_role : str, default METAFLOW_ECS_S3_ACCESS_IAM_ROLE
+        AWS IAM role that AWS Batch container uses to access AWS cloud resources.
+    execution_role : str, default METAFLOW_ECS_FARGATE_EXECUTION_ROLE
+        AWS IAM role that AWS Batch can use [to trigger AWS Fargate tasks]
+        (https://docs.aws.amazon.com/batch/latest/userguide/execution-IAM-role.html).
+    shared_memory : int, optional, default None
+        The value for the size (in MiB) of the /dev/shm volume for this step.
+        This parameter maps to the `--shm-size` option in Docker.
+    max_swap : int, optional, default None
+        The total amount of swap memory (in MiB) a container can use for this
+        step. This parameter is translated to the `--memory-swap` option in
+        Docker where the value is the sum of the container memory plus the
+        `max_swap` value.
+    swappiness : int, optional, default None
+        This allows you to tune memory swappiness behavior for this step.
+        A swappiness value of 0 causes swapping not to happen unless absolutely
+        necessary. A swappiness value of 100 causes pages to be swapped very
+        aggressively. Accepted values are whole numbers between 0 and 100.
     use_tmpfs : bool, default False
-        This enables an explicit tmpfs mount for this step.
+        This enables an explicit tmpfs mount for this step. Note that tmpfs is
+        not available on Fargate compute environments
     tmpfs_tempdir : bool, default True
         sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
-    tmpfs_size : int, optional, default: None
+    tmpfs_size : int, optional, default None
         The value for the size (in MiB) of the tmpfs mount for this step.
         This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
         memory allocated for this step.
-    tmpfs_path : str, optional, default /metaflow_temp
-        Path to tmpfs mount for this step.
-    persistent_volume_claims : Dict[str, str], optional, default None
-        A map (dictionary) of persistent volumes to be mounted to the pod for this step. The map is from persistent
-        volumes to the path to which the volume is to be mounted, e.g., `{'pvc-name': '/path/to/mount/on'}`.
-    shared_memory: int, optional
-        Shared memory size (in MiB) required for this step
-    port: int, optional
-        Port number to specify in the Kubernetes job object
+    tmpfs_path : str, optional, default None
+        Path to tmpfs mount for this step. Defaults to /metaflow_temp.
+    inferentia : int, default 0
+        Number of Inferentia chips required for this step.
+    trainium : int, default None
+        Alias for inferentia. Use only one of the two.
+    efa : int, default 0
+        Number of elastic fabric adapter network devices to attach to container
+    ephemeral_storage: int, default None
+        The total amount, in GiB, of ephemeral storage to set for the task (21-200)
+        This is only relevant for Fargate compute environments
+    log_driver: str, optional, default None
+        The log driver to use for the Amazon ECS container.
+    log_options: List[str], optional, default None
+        List of strings containing options for the chosen log driver. The configurable values
+        depend on the `log driver` chosen. Validation of these options is not supported yet.
+        Example usage: ["awslogs-group:aws/batch/job"]
+    """
+    ...
+
+@typing.overload
+def catch(*, var: typing.Optional[str] = None, print_exception: bool = True) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies that the step will success under all circumstances.
+    
+    The decorator will create an optional artifact, specified by `var`, which
+    contains the exception raised. You can use it to detect the presence
+    of errors, indicating that all happy-path artifacts produced by the step
+    are missing.
+    
+    Parameters
+    ----------
+    var : str, optional, default None
+        Name of the artifact in which to store the caught exception.
+        If not specified, the exception is not stored.
+    print_exception : bool, default True
+        Determines whether or not the exception is printed to
+        stdout when caught.
+    """
+    ...
+
+@typing.overload
+def catch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def catch(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def catch(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, var: typing.Optional[str] = None, print_exception: bool = True):
+    """
+    Specifies that the step will success under all circumstances.
+    
+    The decorator will create an optional artifact, specified by `var`, which
+    contains the exception raised. You can use it to detect the presence
+    of errors, indicating that all happy-path artifacts produced by the step
+    are missing.
+    
+    Parameters
+    ----------
+    var : str, optional, default None
+        Name of the artifact in which to store the caught exception.
+        If not specified, the exception is not stored.
+    print_exception : bool, default True
+        Determines whether or not the exception is printed to
+        stdout when caught.
     """
     ...
 
 @typing.overload
 def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies environment variables to be set prior to the execution of a step.
@@ -1091,100 +1142,114 @@
     ----------
     vars : Dict[str, str], default {}
         Dictionary of environment variables to set.
     """
     ...
 
 @typing.overload
-def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies secrets to be retrieved and injected as environment variables prior to
-    the execution of a step.
+    Specifies the number of times the task corresponding
+    to a step needs to be retried.
+    
+    This decorator is useful for handling transient errors, such as networking issues.
+    If your task contains operations that can't be retried safely, e.g. database updates,
+    it is advisable to annotate it with `@retry(times=0)`.
+    
+    This can be used in conjunction with the `@catch` decorator. The `@catch`
+    decorator will execute a no-op task after all retries have been exhausted,
+    ensuring that the flow execution can continue.
     
     Parameters
     ----------
-    sources : List[Union[str, Dict[str, Any]]], default: []
-        List of secret specs, defining how the secrets are to be retrieved
+    times : int, default 3
+        Number of times to retry this task.
+    minutes_between_retries : int, default 2
+        Number of minutes between retries.
     """
     ...
 
 @typing.overload
-def secrets(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def retry(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def secrets(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def retry(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def secrets(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []):
+def retry(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, times: int = 3, minutes_between_retries: int = 2):
     """
-    Specifies secrets to be retrieved and injected as environment variables prior to
-    the execution of a step.
+    Specifies the number of times the task corresponding
+    to a step needs to be retried.
+    
+    This decorator is useful for handling transient errors, such as networking issues.
+    If your task contains operations that can't be retried safely, e.g. database updates,
+    it is advisable to annotate it with `@retry(times=0)`.
+    
+    This can be used in conjunction with the `@catch` decorator. The `@catch`
+    decorator will execute a no-op task after all retries have been exhausted,
+    ensuring that the flow execution can continue.
     
     Parameters
     ----------
-    sources : List[Union[str, Dict[str, Any]]], default: []
-        List of secret specs, defining how the secrets are to be retrieved
+    times : int, default 3
+        Number of times to retry this task.
+    minutes_between_retries : int, default 2
+        Number of minutes between retries.
     """
     ...
 
 @typing.overload
-def conda(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the Conda environment for the step.
+    Creates a human-readable report, a Metaflow Card, after this step completes.
     
-    Information in this decorator will augment any
-    attributes set in the `@conda_base` flow-level decorator. Hence,
-    you can use `@conda_base` to set packages required by all
-    steps and use `@conda` to specify step-specific overrides.
+    Note that you may add multiple `@card` decorators in a step with different parameters.
     
     Parameters
     ----------
-    packages : Dict[str, str], default {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables @conda.
+    type : str, default 'default'
+        Card type.
+    id : str, optional, default None
+        If multiple cards are present, use this id to identify this card.
+    options : Dict[str, Any], default {}
+        Options passed to the card. The contents depend on the card type.
+    timeout : int, default 45
+        Interrupt reporting if it takes more than this many seconds.
+    
+    
     """
     ...
 
 @typing.overload
-def conda(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def card(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def conda(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def card(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def conda(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
+def card(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45):
     """
-    Specifies the Conda environment for the step.
+    Creates a human-readable report, a Metaflow Card, after this step completes.
     
-    Information in this decorator will augment any
-    attributes set in the `@conda_base` flow-level decorator. Hence,
-    you can use `@conda_base` to set packages required by all
-    steps and use `@conda` to specify step-specific overrides.
+    Note that you may add multiple `@card` decorators in a step with different parameters.
     
     Parameters
     ----------
-    packages : Dict[str, str], default {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables @conda.
+    type : str, default 'default'
+        Card type.
+    id : str, optional, default None
+        If multiple cards are present, use this id to identify this card.
+    options : Dict[str, Any], default {}
+        Options passed to the card. The contents depend on the card type.
+    timeout : int, default 45
+        Interrupt reporting if it takes more than this many seconds.
+    
+    
     """
     ...
 
 @typing.overload
 def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies a timeout for your step.
@@ -1238,206 +1303,131 @@
         Number of minutes to wait prior to timing out.
     hours : int, default 0
         Number of hours to wait prior to timing out.
     """
     ...
 
 @typing.overload
-def batch(*, cpu: int = 1, gpu: int = 0, memory: int = 4096, image: typing.Optional[str] = None, queue: str = "METAFLOW_BATCH_JOB_QUEUE", iam_role: str = "METAFLOW_ECS_S3_ACCESS_IAM_ROLE", execution_role: str = "METAFLOW_ECS_FARGATE_EXECUTION_ROLE", shared_memory: typing.Optional[int] = None, max_swap: typing.Optional[int] = None, swappiness: typing.Optional[int] = None, use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = None, inferentia: int = 0, trainium: int = None, efa: int = 0, ephemeral_storage: int = None, log_driver: typing.Optional[str] = None, log_options: typing.Optional[typing.List[str]] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def pypi(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies that this step should execute on [AWS Batch](https://aws.amazon.com/batch/).
+    Specifies the PyPI packages for the step.
+    
+    Information in this decorator will augment any
+    attributes set in the `@pyi_base` flow-level decorator. Hence,
+    you can use `@pypi_base` to set packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     
     Parameters
     ----------
-    cpu : int, default 1
-        Number of CPUs required for this step. If `@resources` is
-        also present, the maximum value from all decorators is used.
-    gpu : int, default 0
-        Number of GPUs required for this step. If `@resources` is
-        also present, the maximum value from all decorators is used.
-    memory : int, default 4096
-        Memory size (in MB) required for this step. If
-        `@resources` is also present, the maximum value from all decorators is
-        used.
-    image : str, optional, default None
-        Docker image to use when launching on AWS Batch. If not specified, and
-        METAFLOW_BATCH_CONTAINER_IMAGE is specified, that image is used. If
-        not, a default Docker image mapping to the current version of Python is used.
-    queue : str, default METAFLOW_BATCH_JOB_QUEUE
-        AWS Batch Job Queue to submit the job to.
-    iam_role : str, default METAFLOW_ECS_S3_ACCESS_IAM_ROLE
-        AWS IAM role that AWS Batch container uses to access AWS cloud resources.
-    execution_role : str, default METAFLOW_ECS_FARGATE_EXECUTION_ROLE
-        AWS IAM role that AWS Batch can use [to trigger AWS Fargate tasks]
-        (https://docs.aws.amazon.com/batch/latest/userguide/execution-IAM-role.html).
-    shared_memory : int, optional, default None
-        The value for the size (in MiB) of the /dev/shm volume for this step.
-        This parameter maps to the `--shm-size` option in Docker.
-    max_swap : int, optional, default None
-        The total amount of swap memory (in MiB) a container can use for this
-        step. This parameter is translated to the `--memory-swap` option in
-        Docker where the value is the sum of the container memory plus the
-        `max_swap` value.
-    swappiness : int, optional, default None
-        This allows you to tune memory swappiness behavior for this step.
-        A swappiness value of 0 causes swapping not to happen unless absolutely
-        necessary. A swappiness value of 100 causes pages to be swapped very
-        aggressively. Accepted values are whole numbers between 0 and 100.
-    use_tmpfs : bool, default False
-        This enables an explicit tmpfs mount for this step. Note that tmpfs is
-        not available on Fargate compute environments
-    tmpfs_tempdir : bool, default True
-        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
-    tmpfs_size : int, optional, default None
-        The value for the size (in MiB) of the tmpfs mount for this step.
-        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
-        memory allocated for this step.
-    tmpfs_path : str, optional, default None
-        Path to tmpfs mount for this step. Defaults to /metaflow_temp.
-    inferentia : int, default 0
-        Number of Inferentia chips required for this step.
-    trainium : int, default None
-        Alias for inferentia. Use only one of the two.
-    efa : int, default 0
-        Number of elastic fabric adapter network devices to attach to container
-    ephemeral_storage: int, default None
-        The total amount, in GiB, of ephemeral storage to set for the task (21-200)
-        This is only relevant for Fargate compute environments
-    log_driver: str, optional, default None
-        The log driver to use for the Amazon ECS container.
-    log_options: List[str], optional, default None
-        List of strings containing options for the chosen log driver. The configurable values
-        depend on the `log driver` chosen. Validation of these options is not supported yet.
-        Example usage: ["awslogs-group:aws/batch/job"]
+    packages : Dict[str, str], default: {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
 @typing.overload
-def batch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def pypi(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def batch(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def pypi(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def batch(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, cpu: int = 1, gpu: int = 0, memory: int = 4096, image: typing.Optional[str] = None, queue: str = "METAFLOW_BATCH_JOB_QUEUE", iam_role: str = "METAFLOW_ECS_S3_ACCESS_IAM_ROLE", execution_role: str = "METAFLOW_ECS_FARGATE_EXECUTION_ROLE", shared_memory: typing.Optional[int] = None, max_swap: typing.Optional[int] = None, swappiness: typing.Optional[int] = None, use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = None, inferentia: int = 0, trainium: int = None, efa: int = 0, ephemeral_storage: int = None, log_driver: typing.Optional[str] = None, log_options: typing.Optional[typing.List[str]] = None):
+def pypi(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
     """
-    Specifies that this step should execute on [AWS Batch](https://aws.amazon.com/batch/).
+    Specifies the PyPI packages for the step.
+    
+    Information in this decorator will augment any
+    attributes set in the `@pyi_base` flow-level decorator. Hence,
+    you can use `@pypi_base` to set packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     
     Parameters
     ----------
-    cpu : int, default 1
-        Number of CPUs required for this step. If `@resources` is
-        also present, the maximum value from all decorators is used.
-    gpu : int, default 0
-        Number of GPUs required for this step. If `@resources` is
-        also present, the maximum value from all decorators is used.
-    memory : int, default 4096
-        Memory size (in MB) required for this step. If
-        `@resources` is also present, the maximum value from all decorators is
-        used.
-    image : str, optional, default None
-        Docker image to use when launching on AWS Batch. If not specified, and
-        METAFLOW_BATCH_CONTAINER_IMAGE is specified, that image is used. If
-        not, a default Docker image mapping to the current version of Python is used.
-    queue : str, default METAFLOW_BATCH_JOB_QUEUE
-        AWS Batch Job Queue to submit the job to.
-    iam_role : str, default METAFLOW_ECS_S3_ACCESS_IAM_ROLE
-        AWS IAM role that AWS Batch container uses to access AWS cloud resources.
-    execution_role : str, default METAFLOW_ECS_FARGATE_EXECUTION_ROLE
-        AWS IAM role that AWS Batch can use [to trigger AWS Fargate tasks]
-        (https://docs.aws.amazon.com/batch/latest/userguide/execution-IAM-role.html).
-    shared_memory : int, optional, default None
-        The value for the size (in MiB) of the /dev/shm volume for this step.
-        This parameter maps to the `--shm-size` option in Docker.
-    max_swap : int, optional, default None
-        The total amount of swap memory (in MiB) a container can use for this
-        step. This parameter is translated to the `--memory-swap` option in
-        Docker where the value is the sum of the container memory plus the
-        `max_swap` value.
-    swappiness : int, optional, default None
-        This allows you to tune memory swappiness behavior for this step.
-        A swappiness value of 0 causes swapping not to happen unless absolutely
-        necessary. A swappiness value of 100 causes pages to be swapped very
-        aggressively. Accepted values are whole numbers between 0 and 100.
-    use_tmpfs : bool, default False
-        This enables an explicit tmpfs mount for this step. Note that tmpfs is
-        not available on Fargate compute environments
-    tmpfs_tempdir : bool, default True
-        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
-    tmpfs_size : int, optional, default None
-        The value for the size (in MiB) of the tmpfs mount for this step.
-        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
-        memory allocated for this step.
-    tmpfs_path : str, optional, default None
-        Path to tmpfs mount for this step. Defaults to /metaflow_temp.
-    inferentia : int, default 0
-        Number of Inferentia chips required for this step.
-    trainium : int, default None
-        Alias for inferentia. Use only one of the two.
-    efa : int, default 0
-        Number of elastic fabric adapter network devices to attach to container
-    ephemeral_storage: int, default None
-        The total amount, in GiB, of ephemeral storage to set for the task (21-200)
-        This is only relevant for Fargate compute environments
-    log_driver: str, optional, default None
-        The log driver to use for the Amazon ECS container.
-    log_options: List[str], optional, default None
-        List of strings containing options for the chosen log driver. The configurable values
-        depend on the `log driver` chosen. Validation of these options is not supported yet.
-        Example usage: ["awslogs-group:aws/batch/job"]
+    packages : Dict[str, str], default: {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
 @typing.overload
-def conda_base(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the Conda environment for all steps of the flow.
+    Specifies secrets to be retrieved and injected as environment variables prior to
+    the execution of a step.
     
-    Use `@conda_base` to set common libraries required by all
-    steps and use `@conda` to specify step-specific additions.
+    Parameters
+    ----------
+    sources : List[Union[str, Dict[str, Any]]], default: []
+        List of secret specs, defining how the secrets are to be retrieved
+    """
+    ...
+
+@typing.overload
+def secrets(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def secrets(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def secrets(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []):
+    """
+    Specifies secrets to be retrieved and injected as environment variables prior to
+    the execution of a step.
     
     Parameters
     ----------
-    packages : Dict[str, str], default {}
+    sources : List[Union[str, Dict[str, Any]]], default: []
+        List of secret specs, defining how the secrets are to be retrieved
+    """
+    ...
+
+@typing.overload
+def pypi_base(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies the PyPI packages for all steps of the flow.
+    
+    Use `@pypi_base` to set common packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
+    Parameters
+    ----------
+    packages : Dict[str, str], default: {}
         Packages to use for this flow. The key is the name of the package
         and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
+    python : str, optional, default: None
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables Conda.
     """
     ...
 
 @typing.overload
-def conda_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+def pypi_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
     ...
 
-def conda_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
+def pypi_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
     """
-    Specifies the Conda environment for all steps of the flow.
-    
-    Use `@conda_base` to set common libraries required by all
-    steps and use `@conda` to specify step-specific additions.
+    Specifies the PyPI packages for all steps of the flow.
     
+    Use `@pypi_base` to set common packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     Parameters
     ----------
-    packages : Dict[str, str], default {}
+    packages : Dict[str, str], default: {}
         Packages to use for this flow. The key is the name of the package
         and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
+    python : str, optional, default: None
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables Conda.
     """
     ...
 
 @typing.overload
 def trigger_on_finish(*, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the flow(s) that this flow depends on.
@@ -1555,182 +1545,59 @@
         contain only lowercase alphanumeric characters and underscores.
     
     
     """
     ...
 
 @typing.overload
-def schedule(*, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies the times when the flow should be run when running on a
-    production scheduler.
-    
-    Parameters
-    ----------
-    hourly : bool, default False
-        Run the workflow hourly.
-    daily : bool, default True
-        Run the workflow daily.
-    weekly : bool, default False
-        Run the workflow weekly.
-    cron : str, optional, default None
-        Run the workflow at [a custom Cron schedule](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html#cron-expressions)
-        specified by this expression.
-    timezone : str, optional, default None
-        Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
-        which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
-    """
-    ...
-
-@typing.overload
-def schedule(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
-    ...
-
-def schedule(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None):
-    """
-    Specifies the times when the flow should be run when running on a
-    production scheduler.
-    
-    Parameters
-    ----------
-    hourly : bool, default False
-        Run the workflow hourly.
-    daily : bool, default True
-        Run the workflow daily.
-    weekly : bool, default False
-        Run the workflow weekly.
-    cron : str, optional, default None
-        Run the workflow at [a custom Cron schedule](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html#cron-expressions)
-        specified by this expression.
-    timezone : str, optional, default None
-        Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
-        which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
-    """
-    ...
-
-def airflow_s3_key_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, bucket_key: typing.Union[str, typing.List[str]], bucket_name: str, wildcard_match: bool, aws_conn_id: str, verify: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    The `@airflow_s3_key_sensor` decorator attaches a Airflow [S3KeySensor](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/_api/airflow/providers/amazon/aws/sensors/s3/index.html#airflow.providers.amazon.aws.sensors.s3.S3KeySensor)
-    before the start step of the flow. This decorator only works when a flow is scheduled on Airflow
-    and is compiled using `airflow create`. More than one `@airflow_s3_key_sensor` can be
-    added as a flow decorators. Adding more than one decorator will ensure that `start` step
-    starts only after all sensors finish.
-    
-    Parameters
-    ----------
-    timeout : int
-        Time, in seconds before the task times out and fails. (Default: 3600)
-    poke_interval : int
-        Time in seconds that the job should wait in between each try. (Default: 60)
-    mode : str
-        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
-    exponential_backoff : bool
-        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
-    pool : str
-        the slot pool this task should run in,
-        slot pools are a way to limit concurrency for certain tasks. (Default:None)
-    soft_fail : bool
-        Set to true to mark the task as SKIPPED on failure. (Default: False)
-    name : str
-        Name of the sensor on Airflow
-    description : str
-        Description of sensor in the Airflow UI
-    bucket_key : Union[str, List[str]]
-        The key(s) being waited on. Supports full s3:// style url or relative path from root level.
-        When it's specified as a full s3:// url, please leave `bucket_name` as None
-    bucket_name : str
-        Name of the S3 bucket. Only needed when bucket_key is not provided as a full s3:// url.
-        When specified, all the keys passed to bucket_key refers to this bucket. (Default:None)
-    wildcard_match : bool
-        whether the bucket_key should be interpreted as a Unix wildcard pattern. (Default: False)
-    aws_conn_id : str
-        a reference to the s3 connection on Airflow. (Default: None)
-    verify : bool
-        Whether or not to verify SSL certificates for S3 connection. (Default: None)
-    """
-    ...
-
-def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+def conda_base(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
-    The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
-    This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
+    Specifies the Conda environment for all steps of the flow.
     
-    Parameters
-    ----------
-    timeout : int
-        Time, in seconds before the task times out and fails. (Default: 3600)
-    poke_interval : int
-        Time in seconds that the job should wait in between each try. (Default: 60)
-    mode : str
-        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
-    exponential_backoff : bool
-        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
-    pool : str
-        the slot pool this task should run in,
-        slot pools are a way to limit concurrency for certain tasks. (Default:None)
-    soft_fail : bool
-        Set to true to mark the task as SKIPPED on failure. (Default: False)
-    name : str
-        Name of the sensor on Airflow
-    description : str
-        Description of sensor in the Airflow UI
-    external_dag_id : str
-        The dag_id that contains the task you want to wait for.
-    external_task_ids : List[str]
-        The list of task_ids that you want to wait for.
-        If None (default value) the sensor waits for the DAG. (Default: None)
-    allowed_states : List[str]
-        Iterable of allowed states, (Default: ['success'])
-    failed_states : List[str]
-        Iterable of failed or dis-allowed states. (Default: None)
-    execution_delta : datetime.timedelta
-        time difference with the previous execution to look at,
-        the default is the same logical date as the current task or DAG. (Default: None)
-    check_existence: bool
-        Set to True to check if the external task exists or check if
-        the DAG to wait for exists. (Default: True)
-    """
-    ...
-
-@typing.overload
-def pypi_base(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies the PyPI packages for all steps of the flow.
+    Use `@conda_base` to set common libraries required by all
+    steps and use `@conda` to specify step-specific additions.
     
-    Use `@pypi_base` to set common packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
     Parameters
     ----------
-    packages : Dict[str, str], default: {}
+    packages : Dict[str, str], default {}
         Packages to use for this flow. The key is the name of the package
         and the value is the version to use.
-    python : str, optional, default: None
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables Conda.
     """
     ...
 
 @typing.overload
-def pypi_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+def conda_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
     ...
 
-def pypi_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
+def conda_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
     """
-    Specifies the PyPI packages for all steps of the flow.
+    Specifies the Conda environment for all steps of the flow.
+    
+    Use `@conda_base` to set common libraries required by all
+    steps and use `@conda` to specify step-specific additions.
     
-    Use `@pypi_base` to set common packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
     Parameters
     ----------
-    packages : Dict[str, str], default: {}
+    packages : Dict[str, str], default {}
         Packages to use for this flow. The key is the name of the package
         and the value is the version to use.
-    python : str, optional, default: None
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables Conda.
     """
     ...
 
 @typing.overload
 def trigger(*, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the event(s) that this flow depends on.
@@ -1821,14 +1688,147 @@
     options : Dict[str, Any], default {}
         Backend-specific configuration for tuning eventing behavior.
     
     
     """
     ...
 
+@typing.overload
+def schedule(*, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies the times when the flow should be run when running on a
+    production scheduler.
+    
+    Parameters
+    ----------
+    hourly : bool, default False
+        Run the workflow hourly.
+    daily : bool, default True
+        Run the workflow daily.
+    weekly : bool, default False
+        Run the workflow weekly.
+    cron : str, optional, default None
+        Run the workflow at [a custom Cron schedule](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html#cron-expressions)
+        specified by this expression.
+    timezone : str, optional, default None
+        Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
+        which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
+    """
+    ...
+
+@typing.overload
+def schedule(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+    ...
+
+def schedule(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None):
+    """
+    Specifies the times when the flow should be run when running on a
+    production scheduler.
+    
+    Parameters
+    ----------
+    hourly : bool, default False
+        Run the workflow hourly.
+    daily : bool, default True
+        Run the workflow daily.
+    weekly : bool, default False
+        Run the workflow weekly.
+    cron : str, optional, default None
+        Run the workflow at [a custom Cron schedule](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html#cron-expressions)
+        specified by this expression.
+    timezone : str, optional, default None
+        Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
+        which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
+    """
+    ...
+
+def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
+    This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
+    
+    Parameters
+    ----------
+    timeout : int
+        Time, in seconds before the task times out and fails. (Default: 3600)
+    poke_interval : int
+        Time in seconds that the job should wait in between each try. (Default: 60)
+    mode : str
+        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
+    exponential_backoff : bool
+        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
+    pool : str
+        the slot pool this task should run in,
+        slot pools are a way to limit concurrency for certain tasks. (Default:None)
+    soft_fail : bool
+        Set to true to mark the task as SKIPPED on failure. (Default: False)
+    name : str
+        Name of the sensor on Airflow
+    description : str
+        Description of sensor in the Airflow UI
+    external_dag_id : str
+        The dag_id that contains the task you want to wait for.
+    external_task_ids : List[str]
+        The list of task_ids that you want to wait for.
+        If None (default value) the sensor waits for the DAG. (Default: None)
+    allowed_states : List[str]
+        Iterable of allowed states, (Default: ['success'])
+    failed_states : List[str]
+        Iterable of failed or dis-allowed states. (Default: None)
+    execution_delta : datetime.timedelta
+        time difference with the previous execution to look at,
+        the default is the same logical date as the current task or DAG. (Default: None)
+    check_existence: bool
+        Set to True to check if the external task exists or check if
+        the DAG to wait for exists. (Default: True)
+    """
+    ...
+
+def airflow_s3_key_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, bucket_key: typing.Union[str, typing.List[str]], bucket_name: str, wildcard_match: bool, aws_conn_id: str, verify: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    The `@airflow_s3_key_sensor` decorator attaches a Airflow [S3KeySensor](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/_api/airflow/providers/amazon/aws/sensors/s3/index.html#airflow.providers.amazon.aws.sensors.s3.S3KeySensor)
+    before the start step of the flow. This decorator only works when a flow is scheduled on Airflow
+    and is compiled using `airflow create`. More than one `@airflow_s3_key_sensor` can be
+    added as a flow decorators. Adding more than one decorator will ensure that `start` step
+    starts only after all sensors finish.
+    
+    Parameters
+    ----------
+    timeout : int
+        Time, in seconds before the task times out and fails. (Default: 3600)
+    poke_interval : int
+        Time in seconds that the job should wait in between each try. (Default: 60)
+    mode : str
+        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
+    exponential_backoff : bool
+        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
+    pool : str
+        the slot pool this task should run in,
+        slot pools are a way to limit concurrency for certain tasks. (Default:None)
+    soft_fail : bool
+        Set to true to mark the task as SKIPPED on failure. (Default: False)
+    name : str
+        Name of the sensor on Airflow
+    description : str
+        Description of sensor in the Airflow UI
+    bucket_key : Union[str, List[str]]
+        The key(s) being waited on. Supports full s3:// style url or relative path from root level.
+        When it's specified as a full s3:// url, please leave `bucket_name` as None
+    bucket_name : str
+        Name of the S3 bucket. Only needed when bucket_key is not provided as a full s3:// url.
+        When specified, all the keys passed to bucket_key refers to this bucket. (Default:None)
+    wildcard_match : bool
+        whether the bucket_key should be interpreted as a Unix wildcard pattern. (Default: False)
+    aws_conn_id : str
+        a reference to the s3 connection on Airflow. (Default: None)
+    verify : bool
+        Whether or not to verify SSL certificates for S3 connection. (Default: None)
+    """
+    ...
+
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
     pass None to this call.
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/cards.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/cards.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.238947                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.643816                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
-    import metaflow.plugins.cards.card_client
-    import metaflow.plugins.cards.card_modules.components
     import metaflow.plugins.cards.card_modules.basic
+    import typing
     import metaflow.plugins.cards.card_modules.card
+    import metaflow.plugins.cards.card_modules.components
     import metaflow
+    import metaflow.plugins.cards.card_client
 
 def get_cards(task: typing.Union[str, "metaflow.Task"], id: typing.Optional[str] = None, type: typing.Optional[str] = None, follow_resumed: bool = True) -> metaflow.plugins.cards.card_client.CardContainer:
     """
     Get cards related to a `Task`.
     
     Note that `get_cards` resolves the cards contained by the task, but it doesn't actually
     retrieve them from the datastore. Actual card contents are retrieved lazily either when
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/cli.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/cli.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.244457                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.648874                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.metaflow_current
+    import metaflow.exception
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/client/__init__.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/client/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.242055                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.646582                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import datetime
+    import metaflow.client.core
     import metaflow.events
     import typing
-    import metaflow.client.core
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/client/core.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/client/core.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.224613                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.632810                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
-    import datetime
-    import metaflow.client.core
-    import metaflow.exception
-    import metaflow.metaflow_current
     import tarfile
     import metaflow.events
+    import metaflow.exception
+    import typing
+    import metaflow.metaflow_current
+    import metaflow.client.core
+    import datetime
     import metaflow
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/client/filecache.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/client/filecache.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.245301                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.649759                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/clone_util.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/clone_util.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.242614                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.647139                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaDatum(tuple, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/events.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/events.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.226538                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.634704                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow
     import metaflow.events
+    import metaflow
 
 TYPE_CHECKING: bool
 
 class MetaflowEvent(tuple, metaclass=type):
     @staticmethod
     def __new__(_cls, name, id, timestamp, type):
         """
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/exception.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/exception.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.217208                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.625479                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/flowspec.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/flowspec.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.225957                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.634133                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
+    import metaflow.unbounded_foreach
     import metaflow.parameters
+    import typing
     import metaflow.exception
-    import metaflow.unbounded_foreach
     import metaflow.datastore.inputs
 
 class DelayedEvaluationParameter(object, metaclass=type):
     def __init__(self, name, field, fun):
         ...
     def __call__(self, return_str = False):
         ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/includefile.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/includefile.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.235704                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.642120                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import io
+    import metaflow.parameters
     import typing
     import metaflow._vendor.click.types
-    import metaflow.parameters
     import metaflow.plugins.datatools.s3.s3
-    import io
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/metadata/metadata.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/metadata/metadata.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.269008                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.670701                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metadata.metadata
     import metaflow.exception
+    import metaflow.metadata.metadata
 
 class MetaflowInternalError(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 class MetaflowTaggingError(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/metadata/util.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/metadata/util.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.302766                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.701876                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def copy_tree(src, dst, update = False):
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/metaflow_config.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/metaflow_config.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.218222                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.626459                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
@@ -84,14 +84,16 @@
 
 DATATOOLS_LOCALROOT: None
 
 AWS_SECRETS_MANAGER_DEFAULT_REGION: None
 
 GCP_SECRET_MANAGER_PREFIX: None
 
+AZURE_KEY_VAULT_PREFIX: None
+
 ARTIFACT_LOCALROOT: str
 
 CARD_SUFFIX: str
 
 CARD_LOCALROOT: None
 
 CARD_S3ROOT: None
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/metaflow_current.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/metaflow_current.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.313497                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.715308                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.events
     import typing
+    import metaflow.plugins.cards.component_serializer
     import metaflow.metaflow_current
-    import metaflow.events
     import metaflow
-    import metaflow.plugins.cards.component_serializer
 
 TYPE_CHECKING: bool
 
 TEMPDIR: str
 
 class Parallel(tuple, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/mflog/mflog.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/__init__.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.269524                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.650793                                        #
 ##################################################################################
 
 from __future__ import annotations
 
-import typing
-if typing.TYPE_CHECKING:
-    import datetime
 
-VERSION: bytes
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
+        ...
+    def __str__(self):
+        ...
+    ...
 
-RE: bytes
-
-ISOFORMAT: str
-
-MISSING_TIMESTAMP: datetime.datetime
-
-MISSING_TIMESTAMP_STR: str
+MAGIC_FILE: str
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/multicore_utils.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/multicore_utils.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.218650                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.626879                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import typing
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/parameters.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/parameters.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.219723                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.627936                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
+    import metaflow.parameters
     import metaflow._vendor.click.types
     import metaflow.exception
-    import metaflow.parameters
+    import typing
 
 class ParameterFieldFailed(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, name, field):
         ...
     ...
 
 class ParameterFieldTypeMismatch(metaflow.exception.MetaflowException, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/__init__.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.227985                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.636187                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.card
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/airflow.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/airflow.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.274027                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.681992                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.metaflow_current
     import metaflow._vendor.click.types
     import metaflow.exception
-    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
@@ -68,14 +68,16 @@
 
 S3_ENDPOINT_URL: None
 
 SERVICE_HEADERS: dict
 
 SERVICE_INTERNAL_URL: None
 
+AZURE_KEY_VAULT_PREFIX: None
+
 class DelayedEvaluationParameter(object, metaclass=type):
     def __init__(self, name, field, fun):
         ...
     def __call__(self, return_str = False):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/airflow_cli.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/airflow_cli.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.274985                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.682927                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow.exception
     import metaflow.metaflow_current
+    import metaflow.exception
+    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/airflow_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/airflow_decorator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.271784                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.680096                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/airflow_utils.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/airflow_utils.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.271185                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.679724                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 TASK_ID_XCOM_KEY: str
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/exception.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/azure_exceptions.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.272122                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.698729                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -13,15 +13,16 @@
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
-    def __init__(self, msg):
-        ...
+class MetaflowAzureAuthenticationError(metaflow.exception.MetaflowException, metaclass=type):
+    ...
+
+class MetaflowAzureResourceError(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class NotSupportedException(metaflow.exception.MetaflowException, metaclass=type):
+class MetaflowAzurePackageError(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/__init__.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/__init__.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.272470                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.680552                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.airflow.sensors.base_sensor
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.301186                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.711398                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.exception
+    import metaflow.decorators
 
 class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, msg):
         ...
     ...
 
 class AirflowTask(object, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.301561                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.712261                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow.exception
     import metaflow.plugins.airflow.sensors.base_sensor
+    import metaflow.exception
+    import metaflow.decorators
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
         Subclasses will parse the decorator arguments to
@@ -39,16 +39,12 @@
     ...
 
 class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, msg):
         ...
     ...
 
-AIRFLOW_STATES: dict
-
-class ExternalTaskSensorDecorator(metaflow.plugins.airflow.sensors.base_sensor.AirflowSensorDecorator, metaclass=type):
-    def serialize_operator_args(self):
-        ...
+class S3KeySensorDecorator(metaflow.plugins.airflow.sensors.base_sensor.AirflowSensorDecorator, metaclass=type):
     def validate(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.301928                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.711782                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow.exception
     import metaflow.plugins.airflow.sensors.base_sensor
+    import metaflow.exception
+    import metaflow.decorators
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
         Subclasses will parse the decorator arguments to
@@ -39,12 +39,16 @@
     ...
 
 class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, msg):
         ...
     ...
 
-class S3KeySensorDecorator(metaflow.plugins.airflow.sensors.base_sensor.AirflowSensorDecorator, metaclass=type):
+AIRFLOW_STATES: dict
+
+class ExternalTaskSensorDecorator(metaflow.plugins.airflow.sensors.base_sensor.AirflowSensorDecorator, metaclass=type):
+    def serialize_operator_args(self):
+        ...
     def validate(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_client.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.290237                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.691761                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_events.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_events.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.288894                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.690461                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_workflows.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_workflows.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.294233                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.695820                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.metaflow_current
+    import metaflow.parameters
     import metaflow._vendor.click.types
     import metaflow.exception
-    import metaflow.parameters
-    import metaflow.metaflow_current
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
@@ -73,14 +73,16 @@
 
 DEFAULT_METADATA: str
 
 DEFAULT_SECRETS_BACKEND_TYPE: None
 
 GCP_SECRET_MANAGER_PREFIX: None
 
+AZURE_KEY_VAULT_PREFIX: None
+
 KUBERNETES_FETCH_EC2_METADATA: bool
 
 KUBERNETES_LABELS: str
 
 KUBERNETES_NAMESPACE: str
 
 KUBERNETES_NODE_SELECTOR: str
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.295734                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.697365                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.metaflow_current
+    import metaflow.parameters
     import metaflow.decorators
     import metaflow.exception
-    import metaflow.parameters
-    import metaflow.metaflow_current
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.289672                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.691205                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow
-    import metaflow.events
     import metaflow.metaflow_current
+    import metaflow.events
+    import metaflow
+    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/aws_client.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/aws_client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.242361                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.646882                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 cached_aws_sandbox_creds: None
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/aws_utils.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/aws_utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.287372                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.676265                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/batch.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/batch.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.309380                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.704014                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/batch_cli.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/batch_cli.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.310651                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.705349                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -18,14 +18,18 @@
 def sync_local_metadata_from_datastore(metadata_local_dir, task_ds):
     ...
 
 DATASTORE_LOCAL_DIR: str
 
 TASK_LOG_SOURCE: str
 
+UBF_CONTROL: str
+
+UBF_TASK: str
+
 class Batch(object, metaclass=type):
     def __init__(self, metadata, environment):
         ...
     def list_jobs(self, flow_name, run_id, user, echo):
         ...
     def kill_jobs(self, flow_name, run_id, user, echo):
         ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/batch_client.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/batch_client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.308424                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.703038                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.310095                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.704725                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow.exception
     import metaflow.metaflow_current
+    import metaflow.exception
+    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class ResourcesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     ...
 
 def get_run_time_limit_for_task(step_decos):
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.311041                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.710576                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import abc
     import metaflow.plugins.secrets
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.302975                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.705577                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 SFN_DYNAMO_DB_TABLE: None
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.303777                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.707073                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
-class EventBridgeClient(object, metaclass=type):
-    def __init__(self, name):
+AWS_SANDBOX_ENABLED: bool
+
+AWS_SANDBOX_REGION: None
+
+SFN_EXECUTION_LOG_GROUP_ARN: None
+
+class StepFunctionsClient(object, metaclass=type):
+    def __init__(self):
         ...
-    def cron(self, cron):
+    def search(self, name):
         ...
-    def role_arn(self, role_arn):
+    def push(self, name, definition, role_arn, log_execution_history):
         ...
-    def state_machine_arn(self, state_machine_arn):
+    def get(self, name):
         ...
-    def schedule(self):
+    def trigger(self, state_machine_arn, input):
         ...
-    def delete(self):
+    def list_executions(self, state_machine_arn, states):
+        ...
+    def terminate_execution(self, execution_arn):
+        ...
+    def get_state_machine_arn(self, name):
+        ...
+    def delete(self, name):
         ...
-    ...
-
-def format(name):
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.303512                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.706174                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.305943                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.708932                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.307221                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.710171                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.metaflow_current
+    import metaflow.parameters
     import metaflow.decorators
     import metaflow.exception
-    import metaflow.parameters
-    import metaflow.metaflow_current
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/events_decorator.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.304082                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.655291                                        #
 ##################################################################################
 
 from __future__ import annotations
 
+import typing
+if typing.TYPE_CHECKING:
+    import metaflow.metaflow_current
+    import metaflow.decorators
 
-AWS_SANDBOX_ENABLED: bool
+current: metaflow.metaflow_current.Current
 
-AWS_SANDBOX_REGION: None
-
-SFN_EXECUTION_LOG_GROUP_ARN: None
-
-class StepFunctionsClient(object, metaclass=type):
-    def __init__(self):
-        ...
-    def search(self, name):
-        ...
-    def push(self, name, definition, role_arn, log_execution_history):
-        ...
-    def get(self, name):
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
         ...
-    def trigger(self, state_machine_arn, input):
+    def __str__(self):
         ...
-    def list_executions(self, state_machine_arn, states):
-        ...
-    def terminate_execution(self, execution_arn):
+    ...
+
+class TriggerDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
         ...
-    def get_state_machine_arn(self, name):
+    ...
+
+class TriggerOnFinishDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
         ...
-    def delete(self, name):
+    def get_top_level_options(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.303350                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.706003                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/azure_credential.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/azure_credential.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.298031                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.698509                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class AzureDefaultClientProvider(object, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/azure_exceptions.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/exception.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.298249                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.680320                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -13,16 +13,15 @@
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class MetaflowAzureAuthenticationError(metaflow.exception.MetaflowException, metaclass=type):
-    ...
-
-class MetaflowAzureResourceError(metaflow.exception.MetaflowException, metaclass=type):
+class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
+    def __init__(self, msg):
+        ...
     ...
 
-class MetaflowAzurePackageError(metaflow.exception.MetaflowException, metaclass=type):
+class NotSupportedException(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/azure_utils.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/azure_utils.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.298715                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.699129                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.299033                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.699459                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/azure/includefile_support.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/includefile_support.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.259603                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.665638                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_cli.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.282141                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.690045                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
-    import datetime
     import metaflow.parameters
+    import typing
     import metaflow.client.core
+    import datetime
     import metaflow.exception
 
 class Task(metaflow.client.core.MetaflowObject, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     @property
     def metadata(self) -> typing.List[metaflow.client.core.Metadata]:
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_client.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.262380                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.667182                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_client
-    import metaflow
     import metaflow.exception
+    import metaflow
+    import metaflow.plugins.cards.card_client
 
 TYPE_CHECKING: bool
 
 CARD_SUFFIX: str
 
 def resolve_paths_from_task(flow_datastore, pathspec = None, type = None, hash = None, card_id = None):
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_creator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_creator.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.278031                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.685990                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_datastore.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_datastore.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.279448                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.687424                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.278729                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.686683                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.metaflow_current
+    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class CardComponentCollector(object, metaclass=type):
     def __init__(self, logger = None, card_creator = None):
         ...
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/__init__.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/card.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.275827                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.667596                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
 
+TYPE_CHECKING: bool
+
 class MetaflowCard(object, metaclass=type):
     def __init__(self, options = {}, components = [], graph = None):
         ...
     def render(self, task: "metaflow.Task") -> str:
         """
         Produce custom card contents in HTML.
         
@@ -54,14 +56,7 @@
     def render(self):
         """
         `render` returns a string or dictionary. This class can be called on the client side to dynamically add components to the `MetaflowCard`
         """
         ...
     ...
 
-EXT_PKG: str
-
-def iter_namespace(ns_pkg):
-    ...
-
-MF_EXTERNAL_CARDS: list
-
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/basic.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/basic.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.253401                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.660268                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.card
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/card.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/__init__.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.263118                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.683748                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
 
-TYPE_CHECKING: bool
-
 class MetaflowCard(object, metaclass=type):
     def __init__(self, options = {}, components = [], graph = None):
         ...
     def render(self, task: "metaflow.Task") -> str:
         """
         Produce custom card contents in HTML.
         
@@ -56,7 +54,14 @@
     def render(self):
         """
         `render` returns a string or dictionary. This class can be called on the client side to dynamically add components to the `MetaflowCard`
         """
         ...
     ...
 
+EXT_PKG: str
+
+def iter_namespace(ns_pkg):
+    ...
+
+MF_EXTERNAL_CARDS: list
+
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.302265                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.712745                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def main(template, data = None, **kwargs):
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.312477                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.714161                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def render(template = "", data = {}, partials_path = ".", partials_ext = "mustache", partials_dict = {}, padding = "", def_ldel = "{{", def_rdel = "}}", scopes = None, warn = False, keep = False):
     """
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.312084                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.713771                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 linesep: str
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.311721                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.713388                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class ChevronError(SyntaxError, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/components.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/components.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.266901                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.669521                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
+    import metaflow.plugins.cards.card_modules.components
     import metaflow.plugins.cards.card_modules.card
+    import typing
     import metaflow.plugins.cards.card_modules.basic
-    import metaflow.plugins.cards.card_modules.components
 
 class LogComponent(metaflow.plugins.cards.card_modules.basic.DefaultComponent, metaclass=type):
     def __init__(self, data = None):
         ...
     def render(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.300481                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.701397                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class TypeResolvedObject(tuple, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.300668                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.701585                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.basic
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.255078                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.661463                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.card
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/card_resolver.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_resolver.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.279935                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.687908                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class CardDatastore(object, metaclass=type):
     @classmethod
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/component_serializer.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/component_serializer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.277778                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.685742                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.plugins.cards.card_modules.components
     import metaflow.plugins.cards.card_modules.card
     import metaflow.exception
     import metaflow.plugins.cards.card_modules.basic
-    import metaflow.plugins.cards.card_modules.components
 
 class MetaflowCardComponent(object, metaclass=type):
     @property
     def component_id(self):
         ...
     @component_id.setter
     def component_id(self, value):
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/cards/exception.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/exception.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.276383                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.684301                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/catch_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/catch_decorator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.246863                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.653136                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow.exception
     import metaflow.metaflow_current
+    import metaflow.exception
+    import metaflow.decorators
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/__init__.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.249747                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.652616                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.datatools.s3.s3
-    import io
     import metaflow.exception
+    import io
 
 def read_in_chunks(dst, src, src_sz, max_chunk_size):
     ...
 
 class MetaflowLocalNotFound(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/local.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/local.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.258805                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.665107                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/__init__.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.297784                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.678723                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.datatools.s3.s3
-    import io
     import metaflow.exception
+    import io
 
 class RangeInfo(tuple, metaclass=type):
     @staticmethod
     def __new__(_cls, total_size: int, request_offset: int = 0, request_length: int = -1):
         """
         Create new instance of RangeInfo(total_size, request_offset, request_length)
         """
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/s3.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/s3.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.231039                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.639354                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import io
     import typing
+    import metaflow.metaflow_current
     import metaflow.plugins.datatools.s3.s3
     import metaflow.exception
-    import metaflow.metaflow_current
     import metaflow.datastore.inputs
-    import io
 
 TYPE_CHECKING: bool
 
 class FlowSpec(object, metaclass=type):
     def __init__(self, use_cli = True):
         """
         Construct a FlowSpec
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/s3tail.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/s3tail.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.311397                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.710910                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def aws_retry(f):
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/datatools/s3/s3util.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/s3util.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.257860                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.664387                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/debug_logger.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/debug_logger.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.251264                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.657172                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.event_logger
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/debug_monitor.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/debug_monitor.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.251487                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.657613                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.monitor
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/environment_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/environment_decorator.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.248225                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.653442                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/events_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/project_decorator.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.250113                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.655839                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.metaflow_current
-
-current: metaflow.metaflow_current.Current
+    import metaflow.decorators
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class TriggerDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
-        ...
-    ...
+current: metaflow.metaflow_current.Current
+
+VALID_NAME_RE: str
+
+VALID_NAME_LEN: int
 
-class TriggerOnFinishDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
+class ProjectDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
         ...
     def get_top_level_options(self):
         ...
     ...
 
+def format_name(flow_name, project_name, deploy_prod, given_branch, user_name):
+    ...
+
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/frameworks/pytorch.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/frameworks/pytorch.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.275367                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.683300                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow.plugins.parallel_decorator
     import metaflow.metaflow_current
+    import metaflow.plugins.parallel_decorator
+    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class ParallelDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     def __init__(self, attributes = None, statically_defined = False):
         ...
     def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.300134                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.701015                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import abc
     import metaflow.plugins.secrets
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/gs_exceptions.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/utils.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.299442                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.672115                                        #
 ##################################################################################
 
 from __future__ import annotations
 
-import typing
-if typing.TYPE_CHECKING:
-    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class MetaflowGSPackageError(metaflow.exception.MetaflowException, metaclass=type):
+def conda_platform():
+    ...
+
+def wheel_tags(wheel):
+    ...
+
+def pip_tags(python_version, mamba_platform):
+    ...
+
+def parse_filename_from_url(url):
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.299264                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.700122                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class GcpDefaultClientProvider(object, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/gs_utils.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/gs_utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.299721                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.700590                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/gcp/includefile_support.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/includefile_support.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.260437                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.666107                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/kubernetes.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/kubernetes.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.285266                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.674222                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.metaflow_current
+    import metaflow.exception
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
@@ -56,14 +56,16 @@
 
 DEFAULT_METADATA: str
 
 DEFAULT_SECRETS_BACKEND_TYPE: None
 
 GCP_SECRET_MANAGER_PREFIX: None
 
+AZURE_KEY_VAULT_PREFIX: None
+
 KUBERNETES_FETCH_EC2_METADATA: bool
 
 KUBERNETES_LABELS: str
 
 KUBERNETES_SANDBOX_INIT_SCRIPT: None
 
 S3_ENDPOINT_URL: None
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.287040                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.675921                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow._vendor.click.types
     import metaflow.exception
+    import metaflow.decorators
 
 class JSONTypeClass(metaflow._vendor.click.types.ParamType, metaclass=type):
     def convert(self, value, param, ctx):
         ...
     def __str__(self):
         ...
     def __repr__(self):
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/pylint_wrapper.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.215904                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.647830                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -13,23 +13,19 @@
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-CLIENT_REFRESH_INTERVAL_SECONDS: int
-
-class KubernetesClientException(metaflow.exception.MetaflowException, metaclass=type):
+class PyLintWarn(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class KubernetesClient(object, metaclass=type):
-    def __init__(self):
-        ...
-    def get(self):
+class PyLint(object, metaclass=type):
+    def __init__(self, fname):
         ...
-    def job(self, **kwargs):
+    def has_pylint(self):
         ...
-    def jobset(self, **kwargs):
+    def run(self, logger = None, warnings = False, pylint_config = []):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.286261                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.675117                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow.exception
     import metaflow.metaflow_current
+    import metaflow.exception
+    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/parallel_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/parallel_decorator.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.246383                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.650587                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/perimeters.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/perimeters.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.216208                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.624515                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 
 class MetaflowException(Exception, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/project_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.250433                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.624217                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow.metaflow_current
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-current: metaflow.metaflow_current.Current
+CLIENT_REFRESH_INTERVAL_SECONDS: int
 
-VALID_NAME_RE: str
-
-VALID_NAME_LEN: int
+class KubernetesClientException(metaflow.exception.MetaflowException, metaclass=type):
+    ...
 
-class ProjectDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
+class KubernetesClient(object, metaclass=type):
+    def __init__(self):
         ...
-    def get_top_level_options(self):
+    def get(self):
+        ...
+    def job(self, **kwargs):
+        ...
+    def jobset(self, **kwargs):
         ...
-    ...
-
-def format_name(flow_name, project_name, deploy_prod, given_branch, user_name):
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/conda_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/conda_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.282952                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.671582                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/conda_environment.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/conda_environment.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.284005                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.672889                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import io
-    import metaflow.exception
     import abc
     import metaflow.metaflow_environment
+    import metaflow.exception
+    import io
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/pypi_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/pypi_decorator.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.282426                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.671823                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/pypi_environment.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/pypi_environment.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.284388                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.673326                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_environment
     import metaflow.plugins.pypi.conda_environment
+    import metaflow.metaflow_environment
 
 class CondaEnvironment(metaflow.metaflow_environment.MetaflowEnvironment, metaclass=type):
     def __init__(self, flow):
         ...
     def set_local_root(self, local_root):
         ...
     def decospecs(self):
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/pypi/utils.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/profilers/__init__.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,16 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.283246                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.624745                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
-class MetaflowException(Exception, metaclass=type):
-    def __init__(self, msg = "", lineno = None):
+class gpu_profile(object, metaclass=type):
+    def __init__(self, include_artifacts = True, artifact_prefix = "gpu_profile_", interval = 1):
         ...
-    def __str__(self):
+    def __call__(self, f):
         ...
     ...
 
-def conda_platform():
-    ...
-
-def wheel_tags(wheel):
-    ...
-
-def pip_tags(python_version, mamba_platform):
-    ...
-
-def parse_filename_from_url(url):
-    ...
-
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/resources_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/resources_decorator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.247343                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.651005                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/retry_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/retry_decorator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.247224                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.653900                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/secrets/__init__.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/secrets/__init__.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.248440                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.654744                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import abc
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.288523                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.698288                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import abc
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/secrets/secrets_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/secrets/secrets_decorator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.288293                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.698043                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/storage_executor.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/storage_executor.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.250891                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.656529                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/tag_cli.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/tag_cli.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.256916                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.662773                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import datetime
+    import metaflow.events
     import metaflow.client.core
-    import metaflow.exception
     import metaflow.metaflow_current
-    import metaflow.events
+    import datetime
+    import metaflow.exception
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.245825                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.650258                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.unbounded_foreach
+    import metaflow.decorators
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/plugins/timeout_decorator.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/timeout_decorator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.247986                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.651369                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.exception
+    import metaflow.decorators
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/procpoll.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/procpoll.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.243019                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.647545                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.procpoll
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/pylint_wrapper.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/logs_cli.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,45 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.243384                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.663746                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow._vendor.click.core
     import metaflow.exception
+    import metaflow.plugins.logs_cli
 
-class MetaflowException(Exception, metaclass=type):
-    def __init__(self, msg = "", lineno = None):
-        ...
-    def __str__(self):
-        ...
+LOGGER_TIMESTAMP: str
+
+class CommandException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class PyLintWarn(metaflow.exception.MetaflowException, metaclass=type):
+LOG_SOURCES: list
+
+class CustomGroup(metaflow._vendor.click.core.Group, metaclass=type):
+    def __init__(self, name = None, commands = None, default_cmd = None, **attrs):
+        ...
+    def get_command(self, ctx, cmd_name):
+        ...
+    def parse_args(self, ctx, args):
+        ...
+    def resolve_command(self, ctx, args):
+        ...
+    def format_commands(self, ctx, formatter):
+        ...
     ...
 
-class PyLint(object, metaclass=type):
-    def __init__(self, fname):
+class CustomFormatter(object, metaclass=type):
+    def __init__(self, default_cmd, original_formatter):
         ...
-    def has_pylint(self):
+    def __getattr__(self, name):
         ...
-    def run(self, logger = None, warnings = False, pylint_config = []):
+    def write_dl(self, rows):
         ...
     ...
 
+logs: CustomGroup
+
```

### Comparing `ob-metaflow-stubs-3.3/metaflow-stubs/tagging_util.pyi` & `ob-metaflow-stubs-3.4/metaflow-stubs/tagging_util.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.14.1+ob(v1)                                                   #
-# Generated on 2024-05-13T17:42:14.220030                                        #
+# MF version: 2.11.15.2+ob(v1)                                                   #
+# Generated on 2024-05-17T19:44:44.628239                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.3/ob_metaflow_stubs.egg-info/PKG-INFO` & `ob-metaflow-stubs-3.4/ob_metaflow_stubs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-metaflow-stubs
-Version: 3.3
+Version: 3.4
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `ob-metaflow-stubs-3.3/ob_metaflow_stubs.egg-info/SOURCES.txt` & `ob-metaflow-stubs-3.4/ob_metaflow_stubs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 metaflow-stubs/mflog/mflog.pyi
 metaflow-stubs/plugins/__init__.pyi
 metaflow-stubs/plugins/catch_decorator.pyi
 metaflow-stubs/plugins/debug_logger.pyi
 metaflow-stubs/plugins/debug_monitor.pyi
 metaflow-stubs/plugins/environment_decorator.pyi
 metaflow-stubs/plugins/events_decorator.pyi
+metaflow-stubs/plugins/logs_cli.pyi
 metaflow-stubs/plugins/package_cli.pyi
 metaflow-stubs/plugins/parallel_decorator.pyi
 metaflow-stubs/plugins/perimeters.pyi
 metaflow-stubs/plugins/project_decorator.pyi
 metaflow-stubs/plugins/resources_decorator.pyi
 metaflow-stubs/plugins/retry_decorator.pyi
 metaflow-stubs/plugins/storage_executor.pyi
@@ -75,14 +76,15 @@
 metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
 metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
 metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
 metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
 metaflow-stubs/plugins/azure/__init__.pyi
 metaflow-stubs/plugins/azure/azure_credential.pyi
 metaflow-stubs/plugins/azure/azure_exceptions.pyi
+metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi
 metaflow-stubs/plugins/azure/azure_utils.pyi
 metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
 metaflow-stubs/plugins/azure/includefile_support.pyi
 metaflow-stubs/plugins/cards/__init__.pyi
 metaflow-stubs/plugins/cards/card_cli.pyi
 metaflow-stubs/plugins/cards/card_client.pyi
 metaflow-stubs/plugins/cards/card_creator.pyi
```

### Comparing `ob-metaflow-stubs-3.3/setup.py` & `ob-metaflow-stubs-3.4/setup.py`

 * *Files identical despite different names*

