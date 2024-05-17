# Comparing `tmp/cid_cmd-0.3.3.tar.gz` & `tmp/cid_cmd-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cid_cmd-0.3.3.tar", last modified: Thu Apr 25 09:08:11 2024, max compression
+gzip compressed data, was "cid_cmd-0.3.4.tar", last modified: Fri May 17 09:29:57 2024, max compression
```

## Comparing `cid_cmd-0.3.3.tar` & `cid_cmd-0.3.4.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.275941 cid_cmd-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-04-25 09:08:11.275941 cid_cmd-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.255941 cid_cmd-0.3.3/cid/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.251940 cid_cmd-0.3.3/cid/builtin/core/data/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/compute.json
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/ec2_running_cost.json
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/s3_view.json
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/summary_view.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/data/datasets/co/
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/co/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/data/datasets/cudos/
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/cudos/hourly_view.json
--rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/cudos/resource_view.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_ebs_snap.json
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_ebs_storage_all.json
--rw-r--r--   0 runner    (1001) docker     (127)    20695 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_instance_all.json
--rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_s3_storage_all.json
--rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/data/datasets/shared/
--rw-r--r--   0 runner    (1001) docker     (127)    30612 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/shared/customer_all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/data/datasets/tao/
--rw-r--r--   0 runner    (1001) docker     (127)    69315 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/tao/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/data/datasets/trends/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/trends/daily_anomaly_detection.json
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/trends/monthly_anomaly_detection.json
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/trends/monthly_bill_by_account.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.263941 cid_cmd-0.3.3/cid/builtin/core/data/permissions/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/permissions/dashboard_permissions.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/permissions/dashboard_permissions_namespace.json
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/permissions/data_set_permissions.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/permissions/data_source_permissions.json
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/permissions/folder_permissions.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.255941 cid_cmd-0.3.3/cid/builtin/core/data/queries/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.263941 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/compute_savings_plan_eligible_spend.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ec2_running_cost.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ec2_running_cost_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ec2_running_cost_sp.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ec2_running_cost_sp_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ri_sp_mapping.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ri_sp_mapping_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/s3.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/summary_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/summary_view_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/summary_view_sp.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/summary_view_sp_ri.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.267941 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/all_options.sql
--rw-r--r--   0 runner    (1001) docker     (127)    14711 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/auto_scale.json
--rw-r--r--   0 runner    (1001) docker     (127)    27919 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/auto_scale_options.sql
--rw-r--r--   0 runner    (1001) docker     (127)     9097 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/ebs_volume.json
--rw-r--r--   0 runner    (1001) docker     (127)    22473 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/ebs_volume_options.sql
--rw-r--r--   0 runner    (1001) docker     (127)    19144 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/ec2_instance.json
--rw-r--r--   0 runner    (1001) docker     (127)    28308 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/ec2_instance_options.sql
--rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/lambda.json
--rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/lambda_options.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.267941 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/hourly_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/hourly_view_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/hourly_view_sp.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/hourly_view_sp_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/resource_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/resource_view_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/resource_view_sp.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/resource_view_sp_ri.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.267941 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/
--rw-r--r--   0 runner    (1001) docker     (127)    11145 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/first_kpi_instance_mapping_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_ebs_snap_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_ebs_storage_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)    24337 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_instance_all_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)    23573 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRI.sql
--rw-r--r--   0 runner    (1001) docker     (127)    22559 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRISP.sql
--rw-r--r--   0 runner    (1001) docker     (127)    23434 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noSP.sql
--rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_s3_storage_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/last_kpi_tracker_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.271941 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/account_map.sql
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/account_map_dummy.sql
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/aws_accounts.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/aws_regions.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/aws_service_category_map.sql
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/business_units_map.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/cur.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/payer_account_name_map.sql
--rw-r--r--   0 runner    (1001) docker     (127)   163373 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/ta_descriptions.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.271941 cid_cmd-0.3.3/cid/builtin/core/data/queries/tao/
--rw-r--r--   0 runner    (1001) docker     (127)    35595 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/tao/glue_table.json
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/tao/ta_org_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.271941 cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/daily_anomaly_detection.sql
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_anomaly_detection.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_bill_by_account.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_bill_by_account_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)    18712 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12523 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.271941 cid_cmd-0.3.3/cid/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/commands/command_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/commands/init_qs.py
--rw-r--r--   0 runner    (1001) docker     (127)    92373 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19919 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.275941 cid_cmd-0.3.3/cid/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/account_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    22951 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/athena.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/csv2view.py
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/cur.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/glue.py
--rw-r--r--   0 runner    (1001) docker     (127)    21978 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/iam.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/organizations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.275941 cid_cmd-0.3.3/cid/helpers/quicksight/
--rw-r--r--   0 runner    (1001) docker     (127)    68635 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/quicksight/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/quicksight/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/quicksight/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/quicksight/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/quicksight/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/randtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/timezone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.255941 cid_cmd-0.3.3/cid/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.275941 cid_cmd-0.3.3/cid/test/python/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/test/python/test_csv2view.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/test/python/test_isolated_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/test/python/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.275941 cid_cmd-0.3.3/cid_cmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-04-25 09:08:11.000000 cid_cmd-0.3.3/cid_cmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-25 09:08:11.000000 cid_cmd-0.3.3/cid_cmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:08:11.000000 cid_cmd-0.3.3/cid_cmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-25 09:08:11.000000 cid_cmd-0.3.3/cid_cmd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-25 09:08:11.000000 cid_cmd-0.3.3/cid_cmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-25 09:08:11.000000 cid_cmd-0.3.3/cid_cmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-25 09:08:11.275941 cid_cmd-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.543951 cid_cmd-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-05-17 09:29:57.543951 cid_cmd-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.519951 cid_cmd-0.3.4/cid/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.519951 cid_cmd-0.3.4/cid/builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.519951 cid_cmd-0.3.4/cid/builtin/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.519951 cid_cmd-0.3.4/cid/builtin/core/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.515951 cid_cmd-0.3.4/cid/builtin/core/data/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.523951 cid_cmd-0.3.4/cid/builtin/core/data/datasets/cid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/cid/compute.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/cid/ec2_running_cost.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/cid/s3_view.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/cid/summary_view.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.523951 cid_cmd-0.3.4/cid/builtin/core/data/datasets/co/
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/co/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.523951 cid_cmd-0.3.4/cid/builtin/core/data/datasets/cudos/
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/cudos/hourly_view.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/cudos/resource_view.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.523951 cid_cmd-0.3.4/cid/builtin/core/data/datasets/kpi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/kpi/kpi_ebs_snap.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/kpi/kpi_ebs_storage_all.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20695 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/kpi/kpi_instance_all.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/kpi/kpi_s3_storage_all.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/kpi/kpi_tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.523951 cid_cmd-0.3.4/cid/builtin/core/data/datasets/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)    30612 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/shared/customer_all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.523951 cid_cmd-0.3.4/cid/builtin/core/data/datasets/tao/
+-rw-r--r--   0 runner    (1001) docker     (127)    69315 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/tao/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.523951 cid_cmd-0.3.4/cid/builtin/core/data/datasets/trends/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/trends/daily_anomaly_detection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/trends/monthly_anomaly_detection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/datasets/trends/monthly_bill_by_account.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.523951 cid_cmd-0.3.4/cid/builtin/core/data/permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/permissions/dashboard_permissions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/permissions/dashboard_permissions_namespace.json
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/permissions/data_set_permissions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/permissions/data_source_permissions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/permissions/folder_permissions.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.515951 cid_cmd-0.3.4/cid/builtin/core/data/queries/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.527951 cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/compute_savings_plan_eligible_spend.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/ec2_running_cost.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/ec2_running_cost_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/ec2_running_cost_sp.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/ec2_running_cost_sp_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/ri_sp_mapping.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/ri_sp_mapping_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/s3.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/summary_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/summary_view_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/summary_view_sp.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/summary_view_sp_ri.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.531951 cid_cmd-0.3.4/cid/builtin/core/data/queries/co/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/co/all_options.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    14711 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/co/auto_scale.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27919 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/co/auto_scale_options.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     9097 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/co/ebs_volume.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22473 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/co/ebs_volume_options.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    19144 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/co/ec2_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28308 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/co/ec2_instance_options.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/co/lambda.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/co/lambda_options.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.531951 cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/hourly_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/hourly_view_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/hourly_view_sp.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/hourly_view_sp_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/resource_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/resource_view_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/resource_view_sp.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/resource_view_sp_ri.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.531951 cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/
+-rw-r--r--   0 runner    (1001) docker     (127)    11145 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/first_kpi_instance_mapping_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/kpi_ebs_snap_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/kpi_ebs_storage_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    24337 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/kpi_instance_all_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    23573 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRI.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    22559 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRISP.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    23434 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noSP.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/kpi_s3_storage_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/last_kpi_tracker_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.535951 cid_cmd-0.3.4/cid/builtin/core/data/queries/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/shared/account_map.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/shared/account_map_dummy.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/shared/aws_accounts.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/shared/aws_regions.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/shared/aws_service_category_map.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/shared/business_units_map.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/shared/cur.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/shared/payer_account_name_map.sql
+-rw-r--r--   0 runner    (1001) docker     (127)   163373 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/shared/ta_descriptions.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.535951 cid_cmd-0.3.4/cid/builtin/core/data/queries/tao/
+-rw-r--r--   0 runner    (1001) docker     (127)    35595 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/tao/glue_table.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/tao/ta_org_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.535951 cid_cmd-0.3.4/cid/builtin/core/data/queries/trends/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/trends/daily_anomaly_detection.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/trends/monthly_anomaly_detection.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/trends/monthly_bill_by_account.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/trends/monthly_bill_by_account_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    18712 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/builtin/core/data/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12646 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.535951 cid_cmd-0.3.4/cid/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/commands/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/commands/init_qs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92577 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19919 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.539951 cid_cmd-0.3.4/cid/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/account_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22951 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/athena.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/csv2view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/cur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/glue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22921 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/organizations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.539951 cid_cmd-0.3.4/cid/helpers/quicksight/
+-rw-r--r--   0 runner    (1001) docker     (127)    68649 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/quicksight/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/quicksight/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/quicksight/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/quicksight/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/quicksight/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/randtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/helpers/timezone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.515951 cid_cmd-0.3.4/cid/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.539951 cid_cmd-0.3.4/cid/test/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/test/python/test_csv2view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/test/python/test_isolated_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/test/python/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/cid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:29:57.543951 cid_cmd-0.3.4/cid_cmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-05-17 09:29:57.000000 cid_cmd-0.3.4/cid_cmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-17 09:29:57.000000 cid_cmd-0.3.4/cid_cmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:29:57.000000 cid_cmd-0.3.4/cid_cmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-17 09:29:57.000000 cid_cmd-0.3.4/cid_cmd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-17 09:29:57.000000 cid_cmd-0.3.4/cid_cmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-17 09:29:57.000000 cid_cmd-0.3.4/cid_cmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-17 09:29:50.000000 cid_cmd-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-17 09:29:57.543951 cid_cmd-0.3.4/setup.cfg
```

### Comparing `cid_cmd-0.3.3/LICENSE` & `cid_cmd-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/PKG-INFO` & `cid_cmd-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cid-cmd
-Version: 0.3.3
+Version: 0.3.4
 Summary: Cloud Intelligence Dashboards deployment helper tool
 Home-page: https://github.com/aws-samples/aws-cudos-framework-deployment
 Author: AWS CUDOS Team
 License: MIT
 Keywords: aws,cmd,cli,cost intelligence dashboards
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cid_cmd-0.3.3/README.md` & `cid_cmd-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/base.py` & `cid_cmd-0.3.4/cid/base.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/compute.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/cid/compute.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/ec2_running_cost.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/cid/ec2_running_cost.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/s3_view.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/cid/s3_view.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/summary_view.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/cid/summary_view.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/co/dataset.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/co/dataset.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/cudos/hourly_view.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/cudos/hourly_view.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/cudos/resource_view.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/cudos/resource_view.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_ebs_snap.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/kpi/kpi_ebs_snap.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_ebs_storage_all.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/kpi/kpi_ebs_storage_all.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_instance_all.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/kpi/kpi_instance_all.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_s3_storage_all.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/kpi/kpi_s3_storage_all.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_tracker.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/kpi/kpi_tracker.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/shared/customer_all.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/shared/customer_all.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/tao/dataset.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/tao/dataset.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/trends/daily_anomaly_detection.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/trends/daily_anomaly_detection.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/trends/monthly_anomaly_detection.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/trends/monthly_anomaly_detection.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/datasets/trends/monthly_bill_by_account.json` & `cid_cmd-0.3.4/cid/builtin/core/data/datasets/trends/monthly_bill_by_account.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/compute_savings_plan_eligible_spend.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/compute_savings_plan_eligible_spend.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ec2_running_cost.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/ec2_running_cost.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ec2_running_cost_ri.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/ec2_running_cost_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ec2_running_cost_sp.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/ec2_running_cost_sp.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ec2_running_cost_sp_ri.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/ec2_running_cost_sp_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ri_sp_mapping.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/ri_sp_mapping.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ri_sp_mapping_ri.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/ri_sp_mapping_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp_ri.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/s3.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/s3.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/summary_view.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/summary_view.sql`

 * *Files 1% similar despite different names*

```diff
@@ -79,9 +79,12 @@
  -- WHEN ("line_item_line_item_type" = 'SavingsPlanUpfrontFee') THEN "line_item_unblended_cost"
  -- WHEN (("line_item_line_item_type" = 'Fee') AND ("reservation_reservation_a_r_n" <> '')) THEN "line_item_unblended_cost"
  ELSE 0 END) AS double) "ri_sp_upfront_fees"
  , sum(CASE
      WHEN ("line_item_line_item_type" <> 'SavingsPlanNegation') THEN "pricing_public_on_demand_cost" ELSE 0 END) "public_cost"
  FROM
   "${cur_table_name}"
- WHERE (("bill_billing_period_start_date" >= ("date_trunc"('month', current_timestamp) - INTERVAL  '7' MONTH)) AND (CAST("concat"("year", '-', "month", '-01') AS date) >= ("date_trunc"('month', current_date) - INTERVAL  '7' MONTH)))
+ WHERE 
+    (("bill_billing_period_start_date" >= ("date_trunc"('month', current_timestamp) - INTERVAL  '7' MONTH)) 
+    AND (CAST("concat"("year", '-', "month", '-01') AS date) >= ("date_trunc"('month', current_date) - INTERVAL  '7' MONTH))
+    AND "line_item_operation" NOT IN ('EKSPod-EC2','ECSTask-EC2')) 
  GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32,33,34
```

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/summary_view_ri.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/summary_view_ri.sql`

 * *Files 1% similar despite different names*

```diff
@@ -69,10 +69,12 @@
  , sum(CASE
  -- WHEN ("line_item_line_item_type" = 'SavingsPlanUpfrontFee') THEN "line_item_unblended_cost"
      WHEN (("line_item_line_item_type" = 'Fee') AND ("reservation_reservation_a_r_n" <> '')) THEN "line_item_unblended_cost" ELSE 0 END) "ri_sp_upfront_fees"
  , sum(CASE
      WHEN ("line_item_line_item_type" <> 'SavingsPlanNegation') THEN "pricing_public_on_demand_cost" ELSE 0 END) "public_cost"
  FROM
   "${cur_table_name}"
- WHERE (("bill_billing_period_start_date" >= ("date_trunc"('month', current_timestamp) - INTERVAL  '7' MONTH)) AND (CAST("concat"("year", '-', "month", '-01') AS date) >= ("date_trunc"('month', current_date) - INTERVAL  '7' MONTH)))
-
+ WHERE 
+    (("bill_billing_period_start_date" >= ("date_trunc"('month', current_timestamp) - INTERVAL  '7' MONTH)) 
+    AND (CAST("concat"("year", '-', "month", '-01') AS date) >= ("date_trunc"('month', current_date) - INTERVAL  '7' MONTH))
+    AND "line_item_operation" NOT IN ('EKSPod-EC2','ECSTask-EC2'))
  GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32,33,34
```

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/summary_view_sp.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/summary_view_sp.sql`

 * *Files 2% similar despite different names*

```diff
@@ -73,10 +73,12 @@
      WHEN ("line_item_line_item_type" = 'SavingsPlanUpfrontFee') THEN "line_item_unblended_cost"
      -- WHEN (("line_item_line_item_type" = 'Fee') AND ("reservation_reservation_a_r_n" <> '')) THEN "line_item_unblended_cost"
      ELSE 0 END) "ri_sp_upfront_fees"
  , sum(CASE
      WHEN ("line_item_line_item_type" <> 'SavingsPlanNegation') THEN "pricing_public_on_demand_cost" ELSE 0 END) "public_cost"
  FROM
  "${cur_table_name}"
- WHERE (("bill_billing_period_start_date" >= ("date_trunc"('month', current_timestamp) - INTERVAL  '7' MONTH)) AND (CAST("concat"("year", '-', "month", '-01') AS date) >= ("date_trunc"('month', current_date) - INTERVAL  '7' MONTH)))
-
+  WHERE 
+    (("bill_billing_period_start_date" >= ("date_trunc"('month', current_timestamp) - INTERVAL  '7' MONTH)) 
+    AND (CAST("concat"("year", '-', "month", '-01') AS date) >= ("date_trunc"('month', current_date) - INTERVAL  '7' MONTH))
+    AND "line_item_operation" NOT IN ('EKSPod-EC2','ECSTask-EC2'))
  GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32,33,34
```

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/summary_view_sp_ri.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cid/summary_view_sp_ri.sql`

 * *Files 1% similar despite different names*

```diff
@@ -69,10 +69,12 @@
   , sum(CASE
       WHEN ("line_item_line_item_type" = 'SavingsPlanUpfrontFee') THEN "line_item_unblended_cost"
       WHEN (("line_item_line_item_type" = 'Fee') AND ("reservation_reservation_a_r_n" <> '')) THEN "line_item_unblended_cost"ELSE 0 END) "ri_sp_upfront_fees"
   , sum(CASE
       WHEN ("line_item_line_item_type" <> 'SavingsPlanNegation') THEN "pricing_public_on_demand_cost" ELSE 0 END) "public_cost"
   FROM
   "${cur_table_name}"
-  WHERE (("bill_billing_period_start_date" >= ("date_trunc"('month', current_timestamp) - INTERVAL  '7' MONTH)) AND (CAST("concat"("year", '-', "month", '-01') AS date) >= ("date_trunc"('month', current_date) - INTERVAL  '7' MONTH)))
-
+ WHERE 
+    (("bill_billing_period_start_date" >= ("date_trunc"('month', current_timestamp) - INTERVAL  '7' MONTH)) 
+    AND (CAST("concat"("year", '-', "month", '-01') AS date) >= ("date_trunc"('month', current_date) - INTERVAL  '7' MONTH))
+    AND "line_item_operation" NOT IN ('EKSPod-EC2','ECSTask-EC2'))
   GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34
```

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/co/auto_scale.json` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/co/auto_scale.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/co/auto_scale_options.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/co/auto_scale_options.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/co/ebs_volume.json` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/co/ebs_volume.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/co/ebs_volume_options.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/co/ebs_volume_options.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/co/ec2_instance.json` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/co/ec2_instance.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/co/ec2_instance_options.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/co/ec2_instance_options.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/co/lambda.json` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/co/lambda.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/co/lambda_options.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/co/lambda_options.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/hourly_view.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/hourly_view.sql`

 * *Files 7% similar despite different names*

```diff
@@ -17,9 +17,12 @@
   , CAST('' AS varchar) "reservation_a_r_n"
   , "sum"("line_item_unblended_cost") "unblended_cost"
   , CAST(0 AS double)  "reservation_effective_cost"
   , CAST(0 AS double) "savings_plan_effective_cost"
   , "sum"("line_item_usage_amount") "usage_quantity"
   FROM
     "${cur_table_name}"
-  WHERE (((current_date - INTERVAL  '30' DAY) <= line_item_usage_start_date) AND ((("line_item_line_item_type" = 'Usage') OR ("line_item_line_item_type" = 'SavingsPlanCoveredUsage')) OR ("line_item_line_item_type" = 'DiscountedUsage')))
-  GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
+  WHERE 
+    (((current_date - INTERVAL  '30' DAY) <= line_item_usage_start_date) 
+    AND ((("line_item_line_item_type" = 'Usage') OR ("line_item_line_item_type" = 'SavingsPlanCoveredUsage')) OR ("line_item_line_item_type" = 'DiscountedUsage'))
+    AND "line_item_operation" NOT IN ('EKSPod-EC2','ECSTask-EC2'))
+  GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
```

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/hourly_view_ri.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/hourly_view_ri.sql`

 * *Files 4% similar despite different names*

```diff
@@ -17,9 +17,12 @@
   , "reservation_reservation_a_r_n" "reservation_a_r_n"
   , "sum"("line_item_unblended_cost") "unblended_cost"
   , "sum"("reservation_effective_cost") "reservation_effective_cost"
   , CAST(0 AS double) "savings_plan_effective_cost"
   , "sum"("line_item_usage_amount") "usage_quantity"
   FROM
     "${cur_table_name}"
-  WHERE (((current_date - INTERVAL  '30' DAY) <= line_item_usage_start_date) AND ((("line_item_line_item_type" = 'Usage') OR ("line_item_line_item_type" = 'SavingsPlanCoveredUsage')) OR ("line_item_line_item_type" = 'DiscountedUsage')))
-  GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
+  WHERE 
+    (((current_date - INTERVAL  '30' DAY) <= line_item_usage_start_date) 
+    AND ((("line_item_line_item_type" = 'Usage') OR ("line_item_line_item_type" = 'SavingsPlanCoveredUsage')) OR ("line_item_line_item_type" = 'DiscountedUsage'))
+    AND "line_item_operation" NOT IN ('EKSPod-EC2','ECSTask-EC2'))  
+  GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
```

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/hourly_view_sp.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/hourly_view_sp.sql`

 * *Files 7% similar despite different names*

```diff
@@ -17,9 +17,12 @@
   , CAST('' AS varchar) "reservation_a_r_n"
   , "sum"("line_item_unblended_cost") "unblended_cost"
   , CAST(0 AS double) "reservation_effective_cost"
   , "sum"("savings_plan_savings_plan_effective_cost") "savings_plan_effective_cost"
   , "sum"("line_item_usage_amount") "usage_quantity"
   FROM
     "${cur_table_name}"
-  WHERE (((current_date - INTERVAL  '30' DAY) <= line_item_usage_start_date) AND ((("line_item_line_item_type" = 'Usage') OR ("line_item_line_item_type" = 'SavingsPlanCoveredUsage')) OR ("line_item_line_item_type" = 'DiscountedUsage')))
-  GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
+  WHERE 
+    (((current_date - INTERVAL  '30' DAY) <= line_item_usage_start_date) 
+    AND ((("line_item_line_item_type" = 'Usage') OR ("line_item_line_item_type" = 'SavingsPlanCoveredUsage')) OR ("line_item_line_item_type" = 'DiscountedUsage'))
+    AND "line_item_operation" NOT IN ('EKSPod-EC2','ECSTask-EC2'))
+  GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
```

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/hourly_view_sp_ri.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/hourly_view_sp_ri.sql`

 * *Files 9% similar despite different names*

```diff
@@ -17,9 +17,12 @@
     , "reservation_reservation_a_r_n" "reservation_a_r_n"
     , "sum"("line_item_unblended_cost") "unblended_cost"
     , "sum"("reservation_effective_cost") "reservation_effective_cost"
     , "sum"("savings_plan_savings_plan_effective_cost") "savings_plan_effective_cost"
     , "sum"("line_item_usage_amount") "usage_quantity"
     FROM
       "${cur_table_name}"
-    WHERE (((current_date - INTERVAL  '30' DAY) <= line_item_usage_start_date) AND ((("line_item_line_item_type" = 'Usage') OR ("line_item_line_item_type" = 'SavingsPlanCoveredUsage')) OR ("line_item_line_item_type" = 'DiscountedUsage')))
-    GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
+    WHERE 
+        (((current_date - INTERVAL  '30' DAY) <= line_item_usage_start_date) 
+        AND ((("line_item_line_item_type" = 'Usage') OR ("line_item_line_item_type" = 'SavingsPlanCoveredUsage')) OR ("line_item_line_item_type" = 'DiscountedUsage'))
+        AND "line_item_operation" NOT IN ('EKSPod-EC2','ECSTask-EC2'))    
+    GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
```

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/resource_view.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/resource_view.sql`

 * *Files 12% similar despite different names*

```diff
@@ -31,9 +31,12 @@
       , CAST('' AS varchar) "savings_plan_a_r_n"
       , CAST(0 AS double) savings_plan_effective_cost
       , CAST(0 AS double) reservation_effective_cost
       , "sum"("line_item_usage_amount") "usage_quantity"
       , "sum"("line_item_unblended_cost") unblended_cost
       FROM
         "${cur_table_name}"
-      WHERE (((current_date - INTERVAL  '30' DAY) <= line_item_usage_start_date) AND (line_item_resource_id <> ''))
-      GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29
+      WHERE 
+            (((current_date - INTERVAL  '30' DAY) <= line_item_usage_start_date) 
+            AND (line_item_resource_id <> '')
+            AND "line_item_operation" NOT IN ('EKSPod-EC2','ECSTask-EC2'))
+      GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29
```

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/resource_view_ri.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/resource_view_sp_ri.sql`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,19 @@
       , "product_operating_system" "platform"
       , "product_product_family" "product_family"
       , "product_servicecode" "service"
       , "product_storage" "product_storage"
       , "product_to_location" "product_to_location"
       , "product_volume_api_name" "product_volume_api_name"
       , "reservation_reservation_a_r_n" "reservation_a_r_n"
-      , CAST('' AS varchar) "savings_plan_a_r_n"
-      , CAST(0 AS double) savings_plan_effective_cost
+      , "savings_plan_savings_plan_a_r_n" "savings_plan_a_r_n"
+      , "sum"("savings_plan_savings_plan_effective_cost") savings_plan_effective_cost
       , "sum"("reservation_effective_cost") reservation_effective_cost
       , "sum"("line_item_usage_amount") "usage_quantity"
       , "sum"("line_item_unblended_cost") unblended_cost
       FROM
         "${cur_table_name}"
-      WHERE (((current_date - INTERVAL  '30' DAY) <= line_item_usage_start_date) AND (line_item_resource_id <> ''))
-      GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29
+      WHERE 
+            (((current_date - INTERVAL  '30' DAY) <= line_item_usage_start_date) 
+            AND (line_item_resource_id <> '')
+            AND "line_item_operation" NOT IN ('EKSPod-EC2','ECSTask-EC2'))
+      GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29
```

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/resource_view_sp.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/resource_view_sp.sql`

 * *Files 4% similar despite different names*

```diff
@@ -31,9 +31,12 @@
       , "savings_plan_savings_plan_a_r_n" "savings_plan_a_r_n"
       , "sum"("savings_plan_savings_plan_effective_cost") savings_plan_effective_cost
       , CAST(0 AS double) reservation_effective_cost
       , "sum"("line_item_usage_amount") "usage_quantity"
       , "sum"("line_item_unblended_cost") unblended_cost
       FROM
         "${cur_table_name}"
-      WHERE (((current_date - INTERVAL  '30' DAY) <= line_item_usage_start_date) AND (line_item_resource_id <> ''))
-      GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29
+      WHERE 
+            (((current_date - INTERVAL  '30' DAY) <= line_item_usage_start_date) 
+            AND (line_item_resource_id <> '')
+            AND "line_item_operation" NOT IN ('EKSPod-EC2','ECSTask-EC2'))
+      GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29
```

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/resource_view_sp_ri.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/cudos/resource_view_ri.sql`

 * *Files 17% similar despite different names*

```diff
@@ -24,16 +24,19 @@
       , "product_operating_system" "platform"
       , "product_product_family" "product_family"
       , "product_servicecode" "service"
       , "product_storage" "product_storage"
       , "product_to_location" "product_to_location"
       , "product_volume_api_name" "product_volume_api_name"
       , "reservation_reservation_a_r_n" "reservation_a_r_n"
-      , "savings_plan_savings_plan_a_r_n" "savings_plan_a_r_n"
-      , "sum"("savings_plan_savings_plan_effective_cost") savings_plan_effective_cost
+      , CAST('' AS varchar) "savings_plan_a_r_n"
+      , CAST(0 AS double) savings_plan_effective_cost
       , "sum"("reservation_effective_cost") reservation_effective_cost
       , "sum"("line_item_usage_amount") "usage_quantity"
       , "sum"("line_item_unblended_cost") unblended_cost
       FROM
         "${cur_table_name}"
-      WHERE (((current_date - INTERVAL  '30' DAY) <= line_item_usage_start_date) AND (line_item_resource_id <> ''))
-      GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29
+      WHERE 
+            (((current_date - INTERVAL  '30' DAY) <= line_item_usage_start_date) 
+            AND (line_item_resource_id <> '')
+            AND "line_item_operation" NOT IN ('EKSPod-EC2','ECSTask-EC2'))
+      GROUP BY 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29
```

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/first_kpi_instance_mapping_view.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/first_kpi_instance_mapping_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_ebs_snap_view.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/kpi_ebs_snap_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_ebs_storage_view.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/kpi_ebs_storage_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_instance_all_view.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/kpi_instance_all_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRI.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRI.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRISP.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRISP.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noSP.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noSP.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_s3_storage_view.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/kpi_s3_storage_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/last_kpi_tracker_view.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/kpi/last_kpi_tracker_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/aws_accounts.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/shared/aws_accounts.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/aws_regions.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/shared/aws_regions.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/aws_service_category_map.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/shared/aws_service_category_map.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/cur.yaml` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/shared/cur.yaml`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/ta_descriptions.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/shared/ta_descriptions.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/tao/glue_table.json` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/tao/glue_table.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/tao/ta_org_view.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/tao/ta_org_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/daily_anomaly_detection.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/trends/daily_anomaly_detection.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_anomaly_detection.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/trends/monthly_anomaly_detection.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_bill_by_account.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/trends/monthly_bill_by_account.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_bill_by_account_ri.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/trends/monthly_bill_by_account_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp_ri.sql` & `cid_cmd-0.3.4/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/builtin/core/data/resources.yaml` & `cid_cmd-0.3.4/cid/builtin/core/data/resources.yaml`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/cli.py` & `cid_cmd-0.3.4/cid/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,15 @@
      --dashboard-id TEXT                   QuickSight dashboard id (cudos, cost_intelligence_dashboard, kpi_dashboard, ta-organizational-view, trends-dashboard etc)
      --athena-database TEXT                Athena database
      --athena-workgroup TEXT               Athena workgroup
      --glue-data-catalog TEXT              Glue data catalog
      --cur-table-name TEXT                 CUR table name
      --quicksight-datasource-id TEXT       QuickSight Datasource ARN (if not found one with provided Athena workgroup)
      --quicksight-datasource-role-arn TEXT IAM Role used for DataSource Creation (if not provided, will use the default QS Role). Must have access to Athena and S3 buckets.
+     --allow-buckets                       Comma separated list of buckets names to add to the default Cid QuickSight role
      --quicksight-user TEXT                QuickSight user
      --dataset-{dataset_name}-id TEXT      QuickSight dataset id for a specific dataset
      --view-{view_name}-{parameter} TEXT   a custom parameter for a view creation, can use variable: {account_id}
      --account-map-source TEXT             csv, dummy, organization (if autodiscovery impossible)
      --account-map-file TEXT               csv file path relative to current directory (if autodiscovery impossible and csv selected as a source )
      --on-drift (show|override)            Action if a drift of view and dataset is discovered. 'override' = override drift(will destroy customization) or 'show' (default) = show a diff. In Unattended mode (without terminal on-drift will have allways override behaviour)
      --update (yes|no)                     Update if some elements are already installed. Default = 'no'
```

### Comparing `cid_cmd-0.3.3/cid/commands/init_qs.py` & `cid_cmd-0.3.4/cid/commands/init_qs.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/common.py` & `cid_cmd-0.3.4/cid/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1296,19 +1296,19 @@
         """Create datasource with given id
         uses parameters: 'quicksight-datasource-role-arn', 'quicksight-datasource-role'
         """
         role_arn = get_parameters().get('quicksight-datasource-role-arn')
         if not role_arn:
             role_name = get_parameters().get('quicksight-datasource-role')
             if role_name:
-                role_arn = f'arn:aws:iam::{self.base.account_id}:role/{role_name}'
+                role_arn = self.iam.get_role_arn(role_name)
 
         if not role_arn:
             quicksight_trusted_roles = list(self.iam.iterate_role_names(search="Roles[?AssumeRolePolicyDocument.Statement[?Principal.Service=='quicksight.amazonaws.com']].RoleName"))
-            #quicksight_trusted_roles = [role for role in quicksight_trusted_roles if role not in ('aws-quicksight-secretsmanager-role-v0')] # filter out irrelevant roles
+            quicksight_trusted_roles = [role for role in quicksight_trusted_roles if role not in ('aws-quicksight-secretsmanager-role-v0')] # filter out irrelevant roles
             # TODO: filter only roles with Athena and S3 policies
             cid_role_name = 'CidCmdQuickSightDataSourceRole'
             choices = quicksight_trusted_roles
             default = None
             if cid_role_name not in choices:
                 choices.append(cid_role_name + ' <ADD NEW ROLE>' )
                 default = cid_role_name + ' <ADD NEW ROLE>'
@@ -1317,33 +1317,37 @@
             choice = get_parameter(
                 'quicksight-datasource-role',
                 message='Please choose a QuickSight role. It must have access to Athena',
                 choices=['<USE DEFAULT QuickSight ROLE (You will need to login to QuickSight Security and Permissions management and configure S3 and Athena access there)>'] + choices,
                 default=default,
             )
             if "<ADD NEW ROLE>" in choice or choice == cid_role_name: # Create or update role
-                # TODO: allow customer add buckets
+                # TODO: get buckets from dashboard parameters
                 buckets = [
                     f'cid-{self.base.account_id}-share',
                     f'cid-data-{self.base.account_id}',
                     f'costoptimizationdata{self.base.account_id}',
                 ]
+                additional_buckets = get_parameters().get('allow-buckets')
+                if additional_buckets:
+                    buckets += additional_buckets.split(',')
+
                 role_name = self.iam.ensure_data_source_role_exists(
                     role_name=cid_role_name,
                     database=self.athena.DatabaseName,
                     workgroup=self.athena.WorkGroup,
                     buckets=buckets,
                     output_location_bucket = self.athena.workgroup_output_location().split('/')[2],
                 )
                 cid_print(f'Role {role_name} was updated. https://console.aws.amazon.com/iam/home?#/roles/details/{role_name}')
-                role_arn = f'arn:aws:iam::{self.base.account_id}:role/{role_name}'
-            elif 'USE DEFAULT QuickSight ROLE' in choice:
+                role_arn = self.iam.get_role_arn(role_name)
+            elif 'USE DEFAULT QuickSight ROLE' in choice or choice == 'default':
                 role_arn = None
             else:
-                role_arn = choice
+                role_arn = self.iam.get_role_arn(choice)
 
         athena_datasource = self.qs.create_data_source(
             athena_workgroup=self.athena.WorkGroup,
             datasource_id=datasource_id,
             role_arn=role_arn,
         )
         print('athena_datasource', athena_datasource)
@@ -1706,15 +1710,15 @@
                 s3bucket=location.split('/')[2],
                 database=self.athena.DatabaseName,
                 table=table,
                 role_name=crawler_role
             )
 
         if not crawler_role.startswith('arn:'):
-            crawler_role_arn = f"arn:aws:iam::{self.base.account_id}:role/{crawler_role}"
+            crawler_role_arn = f"arn:{self.base.partition}:iam::{self.base.account_id}:role/{crawler_role}"
         else:
             crawler_role_arn = crawler_role
         params = {
             'athena_database_name': self.athena.DatabaseName,
             'crawler_role_arn': crawler_role_arn,
             'location': location,
         }
```

### Comparing `cid_cmd-0.3.3/cid/export.py` & `cid_cmd-0.3.4/cid/export.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/helpers/__init__.py` & `cid_cmd-0.3.4/cid/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/helpers/account_map.py` & `cid_cmd-0.3.4/cid/helpers/account_map.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/helpers/athena.py` & `cid_cmd-0.3.4/cid/helpers/athena.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/helpers/csv2view.py` & `cid_cmd-0.3.4/cid/helpers/csv2view.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/helpers/cur.py` & `cid_cmd-0.3.4/cid/helpers/cur.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/helpers/diff.py` & `cid_cmd-0.3.4/cid/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/helpers/glue.py` & `cid_cmd-0.3.4/cid/helpers/glue.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/helpers/iam.py` & `cid_cmd-0.3.4/cid/helpers/iam.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import copy
 import time
 import logging
 
 import boto3
 from tqdm import tqdm
 
-from cid.exceptions import CidCritical
+from cid.exceptions import CidCritical, CidError
 from cid.base import CidBase
 from cid.utils import get_parameter
 
 logger = logging.getLogger(__name__)
 
 
 class IAM(CidBase):
@@ -57,21 +57,21 @@
                 policy_name: {
                     "Version": "2012-10-17",
                     "Statement": [
                         {
                             "Sid": "AllowListBucket",
                             "Effect": "Allow",
                             "Action": ["s3:ListBucket"],
-                            "Resource": [f"arn:aws:s3:::{s3bucket}"]
+                            "Resource": [f"arn:{self.partition}:s3:::{s3bucket}"]
                         },
                         {
                             "Sid": "AllowReadFromBucket",
                             "Effect": "Allow",
                             "Action": [ "s3:GetObject"],
-                            "Resource": [f"arn:aws:s3:::{s3bucket}/*"]
+                            "Resource": [f"arn:{self.partition}:s3:::{s3bucket}/*"]
                         },
                         {
                             "Sid": "AllowGlueActions",
                             "Effect": "Allow",
                             "Action": [
                                 "glue:GetDatabase",
                                 "glue:GetDatabases",
@@ -147,14 +147,15 @@
                         {
                             "Sid": "AllowGlue",
                             "Effect": "Allow",
                             "Action": [
                                 "glue:GetPartition",
                                 "glue:GetPartitions",
                                 "glue:GetDatabases",
+                                "glue:GetDatabase",
                                 "glue:GetTable",
                                 "glue:GetTables",
                             ],
                             "Resource": [
                                 f"arn:{self.partition}:glue:{self.region}:{self.account_id}:catalog",
                                 f"arn:{self.partition}:glue:{self.region}:{self.account_id}:database/{database}",
                                 f"arn:{self.partition}:glue:{self.region}:{self.account_id}:table/{database}/*",
@@ -319,14 +320,30 @@
         """ Iterate role names
         """
         try:
             yield from self.client.get_paginator('list_roles').paginate().search(search)
         except self.client.exceptions.ClientError as exc:
             logger.warning('Failed to read available IEM roles: {exc}. Most likely not fatal.')
 
+    def get_role_arn(self, role_name:str) -> str:
+        """ Get role arn, and try the best guess if no permissions
+        """
+        try:
+            return self.client.get_role(RoleName=role_name)['Role']['Arn']
+        except self.client.exceptions.NoSuchEntityException:
+            raise CidError(f"Role '{role_name}' does not exist.")
+        except self.client.exceptions.ClientError as exc:
+            if "AccessDenied" in str(exc):
+                logger.debug('Got access denied for describing role. Try the best guess')
+                if role_name.startswith('aws-quicksight-service-role'):
+                    return f'arn:aws:iam::{self.account_id}:role/service-role/{role_name}'
+                else:
+                    return f'arn:aws:iam::{self.account_id}:role/{role_name}'
+            raise CidError(f"An error occurred: {exc}")
+
     def ensure_role_does_not_exist(self, role_name):
         """ Remove a role and all policies if they are not used in other roles
         """
         try:
             self.client.get_role(RoleName=role_name)
         except self.client.exceptions.NoSuchEntityException:
             logger.debug(f'No role {role_name}')
```

### Comparing `cid_cmd-0.3.3/cid/helpers/organizations.py` & `cid_cmd-0.3.4/cid/helpers/organizations.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/helpers/quicksight/__init__.py` & `cid_cmd-0.3.4/cid/helpers/quicksight/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1334,15 +1334,15 @@
             'DashboardId': definition.get('dashboardId'),
             'Name': definition.get('name'),
             'ValidationStrategy': {'Mode': 'LENIENT'},
         }
         theme = definition.get('theme')
         if theme:
             if not theme.startswith('arn:'):
-                theme_arn = 'arn:aws:quicksight::aws:theme/' + theme
+                theme_arn = f'arn:{self.partition}:quicksight::aws:theme/' + theme
             else:
                 raise NotImplementedError('Only standard themes are supported now.')
             create_parameters['ThemeArn'] = theme_arn
 
         if definition.get('sourceTemplate'):
             dataset_references = [
                 {'DataSetPlaceholder': key, 'DataSetArn': value}
```

### Comparing `cid_cmd-0.3.3/cid/helpers/quicksight/dashboard.py` & `cid_cmd-0.3.4/cid/helpers/quicksight/dashboard.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/helpers/quicksight/dataset.py` & `cid_cmd-0.3.4/cid/helpers/quicksight/dataset.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/helpers/quicksight/datasource.py` & `cid_cmd-0.3.4/cid/helpers/quicksight/datasource.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/helpers/quicksight/template.py` & `cid_cmd-0.3.4/cid/helpers/quicksight/template.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/helpers/randtime.py` & `cid_cmd-0.3.4/cid/helpers/randtime.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/helpers/s3.py` & `cid_cmd-0.3.4/cid/helpers/s3.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/helpers/timezone.py` & `cid_cmd-0.3.4/cid/helpers/timezone.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/logger.py` & `cid_cmd-0.3.4/cid/logger.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/plugin.py` & `cid_cmd-0.3.4/cid/plugin.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/test/python/test_merge.py` & `cid_cmd-0.3.4/cid/test/python/test_merge.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid/utils.py` & `cid_cmd-0.3.4/cid/utils.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/cid_cmd.egg-info/PKG-INFO` & `cid_cmd-0.3.4/cid_cmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cid-cmd
-Version: 0.3.3
+Version: 0.3.4
 Summary: Cloud Intelligence Dashboards deployment helper tool
 Home-page: https://github.com/aws-samples/aws-cudos-framework-deployment
 Author: AWS CUDOS Team
 License: MIT
 Keywords: aws,cmd,cli,cost intelligence dashboards
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cid_cmd-0.3.3/cid_cmd.egg-info/SOURCES.txt` & `cid_cmd-0.3.4/cid_cmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.3/setup.cfg` & `cid_cmd-0.3.4/setup.cfg`

 * *Files identical despite different names*

