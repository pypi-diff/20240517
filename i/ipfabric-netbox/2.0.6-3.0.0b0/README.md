# Comparing `tmp/ipfabric_netbox-2.0.6.tar.gz` & `tmp/ipfabric_netbox-3.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric_netbox-2.0.6.tar", last modified: Tue May 14 16:19:48 2024, max compression
+gzip compressed data, was "ipfabric_netbox-3.0.0b0.tar", last modified: Fri May 17 12:51:59 2024, max compression
```

## Comparing `ipfabric_netbox-2.0.6.tar` & `ipfabric_netbox-3.0.0b0.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/
--rw-r--r--   0 root         (0) root         (0)       46 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1750 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1141 2024-03-11 10:17:28.000000 ipfabric_netbox-2.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.386452 ipfabric_netbox-2.0.6/ipfabric_netbox/
--rw-r--r--   0 root         (0) root         (0)     1251 2024-05-14 16:18:34.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.390452 ipfabric_netbox-2.0.6/ipfabric_netbox/api/
--rw-r--r--   0 root         (0) root         (0)      101 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2684 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/api/nested_serializers.py
--rw-r--r--   0 root         (0) root         (0)     4307 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/api/serializers.py
--rw-r--r--   0 root         (0) root         (0)      948 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/api/urls.py
--rw-r--r--   0 root         (0) root         (0)     4429 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/api/views.py
--rw-r--r--   0 root         (0) root         (0)     4848 2024-04-23 10:08:08.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/choices.py
--rw-r--r--   0 root         (0) root         (0)     3877 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/filtersets.py
--rw-r--r--   0 root         (0) root         (0)    43154 2024-04-30 10:44:55.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/forms.py
--rw-r--r--   0 root         (0) root         (0)     2395 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/jobs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.390452 ipfabric_netbox-2.0.6/ipfabric_netbox/migrations/
--rw-r--r--   0 root         (0) root         (0)    13813 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      431 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/migrations/0002_ipfabricsnapshot_status.py
--rw-r--r--   0 root         (0) root         (0)     1579 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/migrations/0003_ipfabricsource_type_and_more.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/migrations/0004_ipfabricsync_auto_merge.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29506 2024-05-14 16:17:46.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/models.py
--rw-r--r--   0 root         (0) root         (0)     1907 2024-03-11 10:17:28.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/navigation.py
--rw-r--r--   0 root         (0) root         (0)     3357 2024-04-30 10:44:55.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/signals.py
--rw-r--r--   0 root         (0) root         (0)     6630 2024-04-30 10:44:55.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/tables.py
--rw-r--r--   0 root         (0) root         (0)      315 2024-03-08 10:45:55.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/template_content.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.386452 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.390452 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/
--rw-r--r--   0 root         (0) root         (0)     3229 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/diff.html
--rw-r--r--   0 root         (0) root         (0)      569 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/json.html
--rw-r--r--   0 root         (0) root         (0)      295 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/logs_pending.html
--rw-r--r--   0 root         (0) root         (0)      710 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/merge_form.html
--rw-r--r--   0 root         (0) root         (0)     2674 2024-03-18 10:24:22.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_button.html
--rw-r--r--   0 root         (0) root         (0)     2136 2024-03-11 10:17:28.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_modal.html
--rw-r--r--   0 root         (0) root         (0)     2885 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/snapshotdata.html
--rw-r--r--   0 root         (0) root         (0)      717 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/sync_delete.html
--rw-r--r--   0 root         (0) root         (0)      517 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/transform_map_field_map.html
--rw-r--r--   0 root         (0) root         (0)      521 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/transform_map_relationship_map.html
--rw-r--r--   0 root         (0) root         (0)     1631 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabric_table.html
--rw-r--r--   0 root         (0) root         (0)     6444 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabricbranch.html
--rw-r--r--   0 root         (0) root         (0)     3482 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsnapshot.html
--rw-r--r--   0 root         (0) root         (0)     3859 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsource.html
--rw-r--r--   0 root         (0) root         (0)     3881 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsync.html
--rw-r--r--   0 root         (0) root         (0)     1100 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap.html
--rw-r--r--   0 root         (0) root         (0)      459 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_list.html
--rw-r--r--   0 root         (0) root         (0)     2562 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_restore.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/partials/
--rw-r--r--   0 root         (0) root         (0)      368 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_all.html
--rw-r--r--   0 root         (0) root         (0)      590 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_progress.html
--rw-r--r--   0 root         (0) root         (0)       81 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_status.html
--rw-r--r--   0 root         (0) root         (0)     1631 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/partials/job_logs.html
--rw-r--r--   0 root         (0) root         (0)      167 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/partials/sync_last_branch.html
--rw-r--r--   0 root         (0) root         (0)     5606 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/sync_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.386452 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.386452 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/static/ipfabric_netbox/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/static/ipfabric_netbox/css/
--rw-r--r--   0 root         (0) root         (0)      118 2024-03-11 10:17:28.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/static/ipfabric_netbox/css/rack.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/ipfabric_netbox/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45898 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/tests/test_models.py
--rw-r--r--   0 root         (0) root         (0)     4430 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20439 2024-05-14 16:18:34.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/ipfutils.py
--rw-r--r--   0 root         (0) root         (0)     3221 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/logging.py
--rw-r--r--   0 root         (0) root         (0)     3119 2024-04-30 10:44:55.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/nbutils.py
--rw-r--r--   0 root         (0) root         (0)     1256 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/transform_map.py
--rw-r--r--   0 root         (0) root         (0)    28517 2024-03-18 10:24:22.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1750 2024-05-14 16:19:48.000000 ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2942 2024-05-14 16:19:48.000000 ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 16:19:48.000000 ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 17:00:30.000000 ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-14 16:19:48.000000 ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-14 16:19:48.000000 ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      961 2024-05-14 16:18:34.000000 ipfabric_netbox-2.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:51:59.547341 ipfabric_netbox-3.0.0b0/
+-rw-r--r--   0 root         (0) root         (0)       46 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1752 2024-05-17 12:51:59.547341 ipfabric_netbox-3.0.0b0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-03-11 10:17:28.000000 ipfabric_netbox-3.0.0b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:51:59.519341 ipfabric_netbox-3.0.0b0/ipfabric_netbox/
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:51:59.523341 ipfabric_netbox-3.0.0b0/ipfabric_netbox/api/
+-rw-r--r--   0 root         (0) root         (0)      101 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/api/nested_serializers.py
+-rw-r--r--   0 root         (0) root         (0)     4307 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/api/serializers.py
+-rw-r--r--   0 root         (0) root         (0)      948 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/api/urls.py
+-rw-r--r--   0 root         (0) root         (0)     4429 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/api/views.py
+-rw-r--r--   0 root         (0) root         (0)     4848 2024-04-23 10:08:08.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/choices.py
+-rw-r--r--   0 root         (0) root         (0)     3877 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/filtersets.py
+-rw-r--r--   0 root         (0) root         (0)    43205 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/forms.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/jobs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:51:59.527341 ipfabric_netbox-3.0.0b0/ipfabric_netbox/migrations/
+-rw-r--r--   0 root         (0) root         (0)    13813 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      431 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/migrations/0002_ipfabricsnapshot_status.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/migrations/0003_ipfabricsource_type_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/migrations/0004_ipfabricsync_auto_merge.py
+-rw-r--r--   0 root         (0) root         (0)     2802 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/migrations/0005_alter_ipfabricrelationshipfield_source_model_and_more.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29555 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/models.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/navigation.py
+-rw-r--r--   0 root         (0) root         (0)     2588 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/signals.py
+-rw-r--r--   0 root         (0) root         (0)     6613 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/tables.py
+-rw-r--r--   0 root         (0) root         (0)      315 2024-03-08 10:45:55.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/template_content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:51:59.515341 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:51:59.531341 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:51:59.539341 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/diff.html
+-rw-r--r--   0 root         (0) root         (0)      569 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/json.html
+-rw-r--r--   0 root         (0) root         (0)      295 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/logs_pending.html
+-rw-r--r--   0 root         (0) root         (0)      710 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/merge_form.html
+-rw-r--r--   0 root         (0) root         (0)     2674 2024-03-18 10:24:22.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_button.html
+-rw-r--r--   0 root         (0) root         (0)     2124 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_modal.html
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/snapshotdata.html
+-rw-r--r--   0 root         (0) root         (0)      717 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/sync_delete.html
+-rw-r--r--   0 root         (0) root         (0)      500 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/transform_map_field_map.html
+-rw-r--r--   0 root         (0) root         (0)      504 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/transform_map_relationship_map.html
+-rw-r--r--   0 root         (0) root         (0)     1631 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/ipfabric_table.html
+-rw-r--r--   0 root         (0) root         (0)     4694 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/ipfabricbranch.html
+-rw-r--r--   0 root         (0) root         (0)     3482 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsnapshot.html
+-rw-r--r--   0 root         (0) root         (0)     3845 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsource.html
+-rw-r--r--   0 root         (0) root         (0)     3867 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsync.html
+-rw-r--r--   0 root         (0) root         (0)     1100 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap.html
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_list.html
+-rw-r--r--   0 root         (0) root         (0)     2562 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_restore.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:51:59.543341 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/partials/
+-rw-r--r--   0 root         (0) root         (0)      368 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_all.html
+-rw-r--r--   0 root         (0) root         (0)      590 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_progress.html
+-rw-r--r--   0 root         (0) root         (0)       81 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_status.html
+-rw-r--r--   0 root         (0) root         (0)     1622 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/partials/job_logs.html
+-rw-r--r--   0 root         (0) root         (0)      167 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/partials/sync_last_branch.html
+-rw-r--r--   0 root         (0) root         (0)     5587 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/sync_list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:51:59.515341 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:51:59.515341 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/static/ipfabric_netbox/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:51:59.543341 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/static/ipfabric_netbox/css/
+-rw-r--r--   0 root         (0) root         (0)      118 2024-03-11 10:17:28.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/static/ipfabric_netbox/css/rack.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:51:59.543341 ipfabric_netbox-3.0.0b0/ipfabric_netbox/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45898 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/tests/test_models.py
+-rw-r--r--   0 root         (0) root         (0)     4430 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:51:59.547341 ipfabric_netbox-3.0.0b0/ipfabric_netbox/utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20437 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/utilities/ipfutils.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/utilities/logging.py
+-rw-r--r--   0 root         (0) root         (0)     3117 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/utilities/nbutils.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/utilities/transform_map.py
+-rw-r--r--   0 root         (0) root         (0)    28452 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:51:59.547341 ipfabric_netbox-3.0.0b0/ipfabric_netbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1752 2024-05-17 12:51:59.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3031 2024-05-17 12:51:59.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 12:51:59.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 17:00:30.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 12:51:59.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-17 12:51:59.000000 ipfabric_netbox-3.0.0b0/ipfabric_netbox.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 12:51:59.547341 ipfabric_netbox-3.0.0b0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      963 2024-05-17 12:51:53.000000 ipfabric_netbox-3.0.0b0/setup.py
```

### Comparing `ipfabric_netbox-2.0.6/PKG-INFO` & `ipfabric_netbox-3.0.0b0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfabric_netbox
-Version: 2.0.6
+Version: 3.0.0b0
 Summary: NetBox plugin to sync IP Fabric data into NetBox
 Home-page: https://gitlab.com/ip-fabric/integrations/ipfabric-netbox-sync
 Author: Solution Architecture
 Author-email: solution.architecture@ipfabric.io
 Project-URL: Bug Tracker, https://gitlab.com/ip-fabric/integrations/ipfabric-netbox-sync/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipfabric_netbox-2.0.6/README.md` & `ipfabric_netbox-3.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/__init__.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 import requests
 from django.db import connection
-from extras.plugins import PluginConfig
+from netbox.plugins import PluginConfig
 
 
 class NetboxIPFabricConfig(PluginConfig):
     name = "ipfabric_netbox"
     verbose_name = "NetBox IP Fabric SoT Plugin"
     description = "Sync IP Fabric into NetBox"
-    version = "2.0.6"
+    version = "3.0.0b0"
     base_url = "ipfabric"
 
     def ready(self):
         super().ready()
         try:
             from ipfabric_netbox.signals import ipfabric_netbox_init
 
             all_tables = connection.introspection.table_names()
-            if "extras_customfield" in all_tables:
+            if all(
+                item in all_tables
+                for item in [
+                    "extras_customfield",
+                    "ipfabric_netbox_ipfabricbranch",
+                    "ipfabric_netbox_ipfabricsource",
+                ]
+            ):
                 ipfabric_netbox_init()
             if "ipfabric_netbox_ipfabrictransformmap" in all_tables:
                 from ipfabric_netbox.models import IPFabricTransformMap
                 from ipfabric_netbox.utilities.transform_map import BuildTransformMaps
 
                 if IPFabricTransformMap.objects.count() == 0:
                     data = requests.get(
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/api/nested_serializers.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/api/serializers.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/api/serializers.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/api/urls.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/api/urls.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/api/views.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/api/views.py`

 * *Files identical despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.db import transaction
 from netbox.api.viewsets import NetBoxModelViewSet
 from netbox.api.viewsets import NetBoxReadOnlyModelViewSet
 from rest_framework.decorators import action
 from rest_framework.response import Response
-from utilities.utils import count_related
+from utilities.query import count_related
 
 from .serializers import IPFabricBranchSerializer
 from .serializers import IPFabricRelationshipFieldSerializer
 from .serializers import IPFabricSnapshotSerializer
 from .serializers import IPFabricSourceSerializer
 from .serializers import IPFabricSyncSerializer
 from .serializers import IPFabricTransformFieldSerializer
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/choices.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/choices.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/filtersets.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/filtersets.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/forms.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 from core.choices import DataSourceStatusChoices
 from django import forms
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ValidationError
 from django.utils import timezone
-from django.utils.translation import gettext as _
+from django.utils.translation import gettext_lazy as _
 from extras.choices import DurationChoices
 from netbox.forms import NetBoxModelFilterSetForm
 from netbox.forms import NetBoxModelForm
 from packaging import version
+from utilities.datetime import local_now
 from utilities.forms import add_blank_choice
-from utilities.forms import BootstrapMixin
 from utilities.forms import FilterForm
 from utilities.forms import get_field_value
 from utilities.forms.fields import CommentField
 from utilities.forms.fields import DynamicModelChoiceField
 from utilities.forms.fields import DynamicModelMultipleChoiceField
+from utilities.forms.rendering import FieldSet
 from utilities.forms.widgets import APISelectMultiple
 from utilities.forms.widgets import DateTimePicker
 from utilities.forms.widgets import HTMXSelect
 from utilities.forms.widgets import NumberWithOptions
-from utilities.utils import local_now
 
 from .choices import IPFabricSnapshotStatusModelChoices
 from .choices import transform_field_source_columns
 from .models import IPFabricBranch
 from .models import IPFabricRelationshipField
 from .models import IPFabricSnapshot
 from .models import IPFabricSource
@@ -121,29 +121,32 @@
 def list_to_choices(choices):
     new_choices = ()
     for choice in choices:
         new_choices = new_choices + ((choice, choice),)
     return new_choices
 
 
-class IPFabricRelationshipFieldForm(BootstrapMixin, forms.ModelForm):
+class IPFabricRelationshipFieldForm(NetBoxModelForm):
     coalesce = forms.BooleanField(required=False, initial=False)
     target_field = forms.CharField(
         label="Target Field",
         required=True,
         help_text="Select target model field.",
         widget=forms.Select(),
     )
 
     fieldsets = (
-        (
-            "Transform Map",
-            ("transform_map", "source_model", "target_field", "coalesce"),
+        FieldSet(
+            "transform_map",
+            "source_model",
+            "target_field",
+            "coalesce",
+            name=_("Transform Map"),
         ),
-        ("Extras", ("template",)),
+        FieldSet("template", name=_("Extras")),
     )
 
     class Meta:
         model = IPFabricRelationshipField
         fields = (
             "transform_map",
             "source_model",
@@ -189,15 +192,15 @@
                         if f.is_relation and f.name not in exclude_fields
                     ]
                     self.fields["target_field"].widget.choices = add_blank_choice(
                         choices
                     )
 
 
-class IPFabricTransformFieldForm(BootstrapMixin, forms.ModelForm):
+class IPFabricTransformFieldForm(NetBoxModelForm):
     coalesce = forms.BooleanField(required=False, initial=False)
     source_field = forms.CharField(
         label="Source Field",
         required=True,
         help_text="Select column from IP Fabric.",
         widget=forms.Select(),
     )
@@ -205,19 +208,22 @@
         label="Target Field",
         required=True,
         help_text="Select target model field.",
         widget=forms.Select(),
     )
 
     fieldsets = (
-        (
-            "Transform Map",
-            ("transform_map", "source_field", "target_field", "coalesce"),
+        FieldSet(
+            "transform_map",
+            "source_field",
+            "target_field",
+            "coalesce",
+            name=_("Transform Map"),
         ),
-        ("Extras", ("template",)),
+        FieldSet("template", name=_("Extras")),
     )
 
     class Meta:
         model = IPFabricTransformField
         fields = (
             "transform_map",
             "source_field",
@@ -271,15 +277,15 @@
                         choices
                     )
                     self.fields["source_field"].widget.choices = add_blank_choice(
                         source_column_choices(transform_map.source_model)
                     )
 
 
-class IPFabricTransformMapForm(BootstrapMixin, forms.ModelForm):
+class IPFabricTransformMapForm(forms.ModelForm):
     status = forms.CharField(
         required=False,
         label=_("Status"),
         widget=forms.Select(),
     )
 
     class Meta:
@@ -320,38 +326,38 @@
                     except Exception as e:  # noqa: F841
                         self.fields["status"].widget.attrs["disabled"] = "disabled"
 
 
 class IPFabricSnapshotFilterForm(NetBoxModelFilterSetForm):
     model = IPFabricSnapshot
     fieldsets = (
-        (None, ("q", "filter_id")),
-        ("Source", ("name", "source_id", "status", "snapshot_id")),
+        FieldSet("q", "filter_id"),
+        FieldSet("name", "source_id", "status", "snapshot_id", name=_("Source")),
     )
     name = forms.CharField(required=False, label=_("Name"))
     status = forms.CharField(required=False, label=_("Status"))
     source_id = DynamicModelMultipleChoiceField(
         queryset=IPFabricSource.objects.all(), required=False, label=_("Source")
     )
     snapshot_id = forms.CharField(required=False, label=_("Snapshot ID"))
 
 
 class IPFabricSourceFilterForm(NetBoxModelFilterSetForm):
     model = IPFabricSource
     fieldsets = (
-        (None, ("q", "filter_id")),
-        ("Data Source", ("status",)),
+        FieldSet("q", "filter_id"),
+        FieldSet("status", name=_("Source")),
     )
     status = forms.MultipleChoiceField(choices=DataSourceStatusChoices, required=False)
 
 
 class IPFabricBranchFilterForm(SavedFiltersMixin, FilterForm):
     fieldsets = (
-        (None, ("q", "filter_id")),
-        ("Source", ("sync_id",)),
+        FieldSet("q", "filter_id"),
+        FieldSet("sync_id", name=_("Source")),
     )
     model = IPFabricBranch
     sync_id = DynamicModelMultipleChoiceField(
         queryset=IPFabricSync.objects.all(), required=False, label=_("Sync")
     )
 
 
@@ -370,19 +376,20 @@
         widgets = {
             "type": HTMXSelect(),
         }
 
     @property
     def fieldsets(self):
         fieldsets = [
-            (_("Source"), ("name", "type", "url")),
-            (_("Parameters"), ("timeout",)),
+            FieldSet("name", "type", "url", name=_("Source")),
+            FieldSet("timeout", name=_("Parameters")),
         ]
+
         if self.source_type == "local":
-            fieldsets[1] = (_("Parameters"), ("auth", "verify", "timeout"))
+            fieldsets[1] = FieldSet("auth", "verify", "timeout", name=_("Parameters"))
 
         return fieldsets
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.source_type = get_field_value(self, "type")
 
@@ -502,43 +509,33 @@
             "source": HTMXSelect(),
             "type": HTMXSelect(),
         }
 
     @property
     def fieldsets(self):
         fieldsets = [
-            (
-                "IP Fabric Source",
-                (
-                    "name",
-                    "source",
-                ),
-            ),
+            FieldSet("name", "source", name=_("IP Fabric Source")),
         ]
         if self.source_type == "local":
             fieldsets.append(
-                (
-                    "Snapshot Information",
-                    ("snapshot_data", "sites"),
-                )
+                FieldSet("snapshot_data", "sites", name=_("Snapshot Information")),
             )
         else:
             fieldsets.append(
-                (
-                    "Snapshot Information",
-                    ("snapshot_data",),
-                )
+                FieldSet("snapshot_data", name=_("Snapshot Information")),
             )
-        fieldsets.append(("Ingestion Type", ("type",)))
+        fieldsets.append(FieldSet("type", name=_("Ingestion Type")))
         if self.backend_fields:
             for k, v in self.backend_fields.items():
-                fieldsets.append((f"{k.upper()} Parameters", v))
-        fieldsets.append(("Ingestion Execution Parameters", ("scheduled", "interval")))
-        fieldsets.append(("Extras", ("auto_merge",)))
-        fieldsets.append(("Tags", ("tags",)))
+                fieldsets.append(FieldSet(*v, name=f"{k.upper()} Parameters"))
+        fieldsets.append(
+            FieldSet("scheduled", "interval", name=_("Ingestion Execution Parameters"))
+        )
+        fieldsets.append(FieldSet("auto_merge", name=_("Extras")))
+        fieldsets.append(FieldSet("tags", name=_("Tags")))
 
         return fieldsets
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.source_type = None
         ingestion_type = get_field_value(self, "source")
@@ -575,14 +572,15 @@
             backend[backend_type] = sync_parameters.get(backend_type)
 
         now = local_now().strftime("%Y-%m-%d %H:%M:%S")
         self.fields["scheduled"].help_text += f" (current time: <strong>{now}</strong>)"
 
         # Add backend-specific form fields
         self.backend_fields = {}
+
         for k, v in backend.items():
             self.backend_fields[k] = []
             for name, form_field in v.items():
                 field_name = f"ipf_{name}"
                 self.backend_fields[k].append(field_name)
                 self.fields[field_name] = copy.copy(form_field)
                 if self.instance and self.instance.parameters:
@@ -1036,15 +1034,15 @@
     ("stp.ports", "Stp - PORTS"),
     ("stp.vlans", "Stp - VLANS"),
     ("vlans.device_detail", "Vlans - DEVICE_DETAIL"),
     ("vlans.device_summary", "Vlans - DEVICE_SUMMARY"),
 ]
 
 
-class IPFabricTableForm(BootstrapMixin, forms.Form):
+class IPFabricTableForm(forms.Form):
     source = DynamicModelChoiceField(
         queryset=IPFabricSource.objects.all(),
         required=False,
         label=_("IP Fabric Source"),
     )
     snapshot_data = DynamicModelChoiceField(
         queryset=IPFabricSnapshot.objects.filter(status="loaded"),
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/jobs.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import timedelta
 
 from core.choices import DataSourceStatusChoices
 from core.choices import JobStatusChoices
 from core.exceptions import SyncError
 from core.models import Job
 from rq.timeouts import JobTimeoutException
-from utilities.utils import local_now
+from utilities.datetime import local_now
 
 from .models import IPFabricBranch
 from .models import IPFabricSource
 from .models import IPFabricSync
 
 logger = logging.getLogger(__name__)
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/migrations/0001_initial.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/migrations/0003_ipfabricsource_type_and_more.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/migrations/0003_ipfabricsource_type_and_more.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/models.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from core.choices import DataSourceStatusChoices
 from core.exceptions import SyncError
 from core.models import Job
 from core.signals import pre_sync
 from dcim.models import VirtualChassis
 from dcim.signals import assign_virtualchassis_master
 from django.apps import apps
-from django.contrib.auth.models import User
+from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.core.cache import cache
 from django.core.validators import MinValueValidator
 from django.db import models
 from django.db.models import Q
 from django.db.models import signals
 from django.urls import reverse
@@ -27,17 +27,17 @@
 from netbox.models import ChangeLoggedModel
 from netbox.models import NetBoxModel
 from netbox.models import PrimaryModel
 from netbox.models.features import JobsMixin
 from netbox.models.features import TagsMixin
 from netbox.registry import registry
 from netbox.staging import checkout
+from utilities.data import shallow_compare_dict
 from utilities.querysets import RestrictedQuerySet
-from utilities.utils import serialize_object
-from utilities.utils import shallow_compare_dict
+from utilities.serialization import serialize_object
 
 from .choices import IPFabricRawDataTypeChoices
 from .choices import IPFabricSnapshotStatusModelChoices
 from .choices import IPFabricSourceTypeChoices
 from .choices import IPFabricSyncTypeChoices
 from .choices import IPFabricTransformMapSourceModelChoices
 from .utilities.ipfutils import IPFabric
@@ -573,15 +573,19 @@
     interval = models.PositiveIntegerField(
         blank=True,
         null=True,
         validators=(MinValueValidator(1),),
         help_text=_("Recurrence interval (in minutes)"),
     )
     user = models.ForeignKey(
-        to=User, on_delete=models.SET_NULL, related_name="+", blank=True, null=True
+        to=settings.AUTH_USER_MODEL,
+        on_delete=models.SET_NULL,
+        related_name="+",
+        blank=True,
+        null=True,
     )
 
     class Meta:
         ordering = ["pk"]
         verbose_name = "IP Fabric Sync"
 
     def __str__(self):
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/navigation.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/navigation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-from extras.plugins import PluginMenuButton
-from extras.plugins import PluginMenuItem
 from netbox.plugins import PluginMenu
-from utilities.choices import ButtonColorChoices
+from netbox.plugins import PluginMenuButton
+from netbox.plugins import PluginMenuItem
+
 
 sync_buttons = [
     PluginMenuButton(
         link="plugins:ipfabric_netbox:ipfabricsync_add",
         title="Add",
         icon_class="mdi mdi-plus-thick",
         permissions=["ipfabric_netbox.add_ipfabricsync"],
-        color=ButtonColorChoices.GREEN,
     )
 ]
 
 source_buttons = [
     PluginMenuButton(
         link="plugins:ipfabric_netbox:ipfabricsource_add",
         title="Add",
         icon_class="mdi mdi-plus-thick",
         permissions=["ipfabric_netbox.add_ipfabricsource"],
-        color=ButtonColorChoices.GREEN,
     )
 ]
 
 source = PluginMenuItem(
     link="plugins:ipfabric_netbox:ipfabricsource_list",
     link_text="Sources",
     buttons=source_buttons,
@@ -50,15 +48,14 @@
     permissions=["ipfabric_netbox.view_ipfabrictransformmap"],
     buttons=[
         PluginMenuButton(
             link="plugins:ipfabric_netbox:ipfabrictransformmap_add",
             title="Add",
             icon_class="mdi mdi-plus-thick",
             permissions=["ipfabric_netbox.add_ipfabrictransformmap"],
-            color=ButtonColorChoices.GREEN,
         )
     ],
 )
 menu = PluginMenu(
     label="IP Fabric",
     icon_class="mdi mdi-cloud-sync",
     groups=(("IP Fabric", (source, snapshot, ingestion, tm)),),
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/signals.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/signals.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,48 @@
 from typing import Optional
 
+from core.models import ObjectType
 from dcim.models import Device
 from dcim.models import Site
-from django.conf import settings
-from django.contrib.contenttypes.models import ContentType
 from extras.choices import CustomFieldTypeChoices
+from extras.choices import CustomFieldUIEditableChoices
+from extras.choices import CustomFieldUIVisibleChoices
 from extras.choices import CustomLinkButtonClassChoices
 from extras.models import CustomField
 from extras.models import CustomLink
-from packaging import version
 
 from .models import IPFabricBranch
 from .models import IPFabricSource
 
-NETBOX_CURRENT_VERSION = version.parse(settings.VERSION)
-
-if NETBOX_CURRENT_VERSION >= version.parse("3.7.0"):
-    from extras.choices import (
-        CustomFieldUIVisibleChoices as CustomFieldUIVisibleChoices,
-    )
-    from extras.choices import CustomFieldUIEditableChoices
-else:
-    from extras.choices import (
-        CustomFieldVisibilityChoices as CustomFieldUIVisibleChoices,
-    )
-
 
 def create_custom_field(
     field_name: str,
     label: str,
     models: list,
     object_type=None,
     cf_type: Optional[str] = "type_text",
     ui_visibility: Optional[str] = "VISIBILITY_READ_ONLY",
 ):
-    if NETBOX_CURRENT_VERSION >= version.parse("3.7.0"):
-        defaults = {
-            "label": label,
-            "object_type": (
-                ContentType.objects.get_for_model(object_type) if object_type else None
-            ),
-            "ui_visible": getattr(CustomFieldUIVisibleChoices, "ALWAYS"),
-            "ui_editable": getattr(CustomFieldUIEditableChoices, "NO"),
-        }
-    else:
-        defaults = {
-            "label": label,
-            "object_type": (
-                ContentType.objects.get_for_model(object_type) if object_type else None
-            ),
-            "ui_visibility": getattr(
-                CustomFieldUIVisibleChoices, "VISIBILITY_READ_ONLY"
-            ),
-        }
+    defaults = {
+        "label": label,
+        "related_object_type": ObjectType.objects.get_for_model(object_type)
+        if object_type
+        else None,
+        "ui_visible": getattr(CustomFieldUIVisibleChoices, "ALWAYS"),
+        "ui_editable": getattr(CustomFieldUIEditableChoices, "NO"),
+    }
 
     custom_field, _ = CustomField.objects.update_or_create(
         type=getattr(CustomFieldTypeChoices, cf_type.upper()),
         name=field_name,
         defaults=defaults,
     )
 
     for model in models:
-        custom_field.content_types.add(ContentType.objects.get_for_model(model))
+        custom_field.object_types.add(ObjectType.objects.get_for_model(model))
 
 
 def ipfabric_netbox_init():
     create_custom_field(
         "ipfabric_source",
         "IP Fabric Source",
         [Device, Site],
@@ -78,14 +55,14 @@
         [Device, Site],
         cf_type="type_object",
         object_type=IPFabricBranch,
     )
     cl, _ = CustomLink.objects.update_or_create(
         defaults={
             "link_text": "{% if object.custom_field_data.ipfabric_source is defined %}{% set SOURCE_ID = object.custom_field_data.ipfabric_source %}{% if SOURCE_ID %}IP Fabric{% endif %}{% endif %}",
-            "link_url": '{% if object.custom_field_data.ipfabric_source is defined %}{% set SOURCE_ID = object.custom_field_data.ipfabric_source %}{% if SOURCE_ID %}{% set BASE_URL = object.custom_fields.filter(object_type__model="ipfabricsource").first().object_type.model_class().objects.get(pk=SOURCE_ID).url %}{{ BASE_URL }}/inventory/devices?options={"filters":{"sn": ["like","{{ object.serial }}"]}}{% endif %}{%endif%}',
+            "link_url": '{% if object.custom_field_data.ipfabric_source is defined %}{% set SOURCE_ID = object.custom_field_data.ipfabric_source %}{% if SOURCE_ID %}{% set BASE_URL = object.custom_fields.filter(related_object_type__model="ipfabricsource").first().related_object_type.model_class().objects.get(pk=SOURCE_ID).url %}{{ BASE_URL }}/inventory/devices?options={"filters":{"sn": ["like","{{ object.serial }}"]}}{% endif %}{%endif%}',
             "new_window": True,
             "button_class": CustomLinkButtonClassChoices.BLUE,
         },
         name="ipfabric",
     )
-    cl.content_types.add(ContentType.objects.get_for_model(Device))
+    cl.object_types.add(ObjectType.objects.get_for_model(Device))
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/tables.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/tables.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     class Meta(NetBoxTable.Meta):
         model = IPFabricSync
         fields = ("id", "status", "snapshot_name")
         default_columns = ("id", "status", "snapshot_name")
 
 
 class StagedChangesTable(NetBoxTable):
-    id = tables.Column()
+    pk = None
     object_type = tables.Column(
         accessor="object_type.model", verbose_name="Object Type"
     )
     name = tables.Column(accessor="object_type.name", verbose_name="Name")
     actions = columns.TemplateColumn(template_code=DIFF_BUTTON)
 
     def render_name(self, value, record):
@@ -177,15 +177,15 @@
         else:
             name = record.object.__str__()
         return name
 
     class Meta(NetBoxTable.Meta):
         model = StagedChange
         name = "staged_changes"
-        fields = ("id", "name", "action", "object_type", "actions")
+        fields = ("name", "action", "object_type", "actions")
         default_columns = ("name", "action", "object_type", "actions")
 
 
 class DeviceIPFTable(tables.Table):
     hostname = Column()
 
     class Meta:
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/diff.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/diff.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/json.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/json.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/merge_form.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/merge_form.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_button.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_button.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_modal.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_modal.html`

 * *Files 8% similar despite different names*

```diff
@@ -5,33 +5,33 @@
     {% if svg %}
         <div class=" d-flex flex-row flex-grow-1 align-items-center">
             {{svg|safe}}
         </div>
         <div>
             <div class="position-absolute top-0 end-0 m-2 border rounded p-2">
                 <ul class="list-unstyled">
-                    <li><span>Fetched: {{ time|annotated_date }}</span></li>
+                    <li><span>Fetched: {{ time|isodatetime }}</span></li>
                     <li>Snapshot Name: {{ snapshot.name }}</li>
                     <li>Snapshot ID: {{ snapshot.snapshot_id }}</li>
-                    <li>Snapshot Date: {{ snapshot.end|annotated_date }}</li>
+                    <li>Snapshot Date: {{ snapshot.end|isodatetime }}</li>
                 </ul>
             </div>
         </div>
     {% else %}
         <div class="d-flex flex-row flex-grow-1 align-items-center">
             {{ error }}
         </div>
         {% if snapshot %}
         <div>
             <div class="border rounded p-2">
                 <ul class="list-unstyled">
-                    <li><span>Fetched: {{ time|annotated_date }}</span></li>
+                    <li><span>Fetched: {{ time|isodatetime }}</span></li>
                     <li>Snapshot Name: {{ snapshot.name }}</li>
                     <li>Snapshot ID: {{ snapshot.snapshot_id }}</li>
-                    <li>Snapshot Date: {{ snapshot.end|annotated_date }}</li>
+                    <li>Snapshot Date: {{ snapshot.end|isodatetime }}</li>
                 </ul>
             </div>
         </div>
         {% endif %}
     {% endif %}
 </div>
 </div>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
 {% load helpers %}
 > {% if svg %}
 {{svg|safe}}
-    * Fetched: {{ time|annotated_date }}
+    * Fetched: {{ time|isodatetime }}
     * Snapshot Name: {{ snapshot.name }}
     * Snapshot ID: {{ snapshot.snapshot_id }}
-    * Snapshot Date: {{ snapshot.end|annotated_date }}
+    * Snapshot Date: {{ snapshot.end|isodatetime }}
 {% else %}
 {{ error }}
 {% if snapshot %}
-    * Fetched: {{ time|annotated_date }}
+    * Fetched: {{ time|isodatetime }}
     * Snapshot Name: {{ snapshot.name }}
     * Snapshot ID: {{ snapshot.snapshot_id }}
-    * Snapshot Date: {{ snapshot.end|annotated_date }}
+    * Snapshot Date: {{ snapshot.end|isodatetime }}
 {% endif %} {% endif %}
 {% if link %}
 _R_e_f_r_e_s_h _O_p_e_n_ _i_n_ _I_P_ _F_a_b_r_i_c
 {% endif %}
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/snapshotdata.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/snapshotdata.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/sync_delete.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/inc/sync_delete.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabric_table.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/ipfabric_table.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabricbranch.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/ipfabricbranch.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,186 +1,141 @@
-{% extends 'base/layout.html' %}
+{% extends 'generic/object.html' %}
 {% load buttons %}
 {% load custom_links %}
 {% load helpers %}
 {% load perms %}
 {% load plugins %}
 {% load tabs %}
 
-{% block header %}
-<div class="d-flex justify-content-between align-items-center">
-  {# Breadcrumbs #}
-  <nav class="breadcrumb-container px-3" aria-label="breadcrumb">
-    <ol class="breadcrumb">
-      {% block breadcrumbs %}
-      <li class="breadcrumb-item"><a href="{% url object|viewname:'list' %}">{{ object|meta:'verbose_name_plural'|bettertitle }}</a></li>
-      {% endblock breadcrumbs %}
-    </ol>
-  </nav>
-  {# Object identifier #}
-  <div class="float-end px-3">
-    <code class="text-muted">
-          {% block object_identifier %}
-            {{ object|meta:"app_label" }}.{{ object|meta:"model_name" }}:{{ object.pk }}
-            {% if object.slug %}({{ object.slug }}){% endif %}
-          {% endblock object_identifier %}
-        </code>
-  </div>
-</div>
-{{ block.super }}
-{% endblock %}
-
 {% block title %}{{ object }}{% endblock %}
 
-{% block subtitle %}
-<div class="object-subtitle">
-  <span>Created {{ object.created|annotated_date }}</span>
-  <span class="separator">&middot;</span>
-  <span>Updated <span title="{{ object.last_updated }}">{{ object.last_updated|timesince }}</span> ago</span>
-</div>
-{% endblock %}
-
-{% block controls %}
+{% block control-buttons %}
 {# Clone/Edit/Delete Buttons #}
 <div class="controls">
   <div class="control-group">
     {% custom_links object %}
   </div>
 {% if perms.core.sync_datasource %}
 {% if object.sync.ready_for_sync %}
   <a href="#"
   hx-get="{% url 'plugins:ipfabric_netbox:ipfabricbranch_merge' pk=object.pk %}"
   hx-target="#htmx-modal-content"
-  class="btn btn-sm btn-success"
+  class="btn btn-success"
   data-bs-toggle="modal"
   data-bs-target="#htmx-modal" disabled
   >
   <span class="mdi mdi-sync" aria-hidden="true"></span>&nbsp;Merge
   </a>
 {% else %}
 <span class="inline-block" tabindex="0" data-bs-toggle="tooltip" data-bs-delay="100" data-bs-placement="bottom">
-  <button class="btn btn-sm btn-success" disabled>
+  <button class="btn btn-success" disabled>
     <i class="mdi mdi-sync" aria-hidden="true"></i> Merge
   </button>
 </span>
 {% endif %}
 {% endif %}
 </div>
-{% endblock controls %}
+{% endblock control-buttons %}
 
-{% block tabs %}
-<ul class="nav nav-tabs px-3">
-  {# Primary tab #}
-  <li class="nav-item" role="presentation">
-    <a class="nav-link{% if not tab %} active{% endif %}" href="{{ object.get_absolute_url }}">{{ object|meta:"verbose_name"|bettertitle }}</a>
-  </li>
-  {# Include tabs for registered model views #}
-  {% model_view_tabs object %}
-</ul>
-{% endblock tabs %}
 
-{% block content-wrapper %}
-<div class="tab-content">
-  {% block content %}
-  <div class="row mb-3">
-    <div class="col col-md-6">
-      <div class="card">
-        <h5 class="card-header">Branch Information</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Name</th>
-              <td>{{ object.name }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Description</th>
-              <td>{{ object.description|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Sync Object</th>
-              <td><a href="{% url 'plugins:ipfabric_netbox:ipfabricsync' pk=object.sync.pk %}">{{ object.sync.name}}</a>
-              </td>
-            </tr>
-            <tr>
-              <th scope="row">Job Object</th>
-              <td><a href="{% url 'core:job' pk=object.job.pk %}">{{ object.job }}</a></td>
-            </tr>
-            <tr>
-              <th scope="row">Sync Status</th>
-                <td><div id="sync_status" hx-swap-oob="true">{% include 'ipfabric_netbox/partials/branch_status.html' with object=object %}</div></td>
-                <!-- <td >{% badge object.sync.get_status_display bg_color=object.sync.get_status_color %}</td> -->
-              </div>
-            </tr>
-            <tr>
-              <th scope="row">Snapshot</th>
-              <td><a
-                  href="{% url 'plugins:ipfabric_netbox:ipfabricsnapshot' pk=object.sync.snapshot_data.pk %}">{{object.sync.snapshot_data.name }}</a></td>
-            </tr>
-            <tr>
-              <th scope="row">Source</th>
-              <td><a
-                  href="{% url 'plugins:ipfabric_netbox:ipfabricsource' pk=object.sync.snapshot_data.source.pk %}">{{object.sync.snapshot_data.source.name }}</a></td>
-            </tr>
-          </table>
-        </div>
+{% block content %}
+<div class="row mb-3">
+  <div class="col col-md-6">
+    <div class="card">
+      <h5 class="card-header">Branch Information</h5>
+      <div class="card-body">
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Name</th>
+            <td>{{ object.name }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Description</th>
+            <td>{{ object.description|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Sync Object</th>
+            <td><a href="{% url 'plugins:ipfabric_netbox:ipfabricsync' pk=object.sync.pk %}">{{ object.sync.name}}</a>
+            </td>
+          </tr>
+          <tr>
+            <th scope="row">Job Object</th>
+            <td><a href="{% url 'core:job' pk=object.job.pk %}">{{ object.job }}</a></td>
+          </tr>
+          <tr>
+            <th scope="row">Sync Status</th>
+              <td><div id="sync_status" hx-swap-oob="true">{% include 'ipfabric_netbox/partials/branch_status.html' with object=object %}</div></td>
+              <!-- <td >{% badge object.sync.get_status_display bg_color=object.sync.get_status_color %}</td> -->
+            </div>
+          </tr>
+          <tr>
+            <th scope="row">Snapshot</th>
+            <td><a
+                href="{% url 'plugins:ipfabric_netbox:ipfabricsnapshot' pk=object.sync.snapshot_data.pk %}">{{object.sync.snapshot_data.name }}</a></td>
+          </tr>
+          <tr>
+            <th scope="row">Source</th>
+            <td><a
+                href="{% url 'plugins:ipfabric_netbox:ipfabricsource' pk=object.sync.snapshot_data.source.pk %}">{{object.sync.snapshot_data.source.name }}</a></td>
+          </tr>
+        </table>
       </div>
-      {% plugin_left_page object %}
     </div>
-    <div class="col col-md-6">
-      <div class="card">
-        <h5 class="card-header">Statistics</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Created</th>
-              <td>
-                {% if object.num_created %}
-                {{ object.num_created }}
-                {% else %}
-                {{ ''|placeholder }}
-                {% endif %}
-              </td>
-            </tr>
-            <tr>
-              <th scope="row">Updated</th>
-              <td>
-                {% if object.num_updated %}
-                {{ object.num_updated }}
-                {% else %}
-                {{ ''|placeholder }}
-                {% endif %}
-              </td>
-            </tr>
-            <tr>
-              <th scope="row">Deleted</th>
-              <td>
-                {% if object.num_deleted %}
-                {{ object.num_deleted }}
-                {% else %}
-                {{ ''|placeholder }}
-                {% endif %}
-              </td>
-            </tr>
-          </table>
-        </div>
-      </div>
-      <div id="sync_progress">
-        {% include 'ipfabric_netbox/partials/branch_progress.html' %}
+    {% plugin_left_page object %}
+  </div>
+  <div class="col col-md-6">
+    <div class="card">
+      <h5 class="card-header">Statistics</h5>
+      <div class="card-body">
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Created</th>
+            <td>
+              {% if object.num_created %}
+              {{ object.num_created }}
+              {% else %}
+              {{ ''|placeholder }}
+              {% endif %}
+            </td>
+          </tr>
+          <tr>
+            <th scope="row">Updated</th>
+            <td>
+              {% if object.num_updated %}
+              {{ object.num_updated }}
+              {% else %}
+              {{ ''|placeholder }}
+              {% endif %}
+            </td>
+          </tr>
+          <tr>
+            <th scope="row">Deleted</th>
+            <td>
+              {% if object.num_deleted %}
+              {{ object.num_deleted }}
+              {% else %}
+              {{ ''|placeholder }}
+              {% endif %}
+            </td>
+          </tr>
+        </table>
       </div>
-      <!-- {% include 'inc/panels/related_objects.html' %} -->
-      {% include 'inc/panels/custom_fields.html' %}
-      {% plugin_right_page object %}
     </div>
-  </div>
-  <div class="row mb-3">
-    <div class="col col-md-12" {% if not object.job.completed %} hx-get="{% url 'plugins:ipfabric_netbox:ipfabricbranch_logs' pk=object.pk %}?type=info"
-      hx-trigger="every 5s" hx-target="#sync_logs" hx-select="#sync_logs" hx-select-oob="#sync_status:innerHTML"
-      hx-swap="innerHTML" {% endif %}>
-      <div id="sync_logs">{% include 'ipfabric_netbox/partials/job_logs.html' with job=object.job %}</div>
+    <div id="sync_progress">
+      {% include 'ipfabric_netbox/partials/branch_progress.html' %}
     </div>
-    {% endblock content %}
+    <!-- {% include 'inc/panels/related_objects.html' %} -->
+    {% include 'inc/panels/custom_fields.html' %}
+    {% plugin_right_page object %}
+  </div>
+</div>
+<div class="row mb-3">
+  <div class="col col-md-12" {% if not object.job.completed %} hx-get="{% url 'plugins:ipfabric_netbox:ipfabricbranch_logs' pk=object.pk %}?type=info"
+    hx-trigger="every 5s" hx-target="#sync_logs" hx-select="#sync_logs" hx-select-oob="#sync_status:innerHTML"
+    hx-swap="innerHTML" {% endif %}>
+    <div id="sync_logs">{% include 'ipfabric_netbox/partials/job_logs.html' with job=object.job %}</div>
   </div>
-  {% endblock content-wrapper %}
+{% endblock content %}
 
   {% block modals %}
   {% include 'inc/htmx_modal.html' with size='lg' %}
   {% endblock modals %}
```

#### html2text {}

```diff
@@ -1,33 +1,15 @@
-{% extends 'base/layout.html' %} {% load buttons %} {% load custom_links %} {%
-load helpers %} {% load perms %} {% load plugins %} {% load tabs %} {% block
-header %}
-{# Breadcrumbs #}
-   1. {% block breadcrumbs %}
-   2. _{_{_ _o_b_j_e_c_t_|_m_e_t_a_:_'_v_e_r_b_o_s_e___n_a_m_e___p_l_u_r_a_l_'_|_b_e_t_t_e_r_t_i_t_l_e_ _}_}
-   3. {% endblock breadcrumbs %}
-{# Object identifier #}
-{% block object_identifier %} {{ object|meta:"app_label" }}.{{ object|meta:
-"model_name" }}:{{ object.pk }} {% if object.slug %}({{ object.slug }}){% endif
-%} {% endblock object_identifier %}
-{{ block.super }} {% endblock %} {% block title %}{{ object }}{% endblock %} {%
-block subtitle %}
-Created {{ object.created|annotated_date }} · Updated {
-{ object.last_updated|timesince }} ago
-{% endblock %} {% block controls %} {# Clone/Edit/Delete Buttons #}
+{% extends 'generic/object.html' %} {% load buttons %} {% load custom_links %}
+{% load helpers %} {% load perms %} {% load plugins %} {% load tabs %} {% block
+title %}{{ object }}{% endblock %} {% block control-buttons %} {# Clone/Edit/
+Delete Buttons #}
 {% custom_links object %}
 {% if perms.core.sync_datasource %} {% if object.sync.ready_for_sync %} _ _M_e_r_g_e_ 
 {% else %} Merge {% endif %} {% endif %}
-{% endblock controls %} {% block tabs %}
-    * {# Primary tab #}
-    * _{_{_ _o_b_j_e_c_t_|_m_e_t_a_:_"_v_e_r_b_o_s_e___n_a_m_e_"_|_b_e_t_t_e_r_t_i_t_l_e_ _}_}
-    * {# Include tabs for registered model views #} {% model_view_tabs object
-      %}
-{% endblock tabs %} {% block content-wrapper %}
-{% block content %}
+{% endblock control-buttons %} {% block content %}
 **** BBrraanncchh IInnffoorrmmaattiioonn ****
 NNaammee        {{ object.name }}
 DDeessccrriippttiioonn {{ object.description|placeholder }}
 SSyynncc OObbjjeecctt _{_{_ _o_b_j_e_c_t_._s_y_n_c_._n_a_m_e_}_}
 JJoobb OObbjjeecctt  _{_{_ _o_b_j_e_c_t_._j_o_b_ _}_}
 SSyynncc SSttaattuuss {% include 'ipfabric_netbox/partials/branch_status.html' with
             object=object %}
@@ -44,10 +26,9 @@
 {% include 'ipfabric_netbox/partials/branch_progress.html' %}
 {% include 'inc/panels/custom_fields.html' %} {% plugin_right_page object %}
 % if not object.job.completed %} hx-get="{% url 'plugins:ipfabric_netbox:
 ipfabricbranch_logs' pk=object.pk %}?type=info" hx-trigger="every 5s" hx-
 target="#sync_logs" hx-select="#sync_logs" hx-select-oob="#sync_status:
 innerHTML" hx-swap="innerHTML" {% endif %}>
 {% include 'ipfabric_netbox/partials/job_logs.html' with job=object.job %}
-{% endblock content %}
-{% endblock content-wrapper %} {% block modals %} {% include 'inc/
-htmx_modal.html' with size='lg' %} {% endblock modals %}
+{% endblock content %} {% block modals %} {% include 'inc/htmx_modal.html' with
+size='lg' %} {% endblock modals %}
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsnapshot.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsnapshot.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsource.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsource.html`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 {% load perms %}
 
 {% block extra_controls %}
 {% if perms.ipfabric_netbox.sync_source %}
 {% if object.ready_for_sync and object.type == 'local' %}
 <form action="{% url 'plugins:ipfabric_netbox:ipfabricsource_sync' pk=object.pk %}" method="post">
   {% csrf_token %}
-  <button type="submit" class="btn btn-sm btn-primary">
+  <button type="submit" class="btn btn-primary">
     <i class="mdi mdi-sync" aria-hidden="true"></i> Sync
   </button>
 </form>
 {% else %}
 <span class="inline-block" tabindex="0" data-bs-toggle="tooltip" data-bs-delay="100" data-bs-placement="bottom">
-  <button class="btn btn-sm btn-primary" disabled>
+  <button class="btn btn-primary" disabled>
     <i class="mdi mdi-sync" aria-hidden="true"></i> Sync
   </button>
 </span>
 {% endif %}
 {% endif %}
 {% endblock %}
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsync.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsync.html`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 {% load render_table from django_tables2 %}
 
 {% block extra_controls %}
   {% if perms.ipfabric_netbox.sync_ingest %}
     {% if object.ready_for_sync %}
       <form action="{% url 'plugins:ipfabric_netbox:ipfabricsync_sync' pk=object.pk %}" method="post">
         {% csrf_token %}
-        <button type="submit" class="btn btn-sm btn-primary">
+        <button type="submit" class="btn btn-primary">
           <i class="mdi mdi-sync" aria-hidden="true"></i> Adhoc Ingestion
         </button>
       </form>
     {% else %}
       <span class="inline-block" tabindex="0" data-bs-toggle="tooltip" data-bs-delay="100" data-bs-placement="bottom">
-        <button class="btn btn-sm btn-primary" disabled>
+        <button class="btn btn-primary" disabled>
           <i class="mdi mdi-sync" aria-hidden="true"></i> Adhoc Ingestion
         </button>
       </span>
     {% endif %}
   {% endif %}
 {% endblock %}
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_restore.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_restore.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_progress.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_progress.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/partials/job_logs.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/partials/job_logs.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 {% load humanize %}
 {% load helpers %}
 
 <p>
 {% if job.started %}
-Started: <strong>{{ job.started|annotated_date }}</strong>
+Started: <strong>{{ job.started|isodatetime }}</strong>
 {% elif job.scheduled %}
-Scheduled for: <strong>{{ job.scheduled|annotated_date }}</strong> ({{ job.scheduled|naturaltime }})
+Scheduled for: <strong>{{ job.scheduled|isodatetime }}</strong> ({{ job.scheduled|naturaltime }})
 {% else %}
-Created: <strong>{{ job.created|annotated_date }}</strong>
+Created: <strong>{{ job.created|isodatetime }}</strong>
 {% endif %}
 {% if job.completed %}
 Duration: <strong>{{ job.duration }}</strong>
 {% endif %}
 <span id="pending-result-label">{% badge job.get_status_display job.get_status_color %}</span>
 </p>
 {% if not job.completed %}
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
 {% load humanize %} {% load helpers %}
-{% if job.started %} Started: {{{{ jjoobb..ssttaarrtteedd||aannnnoottaatteedd__ddaattee }}}} {% elif
-job.scheduled %} Scheduled for: {{{{ jjoobb..sscchheedduulleedd||aannnnoottaatteedd__ddaattee }}}} ({
-{ job.scheduled|naturaltime }}) {% else %} Created: {{
-{{ jjoobb..ccrreeaatteedd||aannnnoottaatteedd__ddaattee }}}} {% endif %} {% if job.completed %} Duration: {{
-{{ jjoobb..dduurraattiioonn }}}} {% endif %} {% badge job.get_status_display
-job.get_status_color %}
+{% if job.started %} Started: {{{{ jjoobb..ssttaarrtteedd||iissooddaatteettiimmee }}}} {% elif
+job.scheduled %} Scheduled for: {{{{ jjoobb..sscchheedduulleedd||iissooddaatteettiimmee }}}} ({
+{ job.scheduled|naturaltime }}) {% else %} Created: {{{{ jjoobb..ccrreeaatteedd||iissooddaatteettiimmee
+}}}} {% endif %} {% if job.completed %} Duration: {{{{ jjoobb..dduurraattiioonn }}}} {% endif %}
+{% badge job.get_status_display job.get_status_color %}
 {% if not job.completed %} {% include 'ipfabric_netbox/inc/logs_pending.html'
 %} {% endif %}
 **** SSyynncc RReessuullttss ****
 TTiimmee       LLeevveell             OObbjjeecctt                      MMeessssaaggee
                              {% if obj and url %} _{_{_ _o_b_j
                              _}_} {% elif obj %} {{ obj }}
 {{ time }} {{ level|title }} {% else %} {                {{ message|markdown }}
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/sync_list.html` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/templates/ipfabric_netbox/sync_list.html`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     <div class="control-group">
       {% block extra_controls %}{% endblock %}
       {% add_button model %}
     </div>
   </div>
 {% endblock controls %}
 
-{% block content-wrapper %}
+{% block content %}
   <div class="tab-content">
     {% for sync in syncs %}
       <div class="card">
         <h5 class="card-header" id="module{{ module.pk }}">
           <!-- TODO: Cannot delete without serializer https://github.com/netbox-community/netbox/issues/13640-->
           <!-- {% if perms.ipfabric_netbox.delete_ipfabricsync %}
             <div class="float-end">
@@ -64,15 +64,15 @@
                     <tr>
                       <td>
                         <a href="{% url 'extras:report' module=module.python_name name=report.class_name %}" id="{{ report.module }}.{{ report.class_name }}">{{ report.name }}</a>
                       </td>
                       <td>{{ report.description|markdown|placeholder }}</td>
                       {% if last_job %}
                         <td>
-                          <a href="{% url 'extras:report_result' job_pk=last_job.pk %}">{{ last_job.created|annotated_date }}</a>
+                          <a href="{% url 'extras:report_result' job_pk=last_job.pk %}">{{ last_job.created|isodatetime }}</a>
                         </td>
                         <td>
                           {% badge last_job.get_status_display last_job.get_status_color %}
                         </td>
                       {% else %}
                         <td class="text-muted">Never</td>
                         <td>{{ ''|placeholder }}</td>
@@ -119,8 +119,8 @@
         <h4 class="alert-heading">Injest Jobs Settings Found</h4>
         {% if perms.extras.add_reportmodule %}
           Get started by <a href="{% url 'plugins:ipfabric_netbox:ipfabricsync_add' %}">creating an injestion</a> from an IP Fabric source.
         {% endif %}
       </div>
     {% endfor %}
   </div>
-{% endblock content-wrapper %}
+{% endblock content %}
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
 {% extends 'base/layout.html' %} {% load buttons %} {% load helpers %} {% load
 perms %} {% block title %}Ingestion{% endblock %} {% block tabs %}
     * Ingestion
 {% endblock tabs %} {% block controls %}
 {% block extra_controls %}{% endblock %} {% add_button model %}
-{% endblock controls %} {% block content-wrapper %}
+{% endblock controls %} {% block content %}
 {% for sync in syncs %}
 _{{_{{_ _ss_yy_nn_cc_.._nn_aa_mm_ee_}}_}}
 {% include 'inc/sync_warning.html' with object=module %}
 SSoouurrccee                         SSnnaappsshhoott                  SSttaattuuss                    LLaasstt RRuunn
 _{                              _{                         {% badge
 _{                              _{                         sync.get_status_display   {
 _s_y_n_c_._s_n_a_p_s_h_o_t___d_a_t_a_._s_o_u_r_c_e_._n_a_m_e _s_y_n_c_._s_n_a_p_s_h_o_t___d_a_t_a_._n_a_m_e_}_} last_job.get_status_color {sync.last_synced}}
 _}_}                                                       %}
 {% empty %}
 ****** IInnjjeesstt JJoobbss SSeettttiinnggss FFoouunndd ******
 {% if perms.extras.add_reportmodule %} Get started by _c_r_e_a_t_i_n_g_ _a_n_ _i_n_j_e_s_t_i_o_n
 from an IP Fabric source. {% endif %}
 {% endfor %}
-{% endblock content-wrapper %}
+{% endblock content %}
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/tests/test_models.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/urls.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/urls.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/ipfutils.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/utilities/ipfutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 import uuid
+from importlib import metadata
 
 from core.exceptions import SyncError
 from dcim.models import Device
 from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist
 from django.shortcuts import get_object_or_404
 from django.utils.text import slugify
 from django_tables2 import Column
 from ipfabric import IPFClient
-from importlib import metadata
 from jinja2.sandbox import SandboxedEnvironment
 from netbox.config import get_config
 from netutils.utils import jinja2_convenience_function
 
 from ..choices import IPFabricSourceTypeChoices
 from .nbutils import device_serial_max_length
 from .nbutils import order_devices
@@ -52,15 +52,17 @@
     def __init__(self, parameters=None, transform_map=None) -> None:
         if parameters:
             self.ipf = IPFClient(**parameters, unloaded=True)
         else:
             self.ipf = IPFClient(
                 **settings.PLUGINS_CONFIG["ipfabric_netbox"], unloaded=True
             )
-        self.ipf._client.headers['user-agent'] += f'; ipfabric-netbox/{metadata.version("ipfabric-netbox")}'
+        self.ipf._client.headers[
+            "user-agent"
+        ] += f'; ipfabric-netbox/{metadata.version("ipfabric-netbox")}'
         self.transform_map = transform_map
 
     def get_snapshots(self) -> dict:
         formatted_snapshots = {}
         if self.ipf:
             for snapshot_ref, snapshot in self.ipf.snapshots.items():
                 if snapshot.status != "done" and snapshot.finish_status != "done":
@@ -294,18 +296,18 @@
                     snapshot_id=self.settings["snapshot_id"]
                 )
 
                 data["device"] = self.client.inventory.devices.all(
                     snapshot_id=self.settings["snapshot_id"], filters=filter
                 )
 
-                data["virtualchassis"] = (
-                    self.client.technology.platforms.stacks_members.all(
-                        snapshot_id=self.settings["snapshot_id"], filters=site_filter
-                    )
+                data[
+                    "virtualchassis"
+                ] = self.client.technology.platforms.stacks_members.all(
+                    snapshot_id=self.settings["snapshot_id"], filters=site_filter
                 )
 
                 data["interface"] = self.client.inventory.interfaces.all(
                     snapshot_id=self.settings["snapshot_id"]
                 )
 
                 data["inventoryitem"] = self.client.inventory.pn.all(
@@ -330,18 +332,18 @@
                 else:
                     networks_filter = {"and": [{"net": ["empty", False]}]}
                 self.logger.log_info(f"Creating network filter: `{networks_filter}`")
                 data["prefix"] = self.client.technology.managed_networks.networks.all(
                     snapshot_id=self.settings["snapshot_id"], filters=networks_filter
                 )
 
-                data["ipaddress"] = (
-                    self.client.technology.addressing.managed_ip_ipv4.all(
-                        snapshot_id=self.settings["snapshot_id"]
-                    )
+                data[
+                    "ipaddress"
+                ] = self.client.technology.addressing.managed_ip_ipv4.all(
+                    snapshot_id=self.settings["snapshot_id"]
                 )
         except Exception as e:
             self.logger.log_failure(
                 f"Error collecting data from IP Fabric: {e}", obj=self.sync
             )
             raise SyncError(f"Error collecting data from IP Fabric: {e}")
 
@@ -469,21 +471,21 @@
 
             self.get_model_or_update("dcim", "devicerole", device, uuid=device_uuid)
 
             device_object = self.get_model_or_update(
                 "dcim", "device", device, uuid=device_uuid
             )
 
-            site_object.custom_field_data["ipfabric_source"] = (
-                self.sync.snapshot_data.source.pk
-            )
-
-            device_object.custom_field_data["ipfabric_source"] = (
-                self.sync.snapshot_data.source.pk
-            )
+            site_object.custom_field_data[
+                "ipfabric_source"
+            ] = self.sync.snapshot_data.source.pk
+
+            device_object.custom_field_data[
+                "ipfabric_source"
+            ] = self.sync.snapshot_data.source.pk
             if branch:
                 site_object.custom_field_data["ipfabric_branch"] = branch.pk
                 device_object.custom_field_data["ipfabric_branch"] = branch.pk
 
             site_object.save()
             device_object.save()
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/logging.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/nbutils.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/utilities/nbutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,17 +32,17 @@
     for device in devices:
         if counter[device["hostname"]] > 1:
             device["hostname"] = f"{device['hostname']} - ({device['sn']})"
         if child_members := members.get(device.get("sn")):
             for child_member in child_members:
                 if device.get("sn") != child_member.get("memberSn"):
                     new_device = deepcopy(device)
-                    new_device["hostname"] = (
-                        f"{device['hostname']}/{child_member.get('member')}"
-                    )
+                    new_device[
+                        "hostname"
+                    ] = f"{device['hostname']}/{child_member.get('member')}"
                     new_device["model"] = child_member.get("pn")
                     new_device["sn"] = child_member.get("memberSn")
                     new_device["virtual_chassis"] = child_member
                     new_devices.append(new_device)
                 else:
                     device["virtual_chassis"] = child_member
             hostnames = [d["hostname"] for d in devices]
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/transform_map.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/utilities/transform_map.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox/views.py` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,21 @@
 from django_tables2 import RequestConfig
 from extras.choices import ChangeActionChoices
 from ipfabric.diagrams import Network
 from ipfabric.diagrams import NetworkSettings
 from netbox.staging import StagedChange
 from netbox.views import generic
 from netbox.views.generic.base import BaseObjectView
+from utilities.data import shallow_compare_dict
 from utilities.forms import ConfirmationForm
-from utilities.htmx import is_htmx
 from utilities.paginator import EnhancedPaginator
 from utilities.paginator import get_paginate_count
-from utilities.utils import count_related
-from utilities.utils import get_viewname
-from utilities.utils import serialize_object
-from utilities.utils import shallow_compare_dict
+from utilities.query import count_related
+from utilities.serialization import serialize_object
+from utilities.views import get_viewname
 from utilities.views import register_model_view
 from utilities.views import ViewTab
 
 from .filtersets import IPFabricBranchFilterSet
 from .filtersets import IPFabricDataFilterSet
 from .filtersets import IPFabricSnapshotFilterSet
 from .filtersets import IPFabricSourceFilterSet
@@ -115,15 +114,15 @@
     queryset = IPFabricTransformMap.objects.all()
     table = IPFabricTransformMapTable
 
     def get_required_permission(self):
         return "ipfabric_netbox.tm_restore"
 
     def get(self, request):
-        if is_htmx(request):
+        if request.htmx:
             viewname = get_viewname(self.queryset.model, action="restore")
             form_url = reverse(viewname)
             form = ConfirmationForm(initial=request.GET)
             dependent_objects = {
                 IPFabricTransformMap: IPFabricTransformMap.objects.all(),
                 IPFabricTransformField: IPFabricTransformField.objects.all(),
                 IPFabricRelationshipField: IPFabricRelationshipField.objects.all(),
@@ -270,15 +269,15 @@
 class IPFabricSnapshotDataJSONView(LoginRequiredMixin, View):
     template_name = "ipfabric_netbox/inc/json.html"
 
     def get(self, request, **kwargs):
         print(kwargs)
         # change_id = kwargs.get("change_pk", None)
 
-        if is_htmx(request):
+        if request.htmx:
             data = get_object_or_404(IPFabricData, pk=kwargs.get("pk"))
             return render(
                 request,
                 self.template_name,
                 {
                     "object": data,
                 },
@@ -395,15 +394,15 @@
     queryset = IPFabricSync.objects.all()
     actions = ("edit",)
 
     def get(self, request, **kwargs):
         instance = self.get_object(**kwargs)
         last_branch = instance.ipfabricbranch_set.last()
 
-        if is_htmx(request):
+        if request.htmx:
             response = render(
                 request,
                 "ipfabric_netbox/partials/sync_last_branch.html",
                 {"last_branch": last_branch},
             )
 
             if instance.status not in ["queued", "syncing"]:
@@ -445,15 +444,15 @@
 class IPFabricSyncDeleteView(generic.ObjectDeleteView):
     queryset = IPFabricSync.objects.all()
     default_return_url = "plugins:ipfabric_netbox:ipfabricsync_list"
 
     def get(self, request, pk):
         obj = get_object_or_404(self.queryset, pk=pk)
 
-        if is_htmx(request):
+        if request.htmx:
             viewname = get_viewname(self.queryset.model, action="delete")
             form_url = reverse(viewname, kwargs={"pk": obj.pk})
             form = ConfirmationForm(initial=request.GET)
             return render(
                 request,
                 "ipfabric_netbox/inc/sync_delete.html",
                 {
@@ -510,15 +509,15 @@
     path="logs",
 )
 class IPFabricBranchLogView(LoginRequiredMixin, View):
     template_name = "ipfabric_netbox/partials/branch_all.html"
 
     def get(self, request, **kwargs):
         branch_id = kwargs.get("pk")
-        if is_htmx(request):
+        if request.htmx:
             branch = IPFabricBranch.objects.get(pk=branch_id)
             data = branch.get_statistics()
             data["object"] = branch
             data["job"] = branch.job
             response = render(
                 request,
                 self.template_name,
@@ -563,15 +562,15 @@
 
     def get_required_permission(self):
         return "ipfabric_netbox.merge_branch"
 
     def get(self, request, pk):
         obj = get_object_or_404(self.queryset, pk=pk)
 
-        if is_htmx(request):
+        if request.htmx:
             viewname = get_viewname(self.queryset.model, action="merge")
             form_url = reverse(viewname, kwargs={"pk": obj.pk})
             form = ConfirmationForm(initial=request.GET)
             return render(
                 request,
                 "ipfabric_netbox/inc/merge_form.html",
                 {
@@ -601,15 +600,15 @@
 )
 class IPFabricBranchChangesDiffView(LoginRequiredMixin, View):
     template_name = "ipfabric_netbox/inc/diff.html"
 
     def get(self, request, model, **kwargs):
         change_id = kwargs.get("change_pk", None)
 
-        if is_htmx(request):
+        if request.htmx:
             if change_id:
                 change = StagedChange.objects.get(pk=change_id)
                 if hasattr(change.object, "pk"):
                     prechange_data = serialize_object(change.object, resolve_tags=False)
                     prechange_data = dict(sorted(prechange_data.items()))
                 else:
                     prechange_data = None
@@ -745,15 +744,15 @@
             request,
             {
                 "paginator_class": EnhancedPaginator,
                 "per_page": get_paginate_count(request),
             },
         ).configure(table)
 
-        if is_htmx(request):
+        if request.htmx:
             return render(
                 request,
                 "htmx/table.html",
                 {
                     "table": table,
                 },
             )
@@ -782,16 +781,15 @@
     path="topology/<int:site>",
     kwargs={"snapshot": ""},
 )
 class IPFabricSourceTopology(LoginRequiredMixin, View):
     template_name = "ipfabric_netbox/inc/site_topology_modal.html"
 
     def get(self, request, pk, site, **kwargs):
-        if is_htmx(request):
-
+        if request.htmx:
             try:
                 site = get_object_or_404(Site, pk=site)
                 source_id = request.GET.get("source")
                 if not source_id:
                     raise Exception("Source ID not available in request.")
                 source = get_object_or_404(IPFabricSource, pk=source_id)
                 snapshot = request.GET.get("snapshot")
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/PKG-INFO` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfabric_netbox
-Version: 2.0.6
+Version: 3.0.0b0
 Summary: NetBox plugin to sync IP Fabric data into NetBox
 Home-page: https://gitlab.com/ip-fabric/integrations/ipfabric-netbox-sync
 Author: Solution Architecture
 Author-email: solution.architecture@ipfabric.io
 Project-URL: Bug Tracker, https://gitlab.com/ip-fabric/integrations/ipfabric-netbox-sync/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/SOURCES.txt` & `ipfabric_netbox-3.0.0b0/ipfabric_netbox.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 ipfabric_netbox/api/serializers.py
 ipfabric_netbox/api/urls.py
 ipfabric_netbox/api/views.py
 ipfabric_netbox/migrations/0001_initial.py
 ipfabric_netbox/migrations/0002_ipfabricsnapshot_status.py
 ipfabric_netbox/migrations/0003_ipfabricsource_type_and_more.py
 ipfabric_netbox/migrations/0004_ipfabricsync_auto_merge.py
+ipfabric_netbox/migrations/0005_alter_ipfabricrelationshipfield_source_model_and_more.py
 ipfabric_netbox/migrations/__init__.py
 ipfabric_netbox/templates/ipfabric_netbox/ipfabric_table.html
 ipfabric_netbox/templates/ipfabric_netbox/ipfabricbranch.html
 ipfabric_netbox/templates/ipfabric_netbox/ipfabricsnapshot.html
 ipfabric_netbox/templates/ipfabric_netbox/ipfabricsource.html
 ipfabric_netbox/templates/ipfabric_netbox/ipfabricsync.html
 ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap.html
```

### Comparing `ipfabric_netbox-2.0.6/setup.py` & `ipfabric_netbox-3.0.0b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ipfabric_netbox",
-    version="2.0.6",
+    version="3.0.0b0",
     author="Solution Architecture",
     author_email="solution.architecture@ipfabric.io",
     description="NetBox plugin to sync IP Fabric data into NetBox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["ipfabric>=6.6.4", "netutils"],
     url="https://gitlab.com/ip-fabric/integrations/ipfabric-netbox-sync",
```

