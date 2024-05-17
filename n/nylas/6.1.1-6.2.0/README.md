# Comparing `tmp/nylas-6.1.1.tar.gz` & `tmp/nylas-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nylas-6.1.1.tar", last modified: Tue Mar  5 22:43:35 2024, max compression
+gzip compressed data, was "nylas-6.2.0.tar", last modified: Fri May 17 18:22:25 2024, max compression
```

## Comparing `nylas-6.1.1.tar` & `nylas-6.2.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-03-05 22:43:35.626826 nylas-6.1.1/
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     1072 2023-05-30 00:19:43.000000 nylas-6.1.1/LICENSE
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     6045 2024-03-05 22:43:35.626678 nylas-6.1.1/PKG-INFO
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     5618 2024-03-05 22:18:14.000000 nylas-6.1.1/README.md
-drwxr-xr-x   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-03-05 22:43:35.606627 nylas-6.1.1/nylas/
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)       54 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/__init__.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)       22 2024-03-05 22:40:39.000000 nylas-6.1.1/nylas/_client_sdk_version.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     4075 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/client.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)      572 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/config.py
-drwxr-xr-x   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-03-05 22:43:35.610135 nylas-6.1.1/nylas/handler/
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/handler/__init__.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     2155 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/handler/api_resources.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     5302 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/handler/http_client.py
-drwxr-xr-x   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-03-05 22:43:35.618846 nylas-6.1.1/nylas/models/
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/__init__.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     2559 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/application_details.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     1996 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/attachments.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     6655 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/auth.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     5609 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/availability.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3581 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/calendars.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     4183 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/connectors.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)    10893 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/contacts.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3285 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/credentials.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     6209 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/drafts.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     4470 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/errors.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)    25604 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/events.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     2670 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/folders.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     1588 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/free_busy.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3577 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/grants.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)      544 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/list_query_params.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     6430 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/messages.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     2710 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/redirect_uri.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3254 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/response.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)      550 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/smart_compose.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     5576 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/threads.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     4449 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/models/webhooks.py
-drwxr-xr-x   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-03-05 22:43:35.625089 nylas-6.1.1/nylas/resources/
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/__init__.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     1110 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/applications.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3291 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/attachments.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     7408 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/auth.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     5479 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/calendars.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3288 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/connectors.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     4350 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/contacts.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3420 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/credentials.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     5016 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/drafts.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     4930 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/events.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     2948 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/folders.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     2179 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/grants.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     6819 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/messages.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     2755 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/redirect_uris.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)      207 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/resource.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     1841 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/smart_compose.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     2637 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/threads.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     4245 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/resources/webhooks.py
-drwxr-xr-x   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-03-05 22:43:35.625626 nylas-6.1.1/nylas/utils/
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/utils/__init__.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     1715 2024-03-05 22:18:14.000000 nylas-6.1.1/nylas/utils/file_utils.py
-drwxr-xr-x   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-03-05 22:43:35.609193 nylas-6.1.1/nylas.egg-info/
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     6045 2024-03-05 22:43:35.000000 nylas-6.1.1/nylas.egg-info/PKG-INFO
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     1518 2024-03-05 22:43:35.000000 nylas-6.1.1/nylas.egg-info/SOURCES.txt
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)        1 2024-03-05 22:43:35.000000 nylas-6.1.1/nylas.egg-info/dependency_links.txt
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)      328 2024-03-05 22:43:35.000000 nylas-6.1.1/nylas.egg-info/requires.txt
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)        6 2024-03-05 22:43:35.000000 nylas-6.1.1/nylas.egg-info/top_level.txt
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)       38 2024-03-05 22:43:35.626886 nylas-6.1.1/setup.cfg
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     4406 2024-03-05 22:18:14.000000 nylas-6.1.1/setup.py
-drwxr-xr-x   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-03-05 22:43:35.626262 nylas-6.1.1/tests/
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     5342 2024-03-05 22:18:14.000000 nylas-6.1.1/tests/conftest.py
--rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3111 2024-03-05 22:18:14.000000 nylas-6.1.1/tests/test_client.py
+drwxr-xr-x   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-05-17 18:22:25.716294 nylas-6.2.0/
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     1072 2023-05-30 00:19:43.000000 nylas-6.2.0/LICENSE
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     6045 2024-05-17 18:22:25.716039 nylas-6.2.0/PKG-INFO
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     5618 2024-04-22 15:26:19.000000 nylas-6.2.0/README.md
+drwxr-xr-x   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-05-17 18:22:25.685586 nylas-6.2.0/nylas/
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)       54 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/__init__.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)       22 2024-05-17 18:21:44.000000 nylas-6.2.0/nylas/_client_sdk_version.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     4075 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/client.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     1120 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/config.py
+drwxr-xr-x   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-05-17 18:22:25.689378 nylas-6.2.0/nylas/handler/
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/handler/__init__.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     2503 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/handler/api_resources.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     6001 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/handler/http_client.py
+drwxr-xr-x   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-05-17 18:22:25.703319 nylas-6.2.0/nylas/models/
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/__init__.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     2559 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/application_details.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     1996 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/attachments.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     6777 2024-05-17 17:51:43.000000 nylas-6.2.0/nylas/models/auth.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     5609 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/availability.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3581 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/calendars.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     4183 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/connectors.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)    10893 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/contacts.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3285 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/credentials.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     6700 2024-05-03 17:30:20.000000 nylas-6.2.0/nylas/models/drafts.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     4470 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/errors.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)    26017 2024-05-17 18:12:36.000000 nylas-6.2.0/nylas/models/events.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     2670 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/folders.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     1588 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/free_busy.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3577 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/grants.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)      544 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/list_query_params.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     8804 2024-05-01 18:07:47.000000 nylas-6.2.0/nylas/models/messages.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     2710 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/redirect_uri.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3254 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/response.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)      550 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/smart_compose.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     5576 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/models/threads.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     4711 2024-05-03 17:30:20.000000 nylas-6.2.0/nylas/models/webhooks.py
+drwxr-xr-x   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-05-17 18:22:25.713690 nylas-6.2.0/nylas/resources/
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/resources/__init__.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     1295 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/resources/applications.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3771 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/resources/attachments.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     8558 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/resources/auth.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     6633 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/resources/calendars.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     4037 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/resources/connectors.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     5385 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/resources/contacts.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     4298 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/resources/credentials.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     6708 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/resources/drafts.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     5915 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/resources/events.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3777 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/resources/folders.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     2816 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/resources/grants.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     9347 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/resources/messages.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3610 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/resources/redirect_uris.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)      207 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/resources/resource.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     2219 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/resources/smart_compose.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3283 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/resources/threads.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     5403 2024-05-15 16:30:09.000000 nylas-6.2.0/nylas/resources/webhooks.py
+drwxr-xr-x   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-05-17 18:22:25.714551 nylas-6.2.0/nylas/utils/
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-04-22 15:26:19.000000 nylas-6.2.0/nylas/utils/__init__.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     2166 2024-05-03 17:49:54.000000 nylas-6.2.0/nylas/utils/file_utils.py
+drwxr-xr-x   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-05-17 18:22:25.688249 nylas-6.2.0/nylas.egg-info/
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     6045 2024-05-17 18:22:25.000000 nylas-6.2.0/nylas.egg-info/PKG-INFO
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     1518 2024-05-17 18:22:25.000000 nylas-6.2.0/nylas.egg-info/SOURCES.txt
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)        1 2024-05-17 18:22:25.000000 nylas-6.2.0/nylas.egg-info/dependency_links.txt
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)      328 2024-05-17 18:22:25.000000 nylas-6.2.0/nylas.egg-info/requires.txt
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)        6 2024-05-17 18:22:25.000000 nylas-6.2.0/nylas.egg-info/top_level.txt
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)       38 2024-05-17 18:22:25.716453 nylas-6.2.0/setup.cfg
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     4406 2024-04-22 15:26:19.000000 nylas-6.2.0/setup.py
+drwxr-xr-x   0 mostafa.r@nylas.com   (502) staff       (20)        0 2024-05-17 18:22:25.715469 nylas-6.2.0/tests/
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     6407 2024-05-03 17:30:20.000000 nylas-6.2.0/tests/conftest.py
+-rw-r--r--   0 mostafa.r@nylas.com   (502) staff       (20)     3111 2024-04-22 15:26:19.000000 nylas-6.2.0/tests/test_client.py
```

### Comparing `nylas-6.1.1/LICENSE` & `nylas-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/PKG-INFO` & `nylas-6.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nylas
-Version: 6.1.1
+Version: 6.2.0
 Summary: Python bindings for the Nylas API platform.
 Home-page: https://github.com/nylas/nylas-python
 Author: Nylas Team
 Author-email: support@nylas.com
 License: MIT
 Keywords: inbox app appserver email nylas contacts calendar
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nylas Version: 6.1.1 Summary: Python bindings for
+Metadata-Version: 2.1 Name: nylas Version: 6.2.0 Summary: Python bindings for
 the Nylas API platform. Home-page: https://github.com/nylas/nylas-python
 Author: Nylas Team Author-email: support@nylas.com License: MIT Keywords: inbox
 app appserver email nylas contacts calendar Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: test Provides-Extra: docs Provides-
 Extra: release License-File: LICENSE _[_A_i_m_e_o_s_ _l_o_g_o_]# Nylas Python SDK [![PyPI -
 Version](https://img.shields.io/pypi/v/nylas)](https://pypi.org/project/nylas/
 ) [![codecov](https://codecov.io/gh/nylas/nylas-python/branch/main/graph/
```

### Comparing `nylas-6.1.1/README.md` & `nylas-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/client.py` & `nylas-6.2.0/nylas/client.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/handler/api_resources.py` & `nylas-6.2.0/nylas/handler/api_resources.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,71 +4,91 @@
 from nylas.resources.resource import Resource
 
 # pylint: disable=too-few-public-methods,missing-class-docstring,missing-function-docstring
 
 
 class ListableApiResource(Resource):
     def list(
-        self, path, response_type, headers=None, query_params=None, request_body=None
+        self,
+        path,
+        response_type,
+        headers=None,
+        query_params=None,
+        request_body=None,
+        overrides=None,
     ) -> ListResponse:
         response_json = self._http_client._execute(
-            "GET", path, headers, query_params, request_body
+            "GET", path, headers, query_params, request_body, overrides=overrides
         )
 
         return ListResponse.from_dict(response_json, response_type)
 
 
 class FindableApiResource(Resource):
     def find(
-        self, path, response_type, headers=None, query_params=None, request_body=None
+        self,
+        path,
+        response_type,
+        headers=None,
+        query_params=None,
+        request_body=None,
+        overrides=None,
     ) -> Response:
         response_json = self._http_client._execute(
-            "GET", path, headers, query_params, request_body
+            "GET", path, headers, query_params, request_body, overrides=overrides
         )
 
         return Response.from_dict(response_json, response_type)
 
 
 class CreatableApiResource(Resource):
     def create(
-        self, path, response_type, headers=None, query_params=None, request_body=None
+        self,
+        path,
+        response_type,
+        headers=None,
+        query_params=None,
+        request_body=None,
+        overrides=None,
     ) -> Response:
         response_json = self._http_client._execute(
-            "POST", path, headers, query_params, request_body
+            "POST", path, headers, query_params, request_body, overrides=overrides
         )
 
         return Response.from_dict(response_json, response_type)
 
 
 class UpdatableApiResource(Resource):
     def update(
         self,
         path,
         response_type,
         headers=None,
         query_params=None,
         request_body=None,
         method="PUT",
+        overrides=None,
     ):
         response_json = self._http_client._execute(
-            method, path, headers, query_params, request_body
+            method, path, headers, query_params, request_body, overrides=overrides
         )
 
         return Response.from_dict(response_json, response_type)
 
 
 class DestroyableApiResource(Resource):
     def destroy(
         self,
         path,
         response_type=None,
         headers=None,
         query_params=None,
         request_body=None,
+        overrides=None,
     ):
         if response_type is None:
             response_type = DeleteResponse
 
         response_json = self._http_client._execute(
-            "DELETE", path, headers, query_params, request_body
+            "DELETE", path, headers, query_params, request_body, overrides=overrides
         )
         return response_type.from_dict(response_json)
```

### Comparing `nylas-6.1.1/nylas/models/application_details.py` & `nylas-6.2.0/nylas/models/application_details.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/models/attachments.py` & `nylas-6.2.0/nylas/models/attachments.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/models/auth.py` & `nylas-6.2.0/nylas/models/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,24 +110,26 @@
         grant_id: ID representing the new Grant.
         scope: List of scopes associated with the token.
         expires_in: The remaining lifetime of the access token, in seconds.
         email: Email address of the grant that is created.
         refresh_token: Returned only if the code is requested using "access_type=offline".
         id_token: A JWT that contains identity information about the user. Digitally signed by Nylas.
         token_type: Always "Bearer".
+        provider: The provider that the code was exchanged with.
     """
 
     access_token: str
     grant_id: str
-    scope: str
     expires_in: int
     email: Optional[str] = None
     refresh_token: Optional[str] = None
+    scope: Optional[str] = None
     id_token: Optional[str] = None
     token_type: Optional[str] = None
+    provider: Optional[Provider] = None
 
 
 @dataclass_json
 @dataclass
 class TokenInfoResponse:
     """
     Class representation of a Nylas token information response.
```

### Comparing `nylas-6.1.1/nylas/models/availability.py` & `nylas-6.2.0/nylas/models/availability.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/models/calendars.py` & `nylas-6.2.0/nylas/models/calendars.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/models/connectors.py` & `nylas-6.2.0/nylas/models/connectors.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/models/contacts.py` & `nylas-6.2.0/nylas/models/contacts.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/models/credentials.py` & `nylas-6.2.0/nylas/models/credentials.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/models/drafts.py` & `nylas-6.2.0/nylas/models/drafts.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,14 +53,27 @@
 
     label: NotRequired[str]
     links: NotRequired[bool]
     opens: NotRequired[bool]
     thread_replies: NotRequired[bool]
 
 
+class CustomHeader(TypedDict):
+    """
+    A key-value pair representing a header that can be added to drafts and outgoing messages.
+
+    Attributes:
+        name: The name of the custom header.
+        value: The value of the custom header.
+    """
+
+    name: str
+    value: str
+
+
 class CreateDraftRequest(TypedDict):
     """
     A request to create a draft.
 
     Attributes:
         subject: The subject of the message.
         to: The recipients of the message.
@@ -69,27 +82,29 @@
         reply_to: The reply-to recipients of the message.
         starred: Whether the message is starred.
         body: The body of the message.
         attachments: The attachments on the message.
         send_at: Unix timestamp to send the message at.
         reply_to_message_id: The ID of the message that you are replying to.
         tracking_options: Options for tracking opens, links, and thread replies.
+        custom_headers: Custom headers to add to the message.
     """
 
     body: NotRequired[str]
     subject: NotRequired[str]
     to: NotRequired[List[EmailName]]
     bcc: NotRequired[List[EmailName]]
     cc: NotRequired[List[EmailName]]
     reply_to: NotRequired[List[EmailName]]
     attachments: NotRequired[List[CreateAttachmentRequest]]
     starred: NotRequired[bool]
     send_at: NotRequired[int]
     reply_to_message_id: NotRequired[str]
     tracking_options: NotRequired[TrackingOptions]
+    custom_headers: NotRequired[List[CustomHeader]]
 
 
 UpdateDraftRequest = CreateDraftRequest
 """ A request to update a draft. """
 
 
 # Need to use Functional typed dicts because "from" and "in" are Python
@@ -144,11 +159,12 @@
         reply_to (NotRequired[List[EmailName]]): The reply-to recipients of the message.
         starred (NotRequired[bool]): Whether the message is starred.
         body (NotRequired[str]): The body of the message.
         attachments (NotRequired[List[CreateAttachmentRequest]]): The attachments on the message.
         send_at (NotRequired[int]): Unix timestamp to send the message at.
         reply_to_message_id (NotRequired[str]): The ID of the message that you are replying to.
         tracking_options (NotRequired[TrackingOptions]): Options for tracking opens, links, and thread replies.
+        custom_headers(NotRequired[List[CustomHeader]]): Custom headers to add to the message.
         use_draft: Whether or not to use draft support. This is primarily used when dealing with large attachments.
     """
 
     use_draft: NotRequired[bool]
```

### Comparing `nylas-6.1.1/nylas/models/errors.py` & `nylas-6.2.0/nylas/models/errors.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/models/events.py` & `nylas-6.2.0/nylas/models/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 ParticipantStatus = Literal["noreply", "yes", "no", "maybe"]
 """ Literal representing the status of an Event participant. """
 
 SendRsvpStatus = Literal["yes", "no", "maybe"]
 """ Literal representing the status of an RSVP. """
 
+EventType = Literal["default", "outOfOffice", "focusTime", "workingLocation"]
+""" Literal representing the event type to filter by. """
+
 
 @dataclass_json
 @dataclass
 class Participant:
     """
     Interface representing an Event participant.
 
@@ -30,15 +33,15 @@
         name: Participant's name.
         status: Participant's status.
         comment: Comment by the participant.
         phone_number: Participant's phone number.
     """
 
     email: str
-    status: ParticipantStatus
+    status: Optional[ParticipantStatus] = None
     name: Optional[str] = None
     comment: Optional[str] = None
     phone_number: Optional[str] = None
 
 
 class EmailName(TypedDict):
     """
@@ -312,20 +315,20 @@
     """
 
     id: str
     grant_id: str
     calendar_id: str
     busy: bool
     participants: List[Participant]
-    visibility: Visibility
     when: When = field(metadata=config(decoder=_decode_when))
     conferencing: Optional[Conferencing] = field(
         default=None, metadata=config(decoder=_decode_conferencing)
     )
     object: str = "event"
+    visibility: Optional[Visibility] = None
     read_only: Optional[bool] = None
     description: Optional[str] = None
     location: Optional[str] = None
     ical_uid: Optional[str] = None
     title: Optional[str] = None
     html_link: Optional[str] = None
     hide_participants: Optional[bool] = None
@@ -718,27 +721,30 @@
         busy: Returns events with a busy status of true.
         order_by: Order results by the specified field.
             Currently only start is supported.
         limit (NotRequired[int]): The maximum number of objects to return.
             This field defaults to 50. The maximum allowed value is 200.
         page_token (NotRequired[str]): An identifier that specifies which page of data to return.
             This value should be taken from a ListResponse object's next_cursor parameter.
+        event_type (NotRequired[List[EventType]]): (Google only) Filter events by event type.
+            You can pass the query parameter multiple times to select or exclude multiple event types.
     """
 
     calendar_id: str
     show_cancelled: NotRequired[bool]
     title: NotRequired[str]
     description: NotRequired[str]
     location: NotRequired[str]
     start: NotRequired[int]
     end: NotRequired[int]
     metadata_pair: NotRequired[Dict[str, Any]]
     expand_recurring: NotRequired[bool]
     busy: NotRequired[bool]
     order_by: NotRequired[str]
+    event_type: NotRequired[List[EventType]]
 
 
 class CreateEventQueryParams(TypedDict):
     """
     Interface representing of the query parameters for creating an event.
 
     Attributes:
```

### Comparing `nylas-6.1.1/nylas/models/folders.py` & `nylas-6.2.0/nylas/models/folders.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/models/free_busy.py` & `nylas-6.2.0/nylas/models/free_busy.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/models/grants.py` & `nylas-6.2.0/nylas/models/grants.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/models/list_query_params.py` & `nylas-6.2.0/nylas/models/list_query_params.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/models/messages.py` & `nylas-6.2.0/nylas/models/messages.py`

 * *Files 25% similar despite different names*

```diff
@@ -194,7 +194,60 @@
     The response from stopping a scheduled message.
 
     Attributes:
         message: A message describing the result of the request.
     """
 
     message: str
+
+
+class CleanMessagesRequest(TypedDict):
+    """
+    Request to clean a list of messages.
+
+    Attributes:
+        message_id: IDs of the email messages to clean.
+        ignore_links: If true, removes link-related tags (<a>) from the email message while keeping the text.
+        ignore_images: If true, removes images from the email message.
+        images_as_markdown: If true, converts images in the email message to Markdown.
+        ignore_tables: If true, removes table-related tags (<table>, <th>, <td>, <tr>) from the email message while
+            keeping rows.
+        remove_conclusion_phrases: If true, removes phrases such as "Best" and "Regards" in the email message signature.
+    """
+
+    message_id: List[str]
+    ignore_links: NotRequired[bool]
+    ignore_images: NotRequired[bool]
+    images_as_markdown: NotRequired[bool]
+    ignore_tables: NotRequired[bool]
+    remove_conclusion_phrases: NotRequired[bool]
+
+
+@dataclass_json
+@dataclass
+class CleanMessagesResponse(Message):
+    """
+    Message object with the cleaned HTML message body.
+
+    Attributes:
+        id (str): Globally unique object identifier.
+        grant_id (str): The grant that this message belongs to.
+        from_ (List[EmailName]): The sender of the message.
+        date (int): The date the message was received.
+        object: The type of object.
+        thread_id (Optional[str]): The thread that this message belongs to.
+        subject (Optional[str]): The subject of the message.
+        to (Optional[List[EmailName]]): The recipients of the message.
+        cc (Optional[List[EmailName]]): The CC recipients of the message.
+        bcc (Optional[List[EmailName]]): The BCC recipients of the message.
+        reply_to (Optional[List[EmailName]]): The reply-to recipients of the message.
+        unread (Optional[bool]): Whether the message is unread.
+        starred (Optional[bool]): Whether the message is starred.
+        snippet (Optional[str]): A snippet of the message body.
+        body (Optional[str]): The body of the message.
+        attachments (Optional[List[Attachment]]): The attachments on the message.
+        folders (Optional[List[str]]): The folders that the message is in.
+        created_at (Optional[int]): Unix timestamp of when the message was created.
+        conversation (str): The cleaned HTML message body.
+    """
+
+    conversation: str = ""
```

### Comparing `nylas-6.1.1/nylas/models/redirect_uri.py` & `nylas-6.2.0/nylas/models/redirect_uri.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/models/response.py` & `nylas-6.2.0/nylas/models/response.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/models/smart_compose.py` & `nylas-6.2.0/nylas/models/smart_compose.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/models/threads.py` & `nylas-6.2.0/nylas/models/threads.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/nylas/models/webhooks.py` & `nylas-6.2.0/nylas/models/webhooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,20 @@
     EVENT_DELETED = "event.deleted"
     GRANT_CREATED = "grant.created"
     GRANT_UPDATED = "grant.updated"
     GRANT_DELETED = "grant.deleted"
     GRANT_EXPIRED = "grant.expired"
     MESSAGE_SEND_SUCCESS = "message.send_success"
     MESSAGE_SEND_FAILED = "message.send_failed"
+    MESSAGE_BOUNCE_DETECTED = "message.bounce_detected"
+    MESSAGE_CREATED = "message.created"
+    MESSAGE_UPDATED = "message.updated"
+    MESSAGE_OPENED = "message.opened"
+    MESSAGE_LINK_CLICKED = "message.link_clicked"
+    THREAD_REPLIED = "thread.replied"
 
 
 @dataclass_json
 @dataclass
 class Webhook:
     """
     Class representing a Nylas webhook.
```

### Comparing `nylas-6.1.1/nylas/resources/applications.py` & `nylas-6.2.0/nylas/resources/applications.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from nylas.config import RequestOverrides
 from nylas.models.application_details import ApplicationDetails
 from nylas.models.response import Response
 from nylas.resources.redirect_uris import RedirectUris
 from nylas.resources.resource import Resource
 
 
 class Applications(Resource):
@@ -18,19 +19,22 @@
         Manage Redirect URIs for your Nylas Application.
 
         Returns:
             RedirectUris: The redirect URIs associated with your Nylas Application.
         """
         return RedirectUris(self._http_client)
 
-    def info(self) -> Response[ApplicationDetails]:
+    def info(self, overrides: RequestOverrides = None) -> Response[ApplicationDetails]:
         """
         Get the application information.
 
+        Args:
+            overrides: The query parameters to include in the request.
+
         Returns:
             Response: The application information.
         """
 
         json_response = self._http_client._execute(
-            method="GET", path="/v3/applications"
+            method="GET", path="/v3/applications", overrides=overrides
         )
         return Response.from_dict(json_response, ApplicationDetails)
```

### Comparing `nylas-6.1.1/nylas/resources/attachments.py` & `nylas-6.2.0/nylas/resources/attachments.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from requests import Response
 
+from nylas.config import RequestOverrides
 from nylas.handler.api_resources import (
     FindableApiResource,
 )
 from nylas.models.attachments import Attachment, FindAttachmentQueryParams
 from nylas.models.response import Response as NylasResponse
 
 
@@ -17,49 +18,54 @@
     """
 
     def find(
         self,
         identifier: str,
         attachment_id: str,
         query_params: FindAttachmentQueryParams,
+        overrides: RequestOverrides = None,
     ) -> NylasResponse[Attachment]:
         """
         Return metadata of an attachment.
 
         Args:
             identifier: The identifier of the Grant to act upon.
             attachment_id: The id of the attachment to retrieve.
             query_params: The query parameters to include in the request.
+            overrides: The request overrides to use for the request.
 
         Returns:
             The attachment metadata.
         """
         return super().find(
             path=f"/v3/grants/{identifier}/attachments/{attachment_id}",
             response_type=Attachment,
             query_params=query_params,
+            overrides=overrides,
         )
 
     def download(
         self,
         identifier: str,
         attachment_id: str,
         query_params: FindAttachmentQueryParams,
+        overrides: RequestOverrides = None,
     ) -> Response:
         """
         Download the attachment data.
 
         This function returns a raw response object to allow you the ability
         to stream the file contents. The response object should be closed
         after use to ensure the connection is closed.
 
         Args:
             identifier: The identifier of the Grant to act upon.
             attachment_id: The id of the attachment to download.
             query_params: The query parameters to include in the request.
+            overrides: The request overrides to use for the request.
 
         Returns:
             The Response object containing the file data.
 
         Example:
             Here is an example of how to use this function when streaming:
 
@@ -74,31 +80,35 @@
                     response.close()  # Ensure the response is closed
             ```
         """
         return self._http_client._execute_download_request(
             path=f"/v3/grants/{identifier}/attachments/{attachment_id}/download",
             query_params=query_params,
             stream=True,
+            overrides=overrides,
         )
 
     def download_bytes(
         self,
         identifier: str,
         attachment_id: str,
         query_params: FindAttachmentQueryParams,
+        overrides: RequestOverrides = None,
     ) -> bytes:
         """
         Download the attachment as a byte array.
 
         Args:
             identifier: The identifier of the Grant to act upon.
             attachment_id: The id of the attachment to download.
             query_params: The query parameters to include in the request.
+            overrides: The request overrides to use for the request.
 
         Returns:
             The raw file data.
         """
         return self._http_client._execute_download_request(
             path=f"/v3/grants/{identifier}/attachments/{attachment_id}/download",
             query_params=query_params,
             stream=False,
+            overrides=overrides,
         )
```

### Comparing `nylas-6.1.1/nylas/resources/contacts.py` & `nylas-6.2.0/nylas/resources/contacts.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from nylas.config import RequestOverrides
 from nylas.handler.api_resources import (
     ListableApiResource,
     FindableApiResource,
     CreatableApiResource,
     UpdatableApiResource,
     DestroyableApiResource,
 )
@@ -27,123 +28,155 @@
     """
     Nylas Contacts API
 
     The Contacts API allows you to manage contacts and contact groups for a user.
     """
 
     def list(
-        self, identifier: str, query_params: ListContactsQueryParams = None
+        self,
+        identifier: str,
+        query_params: ListContactsQueryParams = None,
+        overrides: RequestOverrides = None,
     ) -> ListResponse[Contact]:
         """
         Return all Contacts.
 
         Attributes:
             identifier: The identifier of the Grant to act upon.
             query_params: The query parameters to include in the request.
+            overrides: The request overrides to use for the request.
 
         Returns:
             The list of contacts.
         """
 
         return super().list(
             path=f"/v3/grants/{identifier}/contacts",
             query_params=query_params,
             response_type=Contact,
+            overrides=overrides,
         )
 
     def find(
         self,
         identifier: str,
         contact_id: str,
         query_params: FindContactQueryParams = None,
+        overrides: RequestOverrides = None,
     ) -> Response[Contact]:
         """
         Return a Contact.
 
         Attributes:
             identifier: The identifier of the Grant to act upon.
             contact_id: The ID of the contact to retrieve.
             query_params: The query parameters to include in the request.
+            overrides: The request overrides to use for the request.
 
         Returns:
             The contact.
         """
         return super().find(
             path=f"/v3/grants/{identifier}/contacts/{contact_id}",
             response_type=Contact,
             query_params=query_params,
+            overrides=overrides,
         )
 
     def create(
-        self, identifier: str, request_body: CreateContactRequest
+        self,
+        identifier: str,
+        request_body: CreateContactRequest,
+        overrides: RequestOverrides = None,
     ) -> Response[Contact]:
         """
         Create a Contact.
 
         Attributes:
             identifier: The identifier of the Grant to act upon.
             request_body: The values to create the Contact with.
+            overrides: The request overrides to use for the request.
 
         Returns:
             The created contact.
         """
         return super().create(
             path=f"/v3/grants/{identifier}/contacts",
             response_type=Contact,
             request_body=request_body,
+            overrides=overrides,
         )
 
     def update(
-        self, identifier: str, contact_id: str, request_body: UpdateContactRequest
+        self,
+        identifier: str,
+        contact_id: str,
+        request_body: UpdateContactRequest,
+        overrides: RequestOverrides = None,
     ) -> Response[Contact]:
         """
         Update a Contact.
 
         Attributes:
             identifier: The identifier of the Grant to act upon.
             contact_id: The ID of the Contact to update.
                 Use "primary" to refer to the primary Contact associated with the Grant.
             request_body: The values to update the Contact with.
+            overrides: The request overrides to use for the request.
 
         Returns:
             The updated contact.
         """
         return super().update(
             path=f"/v3/grants/{identifier}/contacts/{contact_id}",
             response_type=Contact,
             request_body=request_body,
+            overrides=overrides,
         )
 
-    def destroy(self, identifier: str, contact_id: str) -> DeleteResponse:
+    def destroy(
+        self,
+        identifier: str,
+        contact_id: str,
+        overrides: RequestOverrides = None,
+    ) -> DeleteResponse:
         """
         Delete a Contact.
 
         Attributes:
             identifier: The identifier of the Grant to act upon.
             contact_id: The ID of the Contact to delete.
                 Use "primary" to refer to the primary Contact associated with the Grant.
+            overrides: The request overrides to use for the request.
 
         Returns:
             The deletion response.
         """
-        return super().destroy(path=f"/v3/grants/{identifier}/contacts/{contact_id}")
+        return super().destroy(
+            path=f"/v3/grants/{identifier}/contacts/{contact_id}", overrides=overrides
+        )
 
     def list_groups(
-        self, identifier: str, query_params: ListContactGroupsQueryParams = None
+        self,
+        identifier: str,
+        query_params: ListContactGroupsQueryParams = None,
+        overrides: RequestOverrides = None,
     ) -> ListResponse[ContactGroup]:
         """
         Return all contact groups.
 
         Attributes:
             identifier: The identifier of the Grant to act upon.
             query_params: The query parameters to include in the request.
+            overrides: The request overrides to use for the request.
 
         Returns:
             The list of contact groups.
         """
         json_response = self._http_client._execute(
             method="GET",
             path=f"/v3/grants/{identifier}/contacts/groups",
             query_params=query_params,
+            overrides=overrides,
         )
 
         return ListResponse.from_dict(json_response, ContactGroup)
```

### Comparing `nylas-6.1.1/nylas/resources/folders.py` & `nylas-6.2.0/nylas/resources/folders.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from nylas.config import RequestOverrides
 from nylas.handler.api_resources import (
     ListableApiResource,
     FindableApiResource,
     CreatableApiResource,
     UpdatableApiResource,
     DestroyableApiResource,
 )
@@ -22,90 +23,122 @@
 ):
     """
     Nylas Folders API
 
     The Nylas folders API allows you to create new folders or manage existing ones.
     """
 
-    def list(self, identifier: str) -> ListResponse[Folder]:
+    def list(
+        self,
+        identifier: str,
+        overrides: RequestOverrides = None,
+    ) -> ListResponse[Folder]:
         """
         Return all Folders.
 
         Args:
             identifier: The identifier of the Grant to act upon.
+            overrides: The request overrides to use.
 
         Returns:
             The list of Folders.
         """
 
         return super().list(
             path=f"/v3/grants/{identifier}/folders",
             response_type=Folder,
+            overrides=overrides,
         )
 
-    def find(self, identifier: str, folder_id: str) -> Response[Folder]:
+    def find(
+        self,
+        identifier: str,
+        folder_id: str,
+        overrides: RequestOverrides = None,
+    ) -> Response[Folder]:
         """
         Return a Folder.
 
         Args:
             identifier: The identifier of the Grant to act upon.
             folder_id: The ID of the Folder to retrieve.
+            overrides: The request overrides to use.
 
         Returns:
             The Folder.
         """
         return super().find(
             path=f"/v3/grants/{identifier}/folders/{folder_id}",
             response_type=Folder,
+            overrides=overrides,
         )
 
     def create(
-        self, identifier: str, request_body: CreateFolderRequest
+        self,
+        identifier: str,
+        request_body: CreateFolderRequest,
+        overrides: RequestOverrides = None,
     ) -> Response[Folder]:
         """
         Create a Folder.
 
         Args:
             identifier: The identifier of the Grant to act upon.
             request_body: The values to create the Folder with.
+            overrides: The request overrides to use.
 
         Returns:
             The created Folder.
         """
         return super().create(
             path=f"/v3/grants/{identifier}/folders",
             response_type=Folder,
             request_body=request_body,
+            overrides=overrides,
         )
 
     def update(
-        self, identifier: str, folder_id: str, request_body: UpdateFolderRequest
+        self,
+        identifier: str,
+        folder_id: str,
+        request_body: UpdateFolderRequest,
+        overrides: RequestOverrides = None,
     ) -> Response[Folder]:
         """
         Update a Folder.
 
         Args:
             identifier: The identifier of the Grant to act upon.
             folder_id: The ID of the Folder to update.
             request_body: The values to update the Folder with.
+            overrides: The request overrides to use.
 
         Returns:
             The updated Folder.
         """
         return super().update(
             path=f"/v3/grants/{identifier}/folders/{folder_id}",
             response_type=Folder,
             request_body=request_body,
+            overrides=overrides,
         )
 
-    def destroy(self, identifier: str, folder_id: str) -> DeleteResponse:
+    def destroy(
+        self,
+        identifier: str,
+        folder_id: str,
+        overrides: RequestOverrides = None,
+    ) -> DeleteResponse:
         """
         Delete a Folder.
 
         Args:
             identifier: The identifier of the Grant to act upon.
             folder_id: The ID of the Folder to delete.
+            overrides: The request overrides to use.
 
         Returns:
             The deletion response.
         """
-        return super().destroy(path=f"/v3/grants/{identifier}/folders/{folder_id}")
+        return super().destroy(
+            path=f"/v3/grants/{identifier}/folders/{folder_id}", overrides=overrides
+        )
```

### Comparing `nylas-6.1.1/nylas/resources/grants.py` & `nylas-6.2.0/nylas/resources/grants.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from nylas.config import RequestOverrides
 from nylas.handler.api_resources import (
     ListableApiResource,
     FindableApiResource,
     UpdatableApiResource,
     DestroyableApiResource,
 )
 from nylas.models.grants import (
@@ -23,67 +24,88 @@
 
     The Grants API allows you to find and manage existing grants for your Nylas application.
 
     Grants represent a specific set of permissions ("scopes") that a specific end user granted Nylas
     for a specific service provider
     """
 
-    def list(self, query_params: ListGrantsQueryParams = None) -> ListResponse[Grant]:
+    def list(
+        self,
+        query_params: ListGrantsQueryParams = None,
+        overrides: RequestOverrides = None,
+    ) -> ListResponse[Grant]:
         """
         Return all Grants.
 
         Args:
             query_params: The query parameters to include in the request.
+            overrides: The request overrides to use.
 
         Returns:
             A list of Grants.
         """
 
         return super().list(
-            path="/v3/grants", response_type=Grant, query_params=query_params
+            path="/v3/grants",
+            response_type=Grant,
+            query_params=query_params,
+            overrides=overrides,
         )
 
-    def find(self, grant_id: str) -> Response[Grant]:
+    def find(
+        self, grant_id: str, overrides: RequestOverrides = None
+    ) -> Response[Grant]:
         """
         Return a Grant.
 
         Args:
             grant_id: The ID of the Grant to retrieve.
+            overrides: The request overrides to use.
 
         Returns:
             The Grant.
         """
 
-        return super().find(path=f"/v3/grants/{grant_id}", response_type=Grant)
+        return super().find(
+            path=f"/v3/grants/{grant_id}", response_type=Grant, overrides=overrides
+        )
 
     def update(
-        self, grant_id: str, request_body: UpdateGrantRequest
+        self,
+        grant_id: str,
+        request_body: UpdateGrantRequest,
+        overrides: RequestOverrides = None,
     ) -> Response[Grant]:
         """
         Update a Grant.
 
         Args:
             grant_id: The ID of the Grant to update.
             request_body: The values to update the Grant with.
+            overrides: The request overrides to use.
 
         Returns:
             The updated Grant.
         """
 
         return super().update(
             path=f"/v3/grants/{grant_id}",
             response_type=Grant,
             request_body=request_body,
+            overrides=overrides,
         )
 
-    def destroy(self, grant_id: str) -> DeleteResponse:
+    def destroy(
+        self, grant_id: str, overrides: RequestOverrides = None
+    ) -> DeleteResponse:
         """
         Delete a Grant.
 
         Args:
             grant_id: The ID of the Grant to delete.
+            overrides: The request overrides to use.
 
         Returns:
             The deletion response.
         """
 
-        return super().destroy(path=f"/v3/grants/{grant_id}")
+        return super().destroy(path=f"/v3/grants/{grant_id}", overrides=overrides)
```

### Comparing `nylas-6.1.1/nylas.egg-info/PKG-INFO` & `nylas-6.2.0/nylas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nylas
-Version: 6.1.1
+Version: 6.2.0
 Summary: Python bindings for the Nylas API platform.
 Home-page: https://github.com/nylas/nylas-python
 Author: Nylas Team
 Author-email: support@nylas.com
 License: MIT
 Keywords: inbox app appserver email nylas contacts calendar
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nylas Version: 6.1.1 Summary: Python bindings for
+Metadata-Version: 2.1 Name: nylas Version: 6.2.0 Summary: Python bindings for
 the Nylas API platform. Home-page: https://github.com/nylas/nylas-python
 Author: Nylas Team Author-email: support@nylas.com License: MIT Keywords: inbox
 app appserver email nylas contacts calendar Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: test Provides-Extra: docs Provides-
 Extra: release License-File: LICENSE _[_A_i_m_e_o_s_ _l_o_g_o_]# Nylas Python SDK [![PyPI -
 Version](https://img.shields.io/pypi/v/nylas)](https://pypi.org/project/nylas/
 ) [![codecov](https://codecov.io/gh/nylas/nylas-python/branch/main/graph/
```

### Comparing `nylas-6.1.1/nylas.egg-info/SOURCES.txt` & `nylas-6.2.0/nylas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/setup.py` & `nylas-6.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `nylas-6.1.1/tests/conftest.py` & `nylas-6.2.0/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -109,14 +109,15 @@
         "access_token": "nylas_access_token",
         "expires_in": 3600,
         "id_token": "jwt_token",
         "refresh_token": "nylas_refresh_token",
         "scope": "https://www.googleapis.com/auth/gmail.readonly profile",
         "token_type": "Bearer",
         "grant_id": "grant_123",
+        "provider": "google",
     }
     return mock_http_client
 
 
 @pytest.fixture
 def http_client_token_info():
     mock_http_client = Mock()
@@ -185,7 +186,36 @@
                 "schedule_id": "rb856334-6d95-432c-86d1-c5dab0ce98be",
                 "status": {"code": "sucess", "description": "schedule send succeeded"},
                 "close_time": 1690579819,
             },
         ],
     }
     return mock_http_client
+
+
+@pytest.fixture
+def http_client_clean_messages():
+    mock_http_client = Mock()
+    mock_http_client._execute.return_value = {
+        "request_id": "dd3ec9a2-8f15-403d-b269-32b1f1beb9f5",
+        "data": [
+            {
+                "body": "Hello, I just sent a message using Nylas!",
+                "from": [
+                    {"name": "Daenerys Targaryen", "email": "daenerys.t@example.com"}
+                ],
+                "grant_id": "41009df5-bf11-4c97-aa18-b285b5f2e386",
+                "id": "message-1",
+                "object": "message",
+                "conversation": "cleaned example",
+            },
+            {
+                "body": "Hello, this is a test message!",
+                "from": [{"name": "Michael Scott", "email": "m.scott@email.com"}],
+                "grant_id": "41009df5-bf11-4c97-aa18-b285b5f2e386",
+                "id": "message-2",
+                "object": "message",
+                "conversation": "another example",
+            },
+        ],
+    }
+    return mock_http_client
```

### Comparing `nylas-6.1.1/tests/test_client.py` & `nylas-6.2.0/tests/test_client.py`

 * *Files identical despite different names*

