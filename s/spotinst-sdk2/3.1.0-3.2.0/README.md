# Comparing `tmp/spotinst-sdk2-3.1.0.tar.gz` & `tmp/spotinst-sdk2-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-sdk2-3.1.0.tar", last modified: Wed Apr 24 11:53:01 2024, max compression
+gzip compressed data, was "spotinst-sdk2-3.2.0.tar", last modified: Fri May 17 06:14:32 2024, max compression
```

## Comparing `spotinst-sdk2-3.1.0.tar` & `spotinst-sdk2-3.2.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    11356 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/LICENSE
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       43 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      751 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/NOTICE.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8093 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/PKG-INFO
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     7177 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/README.md
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       63 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/setup.cfg
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     3535 2024-04-24 11:51:28.000000 spotinst-sdk2-3.1.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.825429 spotinst-sdk2-3.1.0/spotinst_sdk2/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     5098 2024-04-24 11:51:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15928 2023-11-20 13:07:49.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.837425 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.837425 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/admin/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12645 2024-02-01 18:22:35.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/admin/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.837425 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/elastigroup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    78320 2024-04-19 16:12:01.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/elastigroup/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/functions/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3184 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/functions/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/hpc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3376 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/hpc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/managed_instance/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11698 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/managed_instance/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/mcs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      916 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/mcs/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/mrscaler/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6286 2024-02-25 21:58:42.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/mrscaler/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/ocean/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    80602 2024-04-24 11:51:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/ocean/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/ocean_cd/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30586 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/ocean_cd/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/setup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5562 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/setup/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/stateful_node/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16650 2023-11-25 09:32:13.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/stateful_node/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/subscription/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3859 2024-01-27 17:33:52.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/subscription/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/admin/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/admin/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      548 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/admin/user_mapping.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    40959 2024-04-19 15:27:36.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/asg.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1278 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/deployment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      931 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/deployment_action.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/stateful.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/azure_v3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21715 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/azure_v3/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/gcp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17709 2023-08-16 14:46:57.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/gcp/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/functions/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3685 2023-11-08 04:25:02.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/functions/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/hpc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 14:21:47.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/hpc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/hpc/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4954 2023-11-08 04:25:02.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/hpc/aws/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/managed_instance/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/managed_instance/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/managed_instance/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15583 2024-04-19 15:27:36.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/managed_instance/aws/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/mrscaler/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/mrscaler/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/mrscaler/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18653 2024-02-25 21:58:42.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/mrscaler/aws/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36517 2024-02-25 21:58:42.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/aws/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/azure/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19808 2024-04-19 15:58:50.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/azure/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/gcp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24001 2024-04-24 11:51:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/gcp/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      806 2023-04-11 10:16:17.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2988 2023-11-08 04:23:08.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/rollout.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8887 2023-04-11 10:16:17.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/rollout_spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4154 2023-04-11 10:16:17.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/strategy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2652 2023-11-08 04:23:37.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/verification_provider.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9061 2023-11-08 04:23:47.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/verification_template.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/spotinst_sdk2/models/setup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/setup/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/spotinst_sdk2/models/setup/azure/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1082 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/setup/azure/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/spotinst_sdk2/models/setup/gcp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1656 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/setup/gcp/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/spotinst_sdk2/models/stateful_node/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27588 2024-02-25 21:58:42.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/stateful_node/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/spotinst_sdk2/models/subscription/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      856 2023-11-08 04:24:10.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/subscription/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2615 2023-11-08 04:24:57.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/session.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-04-24 11:51:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.837425 spotinst-sdk2-3.1.0/spotinst_sdk2.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8093 2024-04-24 11:53:01.000000 spotinst-sdk2-3.1.0/spotinst_sdk2.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2392 2024-04-24 11:53:01.000000 spotinst-sdk2-3.1.0/spotinst_sdk2.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-24 11:53:01.000000 spotinst-sdk2-3.1.0/spotinst_sdk2.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-04-24 11:53:01.000000 spotinst-sdk2-3.1.0/spotinst_sdk2.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-04-24 11:53:01.000000 spotinst-sdk2-3.1.0/spotinst_sdk2.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.057842 spotinst-sdk2-3.2.0/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    11356 2023-02-24 13:45:28.000000 spotinst-sdk2-3.2.0/LICENSE
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       43 2023-02-24 13:45:28.000000 spotinst-sdk2-3.2.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      751 2023-02-24 13:45:28.000000 spotinst-sdk2-3.2.0/NOTICE.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8093 2024-05-17 06:14:32.057842 spotinst-sdk2-3.2.0/PKG-INFO
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     7177 2023-02-24 13:45:28.000000 spotinst-sdk2-3.2.0/README.md
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       63 2024-05-17 06:14:32.057842 spotinst-sdk2-3.2.0/setup.cfg
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     3535 2024-04-24 11:51:28.000000 spotinst-sdk2-3.2.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     5098 2024-04-24 11:51:28.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15928 2023-11-20 13:07:49.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/admin/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12645 2024-02-01 18:22:35.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/admin/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/elastigroup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    78320 2024-04-19 16:12:01.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/elastigroup/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/functions/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3184 2023-11-08 04:20:46.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/functions/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/hpc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3376 2023-11-08 04:20:46.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/hpc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/managed_instance/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11698 2023-11-08 04:20:46.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/managed_instance/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/mcs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      916 2023-11-08 04:20:46.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/mcs/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/mrscaler/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6286 2024-02-25 21:58:42.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/mrscaler/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/ocean/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    80602 2024-04-24 11:51:28.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/ocean/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/ocean_cd/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30586 2023-11-08 04:20:46.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/ocean_cd/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/setup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5562 2023-11-08 04:20:46.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/setup/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/stateful_node/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16650 2023-11-25 09:32:13.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/stateful_node/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/subscription/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3859 2024-01-27 17:33:52.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/clients/subscription/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/admin/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/admin/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      548 2023-02-24 13:45:28.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/admin/user_mapping.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/aws/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    40959 2024-04-19 15:27:36.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/aws/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-11-08 04:20:46.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/aws/asg.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1278 2023-11-08 04:20:46.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/aws/deployment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      931 2023-11-08 04:20:46.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/aws/deployment_action.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-11-08 04:20:46.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/aws/stateful.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/azure_v3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21715 2023-11-08 04:20:46.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/azure_v3/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/gcp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17709 2023-08-16 14:46:57.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/gcp/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/functions/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3685 2023-11-08 04:25:02.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/functions/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/hpc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 14:21:47.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/hpc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/hpc/aws/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4954 2023-11-08 04:25:02.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/hpc/aws/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/managed_instance/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/managed_instance/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/managed_instance/aws/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15583 2024-04-19 15:27:36.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/managed_instance/aws/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/mrscaler/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/mrscaler/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/mrscaler/aws/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18653 2024-02-25 21:58:42.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/mrscaler/aws/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean/aws/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36517 2024-02-25 21:58:42.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean/aws/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean/azure/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20381 2024-05-17 06:14:16.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean/azure/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean/gcp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24001 2024-04-24 11:51:28.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean/gcp/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean_cd/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      806 2023-04-11 10:16:17.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean_cd/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2988 2023-11-08 04:23:08.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean_cd/rollout.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8887 2023-04-11 10:16:17.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean_cd/rollout_spec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4154 2023-04-11 10:16:17.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean_cd/strategy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2652 2023-11-08 04:23:37.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean_cd/verification_provider.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9061 2023-11-08 04:23:47.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean_cd/verification_template.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.057842 spotinst-sdk2-3.2.0/spotinst_sdk2/models/setup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/setup/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.057842 spotinst-sdk2-3.2.0/spotinst_sdk2/models/setup/azure/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1082 2023-02-24 13:45:28.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/setup/azure/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.057842 spotinst-sdk2-3.2.0/spotinst_sdk2/models/setup/gcp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1656 2023-02-24 13:45:28.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/setup/gcp/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.057842 spotinst-sdk2-3.2.0/spotinst_sdk2/models/stateful_node/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27588 2024-02-25 21:58:42.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/stateful_node/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.057842 spotinst-sdk2-3.2.0/spotinst_sdk2/models/subscription/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      856 2023-11-08 04:24:10.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/models/subscription/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2615 2023-11-08 04:24:57.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/session.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-05-17 06:14:16.000000 spotinst-sdk2-3.2.0/spotinst_sdk2/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 06:14:32.053840 spotinst-sdk2-3.2.0/spotinst_sdk2.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8093 2024-05-17 06:14:31.000000 spotinst-sdk2-3.2.0/spotinst_sdk2.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2392 2024-05-17 06:14:31.000000 spotinst-sdk2-3.2.0/spotinst_sdk2.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-17 06:14:31.000000 spotinst-sdk2-3.2.0/spotinst_sdk2.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-05-17 06:14:31.000000 spotinst-sdk2-3.2.0/spotinst_sdk2.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-05-17 06:14:31.000000 spotinst-sdk2-3.2.0/spotinst_sdk2.egg-info/top_level.txt
```

### Comparing `spotinst-sdk2-3.1.0/LICENSE` & `spotinst-sdk2-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/NOTICE.md` & `spotinst-sdk2-3.2.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/PKG-INFO` & `spotinst-sdk2-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-sdk2
-Version: 3.1.0
+Version: 3.2.0
 Summary: A Python SDK for Spotinst
 Home-page: https://github.com/spotinst/spotinst-sdk-python
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst spot instances aws azure ec2 cloud infrastructure development elastigroup
 Platform: UNKNOWN
```

### Comparing `spotinst-sdk2-3.1.0/README.md` & `spotinst-sdk2-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/setup.py` & `spotinst-sdk2-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/client.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/client.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/admin/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/clients/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/elastigroup/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/clients/elastigroup/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/functions/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/clients/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/hpc/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/clients/hpc/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/managed_instance/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/clients/managed_instance/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/mcs/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/clients/mcs/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/mrscaler/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/clients/mrscaler/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/ocean/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/clients/ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/ocean_cd/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/clients/ocean_cd/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/setup/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/clients/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/stateful_node/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/clients/stateful_node/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/subscription/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/clients/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/admin/user_mapping.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/admin/user_mapping.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/asg.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/aws/asg.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/deployment.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/aws/deployment.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/deployment_action.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/aws/deployment_action.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/stateful.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/aws/stateful.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/azure_v3/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/azure_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/gcp/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/elastigroup/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/functions/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/hpc/aws/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/hpc/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/managed_instance/aws/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/managed_instance/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/mrscaler/aws/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/mrscaler/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/aws/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/azure/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean/azure/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -331,14 +331,27 @@
     memory_optimized = "memoryOptimized"
     compute_optimized = "computeOptimized"
     high_performance_compute = "highPerformanceCompute"
     storage_optimized = "storageOptimized"
     gpu = "GPU"
 
 
+class GpuType(Enum):
+    nvidia_tesla_v100 = "nvidia-tesla-v100" 
+    amd_radeon_instinct_mi25 = "amd-radeon-instinct-mi25"
+    nvidia_a10 = "nvidia-a10" 
+    nvidia_tesla_a100 = "nvidia-tesla-a100" 
+    nvidia_tesla_k80 = "nvidia-tesla-k80" 
+    nvidia_tesla_m60 = "nvidia-tesla-m60" 
+    nvidia_tesla_p100 = "nvidia-tesla-p100" 
+    nvidia_tesla_p40 = "nvidia-tesla-p40" 
+    nvidia_tesla_t4 = "nvidia-tesla-t4" 
+    nvidia_tesla_h100 = "nvidia-tesla-h100"   
+
+
 class Filters:
     """
     # Arguments
     accelerated_networking: AcceleratedNetworking
     disk_performance: DiskPerformance
     architectures: List[Architecture]
     exclude_series: List[str]
@@ -348,14 +361,15 @@
     min_v_cpu: int
     min_gpu: float
     max_gpu: float
     min_data: int
     min_n_i_cs: int
     series: List[str]
     vm_types: List[VmType]
+    gpu_types: List[GpuType]
     """
 
     def __init__(
             self,
             accelerated_networking: AcceleratedNetworking = none,
             disk_performance: DiskPerformance = none,
             architectures: List[Architecture] = none,
@@ -365,29 +379,31 @@
             min_memory_gi_b: float = none,
             min_v_cpu: int = none,
             min_gpu: float = none,
             max_gpu: float = none,
             min_data: int = none,
             min_n_i_cs: int = none,
             series: List[str] = none,
-            vm_types: List[VmType] = none):
+            vm_types: List[VmType] = none,
+            gpu_types: List[GpuType] = none):
         self.accelerated_networking = accelerated_networking
         self.disk_performance = disk_performance
         self.architectures = architectures
         self.exclude_series = exclude_series
         self.max_memory_gi_b = max_memory_gi_b
         self.max_v_cpu = max_v_cpu
         self.min_memory_gi_b = min_memory_gi_b
         self.min_v_cpu = min_v_cpu
         self.min_gpu = min_gpu
         self.max_gpu = max_gpu
         self.min_data = min_data
         self.min_n_i_cs = min_n_i_cs
         self.series = series
         self.vm_types = vm_types
+        self.gpu_types = gpu_types
 
 
 class VmSizes:
     """
     # Arguments
     filters: Filters
     """
```

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/gcp/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean_cd/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/rollout.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean_cd/rollout.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/rollout_spec.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean_cd/rollout_spec.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/strategy.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean_cd/strategy.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/verification_provider.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean_cd/verification_provider.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/verification_template.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/ocean_cd/verification_template.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/setup/azure/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/setup/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/setup/gcp/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/setup/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/stateful_node/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/stateful_node/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/models/subscription/__init__.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/models/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2/session.py` & `spotinst-sdk2-3.2.0/spotinst_sdk2/session.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2.egg-info/PKG-INFO` & `spotinst-sdk2-3.2.0/spotinst_sdk2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-sdk2
-Version: 3.1.0
+Version: 3.2.0
 Summary: A Python SDK for Spotinst
 Home-page: https://github.com/spotinst/spotinst-sdk-python
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst spot instances aws azure ec2 cloud infrastructure development elastigroup
 Platform: UNKNOWN
```

### Comparing `spotinst-sdk2-3.1.0/spotinst_sdk2.egg-info/SOURCES.txt` & `spotinst-sdk2-3.2.0/spotinst_sdk2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

