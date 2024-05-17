# Comparing `tmp/peak_sdk-1.5.0.tar.gz` & `tmp/peak_sdk-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peak_sdk-1.5.0.tar", max compression
+gzip compressed data, was "peak_sdk-1.6.0.tar", max compression
```

## Comparing `peak_sdk-1.5.0.tar` & `peak_sdk-1.6.0.tar`

### file list

```diff
@@ -1,108 +1,113 @@
--rw-r--r--   0        0        0    11340 2024-03-20 08:10:49.998284 peak_sdk-1.5.0/LICENSE
--rw-r--r--   0        0        0     1263 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/__init__.py
--rw-r--r--   0        0        0    22930 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/_metadata.py
--rw-r--r--   0        0        0      886 2024-03-20 08:11:26.582270 peak_sdk-1.5.0/peak/_version.py
--rw-r--r--   0        0        0      904 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/auth.py
--rw-r--r--   0        0        0     1808 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/base_client.py
--rw-r--r--   0        0        0     2486 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/callbacks.py
--rw-r--r--   0        0        0      859 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/__init_.py
--rw-r--r--   0        0        0     5720 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/args.py
--rw-r--r--   0        0        0     2384 2024-03-20 08:11:26.582270 peak_sdk-1.5.0/peak/cli/cli.py
--rw-r--r--   0        0        0     8250 2024-03-20 08:11:26.582270 peak_sdk-1.5.0/peak/cli/helpers.py
--rw-r--r--   0        0        0      898 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/press/__init__.py
--rw-r--r--   0        0        0     1459 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/press/apps/__init__.py
--rw-r--r--   0        0        0    15895 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/press/apps/deployments.py
--rw-r--r--   0        0        0    15566 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/press/apps/specs.py
--rw-r--r--   0        0        0     1499 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/press/blocks/__init__.py
--rw-r--r--   0        0        0    20260 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/press/blocks/deployments.py
--rw-r--r--   0        0        0    29517 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/press/blocks/specs.py
--rw-r--r--   0        0        0     2834 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/press/deployments.py
--rw-r--r--   0        0        0     4611 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/press/specs.py
--rw-r--r--   0        0        0      883 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/resources/__init__.py
--rw-r--r--   0        0        0    12383 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/resources/artifacts.py
--rw-r--r--   0        0        0    43125 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/resources/images.py
--rw-r--r--   0        0        0    23435 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/resources/services.py
--rw-r--r--   0        0        0     2624 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/resources/tenants.py
--rw-r--r--   0        0        0     2628 2024-03-20 08:11:26.582270 peak_sdk-1.5.0/peak/cli/resources/users.py
--rw-r--r--   0        0        0    21349 2024-03-20 08:10:50.002284 peak_sdk-1.5.0/peak/cli/resources/webapps.py
--rw-r--r--   0        0        0    48787 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/cli/resources/workflows.py
--rw-r--r--   0        0        0      185 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/cli/ruff.toml
--rw-r--r--   0        0        0     1654 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/cli/version.py
--rw-r--r--   0        0        0     7447 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/compression.py
--rw-r--r--   0        0        0     1146 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/config.py
--rw-r--r--   0        0        0     3312 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/constants.py
--rw-r--r--   0        0        0     6974 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/exceptions.py
--rw-r--r--   0        0        0    14777 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/handler.py
--rw-r--r--   0        0        0     8812 2024-03-20 08:11:26.582270 peak_sdk-1.5.0/peak/helpers.py
--rw-r--r--   0        0        0     1548 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/logger.py
--rw-r--r--   0        0        0     6230 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/output.py
--rw-r--r--   0        0        0     1112 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/press/__init__.py
--rw-r--r--   0        0        0    41975 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/press/apps.py
--rw-r--r--   0        0        0    59239 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/press/blocks.py
--rw-r--r--   0        0        0     5950 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/press/deployments.py
--rw-r--r--   0        0        0    10850 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/press/specs.py
--rw-r--r--   0        0        0        0 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/py.typed
--rw-r--r--   0        0        0     1188 2024-03-20 08:11:26.582270 peak_sdk-1.5.0/peak/resources/__init__.py
--rw-r--r--   0        0        0    14381 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/resources/artifacts.py
--rw-r--r--   0        0        0    37273 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/resources/images.py
--rw-r--r--   0        0        0    16712 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/resources/services.py
--rw-r--r--   0        0        0     2936 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/resources/tenants.py
--rw-r--r--   0        0        0     3428 2024-03-20 08:11:26.582270 peak_sdk-1.5.0/peak/resources/users.py
--rw-r--r--   0        0        0    13753 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/resources/webapps.py
--rw-r--r--   0        0        0    48716 2024-03-20 08:11:26.582270 peak_sdk-1.5.0/peak/resources/workflows.py
--rw-r--r--   0        0        0      996 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/press/apps/deployments/create_app_deployment.yaml
--rw-r--r--   0        0        0      688 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/press/apps/deployments/create_app_deployment_revision.yaml
--rw-r--r--   0        0        0      302 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/press/apps/deployments/update_app_deployment_metadata.yaml
--rw-r--r--   0        0        0      585 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/press/apps/specs/create_app_spec.yaml
--rw-r--r--   0        0        0      250 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/press/apps/specs/create_app_spec_release.yaml
--rw-r--r--   0        0        0      337 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/press/apps/specs/update_app_spec_metadata.yaml
--rw-r--r--   0        0        0      729 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/press/blocks/deployments/create_block_deployment.yaml
--rw-r--r--   0        0        0      376 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/press/blocks/deployments/create_block_deployment_revision.yaml
--rw-r--r--   0        0        0      156 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/press/blocks/deployments/patch_block_parameters.yaml
--rw-r--r--   0        0        0      304 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/press/blocks/deployments/update_block_deployment_metadata.yaml
--rw-r--r--   0        0        0     2946 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/press/blocks/specs/create_block_spec.yaml
--rw-r--r--   0        0        0     2590 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/press/blocks/specs/create_block_spec_release.yaml
--rw-r--r--   0        0        0      378 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/press/blocks/specs/update_block_spec_metadata.yaml
--rw-r--r--   0        0        0      152 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/artifacts/create_artifact.yaml
--rw-r--r--   0        0        0      104 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/artifacts/create_artifact_version.yaml
--rw-r--r--   0        0        0       99 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/artifacts/update_artifact_metadata.yaml
--rw-r--r--   0        0        0      343 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/images/dockerfile/create_image.yaml
--rw-r--r--   0        0        0      310 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/images/dockerfile/create_image_version.yaml
--rw-r--r--   0        0        0      275 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/images/dockerfile/update_version.yaml
--rw-r--r--   0        0        0      396 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/images/github/create_image.yaml
--rw-r--r--   0        0        0      369 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/images/github/create_image_version.yaml
--rw-r--r--   0        0        0      338 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/images/github/update_version.yaml
--rw-r--r--   0        0        0      390 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/images/upload/create_image.yaml
--rw-r--r--   0        0        0      395 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/images/upload/create_image_version.yaml
--rw-r--r--   0        0        0      414 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/images/upload/create_or_update_image.yaml
--rw-r--r--   0        0        0      321 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/images/upload/update_version.yaml
--rw-r--r--   0        0        0      410 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/services/create_or_update_service.yaml
--rw-r--r--   0        0        0      410 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/services/create_service.yaml
--rw-r--r--   0        0        0      158 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/services/test_service.yaml
--rw-r--r--   0        0        0      377 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/services/update_service.yaml
--rw-r--r--   0        0        0      192 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/webapps/create_or_update_webapp.yaml
--rw-r--r--   0        0        0      208 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/webapps/create_webapp.yaml
--rw-r--r--   0        0        0      199 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/webapps/update_webapp.yaml
--rw-r--r--   0        0        0      556 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/workflows/create_or_update_workflow.yaml
--rw-r--r--   0        0        0     1011 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/workflows/create_workflow.yaml
--rw-r--r--   0        0        0      237 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/workflows/execute_partial_workflow.yaml
--rw-r--r--   0        0        0      160 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/workflows/execute_workflow.yaml
--rw-r--r--   0        0        0      385 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/workflows/patch_workflow.yaml
--rw-r--r--   0        0        0      567 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/workflows/update_workflow.yaml
--rw-r--r--   0        0        0      849 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/workflows/workflow_auto_retry.yaml
--rw-r--r--   0        0        0     1229 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/workflows/workflow_execution_parameters.yaml
--rw-r--r--   0        0        0      457 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/workflows/workflow_input_parameters.yaml
--rw-r--r--   0        0        0      536 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/workflows/workflow_output_parameters.yaml
--rw-r--r--   0        0        0      680 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/sample_yaml/resources/workflows/workflow_skippable_steps.yaml
--rw-r--r--   0        0        0    10157 2024-03-20 08:11:26.582270 peak_sdk-1.5.0/peak/session.py
--rw-r--r--   0        0        0     7113 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/telemetry.py
--rw-r--r--   0        0        0     9758 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/template.py
--rw-r--r--   0        0        0     1048 2024-03-20 08:10:50.006284 peak_sdk-1.5.0/peak/tools/__init__.py
--rw-r--r--   0        0        0    10936 2024-03-20 08:10:50.010284 peak_sdk-1.5.0/peak/tools/logging/__init__.py
--rw-r--r--   0        0        0     1406 2024-03-20 08:10:50.010284 peak_sdk-1.5.0/peak/tools/logging/log_handler.py
--rw-r--r--   0        0        0     1770 2024-03-20 08:10:50.010284 peak_sdk-1.5.0/peak/tools/logging/log_level.py
--rw-r--r--   0        0        0     3330 2024-03-20 08:10:50.010284 peak_sdk-1.5.0/peak/tools/logging/utils.py
--rw-r--r--   0        0        0     2715 2024-03-20 08:11:26.582270 peak_sdk-1.5.0/peak/validators.py
--rw-r--r--   0        0        0     5696 2024-03-20 08:11:26.582270 peak_sdk-1.5.0/pypi-home.md
--rw-r--r--   0        0        0     5395 2024-03-20 08:11:26.582270 peak_sdk-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     7121 1970-01-01 00:00:00.000000 peak_sdk-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11340 2024-05-17 11:51:12.665849 peak_sdk-1.6.0/LICENSE
+-rw-r--r--   0        0        0     1263 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/__init__.py
+-rw-r--r--   0        0        0    24458 2024-05-17 11:51:48.810555 peak_sdk-1.6.0/peak/_metadata.py
+-rw-r--r--   0        0        0      886 2024-05-17 11:51:48.810555 peak_sdk-1.6.0/peak/_version.py
+-rw-r--r--   0        0        0      904 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/auth.py
+-rw-r--r--   0        0        0     1808 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/base_client.py
+-rw-r--r--   0        0        0     2486 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/callbacks.py
+-rw-r--r--   0        0        0      859 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/cli/__init_.py
+-rw-r--r--   0        0        0     5720 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/cli/args.py
+-rw-r--r--   0        0        0     2445 2024-05-17 11:51:48.810555 peak_sdk-1.6.0/peak/cli/cli.py
+-rw-r--r--   0        0        0     8286 2024-05-17 11:51:48.810555 peak_sdk-1.6.0/peak/cli/helpers.py
+-rw-r--r--   0        0        0      898 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/cli/press/__init__.py
+-rw-r--r--   0        0        0     1459 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/cli/press/apps/__init__.py
+-rw-r--r--   0        0        0    15895 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/cli/press/apps/deployments.py
+-rw-r--r--   0        0        0    15566 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/cli/press/apps/specs.py
+-rw-r--r--   0        0        0     1499 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/cli/press/blocks/__init__.py
+-rw-r--r--   0        0        0    20260 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/cli/press/blocks/deployments.py
+-rw-r--r--   0        0        0    29539 2024-05-17 11:51:48.810555 peak_sdk-1.6.0/peak/cli/press/blocks/specs.py
+-rw-r--r--   0        0        0     2834 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/cli/press/deployments.py
+-rw-r--r--   0        0        0     4811 2024-05-17 11:51:48.810555 peak_sdk-1.6.0/peak/cli/press/specs.py
+-rw-r--r--   0        0        0      883 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/cli/resources/__init__.py
+-rw-r--r--   0        0        0     1197 2024-05-17 11:51:48.810555 peak_sdk-1.6.0/peak/cli/resources/alerts/__init__.py
+-rw-r--r--   0        0        0    12062 2024-05-17 11:51:48.810555 peak_sdk-1.6.0/peak/cli/resources/alerts/emails.py
+-rw-r--r--   0        0        0    12383 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/cli/resources/artifacts.py
+-rw-r--r--   0        0        0    43098 2024-05-17 11:51:48.810555 peak_sdk-1.6.0/peak/cli/resources/images.py
+-rw-r--r--   0        0        0    24546 2024-05-17 11:51:48.810555 peak_sdk-1.6.0/peak/cli/resources/services.py
+-rw-r--r--   0        0        0     2624 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/cli/resources/tenants.py
+-rw-r--r--   0        0        0     2628 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/cli/resources/users.py
+-rw-r--r--   0        0        0    21349 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/cli/resources/webapps.py
+-rw-r--r--   0        0        0    52731 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/cli/resources/workflows.py
+-rw-r--r--   0        0        0      267 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/cli/ruff.toml
+-rw-r--r--   0        0        0     1654 2024-05-17 11:51:12.669849 peak_sdk-1.6.0/peak/cli/version.py
+-rw-r--r--   0        0        0     7442 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/compression.py
+-rw-r--r--   0        0        0     1146 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/config.py
+-rw-r--r--   0        0        0     3312 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/constants.py
+-rw-r--r--   0        0        0     6965 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/exceptions.py
+-rw-r--r--   0        0        0    14782 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/handler.py
+-rw-r--r--   0        0        0     8781 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/helpers.py
+-rw-r--r--   0        0        0     1548 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/logger.py
+-rw-r--r--   0        0        0     6180 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/output.py
+-rw-r--r--   0        0        0     1112 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/press/__init__.py
+-rw-r--r--   0        0        0    41911 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/press/apps.py
+-rw-r--r--   0        0        0    59175 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/press/blocks.py
+-rw-r--r--   0        0        0     5934 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/press/deployments.py
+-rw-r--r--   0        0        0    10915 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/press/specs.py
+-rw-r--r--   0        0        0        0 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/py.typed
+-rw-r--r--   0        0        0     1207 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/resources/__init__.py
+-rw-r--r--   0        0        0    12370 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/resources/alerts.py
+-rw-r--r--   0        0        0    14365 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/resources/artifacts.py
+-rw-r--r--   0        0        0    37186 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/resources/images.py
+-rw-r--r--   0        0        0    16910 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/resources/services.py
+-rw-r--r--   0        0        0     2936 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/resources/tenants.py
+-rw-r--r--   0        0        0     3428 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/resources/users.py
+-rw-r--r--   0        0        0    13719 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/resources/webapps.py
+-rw-r--r--   0        0        0    52753 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/resources/workflows.py
+-rw-r--r--   0        0        0      996 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/press/apps/deployments/create_app_deployment.yaml
+-rw-r--r--   0        0        0      688 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/press/apps/deployments/create_app_deployment_revision.yaml
+-rw-r--r--   0        0        0      302 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/press/apps/deployments/update_app_deployment_metadata.yaml
+-rw-r--r--   0        0        0      585 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/press/apps/specs/create_app_spec.yaml
+-rw-r--r--   0        0        0      250 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/press/apps/specs/create_app_spec_release.yaml
+-rw-r--r--   0        0        0      337 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/press/apps/specs/update_app_spec_metadata.yaml
+-rw-r--r--   0        0        0      729 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/press/blocks/deployments/create_block_deployment.yaml
+-rw-r--r--   0        0        0      376 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/press/blocks/deployments/create_block_deployment_revision.yaml
+-rw-r--r--   0        0        0      156 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/press/blocks/deployments/patch_block_parameters.yaml
+-rw-r--r--   0        0        0      304 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/press/blocks/deployments/update_block_deployment_metadata.yaml
+-rw-r--r--   0        0        0     2946 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/press/blocks/specs/create_block_spec.yaml
+-rw-r--r--   0        0        0     2590 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/press/blocks/specs/create_block_spec_release.yaml
+-rw-r--r--   0        0        0      378 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/press/blocks/specs/update_block_spec_metadata.yaml
+-rw-r--r--   0        0        0      152 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/artifacts/create_artifact.yaml
+-rw-r--r--   0        0        0      104 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/artifacts/create_artifact_version.yaml
+-rw-r--r--   0        0        0       99 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/artifacts/update_artifact_metadata.yaml
+-rw-r--r--   0        0        0      256 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/sample_yaml/resources/emails/send_email.yaml
+-rw-r--r--   0        0        0      343 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/images/dockerfile/create_image.yaml
+-rw-r--r--   0        0        0      310 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/images/dockerfile/create_image_version.yaml
+-rw-r--r--   0        0        0      275 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/images/dockerfile/update_version.yaml
+-rw-r--r--   0        0        0      396 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/images/github/create_image.yaml
+-rw-r--r--   0        0        0      369 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/images/github/create_image_version.yaml
+-rw-r--r--   0        0        0      338 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/images/github/update_version.yaml
+-rw-r--r--   0        0        0      390 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/images/upload/create_image.yaml
+-rw-r--r--   0        0        0      395 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/images/upload/create_image_version.yaml
+-rw-r--r--   0        0        0      414 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/images/upload/create_or_update_image.yaml
+-rw-r--r--   0        0        0      321 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/images/upload/update_version.yaml
+-rw-r--r--   0        0        0      428 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/sample_yaml/resources/services/create_or_update_service.yaml
+-rw-r--r--   0        0        0      428 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/sample_yaml/resources/services/create_service.yaml
+-rw-r--r--   0        0        0      158 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/services/test_service.yaml
+-rw-r--r--   0        0        0      395 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/sample_yaml/resources/services/update_service.yaml
+-rw-r--r--   0        0        0      192 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/webapps/create_or_update_webapp.yaml
+-rw-r--r--   0        0        0      208 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/webapps/create_webapp.yaml
+-rw-r--r--   0        0        0      199 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/webapps/update_webapp.yaml
+-rw-r--r--   0        0        0     1188 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/sample_yaml/resources/workflows/create_or_update_workflow.yaml
+-rw-r--r--   0        0        0     1230 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/sample_yaml/resources/workflows/create_workflow.yaml
+-rw-r--r--   0        0        0      237 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/workflows/execute_partial_workflow.yaml
+-rw-r--r--   0        0        0      160 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/workflows/execute_workflow.yaml
+-rw-r--r--   0        0        0     1017 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/sample_yaml/resources/workflows/patch_workflow.yaml
+-rw-r--r--   0        0        0     1199 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/sample_yaml/resources/workflows/update_workflow.yaml
+-rw-r--r--   0        0        0      849 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/workflows/workflow_auto_retry.yaml
+-rw-r--r--   0        0        0     1229 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/workflows/workflow_execution_parameters.yaml
+-rw-r--r--   0        0        0      457 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/workflows/workflow_input_parameters.yaml
+-rw-r--r--   0        0        0      536 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/workflows/workflow_output_parameters.yaml
+-rw-r--r--   0        0        0      680 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/sample_yaml/resources/workflows/workflow_skippable_steps.yaml
+-rw-r--r--   0        0        0    10157 2024-05-17 11:51:12.673849 peak_sdk-1.6.0/peak/session.py
+-rw-r--r--   0        0        0     7086 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/telemetry.py
+-rw-r--r--   0        0        0     9798 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/template.py
+-rw-r--r--   0        0        0     1048 2024-05-17 11:51:12.677849 peak_sdk-1.6.0/peak/tools/__init__.py
+-rw-r--r--   0        0        0     1513 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/tools/logging/__init__.py
+-rw-r--r--   0        0        0     1406 2024-05-17 11:51:12.677849 peak_sdk-1.6.0/peak/tools/logging/log_handler.py
+-rw-r--r--   0        0        0     2665 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/tools/logging/log_level.py
+-rw-r--r--   0        0        0    15653 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/peak/tools/logging/logger.py
+-rw-r--r--   0        0        0     3330 2024-05-17 11:51:12.677849 peak_sdk-1.6.0/peak/tools/logging/utils.py
+-rw-r--r--   0        0        0     2715 2024-05-17 11:51:12.677849 peak_sdk-1.6.0/peak/validators.py
+-rw-r--r--   0        0        0     5696 2024-05-17 11:51:12.677849 peak_sdk-1.6.0/pypi-home.md
+-rw-r--r--   0        0        0     5739 2024-05-17 11:51:48.814555 peak_sdk-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7044 1970-01-01 00:00:00.000000 peak_sdk-1.6.0/PKG-INFO
```

### Comparing `peak_sdk-1.5.0/LICENSE` & `peak_sdk-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/__init__.py` & `peak_sdk-1.6.0/peak/__init__.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/_metadata.py` & `peak_sdk-1.6.0/peak/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,21 +20,22 @@
 #
 """Contains the metadata for all the commands.
 
 The metadata represents the following:
     - table_params: Parameters required for the table output formatting.
     - request_body_yaml_path: File containing the yaml file examples for the command.
 """
+
+from __future__ import annotations
+
 from typing import Any, Dict, List
 
 
 def tag_parser(data: Any) -> str:
-    tag_array = []
-    for tag in data:
-        tag_array.append(tag["name"])
+    tag_array = [tag["name"] for tag in data]
     return ", ".join(tag_array)
 
 
 command_metadata: Dict[str, Any] = {
     "list_images": {
         "table_params": {
             "output_keys": {
@@ -619,14 +620,65 @@
                     "label": "Provider",
                 },
             },
             "title": "Instance Options",
             "data_key": "data",
         },
     },
+    "list_emails": {
+        "table_params": {
+            "output_keys": {
+                "id": {
+                    "label": "ID",
+                },
+                "subject": {
+                    "label": "Subject",
+                },
+                "status": {
+                    "label": "Status",
+                },
+                "templateName": {
+                    "label": "Template Name",
+                },
+                "createdAt": {
+                    "label": "Created At",
+                },
+                "createdBy": {
+                    "label": "Created By",
+                },
+            },
+            "title": "Emails",
+            "data_key": "emails",
+            "subheader_key": "emailCount",
+        },
+    },
+    "list_templates": {
+        "table_params": {
+            "output_keys": {
+                "id": {
+                    "label": "ID",
+                },
+                "name": {
+                    "label": "Name",
+                },
+                "scope": {
+                    "label": "Status",
+                },
+                "createdAt": {
+                    "label": "Created At",
+                },
+                "createdBy": {
+                    "label": "Created By",
+                },
+            },
+            "title": "Templates",
+            "data_key": "templates",
+            "subheader_key": "templateCount",
+        },
+    },
     "create_artifact": {
         "request_body_yaml_path": "sample_yaml/resources/artifacts/create_artifact.yaml",
     },
     "update_artifact_metadata": {
         "request_body_yaml_path": "sample_yaml/resources/artifacts/update_artifact_metadata.yaml",
     },
     "create_artifact_version": {
@@ -676,14 +728,17 @@
     },
     "create_or_update_service": {
         "request_body_yaml_path": "sample_yaml/resources/services/create_or_update_service.yaml",
     },
     "test_service": {
         "request_body_yaml_path": "sample_yaml/resources/services/test_service.yaml",
     },
+    "send_email": {
+        "request_body_yaml_path": "sample_yaml/resources/emails/send_email.yaml",
+    },
     "create_app_spec": {
         "request_body_yaml_path": "sample_yaml/press/apps/specs/create_app_spec.yaml",
     },
     "update_app_spec_metadata": {
         "request_body_yaml_path": "sample_yaml/press/apps/specs/update_app_spec_metadata.yaml",
     },
     "create_app_spec_release": {
```

### Comparing `peak_sdk-1.5.0/peak/_version.py` & `peak_sdk-1.6.0/peak/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # #
 # # This file is part of the peak-sdk.
 # # see (https://github.com/PeakBI/peak-sdk)
 # #
 # # You should have received a copy of the APACHE LICENSE, VERSION 2.0
 # # along with this program. If not, see <https://apache.org/licenses/LICENSE-2.0>
 #
-__version__: str = "1.5.0"
+__version__: str = "1.6.0"
```

### Comparing `peak_sdk-1.5.0/peak/auth.py` & `peak_sdk-1.6.0/peak/auth.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/base_client.py` & `peak_sdk-1.6.0/peak/base_client.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/callbacks.py` & `peak_sdk-1.6.0/peak/callbacks.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/cli/__init_.py` & `peak_sdk-1.6.0/peak/cli/__init_.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/cli/args.py` & `peak_sdk-1.6.0/peak/cli/args.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/cli/cli.py` & `peak_sdk-1.6.0/peak/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,23 +21,24 @@
 """CLI entrypoint."""
 import sys
 
 import peak.config
 import typer
 from peak.cli import args, helpers
 from peak.cli.press import apps, blocks, deployments, specs
-from peak.cli.resources import artifacts, images, services, tenants, users, webapps, workflows
+from peak.cli.resources import alerts, artifacts, images, services, tenants, users, webapps, workflows
 from peak.constants import Sources
 from peak.output import Writer
 
-# Hack to not gray out texts after first paragraph
+# Workaround to not gray out texts after first paragraph
 typer.rich_utils.STYLE_HELPTEXT = ""
 
 typer_app = typer.Typer(rich_markup_mode="markdown", help="Create and Manage Peak Resources")
 typer_app.add_typer(images.app, name="images")
+typer_app.add_typer(alerts.app, name="alerts")
 typer_app.add_typer(artifacts.app, name="artifacts")
 typer_app.add_typer(workflows.app, name="workflows")
 typer_app.add_typer(webapps.app, name="webapps")
 typer_app.add_typer(services.app, name="services")
 typer_app.add_typer(tenants.app, name="tenants")
 typer_app.add_typer(apps.app, name="apps")
 typer_app.add_typer(blocks.app, name="blocks")
```

### Comparing `peak_sdk-1.5.0/peak/cli/helpers.py` & `peak_sdk-1.6.0/peak/cli/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,9 +248,10 @@
         "artifacts": resources.artifacts,
         "images": resources.images,
         "workflows": resources.workflows,
         "services": resources.services,
         "webapps": resources.webapps,
         "tenants": resources.tenants,
         "users": resources.users,
+        "alerts": resources.alerts,
     }
     return command_client_map[command].get_client()  # type: ignore[no-any-return]
```

### Comparing `peak_sdk-1.5.0/peak/cli/press/__init__.py` & `peak_sdk-1.6.0/peak/cli/press/__init__.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/cli/press/apps/__init__.py` & `peak_sdk-1.6.0/peak/cli/press/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/cli/press/apps/deployments.py` & `peak_sdk-1.6.0/peak/cli/press/apps/deployments.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/cli/press/apps/specs.py` & `peak_sdk-1.6.0/peak/cli/press/apps/specs.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/cli/press/blocks/__init__.py` & `peak_sdk-1.6.0/peak/cli/press/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/cli/press/blocks/deployments.py` & `peak_sdk-1.6.0/peak/cli/press/blocks/deployments.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/cli/press/blocks/specs.py` & `peak_sdk-1.6.0/peak/cli/press/blocks/specs.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,15 @@
                 - cron (string | required: false): A valid cron expression.
                   webhook (boolean | required: false): Should be true if webhook type trigger is to be used.
                   webhookId (string | required: false): ID of the webhook.
             watchers (list(map) | required: false):
                 - events (map):
                     success (boolean | required: false): Whether to call event on success.
                     fail (boolean | required: false): Whether to call event on failure.
-                    runtimeExceeded (int | required: false): The runtime after which event is called.
+                    runtimeExceeded (int | required: false): The runtime in minutes after which event is called.
                   user (string | required: false): User to be notified. To be added in case of user watcher.
                   webhook (map | required: false): To be added in case of webhook watcher.
                     name (string): Name of the webhook.
                     url (string): URL of the webhook.
                     payload (string): Webhook payload.
             image (map | required: false):  # To be used only in case of webapp block.
                 version (string | required: false): A valid semantic image version.
@@ -429,15 +429,15 @@
                 cron (string | required: false): A valid cron expression.
                 webhook (boolean | required: false): Should be true if webhook type trigger is to be used.
                 webhookId (string | required: false): ID of the webhook.
             watchers (list(map) | required: false):
                 - events (map):
                     success (boolean | required: false): Whether to call event on success.
                     fail (boolean | required: false): Whether to call event on failure.
-                    runtimeExceeded (int | required: false): The runtime after which event is called.
+                    runtimeExceeded (int | required: false): The runtime in minutes after which event is called.
                   user (string | required: false): User to be notified. To be added in case of user watcher.
                   webhook (map | required: false): To be added in case of webhook watcher.
                     name (string): Name of the webhook.
                     url (string): URL of the webhook.
                     payload (string): Webhook payload.
             image (map | required: false):  # To be used only in case of webapp block.
                 version (string | required: false): A valid semantic image version.
```

### Comparing `peak_sdk-1.5.0/peak/cli/press/deployments.py` & `peak_sdk-1.6.0/peak/cli/press/deployments.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/cli/press/specs.py` & `peak_sdk-1.6.0/peak/cli/press/specs.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 
 app = typer.Typer(
     help="Manage both Block and App specs.",
     short_help="Manage both Block and App specs.",
 )
 console = Console()
 
+RELEASE_VERSION = typer.Option(None, help="The release version of the spec in valid semantic versioning format.")
+
 
 @app.command("list", short_help="List App and Block specs.", options_metavar="list_specs")
 def list_specs(
     ctx: typer.Context,
     page_size: Optional[int] = args.PAGE_SIZE,
     page_number: Optional[int] = args.PAGE_NUMBER,
     status: Optional[List[str]] = args.STATUS_FILTER_SPECS,
@@ -90,25 +92,25 @@
         writer.write(response)
 
 
 @app.command(short_help="List deployments for a spec release.", options_metavar="list_release_deployments")
 def list_release_deployments(
     ctx: typer.Context,
     spec_id: str = args.SPEC_ID,
-    version: str = args.RELEASE_VERSION,
+    version: Optional[str] = RELEASE_VERSION,
     page_size: Optional[int] = args.PAGE_SIZE,
     page_number: Optional[int] = args.PAGE_NUMBER,
     status: Optional[List[str]] = args.STATUS_FILTER_SPEC_RELEASES,
     name: Optional[str] = args.NAME_FILTER,
     title: Optional[str] = args.TITLE_FILTER,
     sort: Optional[List[str]] = args.SORT_KEYS,
     paging: Optional[bool] = PAGING,  # noqa: ARG001
     output_type: Optional[OutputTypes] = OUTPUT_TYPES,  # noqa: ARG001
 ) -> None:
-    """***List*** all the deployments for a given spec release.
+    """***List*** all the deployments for a given spec. Version is optional and if not provided, all deployments for the spec will be returned.
 
     \b
     📝 ***Example usage:***<br/>
     ```bash
     peak specs list-release-deployments --spec-id "632a4e7c-ab86-4ecb-8f34-99b5da531ceb" --status deployed,failed --version 1.0.0
     ```
```

### Comparing `peak_sdk-1.5.0/peak/cli/resources/__init__.py` & `peak_sdk-1.6.0/peak/cli/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/cli/resources/artifacts.py` & `peak_sdk-1.6.0/peak/cli/resources/artifacts.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/cli/resources/images.py` & `peak_sdk-1.6.0/peak/cli/resources/images.py`

 * *Files 0% similar despite different names*

```diff
@@ -1082,8 +1082,8 @@
                 formatted_logs = helpers.format_logs(response["logs"])
                 if len(formatted_logs):
                     writer.write(formatted_logs)
             else:
                 writer.write(response)
                 break
 
-            next_token = response["nextToken"] if "nextToken" in response else None
+            next_token = response.get("nextToken", None)
```

### Comparing `peak_sdk-1.5.0/peak/cli/resources/services.py` & `peak_sdk-1.6.0/peak/cli/resources/services.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,19 @@
 
 _SECRETS = typer.Option(None, help="List of secret names to be passed as environment variables.")
 
 _ENTRYPOINT = typer.Option(None, help="Entrypoint for the service.")
 
 _HEALTH_CHECK_URL = typer.Option(None, help="Endpoint to monitor service's operational status.")
 
+_MIN_INSTANCES = typer.Option(
+    None,
+    help="Minimum number of instances that would run for a service. Default value is 1 and maximum value allowed is 2.",
+)
+
 _HTTP_METHOD = typer.Option(None, help="HTTP method to be used to test the service.")
 
 _PATH = typer.Option(None, help="Path to be used to test the service.")
 
 _PAYLOAD = typer.Option(None, help="Payload to be used to test the service. To be passed in stringified json format.")
 
 MAPPING = {
@@ -164,14 +169,15 @@
     instance_type_id: int = INSTANCE_TYPE_ID,
     session_stickiness: bool = SESSION_STICKINESS,
     service_type: Optional[str] = _SERVICE_TYPE,
     env: Optional[List[str]] = _ENVS,
     secrets: Optional[List[str]] = _SECRETS,
     entrypoint: Optional[str] = _ENTRYPOINT,
     health_check_url: Optional[str] = _HEALTH_CHECK_URL,
+    min_instances: Optional[int] = _MIN_INSTANCES,
     dry_run: Optional[bool] = DRY_RUN,  # noqa: ARG001
     paging: Optional[bool] = PAGING,  # noqa: ARG001
     output_type: Optional[OutputTypesNoTable] = OUTPUT_TYPES,  # noqa: ARG001
     generate: Optional[bool] = GENERATE_YAML,  # noqa: ARG001
 ) -> None:
     """***Create*** a new service and start its deployment.
 
@@ -190,14 +196,15 @@
             instanceTypeId (number): ID of the instance type.
         parameters (map | required: false):
             env (map | required: false): Key-Value pair where key is the name of the env.
             secrets (list(str) | required: false): List of secret names to be passed.
         sessionStickiness (boolean | required: false): Enable session stickiness for the service. Default value is false. Enabling session stickiness will tie each user to a specific server for all their requests. Not required for API type services.
         entrypoint (string | required: false): Entrypoint for the service.
         healthCheckURL (string | required: false): Endpoint to monitor service's operational status.
+        minInstances (number | required: false): Minimum number of instances that would run for a service. Default value is 1 and maximum value allowed is 2.
     ```
 
     \b
     📝 ***Example usage:***
     ```bash
     peak services create '/path/to/file.yml' -v '/path/to/params.yml'
     ```
@@ -248,14 +255,17 @@
 
     if secrets:
         updated_body["parameters"]["secrets"] = parse_list_of_strings(secrets)
 
     if health_check_url:
         updated_body["healthCheckURL"] = health_check_url
 
+    if min_instances:
+        updated_body["minInstances"] = min_instances
+
     with writer.pager():
         response = service_client.create_service(body=updated_body)
         writer.write(response)
 
 
 @app.command(short_help="Update an existing service.", options_metavar="update_service")
 def update(
@@ -270,14 +280,15 @@
     version_id: int = VERSION_ID,
     instance_type_id: int = INSTANCE_TYPE_ID,
     session_stickiness: bool = SESSION_STICKINESS,
     env: Optional[List[str]] = _ENVS,
     secrets: Optional[List[str]] = _SECRETS,
     entrypoint: Optional[str] = _ENTRYPOINT,
     health_check_url: Optional[str] = _HEALTH_CHECK_URL,
+    min_instances: Optional[int] = _MIN_INSTANCES,
     dry_run: Optional[bool] = DRY_RUN,  # noqa: ARG001
     paging: Optional[bool] = PAGING,  # noqa: ARG001
     output_type: Optional[OutputTypesNoTable] = OUTPUT_TYPES,  # noqa: ARG001
     generate: Optional[bool] = GENERATE_YAML,  # noqa: ARG001
 ) -> None:
     """***Update*** an existing service.
 
@@ -301,14 +312,15 @@
             instanceTypeId (number): ID of the instance type.
         parameters (map | required: false):
             env (map | required: false): Key-Value pair where key is the name of the env.
             secrets (list(str) | required: false): List of secret names to be passed.
         sessionStickiness (boolean | required: false): Enable session stickiness for the service. Default value is false. Enabling session stickiness will tie each user to a specific server for all their requests. Not required for API type services.
         entrypoint (string | required: false): Entrypoint for the service.
         healthCheckURL (string | required: false): Endpoint to monitor service's operational status.
+        minInstances (number | required: false): Minimum number of instances that would run for a service. Default value is 1 and maximum value allowed is 2.
     ```
 
     \b
     📝 ***Example usage:***
     ```bash
     peak services update <service-id> '/path/to/file.yml' -v '/path/to/params.yml'
     ```
@@ -357,14 +369,17 @@
 
     if secrets:
         updated_body["parameters"]["secrets"] = parse_list_of_strings(secrets)
 
     if health_check_url:
         updated_body["healthCheckURL"] = health_check_url
 
+    if min_instances:
+        updated_body["minInstances"] = min_instances
+
     with writer.pager():
         response = service_client.update_service(service_id=service_id, body=updated_body)
         writer.write(response)
 
 
 @app.command(
     short_help="Create a new service or Update an existing service.",
@@ -383,14 +398,15 @@
     instance_type_id: int = INSTANCE_TYPE_ID,
     session_stickiness: bool = SESSION_STICKINESS,
     service_type: Optional[str] = _SERVICE_TYPE,
     env: Optional[List[str]] = _ENVS,
     secrets: Optional[List[str]] = _SECRETS,
     entrypoint: Optional[str] = _ENTRYPOINT,
     health_check_url: Optional[str] = _HEALTH_CHECK_URL,
+    min_instances: Optional[int] = _MIN_INSTANCES,
     dry_run: Optional[bool] = DRY_RUN,  # noqa: ARG001
     paging: Optional[bool] = PAGING,  # noqa: ARG001
     output_type: Optional[OutputTypesNoTable] = OUTPUT_TYPES,  # noqa: ARG001
     generate: Optional[bool] = GENERATE_YAML,  # noqa: ARG001
 ) -> None:
     """***Create*** a new service or ***Update*** an existing service based on service name and start its deployment.
 
@@ -414,14 +430,15 @@
             instanceTypeId (number): ID of the instance type.
         parameters (map | required: false):
             env (map | required: false): Key-Value pair where key is the name of the env.
             secrets (list(str) | required: false): List of secret names to be passed.
         sessionStickiness (boolean | required: false): Enable session stickiness for the service. Default value is false. Enabling session stickiness will tie each user to a specific server for all their requests. Not required for API type services.
         entrypoint (string | required: false): Entrypoint for the service.
         healthCheckURL (string | required: false): Endpoint to monitor service's operational status.
+        minInstances (number | required: false): Minimum number of instances that would run for a service. Default value is 1 and maximum value allowed is 2.
     ```
 
     \b
     📝 ***Example usage:***
     ```bash
     peak services create-or-update '/path/to/file.yml' -v '/path/to/params.yml'
     ```
@@ -474,14 +491,17 @@
 
     if secrets:
         updated_body["parameters"]["secrets"] = parse_list_of_strings(secrets)
 
     if health_check_url:
         updated_body["healthCheckURL"] = health_check_url
 
+    if min_instances:
+        updated_body["minInstances"] = min_instances
+
     response = service_client.create_or_update_service(body=updated_body)
     writer.write(response)
 
 
 @app.command(short_help="Delete an existing service.", options_metavar="delete_service")
 def delete(
     ctx: typer.Context,
@@ -547,14 +567,17 @@
             "instanceTypeId": 1
         },
         "sessionStickiness": false,
         "createdAt": "2020-01-01T18:00:00.000Z",
         "createdBy": "someone@peak.ai",
         "updatedAt": "2020-01-01T18:00:00.000Z",
         "updatedBy": "someone@peak.ai",
+        "entrypoint": "/",
+        "healthCheckURL": "/health",
+        "minInstances": 1,
         "tags": [...]
     }
     ```
 
     🔗 [**API Documentation**](https://service.peak.ai/webapps/api-docs/index.htm#/Services/get-service)
     """
     service_client: Service = ctx.obj["client"]
```

### Comparing `peak_sdk-1.5.0/peak/cli/resources/tenants.py` & `peak_sdk-1.6.0/peak/cli/resources/tenants.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/cli/resources/users.py` & `peak_sdk-1.6.0/peak/cli/resources/users.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/cli/resources/webapps.py` & `peak_sdk-1.6.0/peak/cli/resources/webapps.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/cli/resources/workflows.py` & `peak_sdk-1.6.0/peak/cli/resources/workflows.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,24 @@
 
 _STEP_TIMEOUT = typer.Option(None, help="The time after which the step timeouts.")
 
 _CLEAR_IMAGE_CACHE = typer.Option(None, help="Whether to clear image cache on workflow execution.")
 
 _STEP_NAMES = typer.Option(None, help="List of step names to be updated.")
 
+_EXECUTION_STATUS = typer.Option(
+    None,
+    help="List of workflow execution statuses. Valid values are `Success`, `Running`, `Stopped`, `Stopping` and `Failed`.",
+)
+
+_COUNT = typer.Option(
+    None,
+    help="Number of workflow executions required in the provided time range or 90 days. If not provided, all executions are returned.",
+)
+
 
 @app.command(short_help="Create a new workflow.", options_metavar="create_workflow")
 def create(
     ctx: typer.Context,
     file: str = args.TEMPLATE_PATH,
     params_file: str = args.TEMPLATE_PARAMS_FILE,
     params: List[str] = args.TEMPLATE_PARAMS,
@@ -106,20 +116,32 @@
         triggers (list(map) | required: false):
             - cron (string | required: false): A valid cron expression.
               webhook (boolean | required: false): Should be true if webhook type trigger is to be used.
         watchers (list(map) | required: false):
             - events (map):
                 success (boolean | required: false): Whether to call event on success.
                 fail (boolean | required: false): Whether to call event on success.
-                runtimeExceeded (int | required: false): The runtime after which event is called.
-              user (string | required: false): User to be notified.
-              webhook (map | required: false):
+                runtimeExceeded (int | required: false): The runtime in minutes after which event is called.
+              user (string): User to be notified.
+            - events (map):
+                success (boolean | required: false): Whether to call event on success.
+                fail (boolean | required: false): Whether to call event on success.
+                runtimeExceeded (int | required: false): The runtime in minutes after which event is called.
+              webhook (map):
                 name (string): Name of the webhook.
                 url (string): URL of the webhook.
                 payload (string): Webhook payload.
+            - events (map):
+                success (boolean | required: false): Whether to call event on success.
+                fail (boolean | required: false): Whether to call event on success.
+                runtimeExceeded (int | required: false): The runtime in minutes after which event is called.
+              email (map):
+                name (string): Name of the email watcher.
+                recipients (map):
+                    to (list(str)): List of email addresses to send the email to. Email can be sent only to the users who are added in the tenant.
         retryOptions (map | required: false): # Workflow level retry options which will be applied to all steps.
             duration (int | required: false): Duration in seconds after which the step is retried if it fails. Default is 5 seconds and maximum is 120 seconds.
             exitCodes (list(int) | required: false): List of exit codes for which the step is retried. If not provided, the step is retried for all exit codes.
             exponentialBackoff (boolean | required: false): Whether to use exponential backoff for retrying the step. If provided as true, the factor used will be 2.
             numberOfRetries (int | required: false): Number of times the step should be retried. Default is 3 and maximum is 5.
         steps(map):
             <stepName> (map): # Dictionary containing the step configuration. Here the key is name of the step.
@@ -218,20 +240,32 @@
         triggers (list(map) | required: false):
             - cron (string | required: false): A valid cron expression.
               webhook (boolean | required: false): Should be true if webhook type trigger is to be used.
         watchers (list(map) | required: false):
             - events (map):
                 success (boolean | required: false): Whether to call event on success.
                 fail (boolean | required: false): Whether to call event on success.
-                runtimeExceeded (int | required: false): The runtime after which event is called.
-              user (string | required: false): User to be notified.
-              webhook (map | required: false):
+                runtimeExceeded (int | required: false): The runtime in minutes after which event is called.
+              user (string): User to be notified.
+            - events (map):
+                success (boolean | required: false): Whether to call event on success.
+                fail (boolean | required: false): Whether to call event on success.
+                runtimeExceeded (int | required: false): The runtime in minutes after which event is called.
+              webhook (map):
                 name (string): Name of the webhook.
                 url (string): URL of the webhook.
                 payload (string): Webhook payload.
+            - events (map):
+                success (boolean | required: false): Whether to call event on success.
+                fail (boolean | required: false): Whether to call event on success.
+                runtimeExceeded (int | required: false): The runtime in minutes after which event is called.
+              email (map):
+                name (string): Name of the email watcher.
+                recipients (map):
+                    to (list(str)): List of email addresses to send the email to. Email can be sent only to the users who are added in the tenant.
         retryOptions (map | required: false): # Workflow level retry options which will be applied to all steps.
             duration (int | required: false): Duration in seconds after which the step is retried if it fails. Default is 5 seconds and maximum is 120 seconds.
             exitCodes (list(int) | required: false): List of exit codes for which the step is retried. If not provided, the step is retried for all exit codes.
             exponentialBackoff (boolean | required: false): Whether to use exponential backoff for retrying the step. If provided as true, the factor used will be 2.
             numberOfRetries (int | required: false): Number of times the step should be retried. Default is 3 and maximum is 5.
         steps(map):
             <stepName> (map): # Dictionary containing the step configuration. Here the key is name of the step.
@@ -330,20 +364,32 @@
         triggers (list(map) | required: false):
             - cron (string | required: false): A valid cron expression.
               webhook (boolean | required: false): Should be true if webhook type trigger is to be used.
         watchers (list(map) | required: false):
             - events (map):
                 success (boolean | required: false): Whether to call event on success.
                 fail (boolean | required: false): Whether to call event on success.
-                runtimeExceeded (int | required: false): The runtime after which event is called.
-              user (string | required: false): User to be notified.
-              webhook (map | required: false):
+                runtimeExceeded (int | required: false): The runtime in minutes after which event is called.
+              user (string): User to be notified.
+            - events (map):
+                success (boolean | required: false): Whether to call event on success.
+                fail (boolean | required: false): Whether to call event on success.
+                runtimeExceeded (int | required: false): The runtime in minutes after which event is called.
+              webhook (map):
                 name (string): Name of the webhook.
                 url (string): URL of the webhook.
                 payload (string): Webhook payload.
+            - events (map):
+                success (boolean | required: false): Whether to call event on success.
+                fail (boolean | required: false): Whether to call event on success.
+                runtimeExceeded (int | required: false): The runtime in minutes after which event is called.
+              email (map):
+                name (string): Name of the email watcher.
+                recipients (map):
+                    to (list(str)): List of email addresses to send the email to. Email can be sent only to the users who are added in the tenant.
         retryOptions (map | required: false): # Workflow level retry options which will be applied to all steps.
             duration (int | required: false): Duration in seconds after which the step is retried if it fails. Default is 5 seconds and maximum is 120 seconds.
             exitCodes (list(int) | required: false): List of exit codes for which the step is retried. If not provided, the step is retried for all exit codes.
             exponentialBackoff (boolean | required: false): Whether to use exponential backoff for retrying the step. If provided as true, the factor used will be 2.
             numberOfRetries (int | required: false): Number of times the step should be retried. Default is 3 and maximum is 5.
         steps(map):
             <stepName> (map): # Dictionary containing the step configuration. Here the key is name of the step.
@@ -472,20 +518,32 @@
         triggers (list(map) | required: false):
             - cron (string | required: false): A valid cron expression.
               webhook (boolean | required: false): Should be true if webhook type trigger is to be used.
         watchers (list(map) | required: false):
             - events (map):
                 success (boolean | required: false): Whether to call event on success.
                 fail (boolean | required: false): Whether to call event on success.
-                runtimeExceeded (int | required: false): The runtime after which event is called.
-              user (string | required: false): User to be notified.
-              webhook (map | required: false):
+                runtimeExceeded (int | required: false): The runtime in minutes after which event is called.
+              user (string): User to be notified.
+            - events (map):
+                success (boolean | required: false): Whether to call event on success.
+                fail (boolean | required: false): Whether to call event on success.
+                runtimeExceeded (int | required: false): The runtime in minutes after which event is called.
+              webhook (map):
                 name (string): Name of the webhook.
                 url (string): URL of the webhook.
                 payload (string): Webhook payload.
+            - events (map):
+                success (boolean | required: false): Whether to call event on success.
+                fail (boolean | required: false): Whether to call event on success.
+                runtimeExceeded (int | required: false): The runtime in minutes after which event is called.
+              email (map):
+                name (string): Name of the email watcher.
+                recipients (map):
+                    to (list(str)): List of email addresses to send the email to. Email can be sent only to the users who are added in the tenant.
         retryOptions (map | required: false): # Workflow level retry options which will be applied to all steps.
             duration (int | required: false): Duration in seconds after which the step is retried if it fails. Default is 5 seconds and maximum is 120 seconds.
             exitCodes (list(int) | required: false): List of exit codes for which the step is retried. If not provided, the step is retried for all exit codes.
             exponentialBackoff (boolean | required: false): Whether to use exponential backoff for retrying the step. If provided as true, the factor used will be 2.
             numberOfRetries (int | required: false): Number of times the step should be retried. Default is 3 and maximum is 5.
         steps(map):
             <stepName> (map): # Dictionary containing the step configuration. Here the key is name of the step.
@@ -595,15 +653,15 @@
     output_type: Optional[OutputTypes] = OUTPUT_TYPES,  # noqa: ARG001
 ) -> None:
     """***List*** all workflows that exist for the tenant.
 
     \b
     📝 ***Example usage:***<br/>
     ```bash
-    peak workflows list --page-size 10 --page-number 1 --workflow_status "Draft" --last_execution_status "Success" --last_modified_by "abc@peak.ai" --name "test"
+    peak workflows list --page-size 10 --page-number 1 --workflow-status "Draft" --last-execution-status "Success" --last-modified-by "abc@peak.ai" --name "test"
     ```
 
     \b
     🆗 ***Response:***
     ```
     {
         "pageCount": 1,
@@ -843,25 +901,27 @@
 
 @app.command(short_help="List executions for the given workflow.", options_metavar="list_workflow_executions")
 def list_executions(
     ctx: typer.Context,
     workflow_id: int = _WORKFLOW_ID,
     date_from: Optional[str] = args.DATE_FROM,
     date_to: Optional[str] = args.DATE_TO,
+    status: Optional[List[str]] = _EXECUTION_STATUS,
+    count: Optional[int] = _COUNT,
     page_size: Optional[int] = args.PAGE_SIZE,
     page_number: Optional[int] = args.PAGE_NUMBER,
     paging: Optional[bool] = PAGING,  # noqa: ARG001
     output_type: Optional[OutputTypes] = OUTPUT_TYPES,  # noqa: ARG001
 ) -> None:
     """***List*** executions for the given workflow.
 
     \b
     📝 ***Example usage:***<br/>
     ```bash
-    peak workflows list-executions 9999 --page-size 10 --page-number 1
+    peak workflows list-executions 9999 --page-size 10 --page-number 1 --status "Running" --status "Failed"
     ```
 
     \b
     🆗 ***Response:***
     ```
     {
         "executions": [...],
@@ -878,14 +938,16 @@
     writer: Writer = ctx.obj["writer"]
 
     with writer.pager():
         response = workflow_client.list_executions(
             workflow_id=workflow_id,
             date_from=date_from,
             date_to=date_to,
+            status=parse_list_of_strings(status),
+            count=count,
             page_size=page_size,
             page_number=page_number,
             return_iterator=False,
         )
         writer.write(response)
 
 
@@ -970,15 +1032,15 @@
                 formatted_logs = helpers.format_logs(response["logs"])
                 if len(formatted_logs):
                     writer.write(formatted_logs)
             else:
                 writer.write(response)
                 break
 
-            next_token = response["nextToken"] if "nextToken" in response else None
+            next_token = response.get("nextToken", None)
 
 
 @app.command(short_help="Get workflow execution details.", options_metavar="get_execution_details")
 def get_execution_details(
     ctx: typer.Context,
     workflow_id: int = _WORKFLOW_ID_OPTION,
     execution_id: str = _EXECUTION_ID,
```

### Comparing `peak_sdk-1.5.0/peak/cli/version.py` & `peak_sdk-1.6.0/peak/cli/version.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/compression.py` & `peak_sdk-1.6.0/peak/compression.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             for file in included_files:
                 zf.write(path_obj / file, file)
                 parent_directories.update(Path(file).parents)
                 if tmp_file.tell() > constants.MAX_ARTIFACT_SIZE_MB * constants.MB:
                     raise exceptions.FileLimitExceededException(constants.MAX_ARTIFACT_SIZE_MB)
 
             # include directories as API backend need directories explicitly included
-            relative_root_path = Path(".")
+            relative_root_path = Path()
             if relative_root_path in parent_directories:
                 parent_directories.remove(relative_root_path)
             for directory in parent_directories:
                 zf.write(path_obj / directory, directory)
 
         tmp_file.seek(0)
         yield tmp_file
@@ -188,15 +188,15 @@
         files (list[str]): List of file paths to process.
 
     Returns:
         dict[str, dict]: Nested dict file tree structure.
     """
     files_dict: dict[str, dict] = {}  # type: ignore[type-arg]
     for f in files:
-        components = os.path.normpath(f).split(os.sep)
+        components = Path(os.path.normpath(f)).parts
         current_dir = files_dict
         for directory in components[:-1]:
             if directory not in current_dir:
                 current_dir[directory] = {}
             current_dir = current_dir[directory]
         if components[-1] not in current_dir:
             current_dir[components[-1]] = {}
```

### Comparing `peak_sdk-1.5.0/peak/config.py` & `peak_sdk-1.6.0/peak/config.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/constants.py` & `peak_sdk-1.6.0/peak/constants.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/exceptions.py` & `peak_sdk-1.6.0/peak/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,19 @@
 from pathlib import Path
 from typing import Any, ClassVar, Dict, List, Optional, Tuple, Type
 
 
 class PeakBaseException(Exception):
     """Base exception class for the Peak SDK."""
 
-    ...
-
 
 class HttpExceptionsRegistryMeta(type):
     """Registry metaclass."""
 
-    REGISTRY: Dict[int, Any] = defaultdict(lambda: Exception)
+    REGISTRY: ClassVar[Dict[int, Any]] = defaultdict(lambda: Exception)
 
     def __new__(
         cls: "Type[HttpExceptionsRegistryMeta]",
         name: str,
         bases: Tuple[Any, ...],
         attrs: Dict[str, Any],
     ) -> HttpExceptionsRegistryMeta:
@@ -54,15 +52,15 @@
             bases (tuple): Tuple of the child class's inheritance tree
             attrs (dict): Name and value pairs of all the attributes defined in the child class
 
         Returns:
             HttpExceptionsRegistryMeta: the child class itself, forward annotated for type checking
         """
         new_cls: "HttpExceptionsRegistryMeta" = type.__new__(cls, name, bases, attrs)
-        status_code: Optional[int] = attrs.get("STATUS_CODE", None)
+        status_code: Optional[int] = attrs.get("STATUS_CODE")
         if status_code:
             cls.REGISTRY[status_code] = new_cls
         return new_cls
 
 
 class BaseHttpException(PeakBaseException, metaclass=HttpExceptionsRegistryMeta):
     """Base registry class for registering all exceptions."""
@@ -144,19 +142,19 @@
         error_message: str = f"{env_var} environment variable is not set or is empty."
         super().__init__(f"{error_message} {message}")
 
 
 class FileLimitExceededException(PeakBaseException):
     """Limits on the file are exceeded."""
 
-    def __init__(self, max_size: int | float, *, message: str = "", units: str = "MB") -> None:
+    def __init__(self, max_size: float, *, message: str = "", units: str = "MB") -> None:
         """Throw exception with custom message.
 
         Args:
-            max_size (int): Maximum size of the file.
+            max_size (float): Maximum size of the file.
             message (str): Additional message to add to exception.
             units (str): Units of the maximum size.
         """
         error_message: str = f"Compressed directory size is over {max_size}{units}."
         super().__init__(f"{error_message} {message}")
```

### Comparing `peak_sdk-1.5.0/peak/handler.py` & `peak_sdk-1.6.0/peak/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 OptionalSerializable = Optional[Serializable]
 writer = Writer(ignore_debug_mode=True)
 
 
 class HandlerRegistryMeta(type):
     """Metaclass for registering all types of Handler classes."""
 
-    REGISTRY: Dict[ContentType, BaseHandler] = {}
+    REGISTRY: ClassVar[Dict[ContentType, BaseHandler]] = {}
 
     def __new__(
         cls: "Type[HandlerRegistryMeta]",
         name: str,
         bases: Tuple[Any, ...],
         attrs: Dict[str, Any],
     ) -> HandlerRegistryMeta:
@@ -75,35 +75,33 @@
 
         Raises:
             TypeError: if the child class does not have a `CONTENT_TYPE` attribute
         """
         error_invalid_content_type: str = f"Invalid content type for {name} handler"
         new_cls: "HandlerRegistryMeta" = type.__new__(cls, name, bases, attrs)
 
-        content_type: Optional[ContentType] = attrs.get("CONTENT_TYPE", None)
+        content_type: Optional[ContentType] = attrs.get("CONTENT_TYPE")
         try:
             if content_type and ContentType(content_type):
                 cls.REGISTRY[content_type] = new_cls()
         except ValueError as err:
             raise TypeError(error_invalid_content_type) from err
         else:
             return new_cls
 
 
 class _CombinedMeta(HandlerRegistryMeta, ABCMeta):
     """Utility class for combining multiple meta-classes."""
 
-    ...
-
 
 class AuthRetrySession(requests.Session):
     """Session with extra sugar attached."""
 
     # used in testing, so we can modify the backoff_factor etc. to speed up the tests
-    _DEFAULT_RETRY_CONFIG: Dict[str, Any] = {
+    _DEFAULT_RETRY_CONFIG: ClassVar[Dict[str, Any]] = {
         "backoff_factor": 2,
         "total": 5,
         "status_forcelist": [500, 502, 503, 504],
     }
 
     def _add_retries(self, retry_config: Optional[Dict[str, Any]] = None) -> None:
         if retry_config is None:
```

### Comparing `peak_sdk-1.5.0/peak/helpers.py` & `peak_sdk-1.6.0/peak/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     Args:
         body (Dict[str, Any]): the object to be parsed
 
     Returns:
         Dict[str, str]: the parsed object
     """
-    return {key: (value if type(value) == str else json.dumps(value)) for (key, value) in body.items()}
+    return {key: (value if isinstance(value, str) else json.dumps(value)) for (key, value) in body.items()}
 
 
 def remove_keys(body: Dict[str, Any], keys: List[str]) -> Dict[str, Any]:
     """Removes given keys from a dictionary.
 
     Args:
         body (Dict[str, Any]): the object to be parsed
@@ -72,16 +72,15 @@
     """
     if stage == "prod":
         stage = ""
     elif stage == "latest":
         stage = "dev"
 
     domain: str = f"https://{subdomain}.{stage}.peak.ai"
-    domain = domain.replace("..", ".")  # for prod domain
-    return domain
+    return domain.replace("..", ".")  # for prod domain
 
 
 def parse_list_of_strings(param: List[str] | None) -> List[str] | None:
     """Split comma separated strings in the list and flatten that list.
 
     Args:
        param (List[str] | None): List of strings
@@ -109,15 +108,15 @@
         str: lower camel case string
     """
     parts = snake_case_string.split("_")
     return parts[0] + "".join(part.capitalize() for part in parts[1:])
 
 
 def variables_to_dict(*args: Any, frame: FrameType | None = None) -> Dict[str, str]:
-    """Converts arbitary variables to a dictonary.
+    """Converts arbitrary variables to a dictionary.
 
     Args:
         args (str|int): tuple of string|int variables
         frame (FrameType|None): Current Frame of caller
 
     Returns:
         Dict[str, str]: Dictionary containing key value pair of variables
@@ -139,30 +138,30 @@
 
 
 def combine_dictionaries(
     dict1: Dict[str, Any],
     dict2: Dict[str, Any],
     nested_keys_to_skip: Optional[List[str]] = [],  # noqa: B006
 ) -> Dict[str, Any]:
-    """Combines two dictonaries. Values for second dictonary have higer precedence.
+    """Combines two dictionaries. Values for second dictionary have higher precedence.
 
     Args:
         dict1 (Dict[str, Any]): dictionary 1
-        dict2 (Dict[str, Any]): dictonary 2
+        dict2 (Dict[str, Any]): dictionary 2
         nested_keys_to_skip (List[str] | None): Keys for which nested combining is not required.
 
     Returns:
         Dict[str, Any]: Combined dictionary
     """
     if not dict1:
         return dict2
 
     combined_dict = dict(dict1)
     for key in dict2:
-        if key in combined_dict and type(combined_dict[key]) is dict and key not in (nested_keys_to_skip or []):
+        if key in combined_dict and isinstance(combined_dict[key], dict) and key not in (nested_keys_to_skip or []):
             combined_dict[key] = combine_dictionaries(combined_dict[key], dict2[key])
         else:
             combined_dict[key] = dict2[key]
     return combined_dict
 
 
 def map_user_options(
@@ -174,20 +173,20 @@
 
     Args:
         user_options (Dict[str, Any]): Dictionary containing user inputs
         mapping (Dict[str, Any]): Mapping to be used for conversion
         dict_type_keys (List[str]): List of keys which have json type values
 
     Returns:
-        Dict[str, str]: Mappe dictionary
+        Dict[str, str]: Mapped dictionary
     """
     result: Dict[str, Any] = {}
     for key in user_options:
         if key in mapping:
-            nested_dict = result[mapping[key]] if mapping[key] in result else {}
+            nested_dict = result.get(mapping[key], {})
             nested_dict[key] = json.loads(user_options[key]) if key in dict_type_keys else user_options[key]
             result[mapping[key]] = nested_dict
         else:
             result[key] = json.loads(user_options[key]) if key in dict_type_keys else user_options[key]
     return result
```

### Comparing `peak_sdk-1.5.0/peak/logger.py` & `peak_sdk-1.6.0/peak/logger.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/output.py` & `peak_sdk-1.6.0/peak/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         if not len(data[params["data_key"]]):
             console.print(Panel(Text("No data to display.", justify="center")))
             return
 
         title = params["title"]
 
         if "subheader_key" in params and params["subheader_key"] in data:
-            subheader_title = "Total" if "subheader_title" not in params else params["subheader_title"]
+            subheader_title = params.get("subheader_title", "Total")
             title = f'{title} ({subheader_title} = {data[params["subheader_key"]]})'
 
         table = Table(
             expand=True,
             highlight=True,
             row_styles=["grey62", ""],
             header_style="bold cyan",
@@ -131,15 +131,15 @@
                 v = self.__get_data(val, key_details[0])
 
                 if not v:
                     v = "-"
                 elif "parser" in key_details[1]:
                     v = key_details[1]["parser"](v)
 
-                if isinstance(v, (dict, list)):  # noqa: UP038
+                if isinstance(v, (dict, list)):
                     parsed_value = json_highlighter(Text(json.dumps(v, indent=2), overflow="fold"))
                 else:
                     parsed_value = Text(str(v), overflow="fold")
 
                 parsed_values.append(parsed_value)
 
             table.add_row(*parsed_values)
```

### Comparing `peak_sdk-1.5.0/peak/press/__init__.py` & `peak_sdk-1.6.0/peak/press/__init__.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/press/apps.py` & `peak_sdk-1.6.0/peak/press/apps.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,32 +44,30 @@
         title: Optional[str] = None,
         sort: Optional[List[str]] = None,
         scope: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_specs(
         self,
         status: Optional[List[str]] = None,
         featured: Optional[bool] = None,
         name: Optional[str] = None,
         title: Optional[str] = None,
         sort: Optional[List[str]] = None,
         scope: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_specs(
         self,
         status: Optional[List[str]] = None,
         featured: Optional[bool] = None,
         name: Optional[str] = None,
         title: Optional[str] = None,
@@ -436,28 +434,26 @@
         self,
         spec_id: str,
         sort: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_spec_releases(
         self,
         spec_id: str,
         sort: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_spec_releases(
         self,
         spec_id: str,
         sort: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
@@ -591,29 +587,27 @@
         status: Optional[List[str]] = None,
         name: Optional[str] = None,
         sort: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_deployments(
         self,
         status: Optional[List[str]] = None,
         name: Optional[str] = None,
         sort: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_deployments(
         self,
         status: Optional[List[str]] = None,
         name: Optional[str] = None,
         sort: Optional[List[str]] = None,
         page_size: Optional[int] = None,
@@ -840,29 +834,27 @@
         deployment_id: str,
         sort: Optional[List[str]] = None,
         status: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_deployment_revisions(
         self,
         deployment_id: str,
         sort: Optional[List[str]] = None,
         status: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_deployment_revisions(
         self,
         deployment_id: str,
         sort: Optional[List[str]] = None,
         status: Optional[List[str]] = None,
         page_size: Optional[int] = None,
```

### Comparing `peak_sdk-1.5.0/peak/press/blocks.py` & `peak_sdk-1.6.0/peak/press/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,32 +48,30 @@
         title: Optional[str] = None,
         sort: Optional[List[str]] = None,
         scope: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_specs(
         self,
         status: Optional[List[str]] = None,
         featured: Optional[bool] = None,
         name: Optional[str] = None,
         title: Optional[str] = None,
         sort: Optional[List[str]] = None,
         scope: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_specs(
         self,
         status: Optional[List[str]] = None,
         featured: Optional[bool] = None,
         name: Optional[str] = None,
         title: Optional[str] = None,
@@ -578,28 +576,26 @@
         self,
         spec_id: str,
         sort: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_spec_releases(
         self,
         spec_id: str,
         sort: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_spec_releases(
         self,
         spec_id: str,
         sort: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
@@ -770,30 +766,28 @@
         name: Optional[str] = None,
         title: Optional[str] = None,
         sort: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_deployments(
         self,
         status: Optional[List[str]] = None,
         name: Optional[str] = None,
         title: Optional[str] = None,
         sort: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_deployments(
         self,
         status: Optional[List[str]] = None,
         name: Optional[str] = None,
         title: Optional[str] = None,
         sort: Optional[List[str]] = None,
@@ -1066,29 +1060,27 @@
         deployment_id: str,
         sort: Optional[List[str]] = None,
         status: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_deployment_revisions(
         self,
         deployment_id: str,
         sort: Optional[List[str]] = None,
         status: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_deployment_revisions(
         self,
         deployment_id: str,
         sort: Optional[List[str]] = None,
         status: Optional[List[str]] = None,
         page_size: Optional[int] = None,
```

### Comparing `peak_sdk-1.5.0/peak/press/deployments.py` & `peak_sdk-1.6.0/peak/press/deployments.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,30 +40,28 @@
         kind: Optional[str] = None,
         term: Optional[str] = None,
         sort: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_deployments(
         self,
         status: Optional[List[str]] = None,
         kind: Optional[str] = None,
         term: Optional[str] = None,
         sort: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_deployments(
         self,
         status: Optional[List[str]] = None,
         kind: Optional[str] = None,
         term: Optional[str] = None,
         sort: Optional[List[str]] = None,
```

### Comparing `peak_sdk-1.5.0/peak/press/specs.py` & `peak_sdk-1.6.0/peak/press/specs.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # # This file is part of the peak-sdk.
 # # see (https://github.com/PeakBI/peak-sdk)
 # #
 # # You should have received a copy of the APACHE LICENSE, VERSION 2.0
 # # along with this program. If not, see <https://apache.org/licenses/LICENSE-2.0>
 #
 """Specs client module."""
+
 from __future__ import annotations
 
 from typing import Any, Dict, Iterator, List, Literal, Optional, overload
 
 from peak.base_client import BaseClient
 from peak.constants import ContentType, HttpMethods
 from peak.session import Session
@@ -42,32 +43,30 @@
         term: Optional[str] = None,
         sort: Optional[List[str]] = None,
         scope: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_specs(
         self,
         status: Optional[List[str]] = None,
         featured: Optional[bool] = None,
         kind: Optional[str] = None,
         term: Optional[str] = None,
         sort: Optional[List[str]] = None,
         scope: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_specs(
         self,
         status: Optional[List[str]] = None,
         featured: Optional[bool] = None,
         kind: Optional[str] = None,
         term: Optional[str] = None,
@@ -140,63 +139,61 @@
             subdomain="press",
         )
 
     @overload
     def list_spec_release_deployments(
         self,
         spec_id: str,
-        version: str,
+        version: Optional[str],
         status: Optional[List[str]] = None,
         name: Optional[str] = None,
         title: Optional[str] = None,
         sort: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_spec_release_deployments(
         self,
         spec_id: str,
-        version: str,
+        version: Optional[str],
         status: Optional[List[str]] = None,
         name: Optional[str] = None,
         title: Optional[str] = None,
         sort: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_spec_release_deployments(
         self,
         spec_id: str,
-        version: str,
+        version: Optional[str],
         status: Optional[List[str]] = None,
         name: Optional[str] = None,
         title: Optional[str] = None,
         sort: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: bool = True,
     ) -> Iterator[Dict[str, Any]] | Dict[str, Any]:
         """Get all deployments of a App or Block spec release (ordered by most recently created to oldest).
 
         REFERENCE:
-            🔗 `API Documentation <https://press.peak.ai/api-docs/index.htm#/Specs/get_v1_specs__specId__releases__version__deployments>`__
+            🔗 `API Documentation <https://press.peak.ai/api-docs/index.htm#/Specs/get_v1_specs__specId__releases_deployments>`__
 
         Args:
             spec_id (str): The ID of the App or Block spec.
-            version (str): The release version of the spec in valid semantic versioning format.
+            version (str | None): The release version of the spec in valid semantic versioning format. If not provided, all deployments are returned.
             status (List[str] | None): List of statuses to filter deployments.
                 Valid values are `deleting`, `delete_failed`, `deployed`, `deploying`, `failed`, `platform_resource_error`, `redeploying`, `rollback`, `rollback_complete`, `rollback_failed` and `warning`.
             name (str | None): String to filter deployments by name.
             title (str | None): String to filter deployments by title.
             sort (List[str] | None): List of fields with desired ordering in the format `[<field>:<order>, ...]`,
                 where `order` is one of `['asc', 'desc']` and field is an ordered parameter within the response.
                 Valid fields are `createdAt`, `createdBy` and `name`.
@@ -214,21 +211,22 @@
             BadRequestException: The given parameters are invalid.
             UnauthorizedException: The credentials are invalid.
             ForbiddenException: The user does not have permission to perform the operation.
             NotFoundException: The given spec does not exist.
             InternalServerErrorException: the server encountered an unexpected condition that
                 prevented it from fulfilling the request.
         """
-        method, endpoint = HttpMethods.GET, f"{self.BASE_ENDPOINT}/{spec_id}/releases/{version}/deployments"
+        method, endpoint = HttpMethods.GET, f"{self.BASE_ENDPOINT}/{spec_id}/releases/deployments"
 
         params: Dict[str, Any] = {
             "status": status,
             "name": name,
             "title": title,
             "sort": sort,
+            "version": version,
             "pageSize": page_size,
         }
 
         if return_iterator:
             return self.session.create_generator_request(
                 endpoint,
                 method,
```

### Comparing `peak_sdk-1.5.0/peak/resources/__init__.py` & `peak_sdk-1.6.0/peak/resources/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # # This file is part of the peak-sdk.
 # # see (https://github.com/PeakBI/peak-sdk)
 # #
 # # You should have received a copy of the APACHE LICENSE, VERSION 2.0
 # # along with this program. If not, see <https://apache.org/licenses/LICENSE-2.0>
 #
 """This module exports all platform resources from the `Peak-Platform`."""
+
 from __future__ import annotations
 
 from typing import List
 
-from peak.resources import artifacts, images, services, tenants, users, webapps, workflows
+from peak.resources import alerts, artifacts, images, services, tenants, users, webapps, workflows
 
-__all__: List[str] = ["artifacts", "images", "services", "tenants", "users", "webapps", "workflows"]
+__all__: List[str] = ["alerts", "artifacts", "images", "services", "tenants", "users", "webapps", "workflows"]
```

### Comparing `peak_sdk-1.5.0/peak/resources/artifacts.py` & `peak_sdk-1.6.0/peak/resources/artifacts.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,26 +36,24 @@
     @overload
     def list_artifacts(
         self,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_artifacts(
         self,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_artifacts(
         self,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: bool = True,
```

### Comparing `peak_sdk-1.5.0/peak/resources/images.py` & `peak_sdk-1.6.0/peak/resources/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,31 +51,29 @@
         name: Optional[str] = None,
         status: Optional[List[str]] = None,
         scope: Optional[List[str]] = None,
         last_build_status: Optional[List[str]] = None,
         tags: Optional[List[str]] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_images(
         self,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         name: Optional[str] = None,
         status: Optional[List[str]] = None,
         scope: Optional[List[str]] = None,
         last_build_status: Optional[List[str]] = None,
         tags: Optional[List[str]] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_images(
         self,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         name: Optional[str] = None,
         status: Optional[List[str]] = None,
@@ -148,31 +146,29 @@
         page_number: Optional[int] = None,
         version: Optional[str] = None,
         status: Optional[List[str]] = None,
         last_build_status: Optional[List[str]] = None,
         tags: Optional[List[str]] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_image_versions(
         self,
         image_id: int,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         version: Optional[str] = None,
         status: Optional[List[str]] = None,
         last_build_status: Optional[List[str]] = None,
         tags: Optional[List[str]] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_image_versions(
         self,
         image_id: int,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         version: Optional[str] = None,
@@ -552,16 +548,16 @@
         Raises:
             BadRequestException: The given request parameters are invalid.
             UnauthorizedException: The credentials are invalid.
             ForbiddenException: The user does not have permission to perform the operation.
             PayloadTooLargeException: The artifact exceeds maximum size.
             InternalServerErrorException: The server failed to process the request.
         """
-        image_name = body["name"] if "name" in body else ""
-        version = body["version"] if "version" in body else ""
+        image_name = body.get("name", "")
+        version = body.get("version", "")
         response = (
             {} if not len(image_name) else self.list_images(page_size=100, return_iterator=False, name=image_name)
         )
         filtered_images = list(filter(lambda image: image.get("name", "") == image_name, response.get("images", [])))
 
         if len(filtered_images) > 0:
             image_id = filtered_images[0]["id"]
@@ -694,32 +690,30 @@
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         count: Optional[int] = None,
         version_ids: Optional[List[str]] = None,
         build_status: Optional[List[str]] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_image_builds(
         self,
         image_id: int,
         date_from: Optional[str] = None,
         date_to: Optional[str] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         count: Optional[int] = None,
         version_ids: Optional[List[str]] = None,
         build_status: Optional[List[str]] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_image_builds(
         self,
         image_id: int,
         date_from: Optional[str] = None,
         date_to: Optional[str] = None,
         page_size: Optional[int] = None,
```

### Comparing `peak_sdk-1.5.0/peak/resources/services.py` & `peak_sdk-1.6.0/peak/resources/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,29 +40,27 @@
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         status: Optional[List[str]] = None,
         name: Optional[str] = None,
         service_type: Optional[List[str]] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_services(
         self,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         status: Optional[List[str]] = None,
         name: Optional[str] = None,
         service_type: Optional[List[str]] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_services(
         self,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         status: Optional[List[str]] = None,
         name: Optional[str] = None,
@@ -151,15 +149,16 @@
                             "key: string": "value: string"
                         },
                         "secrets": []
                     },
                     "description": "string",
                     "sessionStickiness": "boolean. Not required for 'api' service type.",
                     "entrypoint": "string",
-                    "healthCheckURL": "string"
+                    "healthCheckURL": "string",
+                    "minInstances": "number. Default is 1 and maximum is 2",
                 }
 
         Raises:
             BadRequestException: The given request parameters are invalid.
             UnauthorizedException: The credentials are invalid.
             ForbiddenException: The user does not have permission to perform the operation.
             InternalServerErrorException: The server failed to process the request.
@@ -214,14 +213,15 @@
                         },
                         "secrets": []
                     },
                     "description": "string",
                     "sessionStickiness": "boolean. Not required for 'api' service type.",
                     "entrypoint": "string",
                     "healthCheckURL": "string",
+                    "minInstances": "number. Default is 1 and maximum is 2",
                 }
 
         Raises:
             BadRequestException: The given request parameters are invalid.
             UnauthorizedException: The credentials are invalid.
             ForbiddenException: The user does not have permission to perform the operation.
             NotFoundException: The given service does not exist.
@@ -272,24 +272,25 @@
                         },
                         "secrets": []
                     },
                     "description": "string",
                     "sessionStickiness": "boolean. Not required for 'api' service type.",
                     "entrypoint": "string",
                     "healthCheckURL": "string",
+                    "minInstances": "number. Default is 1 and maximum is 2",
                 }
 
 
         Raises:
             BadRequestException: The given request parameters are invalid.
             UnauthorizedException: The credentials are invalid.
             ForbiddenException: The user does not have permission to perform the operation.
             InternalServerErrorException: The server failed to process the request.
         """
-        service_name = body["name"] if "name" in body else ""
+        service_name = body.get("name", "")
         response = (
             {} if not len(service_name) else self.list_services(page_size=100, return_iterator=False, name=service_name)
         )
         filtered_services = list(
             filter(lambda service: service.get("name", "") == service_name, response.get("services", [])),
         )
```

### Comparing `peak_sdk-1.5.0/peak/resources/tenants.py` & `peak_sdk-1.6.0/peak/resources/tenants.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/resources/users.py` & `peak_sdk-1.6.0/peak/resources/users.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/resources/webapps.py` & `peak_sdk-1.6.0/peak/resources/webapps.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,28 +45,26 @@
         self,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         status: Optional[List[str]] = None,
         name: Optional[str] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_webapps(
         self,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         status: Optional[List[str]] = None,
         name: Optional[str] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_webapps(
         self,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         status: Optional[List[str]] = None,
         name: Optional[str] = None,
@@ -249,15 +247,15 @@
 
         Raises:
             BadRequestException: The given request parameters are invalid.
             UnauthorizedException: The credentials are invalid.
             ForbiddenException: The user does not have permission to perform the operation.
             InternalServerErrorException: The server failed to process the request.
         """
-        webapp_name = body["name"] if "name" in body else ""
+        webapp_name = body.get("name", "")
         response = (
             {} if not len(webapp_name) else self.list_webapps(page_size=100, return_iterator=False, name=webapp_name)
         )
         filtered_webapps = list(
             filter(lambda webapp: webapp.get("name", "") == webapp_name, response.get("webapps", [])),
         )
```

### Comparing `peak_sdk-1.5.0/peak/resources/workflows.py` & `peak_sdk-1.6.0/peak/resources/workflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # # This file is part of the peak-sdk.
 # # see (https://github.com/PeakBI/peak-sdk)
 # #
 # # You should have received a copy of the APACHE LICENSE, VERSION 2.0
 # # along with this program. If not, see <https://apache.org/licenses/LICENSE-2.0>
 #
 """Workflow client module."""
+
 from __future__ import annotations
 
 from typing import Any, Dict, Iterator, List, Literal, Optional, overload
 
 from peak.base_client import BaseClient
 from peak.constants import ContentType, HttpMethods
 from peak.exceptions import InvalidParameterException
@@ -47,30 +48,28 @@
         last_execution_status: Optional[List[str]] = None,
         last_modified_by: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         name: Optional[str] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_workflows(
         self: Workflow,
         workflow_status: Optional[List[str]] = None,
         last_execution_status: Optional[List[str]] = None,
         last_modified_by: Optional[List[str]] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         name: Optional[str] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_workflows(
         self: Workflow,
         workflow_status: Optional[List[str]] = None,
         last_execution_status: Optional[List[str]] = None,
         last_modified_by: Optional[List[str]] = None,
         page_size: Optional[int] = None,
@@ -162,18 +161,38 @@
                         {
                             "events": {
                                 "success": "boolean",
                                 "fail": "boolean",
                                 "runtimeExceeded": "number"
                             },
                             "user": "string",
+                        },
+                        {
+                            "events": {
+                                "success": "boolean",
+                                "fail": "boolean",
+                                "runtimeExceeded": "number"
+                            },
                             "webhook": {
                                 "name": "string(required)",
                                 "url": "string(required)",
-                                "payload": "string(required)",
+                                "payload": "string(required)"
+                            }
+                        },
+                        {
+                            "events": {
+                                "success": "boolean",
+                                "fail": "boolean",
+                                "runtimeExceeded": "number"
+                            },
+                            "email": {
+                                "name": "string",
+                                "recipients": {
+                                    "to": ["string"]
+                                }
                             }
                         }
                     ],
                     "retryOptions": {
                         "duration": "number",
                         "exitCodes": [],
                         "exponentialBackoff": "boolean",
@@ -291,18 +310,38 @@
                         {
                             "events": {
                                 "success": "boolean",
                                 "fail": "boolean",
                                 "runtimeExceeded": "number"
                             },
                             "user": "string",
+                        },
+                        {
+                            "events": {
+                                "success": "boolean",
+                                "fail": "boolean",
+                                "runtimeExceeded": "number"
+                            },
                             "webhook": {
                                 "name": "string(required)",
                                 "url": "string(required)",
-                                "payload": "string(required)",
+                                "payload": "string(required)"
+                            }
+                        },
+                        {
+                            "events": {
+                                "success": "boolean",
+                                "fail": "boolean",
+                                "runtimeExceeded": "number"
+                            },
+                            "email": {
+                                "name": "string",
+                                "recipients": {
+                                    "to": ["string"]
+                                }
                             }
                         }
                     ],
                     "retryOptions": {
                         "duration": "number",
                         "exitCodes": [],
                         "exponentialBackoff": "boolean",
@@ -378,15 +417,15 @@
 
         Raises:
             BadRequestException: The given request parameters are invalid.
             UnauthorizedException: The credentials are invalid.
             ForbiddenException: The user does not have permission to perform the operation.
             InternalServerErrorException: The server failed to process the request.
         """
-        workflow_name = body["name"] if "name" in body else ""
+        workflow_name = body.get("name", "")
         response = (
             {}
             if not len(workflow_name)
             else self.list_workflows(page_size=100, return_iterator=False, name=workflow_name)
         )
         filtered_workflows = list(
             filter(lambda workflow: workflow.get("name", "") == workflow_name, response.get("workflows", [])),
@@ -459,18 +498,38 @@
                         {
                             "events": {
                                 "success": "boolean",
                                 "fail": "boolean",
                                 "runtimeExceeded": "number"
                             },
                             "user": "string",
+                        },
+                        {
+                            "events": {
+                                "success": "boolean",
+                                "fail": "boolean",
+                                "runtimeExceeded": "number"
+                            },
                             "webhook": {
                                 "name": "string(required)",
                                 "url": "string(required)",
-                                "payload": "string(required)",
+                                "payload": "string(required)"
+                            }
+                        },
+                        {
+                            "events": {
+                                "success": "boolean",
+                                "fail": "boolean",
+                                "runtimeExceeded": "number"
+                            },
+                            "email": {
+                                "name": "string",
+                                "recipients": {
+                                    "to": ["string"]
+                                }
                             }
                         }
                     ],
                     "retryOptions": {
                         "duration": "number",
                         "exitCodes": [],
                         "exponentialBackoff": "boolean",
@@ -620,18 +679,38 @@
                         {
                             "events": {
                                 "success": "boolean",
                                 "fail": "boolean",
                                 "runtimeExceeded": "number"
                             },
                             "user": "string",
+                        },
+                        {
+                            "events": {
+                                "success": "boolean",
+                                "fail": "boolean",
+                                "runtimeExceeded": "number"
+                            },
                             "webhook": {
                                 "name": "string(required)",
                                 "url": "string(required)",
-                                "payload": "string(required)",
+                                "payload": "string(required)"
+                            }
+                        },
+                        {
+                            "events": {
+                                "success": "boolean",
+                                "fail": "boolean",
+                                "runtimeExceeded": "number"
+                            },
+                            "email": {
+                                "name": "string",
+                                "recipients": {
+                                    "to": ["string"]
+                                }
                             }
                         }
                     ],
                     "retryOptions": {
                         "duration": "number",
                         "exitCodes": [],
                         "exponentialBackoff": "boolean",
@@ -957,53 +1036,62 @@
 
     @overload
     def list_executions(
         self: Workflow,
         workflow_id: int,
         date_from: Optional[str] = None,
         date_to: Optional[str] = None,
+        status: Optional[List[str]] = None,
+        count: Optional[int] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[False],
-    ) -> Dict[str, Any]:
-        ...
+    ) -> Dict[str, Any]: ...
 
     @overload
     def list_executions(
         self: Workflow,
         workflow_id: int,
         date_from: Optional[str] = None,
         date_to: Optional[str] = None,
+        status: Optional[List[str]] = None,
+        count: Optional[int] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: Literal[True] = True,
-    ) -> Iterator[Dict[str, Any]]:
-        ...
+    ) -> Iterator[Dict[str, Any]]: ...
 
     def list_executions(
         self: Workflow,
         workflow_id: int,
         date_from: Optional[str] = None,
         date_to: Optional[str] = None,
+        status: Optional[List[str]] = None,
+        count: Optional[int] = None,
         page_size: Optional[int] = None,
         page_number: Optional[int] = None,
         *,
         return_iterator: bool = True,
     ) -> Iterator[Dict[str, Any]] | Dict[str, Any]:
         """Lists executions for the given workflow.
 
         REFERENCE:
             🔗 `API Documentation <https://service.peak.ai/workflows/api-docs/index.htm#/Executions/get-workflow-executions>`__
 
         Args:
             workflow_id (int): ID of the workflow to fetch executions.
             date_from (str | None): The date after which the executions should be included (in ISO format). Defaults to None
             date_to (str | None): The date till which the executions should be included (in ISO format). Defaults to None
+            status (List[str] | None): The status of the executions to filter by.
+                Valid values are `Success`, `Running`, `Stopped`, `Stopping` and `Failed`.
+            count (int | None): Number of executions required in the provided time range or 90 days (Ordered by latest to earliest).
+                For example, if 5 is provided, it will return last 5 workflow executions.
+                By default, it will return all the executions.
             page_size (int | None): Number of executions per page.
             page_number (int | None): Page number to fetch. Only used when return_iterator is False.
             return_iterator (bool): Whether to return an iterator object or list of executions for a specified page number, defaults to True.
 
         Returns:
             Iterator[Dict[str, Any]] | Dict[str, Any]: An iterator object which returns an element per iteration, until there are no more elements to return.
             If `return_iterator` is set to False, a dictionary containing the list and pagination details is returned instead.
@@ -1017,14 +1105,16 @@
             NotFoundException: The given workflow does not exist.
             InternalServerErrorException: The server failed to process the request.
             StopIteration: There are no more pages to list
         """
         method, endpoint = HttpMethods.GET, f"{self.BASE_ENDPOINT}/workflows/executions/{workflow_id}"
 
         params: Dict[str, Any] = {
+            "count": count,
+            "statuses": status,
             "dateTo": date_to,
             "dateFrom": date_from,
             "pageSize": page_size,
         }
 
         if return_iterator:
             return self.session.create_generator_request(
```

### Comparing `peak_sdk-1.5.0/peak/sample_yaml/press/apps/deployments/create_app_deployment.yaml` & `peak_sdk-1.6.0/peak/sample_yaml/press/apps/deployments/create_app_deployment.yaml`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/sample_yaml/press/apps/deployments/create_app_deployment_revision.yaml` & `peak_sdk-1.6.0/peak/sample_yaml/press/apps/deployments/create_app_deployment_revision.yaml`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/sample_yaml/press/apps/specs/create_app_spec.yaml` & `peak_sdk-1.6.0/peak/sample_yaml/press/apps/specs/create_app_spec.yaml`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/sample_yaml/press/blocks/deployments/create_block_deployment.yaml` & `peak_sdk-1.6.0/peak/sample_yaml/press/blocks/deployments/create_block_deployment.yaml`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/sample_yaml/press/blocks/specs/create_block_spec.yaml` & `peak_sdk-1.6.0/peak/sample_yaml/press/blocks/specs/create_block_spec.yaml`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/sample_yaml/press/blocks/specs/create_block_spec_release.yaml` & `peak_sdk-1.6.0/peak/sample_yaml/press/blocks/specs/create_block_spec_release.yaml`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/sample_yaml/resources/workflows/create_or_update_workflow.yaml` & `peak_sdk-1.6.0/peak/sample_yaml/resources/workflows/workflow_skippable_steps.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-# workflow.yaml
+# workflow-auto-retry.yaml
 
 body:
-  name: my-new-workflow
+  name: new-workflow
   triggers:
-    - webhook: true
-  tags:
-    - name: CLI
+    - cron: "0 0 * * *"
   steps:
-    step1:
-      command: echo hello world
+    step-1:
       type: standard
-      repository:
-        branch: main
-        token: random_token
-        url: https://example.com
       imageId: 100
       imageVersionId: 100
+      command: echo hello
       resources:
         instanceTypeId: 21
         storage: 10GB
-    step2:
-      command: echo world
+      parents: []
+      stepTimeout: 30
+      clearImageCache: true
+      runConfiguration:
+        skipConfiguration:
+          skip: true
+          skipDAG: true
+    step-2:
       type: standard
-      imageId: 200
-      imageVersionId: 200
+      imageId: 100
+      imageVersionId: 100
+      command: echo world
       resources:
         instanceTypeId: 21
-        storage: 40GB
+        storage: 10GB
+      parents: ["step-1"]
+      stepTimeout: 30
+      clearImageCache: true
```

### Comparing `peak_sdk-1.5.0/peak/sample_yaml/resources/workflows/create_workflow.yaml` & `peak_sdk-1.6.0/peak/sample_yaml/resources/workflows/update_workflow.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 # workflow.yaml
 
 body:
-  name: new-workflow
+  name: updated-workflow
   triggers:
-    - cron: "0 0 * * *"
+    - webhook: true
   watchers:
     - user: abc@peak.ai
       events:
         success: false
         fail: true
     - webhook:
         name: info
         url: "https://abc.com/post"
         payload: '{ "pingback-url": "https:/workflow/123" }'
       events:
         success: false
         fail: true
         runtimeExceeded: 10
+    - email:
+        name: "email-watcher-1"
+        recipients:
+          to:
+            - user1@peak.ai
+            - user2@peak.ai
+      events:
+        success: false
+        fail: true
+        runtimeExceeded: 10
   retryOptions:
     duration: 5
     exitCodes: [1, 2]
     exponentialBackoff: true
     numberOfRetries: 3
   tags:
-    - name: foo
-    - name: bar
+    - name: CLI
   steps:
-    stepName:
+    step1:
+      command: echo hello world
       type: standard
+      repository:
+        branch: main
+        token: random_token
+        url: "https://github.com/org/repo"
       imageId: 100
       imageVersionId: 100
-      command: "python script.py"
       resources:
         instanceTypeId: 21
         storage: 10GB
-      parents: []
-      stepTimeout: 30
-      clearImageCache: true
-      parameters:
-        env:
-          key: value
-        secrets:
-          - secret-1
-          - secret-2
-      repository:
-        branch: main
-        token: random_token
-        url: "https://github.com/org/repo"
+    step2:
+      command: echo world
+      type: standard
+      imageId: 200
+      imageVersionId: 200
+      resources:
+        instanceTypeId: 21
+        storage: 40GB
```

### Comparing `peak_sdk-1.5.0/peak/sample_yaml/resources/workflows/workflow_auto_retry.yaml` & `peak_sdk-1.6.0/peak/sample_yaml/resources/workflows/workflow_auto_retry.yaml`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/sample_yaml/resources/workflows/workflow_execution_parameters.yaml` & `peak_sdk-1.6.0/peak/sample_yaml/resources/workflows/workflow_execution_parameters.yaml`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/sample_yaml/resources/workflows/workflow_output_parameters.yaml` & `peak_sdk-1.6.0/peak/sample_yaml/resources/workflows/workflow_output_parameters.yaml`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/session.py` & `peak_sdk-1.6.0/peak/session.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/telemetry.py` & `peak_sdk-1.6.0/peak/telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             session_meta (Optional[Dict[str, Any]]): Session metadata object that contains information like stage
 
         Returns:
             str: The telemetry URL
         """
         stage = Stage.PROD
         if session_meta:
-            stage = session_meta["stage"] if "stage" in session_meta else Stage.PROD
+            stage = session_meta.get("stage", Stage.PROD)
         base_domain = get_base_domain(stage.value, "service")
         return f"{base_domain}/resource-usage/api/v1/telemetry"
 
     def get_telemetry_data() -> Dict[str, Any]:
         return {
             "sdkVersion": __version__,
             "os": platform.platform(),
```

### Comparing `peak_sdk-1.5.0/peak/template.py` & `peak_sdk-1.6.0/peak/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,18 +34,20 @@
 from peak import exceptions
 from peak.helpers import remove_none_values
 
 
 def _parse_jinja_template(template_path: Path, params: Dict[str, Any]) -> str:
     """Read, parse and render the Jinja template text."""
     jinja_loader = _CustomJinjaLoader()
-    jinja_env = jinja2.Environment(  # TODO: show warning if variable not found in params  # noqa: TD002, TD003, RUF100
-        loader=jinja_loader,
-        autoescape=False,  # noqa: S701
-        extensions=[_IncludeWithIndentation],
+    jinja_env = (
+        jinja2.Environment(  # TODO: show warning if variable not found in params  # noqa: TD002, TD003, RUF100, FIX002
+            loader=jinja_loader,
+            autoescape=False,  # noqa: S701
+            extensions=[_IncludeWithIndentation],
+        )
     )
     jinja_template: jinja2.Template = jinja_env.get_template(str(template_path))
     return jinja_template.render(params, os_env=os.environ)
 
 
 def load_template(
     file: Union[Path, str],
```

### Comparing `peak_sdk-1.5.0/peak/tools/__init__.py` & `peak_sdk-1.6.0/peak/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/tools/logging/log_handler.py` & `peak_sdk-1.6.0/peak/tools/logging/log_handler.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/tools/logging/log_level.py` & `peak_sdk-1.6.0/peak/tools/logging/log_level.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,31 +15,63 @@
 # # This file is part of the peak-sdk.
 # # see (https://github.com/PeakBI/peak-sdk)
 # #
 # # You should have received a copy of the APACHE LICENSE, VERSION 2.0
 # # along with this program. If not, see <https://apache.org/licenses/LICENSE-2.0>
 #
 """Supported Log levels."""
+from __future__ import annotations
 
 import logging
-from enum import Enum
+from enum import IntEnum
+from typing import Final, Literal
 
 
-class LogLevel(Enum):
+class LogLevel(IntEnum):
     """Enumeration of log levels to be used in logging.
 
     Each enum member corresponds to a specific log level defined in the logging module.
     The enum provides a convenient way to specify log levels when configuring loggers.
 
     Attributes:
         DEBUG: Debug log level. Intended for detailed debugging information.
         INFO: Info log level. Used for general information about program execution.
         WARN: Warning log level. Indicates potential issues or unexpected behavior.
+        WARNING: Warning log level. Indicates potential issues or unexpected behavior.
         ERROR: Error log level. Indicates errors that do not prevent program execution.
+        EXCEPTION: Error log level. Indicates errors that do not prevent program execution.
         CRITICAL: Critical log level. Indicates severe errors that might lead to program failure.
+        FATAL: Critical log level. Indicates severe errors that might lead to program failure.
     """
 
     DEBUG = logging.DEBUG
     INFO = logging.INFO
-    WARN = logging.WARN
+    WARN = logging.WARNING
+    WARNING = logging.WARNING
     ERROR = logging.ERROR
+    EXCEPTION = logging.ERROR
     CRITICAL = logging.CRITICAL
+    FATAL = logging.FATAL
+
+
+LogLevelNames = Literal[
+    "DEBUG",
+    "INFO",
+    "WARN",
+    "WARNING",
+    "ERROR",
+    "EXCEPTION",
+    "CRITICAL",
+    "FATAL",
+]
+
+
+LOG_LEVEL_NAMES_TO_LOG_LEVEL: Final[dict[LogLevelNames, LogLevel]] = {
+    "DEBUG": LogLevel.DEBUG,
+    "INFO": LogLevel.INFO,
+    "WARNING": LogLevel.WARN,
+    "WARN": LogLevel.WARN,
+    "ERROR": LogLevel.ERROR,
+    "EXCEPTION": LogLevel.ERROR,
+    "FATAL": LogLevel.CRITICAL,
+    "CRITICAL": LogLevel.CRITICAL,
+}
```

### Comparing `peak_sdk-1.5.0/peak/tools/logging/utils.py` & `peak_sdk-1.6.0/peak/tools/logging/utils.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/peak/validators.py` & `peak_sdk-1.6.0/peak/validators.py`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/pypi-home.md` & `peak_sdk-1.6.0/pypi-home.md`

 * *Files identical despite different names*

### Comparing `peak_sdk-1.5.0/pyproject.toml` & `peak_sdk-1.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peak-sdk"
-version = "1.5.0"
+version = "1.6.0"
 packages = [{ include = "peak" }]
 description = "Python SDK for interacting with the Peak platform"
 authors = ["Peak <support@peak.ai>"]
 license = "Apache License 2.0"
 readme = "pypi-home.md"
 homepage = "https://docs.peak.ai/sdk"
 documentation = "https://docs.peak.ai/sdk/"
@@ -19,73 +19,75 @@
   "Natural Language :: English",
   "Topic :: Software Development :: Libraries :: Application Frameworks",
   "Typing :: Typed"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-requests = "^2.30"
+requests = "^2.31"
 requests-toolbelt = "^1.0"
-pathspec = "^0.11"
+pathspec = "*"
 typer = { version = "^0.9", extras = ['all'] }
 jinja2 = "^3.1"
 pyyaml = "^6.0"
-certifi = ">=2023.7.22"
-shellingham = "<1.5.2"
+certifi = ">=2024.2.2"
+shellingham = "<1.5.4"
 urllib3 = "<2"
 structlog = "^24.1.0"
+orjson = "^3.9.15"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3"
-pytest-sugar = "^0.9"
 pytest-icdiff = "^0.6"
-Pygments = "^2.15"
-types-Pygments = "^2.15"
+pytest-mock = "^3.12"
+pytest-sugar = "^0.9"
+Pygments = "^2.17"
+types-Pygments = "^2.17"
 types-colorama = "^0.4"
-types-setuptools = "^67.7"
+types-setuptools = "^69.1"
 types-urllib3 = "^1.26"
-types-requests = "^2.30"
-types-pyyaml = "^6.0.12.9"
-types-cffi = "^1.15"
+types-requests = "^2.31"
+types-pyyaml = "^6.0"
+types-cffi = "^1.16"
 types-decorator = "^5.1"
-types-jsonschema = "^4.17"
-types-paramiko = "^3.0"
+types-jsonschema = "^4.21"
+types-paramiko = "^3.4"
 types-psutil = "^5.9"
-types-python-dateutil = "^2.8"
+types-python-dateutil = "^2.9"
 types-pywin32 = "^306.0"
 types-six = "^1.16"
 types-typed-ast = "^1.5"
 xdoctest = { extras = ["colors"], version = "^1.1" }
-coverage = { extras = ["toml"], version = "^7.2" }
+coverage = { extras = ["toml"], version = "^7.4" }
 
 [tool.poetry.group.dev.dependencies]
-black = { extras = ["jupyter"], version = ">=23.3.0" }
-furo = ">=2023.3.27"
-mypy = ">=1.2.0"
-pre-commit = ">=3.3.1"
-pre-commit-hooks = ">=4.4.0"
+black = { extras = ["jupyter"], version = ">=24.2.0" }
+furo = ">=2024.1.29"
+mypy = ">=1.9.0"
+pre-commit = ">=3.5.0"
+pre-commit-hooks = ">=4.5.0"
 ochrona = ">=2.0.2"
 darglint = ">=1.8.1"
 sphinx = ">=7.1.2"
 sphinx-autobuild = ">=2021.3.14"
 myst-parser = { version = ">=2.0.0" }
 markdown-it-py = ">=2.2.0"
-shellcheck-py = ">=0.9.0.2"
-nox = ">=2023.4.22"
-nox-poetry = ">=1.0.2"
-blacken-docs = ">=1.13.0"
-click = ">=8.1.3"
+shellcheck-py = ">=0.9.0.6"
+nox = ">=2024.3.2"
+nox-poetry = ">=1.0.3"
+blacken-docs = ">=1.16.0"
+click = ">=8.1.7"
 jupyter = ">=1.0.0"
-notebook = ">=7.0.2"
-nbstripout = ">=0.6.1"
-nbqa = ">=1.7.0"
-jupyter_client = ">=8.2.0"
-ruff = ">=0.0.265"
-tryceratops = ">=2.0.0"
-nbsphinx = ">=0.9.1"
+notebook = ">=7.1.2"
+nbstripout = ">=0.7.1"
+nbqa = ">=1.8.4"
+jupyter_client = ">=8.6.1"
+ruff = ">=0.3.2"
+tryceratops = ">=2.3.2"
+nbsphinx = ">=0.9.3"
 nbsphinx_link = ">=1.3.0"
 pandoc = ">=2.3"
 graphviz = ">=0.20.1"
 detect-secrets = "^1.4.0"
 sphinx-copybutton = "^0.5.2"
 sphinx-multiversion = "^0.2.4"
 sphinx-rtd-theme = "^2.0.0"
@@ -102,32 +104,33 @@
 show_missing = true
 fail_under = 100
 
 [tool.black]
 line-length = 120
 
 [tool.ruff]
-respect-gitignore = true
 src = ["peak", "tests"]
-select = ["ALL"]
-ignore = [
+line-length = 120
+respect-gitignore = true
+lint.select = ["ALL"]
+lint.ignore = [
   "UP006",
   "UP035",
   "UP007",
   "UP037",
   "E501",
   "D401",
   "ANN101",
   "ANN401",
   "PLR0913",
   "TCH",
   "N818",
   "D301"
 ]
-unfixable = [
+lint.unfixable = [
   "T10",
   "T20",
   "B",
   "SIM",
   "RUF",
   "C90",
   "C4",
@@ -136,33 +139,32 @@
   "PIE",
   "PLE",
   "PLC",
   "PLR",
   "PLW",
   "UP"
 ]
-line-length = 120
-dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+lint.dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Ignore all errors in the tests directory.
 "tests/*" = ["S", "INP001", "ANN001", "PTH123", "PTH103", "ERA001"]
 ".github/workflows/files_cache_key.py" = ["S", "INP001"]
 "noxfile.py" = ["S", "INP001"]
 "docs/conf.py" = ["S", "INP001", "A001"]
 "docs/examples/*" = ["ERA001"]
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 docstring-quotes = "double"
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 # Accepts: "google", "numpy", or "pep257".
 convention = "google"
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.nbqa.addopts]
 ruff = ["--ignore=D,T,TRY,E402"]
 
 [tool.mypy]
@@ -194,16 +196,16 @@
 strict_equality = true
 strict_optional = true
 no_implicit_optional = true
 
 # It's hard to make tests compliant using unittest.mock
 [[tool.mypy.overrides]]
 module = 'tests'
-allow_untyped_decorators = true
-allow_untyped_defs = true
+disallow_untyped_defs = false
+disallow_untyped_decorators = false
 
 [[tool.mypy.overrides]]
 module = 'pathspec'
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = 'nox'
@@ -217,21 +219,28 @@
 module = 'requests_toolbelt'
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = 'noxfile'
 ignore_missing_imports = true
 follow_imports = 'skip'
-allow_untyped_decorators = true
+disallow_untyped_decorators = false
 
 [tool.pyright]
 include = ['peak']
 exclude = ["**/.venv", "**/__pycache__", "**/stubs"]
 stubPath = "./stubs"
 useLibraryCodeForTypes = true
 
 [tool.poetry.scripts]
 peak = { callable = "peak.cli.cli:typer_app" }
 
+[tool.pytest.ini_options]
+minversion = 7.0
+addopts = ['--strict-markers', '--strict-config', '-l', '--color=yes']
+xfail_strict = true
+markers = ["slow: marks tests as slow (deselect with '-m \"not slow\"')"]
+console_output_style = 'progress-even-when-capture-no'
+
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `peak_sdk-1.5.0/PKG-INFO` & `peak_sdk-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peak-sdk
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python SDK for interacting with the Peak platform
 Home-page: https://docs.peak.ai/sdk
 License: Apache-2.0
 Author: Peak
 Author-email: support@peak.ai
 Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,26 +12,25 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Typing :: Typed
-Requires-Dist: certifi (>=2023.7.22)
+Requires-Dist: certifi (>=2024.2.2)
 Requires-Dist: jinja2 (>=3.1,<4.0)
-Requires-Dist: pathspec (>=0.11,<0.12)
+Requires-Dist: orjson (>=3.9.15,<4.0.0)
+Requires-Dist: pathspec
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.30,<3.0)
+Requires-Dist: requests (>=2.31,<3.0)
 Requires-Dist: requests-toolbelt (>=1.0,<2.0)
-Requires-Dist: shellingham (<1.5.2)
+Requires-Dist: shellingham (<1.5.4)
 Requires-Dist: structlog (>=24.1.0,<25.0.0)
 Requires-Dist: typer[all] (>=0.9,<0.10)
 Requires-Dist: urllib3 (<2)
 Project-URL: Documentation, https://docs.peak.ai/sdk/
 Description-Content-Type: text/markdown
 
 # Peak SDK
```

