# Comparing `tmp/paasta-tools-1.0.0.tar.gz` & `tmp/paasta-tools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/paasta-tools-1.0.0.tar", last modified: Thu May 16 19:44:12 2024, max compression
+gzip compressed data, was "dist/paasta-tools-1.0.1.tar", last modified: Fri May 17 21:20:53 2024, max compression
```

## Comparing `paasta-tools-1.0.0.tar` & `paasta-tools-1.0.1.tar`

### file list

```diff
@@ -1,343 +1,326 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-16 19:44:10.000000 paasta-tools-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-16 19:44:10.000000 paasta-tools-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/k8s_itests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/k8s_itests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/k8s_itests/test_autoscaling.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/k8s_itests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/adhoc_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1042 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/am_i_mesos_leader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/api/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/api/api_docs/
--rw-r--r--   0 runner    (1001) docker     (127)    77060 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/api_docs/swagger.json
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/api/tweens/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/tweens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/tweens/profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/tweens/request_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/api/views/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/views/autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/views/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/views/flink.py
--rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/views/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/views/metastatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/views/pause_autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/views/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/views/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/api/views/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/apply_external_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/async_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/autoscaling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/autoscaling/autoscaling_service_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/autoscaling/forecasting.py
--rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/autoscaling/load_boost.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/autoscaling/max_all_k8s_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/autoscaling/pause_service_autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/autoscaling/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/bounce_lib.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2042 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/broadcast_log_to_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cassandracluster_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8435 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/check_autoscaler_max_instances.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1140 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/check_cassandracluster_services_replication.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7211 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/check_flink_services_health.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/check_kubernetes_api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5761 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/check_kubernetes_services_replication.py
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/check_oom_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/check_services_replication_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/check_spark_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cleanup_kubernetes_cr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cleanup_kubernetes_crd.py
--rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cleanup_kubernetes_jobs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3946 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cleanup_maintenance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cleanup_tron_namespaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8480 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/autoscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/boost.py
--rw-r--r--   0 runner    (1001) docker     (127)    12968 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/cook_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/get_docker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/get_image_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/get_latest_deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/itest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/list_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/list_deploy_queue.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    49329 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/local_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    52420 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    76217 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/mark_for_deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/mesh_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/metastatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/pause_service_autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/push_to_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/remote_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/rollback.py
--rw-r--r--   0 runner    (1001) docker     (127)    19709 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/security_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    45133 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/spark_run.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14600 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/start_stop_restart.py
--rw-r--r--   0 runner    (1001) docker     (127)    84455 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/status.py
--rw-r--r--   0 runner    (1001) docker     (127)    39825 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/cmds/wait_for_deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/cli/fsm/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/fsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/fsm/autosuggest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/cli/fsm/template/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/fsm/template/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/fsm/template/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/kubernetes-PROD.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/smartstack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/fsm_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/paasta_tabcomplete.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/cli/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/schemas/adhoc_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/schemas/autoscaling_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/cli/schemas/autotuned_defaults/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/schemas/autotuned_defaults/cassandracluster_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/schemas/autotuned_defaults/kubernetes_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/schemas/deploy_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    39538 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/schemas/eks_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    39538 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/schemas/kubernetes_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/schemas/rollback_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/schemas/service_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/schemas/smartstack_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    26509 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/schemas/tron_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    40542 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/clusterman.py
--rw-r--r--   0 runner    (1001) docker     (127)    14188 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/config_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2241 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/bounce_log_latency_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      879 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/check_manual_oapi_changes.sh
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/check_orphans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/create_dynamodb_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/create_paasta_playground.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/emit_allocated_cpu_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/get_running_task_allocation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2638 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/habitat_fixer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12334 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/ide_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/is_pod_healthy_in_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/is_pod_healthy_in_smartstack.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3861 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/kill_bad_containers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1578 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/mass-deploy-tag.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2575 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/mock_patch_checker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17885 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/paasta_update_soa_memcpu.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3959 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/render_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/rightsizer_soaconfigs_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/service_shard_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/service_shard_update.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2480 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/shared_ip_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/timeouts_metrics_prom.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2057 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/contrib/utilization_check.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3137 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/delete_kubernetes_deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/deployment_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6935 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/docker_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/docker_wrapper_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/drain_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/dump_locally_running_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/eks_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    14276 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/envoy_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16304 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/firewall_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/firewall_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/flink_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/flinkeks_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/frameworks/adhoc_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/frameworks/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    24535 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/frameworks/native_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/frameworks/native_service_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/frameworks/task_store.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      248 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/generate_all_deployments
--rwxr-xr-x   0 runner    (1001) docker     (127)     9674 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/generate_deployments_for_service.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4617 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/generate_services_file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/generate_services_yaml.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      835 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/get_mesos_leader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/hacheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/instance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/instance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/instance/hpa_metrics_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    46810 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/instance/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/iptables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/kafkacluster_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/kubernetes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/kubernetes/application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/kubernetes/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16009 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/kubernetes/application/controller_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/kubernetes/application/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/kubernetes/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/kubernetes/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5287 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/kubernetes/bin/kubernetes_remove_evicted_pods.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/kubernetes/bin/paasta_cleanup_stale_nodes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28779 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/kubernetes/bin/paasta_secrets_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)   166865 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/kubernetes_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3910 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/list_kubernetes_service_instances.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1679 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/list_tron_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/log_task_lifecycle_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    25773 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/long_running_service_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/mac_address.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/marathon_dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/mesos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/mesos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/mesos/cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/mesos/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/mesos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/mesos/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/mesos/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/mesos/master.py
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/mesos/mesos_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/mesos/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/mesos/slave.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/mesos/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/mesos/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/mesos/zookeeper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31450 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/mesos_maintenance.py
--rw-r--r--   0 runner    (1001) docker     (127)    35836 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/mesos_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/metrics/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    39707 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/metrics/metastatus_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/metrics/metrics_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/monitoring/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/monitoring/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5883 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/monitoring/check_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/monitoring/check_k8s_api_performance.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1748 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/monitoring/check_mesos_active_frameworks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1720 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/monitoring/check_mesos_duplicate_frameworks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      937 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/monitoring/check_mesos_quorum.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2070 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/monitoring/kill_orphaned_docker_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/monitoring_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/monkrelaycluster_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5758 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/native_mesos_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/nrtsearchservice_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/nrtsearchserviceeks_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/oom_logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4375 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paasta_cluster_boost.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paasta_deploy_tron_jobs
--rwxr-xr-x   0 runner    (1001) docker     (127)     4099 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paasta_execute_docker_command.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4571 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paasta_maintenance.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17402 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paasta_metastatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paasta_native_serviceinit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25707 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paasta_remote_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paasta_service_config_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/api/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/api/autoscaler_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    24615 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/api/resources_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    63296 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/api/service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35200 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16583 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/adhoc_launch_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/autoscaler_count_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/deploy_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/deploy_queue_service_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/envoy_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/envoy_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/envoy_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/flink_cluster_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/flink_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/flink_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/flink_job_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/flink_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/float_and_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/hpa_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/inline_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/inline_response2001.py
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_bounce_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_mesh_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status_cassandracluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status_flink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status_kafkacluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status_kubernetes_autoscaling_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status_kubernetes_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status_tron.py
--rw-r--r--   0 runner    (1001) docker     (127)     6825 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/integer_and_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/kubernetes_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/kubernetes_container_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/kubernetes_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/kubernetes_pod.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/kubernetes_pod_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/kubernetes_pod_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/kubernetes_replica_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/kubernetes_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/meta_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/resource_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/resource_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/smartstack_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/smartstack_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/smartstack_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model/task_tail_lines.py
--rw-r--r--   0 runner    (1001) docker     (127)    74015 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12197 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/paastaapi/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/prune_completed_pods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/puppet_service_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/remote_git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/run-paasta-api-in-dev-mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/run-paasta-api-playground.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/secret_providers/
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/secret_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/secret_providers/vault.py
--rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/secret_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/setup_istio_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/setup_kubernetes_cr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/setup_kubernetes_crd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4642 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/setup_kubernetes_internal_crd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12646 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/setup_kubernetes_job.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37673 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/setup_prometheus_adapter_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5028 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/setup_tron_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)    25551 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/smartstack_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/spark_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1421 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/synapse_srv_namespaces_fact.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools/tron/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/tron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/tron/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/tron/tron_command_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/tron/tron_timeutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    48900 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/tron_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)   145790 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/paasta_tools/vitesscluster_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/paasta_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/requirements-minimal.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:44:12.000000 paasta-tools-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-16 19:44:11.000000 paasta-tools-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/k8s_itests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/k8s_itests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/k8s_itests/test_autoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/k8s_itests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/adhoc_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/api/api_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    75493 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/api_docs/swagger.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/api/tweens/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/tweens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/tweens/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/tweens/request_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/api/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/flink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/pause_autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/apply_external_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/async_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/autoscaling/autoscaling_service_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/autoscaling/forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/autoscaling/max_all_k8s_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/autoscaling/pause_service_autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/autoscaling/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/bounce_lib.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2042 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/broadcast_log_to_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cassandracluster_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8435 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/check_autoscaler_max_instances.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1140 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/check_cassandracluster_services_replication.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7211 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/check_flink_services_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/check_kubernetes_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5761 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/check_kubernetes_services_replication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/check_oom_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/check_services_replication_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/check_spark_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cleanup_kubernetes_cr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cleanup_kubernetes_crd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cleanup_kubernetes_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cleanup_tron_namespaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8426 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/autoscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12968 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/cook_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/get_docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/get_image_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/get_latest_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/itest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/list_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/list_deploy_queue.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    49329 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/local_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52420 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76217 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/mark_for_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/mesh_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/pause_service_autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/push_to_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/remote_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/rollback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19709 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/security_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45133 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/spark_run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14600 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/start_stop_restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81205 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39825 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/wait_for_deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/autosuggest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/template/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/template/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/kubernetes-PROD.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/smartstack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/paasta_tabcomplete.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/adhoc_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/autoscaling_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/autotuned_defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/autotuned_defaults/cassandracluster_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/autotuned_defaults/kubernetes_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/deploy_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    39538 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/eks_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    39538 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/kubernetes_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/rollback_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/service_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/smartstack_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26509 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/tron_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36829 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/clusterman.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14188 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/config_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2241 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/bounce_log_latency_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      879 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/check_manual_oapi_changes.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/check_orphans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/create_dynamodb_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/create_paasta_playground.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/emit_allocated_cpu_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/get_running_task_allocation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2638 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/habitat_fixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12334 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/ide_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/is_pod_healthy_in_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/is_pod_healthy_in_smartstack.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3861 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/kill_bad_containers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1578 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/mass-deploy-tag.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2575 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/mock_patch_checker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17885 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/paasta_update_soa_memcpu.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3959 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/render_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/rightsizer_soaconfigs_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/service_shard_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/service_shard_update.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2480 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/shared_ip_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/timeouts_metrics_prom.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3137 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/delete_kubernetes_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/deployment_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6935 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/docker_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/docker_wrapper_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/drain_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/dump_locally_running_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/eks_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14276 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/envoy_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16304 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/firewall_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/firewall_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/flink_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/flinkeks_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/frameworks/adhoc_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/frameworks/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24535 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/frameworks/native_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/frameworks/native_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/frameworks/task_store.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      248 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/generate_all_deployments
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9674 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/generate_deployments_for_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4617 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/generate_services_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/generate_services_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/hacheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/instance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/instance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/instance/hpa_metrics_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46810 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/instance/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/iptables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kafkacluster_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16009 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/application/controller_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/application/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5287 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/bin/kubernetes_remove_evicted_pods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/bin/paasta_cleanup_stale_nodes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28779 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/bin/paasta_secrets_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)   166865 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3910 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/list_kubernetes_service_instances.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1679 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/list_tron_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/log_task_lifecycle_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25773 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/long_running_service_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mac_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/marathon_dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/mesos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/mesos_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/slave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/zookeeper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31450 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos_maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35540 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/metrics/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37790 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/metrics/metastatus_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/metrics/metrics_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/monitoring/check_k8s_api_performance.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2070 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/monitoring/kill_orphaned_docker_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/monitoring_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/monkrelaycluster_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/nrtsearchservice_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/nrtsearchserviceeks_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/oom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paasta_deploy_tron_jobs
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4099 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paasta_execute_docker_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paasta_native_serviceinit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25707 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paasta_remote_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paasta_service_config_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/api/autoscaler_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20369 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/api/resources_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63296 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/api/service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35200 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16583 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/adhoc_launch_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/autoscaler_count_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/deploy_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/deploy_queue_service_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/envoy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/envoy_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/envoy_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_cluster_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_job_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/float_and_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/hpa_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/inline_response2001.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_bounce_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_mesh_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_cassandracluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_flink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_kafkacluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_kubernetes_autoscaling_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_kubernetes_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_tron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6825 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/integer_and_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_container_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_pod_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_pod_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_replica_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/resource_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/resource_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/smartstack_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/smartstack_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/smartstack_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/task_tail_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74015 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12197 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/prune_completed_pods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/puppet_service_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/remote_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/run-paasta-api-in-dev-mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/run-paasta-api-playground.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/secret_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/secret_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/secret_providers/vault.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/secret_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/setup_istio_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/setup_kubernetes_cr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/setup_kubernetes_crd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4642 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/setup_kubernetes_internal_crd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12646 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/setup_kubernetes_job.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37673 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/setup_prometheus_adapter_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5028 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/setup_tron_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25551 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/smartstack_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/spark_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1421 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/synapse_srv_namespaces_fact.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/tron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/tron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/tron/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/tron/tron_command_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/tron/tron_timeutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48900 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/tron_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)   141092 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/vitesscluster_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/requirements-minimal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/setup.py
```

### Comparing `paasta-tools-1.0.0/README.md` & `paasta-tools-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/k8s_itests/test_autoscaling.py` & `paasta-tools-1.0.1/k8s_itests/test_autoscaling.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/k8s_itests/utils.py` & `paasta-tools-1.0.1/k8s_itests/utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/__init__.py` & `paasta-tools-1.0.1/paasta_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # limitations under the License.
 #
 # It is imperative that this file not contain any imports from our
 # dependencies. Since this file is imported from setup.py in the
 # setup phase, the dependencies may not exist on disk yet.
 #
 # Don't bump version manually. See `make release` docs in ./Makefile
-__version__ = "1.0.0"
+__version__ = "1.0.1"
```

### Comparing `paasta-tools-1.0.0/paasta_tools/adhoc_tools.py` & `paasta-tools-1.0.1/paasta_tools/adhoc_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/am_i_mesos_leader.py` & `paasta-tools-1.0.1/paasta_tools/api/views/version.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,29 +9,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-Usage: ./am_i_mesos_leader.py
-
-Check if this host is the current mesos-master leader.
-This is done by simply calling mesos_tools.is_mesos_leader.
-Exits 0 if this is the leader, and 1 if it isn't.
+PaaSTA service list (instances) etc.
 """
-from sys import exit
-
-from paasta_tools.mesos_tools import is_mesos_leader
-
+from pyramid.view import view_config
 
-def main():
-    if is_mesos_leader():
-        print(True)
-        exit(0)
-    else:
-        print(False)
-        exit(1)
+from paasta_tools import __version__
 
 
-if __name__ == "__main__":
-    main()
+@view_config(route_name="version", request_method="GET", renderer="json")
+def version(request):
+    return __version__
```

### Comparing `paasta-tools-1.0.0/paasta_tools/api/__init__.py` & `paasta-tools-1.0.1/paasta_tools/api/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/api/api.py` & `paasta-tools-1.0.1/paasta_tools/api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,14 @@
     )
     config.add_route(
         "service_autoscaler.pause.get",
         "/v1/service_autoscaler/pause",
         request_method="GET",
     )
     config.add_route("version", "/v1/version")
-    config.add_route("metastatus", "/v1/metastatus")
     config.add_route("deploy_queue.list", "/v1/deploy_queue")
     config.scan()
     return CORS(
         config.make_wsgi_app(), headers="*", methods="*", maxage="180", origin="*"
     )
```

### Comparing `paasta-tools-1.0.0/paasta_tools/api/api_docs/swagger.json` & `paasta-tools-1.0.1/paasta_tools/api/api_docs/swagger.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958133971291867%*

 * *Differences: {"'definitions'": "{delete: ['MetaStatus']}", "'paths'": "{delete: ['/metastatus']}"}*

```diff
@@ -1040,28 +1040,14 @@
                 "type": {
                     "description": "Type of version (ReplicaSet or ControllerRevision)",
                     "type": "string"
                 }
             },
             "type": "object"
         },
-        "MetaStatus": {
-            "description": "Result of `paasta metastatus` command",
-            "properties": {
-                "exit_code": {
-                    "description": "Exit code from `paasta metastatus` command",
-                    "type": "integer"
-                },
-                "output": {
-                    "description": "Output from `paasta metastatus` command",
-                    "type": "string"
-                }
-            },
-            "type": "object"
-        },
         "Resource": {
             "items": {
                 "$ref": "#/definitions/ResourceItem"
             },
             "type": "array"
         },
         "ResourceItem": {
@@ -1391,44 +1377,14 @@
                 },
                 "summary": "Get overview of a flink cluster",
                 "tags": [
                     "service"
                 ]
             }
         },
-        "/metastatus": {
-            "get": {
-                "operationId": "metastatus",
-                "parameters": [
-                    {
-                        "collectionFormat": "csv",
-                        "description": "comma separated list of command arguments",
-                        "in": "query",
-                        "items": {
-                            "type": "string"
-                        },
-                        "name": "cmd_args",
-                        "required": true,
-                        "type": "array"
-                    }
-                ],
-                "responses": {
-                    "200": {
-                        "description": "Detailed metastatus",
-                        "schema": {
-                            "$ref": "#/definitions/MetaStatus"
-                        }
-                    },
-                    "500": {
-                        "description": "Metastatus failure"
-                    }
-                },
-                "summary": "Get metastatus"
-            }
-        },
         "/resources/utilization": {
             "get": {
                 "operationId": "resources",
                 "parameters": [
                     {
                         "collectionFormat": "csv",
                         "description": "comma separated list of keys to group by",
```

### Comparing `paasta-tools-1.0.0/paasta_tools/api/client.py` & `paasta-tools-1.0.1/paasta_tools/api/client.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/api/settings.py` & `paasta-tools-1.0.1/paasta_tools/api/settings.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/api/tweens/profiling.py` & `paasta-tools-1.0.1/paasta_tools/api/tweens/profiling.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/api/tweens/request_logger.py` & `paasta-tools-1.0.1/paasta_tools/api/tweens/request_logger.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/api/views/__init__.py` & `paasta-tools-1.0.1/paasta_tools/api/views/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/api/views/autoscaler.py` & `paasta-tools-1.0.1/paasta_tools/api/views/autoscaler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/api/views/exception.py` & `paasta-tools-1.0.1/paasta_tools/api/views/exception.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/api/views/flink.py` & `paasta-tools-1.0.1/paasta_tools/api/views/flink.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/api/views/instance.py` & `paasta-tools-1.0.1/paasta_tools/api/views/instance.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/api/views/pause_autoscaler.py` & `paasta-tools-1.0.1/paasta_tools/api/views/pause_autoscaler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/api/views/resources.py` & `paasta-tools-1.0.1/paasta_tools/api/views/resources.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/api/views/service.py` & `paasta-tools-1.0.1/paasta_tools/api/views/service.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/apply_external_resources.py` & `paasta-tools-1.0.1/paasta_tools/apply_external_resources.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/async_utils.py` & `paasta-tools-1.0.1/paasta_tools/async_utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/autoscaling/autoscaling_service_lib.py` & `paasta-tools-1.0.1/paasta_tools/autoscaling/autoscaling_service_lib.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/autoscaling/forecasting.py` & `paasta-tools-1.0.1/paasta_tools/autoscaling/forecasting.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/autoscaling/max_all_k8s_services.py` & `paasta-tools-1.0.1/paasta_tools/autoscaling/max_all_k8s_services.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/autoscaling/pause_service_autoscaler.py` & `paasta-tools-1.0.1/paasta_tools/autoscaling/pause_service_autoscaler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/autoscaling/utils.py` & `paasta-tools-1.0.1/paasta_tools/autoscaling/utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/bounce_lib.py` & `paasta-tools-1.0.1/paasta_tools/bounce_lib.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/broadcast_log_to_services.py` & `paasta-tools-1.0.1/paasta_tools/broadcast_log_to_services.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cassandracluster_tools.py` & `paasta-tools-1.0.1/paasta_tools/cassandracluster_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/check_autoscaler_max_instances.py` & `paasta-tools-1.0.1/paasta_tools/check_autoscaler_max_instances.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/check_cassandracluster_services_replication.py` & `paasta-tools-1.0.1/paasta_tools/check_cassandracluster_services_replication.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/check_flink_services_health.py` & `paasta-tools-1.0.1/paasta_tools/check_flink_services_health.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/check_kubernetes_api.py` & `paasta-tools-1.0.1/paasta_tools/check_kubernetes_api.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/check_kubernetes_services_replication.py` & `paasta-tools-1.0.1/paasta_tools/check_kubernetes_services_replication.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/check_oom_events.py` & `paasta-tools-1.0.1/paasta_tools/check_oom_events.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/check_services_replication_tools.py` & `paasta-tools-1.0.1/paasta_tools/check_services_replication_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/check_spark_jobs.py` & `paasta-tools-1.0.1/paasta_tools/check_spark_jobs.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cleanup_kubernetes_cr.py` & `paasta-tools-1.0.1/paasta_tools/cleanup_kubernetes_cr.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cleanup_kubernetes_crd.py` & `paasta-tools-1.0.1/paasta_tools/cleanup_kubernetes_crd.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cleanup_kubernetes_jobs.py` & `paasta-tools-1.0.1/paasta_tools/cleanup_kubernetes_jobs.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cleanup_tron_namespaces.py` & `paasta-tools-1.0.1/paasta_tools/cleanup_tron_namespaces.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/__init__.py` & `paasta-tools-1.0.1/paasta_tools/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cli.py` & `paasta-tools-1.0.1/paasta_tools/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,30 +97,28 @@
     module_name = "paasta_tools.cli.cmds.%s" % command
     add_subparser_fn = load_method(module_name, "add_subparser")
     add_subparser_fn(subparsers)
 
 
 PAASTA_SUBCOMMANDS = {
     "autoscale": "autoscale",
-    "boost": "boost",
     "check": "check",
     "cook-image": "cook_image",
     "get-docker-image": "get_docker_image",
     "get-image-version": "get_image_version",
     "get-latest-deployment": "get_latest_deployment",
     "info": "info",
     "itest": "itest",
     "list-clusters": "list_clusters",
     "list-deploy-queue": "list_deploy_queue",
     "list": "list",
     "local-run": "local_run",
     "logs": "logs",
     "mark-for-deployment": "mark_for_deployment",
     "mesh-status": "mesh_status",
-    "metastatus": "metastatus",
     "pause_service_autoscaler": "pause_service_autoscaler",
     "push-to-registry": "push_to_registry",
     "remote-run": "remote_run",
     "rollback": "rollback",
     "secret": "secret",
     "security-check": "security_check",
     "spark-run": "spark_run",
```

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/__init__.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/autoscale.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/autoscale.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/check.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/check.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/cook_image.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/cook_image.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/get_docker_image.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/get_docker_image.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/get_image_version.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/get_image_version.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/get_latest_deployment.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/get_latest_deployment.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/info.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/info.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/itest.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/itest.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/list.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/list.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/list_clusters.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/list_clusters.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/list_deploy_queue.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/list_deploy_queue.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/local_run.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/local_run.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/logs.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/logs.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/mark_for_deployment.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/mark_for_deployment.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/mesh_status.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/mesh_status.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/pause_service_autoscaler.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/pause_service_autoscaler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/push_to_registry.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/push_to_registry.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/remote_run.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/remote_run.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/rollback.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/rollback.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/secret.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/secret.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/security_check.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/security_check.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/spark_run.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/spark_run.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/start_stop_restart.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/start_stop_restart.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/status.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 from paasta_tools.flinkeks_tools import FlinkEksDeploymentConfig
 from paasta_tools.kafkacluster_tools import KafkaClusterDeploymentConfig
 from paasta_tools.kubernetes_tools import format_pod_event_messages
 from paasta_tools.kubernetes_tools import format_tail_lines_for_kubernetes_pod
 from paasta_tools.kubernetes_tools import KubernetesDeploymentConfig
 from paasta_tools.kubernetes_tools import KubernetesDeployStatus
 from paasta_tools.kubernetes_tools import paasta_prefixed
-from paasta_tools.mesos_tools import format_tail_lines_for_mesos_task
 from paasta_tools.monitoring_tools import get_team
 from paasta_tools.monitoring_tools import list_teams
 from paasta_tools.paasta_service_config_loader import PaastaServiceConfigLoader
 from paasta_tools.paastaapi.model.flink_job_details import FlinkJobDetails
 from paasta_tools.paastaapi.model.flink_jobs import FlinkJobs
 from paasta_tools.paastaapi.models import InstanceStatusKubernetesV2
 from paasta_tools.paastaapi.models import KubernetesContainerV2
@@ -424,105 +423,14 @@
     ]
     row = [str(e) for e in row]
     table = [f"  {line}" for line in format_table([headers, row])]
     output.extend(table)
     return output
 
 
-def create_mesos_running_tasks_table(running_tasks):
-    rows = []
-    table_header = [
-        "Mesos Task ID",
-        "Host deployed to",
-        "Ram",
-        "CPU",
-        "Deployed at what localtime",
-    ]
-    rows.append(table_header)
-    for task in running_tasks or []:
-        mem_string = get_mesos_task_memory_string(task)
-        cpu_string = get_mesos_task_cpu_string(task)
-        deployed_at = datetime.fromtimestamp(task.deployed_timestamp)
-        deployed_at_string = "{} ({})".format(
-            deployed_at.strftime("%Y-%m-%dT%H:%M"), humanize.naturaltime(deployed_at)
-        )
-
-        rows.append(
-            [task.id, task.hostname, mem_string, cpu_string, deployed_at_string]
-        )
-        rows.extend(format_tail_lines_for_mesos_task(task.tail_lines, task.id))
-
-    return format_table(rows)
-
-
-def get_mesos_task_memory_string(task):
-    if task.rss.value is None or task.mem_limit.value is None:
-        return task.rss.error_message or task.mem_limit.error_message
-    elif task.mem_limit.value == 0:
-        return "Undef"
-    else:
-        mem_percent = 100 * task.rss.value / task.mem_limit.value
-        mem_string = "%d/%dMB" % (
-            (task.rss.value / 1024 / 1024),
-            (task.mem_limit.value / 1024 / 1024),
-        )
-        if mem_percent > 90:
-            return PaastaColors.red(mem_string)
-        else:
-            return mem_string
-
-
-def get_mesos_task_cpu_string(task):
-    if task.cpu_shares.value is None or task.cpu_used_seconds.value is None:
-        return task.cpu_shares.error_message
-    else:
-        # The total time a task has been allocated is the total time the task has
-        # been running multiplied by the "shares" a task has.
-        # (see https://github.com/mesosphere/mesos/blob/0b092b1b0/src/webui/master/static/js/controllers.js#L140)
-        allocated_seconds = task.cpu_shares.value * task.duration_seconds
-        if allocated_seconds == 0:
-            return "Undef"
-        else:
-            cpu_percent = round(
-                100 * (task.cpu_used_seconds.value / allocated_seconds), 1
-            )
-            cpu_string = "%s%%" % cpu_percent
-            if cpu_percent > 90:
-                return PaastaColors.red(cpu_string)
-            else:
-                return cpu_string
-
-
-def create_mesos_non_running_tasks_table(non_running_tasks):
-    rows = []
-    table_header = [
-        "Mesos Task ID",
-        "Host deployed to",
-        "Deployed at what localtime",
-        "Status",
-    ]
-    rows.append(table_header)
-
-    for task in non_running_tasks or []:
-        if task.deployed_timestamp is None:
-            deployed_at_string = "Unknown"
-        else:
-            deployed_at = datetime.fromtimestamp(task.deployed_timestamp)
-            deployed_at_string = "{} ({})".format(
-                deployed_at.strftime("%Y-%m-%dT%H:%M"),
-                humanize.naturaltime(deployed_at),
-            )
-
-        rows.append([task.id, task.hostname, deployed_at_string, task.state])
-        rows.extend(format_tail_lines_for_mesos_task(task.tail_lines, task.id))
-
-    table = format_table(rows)
-    return [PaastaColors.grey(formatted_row) for formatted_row in table]
-
-
 def format_kubernetes_pod_table(pods, verbose: int):
     rows: List[Union[tuple, str]] = [
         ("Pod ID", "Host deployed to", "Deployed at what localtime", "Health")
     ]
     for pod in pods:
         local_deployed_datetime = datetime.fromtimestamp(pod.deployed_timestamp)
         hostname = f"{pod.host}" if pod.host is not None else PaastaColors.grey("N/A")
```

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/validate.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/validate.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/cmds/wait_for_deployment.py` & `paasta-tools-1.0.1/paasta_tools/cli/cmds/wait_for_deployment.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/fsm/__init__.py` & `paasta-tools-1.0.1/paasta_tools/cli/fsm/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/fsm/autosuggest.py` & `paasta-tools-1.0.1/paasta_tools/cli/fsm/autosuggest.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/kubernetes-PROD.yaml` & `paasta-tools-1.0.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/kubernetes-PROD.yaml`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/monitoring.yaml` & `paasta-tools-1.0.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/monitoring.yaml`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/fsm_cmd.py` & `paasta-tools-1.0.1/paasta_tools/cli/fsm_cmd.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/paasta_tabcomplete.sh` & `paasta-tools-1.0.1/paasta_tools/cli/paasta_tabcomplete.sh`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/schemas/adhoc_schema.json` & `paasta-tools-1.0.1/paasta_tools/cli/schemas/adhoc_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/schemas/autoscaling_schema.json` & `paasta-tools-1.0.1/paasta_tools/cli/schemas/autoscaling_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/schemas/autotuned_defaults/cassandracluster_schema.json` & `paasta-tools-1.0.1/paasta_tools/cli/schemas/autotuned_defaults/cassandracluster_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/schemas/autotuned_defaults/kubernetes_schema.json` & `paasta-tools-1.0.1/paasta_tools/cli/schemas/autotuned_defaults/kubernetes_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/schemas/deploy_schema.json` & `paasta-tools-1.0.1/paasta_tools/cli/schemas/deploy_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/schemas/eks_schema.json` & `paasta-tools-1.0.1/paasta_tools/cli/schemas/eks_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/schemas/kubernetes_schema.json` & `paasta-tools-1.0.1/paasta_tools/cli/schemas/kubernetes_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/schemas/rollback_schema.json` & `paasta-tools-1.0.1/paasta_tools/cli/schemas/rollback_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/schemas/service_schema.json` & `paasta-tools-1.0.1/paasta_tools/cli/schemas/service_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/schemas/smartstack_schema.json` & `paasta-tools-1.0.1/paasta_tools/cli/schemas/smartstack_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/schemas/tron_schema.json` & `paasta-tools-1.0.1/paasta_tools/cli/schemas/tron_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/cli/utils.py` & `paasta-tools-1.0.1/paasta_tools/cli/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 from paasta_tools.nrtsearchservice_tools import load_nrtsearchservice_instance_config
 from paasta_tools.nrtsearchserviceeks_tools import (
     load_nrtsearchserviceeks_instance_config,
 )
 from paasta_tools.paasta_service_config_loader import PaastaServiceConfigLoader
 from paasta_tools.tron_tools import load_tron_instance_config
 from paasta_tools.utils import _log
-from paasta_tools.utils import _log_audit
 from paasta_tools.utils import _run
 from paasta_tools.utils import compose_job_id
 from paasta_tools.utils import DEFAULT_SOA_CONFIGS_GIT_URL
 from paasta_tools.utils import DEFAULT_SOA_DIR
 from paasta_tools.utils import get_service_instance_list
 from paasta_tools.utils import INSTANCE_TYPE_TO_K8S_NAMESPACE
 from paasta_tools.utils import INSTANCE_TYPES
@@ -489,139 +488,14 @@
             "hint": hint,
             "output": output,
         }
     )
     return (False, output)
 
 
-def get_paasta_metastatus_cmd_args(
-    groupings: Sequence[str],
-    verbose: int = 0,
-    autoscaling_info: bool = False,
-    use_mesos_cache: bool = False,
-) -> Tuple[Sequence[str], int]:
-    if verbose > 0:
-        verbose_arg = ["-%s" % ("v" * verbose)]
-        timeout = 120
-    else:
-        verbose_arg = []
-        timeout = 20
-    autoscaling_arg = ["-a"] if autoscaling_info else []
-    if autoscaling_arg and verbose < 2:
-        verbose_arg = ["-vv"]
-    groupings_args = ["-g", *groupings] if groupings else []
-    cache_arg = ["--use-mesos-cache"] if use_mesos_cache else []
-    cmd_args = [*verbose_arg, *groupings_args, *autoscaling_arg, *cache_arg]
-    return cmd_args, timeout
-
-
-def run_paasta_metastatus(
-    master: str,
-    groupings: Sequence[str],
-    verbose: int = 0,
-    autoscaling_info: bool = False,
-    use_mesos_cache: bool = False,
-) -> Tuple[int, str]:
-    cmd_args, timeout = get_paasta_metastatus_cmd_args(
-        groupings=groupings,
-        verbose=verbose,
-        autoscaling_info=autoscaling_info,
-        use_mesos_cache=use_mesos_cache,
-    )
-    command = (
-        "ssh -A -n -o StrictHostKeyChecking=no {} sudo paasta_metastatus {}".format(
-            master, " ".join(cmd_args)
-        )
-    ).strip()
-    return_code, output = _run(command, timeout=timeout)
-    return return_code, output
-
-
-def run_paasta_cluster_boost(master, action, pool, duration, override, boost, verbose):
-    timeout = 20
-
-    verbose_flag: Optional[str]
-    if verbose > 0:
-        verbose_flag = "-{}".format("v" * verbose)
-    else:
-        verbose_flag = None
-
-    pool_flag = f"--pool {pool}"
-    duration_flag = f"--duration {duration}" if duration is not None else ""
-    boost_flag = f"--boost {boost}" if boost is not None else ""
-    override_flag = "--force" if override is not None else ""
-
-    cmd_args = " ".join(
-        filter(
-            None,
-            [action, pool_flag, duration_flag, boost_flag, override_flag, verbose_flag],
-        )
-    )
-    command = (
-        "ssh -A -n -o StrictHostKeyChecking=no {} paasta_cluster_boost {}".format(
-            master, cmd_args
-        )
-    ).strip()
-    return_code, output = _run(command, timeout=timeout)
-    return return_code, output
-
-
-def execute_paasta_cluster_boost_on_remote_master(
-    clusters,
-    system_paasta_config,
-    action,
-    pool,
-    duration=None,
-    override=None,
-    boost=None,
-    verbose=0,
-):
-    """Returns a string containing an error message if an error occurred.
-    Otherwise returns the output of run_paasta_cluster_boost().
-    """
-    result = {}
-    for cluster in clusters:
-        try:
-            master = connectable_master(cluster, system_paasta_config)
-        except NoMasterError as e:
-            result[cluster] = (255, str(e))
-            continue
-
-        result[cluster] = run_paasta_cluster_boost(
-            master=master,
-            action=action,
-            pool=pool,
-            duration=duration,
-            override=override,
-            boost=boost,
-            verbose=verbose,
-        )
-
-        audit_details = {
-            "boost_action": action,
-            "pool": pool,
-            "duration": duration,
-            "override": override,
-            "boost": boost,
-        }
-        _log_audit(
-            action="cluster-boost", action_details=audit_details, cluster=cluster
-        )
-
-    aggregated_code = 0
-    aggregated_output = ""
-    for cluster in result:
-        code = result[cluster][0]
-        output = result[cluster][1]
-        if not code == 0:
-            aggregated_code = 1
-        aggregated_output += f"\n{cluster}: \n{output}\n"
-    return (aggregated_code, aggregated_output)
-
-
 def run_on_master(
     cluster,
     system_paasta_config,
     cmd_parts,
     timeout=None,
     err_code=-1,
     graceful_exit=False,
```

### Comparing `paasta-tools-1.0.0/paasta_tools/clusterman.py` & `paasta-tools-1.0.1/paasta_tools/clusterman.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/config_utils.py` & `paasta-tools-1.0.1/paasta_tools/config_utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/bounce_log_latency_parser.py` & `paasta-tools-1.0.1/paasta_tools/contrib/bounce_log_latency_parser.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/check_manual_oapi_changes.sh` & `paasta-tools-1.0.1/paasta_tools/contrib/check_manual_oapi_changes.sh`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/check_orphans.py` & `paasta-tools-1.0.1/paasta_tools/contrib/check_orphans.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/create_dynamodb_table.py` & `paasta-tools-1.0.1/paasta_tools/contrib/create_dynamodb_table.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/create_paasta_playground.py` & `paasta-tools-1.0.1/paasta_tools/contrib/create_paasta_playground.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/emit_allocated_cpu_metrics.py` & `paasta-tools-1.0.1/paasta_tools/contrib/emit_allocated_cpu_metrics.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/get_running_task_allocation.py` & `paasta-tools-1.0.1/paasta_tools/contrib/get_running_task_allocation.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/habitat_fixer.py` & `paasta-tools-1.0.1/paasta_tools/contrib/habitat_fixer.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/ide_helper.py` & `paasta-tools-1.0.1/paasta_tools/contrib/ide_helper.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/is_pod_healthy_in_proxy.py` & `paasta-tools-1.0.1/paasta_tools/contrib/is_pod_healthy_in_proxy.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/is_pod_healthy_in_smartstack.py` & `paasta-tools-1.0.1/paasta_tools/contrib/is_pod_healthy_in_smartstack.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/kill_bad_containers.py` & `paasta-tools-1.0.1/paasta_tools/contrib/kill_bad_containers.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/mass-deploy-tag.sh` & `paasta-tools-1.0.1/paasta_tools/contrib/mass-deploy-tag.sh`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/mock_patch_checker.py` & `paasta-tools-1.0.1/paasta_tools/contrib/mock_patch_checker.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/paasta_update_soa_memcpu.py` & `paasta-tools-1.0.1/paasta_tools/contrib/paasta_update_soa_memcpu.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/render_template.py` & `paasta-tools-1.0.1/paasta_tools/contrib/render_template.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/rightsizer_soaconfigs_update.py` & `paasta-tools-1.0.1/paasta_tools/contrib/rightsizer_soaconfigs_update.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/service_shard_remove.py` & `paasta-tools-1.0.1/paasta_tools/contrib/service_shard_remove.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/service_shard_update.py` & `paasta-tools-1.0.1/paasta_tools/contrib/service_shard_update.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/shared_ip_check.py` & `paasta-tools-1.0.1/paasta_tools/contrib/shared_ip_check.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/contrib/timeouts_metrics_prom.py` & `paasta-tools-1.0.1/paasta_tools/contrib/timeouts_metrics_prom.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/delete_kubernetes_deployments.py` & `paasta-tools-1.0.1/paasta_tools/delete_kubernetes_deployments.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/deployment_utils.py` & `paasta-tools-1.0.1/paasta_tools/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/docker_wrapper.py` & `paasta-tools-1.0.1/paasta_tools/docker_wrapper.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/docker_wrapper_imports.py` & `paasta-tools-1.0.1/paasta_tools/docker_wrapper_imports.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/drain_lib.py` & `paasta-tools-1.0.1/paasta_tools/drain_lib.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/dump_locally_running_services.py` & `paasta-tools-1.0.1/paasta_tools/dump_locally_running_services.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/eks_tools.py` & `paasta-tools-1.0.1/paasta_tools/eks_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/envoy_tools.py` & `paasta-tools-1.0.1/paasta_tools/envoy_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/firewall.py` & `paasta-tools-1.0.1/paasta_tools/firewall.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/firewall_logging.py` & `paasta-tools-1.0.1/paasta_tools/firewall_logging.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/firewall_update.py` & `paasta-tools-1.0.1/paasta_tools/firewall_update.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/flink_tools.py` & `paasta-tools-1.0.1/paasta_tools/flink_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/flinkeks_tools.py` & `paasta-tools-1.0.1/paasta_tools/flinkeks_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/frameworks/adhoc_scheduler.py` & `paasta-tools-1.0.1/paasta_tools/frameworks/adhoc_scheduler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/frameworks/constraints.py` & `paasta-tools-1.0.1/paasta_tools/frameworks/constraints.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/frameworks/native_scheduler.py` & `paasta-tools-1.0.1/paasta_tools/frameworks/native_scheduler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/frameworks/native_service_config.py` & `paasta-tools-1.0.1/paasta_tools/frameworks/native_service_config.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/frameworks/task_store.py` & `paasta-tools-1.0.1/paasta_tools/frameworks/task_store.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/generate_deployments_for_service.py` & `paasta-tools-1.0.1/paasta_tools/generate_deployments_for_service.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/generate_services_file.py` & `paasta-tools-1.0.1/paasta_tools/generate_services_file.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/generate_services_yaml.py` & `paasta-tools-1.0.1/paasta_tools/generate_services_yaml.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/hacheck.py` & `paasta-tools-1.0.1/paasta_tools/hacheck.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/instance/hpa_metrics_parser.py` & `paasta-tools-1.0.1/paasta_tools/instance/hpa_metrics_parser.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/instance/kubernetes.py` & `paasta-tools-1.0.1/paasta_tools/instance/kubernetes.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/iptables.py` & `paasta-tools-1.0.1/paasta_tools/iptables.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/kafkacluster_tools.py` & `paasta-tools-1.0.1/paasta_tools/kafkacluster_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/kubernetes/application/controller_wrappers.py` & `paasta-tools-1.0.1/paasta_tools/kubernetes/application/controller_wrappers.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/kubernetes/application/tools.py` & `paasta-tools-1.0.1/paasta_tools/kubernetes/application/tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/kubernetes/bin/kubernetes_remove_evicted_pods.py` & `paasta-tools-1.0.1/paasta_tools/kubernetes/bin/kubernetes_remove_evicted_pods.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/kubernetes/bin/paasta_cleanup_stale_nodes.py` & `paasta-tools-1.0.1/paasta_tools/kubernetes/bin/paasta_cleanup_stale_nodes.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/kubernetes/bin/paasta_secrets_sync.py` & `paasta-tools-1.0.1/paasta_tools/kubernetes/bin/paasta_secrets_sync.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/kubernetes_tools.py` & `paasta-tools-1.0.1/paasta_tools/kubernetes_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/list_kubernetes_service_instances.py` & `paasta-tools-1.0.1/paasta_tools/list_kubernetes_service_instances.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/list_tron_namespaces.py` & `paasta-tools-1.0.1/paasta_tools/list_tron_namespaces.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/log_task_lifecycle_events.py` & `paasta-tools-1.0.1/paasta_tools/log_task_lifecycle_events.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/long_running_service_tools.py` & `paasta-tools-1.0.1/paasta_tools/long_running_service_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/mac_address.py` & `paasta-tools-1.0.1/paasta_tools/mac_address.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/mesos/cfg.py` & `paasta-tools-1.0.1/paasta_tools/mesos/cfg.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/mesos/cluster.py` & `paasta-tools-1.0.1/paasta_tools/mesos/cluster.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/mesos/exceptions.py` & `paasta-tools-1.0.1/paasta_tools/mesos/exceptions.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/mesos/framework.py` & `paasta-tools-1.0.1/paasta_tools/mesos/framework.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/mesos/log.py` & `paasta-tools-1.0.1/paasta_tools/mesos/log.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/mesos/master.py` & `paasta-tools-1.0.1/paasta_tools/mesos/master.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/mesos/mesos_file.py` & `paasta-tools-1.0.1/paasta_tools/mesos/mesos_file.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/mesos/parallel.py` & `paasta-tools-1.0.1/paasta_tools/mesos/parallel.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/mesos/slave.py` & `paasta-tools-1.0.1/paasta_tools/mesos/slave.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/mesos/task.py` & `paasta-tools-1.0.1/paasta_tools/mesos/task.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/mesos/util.py` & `paasta-tools-1.0.1/paasta_tools/mesos/util.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/mesos/zookeeper.py` & `paasta-tools-1.0.1/paasta_tools/mesos/zookeeper.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/mesos_maintenance.py` & `paasta-tools-1.0.1/paasta_tools/mesos_maintenance.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/mesos_tools.py` & `paasta-tools-1.0.1/paasta_tools/mesos_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,22 +149,14 @@
             raise
         log.debug("Mesos Leader: %s" % fqdn)
         return fqdn
     else:
         raise ValueError("Expected to receive a valid URL, got: %s" % url)
 
 
-def is_mesos_leader(hostname: str = MY_HOSTNAME) -> bool:
-    """Check if a hostname is the current mesos leader.
-
-    :param hostname: The hostname to query mesos-master on
-    :returns: True if hostname is the mesos-master leader, False otherwise"""
-    return get_mesos_leader() == hostname
-
-
 class MesosLeaderUnavailable(Exception):
     pass
 
 
 def find_mesos_leader(cluster):
     """Find the leader with redirect given one mesos master."""
     master = (
```

### Comparing `paasta-tools-1.0.0/paasta_tools/metrics/metastatus_lib.py` & `paasta-tools-1.0.1/paasta_tools/metrics/metastatus_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # limitations under the License.
 import copy
 import itertools
 import math
 import re
 from collections import Counter
 from collections import namedtuple
-from collections import OrderedDict
 from typing import Any
 from typing import Callable
 from typing import Mapping
 from typing import NamedTuple
 from typing import Sequence
 from typing import Tuple
 from typing import TypeVar
@@ -470,68 +469,14 @@
     healthy = running > 0
     return HealthCheckResult(
         message=f"Pods: running: {running} pending: {pending} failed: {failed}",
         healthy=healthy,
     )
 
 
-def assert_no_duplicate_frameworks(
-    state: MesosState, framework_list: Sequence[str]
-) -> HealthCheckResult:
-    """A function which asserts that there are no duplicate frameworks running, where
-    frameworks are identified by their name.
-
-    Note the extra spaces in the output strings: this is to account for the extra indentation
-    we add, so we can have:
-
-        frameworks:
-          framework: tron count: 1
-
-    :param state: the state info from the Mesos master
-    :returns: a tuple containing (output, ok): output is a log of the state of frameworks, ok a boolean
-        indicating if there are any duplicate frameworks.
-    """
-    output = ["Frameworks:"]
-    status = True
-    frameworks = state["frameworks"]
-    for name in framework_list:
-        shards = [x["name"] for x in frameworks if x["name"].startswith(name)]
-        for framework, count in OrderedDict(sorted(Counter(shards).items())).items():
-            if count > 1:
-                status = False
-                output.append(
-                    "    CRITICAL: There are %d connected %s frameworks! "
-                    "(Expected 1)" % (count, framework)
-                )
-        output.append("    Framework: %s count: %d" % (name, len(shards)))
-
-    return HealthCheckResult(message=("\n").join(output), healthy=status)
-
-
-def assert_frameworks_exist(
-    state: MesosState, expected: Sequence[str]
-) -> HealthCheckResult:
-    frameworks = [f["name"] for f in state["frameworks"]]
-    not_found = []
-    ok = True
-
-    for f in expected:
-        if f not in frameworks:
-            ok = False
-            not_found.append(f)
-
-    if ok:
-        return HealthCheckResult(message="all expected frameworks found", healthy=ok)
-    else:
-        return HealthCheckResult(
-            message="CRITICAL: framework(s) %s not found" % ", ".join(not_found),
-            healthy=ok,
-        )
-
-
 def get_mesos_slaves_health_status(
     metrics: MesosMetrics,
 ) -> Tuple[int, int]:
     return metrics["master/slaves_active"], metrics["master/slaves_inactive"]
 
 
 def get_kube_nodes_health_status(
```

### Comparing `paasta-tools-1.0.0/paasta_tools/metrics/metrics_lib.py` & `paasta-tools-1.0.1/paasta_tools/metrics/metrics_lib.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/monitoring/__init__.py` & `paasta-tools-1.0.1/paasta_tools/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/monitoring/check_k8s_api_performance.py` & `paasta-tools-1.0.1/paasta_tools/monitoring/check_k8s_api_performance.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/monitoring/kill_orphaned_docker_containers.py` & `paasta-tools-1.0.1/paasta_tools/monitoring/kill_orphaned_docker_containers.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/monitoring_tools.py` & `paasta-tools-1.0.1/paasta_tools/monitoring_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/monkrelaycluster_tools.py` & `paasta-tools-1.0.1/paasta_tools/monkrelaycluster_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/nrtsearchservice_tools.py` & `paasta-tools-1.0.1/paasta_tools/nrtsearchservice_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/nrtsearchserviceeks_tools.py` & `paasta-tools-1.0.1/paasta_tools/nrtsearchserviceeks_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/oom_logger.py` & `paasta-tools-1.0.1/paasta_tools/oom_logger.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paasta_execute_docker_command.py` & `paasta-tools-1.0.1/paasta_tools/paasta_execute_docker_command.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paasta_native_serviceinit.py` & `paasta-tools-1.0.1/paasta_tools/paasta_native_serviceinit.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paasta_remote_run.py` & `paasta-tools-1.0.1/paasta_tools/paasta_remote_run.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paasta_service_config_loader.py` & `paasta-tools-1.0.1/paasta_tools/paasta_service_config_loader.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/__init__.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/api/autoscaler_api.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/api/autoscaler_api.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/api/default_api.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/api/default_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from paasta_tools.paastaapi.model.deploy_queue import DeployQueue
 from paasta_tools.paastaapi.model.inline_object import InlineObject
-from paasta_tools.paastaapi.model.meta_status import MetaStatus
 
 
 class DefaultApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -346,131 +345,14 @@
                 ],
                 'content_type': [],
             },
             api_client=api_client,
             callable=__get_service_autoscaler_pause
         )
 
-        def __metastatus(
-            self,
-            cmd_args,
-            **kwargs
-        ):
-            """Get metastatus  # noqa: E501
-
-            This method makes a synchronous HTTP request by default. To make an
-            asynchronous HTTP request, please pass async_req=True
-
-            >>> thread = api.metastatus(cmd_args, async_req=True)
-            >>> result = thread.get()
-
-            Args:
-                cmd_args ([str]): comma separated list of command arguments
-
-            Keyword Args:
-                _return_http_data_only (bool): response data without head status
-                    code and headers. Default is True.
-                _preload_content (bool): if False, the urllib3.HTTPResponse object
-                    will be returned without reading/decoding response data.
-                    Default is True.
-                _request_timeout (float/tuple): timeout setting for this request. If one
-                    number provided, it will be total request timeout. It can also
-                    be a pair (tuple) of (connection, read) timeouts.
-                    Default is None.
-                _check_input_type (bool): specifies if type checking
-                    should be done one the data sent to the server.
-                    Default is True.
-                _check_return_type (bool): specifies if type checking
-                    should be done one the data received from the server.
-                    Default is True.
-                _host_index (int/None): specifies the index of the server
-                    that we want to use.
-                    Default is read from the configuration.
-                async_req (bool): execute request asynchronously
-
-            Returns:
-                MetaStatus
-                    If the method is called asynchronously, returns the request
-                    thread.
-            """
-            kwargs['async_req'] = kwargs.get(
-                'async_req', False
-            )
-            kwargs['_return_http_data_only'] = kwargs.get(
-                '_return_http_data_only', True
-            )
-            kwargs['_preload_content'] = kwargs.get(
-                '_preload_content', True
-            )
-            kwargs['_request_timeout'] = kwargs.get(
-                '_request_timeout', None
-            )
-            kwargs['_check_input_type'] = kwargs.get(
-                '_check_input_type', True
-            )
-            kwargs['_check_return_type'] = kwargs.get(
-                '_check_return_type', True
-            )
-            kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['cmd_args'] = \
-                cmd_args
-            return self.call_with_http_info(**kwargs)
-
-        self.metastatus = Endpoint(
-            settings={
-                'response_type': (MetaStatus,),
-                'auth': [],
-                'endpoint_path': '/metastatus',
-                'operation_id': 'metastatus',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'cmd_args',
-                ],
-                'required': [
-                    'cmd_args',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'cmd_args':
-                        ([str],),
-                },
-                'attribute_map': {
-                    'cmd_args': 'cmd_args',
-                },
-                'location_map': {
-                    'cmd_args': 'query',
-                },
-                'collection_format_map': {
-                    'cmd_args': 'csv',
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client,
-            callable=__metastatus
-        )
-
         def __show_version(
             self,
             **kwargs
         ):
             """Version of paasta_tools package  # noqa: E501
 
             This method makes a synchronous HTTP request by default. To make an
```

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/api/resources_api.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/api/resources_api.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/api/service_api.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/api/service_api.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/api_client.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/api_client.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/apis/__init__.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/configuration.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/configuration.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/exceptions.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/adhoc_launch_history.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/adhoc_launch_history.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/autoscaler_count_msg.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/autoscaler_count_msg.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/deploy_queue.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/deploy_queue.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/deploy_queue_service_instance.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/deploy_queue_service_instance.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/envoy_backend.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/envoy_backend.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/envoy_location.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/envoy_location.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/envoy_status.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/envoy_status.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/flink_cluster_overview.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_cluster_overview.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/flink_config.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_config.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/flink_job.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_job.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/flink_job_details.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_job_details.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/flink_jobs.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_jobs.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/float_and_error.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/float_and_error.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/hpa_metric.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/hpa_metric.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/inline_object.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/inline_object.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/inline_response200.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/inline_response2001.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_bounce_status.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_bounce_status.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_mesh_status.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_mesh_status.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status_adhoc.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_adhoc.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status_cassandracluster.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_cassandracluster.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status_flink.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_flink.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status_kafkacluster.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_kafkacluster.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status_kubernetes.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_kubernetes.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status_kubernetes_autoscaling_status.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_kubernetes_autoscaling_status.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status_kubernetes_v2.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_kubernetes_v2.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_status_tron.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_tron.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/instance_tasks.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_tasks.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/integer_and_error.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/integer_and_error.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/kubernetes_container.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_container.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/kubernetes_container_v2.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_container_v2.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/kubernetes_healthcheck.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_healthcheck.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/kubernetes_pod.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/kubernetes_pod_event.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_pod_event.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/kubernetes_pod_v2.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_pod_v2.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/kubernetes_replica_set.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_replica_set.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/kubernetes_version.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_version.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/meta_status.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/resource_value.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class MetaStatus(ModelNormal):
+class ResourceValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -72,26 +72,28 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'exit_code': (int,),  # noqa: E501
-            'output': (str,),  # noqa: E501
+            'free': (float,),  # noqa: E501
+            'total': (float,),  # noqa: E501
+            'used': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'exit_code': 'exit_code',  # noqa: E501
-        'output': 'output',  # noqa: E501
+        'free': 'free',  # noqa: E501
+        'total': 'total',  # noqa: E501
+        'used': 'used',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
@@ -99,15 +101,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """MetaStatus - a model defined in OpenAPI
+        """ResourceValue - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +134,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            exit_code (int): Exit code from &#x60;paasta metastatus&#x60; command. [optional]  # noqa: E501
-            output (str): Output from &#x60;paasta metastatus&#x60; command. [optional]  # noqa: E501
+            free (float): [optional]  # noqa: E501
+            total (float): [optional]  # noqa: E501
+            used (float): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/resource.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/resource.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/resource_item.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/resource_item.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/resource_value.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/task_tail_lines.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class ResourceValue(ModelNormal):
+class TaskTailLines(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -72,28 +72,28 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'free': (float,),  # noqa: E501
-            'total': (float,),  # noqa: E501
-            'used': (float,),  # noqa: E501
+            'error_message': (str,),  # noqa: E501
+            'stderr': ([str],),  # noqa: E501
+            'stdout': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'free': 'free',  # noqa: E501
-        'total': 'total',  # noqa: E501
-        'used': 'used',  # noqa: E501
+        'error_message': 'error_message',  # noqa: E501
+        'stderr': 'stderr',  # noqa: E501
+        'stdout': 'stdout',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
@@ -101,15 +101,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ResourceValue - a model defined in OpenAPI
+        """TaskTailLines - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,17 +134,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            free (float): [optional]  # noqa: E501
-            total (float): [optional]  # noqa: E501
-            used (float): [optional]  # noqa: E501
+            error_message (str): Error message when fetching tail lines fails. [optional]  # noqa: E501
+            stderr ([str]): The requested number of lines from the task&#39;s stderr. [optional]  # noqa: E501
+            stdout ([str]): The requested number of lines from the task&#39;s stdout. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/smartstack_backend.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/smartstack_backend.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/smartstack_location.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/smartstack_location.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model/smartstack_status.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model/smartstack_status.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/model_utils.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/model_utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/models/__init__.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 from paasta_tools.paastaapi.model.kubernetes_container_v2 import KubernetesContainerV2
 from paasta_tools.paastaapi.model.kubernetes_healthcheck import KubernetesHealthcheck
 from paasta_tools.paastaapi.model.kubernetes_pod import KubernetesPod
 from paasta_tools.paastaapi.model.kubernetes_pod_event import KubernetesPodEvent
 from paasta_tools.paastaapi.model.kubernetes_pod_v2 import KubernetesPodV2
 from paasta_tools.paastaapi.model.kubernetes_replica_set import KubernetesReplicaSet
 from paasta_tools.paastaapi.model.kubernetes_version import KubernetesVersion
-from paasta_tools.paastaapi.model.meta_status import MetaStatus
 from paasta_tools.paastaapi.model.resource import Resource
 from paasta_tools.paastaapi.model.resource_item import ResourceItem
 from paasta_tools.paastaapi.model.resource_value import ResourceValue
 from paasta_tools.paastaapi.model.smartstack_backend import SmartstackBackend
 from paasta_tools.paastaapi.model.smartstack_location import SmartstackLocation
 from paasta_tools.paastaapi.model.smartstack_status import SmartstackStatus
 from paasta_tools.paastaapi.model.task_tail_lines import TaskTailLines
```

### Comparing `paasta-tools-1.0.0/paasta_tools/paastaapi/rest.py` & `paasta-tools-1.0.1/paasta_tools/paastaapi/rest.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/prune_completed_pods.py` & `paasta-tools-1.0.1/paasta_tools/prune_completed_pods.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/puppet_service_tools.py` & `paasta-tools-1.0.1/paasta_tools/puppet_service_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/remote_git.py` & `paasta-tools-1.0.1/paasta_tools/remote_git.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/run-paasta-api-in-dev-mode.py` & `paasta-tools-1.0.1/paasta_tools/run-paasta-api-in-dev-mode.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/run-paasta-api-playground.py` & `paasta-tools-1.0.1/paasta_tools/run-paasta-api-playground.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/secret_providers/__init__.py` & `paasta-tools-1.0.1/paasta_tools/secret_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/secret_providers/vault.py` & `paasta-tools-1.0.1/paasta_tools/secret_providers/vault.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/secret_tools.py` & `paasta-tools-1.0.1/paasta_tools/secret_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/setup_istio_mesh.py` & `paasta-tools-1.0.1/paasta_tools/setup_istio_mesh.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/setup_kubernetes_cr.py` & `paasta-tools-1.0.1/paasta_tools/setup_kubernetes_cr.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/setup_kubernetes_crd.py` & `paasta-tools-1.0.1/paasta_tools/setup_kubernetes_crd.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/setup_kubernetes_internal_crd.py` & `paasta-tools-1.0.1/paasta_tools/setup_kubernetes_internal_crd.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/setup_kubernetes_job.py` & `paasta-tools-1.0.1/paasta_tools/setup_kubernetes_job.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/setup_prometheus_adapter_config.py` & `paasta-tools-1.0.1/paasta_tools/setup_prometheus_adapter_config.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/setup_tron_namespace.py` & `paasta-tools-1.0.1/paasta_tools/setup_tron_namespace.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/slack.py` & `paasta-tools-1.0.1/paasta_tools/slack.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/smartstack_tools.py` & `paasta-tools-1.0.1/paasta_tools/smartstack_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/spark_tools.py` & `paasta-tools-1.0.1/paasta_tools/spark_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/synapse_srv_namespaces_fact.py` & `paasta-tools-1.0.1/paasta_tools/synapse_srv_namespaces_fact.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/tron/client.py` & `paasta-tools-1.0.1/paasta_tools/tron/client.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/tron/tron_command_context.py` & `paasta-tools-1.0.1/paasta_tools/tron/tron_command_context.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/tron/tron_timeutils.py` & `paasta-tools-1.0.1/paasta_tools/tron/tron_timeutils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/tron_tools.py` & `paasta-tools-1.0.1/paasta_tools/tron_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools/utils.py` & `paasta-tools-1.0.1/paasta_tools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1916,39 +1916,24 @@
     api_client_timeout: int
     api_endpoints: Dict[str, str]
     api_profiling_config: Dict
     auth_certificate_ttl: str
     auto_config_instance_types_enabled: Dict[str, bool]
     auto_config_instance_type_aliases: Dict[str, str]
     auto_hostname_unique_size: int
-    boost_regions: List[str]
-    cluster_autoscaler_max_decrease: float
-    cluster_autoscaler_max_increase: float
-    cluster_autoscaling_draining_enabled: bool
-    cluster_autoscaling_resources: IdToClusterAutoscalingResourcesDict
-    cluster_boost_enabled: bool
     cluster_fqdn_format: str
     clusters: Sequence[str]
     cluster: str
     cr_owners: Dict[str, str]
     dashboard_links: Dict[str, Dict[str, str]]
     datastore_credentials_vault_env_overrides: Dict[str, str]
     default_push_groups: List
     default_should_use_uwsgi_exporter: bool
     deploy_blacklist: UnsafeDeployBlacklist
-    deployd_big_bounce_deadline: float
-    deployd_log_level: str
-    deployd_maintenance_polling_frequency: int
-    deployd_max_service_instance_failures: int
     deployd_metrics_provider: str
-    deployd_number_workers: int
-    deployd_startup_bounce_deadline: float
-    deployd_startup_oracle_enabled: bool
-    deployd_use_zk_queue: bool
-    deployd_worker_failure_backoff_factor: int
     deploy_whitelist: UnsafeDeployWhitelist
     disabled_watchers: List
     dockercfg_location: str
     docker_registry: str
     enable_client_cert_auth: bool
     enable_nerve_readiness_check: bool
     enable_envoy_readiness_check: bool
@@ -1970,15 +1955,14 @@
     ldap_reader_password: str
     ldap_reader_username: str
     ldap_search_base: str
     ldap_search_ou: str
     local_run_config: LocalRunConfig
     log_reader: LogReaderConfig
     log_writer: LogWriterConfig
-    maintenance_resource_reservation_enabled: bool
     mark_for_deployment_max_polling_threads: int
     mark_for_deployment_default_polling_interval: float
     mark_for_deployment_default_diagnosis_interval: float
     mark_for_deployment_default_default_time_before_first_diagnosis: float
     mark_for_deployment_should_ping_for_unhealthy_pods: bool
     mesos_config: Dict
     metrics_provider: str
@@ -2341,47 +2325,14 @@
         :returns: A string identifying the metrics_provider
         """
         deployd_metrics_provider = self.config_dict.get("deployd_metrics_provider")
         if deployd_metrics_provider is not None:
             return deployd_metrics_provider
         return self.config_dict.get("metrics_provider")
 
-    def get_deployd_worker_failure_backoff_factor(self) -> int:
-        """Get the factor for calculating exponential backoff when a deployd worker
-        fails to bounce a service
-
-        :returns: An integer
-        """
-        return self.config_dict.get("deployd_worker_failure_backoff_factor", 30)
-
-    def get_deployd_maintenance_polling_frequency(self) -> int:
-        """Get the frequency in seconds that the deployd maintenance watcher should
-        poll mesos's api for new draining hosts
-
-        :returns: An integer
-        """
-        return self.config_dict.get("deployd_maintenance_polling_frequency", 30)
-
-    def get_deployd_startup_oracle_enabled(self) -> bool:
-        """This controls whether deployd will add all services that need a bounce on
-        startup. Generally this is desirable behavior. If you are performing a bounce
-        of *all* services you will want to disable this.
-
-        :returns: A boolean
-        """
-        return self.config_dict.get("deployd_startup_oracle_enabled", True)
-
-    def get_deployd_max_service_instance_failures(self) -> int:
-        """Determines how many times a service instance entry in deployd's queue
-        can fail before it will be removed from the queue.
-
-        :returns: An integer
-        """
-        return self.config_dict.get("deployd_max_service_instance_failures", 20)
-
     def get_sensu_host(self) -> str:
         """Get the host that we should send sensu events to.
 
         :returns: the sensu_host string, or localhost if not specified.
         """
         return self.config_dict.get("sensu_host", "localhost")
 
@@ -2419,43 +2370,14 @@
         return self.config_dict.get(
             "synapse_haproxy_url_format", DEFAULT_SYNAPSE_HAPROXY_URL_FORMAT
         )
 
     def get_service_discovery_providers(self) -> Dict[str, Any]:
         return self.config_dict.get("service_discovery_providers", {})
 
-    def get_cluster_autoscaling_resources(self) -> IdToClusterAutoscalingResourcesDict:
-        return self.config_dict.get("cluster_autoscaling_resources", {})
-
-    def get_cluster_autoscaling_draining_enabled(self) -> bool:
-        """Enable mesos maintenance mode and trigger draining of instances before the
-        autoscaler terminates the instance.
-
-        :returns A bool"""
-        return self.config_dict.get("cluster_autoscaling_draining_enabled", True)
-
-    def get_cluster_autoscaler_max_increase(self) -> float:
-        """Set the maximum increase that the cluster autoscaler can make in each run
-
-        :returns A float"""
-        return self.config_dict.get("cluster_autoscaler_max_increase", 0.2)
-
-    def get_cluster_autoscaler_max_decrease(self) -> float:
-        """Set the maximum decrease that the cluster autoscaler can make in each run
-
-        :returns A float"""
-        return self.config_dict.get("cluster_autoscaler_max_decrease", 0.1)
-
-    def get_cluster_boost_enabled(self) -> bool:
-        """Enable the cluster boost. Note that the boost only applies to the CPUs.
-        If the boost is toggled on here but not configured, it will be transparent.
-
-        :returns A bool: True means cluster boost is enabled."""
-        return self.config_dict.get("cluster_boost_enabled", False)
-
     def get_resource_pool_settings(self) -> PoolToResourcePoolSettingsDict:
         return self.config_dict.get("resource_pool_settings", {})
 
     def get_cluster_fqdn_format(self) -> str:
         """Get a format string that constructs a DNS name pointing at the paasta masters in a cluster. This format
         string gets one parameter: cluster. Defaults to 'paasta-{cluster:s}.yelp'.
 
@@ -2527,52 +2449,14 @@
     def get_security_check_command(self) -> Optional[str]:
         """Get the script to be executed during the security-check build step
 
         :return: The name of the file
         """
         return self.config_dict.get("security_check_command", None)
 
-    def get_deployd_number_workers(self) -> int:
-        """Get the number of workers to consume deployment q
-
-        :return: integer
-        """
-        return self.config_dict.get("deployd_number_workers", 4)
-
-    def get_deployd_big_bounce_deadline(self) -> float:
-        """Get the amount of time in the future to set the deadline when enqueuing instances for SystemPaastaConfig
-        changes.
-
-        :return: float
-        """
-
-        return float(
-            self.config_dict.get("deployd_big_bounce_deadline", 7 * 24 * 60 * 60)
-        )
-
-    def get_deployd_startup_bounce_deadline(self) -> float:
-        """Get the amount of time in the future to set the deadline when enqueuing instances on deployd startup.
-
-        :return: float
-        """
-
-        return float(
-            self.config_dict.get("deployd_startup_bounce_deadline", 7 * 24 * 60 * 60)
-        )
-
-    def get_deployd_log_level(self) -> str:
-        """Get the log level for paasta-deployd
-
-        :return: string name of python logging level, e.g. INFO, DEBUG etc.
-        """
-        return self.config_dict.get("deployd_log_level", "INFO")
-
-    def get_deployd_use_zk_queue(self) -> bool:
-        return self.config_dict.get("deployd_use_zk_queue", True)
-
     def get_hacheck_sidecar_image_url(self) -> str:
         """Get the docker image URL for the hacheck sidecar container"""
         return self.config_dict.get("hacheck_sidecar_image_url")
 
     def get_register_k8s_pods(self) -> bool:
         """Enable registration of k8s services in nerve"""
         return self.config_dict.get("register_k8s_pods", False)
@@ -2654,17 +2538,14 @@
         return socket.getservbyname(
             self.config_dict.get("envoy_admin_domain_name", "envoy-admin")
         )
 
     def get_pdb_max_unavailable(self) -> Union[str, int]:
         return self.config_dict.get("pdb_max_unavailable", 0)
 
-    def get_boost_regions(self) -> List[str]:
-        return self.config_dict.get("boost_regions", [])
-
     def get_pod_defaults(self) -> Dict[str, Any]:
         return self.config_dict.get("pod_defaults", {})
 
     def get_ldap_search_base(self) -> str:
         return self.config_dict.get("ldap_search_base", None)
 
     def get_ldap_search_ou(self) -> str:
```

### Comparing `paasta-tools-1.0.0/paasta_tools/vitesscluster_tools.py` & `paasta-tools-1.0.1/paasta_tools/vitesscluster_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/paasta_tools.egg-info/SOURCES.txt` & `paasta-tools-1.0.1/paasta_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 requirements-minimal.txt
 setup.py
 k8s_itests/__init__.py
 k8s_itests/test_autoscaling.py
 k8s_itests/utils.py
 paasta_tools/__init__.py
 paasta_tools/adhoc_tools.py
-paasta_tools/am_i_mesos_leader.py
 paasta_tools/apply_external_resources.py
 paasta_tools/async_utils.py
 paasta_tools/bounce_lib.py
 paasta_tools/broadcast_log_to_services.py
 paasta_tools/cassandracluster_tools.py
 paasta_tools/check_autoscaler_max_instances.py
 paasta_tools/check_cassandracluster_services_replication.py
@@ -21,15 +20,14 @@
 paasta_tools/check_kubernetes_services_replication.py
 paasta_tools/check_oom_events.py
 paasta_tools/check_services_replication_tools.py
 paasta_tools/check_spark_jobs.py
 paasta_tools/cleanup_kubernetes_cr.py
 paasta_tools/cleanup_kubernetes_crd.py
 paasta_tools/cleanup_kubernetes_jobs.py
-paasta_tools/cleanup_maintenance.py
 paasta_tools/cleanup_tron_namespaces.py
 paasta_tools/clusterman.py
 paasta_tools/config_utils.py
 paasta_tools/delete_kubernetes_deployments.py
 paasta_tools/deployment_utils.py
 paasta_tools/docker_wrapper.py
 paasta_tools/docker_wrapper_imports.py
@@ -42,38 +40,33 @@
 paasta_tools/firewall_update.py
 paasta_tools/flink_tools.py
 paasta_tools/flinkeks_tools.py
 paasta_tools/generate_all_deployments
 paasta_tools/generate_deployments_for_service.py
 paasta_tools/generate_services_file.py
 paasta_tools/generate_services_yaml.py
-paasta_tools/get_mesos_leader.py
 paasta_tools/hacheck.py
 paasta_tools/iptables.py
 paasta_tools/kafkacluster_tools.py
 paasta_tools/kubernetes_tools.py
 paasta_tools/list_kubernetes_service_instances.py
 paasta_tools/list_tron_namespaces.py
 paasta_tools/log_task_lifecycle_events.py
 paasta_tools/long_running_service_tools.py
 paasta_tools/mac_address.py
 paasta_tools/marathon_dashboard.py
 paasta_tools/mesos_maintenance.py
 paasta_tools/mesos_tools.py
 paasta_tools/monitoring_tools.py
 paasta_tools/monkrelaycluster_tools.py
-paasta_tools/native_mesos_scheduler.py
 paasta_tools/nrtsearchservice_tools.py
 paasta_tools/nrtsearchserviceeks_tools.py
 paasta_tools/oom_logger.py
-paasta_tools/paasta_cluster_boost.py
 paasta_tools/paasta_deploy_tron_jobs
 paasta_tools/paasta_execute_docker_command.py
-paasta_tools/paasta_maintenance.py
-paasta_tools/paasta_metastatus.py
 paasta_tools/paasta_native_serviceinit.py
 paasta_tools/paasta_remote_run.py
 paasta_tools/paasta_service_config_loader.py
 paasta_tools/prune_completed_pods.py
 paasta_tools/puppet_service_tools.py
 paasta_tools/py.typed
 paasta_tools/remote_git.py
@@ -109,49 +102,45 @@
 paasta_tools/api/tweens/profiling.py
 paasta_tools/api/tweens/request_logger.py
 paasta_tools/api/views/__init__.py
 paasta_tools/api/views/autoscaler.py
 paasta_tools/api/views/exception.py
 paasta_tools/api/views/flink.py
 paasta_tools/api/views/instance.py
-paasta_tools/api/views/metastatus.py
 paasta_tools/api/views/pause_autoscaler.py
 paasta_tools/api/views/resources.py
 paasta_tools/api/views/service.py
 paasta_tools/api/views/version.py
 paasta_tools/autoscaling/__init__.py
 paasta_tools/autoscaling/autoscaling_service_lib.py
 paasta_tools/autoscaling/forecasting.py
-paasta_tools/autoscaling/load_boost.py
 paasta_tools/autoscaling/max_all_k8s_services.py
 paasta_tools/autoscaling/pause_service_autoscaler.py
 paasta_tools/autoscaling/utils.py
 paasta_tools/cli/__init__.py
 paasta_tools/cli/cli.py
 paasta_tools/cli/fsm_cmd.py
 paasta_tools/cli/paasta_tabcomplete.sh
 paasta_tools/cli/utils.py
 paasta_tools/cli/cmds/__init__.py
 paasta_tools/cli/cmds/autoscale.py
-paasta_tools/cli/cmds/boost.py
 paasta_tools/cli/cmds/check.py
 paasta_tools/cli/cmds/cook_image.py
 paasta_tools/cli/cmds/get_docker_image.py
 paasta_tools/cli/cmds/get_image_version.py
 paasta_tools/cli/cmds/get_latest_deployment.py
 paasta_tools/cli/cmds/info.py
 paasta_tools/cli/cmds/itest.py
 paasta_tools/cli/cmds/list.py
 paasta_tools/cli/cmds/list_clusters.py
 paasta_tools/cli/cmds/list_deploy_queue.py
 paasta_tools/cli/cmds/local_run.py
 paasta_tools/cli/cmds/logs.py
 paasta_tools/cli/cmds/mark_for_deployment.py
 paasta_tools/cli/cmds/mesh_status.py
-paasta_tools/cli/cmds/metastatus.py
 paasta_tools/cli/cmds/pause_service_autoscaler.py
 paasta_tools/cli/cmds/push_to_registry.py
 paasta_tools/cli/cmds/remote_run.py
 paasta_tools/cli/cmds/rollback.py
 paasta_tools/cli/cmds/secret.py
 paasta_tools/cli/cmds/security_check.py
 paasta_tools/cli/cmds/spark_run.py
@@ -196,15 +185,14 @@
 paasta_tools/contrib/paasta_update_soa_memcpu.py
 paasta_tools/contrib/render_template.py
 paasta_tools/contrib/rightsizer_soaconfigs_update.py
 paasta_tools/contrib/service_shard_remove.py
 paasta_tools/contrib/service_shard_update.py
 paasta_tools/contrib/shared_ip_check.py
 paasta_tools/contrib/timeouts_metrics_prom.py
-paasta_tools/contrib/utilization_check.py
 paasta_tools/frameworks/__init__.py
 paasta_tools/frameworks/adhoc_scheduler.py
 paasta_tools/frameworks/constraints.py
 paasta_tools/frameworks/native_scheduler.py
 paasta_tools/frameworks/native_service_config.py
 paasta_tools/frameworks/task_store.py
 paasta_tools/instance/__init__.py
@@ -231,19 +219,15 @@
 paasta_tools/mesos/task.py
 paasta_tools/mesos/util.py
 paasta_tools/mesos/zookeeper.py
 paasta_tools/metrics/__init__.py
 paasta_tools/metrics/metastatus_lib.py
 paasta_tools/metrics/metrics_lib.py
 paasta_tools/monitoring/__init__.py
-paasta_tools/monitoring/check_capacity.py
 paasta_tools/monitoring/check_k8s_api_performance.py
-paasta_tools/monitoring/check_mesos_active_frameworks.py
-paasta_tools/monitoring/check_mesos_duplicate_frameworks.py
-paasta_tools/monitoring/check_mesos_quorum.py
 paasta_tools/monitoring/kill_orphaned_docker_containers.py
 paasta_tools/paastaapi/__init__.py
 paasta_tools/paastaapi/api_client.py
 paasta_tools/paastaapi/configuration.py
 paasta_tools/paastaapi/exceptions.py
 paasta_tools/paastaapi/model_utils.py
 paasta_tools/paastaapi/rest.py
@@ -288,15 +272,14 @@
 paasta_tools/paastaapi/model/kubernetes_container_v2.py
 paasta_tools/paastaapi/model/kubernetes_healthcheck.py
 paasta_tools/paastaapi/model/kubernetes_pod.py
 paasta_tools/paastaapi/model/kubernetes_pod_event.py
 paasta_tools/paastaapi/model/kubernetes_pod_v2.py
 paasta_tools/paastaapi/model/kubernetes_replica_set.py
 paasta_tools/paastaapi/model/kubernetes_version.py
-paasta_tools/paastaapi/model/meta_status.py
 paasta_tools/paastaapi/model/resource.py
 paasta_tools/paastaapi/model/resource_item.py
 paasta_tools/paastaapi/model/resource_value.py
 paasta_tools/paastaapi/model/smartstack_backend.py
 paasta_tools/paastaapi/model/smartstack_location.py
 paasta_tools/paastaapi/model/smartstack_status.py
 paasta_tools/paastaapi/model/task_tail_lines.py
```

### Comparing `paasta-tools-1.0.0/paasta_tools.egg-info/entry_points.txt` & `paasta-tools-1.0.1/paasta_tools.egg-info/entry_points.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [console_scripts]
 paasta = paasta_tools.cli.cli:main
 paasta-api = paasta_tools.api.api:main
 paasta-deployd = paasta_tools.deployd.master:main
 paasta-fsm = paasta_tools.cli.fsm_cmd:main
 paasta_broadcast_log = paasta_tools.broadcast_log_to_services:main
-paasta_cleanup_maintenance = paasta_tools.cleanup_maintenance:main
 paasta_cleanup_tron_namespaces = paasta_tools.cleanup_tron_namespaces:main
 paasta_docker_wrapper = paasta_tools.docker_wrapper:main
 paasta_dump_locally_running_services = paasta_tools.dump_locally_running_services:main
 paasta_firewall_logging = paasta_tools.firewall_logging:main
 paasta_firewall_update = paasta_tools.firewall_update:main
 paasta_habitat_fixer = paasta_tools.contrib.habitat_fixer:main
 paasta_list_kubernetes_service_instances = paasta_tools.list_kubernetes_service_instances:main
```

### Comparing `paasta-tools-1.0.0/paasta_tools.egg-info/requires.txt` & `paasta-tools-1.0.1/paasta_tools.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/requirements-minimal.txt` & `paasta-tools-1.0.1/requirements-minimal.txt`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.0/setup.py` & `paasta-tools-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     author_email="compute-infra@yelp.com",
     description="Tools for Yelps SOA infrastructure",
     packages=find_packages(exclude=("tests*", "scripts*")),
     include_package_data=True,
     python_requires=">=3.8.0",
     install_requires=get_install_requires(),
     scripts=[
-        "paasta_tools/am_i_mesos_leader.py",
         "paasta_tools/apply_external_resources.py",
         "paasta_tools/check_autoscaler_max_instances.py",
         "paasta_tools/check_cassandracluster_services_replication.py",
         "paasta_tools/check_flink_services_health.py",
         "paasta_tools/check_kubernetes_api.py",
         "paasta_tools/check_kubernetes_services_replication.py",
         "paasta_tools/check_oom_events.py",
@@ -54,29 +53,21 @@
         "paasta_tools/cleanup_kubernetes_jobs.py",
         "paasta_tools/cli/paasta_tabcomplete.sh",
         "paasta_tools/delete_kubernetes_deployments.py",
         "paasta_tools/generate_all_deployments",
         "paasta_tools/generate_deployments_for_service.py",
         "paasta_tools/generate_services_file.py",
         "paasta_tools/generate_services_yaml.py",
-        "paasta_tools/get_mesos_leader.py",
         "paasta_tools/kubernetes/bin/kubernetes_remove_evicted_pods.py",
         "paasta_tools/kubernetes/bin/paasta_cleanup_stale_nodes.py",
         "paasta_tools/kubernetes/bin/paasta_secrets_sync.py",
         "paasta_tools/log_task_lifecycle_events.py",
-        "paasta_tools/monitoring/check_capacity.py",
-        "paasta_tools/monitoring/check_mesos_active_frameworks.py",
-        "paasta_tools/monitoring/check_mesos_duplicate_frameworks.py",
-        "paasta_tools/monitoring/check_mesos_quorum.py",
         "paasta_tools/monitoring/kill_orphaned_docker_containers.py",
-        "paasta_tools/paasta_cluster_boost.py",
         "paasta_tools/paasta_deploy_tron_jobs",
         "paasta_tools/paasta_execute_docker_command.py",
-        "paasta_tools/paasta_maintenance.py",
-        "paasta_tools/paasta_metastatus.py",
         "paasta_tools/paasta_remote_run.py",
         "paasta_tools/setup_istio_mesh.py",
         "paasta_tools/setup_kubernetes_cr.py",
         "paasta_tools/setup_kubernetes_crd.py",
         "paasta_tools/setup_kubernetes_internal_crd.py",
         "paasta_tools/setup_kubernetes_job.py",
         "paasta_tools/setup_prometheus_adapter_config.py",
@@ -91,15 +82,14 @@
             "paasta-deployd=paasta_tools.deployd.master:main",
             "paasta-fsm=paasta_tools.cli.fsm_cmd:main",
             "paasta_prune_completed_pods=paasta_tools.prune_completed_pods:main",
             "paasta_cleanup_tron_namespaces=paasta_tools.cleanup_tron_namespaces:main",
             "paasta_list_kubernetes_service_instances=paasta_tools.list_kubernetes_service_instances:main",
             "paasta_list_tron_namespaces=paasta_tools.list_tron_namespaces:main",
             "paasta_setup_tron_namespace=paasta_tools.setup_tron_namespace:main",
-            "paasta_cleanup_maintenance=paasta_tools.cleanup_maintenance:main",
             "paasta_docker_wrapper=paasta_tools.docker_wrapper:main",
             "paasta_firewall_update=paasta_tools.firewall_update:main",
             "paasta_firewall_logging=paasta_tools.firewall_logging:main",
             "paasta_oom_logger=paasta_tools.oom_logger:main",
             "paasta_broadcast_log=paasta_tools.broadcast_log_to_services:main",
             "paasta_dump_locally_running_services=paasta_tools.dump_locally_running_services:main",
             "paasta_habitat_fixer=paasta_tools.contrib.habitat_fixer:main",
```

