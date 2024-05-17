# Comparing `tmp/fbpcp-0.6.2.tar.gz` & `tmp/fbpcp-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fbpcp-0.6.2.tar", last modified: Thu Oct 26 12:59:19 2023, max compression
+gzip compressed data, was "fbpcp-0.6.3.tar", last modified: Fri May 17 20:09:27 2024, max compression
```

## Comparing `fbpcp-0.6.2.tar` & `fbpcp-0.6.3.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.020945 fbpcp-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-10-26 12:59:04.000000 fbpcp-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2023-10-26 12:59:19.020945 fbpcp-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2023-10-26 12:59:04.000000 fbpcp-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:18.984945 fbpcp-0.6.2/fbpcp/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:18.984945 fbpcp-0.6.2/fbpcp/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:18.988945 fbpcp-0.6.2/fbpcp/decorator/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/decorator/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/decorator/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:18.992945 fbpcp-0.6.2/fbpcp/entity/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/certificate_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/cloud_cost.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/cloud_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/cluster_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/container_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/container_insight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/container_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/container_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/container_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/container_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/file_information.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/firewall_ruleset.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/insight.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/log_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/pce.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/pce_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/pce_network.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/policy_settings_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/policy_statement.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/route_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/vpc_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/entity/vpc_peering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:18.992945 fbpcp-0.6.2/fbpcp/error/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:18.992945 fbpcp-0.6.2/fbpcp/error/mapper/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/error/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/error/mapper/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/error/mapper/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/error/mapper/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/error/pcp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:18.996945 fbpcp-0.6.2/fbpcp/gateway/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/gateway/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/gateway/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/gateway/costexplorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/gateway/ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11150 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/gateway/ecs.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/gateway/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/gateway/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/gateway/kms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6094 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/gateway/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/gateway/secrets_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:18.996945 fbpcp-0.6.2/fbpcp/mapper/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10005 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/mapper/aws.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:18.996945 fbpcp-0.6.2/fbpcp/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/metrics/emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/metrics/getter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.000945 fbpcp-0.6.2/fbpcp/service/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/billing_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     6515 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/container_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/insights.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/log_cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    14550 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/onedocker.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/pce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/pce_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/policy_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/policy_validation_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/secrets_manager_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10996 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/storage_gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9098 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/service/storage_s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.004945 fbpcp-0.6.2/fbpcp/util/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/util/arg_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/util/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/util/gcspath.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/util/reflect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/util/s3path.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/util/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2023-10-26 12:59:04.000000 fbpcp-0.6.2/fbpcp/util/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:18.984945 fbpcp-0.6.2/fbpcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2023-10-26 12:59:18.000000 fbpcp-0.6.2/fbpcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2023-10-26 12:59:18.000000 fbpcp-0.6.2/fbpcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-26 12:59:18.000000 fbpcp-0.6.2/fbpcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-10-26 12:59:18.000000 fbpcp-0.6.2/fbpcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-26 12:59:18.000000 fbpcp-0.6.2/fbpcp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.004945 fbpcp-0.6.2/onedocker/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.004945 fbpcp-0.6.2/onedocker/common/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/common/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/common/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.008945 fbpcp-0.6.2/onedocker/entity/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/entity/attestation_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/entity/exit_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/entity/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/entity/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/entity/opawdl_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/entity/opawdl_state_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/entity/opawdl_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/entity/opawdl_workflow_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/entity/package_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.008945 fbpcp-0.6.2/onedocker/gateway/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/gateway/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/gateway/repository_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.008945 fbpcp-0.6.2/onedocker/mapper/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/mapper/aws.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.008945 fbpcp-0.6.2/onedocker/repository/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/repository/onedocker_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/repository/onedocker_repository_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/repository/opawdl_workflow_instance_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/repository/opawdl_workflow_instance_repository_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.008945 fbpcp-0.6.2/onedocker/script/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.008945 fbpcp-0.6.2/onedocker/script/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/script/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/script/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/script/cli/onedocker_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.012945 fbpcp-0.6.2/onedocker/script/runner/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/script/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/script/runner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11019 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/script/runner/onedocker_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.012945 fbpcp-0.6.2/onedocker/service/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/service/attestation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/service/attestation_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/service/attestation_pc.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/service/certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/service/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/service/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/service/opawdl_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.012945 fbpcp-0.6.2/onedocker/util/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/util/opawdl_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-10-26 12:59:04.000000 fbpcp-0.6.2/onedocker/util/service_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.012945 fbpcp-0.6.2/pce/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.016945 fbpcp-0.6.2/pce/entity/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/entity/iam_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/entity/log_group_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/entity/mpc_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.016945 fbpcp-0.6.2/pce/gateway/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/gateway/ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/gateway/ecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/gateway/iam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/gateway/logs_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/gateway/sts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.016945 fbpcp-0.6.2/pce/mapper/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/mapper/aws.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.016945 fbpcp-0.6.2/pce/validator/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/validator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/validator/duplicate_pce_resources_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 12:59:19.020945 fbpcp-0.6.2/pce/validator/message_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/validator/message_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/validator/message_templates/error_message_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/validator/message_templates/pce_standard_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/validator/message_templates/resource_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/validator/message_templates/validator_step_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/validator/message_templates/warning_message_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    25924 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/validator/validation_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pce/validator/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-10-26 12:59:04.000000 fbpcp-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-26 12:59:19.020945 fbpcp-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-10-26 12:59:04.000000 fbpcp-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.338453 fbpcp-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-17 20:09:23.000000 fbpcp-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-17 20:09:27.338453 fbpcp-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-17 20:09:23.000000 fbpcp-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.310453 fbpcp-0.6.3/fbpcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.310453 fbpcp-0.6.3/fbpcp/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.314453 fbpcp-0.6.3/fbpcp/decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/decorator/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/decorator/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.318453 fbpcp-0.6.3/fbpcp/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/certificate_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/cloud_cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/cloud_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/cluster_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/container_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/container_insight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/container_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/container_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/container_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/container_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/file_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/firewall_ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/insight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/log_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/pce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/pce_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/pce_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/policy_settings_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/policy_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/route_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/vpc_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/entity/vpc_peering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.318453 fbpcp-0.6.3/fbpcp/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.318453 fbpcp-0.6.3/fbpcp/error/mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/error/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/error/mapper/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/error/mapper/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/error/mapper/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/error/pcp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.318453 fbpcp-0.6.3/fbpcp/gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/gateway/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/gateway/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/gateway/costexplorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/gateway/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11152 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/gateway/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/gateway/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/gateway/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/gateway/kms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/gateway/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/gateway/secrets_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.318453 fbpcp-0.6.3/fbpcp/mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/mapper/aws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.318453 fbpcp-0.6.3/fbpcp/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/metrics/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/metrics/getter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.322453 fbpcp-0.6.3/fbpcp/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/billing_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/container_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/insights.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/log_cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14550 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/onedocker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/pce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/pce_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/policy_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/policy_validation_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/secrets_manager_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10996 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/storage_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9098 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/service/storage_s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.322453 fbpcp-0.6.3/fbpcp/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/util/arg_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/util/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/util/gcspath.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/util/reflect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/util/s3path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/util/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-17 20:09:23.000000 fbpcp-0.6.3/fbpcp/util/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.334453 fbpcp-0.6.3/fbpcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-17 20:09:27.000000 fbpcp-0.6.3/fbpcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-17 20:09:27.000000 fbpcp-0.6.3/fbpcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:09:27.000000 fbpcp-0.6.3/fbpcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-17 20:09:27.000000 fbpcp-0.6.3/fbpcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 20:09:27.000000 fbpcp-0.6.3/fbpcp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.326453 fbpcp-0.6.3/onedocker/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.326453 fbpcp-0.6.3/onedocker/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/common/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/common/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.326453 fbpcp-0.6.3/onedocker/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/entity/attestation_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/entity/exit_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/entity/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/entity/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/entity/opawdl_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/entity/opawdl_state_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/entity/opawdl_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/entity/opawdl_workflow_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/entity/package_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.326453 fbpcp-0.6.3/onedocker/gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/gateway/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/gateway/repository_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.326453 fbpcp-0.6.3/onedocker/mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/mapper/aws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.326453 fbpcp-0.6.3/onedocker/repository/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/repository/onedocker_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/repository/onedocker_repository_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/repository/opawdl_workflow_instance_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/repository/opawdl_workflow_instance_repository_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.326453 fbpcp-0.6.3/onedocker/script/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.330453 fbpcp-0.6.3/onedocker/script/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/script/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/script/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/script/cli/onedocker_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.330453 fbpcp-0.6.3/onedocker/script/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/script/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/script/runner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11019 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/script/runner/onedocker_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.330453 fbpcp-0.6.3/onedocker/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/service/attestation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/service/attestation_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/service/attestation_pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/service/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/service/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/service/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/service/opawdl_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.330453 fbpcp-0.6.3/onedocker/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/util/opawdl_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-17 20:09:23.000000 fbpcp-0.6.3/onedocker/util/service_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.330453 fbpcp-0.6.3/pce/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.330453 fbpcp-0.6.3/pce/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/entity/iam_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/entity/log_group_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/entity/mpc_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.334453 fbpcp-0.6.3/pce/gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/gateway/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/gateway/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/gateway/iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/gateway/logs_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/gateway/sts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.334453 fbpcp-0.6.3/pce/mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/mapper/aws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.334453 fbpcp-0.6.3/pce/validator/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/validator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/validator/duplicate_pce_resources_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:27.334453 fbpcp-0.6.3/pce/validator/message_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/validator/message_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/validator/message_templates/error_message_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/validator/message_templates/pce_standard_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/validator/message_templates/resource_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/validator/message_templates/validator_step_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/validator/message_templates/warning_message_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25924 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/validator/validation_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pce/validator/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 20:09:23.000000 fbpcp-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 20:09:27.338453 fbpcp-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-17 20:09:23.000000 fbpcp-0.6.3/setup.py
```

### Comparing `fbpcp-0.6.2/LICENSE` & `fbpcp-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/PKG-INFO` & `fbpcp-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fbpcp
-Version: 0.6.2
+Version: 0.6.3
 Summary: Facebook Private Computation Platform
 Home-page: https://github.com/facebookresearch/fbpcp
 Author: Facebook
 Author-email: researchtool-help@fb.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3==1.18.57
 Requires-Dist: urllib3==1.26.18
 Requires-Dist: dataclasses-json==0.5.2
 Requires-Dist: pyyaml==5.4.1
-Requires-Dist: tqdm==4.55.1
+Requires-Dist: tqdm==4.66.3
 Requires-Dist: google-cloud-storage==1.30.0
 Requires-Dist: docopt==0.6.2
 Requires-Dist: schema==0.7.5
 Requires-Dist: psutil==5.8.0
 Requires-Dist: click==7.1.2
 Requires-Dist: kubernetes==12.0.1
```

### Comparing `fbpcp-0.6.2/README.md` & `fbpcp-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/decorator/error_handler.py` & `fbpcp-0.6.3/fbpcp/decorator/error_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-unsafe
+
 import functools
 from typing import Callable
 
 from botocore.exceptions import ClientError
 from fbpcp.error.mapper.aws import map_aws_error
 from fbpcp.error.mapper.gcp import map_gcp_error
 from fbpcp.error.mapper.k8s import map_k8s_error
```

### Comparing `fbpcp-0.6.2/fbpcp/decorator/metrics.py` & `fbpcp-0.6.3/fbpcp/decorator/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-unsafe
+
 """Metrics Decorators
 
 The decorators in this file are designed to deocrate classes that implement MetricsGetter.
 """
 
 import asyncio
 import functools
```

### Comparing `fbpcp-0.6.2/fbpcp/entity/certificate_request.py` & `fbpcp-0.6.3/fbpcp/entity/certificate_request.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/entity/cluster_instance.py` & `fbpcp-0.6.3/fbpcp/entity/cluster_instance.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/entity/container_definition.py` & `fbpcp-0.6.3/fbpcp/entity/container_definition.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/entity/container_instance.py` & `fbpcp-0.6.3/fbpcp/entity/container_instance.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/entity/container_type.py` & `fbpcp-0.6.3/fbpcp/entity/container_type.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/entity/firewall_ruleset.py` & `fbpcp-0.6.3/fbpcp/entity/firewall_ruleset.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/entity/insight.py` & `fbpcp-0.6.3/fbpcp/entity/insight.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/entity/pce_compute.py` & `fbpcp-0.6.3/fbpcp/entity/pce_compute.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/entity/pce_network.py` & `fbpcp-0.6.3/fbpcp/entity/pce_network.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/entity/policy_settings_config.py` & `fbpcp-0.6.3/fbpcp/entity/policy_settings_config.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/entity/policy_statement.py` & `fbpcp-0.6.3/fbpcp/entity/policy_statement.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/entity/route_table.py` & `fbpcp-0.6.3/fbpcp/entity/route_table.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/entity/vpc_instance.py` & `fbpcp-0.6.3/fbpcp/entity/vpc_instance.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/entity/vpc_peering.py` & `fbpcp-0.6.3/fbpcp/entity/vpc_peering.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/error/mapper/aws.py` & `fbpcp-0.6.3/fbpcp/error/mapper/aws.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from fbpcp.error.pcp import (
     InvalidParameterError,
     LimitExceededError,
     PcpError,
     ThrottlingError,
 )
 
+
 # reference: https://boto3.amazonaws.com/v1/documentation/api/latest/guide/error-handling.html
 def map_aws_error(error: ClientError) -> PcpError:
     code = error.response["Error"]["Code"]
     response_metadata = error.response["ResponseMetadata"]
     message = f"{error}\n\n Details: {response_metadata}\n"
 
     if code == "InvalidParameterException":
```

### Comparing `fbpcp-0.6.2/fbpcp/error/mapper/gcp.py` & `fbpcp-0.6.3/fbpcp/error/mapper/gcp.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/error/mapper/k8s.py` & `fbpcp-0.6.3/fbpcp/error/mapper/k8s.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from kubernetes.client.exceptions import (
     ApiException,
     ApiTypeError,
     ApiValueError,
     OpenApiException,
 )
 
+
 # reference: https://github.com/kubernetes-client/python/blob/d3de7a85a63fa6bec6518d1cc75dc5e9458b9bbc/kubernetes/client/exceptions.py
 def map_k8s_error(error: OpenApiException) -> PcpError:
     message = str(error)
     if isinstance(error, (ApiValueError, ApiTypeError)):
         return InvalidParameterError(message)
     elif isinstance(error, ApiException):
         code = error.status
```

### Comparing `fbpcp-0.6.2/fbpcp/gateway/aws.py` & `fbpcp-0.6.3/fbpcp/gateway/aws.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/gateway/cloudwatch.py` & `fbpcp-0.6.3/fbpcp/gateway/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/gateway/costexplorer.py` & `fbpcp-0.6.3/fbpcp/gateway/costexplorer.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/gateway/ec2.py` & `fbpcp-0.6.3/fbpcp/gateway/ec2.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/gateway/ecs.py` & `fbpcp-0.6.3/fbpcp/gateway/ecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,17 +107,17 @@
     ) -> List[Optional[ContainerInstance]]:
         response = self.client.describe_tasks(
             cluster=cluster, tasks=tasks
         )  # not necessarily in order of `tasks`
 
         arn_to_instance: Dict[str, Optional[ContainerInstance]] = {}
         for resp_task_dict in response["tasks"]:
-            arn_to_instance[
-                resp_task_dict["taskArn"]
-            ] = map_ecstask_to_containerinstance(resp_task_dict)
+            arn_to_instance[resp_task_dict["taskArn"]] = (
+                map_ecstask_to_containerinstance(resp_task_dict)
+            )
 
         for failure in response["failures"]:
             self.logger.warning(
                 f"ECSGateway failed to describe a task {failure['arn']}, reason: {failure['reason']}"
             )
 
         return [arn_to_instance.get(arn, None) for arn in tasks]
```

### Comparing `fbpcp-0.6.2/fbpcp/gateway/gcp.py` & `fbpcp-0.6.3/fbpcp/gateway/gcp.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/gateway/gcs.py` & `fbpcp-0.6.3/fbpcp/gateway/gcs.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/gateway/kms.py` & `fbpcp-0.6.3/fbpcp/gateway/kms.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/gateway/s3.py` & `fbpcp-0.6.3/fbpcp/gateway/s3.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/gateway/secrets_manager.py` & `fbpcp-0.6.3/fbpcp/gateway/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/mapper/aws.py` & `fbpcp-0.6.3/fbpcp/mapper/aws.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/service/billing.py` & `fbpcp-0.6.3/fbpcp/service/billing.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/service/billing_aws.py` & `fbpcp-0.6.3/fbpcp/service/billing_aws.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/service/container.py` & `fbpcp-0.6.3/fbpcp/service/container.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/service/container_aws.py` & `fbpcp-0.6.3/fbpcp/service/container_aws.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/service/log.py` & `fbpcp-0.6.3/fbpcp/service/log.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/service/log_cloudwatch.py` & `fbpcp-0.6.3/fbpcp/service/log_cloudwatch.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/service/onedocker.py` & `fbpcp-0.6.3/fbpcp/service/onedocker.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/service/pce_aws.py` & `fbpcp-0.6.3/fbpcp/service/pce_aws.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/service/policy_validation.py` & `fbpcp-0.6.3/fbpcp/service/policy_validation.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/service/policy_validation_aws.py` & `fbpcp-0.6.3/fbpcp/service/policy_validation_aws.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/service/secrets_manager.py` & `fbpcp-0.6.3/fbpcp/service/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/service/secrets_manager_aws.py` & `fbpcp-0.6.3/fbpcp/service/secrets_manager_aws.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/service/storage.py` & `fbpcp-0.6.3/fbpcp/service/storage.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/service/storage_gcs.py` & `fbpcp-0.6.3/fbpcp/service/storage_gcs.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/service/storage_s3.py` & `fbpcp-0.6.3/fbpcp/service/storage_s3.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/util/aws.py` & `fbpcp-0.6.3/fbpcp/util/aws.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/util/gcspath.py` & `fbpcp-0.6.3/fbpcp/util/gcspath.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/util/s3path.py` & `fbpcp-0.6.3/fbpcp/util/s3path.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp/util/yaml.py` & `fbpcp-0.6.3/fbpcp/util/yaml.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/fbpcp.egg-info/PKG-INFO` & `fbpcp-0.6.3/fbpcp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fbpcp
-Version: 0.6.2
+Version: 0.6.3
 Summary: Facebook Private Computation Platform
 Home-page: https://github.com/facebookresearch/fbpcp
 Author: Facebook
 Author-email: researchtool-help@fb.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3==1.18.57
 Requires-Dist: urllib3==1.26.18
 Requires-Dist: dataclasses-json==0.5.2
 Requires-Dist: pyyaml==5.4.1
-Requires-Dist: tqdm==4.55.1
+Requires-Dist: tqdm==4.66.3
 Requires-Dist: google-cloud-storage==1.30.0
 Requires-Dist: docopt==0.6.2
 Requires-Dist: schema==0.7.5
 Requires-Dist: psutil==5.8.0
 Requires-Dist: click==7.1.2
 Requires-Dist: kubernetes==12.0.1
```

### Comparing `fbpcp-0.6.2/fbpcp.egg-info/SOURCES.txt` & `fbpcp-0.6.3/fbpcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/common/env.py` & `fbpcp-0.6.3/onedocker/common/env.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-unsafe
+
 # This is the repository path that OneDocker downloads binaries from
 ONEDOCKER_REPOSITORY_PATH = "ONEDOCKER_REPOSITORY_PATH"
 
 # This is the repository path that OneDocker downloads binary checksums from
 ONEDOCKER_CHECKSUM_REPOSITORY_PATH = "ONEDOCKER_CHECKSUM_REPOSITORY_PATH"
 
 # This is the local path that the binaries reside
```

### Comparing `fbpcp-0.6.2/onedocker/common/util.py` & `fbpcp-0.6.3/onedocker/common/util.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/entity/attestation_document.py` & `fbpcp-0.6.3/onedocker/entity/attestation_document.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/entity/exit_code.py` & `fbpcp-0.6.3/onedocker/entity/exit_code.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/entity/measurement.py` & `fbpcp-0.6.3/onedocker/entity/measurement.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/entity/metadata.py` & `fbpcp-0.6.3/onedocker/entity/metadata.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/entity/opawdl_state.py` & `fbpcp-0.6.3/onedocker/entity/opawdl_state.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/entity/opawdl_state_instance.py` & `fbpcp-0.6.3/onedocker/entity/opawdl_state_instance.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/entity/opawdl_workflow.py` & `fbpcp-0.6.3/onedocker/entity/opawdl_workflow.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/entity/opawdl_workflow_instance.py` & `fbpcp-0.6.3/onedocker/entity/opawdl_workflow_instance.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/gateway/dynamodb.py` & `fbpcp-0.6.3/onedocker/gateway/dynamodb.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/gateway/repository_service.py` & `fbpcp-0.6.3/onedocker/gateway/repository_service.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/mapper/aws.py` & `fbpcp-0.6.3/onedocker/mapper/aws.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/repository/onedocker_package.py` & `fbpcp-0.6.3/onedocker/repository/onedocker_package.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/repository/onedocker_repository_service.py` & `fbpcp-0.6.3/onedocker/repository/onedocker_repository_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-unsafe
+
 from typing import Dict, List, Optional
 
 from fbpcp.error.pcp import PcpError
 from fbpcp.service.storage import StorageService
 from onedocker.entity.measurement import MeasurementType
 from onedocker.entity.metadata import PackageMetadata
```

### Comparing `fbpcp-0.6.2/onedocker/repository/opawdl_workflow_instance_repository.py` & `fbpcp-0.6.3/onedocker/repository/opawdl_workflow_instance_repository.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/repository/opawdl_workflow_instance_repository_local.py` & `fbpcp-0.6.3/onedocker/repository/opawdl_workflow_instance_repository_local.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/script/cli/onedocker_cli.py` & `fbpcp-0.6.3/onedocker/script/cli/onedocker_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-unsafe
+
 
 """
 CLI for uploading an executable to one docker repo
 
 
 Usage:
     onedocker-cli upload --config=<config> --package_name=<package_name> --package_path=<package_path> --version=<version>
```

### Comparing `fbpcp-0.6.2/onedocker/script/runner/onedocker_runner.py` & `fbpcp-0.6.3/onedocker/script/runner/onedocker_runner.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/service/attestation_factory.py` & `fbpcp-0.6.3/onedocker/service/attestation_factory.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/service/attestation_pc.py` & `fbpcp-0.6.3/onedocker/service/attestation_pc.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/service/certificate.py` & `fbpcp-0.6.3/onedocker/service/certificate.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/service/measurement.py` & `fbpcp-0.6.3/onedocker/service/measurement.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/service/metadata.py` & `fbpcp-0.6.3/onedocker/service/metadata.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/service/opawdl_driver.py` & `fbpcp-0.6.3/onedocker/service/opawdl_driver.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/util/opawdl_parser.py` & `fbpcp-0.6.3/onedocker/util/opawdl_parser.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/onedocker/util/service_builder.py` & `fbpcp-0.6.3/onedocker/util/service_builder.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/pce/gateway/ec2.py` & `fbpcp-0.6.3/pce/gateway/ec2.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/pce/gateway/ecs.py` & `fbpcp-0.6.3/pce/gateway/ecs.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/pce/gateway/iam.py` & `fbpcp-0.6.3/pce/gateway/iam.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/pce/gateway/logs_aws.py` & `fbpcp-0.6.3/pce/gateway/logs_aws.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/pce/gateway/sts.py` & `fbpcp-0.6.3/pce/gateway/sts.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/pce/mapper/aws.py` & `fbpcp-0.6.3/pce/mapper/aws.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/pce/validator/duplicate_pce_resources_checker.py` & `fbpcp-0.6.3/pce/validator/duplicate_pce_resources_checker.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/pce/validator/message_templates/error_message_templates.py` & `fbpcp-0.6.3/pce/validator/message_templates/error_message_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     CONTAINER_IMAGE,
     CONTAINER_MEMORY,
     FIREWALL_RULE_FINAL_PORT,
     FIREWALL_RULE_INITIAL_PORT,
     IGW_ROUTE_DESTINATION_CIDR_BLOCK,
 )
 
+
 # PCE networking validation error messages
 class NetworkingErrorTemplate(Enum):
     # VPC
     VPC_NON_PRIVATE_CIDR = "The CIDR of the vpc {vpc_cidr} is not a private range."
 
     # Firewall
     FIREWALL_CIDR_NOT_OVERLAPS_VPC = "VPC peering for VPC {peer_target_id} doesn't have an inbound rule to allow traffic to {vpc_id}:{vpc_cidr}."
```

### Comparing `fbpcp-0.6.2/pce/validator/message_templates/pce_standard_constants.py` & `fbpcp-0.6.3/pce/validator/message_templates/pce_standard_constants.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/pce/validator/message_templates/validator_step_names.py` & `fbpcp-0.6.3/pce/validator/message_templates/validator_step_names.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/pce/validator/message_templates/warning_message_templates.py` & `fbpcp-0.6.3/pce/validator/message_templates/warning_message_templates.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/pce/validator/validation_suite.py` & `fbpcp-0.6.3/pce/validator/validation_suite.py`

 * *Files identical despite different names*

### Comparing `fbpcp-0.6.2/pce/validator/validator.py` & `fbpcp-0.6.3/pce/validator/validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+# pyre-unsafe
+
 """
 
 
 Usage:
     pce_validator --region=<region> --pce-id=<pce_id> [--key-id=<key_id>] [--key-data=<key_data>] [--role=<role>] [--run-step=<run-step> | --skip-step=<skip-step>]...
 
 Options ([+] can be repeated):
```

### Comparing `fbpcp-0.6.2/setup.py` & `fbpcp-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 from setuptools import find_packages, setup
 
 install_requires = [
     "boto3==1.18.57",
     "urllib3==1.26.18",
     "dataclasses-json==0.5.2",
     "pyyaml==5.4.1",
-    "tqdm==4.55.1",
+    "tqdm==4.66.3",
     "google-cloud-storage==1.30.0",
     "docopt==0.6.2",
     "schema==0.7.5",
     "psutil==5.8.0",
     "click==7.1.2",
     "kubernetes==12.0.1",
 ]
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="fbpcp",
-    version="0.6.2",
+    version="0.6.3",
     description="Facebook Private Computation Platform",
     author="Facebook",
     author_email="researchtool-help@fb.com",
     url="https://github.com/facebookresearch/fbpcp",
     install_requires=install_requires,
     packages=find_packages(),
     long_description_content_type="text/markdown",
```

