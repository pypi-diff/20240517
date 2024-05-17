# Comparing `tmp/celitech_sdk-1.1.57.tar.gz` & `tmp/celitech_sdk-1.1.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celitech_sdk-1.1.57.tar", last modified: Fri May 10 09:37:46 2024, max compression
+gzip compressed data, was "celitech_sdk-1.1.58.tar", last modified: Fri May 17 11:29:05 2024, max compression
```

## Comparing `celitech_sdk-1.1.57.tar` & `celitech_sdk-1.1.58.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.340386 celitech_sdk-1.1.57/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15417 2024-05-10 09:37:46.340386 celitech_sdk-1.1.57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:37:46.340386 celitech_sdk-1.1.57/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.328387 celitech_sdk-1.1.57/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.332387 celitech_sdk-1.1.57/src/celitech/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.332387 celitech_sdk-1.1.57/src/celitech/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/hooks/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.332387 celitech_sdk-1.1.57/src/celitech/models/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/create_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/create_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/edit_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/edit_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/get_esim_device_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/get_esim_history_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/get_esim_mac_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/get_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/get_purchase_consumption_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/list_destinations_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/list_packages_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/list_purchases_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/top_up_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/top_up_esim_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.336387 celitech_sdk-1.1.57/src/celitech/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/utils/cast_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/models/utils/json_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.336387 celitech_sdk-1.1.57/src/celitech/net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.336387 celitech_sdk-1.1.57/src/celitech/net/environment/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/environment/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.336387 celitech_sdk-1.1.57/src/celitech/net/headers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/headers/base_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.336387 celitech_sdk-1.1.57/src/celitech/net/request_chain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/request_chain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.336387 celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/hook_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/http_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/request_chain/request_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.336387 celitech_sdk-1.1.57/src/celitech/net/transport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/transport/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/transport/request_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/transport/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/transport/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/net/transport/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.340386 celitech_sdk-1.1.57/src/celitech/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/services/destinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/services/e_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/services/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/services/purchases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.340386 celitech_sdk-1.1.57/src/celitech/services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/services/utils/base_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/services/utils/default_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-05-10 09:37:34.000000 celitech_sdk-1.1.57/src/celitech/services/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:37:46.340386 celitech_sdk-1.1.57/src/celitech_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15417 2024-05-10 09:37:46.000000 celitech_sdk-1.1.57/src/celitech_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-10 09:37:46.000000 celitech_sdk-1.1.57/src/celitech_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:37:46.000000 celitech_sdk-1.1.57/src/celitech_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 09:37:46.000000 celitech_sdk-1.1.57/src/celitech_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 09:37:46.000000 celitech_sdk-1.1.57/src/celitech_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.435221 celitech_sdk-1.1.58/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15417 2024-05-17 11:29:05.435221 celitech_sdk-1.1.58/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 11:29:05.435221 celitech_sdk-1.1.58/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.423221 celitech_sdk-1.1.58/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.427221 celitech_sdk-1.1.58/src/celitech/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.427221 celitech_sdk-1.1.58/src/celitech/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/hooks/hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.431221 celitech_sdk-1.1.58/src/celitech/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/create_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/create_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/edit_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/edit_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/get_esim_device_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/get_esim_history_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/get_esim_mac_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/get_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/get_purchase_consumption_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/list_destinations_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/list_packages_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/list_purchases_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/top_up_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/top_up_esim_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.431221 celitech_sdk-1.1.58/src/celitech/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/utils/cast_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/models/utils/json_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.431221 celitech_sdk-1.1.58/src/celitech/net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.431221 celitech_sdk-1.1.58/src/celitech/net/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/environment/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.431221 celitech_sdk-1.1.58/src/celitech/net/headers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/headers/base_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.431221 celitech_sdk-1.1.58/src/celitech/net/request_chain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/request_chain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.431221 celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/hook_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/http_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/request_chain/request_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.435221 celitech_sdk-1.1.58/src/celitech/net/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/transport/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/transport/request_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/transport/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/transport/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/net/transport/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.435221 celitech_sdk-1.1.58/src/celitech/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/services/destinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/services/e_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/services/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/services/purchases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.435221 celitech_sdk-1.1.58/src/celitech/services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/services/utils/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/services/utils/default_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-05-17 11:28:53.000000 celitech_sdk-1.1.58/src/celitech/services/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:29:05.435221 celitech_sdk-1.1.58/src/celitech_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15417 2024-05-17 11:29:05.000000 celitech_sdk-1.1.58/src/celitech_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-17 11:29:05.000000 celitech_sdk-1.1.58/src/celitech_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 11:29:05.000000 celitech_sdk-1.1.58/src/celitech_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:29:05.000000 celitech_sdk-1.1.58/src/celitech_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 11:29:05.000000 celitech_sdk-1.1.58/src/celitech_sdk.egg-info/top_level.txt
```

### Comparing `celitech_sdk-1.1.57/LICENSE` & `celitech_sdk-1.1.58/LICENSE`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/PKG-INFO` & `celitech_sdk-1.1.58/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: celitech-sdk
-Version: 1.1.57
+Version: 1.1.58
 Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# Celitech Python SDK 1.1.57
+# Celitech Python SDK 1.1.58
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.57
+- SDK version: 1.1.58
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
```

### Comparing `celitech_sdk-1.1.57/README.md` & `celitech_sdk-1.1.58/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# Celitech Python SDK 1.1.57
+# Celitech Python SDK 1.1.58
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.57
+- SDK version: 1.1.58
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
```

### Comparing `celitech_sdk-1.1.57/src/celitech/hooks/hook.py` & `celitech_sdk-1.1.58/src/celitech/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/models/__init__.py` & `celitech_sdk-1.1.58/src/celitech/models/__init__.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/models/base.py` & `celitech_sdk-1.1.58/src/celitech/models/base.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/models/create_purchase_ok_response.py` & `celitech_sdk-1.1.58/src/celitech/models/create_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/models/create_purchase_request.py` & `celitech_sdk-1.1.58/src/celitech/models/create_purchase_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 
     :param destination: ISO representation of the package's destination
     :type destination: str
     :param data_limit_in_gb: Size of the package in GB. The available options are 1, 2, 3, 5, 8, 20GB
     :type data_limit_in_gb: float
     :param start_date: Start date of the package's validity in the format 'yyyy-MM-dd'. This date can be set to the current day or any day within the next 12 months.
     :type start_date: str
-    :param end_date: End date of the package's validity in the format 'yyyy-MM-dd'. End date can be maximum 60 days after Start date.
+    :param end_date: End date of the package's validity in the format 'yyyy-MM-dd'. End date can be maximum 90 days after Start date.
     :type end_date: str
     :param email: Email address where the purchase confirmation email will be sent (including QR Code & activation steps), defaults to None
     :type email: str, optional
     :param network_brand: Customize the network brand of the issued eSIM. This parameter is accessible to platforms with Diamond tier and requires an alphanumeric string of up to 15 characters, defaults to None
     :type network_brand: str, optional
     :param start_time: Epoch value representing the start time of the package's validity. This timestamp can be set to the current time or any time within the next 12 months., defaults to None
     :type start_time: float, optional
-    :param end_time: Epoch value representing the end time of the package's validity. End time can be maximum 60 days after Start time., defaults to None
+    :param end_time: Epoch value representing the end time of the package's validity. End time can be maximum 90 days after Start time., defaults to None
     :type end_time: float, optional
     """
 
     def __init__(
         self,
         destination: str,
         data_limit_in_gb: float,
```

### Comparing `celitech_sdk-1.1.57/src/celitech/models/edit_purchase_ok_response.py` & `celitech_sdk-1.1.58/src/celitech/models/edit_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/models/edit_purchase_request.py` & `celitech_sdk-1.1.58/src/celitech/models/edit_purchase_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 class EditPurchaseRequest(BaseModel):
     """EditPurchaseRequest
 
     :param purchase_id: ID of the purchase
     :type purchase_id: str
     :param start_date: Start date of the package's validity in the format 'yyyy-MM-dd'. This date can be set to the current day or any day within the next 12 months.
     :type start_date: str
-    :param end_date: End date of the package's validity in the format 'yyyy-MM-dd'. End date can be maximum 60 days after Start date.
+    :param end_date: End date of the package's validity in the format 'yyyy-MM-dd'. End date can be maximum 90 days after Start date.
     :type end_date: str
     :param start_time: Epoch value representing the start time of the package's validity. This timestamp can be set to the current time or any time within the next 12 months., defaults to None
     :type start_time: float, optional
-    :param end_time: Epoch value representing the end time of the package's validity. End time can be maximum 60 days after Start time., defaults to None
+    :param end_time: Epoch value representing the end time of the package's validity. End time can be maximum 90 days after Start time., defaults to None
     :type end_time: float, optional
     """
 
     def __init__(
         self,
         purchase_id: str,
         start_date: str,
```

### Comparing `celitech_sdk-1.1.57/src/celitech/models/get_esim_device_ok_response.py` & `celitech_sdk-1.1.58/src/celitech/models/get_esim_device_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/models/get_esim_history_ok_response.py` & `celitech_sdk-1.1.58/src/celitech/models/get_esim_history_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/models/get_esim_mac_ok_response.py` & `celitech_sdk-1.1.58/src/celitech/models/get_esim_mac_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/models/get_esim_ok_response.py` & `celitech_sdk-1.1.58/src/celitech/models/get_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/models/get_purchase_consumption_ok_response.py` & `celitech_sdk-1.1.58/src/celitech/models/get_purchase_consumption_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/models/list_destinations_ok_response.py` & `celitech_sdk-1.1.58/src/celitech/models/list_destinations_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/models/list_packages_ok_response.py` & `celitech_sdk-1.1.58/src/celitech/models/list_packages_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/models/list_purchases_ok_response.py` & `celitech_sdk-1.1.58/src/celitech/models/list_purchases_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/models/top_up_esim_ok_response.py` & `celitech_sdk-1.1.58/src/celitech/models/top_up_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/models/top_up_esim_request.py` & `celitech_sdk-1.1.58/src/celitech/models/top_up_esim_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 
     :param iccid: ID of the eSIM
     :type iccid: str
     :param data_limit_in_gb: Size of the package in GB. The available options are 1, 2, 3, 5, 8, 20GB
     :type data_limit_in_gb: float
     :param start_date: Start date of the package's validity in the format 'yyyy-MM-dd'. This date can be set to the current day or any day within the next 12 months.
     :type start_date: str
-    :param end_date: End date of the package's validity in the format 'yyyy-MM-dd'. End date can be maximum 60 days after Start date.
+    :param end_date: End date of the package's validity in the format 'yyyy-MM-dd'. End date can be maximum 90 days after Start date.
     :type end_date: str
     :param email: Email address where the purchase confirmation email will be sent (excluding QR Code & activation steps), defaults to None
     :type email: str, optional
     :param start_time: Epoch value representing the start time of the package's validity. This timestamp can be set to the current time or any time within the next 12 months., defaults to None
     :type start_time: float, optional
-    :param end_time: Epoch value representing the end time of the package's validity. End time can be maximum 60 days after Start time., defaults to None
+    :param end_time: Epoch value representing the end time of the package's validity. End time can be maximum 90 days after Start time., defaults to None
     :type end_time: float, optional
     """
 
     def __init__(
         self,
         iccid: str,
         data_limit_in_gb: float,
```

### Comparing `celitech_sdk-1.1.57/src/celitech/models/utils/cast_models.py` & `celitech_sdk-1.1.58/src/celitech/models/utils/cast_models.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/models/utils/json_map.py` & `celitech_sdk-1.1.58/src/celitech/models/utils/json_map.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/base_handler.py` & `celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/hook_handler.py` & `celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/hook_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/http_handler.py` & `celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/http_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/net/request_chain/handlers/retry_handler.py` & `celitech_sdk-1.1.58/src/celitech/net/request_chain/handlers/retry_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/net/request_chain/request_chain.py` & `celitech_sdk-1.1.58/src/celitech/net/request_chain/request_chain.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/net/transport/request.py` & `celitech_sdk-1.1.58/src/celitech/net/transport/request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/net/transport/request_error.py` & `celitech_sdk-1.1.58/src/celitech/net/transport/request_error.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/net/transport/response.py` & `celitech_sdk-1.1.58/src/celitech/net/transport/response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/net/transport/serializer.py` & `celitech_sdk-1.1.58/src/celitech/net/transport/serializer.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/net/transport/utils.py` & `celitech_sdk-1.1.58/src/celitech/net/transport/utils.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/sdk.py` & `celitech_sdk-1.1.58/src/celitech/sdk.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/services/destinations.py` & `celitech_sdk-1.1.58/src/celitech/services/destinations.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/services/e_sim.py` & `celitech_sdk-1.1.58/src/celitech/services/e_sim.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/services/packages.py` & `celitech_sdk-1.1.58/src/celitech/services/packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,25 +21,25 @@
     ) -> ListPackagesOkResponse:
         """List of available packages
 
         :param destination: ISO representation of the package's destination., defaults to None
         :type destination: str, optional
         :param start_date: Start date of the package's validity in the format 'yyyy-MM-dd'. This date can be set to the current day or any day within the next 12 months., defaults to None
         :type start_date: str, optional
-        :param end_date: End date of the package's validity in the format 'yyyy-MM-dd'. End date can be maximum 60 days after Start date., defaults to None
+        :param end_date: End date of the package's validity in the format 'yyyy-MM-dd'. End date can be maximum 90 days after Start date., defaults to None
         :type end_date: str, optional
         :param after_cursor: To get the next batch of results, use this parameter. It tells the API where to start fetching data after the last item you received. It helps you avoid repeats and efficiently browse through large sets of data., defaults to None
         :type after_cursor: str, optional
         :param limit: Maximum number of packages to be returned in the response. The value must be greater than 0 and less than or equal to 160. If not provided, the default value is 20, defaults to None
         :type limit: float, optional
         :param start_time: Epoch value representing the start time of the package's validity. This timestamp can be set to the current time or any time within the next 12 months, defaults to None
         :type start_time: int, optional
-        :param end_time: Epoch value representing the end time of the package's validity. End time can be maximum 60 days after Start time, defaults to None
+        :param end_time: Epoch value representing the end time of the package's validity. End time can be maximum 90 days after Start time, defaults to None
         :type end_time: int, optional
-        :param duration: Duration in seconds for the package's validity. If this parameter is present, it will override the startTime and endTime parameters. The maximum duration for a package's validity period is 60 days, defaults to None
+        :param duration: Duration in seconds for the package's validity. If this parameter is present, it will override the startTime and endTime parameters. The maximum duration for a package's validity period is 90 days, defaults to None
         :type duration: float, optional
         ...
         :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
         ...
         :return: Successful Response
         :rtype: ListPackagesOkResponse
         """
```

### Comparing `celitech_sdk-1.1.57/src/celitech/services/purchases.py` & `celitech_sdk-1.1.58/src/celitech/services/purchases.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/services/utils/base_service.py` & `celitech_sdk-1.1.58/src/celitech/services/utils/base_service.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/services/utils/default_headers.py` & `celitech_sdk-1.1.58/src/celitech/services/utils/default_headers.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech/services/utils/validator.py` & `celitech_sdk-1.1.58/src/celitech/services/utils/validator.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.57/src/celitech_sdk.egg-info/PKG-INFO` & `celitech_sdk-1.1.58/src/celitech_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: celitech-sdk
-Version: 1.1.57
+Version: 1.1.58
 Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# Celitech Python SDK 1.1.57
+# Celitech Python SDK 1.1.58
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.57
+- SDK version: 1.1.58
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
```

### Comparing `celitech_sdk-1.1.57/src/celitech_sdk.egg-info/SOURCES.txt` & `celitech_sdk-1.1.58/src/celitech_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

