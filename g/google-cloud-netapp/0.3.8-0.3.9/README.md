# Comparing `tmp/google-cloud-netapp-0.3.8.tar.gz` & `tmp/google-cloud-netapp-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-netapp-0.3.8.tar", last modified: Thu Mar  7 18:10:03 2024, max compression
+gzip compressed data, was "google-cloud-netapp-0.3.9.tar", last modified: Fri Mar 22 12:19:42 2024, max compression
```

## Comparing `google-cloud-netapp-0.3.8.tar` & `google-cloud-netapp-0.3.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-07 18:10:03.979005 google-cloud-netapp-0.3.8/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5065 2024-03-07 18:10:03.979005 google-cloud-netapp-0.3.8/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3704 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-07 18:10:03.963004 google-cloud-netapp-0.3.8/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-07 18:10:03.963004 google-cloud-netapp-0.3.8/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-07 18:10:03.967005 google-cloud-netapp-0.3.8/google/cloud/netapp/
--rw-rw-r--   0 root         (0)     1003     6270 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-07 18:10:03.967005 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/
--rw-rw-r--   0 root         (0)     1003     5938 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    20077 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-07 18:10:03.967005 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-07 18:10:03.971005 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/
--rw-rw-r--   0 root         (0)     1003      737 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/__init__.py
--rw-rw-r--   0 root         (0)     1003   283639 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/async_client.py
--rw-rw-r--   0 root         (0)     1003   306005 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/client.py
--rw-rw-r--   0 root         (0)     1003    46079 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-07 18:10:03.971005 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/transports/
--rw-rw-r--   0 root         (0)     1003     1288 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    37254 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/transports/base.py
--rw-rw-r--   0 root         (0)     1003    75291 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    77048 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   290460 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-07 18:10:03.975005 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/
--rw-rw-r--   0 root         (0)     1003     5652 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    11218 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/active_directory.py
--rw-rw-r--   0 root         (0)     1003    11350 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/backup.py
--rw-rw-r--   0 root         (0)     1003     9958 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/backup_policy.py
--rw-rw-r--   0 root         (0)     1003     8142 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/backup_vault.py
--rw-rw-r--   0 root         (0)     1003     2851 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/cloud_netapp_service.py
--rw-rw-r--   0 root         (0)     1003     1824 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003    10331 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/kms.py
--rw-rw-r--   0 root         (0)     1003    19307 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/replication.py
--rw-rw-r--   0 root         (0)     1003     8125 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/snapshot.py
--rw-rw-r--   0 root         (0)     1003    10479 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/storage_pool.py
--rw-rw-r--   0 root         (0)     1003    32924 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/volume.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-07 18:10:03.975005 google-cloud-netapp-0.3.8/google_cloud_netapp.egg-info/
--rw-r--r--   0 root         (0)     1003     5065 2024-03-07 18:10:03.000000 google-cloud-netapp-0.3.8/google_cloud_netapp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1771 2024-03-07 18:10:03.000000 google-cloud-netapp-0.3.8/google_cloud_netapp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-07 18:10:03.000000 google-cloud-netapp-0.3.8/google_cloud_netapp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-07 18:10:03.000000 google-cloud-netapp-0.3.8/google_cloud_netapp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-03-07 18:10:03.000000 google-cloud-netapp-0.3.8/google_cloud_netapp.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-07 18:10:03.000000 google-cloud-netapp-0.3.8/google_cloud_netapp.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-07 18:10:03.979005 google-cloud-netapp-0.3.8/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3159 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-07 18:10:03.975005 google-cloud-netapp-0.3.8/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-07 18:10:03.975005 google-cloud-netapp-0.3.8/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-07 18:10:03.975005 google-cloud-netapp-0.3.8/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-07 18:10:03.979005 google-cloud-netapp-0.3.8/tests/unit/gapic/netapp_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/tests/unit/gapic/netapp_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003  1213636 2024-03-07 18:06:43.000000 google-cloud-netapp-0.3.8/tests/unit/gapic/netapp_v1/test_net_app.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:42.841706 google-cloud-netapp-0.3.9/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5065 2024-03-22 12:19:42.841706 google-cloud-netapp-0.3.9/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3704 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:42.825704 google-cloud-netapp-0.3.9/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:42.825704 google-cloud-netapp-0.3.9/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:42.829705 google-cloud-netapp-0.3.9/google/cloud/netapp/
+-rw-rw-r--   0 root         (0)     1003     6270 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:42.829705 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/
+-rw-rw-r--   0 root         (0)     1003     5938 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20077 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:42.829705 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:42.829705 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/
+-rw-rw-r--   0 root         (0)     1003      737 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/__init__.py
+-rw-rw-r--   0 root         (0)     1003   283639 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/async_client.py
+-rw-rw-r--   0 root         (0)     1003   306005 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/client.py
+-rw-rw-r--   0 root         (0)     1003    46079 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:42.833705 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/transports/
+-rw-rw-r--   0 root         (0)     1003     1288 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    37254 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    75291 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    77048 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   290460 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:42.837705 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/
+-rw-rw-r--   0 root         (0)     1003     5652 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11218 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/active_directory.py
+-rw-rw-r--   0 root         (0)     1003    11350 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/backup.py
+-rw-rw-r--   0 root         (0)     1003     9958 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/backup_policy.py
+-rw-rw-r--   0 root         (0)     1003     8142 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/backup_vault.py
+-rw-rw-r--   0 root         (0)     1003     2851 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/cloud_netapp_service.py
+-rw-rw-r--   0 root         (0)     1003     1824 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003    10331 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/kms.py
+-rw-rw-r--   0 root         (0)     1003    19307 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/replication.py
+-rw-rw-r--   0 root         (0)     1003     8125 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/snapshot.py
+-rw-rw-r--   0 root         (0)     1003    10447 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/storage_pool.py
+-rw-rw-r--   0 root         (0)     1003    32892 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/volume.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:42.837705 google-cloud-netapp-0.3.9/google_cloud_netapp.egg-info/
+-rw-r--r--   0 root         (0)     1003     5065 2024-03-22 12:19:42.000000 google-cloud-netapp-0.3.9/google_cloud_netapp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1771 2024-03-22 12:19:42.000000 google-cloud-netapp-0.3.9/google_cloud_netapp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-03-22 12:19:42.000000 google-cloud-netapp-0.3.9/google_cloud_netapp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-03-22 12:19:42.000000 google-cloud-netapp-0.3.9/google_cloud_netapp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-03-22 12:19:42.000000 google-cloud-netapp-0.3.9/google_cloud_netapp.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-03-22 12:19:42.000000 google-cloud-netapp-0.3.9/google_cloud_netapp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-03-22 12:19:42.841706 google-cloud-netapp-0.3.9/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3159 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:42.837705 google-cloud-netapp-0.3.9/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:42.837705 google-cloud-netapp-0.3.9/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:42.837705 google-cloud-netapp-0.3.9/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:42.837705 google-cloud-netapp-0.3.9/tests/unit/gapic/netapp_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/tests/unit/gapic/netapp_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003  1213636 2024-03-22 12:15:15.000000 google-cloud-netapp-0.3.9/tests/unit/gapic/netapp_v1/test_net_app.py
```

### Comparing `google-cloud-netapp-0.3.8/LICENSE` & `google-cloud-netapp-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/MANIFEST.in` & `google-cloud-netapp-0.3.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/PKG-INFO` & `google-cloud-netapp-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-netapp
-Version: 0.3.8
+Version: 0.3.9
 Summary: Google Cloud Netapp API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-netapp
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-netapp-0.3.8/README.rst` & `google-cloud-netapp-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp/__init__.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp/gapic_version.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.3.8"  # {x-release-please-version}
+__version__ = "0.3.9"  # {x-release-please-version}
```

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/__init__.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/gapic_metadata.json` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/gapic_version.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.3.8"  # {x-release-please-version}
+__version__ = "0.3.9"  # {x-release-please-version}
```

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/__init__.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/__init__.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/async_client.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/client.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/pagers.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/transports/__init__.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/transports/base.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/transports/grpc.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/transports/grpc_asyncio.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/services/net_app/transports/rest.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/services/net_app/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/__init__.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/active_directory.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/active_directory.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/backup.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/backup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/backup_policy.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/backup_policy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/backup_vault.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/backup_vault.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/cloud_netapp_service.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/cloud_netapp_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/common.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/kms.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/kms.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/replication.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/replication.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/snapshot.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/snapshot.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/storage_pool.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/storage_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,17 +238,16 @@
         kms_config (str):
             Optional. Specifies the KMS config to be used
             for volume encryption.
         ldap_enabled (bool):
             Optional. Flag indicating if the pool is NFS
             LDAP enabled or not.
         psa_range (str):
-            Optional. This field is currently not
-            implemented. Currently values provided in this
-            field will be ignored.
+            Optional. This field is not implemented. The
+            values provided in this field are ignored.
         encryption_type (google.cloud.netapp_v1.types.EncryptionType):
             Output only. Specifies the current pool
             encryption key source.
         global_access_allowed (bool):
             Deprecated. Used to allow SO pool to access
             AD or DNS server from other regions.
```

### Comparing `google-cloud-netapp-0.3.8/google/cloud/netapp_v1/types/volume.py` & `google-cloud-netapp-0.3.9/google/cloud/netapp_v1/types/volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
     Values:
         SECURITY_STYLE_UNSPECIFIED (0):
             SecurityStyle is unspecified
         NTFS (1):
             SecurityStyle uses NTFS
         UNIX (2):
-            SecurityStyle uses NTFS
+            SecurityStyle uses UNIX
     """
     SECURITY_STYLE_UNSPECIFIED = 0
     NTFS = 1
     UNIX = 2
 
 
 class RestrictedAction(proto.Enum):
@@ -367,17 +367,16 @@
         state_details (str):
             Output only. State details of the volume
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Create time of the volume
         share_name (str):
             Required. Share name of the volume
         psa_range (str):
-            Output only. This field is currently not
-            implemented. Currently values provided in this
-            field will be ignored.
+            Output only. This field is not implemented.
+            The values provided in this field are ignored.
         storage_pool (str):
             Required. StoragePool name of the volume
         network (str):
             Output only. VPC Network name.
             Format:
             projects/{project}/global/networks/{network}
         service_level (google.cloud.netapp_v1.types.ServiceLevel):
```

### Comparing `google-cloud-netapp-0.3.8/google_cloud_netapp.egg-info/PKG-INFO` & `google-cloud-netapp-0.3.9/google_cloud_netapp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-netapp
-Version: 0.3.8
+Version: 0.3.9
 Summary: Google Cloud Netapp API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-netapp
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-netapp-0.3.8/google_cloud_netapp.egg-info/SOURCES.txt` & `google-cloud-netapp-0.3.9/google_cloud_netapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/setup.py` & `google-cloud-netapp-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/tests/__init__.py` & `google-cloud-netapp-0.3.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/tests/unit/__init__.py` & `google-cloud-netapp-0.3.9/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/tests/unit/gapic/__init__.py` & `google-cloud-netapp-0.3.9/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/tests/unit/gapic/netapp_v1/__init__.py` & `google-cloud-netapp-0.3.9/tests/unit/gapic/netapp_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.3.8/tests/unit/gapic/netapp_v1/test_net_app.py` & `google-cloud-netapp-0.3.9/tests/unit/gapic/netapp_v1/test_net_app.py`

 * *Files identical despite different names*

