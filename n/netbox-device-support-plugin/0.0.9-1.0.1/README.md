# Comparing `tmp/netbox-device-support-plugin-0.0.9.tar.gz` & `tmp/netbox_device_support_plugin-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-device-support-plugin-0.0.9.tar", last modified: Tue Nov 21 12:51:45 2023, max compression
+gzip compressed data, was "netbox_device_support_plugin-1.0.1.tar", last modified: Fri May 17 18:07:56 2024, max compression
```

## Comparing `netbox-device-support-plugin-0.0.9.tar` & `netbox_device_support_plugin-1.0.1.tar`

### file list

```diff
@@ -1,56 +1,64 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/
--rw-r--r--   0 vsts      (1001) docker     (127)     1068 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)       58 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    13514 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    12867 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.780943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (127)      678 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2448 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.780943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/api/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3199 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/api/serializers.py
--rw-r--r--   0 vsts      (1001) docker     (127)      415 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/api/urls.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1239 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/api/views.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5438 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/filtersets.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12196 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/forms.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.780943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/management/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39500 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/migrations/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35472 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/models.py
--rw-r--r--   0 vsts      (1001) docker     (127)      537 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/navigation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4954 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/tables.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5150 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.776943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/
--rw-r--r--   0 vsts      (1001) docker     (127)     6651 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/cisco_device_support.html
--rw-r--r--   0 vsts      (1001) docker     (127)     4524 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/
--rw-r--r--   0 vsts      (1001) docker     (127)      832 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      896 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1078 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      888 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1038 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1030 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      966 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1046 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/fortinet/
--rw-r--r--   0 vsts      (1001) docker     (127)     4709 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2960 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templatetags/filters.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1585 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/urls.py
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2491 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/views.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    13514 2023-11-21 12:51:45.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2205 2023-11-21 12:51:45.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-11-21 12:51:45.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-11-21 12:51:45.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)       29 2023-11-21 12:51:45.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2023-11-21 12:51:45.788943 netbox-device-support-plugin-0.0.9/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1570 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1068 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)       58 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    13514 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    12867 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.937671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2917 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.937671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/api/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4667 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/api/serializers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/api/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1657 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/api/views.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6089 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/filtersets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13398 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/forms.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.937671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.937671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40834 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8273 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/commands/sync_fortinet_support_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8319 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/commands/sync_purestorage_support_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.937671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (127)     7956 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/migrations/0001_initial.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    32812 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/models.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      739 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/navigation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5749 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/tables.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6535 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.933671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.937671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6284 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/cisco_device_support.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     4237 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/
+-rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      896 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1078 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1030 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      966 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1046 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/fortinet/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4308 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/fortinet/inc/
+-rw-r--r--   0 vsts      (1001) docker     (127)      896 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/fortinet/inc/device_eor_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      896 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/fortinet/inc/device_eos_bar.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/purestorage/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1845 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/purestorage/purestorage_device_support.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2960 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2107 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3402 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/views.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    13514 2024-05-17 18:07:56.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2649 2024-05-17 18:07:56.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-17 18:07:56.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-17 18:07:56.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-05-17 18:07:56.000000 netbox_device_support_plugin-1.0.1/netbox_device_support_plugin.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-17 18:07:56.941671 netbox_device_support_plugin-1.0.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1570 2024-05-17 18:07:39.000000 netbox_device_support_plugin-1.0.1/setup.py
```

### Comparing `netbox-device-support-plugin-0.0.9/LICENSE` & `netbox_device_support_plugin-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.9/PKG-INFO` & `netbox_device_support_plugin-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-device-support-plugin
-Version: 0.0.9
+Version: 1.0.1
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-device-support-plugin-0.0.9/README.md` & `netbox_device_support_plugin-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/admin.py` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 from django.contrib import admin
-from .models import CiscoDeviceTypeSupport, CiscoDeviceSupport, FortinetDeviceSupport
+from .models import (
+    CiscoDeviceTypeSupport,
+    CiscoDeviceSupport,
+    FortinetDeviceSupport,
+    PureStorageDeviceSupport,
+)
 
 
 #### Cisco Support ##########################################################################################
 
 
 @admin.register(CiscoDeviceTypeSupport)
 class DeviceSupportAdmin(admin.ModelAdmin):
@@ -68,14 +73,15 @@
         "warranty_type",
         "partner_status",
         "partner_service_level",
         "partner_customer_number",
         "partner_coverage_end_date",
     )
 
+
 #### Fortinet Support #######################################################################################
 
 
 @admin.register(FortinetDeviceSupport)
 class DeviceSupportAdmin(admin.ModelAdmin):
     exclude = (
         "name",
@@ -89,8 +95,29 @@
         "device",
         "name",
         "serial",
         "pid",
         "recommended_release",
         "desired_release",
         "current_release",
-    )
+    )
+
+
+#### PureStorage Support ####################################################################################
+
+
+@admin.register(PureStorageDeviceSupport)
+class DeviceSupportAdmin(admin.ModelAdmin):
+    exclude = (
+        "name",
+        "serial",
+        "pid",
+    )
+
+    list_display = (
+        "device",
+        "name",
+        "serial",
+        "pid",
+        "desired_release",
+        "current_release",
+    )
```

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/api/serializers.py` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/api/serializers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,112 @@
 from rest_framework import serializers
 
 from netbox.api.serializers import NetBoxModelSerializer
-from dcim.api.serializers import NestedDeviceTypeSerializer, NestedDeviceSerializer
-from ..models import CiscoDeviceTypeSupport, CiscoDeviceSupport, FortinetDeviceSupport
+from dcim.api.serializers import DeviceTypeSerializer, DeviceSerializer
+from ..models import (
+    CiscoDeviceTypeSupport,
+    CiscoDeviceSupport,
+    FortinetDeviceSupport,
+    PureStorageDeviceSupport,
+)
 
 
 #### Cisco Support ##########################################################################################
 
 
 class CiscoDeviceTypeSupportSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_device_support_plugin-api:ciscodevicetypesupport-detail"
     )
 
-    device_type = NestedDeviceTypeSerializer()
+    device_type = DeviceTypeSerializer(nested=True)
 
     class Meta:
         model = CiscoDeviceTypeSupport
         # fmt: off
-        fields = [
+        fields = (
             "id", "url", "display", "name", "device_type", "pid", "eox_has_error", "eox_error",
             "eox_announcement_date", "end_of_sale_date", "end_of_sw_maintenance_releases",
             "end_of_security_vul_support_date", "end_of_routine_failure_analysis_date",
             "end_of_service_contract_renewal", "last_date_of_support", "end_of_svc_attach_date",
             "tags", "custom_fields", "created", "last_updated",
-        ]
+        )
+        brief_fields = ("id", "url", "display", "name", "device_type", "pid", "eox_has_error", "eox_error")
         # fmt: on
 
 
 class CiscoDeviceSupportSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_device_support_plugin-api:ciscodevicesupport-detail"
     )
 
-    device = NestedDeviceSerializer()
+    device = DeviceSerializer(nested=True)
 
     class Meta:
         model = CiscoDeviceSupport
         # fmt: off
-        fields = [
+        fields = (
             "id", "url", "display", "name", "device", "pid", "serial", "api_status", "sr_no_owner",
             "is_covered", "coverage_end_date", "contract_supplier", "service_line_descr",
             "service_contract_number", "warranty_end_date", "warranty_type", "partner_status",
             "partner_service_level", "partner_customer_number", "partner_coverage_end_date",
             "recommended_release", "desired_release", "current_release", "desired_release_status",
             "current_release_status", "eox_has_error", "eox_error", "eox_announcement_date",
             "end_of_sale_date", "end_of_sw_maintenance_releases", "end_of_security_vul_support_date",
             "end_of_routine_failure_analysis_date", "end_of_service_contract_renewal",
             "last_date_of_support", "end_of_svc_attach_date", "tags", "custom_fields", "created",
             "last_updated",
-        ]
+        )
+        brief_fields = (
+            "id", "url", "display", "name", "device", "pid", "serial", "api_status",
+            "sr_no_owner","is_covered", "coverage_end_date", "contract_supplier",
+        )
         # fmt: on
 
 
 #### Fortinet Support #######################################################################################
 
-"""
+
 class FortinetDeviceSupportSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_device_support_plugin-api:fortinetdevicesupport-detail"
     )
 
-    device = NestedDeviceSerializer()
+    device = DeviceSerializer(nested=True)
 
     class Meta:
         model = FortinetDeviceSupport
         # fmt: off
-        fields = [
+        fields = (
+            "id", "url", "display", "name", "device", "pid", "serial", "recommended_release",
+            "desired_release", "current_release", "desired_release_status", "current_release_status",
+            "partner", "end_of_renewal_date", "end_of_support_date", "tags", "custom_fields", "created",
+            "last_updated",
+        )
+        brief_fields = (
             "id", "url", "display", "name", "device", "pid", "serial", "recommended_release",
             "desired_release", "current_release", "desired_release_status", "current_release_status",
+        )
+        # fmt: on
+
+
+#### PureStorage Support ####################################################################################
+
+
+class PureStorageDeviceSupportSerializer(NetBoxModelSerializer):
+    url = serializers.HyperlinkedIdentityField(
+        view_name="plugins-api:netbox_device_support_plugin-api:purestoragedevicesupport-detail"
+    )
+
+    device = DeviceSerializer(nested=True)
+
+    class Meta:
+        model = PureStorageDeviceSupport
+        # fmt: off
+        fields = (
+            "id", "url", "display", "name", "device", "pid", "serial", "desired_release", "current_release",
             "tags", "custom_fields", "created", "last_updated",
-        ]
+        )
+        brief_fields = (
+            "id", "url", "display", "name", "device", "pid", "serial", "desired_release", "current_release",
+        )
         # fmt: on
-"""
```

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/api/views.py` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/api/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from netbox.api.viewsets import NetBoxModelViewSet
 
 from .. import models, filtersets
 from .serializers import (
     CiscoDeviceSupportSerializer,
     CiscoDeviceTypeSupportSerializer,
     FortinetDeviceSupportSerializer,
+    PureStorageDeviceSupportSerializer,
 )
 
 
 #### Cisco Support ##########################################################################################
 
 
 class CiscoDeviceSupportViewSet(NetBoxModelViewSet):
@@ -22,13 +23,20 @@
     serializer_class = CiscoDeviceTypeSupportSerializer
     filterset_class = filtersets.CiscoDeviceTypeSupportFilterSet
 
 
 #### Fortinet Support #######################################################################################
 
 
-"""
 class FortinetDeviceSupportViewSet(NetBoxModelViewSet):
     queryset = models.FortinetDeviceSupport.objects.all().prefetch_related("device")
     serializer_class = FortinetDeviceSupportSerializer
     filterset_class = filtersets.FortinetDeviceSupportFilterSet
-"""
+
+
+#### PureStorage Support ####################################################################################
+
+
+class PureStorageDeviceSupportViewSet(NetBoxModelViewSet):
+    queryset = models.PureStorageDeviceSupport.objects.all().prefetch_related("device")
+    serializer_class = PureStorageDeviceSupportSerializer
+    filterset_class = filtersets.PureStorageDeviceSupportFilterSet
```

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/filtersets.py` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/filtersets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import django_filters
 from utilities.filters import MultiValueCharFilter
 from netbox.filtersets import BaseFilterSet
-from .models import CiscoDeviceSupport, CiscoDeviceTypeSupport, FortinetDeviceSupport
+from .models import (
+    CiscoDeviceSupport,
+    CiscoDeviceTypeSupport,
+    FortinetDeviceSupport,
+    PureStorageDeviceSupport,
+)
 
 
 #### Cisco Support ##########################################################################################
 
 
 class CiscoDeviceSupportFilterSet(BaseFilterSet):
     name = MultiValueCharFilter(lookup_expr="iexact")
@@ -129,15 +134,35 @@
 
     desired_release = MultiValueCharFilter(lookup_expr="iexact")
 
     current_release_status = django_filters.BooleanFilter(required=False)
 
     current_release = MultiValueCharFilter(lookup_expr="iexact")
 
+    partner = MultiValueCharFilter(lookup_expr="icontains")
+
     class Meta:
         model = FortinetDeviceSupport
         # fmt: off
         fields = (
             "id", "name", "pid", "recommended_release", "desired_release_status", "desired_release",
-            "current_release_status", "current_release"
+            "current_release_status", "current_release", "partner", "end_of_renewal_date",
+            "end_of_support_date",
+        )
+        # fmt: on
+
+
+#### PureStorage Support ####################################################################################
+
+
+class PureStorageDeviceSupportFilterSet(BaseFilterSet):
+    name = MultiValueCharFilter(lookup_expr="iexact")
+
+    pid = MultiValueCharFilter(lookup_expr="iexact")
+
+    class Meta:
+        model = PureStorageDeviceSupport
+        # fmt: off
+        fields = (
+            "id", "name", "pid", "desired_release", "current_release",
         )
         # fmt: on
```

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/forms.py` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/forms.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,71 +1,63 @@
 from django import forms
-from extras.forms.mixins import SavedFiltersMixin
+from netbox.forms.mixins import SavedFiltersMixin
 from utilities.forms import BOOLEAN_WITH_BLANK_CHOICES, FilterForm
-from .models import CiscoDeviceSupport, CiscoDeviceTypeSupport, FortinetDeviceSupport
+from utilities.forms.rendering import FieldSet
+from .models import (
+    CiscoDeviceSupport,
+    CiscoDeviceTypeSupport,
+    FortinetDeviceSupport,
+    PureStorageDeviceSupport,
+)
 
 
 #### Cisco Support ##########################################################################################
 
 
 class CiscoDeviceSupportFilterForm(SavedFiltersMixin, FilterForm):
     model = CiscoDeviceSupport
 
     fieldsets = (
-        (
-            "General",
-            (
-                "name",
-                "pid",
-            ),
+        FieldSet("name", "pid", name=("General")),
+        FieldSet(
+            "recommended_release",
+            "desired_release_status",
+            "desired_release",
+            "current_release_status",
+            "current_release",
+            name=("Software Release"),
         ),
-        (
-            "Software Release",
-            (
-                "recommended_release",
-                "desired_release_status",
-                "desired_release",
-                "current_release_status",
-                "current_release",
-            ),
+        FieldSet(
+            "sr_no_owner",
+            "is_covered",
+            "contract_supplier",
+            "coverage_end_date",
+            "service_line_descr",
+            "warranty_end_date",
+            name=("Device Support"),
         ),
-        (
-            "Device Support",
-            (
-                "sr_no_owner",
-                "is_covered",
-                "contract_supplier",
-                "coverage_end_date",
-                "service_line_descr",
-                "warranty_end_date",
-            ),
+        FieldSet(
+            "partner_status",
+            "partner_service_level",
+            "partner_customer_number",
+            "partner_coverage_end_date",
+            name=("Partner Contract"),
         ),
-        (
-            "Partner Contract",
-            (
-                "partner_status",
-                "partner_service_level",
-                "partner_customer_number",
-                "partner_coverage_end_date",
-            ),
-        ),
-        (
-            "Device Type Support",
-            (
-                "eox_has_error",
-                "eox_error",
-                "eox_announcement_date",
-                "end_of_sale_date",
-                "end_of_sw_maintenance_releases",
-                "end_of_security_vul_support_date",
-                "end_of_routine_failure_analysis_date",
-                "end_of_service_contract_renewal",
-                "end_of_svc_attach_date",
-                "last_date_of_support",
-            ),
+        FieldSet(
+            "eox_has_error",
+            "eox_error",
+            "eox_announcement_date",
+            "end_of_sale_date",
+            "end_of_sw_maintenance_releases",
+            "end_of_security_vul_support_date",
+            "end_of_routine_failure_analysis_date",
+            "end_of_service_contract_renewal",
+            "end_of_svc_attach_date",
+            "last_date_of_support",
+            name=("Device Type Support"),
         ),
     )
 
     name = forms.CharField(
         required=False,
         label="Device Name",
         help_text="Case-insensitive exact match",
@@ -233,35 +225,27 @@
     )
 
 
 class CiscoDeviceTypeSupportFilterForm(SavedFiltersMixin, FilterForm):
     model = CiscoDeviceTypeSupport
 
     fieldsets = (
-        (
-            "General",
-            (
-                "name",
-                "pid",
-            ),
-        ),
-        (
-            "Device Type Support",
-            (
-                "eox_has_error",
-                "eox_error",
-                "eox_announcement_date",
-                "end_of_sale_date",
-                "end_of_sw_maintenance_releases",
-                "end_of_security_vul_support_date",
-                "end_of_routine_failure_analysis_date",
-                "end_of_service_contract_renewal",
-                "end_of_svc_attach_date",
-                "last_date_of_support",
-            ),
+        FieldSet("name", "pid", name=("General")),
+        FieldSet(
+            "eox_has_error",
+            "eox_error",
+            "eox_announcement_date",
+            "end_of_sale_date",
+            "end_of_sw_maintenance_releases",
+            "end_of_security_vul_support_date",
+            "end_of_routine_failure_analysis_date",
+            "end_of_service_contract_renewal",
+            "end_of_svc_attach_date",
+            "last_date_of_support",
+            name=("Device Type Support"),
         ),
     )
 
     name = forms.CharField(
         required=False,
         label="Device Type Name",
         help_text="Case-insensitive exact match",
@@ -338,31 +322,24 @@
 #### Fortinet Support #######################################################################################
 
 
 class FortinetDeviceSupportFilterForm(SavedFiltersMixin, FilterForm):
     model = FortinetDeviceSupport
 
     fieldsets = (
-        (
-            "General",
-            (
-                "name",
-                "pid",
-            ),
-        ),
-        (
-            "Software Release",
-            (
-                "recommended_release",
-                "desired_release_status",
-                "desired_release",
-                "current_release_status",
-                "current_release",
-            ),
+        FieldSet("name", "pid", name=("General")),
+        FieldSet(
+            "recommended_release",
+            "desired_release_status",
+            "desired_release",
+            "current_release_status",
+            "current_release",
+            name=("Software Release"),
         ),
+        FieldSet("partner", "end_of_renewal_date", "end_of_support_date", name=("Device Support")),
     )
 
     name = forms.CharField(
         required=False,
         label="Device Name",
         help_text="Case-insensitive exact match",
     )
@@ -400,7 +377,61 @@
     )
 
     current_release = forms.CharField(
         required=False,
         label="Current Release",
         help_text="Case-insensitive exact match",
     )
+
+    partner = forms.CharField(
+        required=False,
+        label="Partner",
+        help_text="Case-insensitive exact match",
+    )
+
+    end_of_renewal_date = forms.CharField(
+        required=False,
+        label="End of Renewal Year",
+        help_text="Specify the end of renewal year (exact year match)",
+    )
+
+    end_of_support_date = forms.CharField(
+        required=False,
+        label="End of Support Year",
+        help_text="Specify the end of support year (exact year match)",
+    )
+
+
+#### PureStorage Support ####################################################################################
+
+
+class PureStorageDeviceSupportFilterForm(SavedFiltersMixin, FilterForm):
+    model = PureStorageDeviceSupport
+
+    fieldsets = (
+        FieldSet("name", "pid", name=("General")),
+        FieldSet("desired_release", "current_release", name=("Software Release")),
+    )
+
+    name = forms.CharField(
+        required=False,
+        label="Device Name",
+        help_text="Case-insensitive exact match",
+    )
+
+    pid = forms.CharField(
+        required=False,
+        label="PID",
+        help_text="Case-insensitive exact match",
+    )
+
+    desired_release = forms.CharField(
+        required=False,
+        label="Desired Release",
+        help_text="Case-insensitive exact match",
+    )
+
+    current_release = forms.CharField(
+        required=False,
+        label="Current Release",
+        help_text="Case-insensitive exact match",
+    )
```

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import sys
 import time
 import requests
-import json
-import django.utils.text
-
 from colorama import Fore, Style, init
 from django.conf import settings
-from django.core.management.base import BaseCommand, CommandError
+from django.core.management.base import BaseCommand
 from django.core.exceptions import MultipleObjectsReturned
 from typing import Generator, Union
 from datetime import datetime
-from requests import api
 from dcim.models import Manufacturer
 from dcim.models import Device, DeviceType
 from netbox_device_support_plugin.models import CiscoDeviceTypeSupport, CiscoDeviceSupport
 
 init(autoreset=True, strip=False)
 
 
@@ -100,17 +96,19 @@
             # Skip empty PID values
             if item[1] and item[0] == "base_pid":
                 pid = item[1]
                 break
             elif item[1] and item[0] == "orderable_pid":
                 pid = item[1]
                 break
-        # The software package suffic -A or -E can be removed as the newer basePID don't have this anymore
-        chg_suffixes = ["-A", "-E"]
-        pid = pid[:-2] if pid.endswith(tuple(chg_suffixes)) else pid
+        # Some basePID needs -A / -E to be removed or the API call will fail -> Maybe is a bug in the API
+        pid_prefixes = ["C9300X-24Y", "C9500-32C", "C9500-48Y4C"]
+        if pid.startswith(tuple(pid_prefixes)):
+            # The software package suffix -A or -E can be removed
+            pid = pid[:-2] if pid.endswith(tuple(["-A", "-E"])) else pid
 
         return pid
 
     def get_cisco_support_api_data(self, url, header):
         # Create a empty data dict for verification and to fill with the API response
         data = {}
 
@@ -188,19 +186,28 @@
 
         # If the recommended_release string is empty, print the error_description and return False
         if not recommended_release:
             error_description_stdout = error_description.replace("\n", " / ")
             # Remove the last two characters from the string to remove the trailing slash
             if error_description_stdout.endswith(" / "):
                 error_description_stdout = error_description_stdout[:-2]
-            print(self.task_error(text=text, changed=False))
-            print(f"{serial_number} - recommended_release: {error_description_stdout}")
+            # Error 'No records Found' is not a real error, but a valid response from the API
+            if "No records Found" in error_description:
+                print(self.task_info(text=text, changed=False))
+                print(f"{serial_number} - recommended_release: No records Found")
+                ds.recommended_release = "No records Found"
+                rtn = True
+            else:
+                print(self.task_error(text=text, changed=False))
+                print(f"{serial_number} - recommended_release: {error_description_stdout}")
+                ds.recommended_release = ""
+                rtn = False
             # Save model object for device
             ds.save()
-            return False
+            return rtn
 
         recommended_release_stdout = recommended_release.replace("\n", " / ")
         # Remove the last two characters from the string to remove the trailing slash
         if recommended_release_stdout.endswith(" / "):
             recommended_release_stdout = recommended_release_stdout[:-2]
 
         print(self.task_info(text=text, changed=False))
@@ -348,15 +355,15 @@
 
         except KeyError:
             print(f"{device['sr_no']} - warranty_end_date: : None")
 
         #### Get covered_product_line_end_date ##############################################################
         try:
             if not device["covered_product_line_end_date"]:
-                print(f"{device['sr_no']} - covered_product_line_end_date: : None")
+                print(f"{device['sr_no']} - covered_product_line_end_date: None")
             else:
                 coverage_end_date_string = device["covered_product_line_end_date"]
                 coverage_end_date = datetime.strptime(coverage_end_date_string, "%Y-%m-%d").date()
                 print(f"{device['sr_no']} - coverage_end_date: {coverage_end_date}")
 
                 # Update coverage_end_date
                 ds.coverage_end_date = coverage_end_date
@@ -686,15 +693,15 @@
 
         return api_call_headers
 
     # Main entry point for the sync_cisco_support command of manage.py
     def handle(self, *args, **kwargs):
         SYNC_FAILED = False
         PLUGIN_SETTINGS = settings.PLUGINS_CONFIG.get("netbox_device_support_plugin", dict())
-        MANUFACTURER = PLUGIN_SETTINGS.get("MANUFACTURER", "Cisco")
+        MANUFACTURER = PLUGIN_SETTINGS.get("CISCO_MANUFACTURER", "Cisco")
 
         # Logon one time and gather the required API key
         api_call_headers = self.logon()
 
         base_url = "https://apix.cisco.com"
 
         #### Step 1: Prepare all PIDs and serial numbers ####################################################
@@ -713,14 +720,26 @@
         print(self.task_name(text="Get EoX Data for PIDs"))
 
         for pid in product_ids:
             # Get the Cisco Support API data
             url = f"{base_url}/supporttools/eox/rest/5/EOXByProductID/1/{pid}?responseencoding=json"
             response, data = self.get_cisco_support_api_data(url=url, header=api_call_headers)
 
+            # Check if JSON contains EOXError
+            if "EOXError" in data["EOXRecord"][0]:
+                # Error SSA_ERR_021_Pid (Incorrect PID) can be wrong and therefor a second API call is made
+                # with a wildcard search for the PID
+                if (
+                    "SSA_ERR_021_Pid" in data["EOXRecord"][0]["EOXError"]["ErrorID"]
+                    or "Incorrect PID" in data["EOXRecord"][0]["EOXError"]["ErrorDescription"]
+                ):
+                    # Get the Cisco Support API data with a wildcard search for the PID
+                    url = f"{base_url}/supporttools/eox/rest/5/EOXByProductID/1/*{pid}*?responseencoding=json"
+                    response, data = self.get_cisco_support_api_data(url=url, header=api_call_headers)
+
             # Validate the data dict
             if data:
                 # Call our Device Type Update method for that particular PID
                 if not self.update_device_type_eox_data(pid, data):
                     SYNC_FAILED = True
             else:
                 # Show an error
@@ -733,15 +752,15 @@
         print(self.task_title(title="Update Device Support Information"))
         print(self.task_name(text="Get SNI Owner Status"))
 
         serial_numbers_copy = serial_numbers.copy()
         while serial_numbers_copy:
             # Pop the first items_to_fetch items of serial_numbers_copy into current_slice and then delete
             # them from serial numbers. We want to pass x items to the API each time we call it
-            items_to_fetch = 10
+            items_to_fetch = 50
             current_slice = serial_numbers_copy[:items_to_fetch]
             serial_numbers_copy[:items_to_fetch] = []
 
             # Get the Cisco Support API data
             url = f"{base_url}/sn2info/v2/coverage/owner_status/serial_numbers/{','.join(current_slice)}"
             response, data = self.get_cisco_support_api_data(url=url, header=api_call_headers)
 
@@ -756,25 +775,25 @@
                 # Show an error
                 SYNC_FAILED = True
                 print(self.task_error(text=f"Get data for serial number", changed=False))
                 print(f"API Response: {response}")
                 print(f"API Response Text: {response.text}")
                 print(f"Serial Numbers: {data['serial_numbers']}")
 
-        #### Step 4: Get SNI summary and EoX for all serial numbers #########################################
-        print(self.task_name(text="Get SNI Summary and EoX"))
+        #### Step 4: Get SNI summary for all serial numbers #################################################
+        print(self.task_name(text="Get SNI Summary"))
 
         # Dict to store the serial number and pid as key-value pair to use later for the recommended release
         serial_pid = {}
 
         serial_numbers_copy = serial_numbers.copy()
         while serial_numbers_copy:
             # Pop the first items_to_fetch items of serial_numbers_copy into current_slice and then delete them from serial
             # numbers. We want to pass x items to the API each time we call it
-            items_to_fetch = 10
+            items_to_fetch = 50
             current_slice = serial_numbers_copy[:items_to_fetch]
             serial_numbers_copy[:items_to_fetch] = []
 
             # Get the Cisco Support API data
             url = f"{base_url}/sn2info/v2/coverage/summary/serial_numbers/{','.join(current_slice)}"
             response, data = self.get_cisco_support_api_data(url=url, header=api_call_headers)
 
@@ -806,16 +825,16 @@
                 text = f"Get data for serial number {serial_number}"
                 print(self.task_error(text=text, changed=False))
                 print(f"{serial_number} - No PID found for this serial number")
                 continue
 
             # Normalize the PID list to match the base_pid of the API specs
             # Find PIDs which don't have a Cisco software
-            rm_prefixes = ["UCSC-C220-M5SX", "AIR-CAP"]
-            rm_suffixes = ["AXI", "AXI"]
+            rm_prefixes = ["UCSC", "AIR-CAP"]
+            rm_suffixes = ["AXI", "AXI-E", "AXE", "AXE-E"]
             if pid.startswith(tuple(rm_prefixes)) or pid.endswith(tuple(rm_suffixes)):
                 data = "PID without Cisco software"
                 # Call our Device Type Update method for that particular PID
                 self.update_device_ss_data(serial_number, pid, data)
                 continue
 
             # Call the release suggestions
```

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/models.py` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -70,408 +70,256 @@
 
     end_of_svc_attach_date = models.DateField(blank=True, null=True, verbose_name="End of Svc-Attach. Date")
 
     last_date_of_support = models.DateField(blank=True, null=True, verbose_name="Last Date of Support")
 
     #### Property Fileds for CiscoDeviceTypeSupport #########################################################
 
-    # Property field for end of sales date progress bar
-    @property
-    def end_of_sale_total(self):
-        """
-        Total days until EoX. Return None if end_of_sale_date not defined.
-        """
-        if self.eox_announcement_date and self.end_of_sale_date:
-            delta = self.end_of_sale_date - self.eox_announcement_date
-            return delta.days
-
-    # Property field for end of sales date progress bar
-    @property
-    def end_of_sale_remaining(self):
-        """
-        How many days are remaining. Return None if end_of_sale not defined.
-        """
-        if self.eox_announcement_date and self.end_of_sale_date:
-            delta = self.end_of_sale_date - date.today()
-            return delta.days
-        return None
-
-    # Property field for end of sales date progress bar
-    @property
-    def end_of_sale_elapsed(self):
-        """
-        How many days are elaped. Return None if end_of_sale not defined.
-        """
-        if self.eox_announcement_date and self.end_of_sale_date:
-            return self.end_of_sale_total - self.end_of_sale_remaining
-        return None
-
-    # Property field for end of sales date progress bar
+    #### Property field for end of sales date progress bar
     @property
     def end_of_sale_progress(self):
         """
-        Coverage progress in percent. Return None if coverage_end_date not defined.
+        Coverage progress in percent.
         """
         if self.eox_announcement_date and self.end_of_sale_date:
-            return round(self.end_of_sale_elapsed / self.end_of_sale_total * 100)
+            # Total days until EoX
+            total = self.end_of_sale_date - self.eox_announcement_date
+            total = total.days
+            # How many days are remaining until EoX
+            remaining = self.end_of_sale_date - date.today()
+            remaining = remaining.days
+            # How many days are elaped since EoX announcement
+            elapsed = total - remaining
+            # Return the progress in percent
+            return round(elapsed / total * 100)
         return None
 
-    # Property field for end of sales date progress bar
     @property
     def end_of_sale_progress_bar_class(self):
         """
         Coverage progress bar class.
         """
         if self.eox_announcement_date and self.end_of_sale_date:
-            if self.end_of_sale_remaining < 60:
+            # How many days are remaining until EoX
+            remaining = self.end_of_sale_date - date.today()
+            remaining = remaining.days
+            # Set the CSS class for the progress bar
+            if remaining < 60:
                 return "bg-danger"
-            if self.end_of_sale_remaining < 365:
+            if remaining < 365:
                 return "bg-warning"
         return "bg-success"
 
-    # Property field for end of software maintenance date progress bar
-    @property
-    def end_of_sw_maintenance_releases_total(self):
-        """
-        Total days until EoX. Return None if end_of_sale_date not defined.
-        """
-        if self.eox_announcement_date and self.end_of_sw_maintenance_releases:
-            delta = self.end_of_sw_maintenance_releases - self.eox_announcement_date
-            return delta.days
-
-    # Property field for end of software maintenance date progress bar
-    @property
-    def end_of_sw_maintenance_releases_remaining(self):
-        """
-        How many days are remaining. Return None if end_of_sale not defined.
-        """
-        if self.eox_announcement_date and self.end_of_sw_maintenance_releases:
-            delta = self.end_of_sw_maintenance_releases - date.today()
-            return delta.days
-        return None
-
-    # Property field for end of software maintenance date progress bar
-    @property
-    def end_of_sw_maintenance_releases_elapsed(self):
-        """
-        How many days are elaped. Return None if end_of_sale not defined.
-        """
-        if self.eox_announcement_date and self.end_of_sw_maintenance_releases:
-            return self.end_of_sw_maintenance_releases_total - self.end_of_sw_maintenance_releases_remaining
-        return None
-
-    # Property field for end of software maintenance date progress bar
+    #### Property field for end of software maintenance date progress bar
     @property
     def end_of_sw_maintenance_releases_progress(self):
         """
-        Coverage progress in percent. Return None if coverage_end_date not defined.
+        Coverage progress in percent.
         """
         if self.eox_announcement_date and self.end_of_sw_maintenance_releases:
-            return round(
-                self.end_of_sw_maintenance_releases_elapsed / self.end_of_sw_maintenance_releases_total * 100
-            )
+            # Total days until EoX
+            total = self.end_of_sw_maintenance_releases - self.eox_announcement_date
+            total = total.days
+            # How many days are remaining until EoX
+            remaining = self.end_of_sw_maintenance_releases - date.today()
+            remaining = remaining.days
+            # How many days are elaped since EoX announcement
+            elapsed = total - remaining
+            # Return the progress in percent
+            return round(elapsed / total * 100)
         return None
 
-    # Property field for end of software maintenance date progress bar
     @property
     def end_of_sw_maintenance_releases_progress_bar_class(self):
         """
         Coverage progress bar class.
         """
         if self.eox_announcement_date and self.end_of_sw_maintenance_releases:
-            if self.end_of_sw_maintenance_releases_remaining < 60:
+            # How many days are remaining until EoX
+            remaining = self.end_of_sw_maintenance_releases - date.today()
+            remaining = remaining.days
+            # Set the CSS class for the progress bar
+            if remaining < 60:
                 return "bg-danger"
-            if self.end_of_sw_maintenance_releases_remaining < 365:
+            if remaining < 365:
                 return "bg-warning"
         return "bg-success"
 
-    # Property field for end of security vulnerability support date progress bar
-    @property
-    def end_of_security_vul_support_date_total(self):
-        """
-        Total days until EoX. Return None if end_of_sale_date not defined.
-        """
-        if self.eox_announcement_date and self.end_of_security_vul_support_date:
-            delta = self.end_of_security_vul_support_date - self.eox_announcement_date
-            return delta.days
-
-    # Property field for end of security vulnerability support date progress bar
-    @property
-    def end_of_security_vul_support_date_remaining(self):
-        """
-        How many days are remaining. Return None if end_of_sale not defined.
-        """
-        if self.eox_announcement_date and self.end_of_security_vul_support_date:
-            delta = self.end_of_security_vul_support_date - date.today()
-            return delta.days
-        return None
-
-    # Property field for end of security vulnerability support date progress bar
-    @property
-    def end_of_security_vul_support_date_elapsed(self):
-        """
-        How many days are elaped. Return None if end_of_sale not defined.
-        """
-        if self.eox_announcement_date and self.end_of_security_vul_support_date:
-            return (
-                self.end_of_security_vul_support_date_total - self.end_of_security_vul_support_date_remaining
-            )
-        return None
-
-    # Property field for end of security vulnerability support date progress bar
+    #### Property field for end of security vulnerability support date progress bar
     @property
     def end_of_security_vul_support_date_progress(self):
         """
-        Coverage progress in percent. Return None if coverage_end_date not defined.
+        Coverage progress in percent.
         """
         if self.eox_announcement_date and self.end_of_security_vul_support_date:
-            return round(
-                self.end_of_security_vul_support_date_elapsed
-                / self.end_of_security_vul_support_date_total
-                * 100
-            )
+            # Total days until EoX
+            total = self.end_of_security_vul_support_date - self.eox_announcement_date
+            total = total.days
+            # How many days are remaining until EoX
+            remaining = self.end_of_security_vul_support_date - date.today()
+            remaining = remaining.days
+            # How many days are elaped since EoX announcement
+            elapsed = total - remaining
+            # Return the progress in percent
+            return round(elapsed / total * 100)
         return None
 
-    # Property field for end of security vulnerability support date progress bar
     @property
     def end_of_security_vul_support_date_progress_bar_class(self):
         """
         Coverage progress bar class.
         """
         if self.eox_announcement_date and self.end_of_security_vul_support_date:
-            if self.end_of_security_vul_support_date_remaining < 60:
+            # How many days are remaining until EoX
+            remaining = self.end_of_security_vul_support_date - date.today()
+            remaining = remaining.days
+            # Set the CSS class for the progress bar
+            if remaining < 60:
                 return "bg-danger"
-            if self.end_of_security_vul_support_date_remaining < 365:
+            if remaining < 365:
                 return "bg-warning"
         return "bg-success"
 
-    # Property field for end of routine failure analysis date progress bar
-    @property
-    def end_of_routine_failure_analysis_date_total(self):
-        """
-        Total days until EoX. Return None if end_of_sale_date not defined.
-        """
-        if self.eox_announcement_date and self.end_of_routine_failure_analysis_date:
-            delta = self.end_of_routine_failure_analysis_date - self.eox_announcement_date
-            return delta.days
-
-    # Property field for end of routine failure analysis date progress bar
-    @property
-    def end_of_routine_failure_analysis_date_remaining(self):
-        """
-        How many days are remaining. Return None if end_of_sale not defined.
-        """
-        if self.eox_announcement_date and self.end_of_routine_failure_analysis_date:
-            delta = self.end_of_routine_failure_analysis_date - date.today()
-            return delta.days
-        return None
-
-    # Property field for end of routine failure analysis date progress bar
-    @property
-    def end_of_routine_failure_analysis_date_elapsed(self):
-        """
-        How many days are elaped. Return None if end_of_sale not defined.
-        """
-        if self.eox_announcement_date and self.end_of_routine_failure_analysis_date:
-            return (
-                self.end_of_routine_failure_analysis_date_total
-                - self.end_of_routine_failure_analysis_date_remaining
-            )
-        return None
-
-    # Property field for end of routine failure analysis date progress bar
+    #### Property field for end of routine failure analysis date progress bar
     @property
     def end_of_routine_failure_analysis_date_progress(self):
         """
-        Coverage progress in percent. Return None if coverage_end_date not defined.
+        Coverage progress in percent.
         """
         if self.eox_announcement_date and self.end_of_routine_failure_analysis_date:
-            return round(
-                self.end_of_routine_failure_analysis_date_elapsed
-                / self.end_of_routine_failure_analysis_date_total
-                * 100
-            )
+            # Total days until EoX
+            total = self.end_of_routine_failure_analysis_date - self.eox_announcement_date
+            total = total.days
+            # How many days are remaining until EoX
+            remaining = self.end_of_routine_failure_analysis_date - date.today()
+            remaining = remaining.days
+            # How many days are elaped since EoX announcement
+            elapsed = total - remaining
+            # Return the progress in percent
+            return round(elapsed / total * 100)
         return None
 
-    # Property field for end of routine failure analysis date progress bar
     @property
     def end_of_routine_failure_analysis_date_progress_bar_class(self):
         """
         Coverage progress bar class.
         """
         if self.eox_announcement_date and self.end_of_routine_failure_analysis_date:
-            if self.end_of_routine_failure_analysis_date_remaining < 60:
+            # How many days are remaining until EoX
+            remaining = self.end_of_routine_failure_analysis_date - date.today()
+            remaining = remaining.days
+            # Set the CSS class for the progress bar
+            if remaining < 60:
                 return "bg-danger"
-            if self.end_of_routine_failure_analysis_date_remaining < 365:
+            if remaining < 365:
                 return "bg-warning"
         return "bg-success"
 
-    # Property field for end of service contract renewal date progress bar
-    @property
-    def end_of_service_contract_renewal_total(self):
-        """
-        Total days until EoX. Return None if end_of_sale_date not defined.
-        """
-        if self.eox_announcement_date and self.end_of_service_contract_renewal:
-            delta = self.end_of_service_contract_renewal - self.eox_announcement_date
-            return delta.days
-
-    # Property field for end of service contract renewal date progress bar
-    @property
-    def end_of_service_contract_renewal_remaining(self):
-        """
-        How many days are remaining. Return None if end_of_sale not defined.
-        """
-        if self.eox_announcement_date and self.end_of_service_contract_renewal:
-            delta = self.end_of_service_contract_renewal - date.today()
-            return delta.days
-        return None
-
-    # Property field for end of service contract renewal date progress bar
-    @property
-    def end_of_service_contract_renewal_elapsed(self):
-        """
-        How many days are elaped. Return None if end_of_sale not defined.
-        """
-        if self.eox_announcement_date and self.end_of_service_contract_renewal:
-            return self.end_of_service_contract_renewal_total - self.end_of_service_contract_renewal_remaining
-        return None
-
-    # Property field for end of service contract renewal date progress bar
+    #### Property field for end of service contract renewal date progress bar
     @property
     def end_of_service_contract_renewal_progress(self):
         """
-        Coverage progress in percent. Return None if coverage_end_date not defined.
+        Coverage progress in percent.
         """
         if self.eox_announcement_date and self.end_of_service_contract_renewal:
-            return round(
-                self.end_of_service_contract_renewal_elapsed
-                / self.end_of_service_contract_renewal_total
-                * 100
-            )
+            # Total days until EoX
+            total = self.end_of_service_contract_renewal - self.eox_announcement_date
+            total = total.days
+            # How many days are remaining until EoX
+            remaining = self.end_of_service_contract_renewal - date.today()
+            remaining = remaining.days
+            # How many days are elaped since EoX announcement
+            elapsed = total - remaining
+            # Return the progress in percent
+            return round(elapsed / total * 100)
         return None
 
-    # Property field for end of service contract renewal date progress bar
     @property
     def end_of_service_contract_renewal_progress_bar_class(self):
         """
         Coverage progress bar class.
         """
         if self.eox_announcement_date and self.end_of_service_contract_renewal:
-            if self.end_of_service_contract_renewal_remaining < 60:
+            # How many days are remaining until EoX
+            remaining = self.end_of_service_contract_renewal - date.today()
+            remaining = remaining.days
+            # Set the CSS class for the progress bar
+            if remaining < 60:
                 return "bg-danger"
-            if self.end_of_service_contract_renewal_remaining < 365:
+            if remaining < 365:
                 return "bg-warning"
         return "bg-success"
 
-    # Property field for end of svc attach date progress bar
-    @property
-    def end_of_svc_attach_date_total(self):
-        """
-        Total days until EoX. Return None if end_of_sale_date not defined.
-        """
-        if self.eox_announcement_date and self.end_of_svc_attach_date:
-            delta = self.end_of_svc_attach_date - self.eox_announcement_date
-            return delta.days
-
-    # Property field for end of svc attach date progress bar
-    @property
-    def end_of_svc_attach_date_remaining(self):
-        """
-        How many days are remaining. Return None if end_of_sale not defined.
-        """
-        if self.eox_announcement_date and self.end_of_svc_attach_date:
-            delta = self.end_of_svc_attach_date - date.today()
-            return delta.days
-        return None
-
-    # Property field for end of svc attach date progress bar
-    @property
-    def end_of_svc_attach_date_elapsed(self):
-        """
-        How many days are elaped. Return None if end_of_sale not defined.
-        """
-        if self.eox_announcement_date and self.end_of_svc_attach_date:
-            return self.end_of_svc_attach_date_total - self.end_of_svc_attach_date_remaining
-        return None
-
-    # Property field for end of svc attach date progress bar
+    #### Property field for end of svc attach date progress bar
     @property
     def end_of_svc_attach_date_progress(self):
         """
-        Coverage progress in percent. Return None if coverage_end_date not defined.
+        Coverage progress in percent.
         """
         if self.eox_announcement_date and self.end_of_svc_attach_date:
-            return round(self.end_of_svc_attach_date_elapsed / self.end_of_svc_attach_date_total * 100)
+            # Total days until EoX
+            total = self.end_of_svc_attach_date - self.eox_announcement_date
+            total = total.days
+            # How many days are remaining until EoX
+            remaining = self.end_of_svc_attach_date - date.today()
+            remaining = remaining.days
+            # How many days are elaped since EoX announcement
+            elapsed = total - remaining
+            # Return the progress in percent
+            return round(elapsed / total * 100)
         return None
 
-    # Property field for end of svc attach date progress bar
     @property
     def end_of_svc_attach_date_progress_bar_class(self):
         """
         Coverage progress bar class.
         """
         if self.eox_announcement_date and self.end_of_svc_attach_date:
-            if self.end_of_svc_attach_date_remaining < 60:
+            # How many days are remaining until EoX
+            remaining = self.end_of_svc_attach_date - date.today()
+            remaining = remaining.days
+            # Set the CSS class for the progress bar
+            if remaining < 60:
                 return "bg-danger"
-            if self.end_of_svc_attach_date_remaining < 365:
+            if remaining < 365:
                 return "bg-warning"
         return "bg-success"
 
-    # Property field for last day of support progress bar
-    @property
-    def last_date_of_support_total(self):
-        """
-        Total days until EoX. Return None if end_of_sale_date not defined.
-        """
-        if self.eox_announcement_date and self.last_date_of_support:
-            delta = self.last_date_of_support - self.eox_announcement_date
-            return delta.days
-
-    # Property field for last day of support progress bar
-    @property
-    def last_date_of_support_remaining(self):
-        """
-        How many days are remaining. Return None if end_of_sale not defined.
-        """
-        if self.eox_announcement_date and self.last_date_of_support:
-            delta = self.last_date_of_support - date.today()
-            return delta.days
-        return None
-
-    # Property field for last day of support progress bar
-    @property
-    def last_date_of_support_elapsed(self):
-        """
-        How many days are elaped. Return None if end_of_sale not defined.
-        """
-        if self.eox_announcement_date and self.last_date_of_support:
-            return self.last_date_of_support_total - self.last_date_of_support_remaining
-        return None
-
-    # Property field for last day of support progress bar
+    #### Property field for last day of support progress bar
     @property
     def last_date_of_support_progress(self):
         """
-        Coverage progress in percent. Return None if coverage_end_date not defined.
+        Coverage progress in percent.
         """
         if self.eox_announcement_date and self.last_date_of_support:
-            return round(self.last_date_of_support_elapsed / self.last_date_of_support_total * 100)
+            # Total days until EoX
+            total = self.last_date_of_support - self.eox_announcement_date
+            total = total.days
+            # How many days are remaining until EoX
+            remaining = self.last_date_of_support - date.today()
+            remaining = remaining.days
+            # How many days are elaped since EoX announcement
+            elapsed = total - remaining
+            # Return the progress in percent
+            return round(elapsed / total * 100)
         return None
 
-    # Property field for last day of support progress bar
     @property
     def last_date_of_support_progress_bar_class(self):
         """
         Coverage progress bar class.
         """
         if self.eox_announcement_date and self.last_date_of_support:
-            if self.last_date_of_support_remaining < 60:
+            # How many days are remaining until EoX
+            remaining = self.last_date_of_support - date.today()
+            remaining = remaining.days
+            # Set the CSS class for the progress bar
+            if remaining < 60:
                 return "bg-danger"
-            if self.last_date_of_support_remaining < 365:
+            if remaining < 365:
                 return "bg-warning"
         return "bg-success"
 
 
 class CiscoDeviceSupport(ChangeLoggedModel):
     objects = RestrictedQuerySet.as_manager()
 
@@ -622,117 +470,79 @@
     # Field for contracts over a Cisco partner like IBM TLS
     partner_coverage_end_date = models.DateField(
         blank=True, null=True, verbose_name="Partner Coverage End Date"
     )
 
     #### Property Fileds for CiscoDeviceSupport #############################################################
 
-    # Property field for coverage end date progress bar
+    #### Property field for coverage progress bar
     @property
-    def coverage_total(self):
-        """
-        Return 1826 days (5 years) as we cant calculate the total because we don't have the start date.
-        Return None if coverage_end_date not defined.
-        """
-        return 1826 if self.coverage_end_date else None
-
-    # Property field for coverage end date progress bar
-    @property
-    def coverage_remaining(self):
+    def coverage_progress(self):
         """
-        How many coverage days are remaining. Return None if coverage_end_date not defined.
+        Coverage progress in percent.
         """
         if self.coverage_end_date:
-            delta = self.coverage_end_date - date.today()
-            return delta.days
+            # Total days until EoX. 1826 days (5 years) as there is not a start date.
+            total = 1826
+            # How many days are remaining until EoX
+            remaining = self.coverage_end_date - date.today()
+            remaining = remaining.days
+            # How many days are elaped since EoX announcement
+            elapsed = total - remaining
+            # Return the progress in percent
+            return round(elapsed / total * 100)
         return None
 
-    # Property field for coverage end date progress bar
-    @property
-    def coverage_elapsed(self):
-        """
-        How many coverage days are elaped. Return None if coverage_end_date not defined.
-        """
-        return self.coverage_total - self.coverage_remaining if self.coverage_end_date else None
-
-    # Property field for coverage end date progress bar
-    @property
-    def coverage_progress(self):
-        """
-        Coverage progress in percent. Return None if coverage_end_date not defined.
-        """
-        return round(self.coverage_elapsed / self.coverage_total * 100) if self.coverage_end_date else None
-
-    # Property field for coverage end date progress bar
     @property
     def coverage_progress_bar_class(self):
         """
         Coverage progress bar class.
         """
         if self.coverage_end_date:
-            if self.coverage_remaining < 60:
+            # How many days are remaining until EoX
+            remaining = self.coverage_end_date - date.today()
+            remaining = remaining.days
+            # Set the CSS class for the progress bar
+            if remaining < 60:
                 return "bg-danger"
-            if self.coverage_remaining < 365:
+            if remaining < 365:
                 return "bg-warning"
         return "bg-success"
 
-    # Property field for partner coverage end date progress bar
+    #### Property field for partner coverage end date progress bar
     @property
-    def partner_coverage_total(self):
-        """
-        Return 1826 days (5 years) as we cant calculate the total because we don't have the start date.
-        Return None if partner_coverage_end_date not defined.
-        """
-        return 1826 if self.partner_coverage_end_date else None
-
-    # Property field for partner coverage end date progress bar
-    @property
-    def partner_coverage_remaining(self):
+    def partner_coverage_progress(self):
         """
-        How many coverage days are remaining. Return None if partner_coverage_end_date not defined.
+        Coverage progress in percent.
         """
         if self.partner_coverage_end_date:
-            delta = self.partner_coverage_end_date - date.today()
-            return delta.days
+            # Total days until EoX. 1826 days (5 years) as there is not a start date.
+            total = 1826
+            # How many days are remaining until EoX
+            remaining = self.partner_coverage_end_date - date.today()
+            remaining = remaining.days
+            # How many days are elaped since EoX announcement
+            elapsed = total - remaining
+            # Return the progress in percent
+            return round(elapsed / total * 100)
         return None
 
-    # Property field for partner coverage end date progress bar
-    @property
-    def partner_coverage_elapsed(self):
-        """
-        How many coverage days are elaped. Return None if partner_coverage_end_date not defined.
-        """
-        return (
-            self.partner_coverage_total - self.partner_coverage_remaining
-            if self.partner_coverage_end_date
-            else None
-        )
-
-    # Property field for partner coverage end date progress bar
-    @property
-    def partner_coverage_progress(self):
-        """
-        Coverage progress in percent. Return None if partner_coverage_end_date not defined.
-        """
-        return (
-            round(self.partner_coverage_elapsed / self.partner_coverage_total * 100)
-            if self.partner_coverage_end_date
-            else None
-        )
-
-    # Property field for partner coverage end date progress bar
     @property
     def partner_coverage_progress_bar_class(self):
         """
         Coverage progress bar class.
         """
         if self.partner_coverage_end_date:
-            if self.partner_coverage_remaining < 60:
+            # How many days are remaining until EoX
+            remaining = self.partner_coverage_end_date - date.today()
+            remaining = remaining.days
+            # Set the CSS class for the progress bar
+            if remaining < 60:
                 return "bg-danger"
-            if self.partner_coverage_remaining < 365:
+            if remaining < 365:
                 return "bg-warning"
         return "bg-success"
 
     #### Fileds same as CiscoDeviceTypeSupport ##############################################################
     # Create these fields again because referencing them from the CiscoDeviceTypeSupport model was not working
 
     # Field get set in custom save() function
@@ -826,22 +636,148 @@
 
     # Field get set in custom save() function
     serial = models.CharField(max_length=100, blank=True, null=True, verbose_name="Serial")
 
     # Field get set in custom save() function
     pid = models.CharField(max_length=100, blank=True, null=True, verbose_name="PID")
 
-    #### Fileds for FortinetDeviceSupport #########################################################################
+    #### Fileds for FortinetDeviceSupport ###################################################################
 
     recommended_release = models.TextField(
         max_length=100, blank=True, null=True, verbose_name="Recommended Release"
     )
 
     desired_release = models.CharField(max_length=100, blank=True, null=True, verbose_name="Desired Release")
 
     current_release = models.CharField(max_length=100, blank=True, null=True, verbose_name="Current Release")
 
     # Field get set in custom save() function
     desired_release_status = models.BooleanField(default=False, verbose_name="Desired Rel. Status")
 
     # Field get set in custom save() function
     current_release_status = models.BooleanField(default=False, verbose_name="Current Rel. Status")
+
+    partner = models.CharField(max_length=100, blank=True, null=True, verbose_name="Partner")
+
+    end_of_renewal_date = models.DateField(blank=True, null=True, verbose_name="End of Renewal Date")
+
+    end_of_support_date = models.DateField(blank=True, null=True, verbose_name="End of Support Date")
+
+    #### Property field for end of renewal date progress bar
+
+    @property
+    def end_of_renewal_progress(self):
+        """
+        Coverage progress in percent.
+        """
+        if self.end_of_renewal_date:
+            # Total days until EoX. 365 days (1 years) as there is not a start date.
+            # EoR is normaly 60-90 days in advance announced.
+            total = 365
+            # How many days are remaining until EoX
+            remaining = self.end_of_renewal_date - date.today()
+            remaining = remaining.days
+            # How many days are elaped since EoX announcement
+            elapsed = total - remaining
+            # Return the progress in percent
+            return round(elapsed / total * 100)
+        return None
+
+    @property
+    def end_of_renewal_progress_bar_class(self):
+        """
+        Coverage progress bar class.
+        """
+        if self.end_of_renewal_date:
+            # How many days are remaining until EoX
+            remaining = self.end_of_renewal_date - date.today()
+            remaining = remaining.days
+            # Set the CSS class for the progress bar
+            if remaining < 60:
+                return "bg-danger"
+            if remaining < 365:
+                return "bg-warning"
+        return "bg-success"
+
+    #### Property field for end of support date progress bar
+
+    @property
+    def end_of_support_progress(self):
+        """
+        Coverage progress in percent.
+        """
+        if self.end_of_support_date:
+            # Total days until EoX. 1826 days (5 years) as there is not a start date.
+            # EoS is normaly 5 years after the EoR date.
+            total = 1826
+            # How many days are remaining until EoX
+            remaining = self.end_of_support_date - date.today()
+            remaining = remaining.days
+            # How many days are elaped since EoX announcement
+            elapsed = total - remaining
+            # Return the progress in percent
+            return round(elapsed / total * 100)
+        return None
+
+    @property
+    def end_of_support_progress_bar_class(self):
+        """
+        Coverage progress bar class.
+        """
+        if self.end_of_support_date:
+            # How many days are remaining until EoX
+            remaining = self.end_of_support_date - date.today()
+            remaining = remaining.days
+            # Set the CSS class for the progress bar
+            if remaining < 60:
+                return "bg-danger"
+            if remaining < 365:
+                return "bg-warning"
+        return "bg-success"
+
+
+#### PureStorage Support ####################################################################################
+
+
+class PureStorageDeviceSupport(ChangeLoggedModel):
+    objects = RestrictedQuerySet.as_manager()
+
+    device = models.OneToOneField(to="dcim.Device", on_delete=models.CASCADE, verbose_name="Device")
+
+    def __str__(self):
+        return f"{self.device}"
+
+    def get_absolute_url(self):
+        return reverse("plugins:netbox_device_support_plugin:purestoragedevicesupport_list")
+
+    def save(self, *args, **kwargs):
+        # Query the Device model
+        device_obj = Device.objects.select_related().get(id=self.device.id)
+        # Set the name from the Device name
+        self.name = device_obj.name
+        # Set the pid from the Device serial
+        self.serial = device_obj.serial
+
+        # Query the DeviceType model
+        device_type_obj = DeviceType.objects.select_related().get(id=self.device.device_type.id)
+        # Set the pid from the DeviceType part_number
+        self.pid = device_type_obj.part_number
+
+        # Call the "real" save() method.
+        super().save(*args, **kwargs)
+
+    #### Fileds overwritten by custom save() function #######################################################
+
+    # Field get set in custom save() function
+    name = models.CharField(max_length=100, blank=True, null=True, verbose_name="Name")
+
+    # Field get set in custom save() function
+    serial = models.CharField(max_length=100, blank=True, null=True, verbose_name="Serial")
+
+    # Field get set in custom save() function
+    pid = models.CharField(max_length=100, blank=True, null=True, verbose_name="PID")
+
+    #### Fileds for PureStorageDeviceSupport ################################################################
+
+    desired_release = models.CharField(max_length=100, blank=True, null=True, verbose_name="Desired Release")
+
+    current_release = models.CharField(max_length=100, blank=True, null=True, verbose_name="Current Release")
```

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/navigation.py` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/navigation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,23 @@
-from extras.plugins import PluginMenuItem
+from netbox.plugins import PluginMenuItem
 
 menu_items = (
     # Cisco Support
     PluginMenuItem(
-        link="plugins:netbox_device_support_plugin:ciscodevicesupport_list", link_text="Cisco Device Support"
+        link="plugins:netbox_device_support_plugin:ciscodevicesupport_list",
+        link_text="Cisco Device Support",
     ),
     PluginMenuItem(
         link="plugins:netbox_device_support_plugin:ciscodevicetypesupport_list",
         link_text="Cisco Device Type Support",
     ),
     # Fortnet Support
     PluginMenuItem(
-        link="plugins:netbox_device_support_plugin:fortinetdevicesupport_list", link_text="Fortinet Device Support"
+        link="plugins:netbox_device_support_plugin:fortinetdevicesupport_list",
+        link_text="Fortinet Device Support",
+    ),
+    # PureStorage Support
+    PluginMenuItem(
+        link="plugins:netbox_device_support_plugin:purestoragedevicesupport_list",
+        link_text="PureStorage Device Support",
     ),
 )
```

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/tables.py` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/tables.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import django_tables2 as tables
 from django.utils.translation import gettext as _
 
 from netbox.tables import NetBoxTable, columns
-from .models import CiscoDeviceSupport, CiscoDeviceTypeSupport, FortinetDeviceSupport
+from .models import (
+    CiscoDeviceSupport,
+    CiscoDeviceTypeSupport,
+    FortinetDeviceSupport,
+    PureStorageDeviceSupport,
+)
 
 
 #### Cisco Support ##########################################################################################
 
 
 class CiscoDeviceSupportTable(NetBoxTable):
     id = tables.Column(linkify=False)
@@ -104,14 +109,37 @@
     actions = columns.ActionsColumn(actions=("delete",))
 
     class Meta(NetBoxTable.Meta):
         model = FortinetDeviceSupport
         # fmt: off
         fields = (
             "pk", "id", "device", "pid", "serial", "recommended_release", "desired_release", "current_release",
-            "desired_release_status", "current_release_status"
+            "desired_release_status", "current_release_status", "partner", "end_of_renewal_date",
+            "end_of_support_date",
         )
         default_columns = (
             "device", "desired_release_status", "desired_release", "current_release_status",
-            "current_release"
+            "current_release", "end_of_renewal_date", "end_of_support_date",
+        )
+        # fmt: on
+
+
+#### PureStorage Support ####################################################################################
+
+
+class PureStorageDeviceSupportTable(NetBoxTable):
+    id = tables.Column(linkify=False)
+
+    device = tables.Column(linkify=True)
+
+    actions = columns.ActionsColumn(actions=("delete",))
+
+    class Meta(NetBoxTable.Meta):
+        model = PureStorageDeviceSupport
+        # fmt: off
+        fields = (
+            "pk", "id", "device", "pid", "serial", "desired_release", "current_release",
+        )
+        default_columns = (
+            "device", "desired_release", "current_release",
         )
         # fmt: on
```

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/template_content.py` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/template_content.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from datetime import datetime
 
 from django.shortcuts import get_object_or_404
 from django.conf import settings
-from extras.plugins import PluginTemplateExtension
-from .models import CiscoDeviceTypeSupport, CiscoDeviceSupport, FortinetDeviceSupport
+from netbox.plugins import PluginTemplateExtension
+from .models import (
+    CiscoDeviceTypeSupport,
+    CiscoDeviceSupport,
+    FortinetDeviceSupport,
+    PureStorageDeviceSupport,
+)
 
 
 PLUGIN_SETTINGS = settings.PLUGINS_CONFIG.get("netbox_device_support_plugin", dict())
 TEMPLATE_EXTENSION_PLACEMENT = PLUGIN_SETTINGS.get("TEMPLATE_EXTENSION_PLACEMENT", "right")
 
 
 #### Cisco Support ##########################################################################################
@@ -126,15 +131,51 @@
 
         return self.render(
             "fortinet/fortinet_device_support.html",
             {"fortinet_device_support": fortinet_device_support},
         )
 
 
+#### PureStorage Support ####################################################################################
+
+
+class PureStorageDeviceSupportInformation(PluginTemplateExtension):
+    model = "dcim.device"
+
+    if TEMPLATE_EXTENSION_PLACEMENT == "left":
+
+        def left_page(self):
+            try:
+                purestorage_device_support = PureStorageDeviceSupport.objects.get(
+                    device=self.context["object"]
+                )
+            except PureStorageDeviceSupport.DoesNotExist:
+                print("No PureStorage Device Support Entry found")
+                purestorage_device_support = None
+
+            return self.render(
+                "purestorage/purestorage_device_support.html",
+                {"purestorage_device_support": purestorage_device_support},
+            )
+
+    def right_page(self):
+        try:
+            purestorage_device_support = PureStorageDeviceSupport.objects.get(device=self.context["object"])
+        except PureStorageDeviceSupport.DoesNotExist:
+            print("No PureStorage Device Support Entry found")
+            purestorage_device_support = None
+
+        return self.render(
+            "purestorage/purestorage_device_support.html",
+            {"purestorage_device_support": purestorage_device_support},
+        )
+
+
 #### Template Extensions ####################################################################################
 
 # Template extensions to be loaded when the plugin is loaded
 template_extensions = [
     CiscoDeviceTypeSupportInformation,
     CiscoDeviceSupportInformation,
     FortinetDeviceSupportInformation,
+    PureStorageDeviceSupportInformation,
 ]
```

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/cisco_device_support.html` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/cisco_device_support.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,105 @@
 {% load filters %}
 
 {% if cisco_device_support %}
     <div class="card">
         <h5 class="card-header">Cisco Software Release</h5>
-        <div class="card-body">
-            <table class="table table-hover panel-body attr-table">
-                <tbody>
-                    <tr {{ cisco_device_support.recommended_release|coverage_class }} >
-                        <td style="width: 40%">Recommended Release</td>
-                        <td colspan="2">{{ cisco_device_support.recommended_release|linebreaks }}</td>
-                    </tr>
-                    {% if "PID without Cisco software" in cisco_device_support.recommended_release %}
-                        {# Comment: If PID have no Cisco software omit the desired and current release #}
-                    {% else %}
-                        <tr {{ cisco_device_support.desired_release_status|desired_release_status_class }}>
-                            <td>Desired Release</td>
-                            <td style="width: 40px"><i {{ cisco_device_support.desired_release_status|coverage_class_boolian }}></i></td>
-                            <td>{{ cisco_device_support.desired_release }}</td>
-                        </tr>
-                        <tr {{ cisco_device_support.current_release_status|current_release_status_class }}>
-                            <td>Current Release</td>
-                            <td style="width: 40px"><i {{ cisco_device_support.current_release_status|coverage_class_boolian }}></i></td>
-                            <td>{{ cisco_device_support.current_release }}</td>
-                        </tr>
-                    {% endif %}
-                </tbody>
-            </table>
-            <div class="text-muted">Last updated: {{ cisco_device_support.last_updated }}</div>
-        </div>
+        <table class="table table-hover panel-body attr-table">
+            <tbody>
+                <tr {{ cisco_device_support.recommended_release|coverage_class }} >
+                    <td style="width: 40%">Recommended Release</td>
+                    <td colspan="2">{{ cisco_device_support.recommended_release|linebreaksbr|placeholder }}</td>
+                </tr>
+                {% if "PID without Cisco software" in cisco_device_support.recommended_release %}
+                    {# Comment: If PID have no Cisco software omit the desired and current release #}
+                {% else %}
+                    <tr {{ cisco_device_support.desired_release_status|desired_release_status_class }}>
+                        <td>Desired Release</td>
+                        <td style="width: 40px"><i {{ cisco_device_support.desired_release_status|coverage_class_boolian }}></i></td>
+                        <td>{{ cisco_device_support.desired_release|placeholder }}</td>
+                    </tr>
+                    <tr {{ cisco_device_support.current_release_status|current_release_status_class }}>
+                        <td>Current Release</td>
+                        <td style="width: 40px"><i {{ cisco_device_support.current_release_status|coverage_class_boolian }}></i></td>
+                        <td>{{ cisco_device_support.current_release|placeholder }}</td>
+                    </tr>
+                {% endif %}
+            </tbody>
+        </table>
+        <div class="text-muted">Last updated: {{ cisco_device_support.last_updated }}</div>
     </div>
     <div class="card">
-        <div class="card-body">
-            <h5 class="card-header" style="padding:0px 0px 16px 0px">Cisco Device Support</h5>
+        <h5 class="card-header" style="padding:0px 0px 16px 0px">Cisco Device Support</h5>
+        <table class="table table-hover panel-body attr-table">
+            <tbody>
+                <tr {{ cisco_device_support.sr_no_owner|coverage_class }}>
+                    <td style="width: 40%">Is associated with a Cisco ID</td>
+                    <td style="width: 40px"><i {{ cisco_device_support.sr_no_owner|coverage_class_boolian }}></i></td>
+                    <td>{{ cisco_device_support.api_status|placeholder }}</td>
+                </tr>
+                <tr {{ cisco_device_support.contract_supplier|coverage_class }}>
+                    <td>Contract Status</td>
+                    <td><i {{ cisco_device_support.contract_supplier|coverage_class_boolian }}></i></td>
+                    <td>{{ cisco_device_support.contract_supplier|contract_supplier_text|placeholder }}</td>
+                </tr>
+                <tr {{ cisco_device_support.is_covered|coverage_class }}>
+                    <td>Is under Cisco Support?</td>
+                    <td colspan="2"><i {{ cisco_device_support.is_covered|coverage_class_boolian }}></i></td>
+                </tr>
+                <tr {{ cisco_device_support.coverage_end_date|expiration_class }}>
+                    <td>Contract Coverage End Date</td>
+                    <td colspan="2">
+                        {{ cisco_device_support.coverage_end_date|placeholder }}<br>
+                        {% include "cisco/inc/device_contract_coverage_bar.html" %}
+                    </td>
+                </tr>
+                <tr {{ cisco_device_support.service_line_descr|coverage_class }}>
+                    <td>Service Level Description</td>
+                    <td colspan="2">{{ cisco_device_support.service_line_descr|placeholder }}</td>
+                </tr>
+                <tr {{ cisco_device_support.service_contract_number|coverage_class }}>
+                    <td>Service Contract Number</td>
+                    <td colspan="2">{{ cisco_device_support.service_contract_number|placeholder }}</td>
+                </tr>
+                <tr {{ cisco_device_support.warranty_end_date|coverage_class }}>
+                    <td>Warranty End Date</td>
+                    <td colspan="2">{{ cisco_device_support.warranty_end_date|placeholder }}</td>
+                </tr>
+                <tr {{ cisco_device_support.warranty_type|coverage_class }}>
+                    <td>Warranty Type</td>
+                    <td colspan="2">{{ cisco_device_support.warranty_type|placeholder }}</td>
+                </tr>
+            </tbody>
+        </table>
+        {% if not cisco_device_support.contract_supplier or "Cisco SNTC" in cisco_device_support.contract_supplier or "Not covered" in cisco_device_support.contract_supplier %}
+            {# Comment: Omit the partner support contract table #}
+        {% else %}
+            <h5 class="card-header" style="padding:16px 0px 16px 0px">{{ cisco_device_support.contract_supplier }} Device Support</h5>
             <table class="table table-hover panel-body attr-table">
                 <tbody>
-                    <tr {{ cisco_device_support.sr_no_owner|coverage_class }}>
-                        <td style="width: 40%">Is associated with a Cisco ID</td>
-                        <td style="width: 40px"><i {{ cisco_device_support.sr_no_owner|coverage_class_boolian }}></i></td>
-                        <td>{{ cisco_device_support.api_status }}</td>
-                    </tr>
-                    <tr {{ cisco_device_support.contract_supplier|coverage_class }}>
-                        <td>Contract Status</td>
-                        <td><i {{ cisco_device_support.contract_supplier|coverage_class_boolian }}></i></td>
-                        <td>{{ cisco_device_support.contract_supplier|contract_supplier_text }}</td>
-                    </tr>
-                    <tr {{ cisco_device_support.is_covered|coverage_class }}>
-                        <td>Is under Cisco Support?</td>
-                        <td colspan="2"><i {{ cisco_device_support.is_covered|coverage_class_boolian }}></i></td>
+                    <tr {{ cisco_device_support.partner_status|coverage_class }}>
+                        <td style="width: 40%">Contract Status</td>
+                        <td>{{ cisco_device_support.partner_status|placeholder }}</td>
                     </tr>
-                    <tr {{ cisco_device_support.coverage_end_date|expiration_class }}>
+                    <tr {{ cisco_device_support.partner_coverage_end_date|expiration_class }}>
                         <td>Contract Coverage End Date</td>
-                        <td colspan="2">
-                            {{ cisco_device_support.coverage_end_date }}<br>
-                            {% include "cisco/inc/device_contract_coverage_bar.html" %}
+                        <td>
+                            {{ cisco_device_support.partner_coverage_end_date|placeholder }}<br>
+                            {% include "cisco/inc/device_partner_contract_coverage_bar.html" %}
                         </td>
                     </tr>
-                    <tr {{ cisco_device_support.service_line_descr|coverage_class }}>
+                    <tr {{ cisco_device_support.partner_service_level|coverage_class }}>
                         <td>Service Level Description</td>
-                        <td colspan="2">{{ cisco_device_support.service_line_descr }}</td>
+                        <td>{{ cisco_device_support.partner_service_level|placeholder }}</td>
                     </tr>
-                    <tr {{ cisco_device_support.service_contract_number|coverage_class }}>
-                        <td>Service Contract Number</td>
-                        <td colspan="2">{{ cisco_device_support.service_contract_number }}</td>
-                    </tr>
-                    <tr {{ cisco_device_support.warranty_end_date|coverage_class }}>
-                        <td>Warranty End Date</td>
-                        <td colspan="2">{{ cisco_device_support.warranty_end_date }}</td>
-                    </tr>
-                    <tr {{ cisco_device_support.warranty_type|coverage_class }}>
-                        <td>Warranty Type</td>
-                        <td colspan="2">{{ cisco_device_support.warranty_type }}</td>
+                    <tr {{ cisco_device_support.partner_customer_number|coverage_class }}>
+                        <td>Customer Number</td>
+                        <td>{{ cisco_device_support.partner_customer_number|placeholder }}</td>
                     </tr>
                 </tbody>
             </table>
-            {% if not cisco_device_support.contract_supplier or "Cisco SNTC" in cisco_device_support.contract_supplier or "Not covered" in cisco_device_support.contract_supplier %}
-                {# Comment: Omit the partner support contract table #}
-            {% else %}
-                <h5 class="card-header" style="padding:16px 0px 16px 0px">{{ cisco_device_support.contract_supplier }} Device Support</h5>
-                <table class="table table-hover panel-body attr-table">
-                    <tbody>
-                        <tr {{ cisco_device_support.partner_status|coverage_class }}>
-                            <td style="width: 40%">Contract Status</td>
-                            <td>{{ cisco_device_support.partner_status }}</td>
-                        </tr>
-                        <tr {{ cisco_device_support.partner_coverage_end_date|expiration_class }}>
-                            <td>Contract Coverage End Date</td>
-                            <td>
-                                {{ cisco_device_support.partner_coverage_end_date }}<br>
-                                {% include "cisco/inc/device_partner_contract_coverage_bar.html" %}
-                            </td>
-                        </tr>
-                        <tr {{ cisco_device_support.partner_service_level|coverage_class }}>
-                            <td>Service Level Description</td>
-                            <td>{{ cisco_device_support.partner_service_level }}</td>
-                        </tr>
-                        <tr {{ cisco_device_support.partner_customer_number|coverage_class }}>
-                            <td>Customer Number</td>
-                            <td>{{ cisco_device_support.partner_customer_number }}</td>
-                        </tr>
-                    </tbody>
-                </table>
-            {% endif %}
-            <div class="text-muted">Last updated: {{ cisco_device_support.last_updated }}</div>
-        </div>
+        {% endif %}
+        <div class="text-muted">Last updated: {{ cisco_device_support.last_updated }}</div>
     </div>
-{% else %}
-    {# No cisco_device_support information available #}
 {% endif %}
 
 {% include "cisco/cisco_device_type_support.html" %}
```

#### html2text {}

```diff
@@ -5,9 +5,8 @@
 {% if not cisco_device_support.contract_supplier or "Cisco SNTC" in
 cisco_device_support.contract_supplier or "Not covered" in
 cisco_device_support.contract_supplier %} {# Comment: Omit the partner support
 contract table #} {% else %}
 **** {{{{ cciissccoo__ddeevviiccee__ssuuppppoorrtt..ccoonnttrraacctt__ssuupppplliieerr }}}} DDeevviiccee SSuuppppoorrtt ****
 {% endif %}
 Last updated: {{ cisco_device_support.last_updated }}
-{% else %} {# No cisco_device_support information available #} {% endif %} {%
-include "cisco/cisco_device_type_support.html" %}
+{% endif %} {% include "cisco/cisco_device_type_support.html" %}
```

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,73 @@
 {% load filters %}
 
 {% if cisco_device_type_support %}
     <div class="card">
         <h5 class="card-header">Cisco Device Type Support</h5>
-        <div class="card-body">
-            <table class="table table-hover panel-body attr-table">
-                <tbody>
-                    {% if cisco_device_type_support.eox_announcement_date %}
-                        <tr {{ cisco_device_type_support.eox_announcement_date|expiration_class }}>
-                            <td style="width: 45%">EoX Announcement Date</td>
-                            <td>{{ cisco_device_type_support.eox_announcement_date }}</td>
-                        </tr>
-                        <tr {{ cisco_device_type_support.end_of_sale_date|expiration_class }}>
-                            <td>End-of-Sale Date</td>
-                            <td>
-                                {{ cisco_device_type_support.end_of_sale_date }}<br>
-                                {% include "cisco/inc/device_type_eos_bar.html" %}
-                            </td>
-                        </tr>
-                        <tr {{ cisco_device_type_support.end_of_sw_maintenance_releases|expiration_class }}>
-                            <td>End of SW Maintenance Releases Date</td>
-                            <td>
-                                {{ cisco_device_type_support.end_of_sw_maintenance_releases }}<br>
-                                {% include "cisco/inc/device_type_eosm_bar.html" %}
-                            </td>
-                        </tr>
-                        <tr {{ cisco_device_type_support.end_of_routine_failure_analysis_date|expiration_class }}>
-                            <td>End of Routine Failure Analysis Date</td>
-                            <td>
-                                {{ cisco_device_type_support.end_of_routine_failure_analysis_date }}<br>
-                                {% include "cisco/inc/device_type_eorfa_bar.html" %}
-                            </td>
-                        </tr>
-                        <tr {{ cisco_device_type_support.end_of_svc_attach_date|expiration_class }}>
-                            <td>End of New Service Attachment Date</td>
-                            <td>
-                                {{ cisco_device_type_support.end_of_svc_attach_date }}<br>
-                                {% include "cisco/inc/device_type_eosvca_bar.html" %}
-                            </td>
-                        </tr>
-                        <tr {{ cisco_device_type_support.end_of_service_contract_renewal|expiration_class }}>
-                            <td>End of Service Contract Renewal Date</td>
-                            <td>
-                                {{ cisco_device_type_support.end_of_service_contract_renewal }}<br>
-                                {% include "cisco/inc/device_type_eoscr_bar.html" %}
-                            </td>
-                        </tr>
-                        <tr {{ cisco_device_type_support.end_of_security_vul_support_date|expiration_class }}>
-                            <td>End of Vulnerability/Security Support</td>
-                            <td>
-                                {{ cisco_device_type_support.end_of_security_vul_support_date }}<br>
-                                {% include "cisco/inc/device_type_eosvs_bar.html" %}
-                            </td>
-                        </tr>
-                        <tr {{ cisco_device_type_support.last_date_of_support|expiration_class }}>
-                            <td>Last Date of Support</td>
-                            <td>
-                                {{ cisco_device_type_support.last_date_of_support }}<br>
-                                {% include "cisco/inc/device_type_last_day_support_bar.html" %}
-                            </td>
-                        </tr>
-                    {% else %}
-                        <tr {{ cisco_device_type_support.eox_has_error|eox_class }}>
-                            <td style="width: 40%">EoX Status</td>
-                            <td style="width: 40px"><i {{ cisco_device_type_support.eox_has_error|eox_class_boolian }}></i></td>
-                            <td>{{ cisco_device_type_support.eox_error }}</td>
-                        </tr>
-                    {% endif %}
-                </tbody>
-            </table>
-            <div class="text-muted">Last updated: {{ cisco_device_type_support.last_updated }}</div>
-        </div>
+        <table class="table table-hover panel-body attr-table">
+            <tbody>
+                {% if cisco_device_type_support.eox_announcement_date %}
+                    <tr {{ cisco_device_type_support.eox_announcement_date|expiration_class }}>
+                        <td style="width: 45%">EoX Announcement Date</td>
+                        <td>{{ cisco_device_type_support.eox_announcement_date|placeholder }}</td>
+                    </tr>
+                    <tr {{ cisco_device_type_support.end_of_sale_date|expiration_class }}>
+                        <td>End-of-Sale Date</td>
+                        <td>
+                            {{ cisco_device_type_support.end_of_sale_date|placeholder }}<br>
+                            {% include "cisco/inc/device_type_eos_bar.html" %}
+                        </td>
+                    </tr>
+                    <tr {{ cisco_device_type_support.end_of_sw_maintenance_releases|expiration_class }}>
+                        <td>End of SW Maintenance Releases Date</td>
+                        <td>
+                            {{ cisco_device_type_support.end_of_sw_maintenance_releases|placeholder }}<br>
+                            {% include "cisco/inc/device_type_eosm_bar.html" %}
+                        </td>
+                    </tr>
+                    <tr {{ cisco_device_type_support.end_of_routine_failure_analysis_date|expiration_class }}>
+                        <td>End of Routine Failure Analysis Date</td>
+                        <td>
+                            {{ cisco_device_type_support.end_of_routine_failure_analysis_date|placeholder }}<br>
+                            {% include "cisco/inc/device_type_eorfa_bar.html" %}
+                        </td>
+                    </tr>
+                    <tr {{ cisco_device_type_support.end_of_svc_attach_date|expiration_class }}>
+                        <td>End of New Service Attachment Date</td>
+                        <td>
+                            {{ cisco_device_type_support.end_of_svc_attach_date|placeholder }}<br>
+                            {% include "cisco/inc/device_type_eosvca_bar.html" %}
+                        </td>
+                    </tr>
+                    <tr {{ cisco_device_type_support.end_of_service_contract_renewal|expiration_class }}>
+                        <td>End of Service Contract Renewal Date</td>
+                        <td>
+                            {{ cisco_device_type_support.end_of_service_contract_renewal|placeholder }}<br>
+                            {% include "cisco/inc/device_type_eoscr_bar.html" %}
+                        </td>
+                    </tr>
+                    <tr {{ cisco_device_type_support.end_of_security_vul_support_date|expiration_class }}>
+                        <td>End of Vulnerability/Security Support</td>
+                        <td>
+                            {{ cisco_device_type_support.end_of_security_vul_support_date|placeholder }}<br>
+                            {% include "cisco/inc/device_type_eosvs_bar.html" %}
+                        </td>
+                    </tr>
+                    <tr {{ cisco_device_type_support.last_date_of_support|expiration_class }}>
+                        <td>Last Date of Support</td>
+                        <td>
+                            {{ cisco_device_type_support.last_date_of_support|placeholder }}<br>
+                            {% include "cisco/inc/device_type_last_day_support_bar.html" %}
+                        </td>
+                    </tr>
+                {% else %}
+                    <tr {{ cisco_device_type_support.eox_has_error|eox_class }}>
+                        <td style="width: 40%">EoX Status</td>
+                        <td style="width: 40px"><i {{ cisco_device_type_support.eox_has_error|eox_class_boolian }}></i></td>
+                        <td>{{ cisco_device_type_support.eox_error }}</td>
+                    </tr>
+                {% endif %}
+            </tbody>
+        </table>
+        <div class="text-muted">Last updated: {{ cisco_device_type_support.last_updated }}</div>
     </div>
-{% else %}
-    {# No cisco_device_type_support information available #}
 {% endif %}
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
 {% load filters %} {% if cisco_device_type_support %}
 **** CCiissccoo DDeevviiccee TTyyppee SSuuppppoorrtt ****
 Last updated: {{ cisco_device_type_support.last_updated }}
-{% else %} {# No cisco_device_type_support information available #} {% endif %}
+{% endif %}
```

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,91 @@
 {% load filters %}
 
 {% if fortinet_device_support %}
     <div class="card">
         <h5 class="card-header">Fortinet Software Release</h5>
-        <div class="card-body">
-            <table class="table table-hover panel-body attr-table">
-                <tbody>
-                    <tr {{ fortinet_device_support.recommended_release|coverage_class }} >
-                        <td style="width: 40%">Recommended Release</td>
-                        <td colspan="2">{{ fortinet_device_support.recommended_release|linebreaks }}</td>
-                    </tr>
-                    <tr {{ fortinet_device_support.desired_release_status|desired_release_status_class }}>
-                        <td>Desired Release</td>
-                        <td style="width: 40px"><i {{ fortinet_device_support.desired_release_status|coverage_class_boolian }}></i></td>
-                        <td>{{ fortinet_device_support.desired_release }}</td>
-                    </tr>
-                    <tr {{ fortinet_device_support.current_release_status|current_release_status_class }}>
-                        <td>Current Release</td>
-                        <td style="width: 40px"><i {{ fortinet_device_support.current_release_status|coverage_class_boolian }}></i></td>
-                        <td>{{ fortinet_device_support.current_release }}</td>
-                    </tr>
-                </tbody>
-            </table>
-            <div class="text-muted">Last updated: {{ fortinet_device_support.last_updated }}</div>
-        </div>
+        <table class="table table-hover panel-body attr-table">
+            <tbody>
+                <tr {{ fortinet_device_support.recommended_release|coverage_class }} >
+                    <td style="width: 40%">Recommended Release</td>
+                    <td colspan="2">{{ fortinet_device_support.recommended_release|linebreaksbr|placeholder }}</td>
+                </tr>
+                <tr {{ fortinet_device_support.desired_release_status|desired_release_status_class }}>
+                    <td>Desired Release</td>
+                    <td style="width: 40px"><i {{ fortinet_device_support.desired_release_status|coverage_class_boolian }}></i></td>
+                    <td>{{ fortinet_device_support.desired_release|placeholder }}</td>
+                </tr>
+                <tr {{ fortinet_device_support.current_release_status|current_release_status_class }}>
+                    <td>Current Release</td>
+                    <td style="width: 40px"><i {{ fortinet_device_support.current_release_status|coverage_class_boolian }}></i></td>
+                    <td>{{ fortinet_device_support.current_release|placeholder }}</td>
+                </tr>
+            </tbody>
+        </table>
+        <div class="text-muted">Last updated: {{ fortinet_device_support.last_updated }}</div>
     </div>
     <div class="card">
         <h5 class="card-header">Fortinet License Coverage</h5>
-        <div class="card-body">
-            <table class="table table-hover panel-body attr-table">
-                <tbody>
-                    <tr>
-                        <td style="width: 40%">'License Description'<br>'(License Type)'</td>
-                        <td>'Expiration Date'<br>'Expiration Bar'</td>
-                    </tr>
-                    <tr>
-                        <td>'License Description'<br>'(License Type)'</td>
-                        <td>'Expiration Date'<br>'Expiration Bar'</td>
-                    </tr>
-                    <tr>
-                        <td>'License Description'<br>'(License Type)'</td>
-                        <td>'Expiration Date'<br>'Expiration Bar'</td>
-                    </tr>
-                    <tr>
-                        <td>'License Description'<br>'(License Type)'</td>
-                        <td>'Expiration Date'<br>'Expiration Bar'</td>
-                    </tr>
-                </tbody>
-            </table>
-            <div class="text-muted">Last updated: {{ fortinet_device_support.last_updated }}</div>
-        </div>
+        <table class="table table-hover panel-body attr-table">
+            <tbody>
+                <tr>
+                    <td colspan="2" class="text-center text-muted">— Not implemented yet —</td>
+                </tr>
+                <tr>
+                    <td style="width: 40%" class="text-muted">
+                        'License Description'<br>
+                        '(License Type)'
+                    </td>
+                    <td class="text-muted">
+                        'Expiration Date'<br>
+                        'Expiration Bar'
+                    </td>
+                </tr>
+            </tbody>
+        </table>
+        <div class="text-muted">Last updated: {{ fortinet_device_support.last_updated }}</div>
     </div>
     <div class="card">
         <h5 class="card-header">Fortinet Device Support</h5>
-        <div class="card-body">
-            <table class="table table-hover panel-body attr-table">
-                <tbody>
-                    <tr>
-                        <td style="width: 40%">Partner</td>
-                        <td>Not implemented yet ...</td>
-                    </tr>
-                    <tr>
-                        <td>End of Renewal Date</td>
-                        <td>Not implemented yet ...</td>
-                    </tr>
-                    <tr>
-                        <td>End of Support Date</td>
-                        <td>Not implemented yet ...</td>
-                    </tr>
-                </tbody>
-            </table>
-            <h6 class="card-header" style="padding:16px 0px 16px 0px">Support Entitlements</h6>
-            <table class="table table-hover panel-body attr-table">
-                <tbody>
-                    <tr>
-                        <td style="width: 40%">'Support Description'<br>'(Support Level)'</td>
-                        <td>'Expiration Date'<br>'Expiration Bar'</td>
-                    </tr>
-                    <tr>
-                        <td>'Support Description'<br>'(Support Level)'</td>
-                        <td>'Expiration Date'<br>'Expiration Bar'</td>
-                    </tr>
-                    <tr>
-                        <td>'Support Description'<br>'(Support Level)'</td>
-                        <td>'Expiration Date'<br>'Expiration Bar'</td>
-                    </tr>
-                    <tr>
-                        <td>'Support Description'<br>'(Support Level)'</td>
-                        <td>'Expiration Date'<br>'Expiration Bar'</td>
-                    </tr>
-                </tbody>
-            </table>
-            <div class="text-muted">Last updated: {{ fortinet_device_support.last_updated }}</div>
-        </div>
+        <table class="table table-hover panel-body attr-table">
+            <tbody>
+                <tr {{ fortinet_device_support.partner|coverage_class }}>
+                    <td style="width: 40%">Partner</td>
+                    <td>{{ fortinet_device_support.partner|placeholder }}</td>
+                </tr>
+                <tr {{ fortinet_device_support.end_of_renewal_date|expiration_class }}>
+                    <td>End of Renewal Date</td>
+                    <td>
+                        {{ fortinet_device_support.end_of_renewal_date|placeholder }}<br>
+                        {% include "fortinet/inc/device_eor_bar.html" %}
+                    </td>
+                </tr>
+                <tr {{ fortinet_device_support.end_of_support_date|expiration_class }}>
+                    <td>End of Support Date</td>
+                    <td>
+                        {{ fortinet_device_support.end_of_support_date|placeholder }}<br>
+                        {% include "fortinet/inc/device_eos_bar.html" %}
+                    </td>
+                </tr>
+            </tbody>
+        </table>
+        <h6 class="card-header" style="padding:16px 0px 16px 0px">Entitlements</h6>
+        <table class="table table-hover panel-body attr-table">
+            <tbody>
+                <tr>
+                    <td colspan="2" class="text-center text-muted">— Not implemented yet —</td>
+                </tr>
+                <tr>
+                    <td style="width: 40%" class="text-muted">
+                        'Support Description'<br>
+                        '(Support Level)'
+                    </td>
+                    <td class="text-muted">
+                        'Expiration Date'<br>
+                        'Expiration Bar'
+                    </td>
+                </tr>
+            </tbody>
+        </table>
+        <div class="text-muted">Last updated: {{ fortinet_device_support.last_updated }}</div>
     </div>
-{% else %}
-    {# No fortinet_device_support information available #}
 {% endif %}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,28 +1,15 @@
 {% load filters %} {% if fortinet_device_support %}
 **** FFoorrttiinneett SSooffttwwaarree RReelleeaassee ****
 Last updated: {{ fortinet_device_support.last_updated }}
 **** FFoorrttiinneett LLiicceennssee CCoovveerraaggee ****
-'License Description' 'Expiration Date'
-'(License Type)'      'Expiration Bar'
-'License Description' 'Expiration Date'
-'(License Type)'      'Expiration Bar'
-'License Description' 'Expiration Date'
-'(License Type)'      'Expiration Bar'
+â Not implemented yet â
 'License Description' 'Expiration Date'
 '(License Type)'      'Expiration Bar'
 Last updated: {{ fortinet_device_support.last_updated }}
 **** FFoorrttiinneett DDeevviiccee SSuuppppoorrtt ****
-Partner             Not implemented yet ...
-End of Renewal Date Not implemented yet ...
-End of Support Date Not implemented yet ...
-** SSuuppppoorrtt EEnnttiittlleemmeennttss **
-'Support Description' 'Expiration Date'
-'(Support Level)'     'Expiration Bar'
-'Support Description' 'Expiration Date'
-'(Support Level)'     'Expiration Bar'
-'Support Description' 'Expiration Date'
-'(Support Level)'     'Expiration Bar'
+** EEnnttiittlleemmeennttss **
+â Not implemented yet â
 'Support Description' 'Expiration Date'
 '(Support Level)'     'Expiration Bar'
 Last updated: {{ fortinet_device_support.last_updated }}
-{% else %} {# No fortinet_device_support information available #} {% endif %}
+{% endif %}
```

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templatetags/filters.py` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/views.py` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin/views.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class CiscoDeviceSupportListView(generic.ObjectListView):
     queryset = models.CiscoDeviceSupport.objects.all()
     filterset = filtersets.CiscoDeviceSupportFilterSet
     filterset_form = forms.CiscoDeviceSupportFilterForm
     table = tables.CiscoDeviceSupportTable
-    actions = ("export", "delete")
+    actions = {"export": set(), "bulk_delete": {"delete"}}
 
 
 class CiscoDeviceSupportDeleteView(generic.ObjectDeleteView):
     queryset = models.CiscoDeviceSupport.objects.all()
 
 
 class CiscoDeviceSupportBulkDeleteView(generic.BulkDeleteView):
@@ -29,15 +29,15 @@
 
 
 class CiscoDeviceTypeSupportListView(generic.ObjectListView):
     queryset = models.CiscoDeviceTypeSupport.objects.all()
     filterset = filtersets.CiscoDeviceTypeSupportFilterSet
     filterset_form = forms.CiscoDeviceTypeSupportFilterForm
     table = tables.CiscoDeviceTypeSupportTable
-    actions = ("export", "delete")
+    actions = {"export": set(), "bulk_delete": {"delete"}}
 
 
 class CiscoDeviceTypeSupportDeleteView(generic.ObjectDeleteView):
     queryset = models.CiscoDeviceTypeSupport.objects.all()
 
 
 class CiscoDeviceTypeSupportBulkDeleteView(generic.BulkDeleteView):
@@ -50,18 +50,39 @@
 
 
 class FortinetDeviceSupportListView(generic.ObjectListView):
     queryset = models.FortinetDeviceSupport.objects.all()
     filterset = filtersets.FortinetDeviceSupportFilterSet
     filterset_form = forms.FortinetDeviceSupportFilterForm
     table = tables.FortinetDeviceSupportTable
-    actions = ("export", "delete")
+    actions = {"export": set(), "bulk_delete": {"delete"}}
 
 
 class FortinetDeviceSupportDeleteView(generic.ObjectDeleteView):
     queryset = models.FortinetDeviceSupport.objects.all()
 
 
 class FortinetDeviceSupportBulkDeleteView(generic.BulkDeleteView):
     queryset = models.FortinetDeviceSupport.objects.all()
     filterset = filtersets.FortinetDeviceSupportFilterSet
     table = tables.FortinetDeviceSupport
+
+
+#### PureStorage Support ####################################################################################
+
+
+class PureStorageDeviceSupportListView(generic.ObjectListView):
+    queryset = models.PureStorageDeviceSupport.objects.all()
+    filterset = filtersets.PureStorageDeviceSupportFilterSet
+    filterset_form = forms.PureStorageDeviceSupportFilterForm
+    table = tables.PureStorageDeviceSupportTable
+    actions = {"export": set(), "bulk_delete": {"delete"}}
+
+
+class PureStorageDeviceSupportDeleteView(generic.ObjectDeleteView):
+    queryset = models.PureStorageDeviceSupport.objects.all()
+
+
+class PureStorageDeviceSupportBulkDeleteView(generic.BulkDeleteView):
+    queryset = models.PureStorageDeviceSupport.objects.all()
+    filterset = filtersets.PureStorageDeviceSupportFilterSet
+    table = tables.PureStorageDeviceSupport
```

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin.egg-info/PKG-INFO` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-device-support-plugin
-Version: 0.0.9
+Version: 1.0.1
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin.egg-info/SOURCES.txt` & `netbox_device_support_plugin-1.0.1/netbox_device_support_plugin.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,22 +21,28 @@
 netbox_device_support_plugin/api/__init__.py
 netbox_device_support_plugin/api/serializers.py
 netbox_device_support_plugin/api/urls.py
 netbox_device_support_plugin/api/views.py
 netbox_device_support_plugin/management/__init__.py
 netbox_device_support_plugin/management/commands/__init__.py
 netbox_device_support_plugin/management/commands/sync_cisco_support_data.py
+netbox_device_support_plugin/management/commands/sync_fortinet_support_data.py
+netbox_device_support_plugin/management/commands/sync_purestorage_support_data.py
+netbox_device_support_plugin/migrations/0001_initial.py
 netbox_device_support_plugin/migrations/__init__.py
 netbox_device_support_plugin/templates/cisco/cisco_device_support.html
 netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html
 netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html
 netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html
 netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html
 netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html
 netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html
 netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html
 netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html
 netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html
 netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html
 netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html
+netbox_device_support_plugin/templates/fortinet/inc/device_eor_bar.html
+netbox_device_support_plugin/templates/fortinet/inc/device_eos_bar.html
+netbox_device_support_plugin/templates/purestorage/purestorage_device_support.html
 netbox_device_support_plugin/templatetags/__init__.py
 netbox_device_support_plugin/templatetags/filters.py
```

### Comparing `netbox-device-support-plugin-0.0.9/setup.py` & `netbox_device_support_plugin-1.0.1/setup.py`

 * *Files identical despite different names*

