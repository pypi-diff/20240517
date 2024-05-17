# Comparing `tmp/moesifapi-1.4.5.tar.gz` & `tmp/moesifapi-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moesifapi-1.4.5.tar", last modified: Mon Apr  8 23:29:43 2024, max compression
+gzip compressed data, was "moesifapi-1.4.6.tar", last modified: Wed May  8 23:10:57 2024, max compression
```

## Comparing `moesifapi-1.4.5.tar` & `moesifapi-1.4.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-08 23:29:43.531545 moesifapi-1.4.5/
--rwxr-xr-x   0 keyur      (501) staff       (20)    11918 2020-05-11 16:17:23.000000 moesifapi-1.4.5/LICENSE
--rw-r--r--   0 keyur      (501) staff       (20)       61 2020-05-11 16:17:23.000000 moesifapi-1.4.5/MANIFEST.in
--rw-r--r--   0 keyur      (501) staff       (20)    13737 2024-04-08 23:29:43.532299 moesifapi-1.4.5/PKG-INFO
--rwxr-xr-x   0 keyur      (501) staff       (20)    12654 2024-03-29 18:28:28.000000 moesifapi-1.4.5/README.md
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-08 23:29:43.494394 moesifapi-1.4.5/moesifapi/
--rwxr-xr-x   0 keyur      (501) staff       (20)      209 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/__init__.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     5538 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/api_helper.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-08 23:29:43.500930 moesifapi-1.4.5/moesifapi/app_config/
--rw-r--r--   0 keyur      (501) staff       (20)       25 2024-04-06 01:03:24.000000 moesifapi-1.4.5/moesifapi/app_config/__init__.py
--rw-r--r--   0 keyur      (501) staff       (20)     2688 2024-04-06 01:03:24.000000 moesifapi-1.4.5/moesifapi/app_config/app_config.py
--rw-r--r--   0 keyur      (501) staff       (20)     4028 2024-04-06 01:03:24.000000 moesifapi-1.4.5/moesifapi/app_config/regex_config_helper.py
--rw-r--r--   0 keyur      (501) staff       (20)     5064 2024-04-06 01:03:24.000000 moesifapi-1.4.5/moesifapi/config_manager.py
--rwxr-xr-x   0 keyur      (501) staff       (20)      294 2023-07-01 00:47:27.000000 moesifapi-1.4.5/moesifapi/configuration.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-08 23:29:43.506145 moesifapi-1.4.5/moesifapi/controllers/
--rwxr-xr-x   0 keyur      (501) staff       (20)       94 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/controllers/__init__.py
--rwxr-xr-x   0 keyur      (501) staff       (20)    19397 2024-03-29 18:28:28.000000 moesifapi-1.4.5/moesifapi/controllers/api_controller.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     1493 2024-03-29 18:28:28.000000 moesifapi-1.4.5/moesifapi/controllers/base_controller.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     2342 2021-02-17 05:27:26.000000 moesifapi-1.4.5/moesifapi/controllers/health_controller.py
--rwxr-xr-x   0 keyur      (501) staff       (20)      409 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/decorators.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-08 23:29:43.508993 moesifapi-1.4.5/moesifapi/exceptions/
--rwxr-xr-x   0 keyur      (501) staff       (20)       29 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/exceptions/__init__.py
--rwxr-xr-x   0 keyur      (501) staff       (20)      827 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/exceptions/api_exception.py
--rw-r--r--   0 keyur      (501) staff       (20)    11182 2024-04-06 01:03:24.000000 moesifapi-1.4.5/moesifapi/governance_manager.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-08 23:29:43.515685 moesifapi-1.4.5/moesifapi/http/
--rwxr-xr-x   0 keyur      (501) staff       (20)      205 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/http/__init__.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     1117 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/http/http_call_back.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     7690 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/http/http_client.py
--rwxr-xr-x   0 keyur      (501) staff       (20)      962 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/http/http_context.py
--rwxr-xr-x   0 keyur      (501) staff       (20)      791 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/http/http_method_enum.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     2343 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/http/http_request.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     1004 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/http/http_response.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     2815 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/http/requests_client.py
--rw-r--r--   0 keyur      (501) staff       (20)      148 2024-04-06 01:03:24.000000 moesifapi-1.4.5/moesifapi/logger_helper.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-08 23:29:43.524229 moesifapi-1.4.5/moesifapi/models/
--rwxr-xr-x   0 keyur      (501) staff       (20)      245 2024-03-29 18:28:28.000000 moesifapi-1.4.5/moesifapi/models/__init__.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     1836 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/models/base_model.py
--rw-r--r--   0 keyur      (501) staff       (20)     3002 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/models/campaign_model.py
--rw-r--r--   0 keyur      (501) staff       (20)     3182 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/models/company_model.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     4135 2024-03-29 18:28:28.000000 moesifapi-1.4.5/moesifapi/models/event_model.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     3141 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/models/event_request_model.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     2638 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/models/event_response_model.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     1525 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/models/status_model.py
--rw-r--r--   0 keyur      (501) staff       (20)     3047 2024-03-29 18:28:28.000000 moesifapi-1.4.5/moesifapi/models/subscription_model.py
--rw-r--r--   0 keyur      (501) staff       (20)     3470 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/models/user_model.py
--rwxr-xr-x   0 keyur      (501) staff       (20)      461 2020-05-11 16:17:23.000000 moesifapi-1.4.5/moesifapi/moesif_api_client.py
--rw-r--r--   0 keyur      (501) staff       (20)     2344 2024-04-06 01:03:24.000000 moesifapi-1.4.5/moesifapi/parse_body.py
--rw-r--r--   0 keyur      (501) staff       (20)     8043 2024-04-06 01:03:24.000000 moesifapi-1.4.5/moesifapi/update_companies.py
--rw-r--r--   0 keyur      (501) staff       (20)     7784 2024-04-06 01:03:24.000000 moesifapi-1.4.5/moesifapi/update_users.py
--rw-r--r--   0 keyur      (501) staff       (20)     8502 2024-04-06 01:03:24.000000 moesifapi-1.4.5/moesifapi/workers.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-08 23:29:43.498491 moesifapi-1.4.5/moesifapi.egg-info/
--rw-r--r--   0 keyur      (501) staff       (20)    13737 2024-04-08 23:29:43.000000 moesifapi-1.4.5/moesifapi.egg-info/PKG-INFO
--rw-r--r--   0 keyur      (501) staff       (20)     1637 2024-04-08 23:29:43.000000 moesifapi-1.4.5/moesifapi.egg-info/SOURCES.txt
--rw-r--r--   0 keyur      (501) staff       (20)        1 2024-04-08 23:29:43.000000 moesifapi-1.4.5/moesifapi.egg-info/dependency_links.txt
--rw-r--r--   0 keyur      (501) staff       (20)       45 2024-04-08 23:29:43.000000 moesifapi-1.4.5/moesifapi.egg-info/entry_points.txt
--rw-r--r--   0 keyur      (501) staff       (20)      119 2024-04-08 23:29:43.000000 moesifapi-1.4.5/moesifapi.egg-info/requires.txt
--rw-r--r--   0 keyur      (501) staff       (20)       16 2024-04-08 23:29:43.000000 moesifapi-1.4.5/moesifapi.egg-info/top_level.txt
--rw-r--r--   0 keyur      (501) staff       (20)       67 2024-04-08 23:29:43.533637 moesifapi-1.4.5/setup.cfg
--rw-r--r--   0 keyur      (501) staff       (20)     3724 2024-04-08 23:28:15.000000 moesifapi-1.4.5/setup.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-08 23:29:43.525164 moesifapi-1.4.5/tests/
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-08 23:29:43.529191 moesifapi-1.4.5/tests/controllers/
--rwxr-xr-x   0 keyur      (501) staff       (20)        0 2020-05-11 16:17:23.000000 moesifapi-1.4.5/tests/controllers/__init__.py
--rwxr-xr-x   0 keyur      (501) staff       (20)      887 2024-04-06 01:04:20.000000 moesifapi-1.4.5/tests/controllers/controller_test_base.py
--rwxr-xr-x   0 keyur      (501) staff       (20)    17361 2024-03-29 18:28:28.000000 moesifapi-1.4.5/tests/controllers/test_api_controller.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     4922 2020-05-11 16:17:23.000000 moesifapi-1.4.5/tests/test_helper.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.845313 moesifapi-1.4.6/
+-rwxr-xr-x   0 keyur      (501) staff       (20)    11918 2020-05-11 16:17:23.000000 moesifapi-1.4.6/LICENSE
+-rw-r--r--   0 keyur      (501) staff       (20)       61 2020-05-11 16:17:23.000000 moesifapi-1.4.6/MANIFEST.in
+-rw-r--r--   0 keyur      (501) staff       (20)    13737 2024-05-08 23:10:57.845555 moesifapi-1.4.6/PKG-INFO
+-rwxr-xr-x   0 keyur      (501) staff       (20)    12654 2024-03-29 18:28:28.000000 moesifapi-1.4.6/README.md
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.786080 moesifapi-1.4.6/moesifapi/
+-rwxr-xr-x   0 keyur      (501) staff       (20)      209 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     5538 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/api_helper.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.790691 moesifapi-1.4.6/moesifapi/app_config/
+-rw-r--r--   0 keyur      (501) staff       (20)       25 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/app_config/__init__.py
+-rw-r--r--   0 keyur      (501) staff       (20)     2688 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/app_config/app_config.py
+-rw-r--r--   0 keyur      (501) staff       (20)     4028 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/app_config/regex_config_helper.py
+-rw-r--r--   0 keyur      (501) staff       (20)     5064 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/config_manager.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      343 2024-05-08 23:09:55.000000 moesifapi-1.4.6/moesifapi/configuration.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.795658 moesifapi-1.4.6/moesifapi/controllers/
+-rwxr-xr-x   0 keyur      (501) staff       (20)       94 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/controllers/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)    19878 2024-05-08 23:09:55.000000 moesifapi-1.4.6/moesifapi/controllers/api_controller.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     1493 2024-03-29 18:28:28.000000 moesifapi-1.4.6/moesifapi/controllers/base_controller.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     2342 2021-02-17 05:27:26.000000 moesifapi-1.4.6/moesifapi/controllers/health_controller.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      409 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/decorators.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.797738 moesifapi-1.4.6/moesifapi/exceptions/
+-rwxr-xr-x   0 keyur      (501) staff       (20)       29 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/exceptions/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      827 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/exceptions/api_exception.py
+-rw-r--r--   0 keyur      (501) staff       (20)    11182 2024-05-08 18:35:25.000000 moesifapi-1.4.6/moesifapi/governance_manager.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.833772 moesifapi-1.4.6/moesifapi/http/
+-rwxr-xr-x   0 keyur      (501) staff       (20)      205 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/http/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     1117 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/http/http_call_back.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     7690 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/http/http_client.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      962 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/http/http_context.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      791 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/http/http_method_enum.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     2343 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/http/http_request.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     1004 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/http/http_response.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     3291 2024-05-08 23:09:55.000000 moesifapi-1.4.6/moesifapi/http/requests_client.py
+-rw-r--r--   0 keyur      (501) staff       (20)      148 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/logger_helper.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.841401 moesifapi-1.4.6/moesifapi/models/
+-rwxr-xr-x   0 keyur      (501) staff       (20)      245 2024-03-29 18:28:28.000000 moesifapi-1.4.6/moesifapi/models/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     1836 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/models/base_model.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3002 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/models/campaign_model.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3182 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/models/company_model.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     4135 2024-03-29 18:28:28.000000 moesifapi-1.4.6/moesifapi/models/event_model.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     3141 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/models/event_request_model.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     2638 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/models/event_response_model.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     1525 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/models/status_model.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3047 2024-03-29 18:28:28.000000 moesifapi-1.4.6/moesifapi/models/subscription_model.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3470 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/models/user_model.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      461 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/moesif_api_client.py
+-rw-r--r--   0 keyur      (501) staff       (20)     2344 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/parse_body.py
+-rw-r--r--   0 keyur      (501) staff       (20)     8043 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/update_companies.py
+-rw-r--r--   0 keyur      (501) staff       (20)     7784 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/update_users.py
+-rw-r--r--   0 keyur      (501) staff       (20)     8502 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/workers.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.788787 moesifapi-1.4.6/moesifapi.egg-info/
+-rw-r--r--   0 keyur      (501) staff       (20)    13737 2024-05-08 23:10:57.000000 moesifapi-1.4.6/moesifapi.egg-info/PKG-INFO
+-rw-r--r--   0 keyur      (501) staff       (20)     1637 2024-05-08 23:10:57.000000 moesifapi-1.4.6/moesifapi.egg-info/SOURCES.txt
+-rw-r--r--   0 keyur      (501) staff       (20)        1 2024-05-08 23:10:57.000000 moesifapi-1.4.6/moesifapi.egg-info/dependency_links.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       45 2024-05-08 23:10:57.000000 moesifapi-1.4.6/moesifapi.egg-info/entry_points.txt
+-rw-r--r--   0 keyur      (501) staff       (20)      119 2024-05-08 23:10:57.000000 moesifapi-1.4.6/moesifapi.egg-info/requires.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       16 2024-05-08 23:10:57.000000 moesifapi-1.4.6/moesifapi.egg-info/top_level.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       67 2024-05-08 23:10:57.846238 moesifapi-1.4.6/setup.cfg
+-rw-r--r--   0 keyur      (501) staff       (20)     3724 2024-05-08 23:09:55.000000 moesifapi-1.4.6/setup.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.842225 moesifapi-1.4.6/tests/
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.844234 moesifapi-1.4.6/tests/controllers/
+-rwxr-xr-x   0 keyur      (501) staff       (20)        0 2020-05-11 16:17:23.000000 moesifapi-1.4.6/tests/controllers/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      887 2024-04-06 01:04:20.000000 moesifapi-1.4.6/tests/controllers/controller_test_base.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)    17361 2024-03-29 18:28:28.000000 moesifapi-1.4.6/tests/controllers/test_api_controller.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     4922 2020-05-11 16:17:23.000000 moesifapi-1.4.6/tests/test_helper.py
```

### Comparing `moesifapi-1.4.5/LICENSE` & `moesifapi-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/PKG-INFO` & `moesifapi-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moesifapi
-Version: 1.4.5
+Version: 1.4.6
 Summary: Moesif API Lib for Python
 Home-page: https://www.moesif.com/docs/api?python#api-libs
 Author: Moesif, Inc
 Author-email: derric@moesif.com
 License: Apache Software License
 Keywords: log analysis restful api development debug
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moesifapi-1.4.5/README.md` & `moesifapi-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/api_helper.py` & `moesifapi-1.4.6/moesifapi/api_helper.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/app_config/app_config.py` & `moesifapi-1.4.6/moesifapi/app_config/app_config.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/app_config/regex_config_helper.py` & `moesifapi-1.4.6/moesifapi/app_config/regex_config_helper.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/config_manager.py` & `moesifapi-1.4.6/moesifapi/config_manager.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/controllers/api_controller.py` & `moesifapi-1.4.6/moesifapi/controllers/api_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,30 @@
 """
     moesifapi.controllers.api_controller
 
 
 """
 
 from .base_controller import *
-
+import gzip
 
 
 class ApiController(BaseController):
 
     """A Controller to access Endpoints in the moesifapi API."""
 
+    @classmethod
+    def generate_post_payload(cls, body, headers):
+        try:
+            payload = gzip.compress(APIHelper.json_serialize(body).encode('utf-8'))
+            headers['Content-Encoding'] = 'gzip'
+        except:
+            payload = APIHelper.json_serialize(body)
+        return payload, headers
+
     def __init__(self, http_client = None, http_call_back = None):
         """Constructor which allows a different HTTP client for this controller."""
         BaseController.__init__(self, http_client, http_call_back)
 
     def create_event(self,
                      body):
         """Does a POST request to /v1/events.
@@ -50,16 +59,19 @@
         # Prepare headers
         _headers = {
             'content-type': 'application/json; charset=utf-8',
             'X-Moesif-Application-Id': Configuration.application_id,
             'User-Agent': Configuration.version,
         }
 
+        # Generate http payload
+        _body, _headers = self.generate_post_payload(body, _headers)
+
         # Prepare the API call.
-        _request = self.http_client.post(_query_url, headers=_headers, parameters=APIHelper.json_serialize(body))
+        _request = self.http_client.post(_query_url, headers=_headers, parameters=_body)
 
         # Invoke the on before request HttpCallBack if specified
         if self.http_call_back != None:
             self.http_call_back.on_before_request(_request)
 
         # Invoke the API call  to fetch the response.
         _response = self.http_client.execute_as_string(_request)
@@ -111,16 +123,19 @@
         # Prepare headers
         _headers = {
             'content-type': 'application/json; charset=utf-8',
             'X-Moesif-Application-Id': Configuration.application_id,
             'User-Agent': Configuration.version,
         }
 
+        # Generate http payload
+        _body, _headers = self.generate_post_payload(body, _headers)
+
         # Prepare the API call.
-        _request = self.http_client.post(_query_url, headers=_headers, parameters=APIHelper.json_serialize(body))
+        _request = self.http_client.post(_query_url, headers=_headers, parameters=_body)
 
         # Invoke the on before request HttpCallBack if specified
         if self.http_call_back != None:
             self.http_call_back.on_before_request(_request)
 
         # Invoke the API call  to fetch the response.
         _response = self.http_client.execute_as_string(_request)
```

### Comparing `moesifapi-1.4.5/moesifapi/controllers/base_controller.py` & `moesifapi-1.4.6/moesifapi/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/controllers/health_controller.py` & `moesifapi-1.4.6/moesifapi/controllers/health_controller.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/exceptions/api_exception.py` & `moesifapi-1.4.6/moesifapi/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/governance_manager.py` & `moesifapi-1.4.6/moesifapi/governance_manager.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/http/http_call_back.py` & `moesifapi-1.4.6/moesifapi/http/http_call_back.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/http/http_client.py` & `moesifapi-1.4.6/moesifapi/http/http_client.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/http/http_context.py` & `moesifapi-1.4.6/moesifapi/http/http_context.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/http/http_method_enum.py` & `moesifapi-1.4.6/moesifapi/http/http_method_enum.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/http/http_request.py` & `moesifapi-1.4.6/moesifapi/http/http_request.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/http/http_response.py` & `moesifapi-1.4.6/moesifapi/http/http_response.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/http/requests_client.py` & `moesifapi-1.4.6/moesifapi/http/requests_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,34 @@
 """
     moesifapi.http.requests_client
 
 
 """
 
 import requests
-
+from requests.adapters import HTTPAdapter
+from ..configuration import Configuration
 from .http_client import HttpClient
 from .http_response import HttpResponse
 from .http_method_enum import HttpMethodEnum
 
 class RequestsClient(HttpClient):
 
     """An implementation of HttpClient that uses Requests as its HTTP Client
     
     """
+
+    # connection pool here
+
+    def __init__(self):
+        self.session = requests.Session()
+        self.adapter = HTTPAdapter(pool_connections=Configuration.pool_connections, pool_maxsize=Configuration.pool_maxsize)
+        self.session.mount('http://', self.adapter)
+        self.session.mount('https://', self.adapter)
+
     def execute_as_string(self, request):
         """Execute a given HttpRequest to get a string response back
        
         Args:
             request (HttpRequest): The given HttpRequest to execute.
             
         Returns:
@@ -28,21 +38,22 @@
             
         """	
         auth = None
 
         if request.username or request.password:
             auth=(request.username, request.password)
 
-        response = requests.request(HttpMethodEnum.to_string(request.http_method), 
-                                    request.query_url, 
-                                    headers=request.headers,
-                                    params=request.query_parameters, 
-                                    data=request.parameters,
-                                    files=request.files,
-                                    auth=auth)
+        # connection pool to make request
+        response = self.session.request(HttpMethodEnum.to_string(request.http_method),
+                                        request.query_url,
+                                        headers=request.headers,
+                                        params=request.query_parameters,
+                                        data=request.parameters,
+                                        files=request.files,
+                                        auth=auth)
 
         return self.convert_response(response, False)
     
     def execute_as_binary(self, request):
         """Execute a given HttpRequest to get a binary response back
        
         Args:
```

### Comparing `moesifapi-1.4.5/moesifapi/models/base_model.py` & `moesifapi-1.4.6/moesifapi/models/base_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/models/campaign_model.py` & `moesifapi-1.4.6/moesifapi/models/campaign_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/models/company_model.py` & `moesifapi-1.4.6/moesifapi/models/company_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/models/event_model.py` & `moesifapi-1.4.6/moesifapi/models/event_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/models/event_request_model.py` & `moesifapi-1.4.6/moesifapi/models/event_request_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/models/event_response_model.py` & `moesifapi-1.4.6/moesifapi/models/event_response_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/models/status_model.py` & `moesifapi-1.4.6/moesifapi/models/status_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/models/subscription_model.py` & `moesifapi-1.4.6/moesifapi/models/subscription_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/models/user_model.py` & `moesifapi-1.4.6/moesifapi/models/user_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/parse_body.py` & `moesifapi-1.4.6/moesifapi/parse_body.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/update_companies.py` & `moesifapi-1.4.6/moesifapi/update_companies.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/update_users.py` & `moesifapi-1.4.6/moesifapi/update_users.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi/workers.py` & `moesifapi-1.4.6/moesifapi/workers.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/moesifapi.egg-info/PKG-INFO` & `moesifapi-1.4.6/moesifapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moesifapi
-Version: 1.4.5
+Version: 1.4.6
 Summary: Moesif API Lib for Python
 Home-page: https://www.moesif.com/docs/api?python#api-libs
 Author: Moesif, Inc
 Author-email: derric@moesif.com
 License: Apache Software License
 Keywords: log analysis restful api development debug
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moesifapi-1.4.5/moesifapi.egg-info/SOURCES.txt` & `moesifapi-1.4.6/moesifapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/setup.py` & `moesifapi-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 setup(
     name='moesifapi',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.4.5',
+    version='1.4.6',
 
     description='Moesif API Lib for Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://www.moesif.com/docs/api?python#api-libs',
```

### Comparing `moesifapi-1.4.5/tests/controllers/controller_test_base.py` & `moesifapi-1.4.6/tests/controllers/controller_test_base.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/tests/controllers/test_api_controller.py` & `moesifapi-1.4.6/tests/controllers/test_api_controller.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.5/tests/test_helper.py` & `moesifapi-1.4.6/tests/test_helper.py`

 * *Files identical despite different names*

