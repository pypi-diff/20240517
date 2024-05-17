# Comparing `tmp/skypilot_nightly-1.0.0.dev20240515.tar.gz` & `tmp/skypilot_nightly-1.0.0.dev20240516.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot_nightly-1.0.0.dev20240515.tar", last modified: Wed May 15 15:03:07 2024, max compression
+gzip compressed data, was "skypilot_nightly-1.0.0.dev20240516.tar", last modified: Thu May 16 10:38:19 2024, max compression
```

## Comparing `skypilot_nightly-1.0.0.dev20240515.tar` & `skypilot_nightly-1.0.0.dev20240516.tar`

### file list

```diff
@@ -1,339 +1,339 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.920903 skypilot_nightly-1.0.0.dev20240515/
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-15 15:03:07.920903 skypilot_nightly-1.0.0.dev20240515/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:03:07.920903 skypilot_nightly-1.0.0.dev20240515/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-15 15:03:05.000000 skypilot_nightly-1.0.0.dev20240515/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.860903 skypilot_nightly-1.0.0.dev20240515/sky/
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-15 15:03:07.000000 skypilot_nightly-1.0.0.dev20240515/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.864903 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    21408 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.864903 skypilot_nightly-1.0.0.dev20240515/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)   125420 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   230760 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.864903 skypilot_nightly-1.0.0.dev20240515/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.864903 skypilot_nightly-1.0.0.dev20240515/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    26446 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (127)   192150 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.868903 skypilot_nightly-1.0.0.dev20240515/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    31006 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    31817 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/cloud_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    48019 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20376 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/paperspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11166 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.872903 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/cudo_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.872903 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/fluidstack_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/kubernetes_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/paperspace_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/runpod_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/vsphere_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.872903 skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/oci_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/scp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    34233 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.876903 skypilot_nightly-1.0.0.dev20240515/sky/data/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   118872 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25107 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/global_user_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.876903 skypilot_nightly-1.0.0.dev20240515/sky/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    13430 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.876903 skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.876903 skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.876903 skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    25556 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23041 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/state.py
--rw-r--r--   0 runner    (1001) docker     (127)    33067 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    54188 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.876903 skypilot_nightly-1.0.0.dev20240515/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.876903 skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    36307 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.880903 skypilot_nightly-1.0.0.dev20240515/sky/provision/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/azure/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.880903 skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/cudo_machine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/cudo_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    16758 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/docker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.880903 skypilot_nightly-1.0.0.dev20240515/sky/provision/fluidstack/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/fluidstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/fluidstack/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/fluidstack/fluidstack_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/fluidstack/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.880903 skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24215 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22186 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/instance_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.880903 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28319 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    32919 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.880903 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/manifests/smarter-device-manager-configmap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    62091 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.884903 skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25103 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/provisioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.884903 skypilot_nightly-1.0.0.dev20240515/sky/provision/runpod/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/runpod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/runpod/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/runpod/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/runpod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.884903 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.888903 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/cls_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/cls_api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/custom_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/metadata_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/service_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/service_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/ssl_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/vapiconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/vim_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24488 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/vsphere_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    65346 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.888903 skypilot_nightly-1.0.0.dev20240515/sky/serve/
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/autoscalers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11548 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/load_balancing_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    56630 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/replica_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/serve_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    37183 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/serve_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/service_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.888903 skypilot_nightly-1.0.0.dev20240515/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-15 15:03:05.000000 skypilot_nightly-1.0.0.dev20240515/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.892903 skypilot_nightly-1.0.0.dev20240515/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    35198 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/log_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/log_lib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.892903 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.892903 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19215 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    16355 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.892903 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.892903 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13971 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.892903 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.896903 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/scp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.896903 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skypilot_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    47130 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.900903 skypilot_nightly-1.0.0.dev20240515/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/cudo-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/fluidstack-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/jobs-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-ingress.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-loadbalancer.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-ssh-jump.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/paperspace-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/runpod-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/sky-serve-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/vsphere-ray.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.900903 skypilot_nightly-1.0.0.dev20240515/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.904903 skypilot_nightly-1.0.0.dev20240515/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.904903 skypilot_nightly-1.0.0.dev20240515/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/cluster_yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22168 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/command_runner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34359 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/controller_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/env_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.904903 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9759 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/create_cluster.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/delete_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/generate_kind_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4422 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/generate_static_kubeconfig.sh
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/gpu_labeler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/resources_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22737 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.908903 skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-15 15:03:07.000000 skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-05-15 15:03:07.000000 skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:03:07.000000 skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 15:03:07.000000 skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-15 15:03:07.000000 skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 15:03:07.000000 skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.908903 skypilot_nightly-1.0.0.dev20240515/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17529 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_jobs_and_serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_serve_autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)   216332 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_wheels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.066670 skypilot_nightly-1.0.0.dev20240516/
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-16 10:38:19.066670 skypilot_nightly-1.0.0.dev20240516/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 10:38:19.066670 skypilot_nightly-1.0.0.dev20240516/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-16 10:38:16.000000 skypilot_nightly-1.0.0.dev20240516/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.006671 skypilot_nightly-1.0.0.dev20240516/sky/
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-16 10:38:18.000000 skypilot_nightly-1.0.0.dev20240516/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.010671 skypilot_nightly-1.0.0.dev20240516/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/adaptors/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/adaptors/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/adaptors/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/adaptors/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/adaptors/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21408 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.010671 skypilot_nightly-1.0.0.dev20240516/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125420 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   230760 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.010671 skypilot_nightly-1.0.0.dev20240516/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.010671 skypilot_nightly-1.0.0.dev20240516/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26446 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)   192402 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.014670 skypilot_nightly-1.0.0.dev20240516/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31006 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31817 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/cloud_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48019 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20376 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/paperspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11166 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.018671 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/cudo_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.018671 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/fluidstack_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/kubernetes_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/paperspace_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/runpod_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/vsphere_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.018671 skypilot_nightly-1.0.0.dev20240516/sky/clouds/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/utils/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/utils/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/utils/oci_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/utils/scp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/clouds/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34233 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.022671 skypilot_nightly-1.0.0.dev20240516/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118872 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25107 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/global_user_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.022671 skypilot_nightly-1.0.0.dev20240516/sky/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/jobs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/jobs/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13430 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/jobs/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.022671 skypilot_nightly-1.0.0.dev20240516/sky/jobs/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/jobs/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.022671 skypilot_nightly-1.0.0.dev20240516/sky/jobs/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/jobs/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.022671 skypilot_nightly-1.0.0.dev20240516/sky/jobs/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/jobs/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    25556 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/jobs/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23041 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/jobs/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33067 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/jobs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54188 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.022671 skypilot_nightly-1.0.0.dev20240516/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.022671 skypilot_nightly-1.0.0.dev20240516/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36307 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/aws/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.026671 skypilot_nightly-1.0.0.dev20240516/sky/provision/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/azure/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.026671 skypilot_nightly-1.0.0.dev20240516/sky/provision/cudo/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/cudo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/cudo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/cudo/cudo_machine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/cudo/cudo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/cudo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16758 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/docker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.026671 skypilot_nightly-1.0.0.dev20240516/sky/provision/fluidstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/fluidstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/fluidstack/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/fluidstack/fluidstack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/fluidstack/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.026671 skypilot_nightly-1.0.0.dev20240516/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24215 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22186 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/instance_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.026671 skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28319 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32919 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.026671 skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/manifests/smarter-device-manager-configmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62091 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.030671 skypilot_nightly-1.0.0.dev20240516/sky/provision/paperspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/paperspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/paperspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/paperspace/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/paperspace/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/paperspace/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25103 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/provisioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.030671 skypilot_nightly-1.0.0.dev20240516/sky/provision/runpod/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/runpod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/runpod/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/runpod/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/runpod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.030671 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.030671 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/cls_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/cls_api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/metadata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/service_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/ssl_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/vapiconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/vim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24488 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/vsphere_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65346 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.034670 skypilot_nightly-1.0.0.dev20240516/sky/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/serve/autoscalers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/serve/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/serve/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/serve/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11548 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/serve/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/serve/load_balancing_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56630 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/serve/replica_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/serve/serve_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37183 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/serve/serve_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/serve/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/serve/service_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.034670 skypilot_nightly-1.0.0.dev20240516/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-16 10:38:16.000000 skypilot_nightly-1.0.0.dev20240516/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.038670 skypilot_nightly-1.0.0.dev20240516/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35198 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/log_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/log_lib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.038670 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.038670 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19215 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/azure/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16355 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.038670 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.038670 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13971 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.038670 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.042670 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/scp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.042670 skypilot_nightly-1.0.0.dev20240516/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/skypilot_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47130 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.046670 skypilot_nightly-1.0.0.dev20240516/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/cudo-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/fluidstack-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/jobs-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/kubernetes-ingress.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/kubernetes-loadbalancer.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/kubernetes-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/kubernetes-ssh-jump.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/paperspace-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/runpod-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/sky-serve-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/templates/vsphere-ray.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.046670 skypilot_nightly-1.0.0.dev20240516/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.050670 skypilot_nightly-1.0.0.dev20240516/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.050670 skypilot_nightly-1.0.0.dev20240516/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/cluster_yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22168 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/command_runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34359 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/controller_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/env_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.050670 skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9759 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/create_cluster.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/delete_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/generate_kind_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4422 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/generate_static_kubeconfig.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/gpu_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/resources_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22737 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.054670 skypilot_nightly-1.0.0.dev20240516/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-16 10:38:18.000000 skypilot_nightly-1.0.0.dev20240516/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-05-16 10:38:18.000000 skypilot_nightly-1.0.0.dev20240516/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 10:38:18.000000 skypilot_nightly-1.0.0.dev20240516/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 10:38:18.000000 skypilot_nightly-1.0.0.dev20240516/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-16 10:38:18.000000 skypilot_nightly-1.0.0.dev20240516/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 10:38:18.000000 skypilot_nightly-1.0.0.dev20240516/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:19.054670 skypilot_nightly-1.0.0.dev20240516/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17529 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/tests/test_jobs_and_serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/tests/test_serve_autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)   216332 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/tests/test_wheels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-16 10:38:13.000000 skypilot_nightly-1.0.0.dev20240516/tests/test_yaml_parser.py
```

### Comparing `skypilot_nightly-1.0.0.dev20240515/LICENSE` & `skypilot_nightly-1.0.0.dev20240516/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/MANIFEST.in` & `skypilot_nightly-1.0.0.dev20240516/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/PKG-INFO` & `skypilot_nightly-1.0.0.dev20240516/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240515
+Version: 1.0.0.dev20240516
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot_nightly-1.0.0.dev20240515/README.md` & `skypilot_nightly-1.0.0.dev20240516/README.md`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/pyproject.toml` & `skypilot_nightly-1.0.0.dev20240516/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/setup.py` & `skypilot_nightly-1.0.0.dev20240516/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/__init__.py` & `skypilot_nightly-1.0.0.dev20240516/sky/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """The SkyPilot package."""
 import os
 import subprocess
 from typing import Optional
 import urllib.request
 
 # Replaced with the current commit when building the wheels.
-_SKYPILOT_COMMIT_SHA = '5a2f1b855e0a8b0a099390882209914f34ea8b98'
+_SKYPILOT_COMMIT_SHA = 'f24425c62299170d377268e91fee8a8fb5d43b12'
 
 
 def _get_git_commit():
     if 'SKYPILOT_COMMIT_SHA' not in _SKYPILOT_COMMIT_SHA:
         # This is a release build, so we don't need to get the commit hash from
         # git, as it's already been set.
         return _SKYPILOT_COMMIT_SHA
@@ -31,15 +31,15 @@
             commit_hash += '-dirty'
         return commit_hash
     except Exception:  # pylint: disable=broad-except
         return _SKYPILOT_COMMIT_SHA
 
 
 __commit__ = _get_git_commit()
-__version__ = '1.0.0.dev20240515'
+__version__ = '1.0.0.dev20240516'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 
 # ---------------------- Proxy Configuration ---------------------- #
 def _set_http_proxy_env_vars() -> None:
     urllib_proxies = dict(urllib.request.getproxies())
```

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/aws.py` & `skypilot_nightly-1.0.0.dev20240516/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/azure.py` & `skypilot_nightly-1.0.0.dev20240516/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/cloudflare.py` & `skypilot_nightly-1.0.0.dev20240516/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/common.py` & `skypilot_nightly-1.0.0.dev20240516/sky/adaptors/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/gcp.py` & `skypilot_nightly-1.0.0.dev20240516/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/ibm.py` & `skypilot_nightly-1.0.0.dev20240516/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/kubernetes.py` & `skypilot_nightly-1.0.0.dev20240516/sky/adaptors/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/oci.py` & `skypilot_nightly-1.0.0.dev20240516/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/vsphere.py` & `skypilot_nightly-1.0.0.dev20240516/sky/adaptors/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/authentication.py` & `skypilot_nightly-1.0.0.dev20240516/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/backends/__init__.py` & `skypilot_nightly-1.0.0.dev20240516/sky/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/backends/backend.py` & `skypilot_nightly-1.0.0.dev20240516/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/backends/backend_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/backends/cloud_vm_ray_backend.py` & `skypilot_nightly-1.0.0.dev20240516/sky/backends/cloud_vm_ray_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/backends/docker_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/backends/local_docker_backend.py` & `skypilot_nightly-1.0.0.dev20240516/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot_nightly-1.0.0.dev20240516/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/backends/wheel_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/benchmark/benchmark_state.py` & `skypilot_nightly-1.0.0.dev20240516/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/benchmark/benchmark_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/check.py` & `skypilot_nightly-1.0.0.dev20240516/sky/check.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 """Credential checks: check cloud credentials and enable clouds."""
 import traceback
-from typing import Dict, Iterable, List, Optional, Tuple
+from types import ModuleType
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import click
 import colorama
 import rich
 
-from sky import clouds
+from sky import clouds as sky_clouds
 from sky import exceptions
 from sky import global_user_state
 from sky.adaptors import cloudflare
 from sky.utils import ux_utils
 
 
-# TODO(zhwu): add check for a single cloud to improve performance
-def check(quiet: bool = False, verbose: bool = False) -> None:
+def check(
+    quiet: bool = False,
+    verbose: bool = False,
+    clouds: Optional[Tuple[str]] = None,
+) -> None:
     echo = (lambda *_args, **_kwargs: None) if quiet else click.echo
     echo('Checking credentials to enable clouds for SkyPilot.')
-
     enabled_clouds = []
+    disabled_clouds = []
 
-    def check_one_cloud(cloud_tuple: Tuple[str, clouds.Cloud]) -> None:
+    def check_one_cloud(
+            cloud_tuple: Tuple[str, Union[sky_clouds.Cloud,
+                                          ModuleType]]) -> None:
         cloud_repr, cloud = cloud_tuple
         echo(f'  Checking {cloud_repr}...', nl=False)
         try:
             ok, reason = cloud.check_credentials()
         except Exception:  # pylint: disable=broad-except
             # Catch all exceptions to prevent a single cloud from blocking the
             # check for other clouds.
@@ -39,60 +45,84 @@
             if verbose and cloud is not cloudflare:
                 activated_account = cloud.get_current_user_identity_str()
                 if activated_account is not None:
                     echo(f'    Activated account: {activated_account}')
             if reason is not None:
                 echo(f'    Hint: {reason}')
         else:
+            disabled_clouds.append(cloud_repr)
             echo(f'    Reason: {reason}')
 
-    clouds_to_check = [
-        (repr(cloud), cloud) for cloud in clouds.CLOUD_REGISTRY.values()
-    ]
-    clouds_to_check.append(('Cloudflare, for R2 object store', cloudflare))
+    if clouds is not None:
+        clouds_to_check: List[Tuple[str, Any]] = []
+        for cloud in clouds:
+            if cloud.lower() == 'cloudflare':
+                clouds_to_check.append(
+                    ('Cloudflare, for R2 object store', cloudflare))
+            else:
+                cloud_obj = sky_clouds.CLOUD_REGISTRY.from_str(cloud)
+                assert cloud_obj is not None, f'Cloud {cloud!r} not found'
+                clouds_to_check.append((repr(cloud_obj), cloud_obj))
+    else:
+        clouds_to_check = [(repr(cloud_obj), cloud_obj)
+                           for cloud_obj in sky_clouds.CLOUD_REGISTRY.values()]
+        clouds_to_check.append(('Cloudflare, for R2 object store', cloudflare))
 
     for cloud_tuple in sorted(clouds_to_check):
         check_one_cloud(cloud_tuple)
 
-    # Cloudflare is not a real cloud in clouds.CLOUD_REGISTRY, and should not be
-    # inserted into the DB (otherwise `sky launch` and other code would error
-    # out when it's trying to look it up in the registry).
-    enabled_clouds = [
+    # Cloudflare is not a real cloud in sky_clouds.CLOUD_REGISTRY, and should
+    # not be inserted into the DB (otherwise `sky launch` and other code would
+    # error out when it's trying to look it up in the registry).
+    enabled_clouds_set = {
         cloud for cloud in enabled_clouds if not cloud.startswith('Cloudflare')
-    ]
-    global_user_state.set_enabled_clouds(enabled_clouds)
+    }
+    disabled_clouds_set = {
+        cloud for cloud in disabled_clouds if not cloud.startswith('Cloudflare')
+    }
+    previously_enabled_clouds_set = {
+        repr(cloud) for cloud in global_user_state.get_cached_enabled_clouds()
+    }
+
+    # Determine the set of enabled clouds: previously enabled clouds + newly
+    # enabled clouds - newly disabled clouds.
+    all_enabled_clouds = ((previously_enabled_clouds_set | enabled_clouds_set) -
+                          disabled_clouds_set)
+    global_user_state.set_enabled_clouds(list(all_enabled_clouds))
 
-    if len(enabled_clouds) == 0:
+    if len(all_enabled_clouds) == 0:
         echo(
             click.style(
                 'No cloud is enabled. SkyPilot will not be able to run any '
                 'task. Run `sky check` for more info.',
                 fg='red',
                 bold=True))
         raise SystemExit()
     else:
+        clouds_arg = (' ' +
+                      ' '.join(disabled_clouds) if clouds is not None else '')
         echo(
             click.style(
                 '\nTo enable a cloud, follow the hints above and rerun: ',
-                dim=True) + click.style('sky check', bold=True) + '\n' +
-            click.style(
+                dim=True) + click.style(f'sky check{clouds_arg}', bold=True) +
+            '\n' + click.style(
                 'If any problems remain, refer to detailed docs at: '
                 'https://skypilot.readthedocs.io/en/latest/getting-started/installation.html',  # pylint: disable=line-too-long
                 dim=True))
 
         # Pretty print for UX.
         if not quiet:
             enabled_clouds_str = '\n  :heavy_check_mark: '.join(
-                [''] + sorted(enabled_clouds))
+                [''] + sorted(all_enabled_clouds))
             rich.print('\n[green]:tada: Enabled clouds :tada:'
                        f'{enabled_clouds_str}[/green]')
 
 
 def get_cached_enabled_clouds_or_refresh(
-        raise_if_no_cloud_access: bool = False) -> List[clouds.Cloud]:
+        raise_if_no_cloud_access: bool = False) -> List[sky_clouds.Cloud]:
     """Returns cached enabled clouds and if no cloud is enabled, refresh.
 
     This function will perform a refresh if no public cloud is enabled.
 
     Args:
         raise_if_no_cloud_access: if True, raise an exception if no public
             cloud is enabled.
@@ -116,25 +146,26 @@
             raise exceptions.NoCloudAccessError(
                 'Cloud access is not set up. Run: '
                 f'{colorama.Style.BRIGHT}sky check{colorama.Style.RESET_ALL}')
     return cached_enabled_clouds
 
 
 def get_cloud_credential_file_mounts(
-        excluded_clouds: Optional[Iterable[clouds.Cloud]]) -> Dict[str, str]:
+        excluded_clouds: Optional[Iterable[sky_clouds.Cloud]]
+) -> Dict[str, str]:
     """Returns the files necessary to access all enabled clouds.
 
     Returns a dictionary that will be added to a task's file mounts
     and a list of patterns that will be excluded (used as rsync_exclude).
     """
     enabled_clouds = get_cached_enabled_clouds_or_refresh()
     file_mounts = {}
     for cloud in enabled_clouds:
         if (excluded_clouds is not None and
-                clouds.cloud_in_iterable(cloud, excluded_clouds)):
+                sky_clouds.cloud_in_iterable(cloud, excluded_clouds)):
             continue
         cloud_file_mounts = cloud.get_credential_file_mounts()
         file_mounts.update(cloud_file_mounts)
     # Currently, get_cached_enabled_clouds_or_refresh() does not support r2 as
     # only clouds with computing instances are marked as enabled by skypilot.
     # This will be removed when cloudflare/r2 is added as a 'cloud'.
     r2_is_enabled, _ = cloudflare.check_credentials()
```

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/cli.py` & `skypilot_nightly-1.0.0.dev20240516/sky/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 import dotenv
 from rich import progress as rich_progress
 import yaml
 
 import sky
 from sky import backends
 from sky import check as sky_check
-from sky import clouds
+from sky import clouds as sky_clouds
 from sky import core
 from sky import exceptions
 from sky import global_user_state
 from sky import jobs as managed_jobs
 from sky import serve as serve_lib
 from sky import sky_logging
 from sky import status_lib
@@ -475,15 +475,15 @@
         ports: Optional[Tuple[str]] = None) -> Dict[str, Any]:
     """Parses the override parameters into a dictionary."""
     override_params: Dict[str, Any] = {}
     if cloud is not None:
         if cloud.lower() == 'none':
             override_params['cloud'] = None
         else:
-            override_params['cloud'] = clouds.CLOUD_REGISTRY.from_str(cloud)
+            override_params['cloud'] = sky_clouds.CLOUD_REGISTRY.from_str(cloud)
     if region is not None:
         if region.lower() == 'none':
             override_params['region'] = None
         else:
             override_params['region'] = region
     if zone is not None:
         if zone.lower() == 'none':
@@ -2859,31 +2859,35 @@
         subprocess_utils.run_in_parallel(_down_or_stop, clusters)
         progress.live.transient = False
         # Make sure the progress bar not mess up the terminal.
         progress.refresh()
 
 
 @cli.command()
+@click.argument('clouds', required=False, type=str, nargs=-1)
 @click.option('--verbose',
               '-v',
               is_flag=True,
               default=False,
               help='Show the activated account for each cloud.')
 @usage_lib.entrypoint
-def check(verbose: bool):
+def check(clouds: Tuple[str], verbose: bool):
     """Check which clouds are available to use.
 
     This checks access credentials for all clouds supported by SkyPilot. If a
     cloud is detected to be inaccessible, the reason and correction steps will
     be shown.
 
+    If CLOUDS are specified, checks credentials for only those clouds.
+
     The enabled clouds are cached and form the "search space" to be considered
     for each task.
     """
-    sky_check.check(verbose=verbose)
+    clouds_arg = clouds if len(clouds) > 0 else None
+    sky_check.check(verbose=verbose, clouds=clouds_arg)
 
 
 @cli.command()
 @click.argument('accelerator_str', required=False)
 @click.option('--all',
               '-a',
               is_flag=True,
@@ -2954,15 +2958,15 @@
             'The --all-regions flag is only valid when an accelerator '
             'is specified.')
     if all_regions and region is not None:
         raise click.UsageError(
             '--all-regions and --region flags cannot be used simultaneously.')
 
     # This will validate 'cloud' and raise if not found.
-    cloud_obj = clouds.CLOUD_REGISTRY.from_str(cloud)
+    cloud_obj = sky_clouds.CLOUD_REGISTRY.from_str(cloud)
     service_catalog.validate_region_zone(region, None, clouds=cloud)
     show_all = all
     if show_all and accelerator_str is not None:
         raise click.UsageError('--all is only allowed without a GPU name.')
 
     def _list_to_str(lst):
         return ', '.join([str(e) for e in lst])
@@ -2974,15 +2978,15 @@
             ['GOOGLE_TPU', 'AVAILABLE_QUANTITIES'])
         other_table = log_utils.create_table(
             ['OTHER_GPU', 'AVAILABLE_QUANTITIES'])
 
         name, quantity = None, None
 
         # Kubernetes specific bools
-        cloud_is_kubernetes = isinstance(cloud_obj, clouds.Kubernetes)
+        cloud_is_kubernetes = isinstance(cloud_obj, sky_clouds.Kubernetes)
         kubernetes_autoscaling = kubernetes_utils.get_autoscaler_type(
         ) is not None
 
         if accelerator_str is None:
             result = service_catalog.list_accelerator_counts(
                 gpus_only=True,
                 clouds=cloud,
```

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/cloud_stores.py` & `skypilot_nightly-1.0.0.dev20240516/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/__init__.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/aws.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/azure.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/cloud.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/cloud_registry.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/cloud_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/cudo.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/fluidstack.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/gcp.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/ibm.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/kubernetes.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/lambda_cloud.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/oci.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/paperspace.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/paperspace.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/runpod.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/runpod.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/scp.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/__init__.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/aws_catalog.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/azure_catalog.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/common.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/config.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/cudo_catalog.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/cudo_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/fluidstack_catalog.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/fluidstack_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/kubernetes_catalog.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/kubernetes_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/oci_catalog.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/paperspace_catalog.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/paperspace_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/runpod_catalog.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/runpod_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/scp_catalog.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/vsphere_catalog.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/service_catalog/vsphere_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/gcp_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/utils/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/lambda_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/utils/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/oci_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/utils/oci_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/scp_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/utils/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/clouds/vsphere.py` & `skypilot_nightly-1.0.0.dev20240516/sky/clouds/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/core.py` & `skypilot_nightly-1.0.0.dev20240516/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/dag.py` & `skypilot_nightly-1.0.0.dev20240516/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/data/data_transfer.py` & `skypilot_nightly-1.0.0.dev20240516/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/data/data_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/data/mounting_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/data/storage.py` & `skypilot_nightly-1.0.0.dev20240516/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/data/storage_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/exceptions.py` & `skypilot_nightly-1.0.0.dev20240516/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/execution.py` & `skypilot_nightly-1.0.0.dev20240516/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/global_user_state.py` & `skypilot_nightly-1.0.0.dev20240516/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/jobs/__init__.py` & `skypilot_nightly-1.0.0.dev20240516/sky/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/jobs/constants.py` & `skypilot_nightly-1.0.0.dev20240516/sky/jobs/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/jobs/controller.py` & `skypilot_nightly-1.0.0.dev20240516/sky/jobs/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/jobs/core.py` & `skypilot_nightly-1.0.0.dev20240516/sky/jobs/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/dashboard.py` & `skypilot_nightly-1.0.0.dev20240516/sky/jobs/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/static/favicon.ico` & `skypilot_nightly-1.0.0.dev20240516/sky/jobs/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/templates/index.html` & `skypilot_nightly-1.0.0.dev20240516/sky/jobs/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/jobs/recovery_strategy.py` & `skypilot_nightly-1.0.0.dev20240516/sky/jobs/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/jobs/state.py` & `skypilot_nightly-1.0.0.dev20240516/sky/jobs/state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/jobs/utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/optimizer.py` & `skypilot_nightly-1.0.0.dev20240516/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/__init__.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/__init__.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/config.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/instance.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/azure/instance.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/azure/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/common.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/__init__.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/cudo/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/cudo_machine_type.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/cudo/cudo_machine_type.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/cudo_wrapper.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/cudo/cudo_wrapper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/instance.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/cudo/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/docker_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/fluidstack/__init__.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/fluidstack/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/fluidstack/fluidstack_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/fluidstack/fluidstack_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/fluidstack/instance.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/fluidstack/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/__init__.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/config.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/constants.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/instance.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/instance_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/instance_setup.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/instance_setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/__init__.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/config.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/instance.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/network.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/network.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/network_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/network_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/logging.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/logging.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/metadata_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/__init__.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/paperspace/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/config.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/paperspace/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/constants.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/paperspace/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/instance.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/paperspace/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/paperspace/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/provisioner.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/provisioner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/runpod/instance.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/runpod/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/runpod/utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/runpod/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/__init__.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/cls_api_client.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/cls_api_client.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/cls_api_helper.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/cls_api_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/metadata_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/service_manager.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/service_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/service_manager_factory.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/service_manager_factory.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/ssl_helper.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/ssl_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/vapiconnect.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/vapiconnect.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/vim_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/common/vim_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/instance.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/vsphere_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/provision/vsphere/vsphere_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/resources.py` & `skypilot_nightly-1.0.0.dev20240516/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/serve/__init__.py` & `skypilot_nightly-1.0.0.dev20240516/sky/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/serve/autoscalers.py` & `skypilot_nightly-1.0.0.dev20240516/sky/serve/autoscalers.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/serve/constants.py` & `skypilot_nightly-1.0.0.dev20240516/sky/serve/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/serve/controller.py` & `skypilot_nightly-1.0.0.dev20240516/sky/serve/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/serve/core.py` & `skypilot_nightly-1.0.0.dev20240516/sky/serve/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/serve/load_balancer.py` & `skypilot_nightly-1.0.0.dev20240516/sky/serve/load_balancer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/serve/load_balancing_policies.py` & `skypilot_nightly-1.0.0.dev20240516/sky/serve/load_balancing_policies.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/serve/replica_managers.py` & `skypilot_nightly-1.0.0.dev20240516/sky/serve/replica_managers.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/serve/serve_state.py` & `skypilot_nightly-1.0.0.dev20240516/sky/serve/serve_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/serve/serve_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/serve/serve_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/serve/service.py` & `skypilot_nightly-1.0.0.dev20240516/sky/serve/service.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/serve/service_spec.py` & `skypilot_nightly-1.0.0.dev20240516/sky/serve/service_spec.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/setup_files/MANIFEST.in` & `skypilot_nightly-1.0.0.dev20240516/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/setup_files/setup.py` & `skypilot_nightly-1.0.0.dev20240516/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/sky_logging.py` & `skypilot_nightly-1.0.0.dev20240516/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/LICENSE` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/attempt_skylet.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/autostop_lib.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/configs.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/constants.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/events.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/job_lib.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/log_lib.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/log_lib.pyi` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/log_lib.pyi`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/azure-config-template.json` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/config.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/node_provider.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/command_runner.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/ibm/node_provider.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/ibm/utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/oci/node_provider.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/oci/query_helper.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/scp/config.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/scp/node_provider.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/__init__.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/worker.py.patch` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/skylet.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skylet/subprocess_daemon.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/skypilot_config.py` & `skypilot_nightly-1.0.0.dev20240516/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/status_lib.py` & `skypilot_nightly-1.0.0.dev20240516/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/task.py` & `skypilot_nightly-1.0.0.dev20240516/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/aws-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/azure-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/cudo-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/cudo-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/fluidstack-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/fluidstack-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/gcp-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/ibm-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/jobs-controller.yaml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/jobs-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-ingress.yml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/kubernetes-ingress.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-port-forward-proxy-command.sh.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/kubernetes-port-forward-proxy-command.sh.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/kubernetes-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-ssh-jump.yml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/kubernetes-ssh-jump.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/lambda-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/local-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/oci-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/paperspace-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/paperspace-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/runpod-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/runpod-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/scp-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/sky-serve-controller.yaml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/sky-serve-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/templates/vsphere-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240516/sky/templates/vsphere-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/usage/constants.py` & `skypilot_nightly-1.0.0.dev20240516/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/usage/usage_lib.py` & `skypilot_nightly-1.0.0.dev20240516/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/accelerator_registry.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/cli_utils/status_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/cluster_yaml_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/cluster_yaml_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/command_runner.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/command_runner.pyi` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/command_runner.pyi`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/common_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/controller_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/controller_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/dag_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/db_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/env_options.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/create_cluster.sh` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/create_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/delete_cluster.sh` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/delete_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/generate_kind_config.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/generate_kind_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/generate_static_kubeconfig.sh` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/generate_static_kubeconfig.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/gpu_labeler.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/gpu_labeler.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes_enums.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/kubernetes_enums.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/log_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/resources_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/resources_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/rich_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/schemas.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/subprocess_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/timeline.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/ux_utils.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/sky/utils/validator.py` & `skypilot_nightly-1.0.0.dev20240516/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/PKG-INFO` & `skypilot_nightly-1.0.0.dev20240516/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240515
+Version: 1.0.0.dev20240516
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot_nightly-1.0.0.dev20240516/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/requires.txt` & `skypilot_nightly-1.0.0.dev20240516/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/tests/test_cli.py` & `skypilot_nightly-1.0.0.dev20240516/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/tests/test_config.py` & `skypilot_nightly-1.0.0.dev20240516/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/tests/test_jobs.py` & `skypilot_nightly-1.0.0.dev20240516/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/tests/test_jobs_and_serve.py` & `skypilot_nightly-1.0.0.dev20240516/tests/test_jobs_and_serve.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/tests/test_list_accelerators.py` & `skypilot_nightly-1.0.0.dev20240516/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/tests/test_optimizer_dryruns.py` & `skypilot_nightly-1.0.0.dev20240516/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/tests/test_optimizer_random_dag.py` & `skypilot_nightly-1.0.0.dev20240516/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/tests/test_serve_autoscaler.py` & `skypilot_nightly-1.0.0.dev20240516/tests/test_serve_autoscaler.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/tests/test_smoke.py` & `skypilot_nightly-1.0.0.dev20240516/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/tests/test_storage.py` & `skypilot_nightly-1.0.0.dev20240516/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/tests/test_wheels.py` & `skypilot_nightly-1.0.0.dev20240516/tests/test_wheels.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240515/tests/test_yaml_parser.py` & `skypilot_nightly-1.0.0.dev20240516/tests/test_yaml_parser.py`

 * *Files identical despite different names*

