# Comparing `tmp/gravitino-0.5.0.dev20.tar.gz` & `tmp/gravitino-0.5.0.dev21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitino-0.5.0.dev20.tar", last modified: Thu May 16 14:46:52 2024, max compression
+gzip compressed data, was "gravitino-0.5.0.dev21.tar", last modified: Fri May 17 08:55:50 2024, max compression
```

## Comparing `gravitino-0.5.0.dev20.tar` & `gravitino-0.5.0.dev21.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-16 14:46:52.985937 gravitino-0.5.0.dev20/
--rw-r--r--   0 xun        (501) staff       (20)       71 2024-05-16 14:24:20.000000 gravitino-0.5.0.dev20/MANIFEST.in
--rw-r--r--   0 xun        (501) staff       (20)     6345 2024-05-16 14:46:52.985724 gravitino-0.5.0.dev20/PKG-INFO
--rw-r--r--   0 xun        (501) staff       (20)     5390 2024-05-16 14:46:52.000000 gravitino-0.5.0.dev20/README.md
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-16 14:46:52.968614 gravitino-0.5.0.dev20/gravitino/
--rw-r--r--   0 xun        (501) staff       (20)      649 2024-05-15 07:09:38.000000 gravitino-0.5.0.dev20/gravitino/__init__.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-16 14:46:52.972750 gravitino-0.5.0.dev20/gravitino/api/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev20/gravitino/api/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      943 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/api/audit.py
--rw-r--r--   0 xun        (501) staff       (20)      441 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/api/auditable.py
--rw-r--r--   0 xun        (501) staff       (20)     4160 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/api/catalog.py
--rw-r--r--   0 xun        (501) staff       (20)     8760 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/api/catalog_change.py
--rw-r--r--   0 xun        (501) staff       (20)     3558 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/api/fileset.py
--rw-r--r--   0 xun        (501) staff       (20)     9227 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/api/fileset_change.py
--rw-r--r--   0 xun        (501) staff       (20)     1156 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/api/metalake.py
--rw-r--r--   0 xun        (501) staff       (20)     3408 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/api/metalake_change.py
--rw-r--r--   0 xun        (501) staff       (20)     1045 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/api/schema.py
--rw-r--r--   0 xun        (501) staff       (20)     4848 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/api/schema_change.py
--rw-r--r--   0 xun        (501) staff       (20)     3885 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/api/supports_schemas.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-16 14:46:52.973411 gravitino-0.5.0.dev20/gravitino/catalog/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-05-15 07:09:38.000000 gravitino-0.5.0.dev20/gravitino/catalog/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     7452 2024-05-15 07:09:38.000000 gravitino-0.5.0.dev20/gravitino/catalog/base_schema_catalog.py
--rw-r--r--   0 xun        (501) staff       (20)     7555 2024-05-15 07:09:38.000000 gravitino-0.5.0.dev20/gravitino/catalog/fileset_catalog.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-16 14:46:52.975059 gravitino-0.5.0.dev20/gravitino/client/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev20/gravitino/client/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     4795 2024-05-14 03:08:07.000000 gravitino-0.5.0.dev20/gravitino/client/gravitino_admin_client.py
--rw-r--r--   0 xun        (501) staff       (20)     2818 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/client/gravitino_client.py
--rw-r--r--   0 xun        (501) staff       (20)     2528 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/client/gravitino_client_base.py
--rw-r--r--   0 xun        (501) staff       (20)     7620 2024-05-14 03:08:07.000000 gravitino-0.5.0.dev20/gravitino/client/gravitino_metalake.py
--rw-r--r--   0 xun        (501) staff       (20)      432 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/client/gravitino_version.py
--rw-r--r--   0 xun        (501) staff       (20)      119 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev20/gravitino/constants.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-16 14:46:52.977135 gravitino-0.5.0.dev20/gravitino/dto/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev20/gravitino/dto/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     1778 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/audit_dto.py
--rw-r--r--   0 xun        (501) staff       (20)     1622 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/catalog_dto.py
--rw-r--r--   0 xun        (501) staff       (20)     3038 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/dto_converters.py
--rw-r--r--   0 xun        (501) staff       (20)     1328 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/fileset_dto.py
--rw-r--r--   0 xun        (501) staff       (20)     1944 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/metalake_dto.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-16 14:46:52.980489 gravitino-0.5.0.dev20/gravitino/dto/requests/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev20/gravitino/dto/requests/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     1632 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/requests/catalog_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     2659 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/requests/catalog_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1081 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/requests/catalog_updates_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1506 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/requests/fileset_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     4267 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/requests/fileset_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)      767 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/requests/fileset_updates_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1096 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/requests/metalake_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     4146 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/requests/metalake_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1030 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/requests/metalake_updates_request.py
--rw-r--r--   0 xun        (501) staff       (20)      935 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/requests/schema_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     2520 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/requests/schema_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1007 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/requests/schema_updates_request.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-16 14:46:52.982029 gravitino-0.5.0.dev20/gravitino/dto/responses/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev20/gravitino/dto/responses/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      684 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/responses/base_response.py
--rw-r--r--   0 xun        (501) staff       (20)      575 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/responses/catalog_list_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1077 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/responses/catalog_response.py
--rw-r--r--   0 xun        (501) staff       (20)      477 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/responses/drop_response.py
--rw-r--r--   0 xun        (501) staff       (20)      874 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/responses/entity_list_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1111 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/responses/fileset_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1163 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/responses/metalake_list_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1112 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/responses/metalake_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1079 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/responses/schema_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1397 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/dto/schema_dto.py
--rw-r--r--   0 xun        (501) staff       (20)      434 2024-05-14 03:08:07.000000 gravitino-0.5.0.dev20/gravitino/dto/version_dto.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-16 14:46:52.983518 gravitino-0.5.0.dev20/gravitino/exceptions/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev20/gravitino/exceptions/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      302 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev20/gravitino/exceptions/gravitino_runtime_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      363 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev20/gravitino/exceptions/illegal_name_identifier_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      352 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev20/gravitino/exceptions/illegal_namespace_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      289 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/exceptions/no_such_metalake_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      324 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/exceptions/not_found_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev20/gravitino/exceptions.py
--rw-r--r--   0 xun        (501) staff       (20)     4404 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev20/gravitino/gravitino_client.py
--rw-r--r--   0 xun        (501) staff       (20)     9440 2024-05-14 03:08:07.000000 gravitino-0.5.0.dev20/gravitino/name_identifier.py
--rw-r--r--   0 xun        (501) staff       (20)     7759 2024-05-14 03:08:07.000000 gravitino-0.5.0.dev20/gravitino/namespace.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-16 14:46:52.983960 gravitino-0.5.0.dev20/gravitino/rest/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-05-15 07:09:38.000000 gravitino-0.5.0.dev20/gravitino/rest/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     1200 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev20/gravitino/rest/rest_message.py
--rw-r--r--   0 xun        (501) staff       (20)     2430 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev20/gravitino/service.py
--rw-r--r--   0 xun        (501) staff       (20)      321 2024-05-14 03:08:07.000000 gravitino-0.5.0.dev20/gravitino/typing.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-16 14:46:52.984551 gravitino-0.5.0.dev20/gravitino/utils/
--rw-r--r--   0 xun        (501) staff       (20)      175 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev20/gravitino/utils/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     2692 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev20/gravitino/utils/exceptions.py
--rw-r--r--   0 xun        (501) staff       (20)     5529 2024-05-14 03:08:07.000000 gravitino-0.5.0.dev20/gravitino/utils/http_client.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-16 14:46:52.985141 gravitino-0.5.0.dev20/gravitino.egg-info/
--rw-r--r--   0 xun        (501) staff       (20)     6345 2024-05-16 14:46:52.000000 gravitino-0.5.0.dev20/gravitino.egg-info/PKG-INFO
--rw-r--r--   0 xun        (501) staff       (20)     2864 2024-05-16 14:46:52.000000 gravitino-0.5.0.dev20/gravitino.egg-info/SOURCES.txt
--rw-r--r--   0 xun        (501) staff       (20)        1 2024-05-16 14:46:52.000000 gravitino-0.5.0.dev20/gravitino.egg-info/dependency_links.txt
--rw-r--r--   0 xun        (501) staff       (20)       78 2024-05-16 14:46:52.000000 gravitino-0.5.0.dev20/gravitino.egg-info/requires.txt
--rw-r--r--   0 xun        (501) staff       (20)       10 2024-05-16 14:46:52.000000 gravitino-0.5.0.dev20/gravitino.egg-info/top_level.txt
--rw-r--r--   0 xun        (501) staff       (20)      146 2024-05-15 07:09:38.000000 gravitino-0.5.0.dev20/requirements-dev.txt
--rw-r--r--   0 xun        (501) staff       (20)      176 2024-05-15 07:09:38.000000 gravitino-0.5.0.dev20/requirements.txt
--rw-r--r--   0 xun        (501) staff       (20)       38 2024-05-16 14:46:52.985979 gravitino-0.5.0.dev20/setup.cfg
--rw-r--r--   0 xun        (501) staff       (20)     1287 2024-05-16 14:46:43.000000 gravitino-0.5.0.dev20/setup.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-16 14:46:52.984835 gravitino-0.5.0.dev20/tests/
--rw-r--r--   0 xun        (501) staff       (20)     2192 2024-05-15 07:09:38.000000 gravitino-0.5.0.dev20/tests/test_gravitino_client.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-17 08:55:50.904673 gravitino-0.5.0.dev21/
+-rw-r--r--   0 xun        (501) staff       (20)      173 2024-05-17 03:32:45.000000 gravitino-0.5.0.dev21/MANIFEST.in
+-rw-r--r--   0 xun        (501) staff       (20)     6355 2024-05-17 08:55:50.904425 gravitino-0.5.0.dev21/PKG-INFO
+-rw-r--r--   0 xun        (501) staff       (20)     5392 2024-05-17 08:55:49.000000 gravitino-0.5.0.dev21/README.md
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-17 08:55:50.886518 gravitino-0.5.0.dev21/gravitino/
+-rw-r--r--   0 xun        (501) staff       (20)      649 2024-05-15 07:09:38.000000 gravitino-0.5.0.dev21/gravitino/__init__.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-17 08:55:50.890803 gravitino-0.5.0.dev21/gravitino/api/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev21/gravitino/api/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      943 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/api/audit.py
+-rw-r--r--   0 xun        (501) staff       (20)      441 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/api/auditable.py
+-rw-r--r--   0 xun        (501) staff       (20)     4160 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/api/catalog.py
+-rw-r--r--   0 xun        (501) staff       (20)     8760 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/api/catalog_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     3558 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/api/fileset.py
+-rw-r--r--   0 xun        (501) staff       (20)     9227 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/api/fileset_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     1156 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/api/metalake.py
+-rw-r--r--   0 xun        (501) staff       (20)     3408 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/api/metalake_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     1045 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/api/schema.py
+-rw-r--r--   0 xun        (501) staff       (20)     4848 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/api/schema_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     3885 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/api/supports_schemas.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-17 08:55:50.891514 gravitino-0.5.0.dev21/gravitino/catalog/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-05-15 07:09:38.000000 gravitino-0.5.0.dev21/gravitino/catalog/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     7452 2024-05-15 07:09:38.000000 gravitino-0.5.0.dev21/gravitino/catalog/base_schema_catalog.py
+-rw-r--r--   0 xun        (501) staff       (20)     7555 2024-05-15 07:09:38.000000 gravitino-0.5.0.dev21/gravitino/catalog/fileset_catalog.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-17 08:55:50.893636 gravitino-0.5.0.dev21/gravitino/client/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev21/gravitino/client/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     4795 2024-05-14 03:08:07.000000 gravitino-0.5.0.dev21/gravitino/client/gravitino_admin_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     2818 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/client/gravitino_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     2528 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/client/gravitino_client_base.py
+-rw-r--r--   0 xun        (501) staff       (20)     7620 2024-05-14 03:08:07.000000 gravitino-0.5.0.dev21/gravitino/client/gravitino_metalake.py
+-rw-r--r--   0 xun        (501) staff       (20)      432 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/client/gravitino_version.py
+-rw-r--r--   0 xun        (501) staff       (20)      119 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev21/gravitino/constants.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-17 08:55:50.895761 gravitino-0.5.0.dev21/gravitino/dto/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev21/gravitino/dto/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1778 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/audit_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     1622 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/catalog_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     3038 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/dto_converters.py
+-rw-r--r--   0 xun        (501) staff       (20)     1328 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/fileset_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     1944 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/metalake_dto.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-17 08:55:50.899254 gravitino-0.5.0.dev21/gravitino/dto/requests/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev21/gravitino/dto/requests/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1632 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/requests/catalog_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     2659 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/requests/catalog_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1081 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/requests/catalog_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1506 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/requests/fileset_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     4267 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/requests/fileset_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      767 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/requests/fileset_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1096 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/requests/metalake_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     4146 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/requests/metalake_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1030 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/requests/metalake_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      935 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/requests/schema_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     2520 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/requests/schema_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1007 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/requests/schema_updates_request.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-17 08:55:50.900783 gravitino-0.5.0.dev21/gravitino/dto/responses/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev21/gravitino/dto/responses/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      684 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/responses/base_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      575 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/responses/catalog_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1077 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/responses/catalog_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      477 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/responses/drop_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      874 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/responses/entity_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1111 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/responses/fileset_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1163 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/responses/metalake_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1112 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/responses/metalake_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1079 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/responses/schema_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1397 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/dto/schema_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)      434 2024-05-14 03:08:07.000000 gravitino-0.5.0.dev21/gravitino/dto/version_dto.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-17 08:55:50.902110 gravitino-0.5.0.dev21/gravitino/exceptions/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev21/gravitino/exceptions/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      302 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev21/gravitino/exceptions/gravitino_runtime_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      363 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev21/gravitino/exceptions/illegal_name_identifier_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      352 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev21/gravitino/exceptions/illegal_namespace_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      289 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/exceptions/no_such_metalake_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      324 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/exceptions/not_found_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev21/gravitino/exceptions.py
+-rw-r--r--   0 xun        (501) staff       (20)     4404 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev21/gravitino/gravitino_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     9440 2024-05-14 03:08:07.000000 gravitino-0.5.0.dev21/gravitino/name_identifier.py
+-rw-r--r--   0 xun        (501) staff       (20)     7759 2024-05-14 03:08:07.000000 gravitino-0.5.0.dev21/gravitino/namespace.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-17 08:55:50.902518 gravitino-0.5.0.dev21/gravitino/rest/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-05-15 07:09:38.000000 gravitino-0.5.0.dev21/gravitino/rest/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1200 2024-05-13 10:34:46.000000 gravitino-0.5.0.dev21/gravitino/rest/rest_message.py
+-rw-r--r--   0 xun        (501) staff       (20)     2430 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev21/gravitino/service.py
+-rw-r--r--   0 xun        (501) staff       (20)      321 2024-05-14 03:08:07.000000 gravitino-0.5.0.dev21/gravitino/typing.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-17 08:55:50.903080 gravitino-0.5.0.dev21/gravitino/utils/
+-rw-r--r--   0 xun        (501) staff       (20)      175 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev21/gravitino/utils/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     2692 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev21/gravitino/utils/exceptions.py
+-rw-r--r--   0 xun        (501) staff       (20)     5529 2024-05-14 03:08:07.000000 gravitino-0.5.0.dev21/gravitino/utils/http_client.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-17 08:55:50.903691 gravitino-0.5.0.dev21/gravitino.egg-info/
+-rw-r--r--   0 xun        (501) staff       (20)     6355 2024-05-17 08:55:50.000000 gravitino-0.5.0.dev21/gravitino.egg-info/PKG-INFO
+-rw-r--r--   0 xun        (501) staff       (20)     2864 2024-05-17 08:55:50.000000 gravitino-0.5.0.dev21/gravitino.egg-info/SOURCES.txt
+-rw-r--r--   0 xun        (501) staff       (20)        1 2024-05-17 08:55:50.000000 gravitino-0.5.0.dev21/gravitino.egg-info/dependency_links.txt
+-rw-r--r--   0 xun        (501) staff       (20)       78 2024-05-17 08:55:50.000000 gravitino-0.5.0.dev21/gravitino.egg-info/requires.txt
+-rw-r--r--   0 xun        (501) staff       (20)       10 2024-05-17 08:55:50.000000 gravitino-0.5.0.dev21/gravitino.egg-info/top_level.txt
+-rw-r--r--   0 xun        (501) staff       (20)      146 2024-05-15 07:09:38.000000 gravitino-0.5.0.dev21/requirements-dev.txt
+-rw-r--r--   0 xun        (501) staff       (20)      176 2024-05-15 07:09:38.000000 gravitino-0.5.0.dev21/requirements.txt
+-rw-r--r--   0 xun        (501) staff       (20)       38 2024-05-17 08:55:50.904724 gravitino-0.5.0.dev21/setup.cfg
+-rw-r--r--   0 xun        (501) staff       (20)     1295 2024-05-17 08:55:27.000000 gravitino-0.5.0.dev21/setup.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-17 08:55:50.903381 gravitino-0.5.0.dev21/tests/
+-rw-r--r--   0 xun        (501) staff       (20)     2192 2024-05-15 07:09:38.000000 gravitino-0.5.0.dev21/tests/test_gravitino_client.py
```

### Comparing `gravitino-0.5.0.dev20/PKG-INFO` & `gravitino-0.5.0.dev21/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gravitino
-Version: 0.5.0.dev20
-Summary: Gravitino Python client
+Version: 0.5.0.dev21
+Summary: Python lib/client for Gravitino
 Home-page: https://github.com/datastrato/gravitino
 Author: datastrato
 Author-email: support@datastrato.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -55,17 +55,17 @@
 
 We offer a playground environment to help you quickly understand how to use Gravitino Python
 client to manage non-tabular data on HDFS via Fileset in Gravitino. You can refer to the
 document [How to use the playground#Launch AI components of playground](https://datastrato.ai/docs/latest/how-to-use-the-playground/#launch-ai-components-of-playground)
 to launch a Gravitino server, HDFS and Jupyter notebook environment in you local Docker environment.
 
 Waiting for the playground Docker environment to start, you can directly open
-`http://localhost:8888/lab/tree/gravitino-fileset-sample.ipynb` in the browser and run the example.
+`http://localhost:8888/lab/tree/gravitino-fileset-example.ipynb` in the browser and run the example.
 
-The [gravitino-fileset-example](https://github.com/datastrato/gravitino-playground/blob/main/init/jupyter/gravitino-fileset-sample.ipynb)
+The [gravitino-fileset-example](https://github.com/datastrato/gravitino-playground/blob/main/init/jupyter/gravitino-fileset-example.ipynb)
 contains the following code snippets:
 
 1. Install HDFS Python client.
 2. Create a HDFS client to connect HDFS and to do some test operations.
 3. Install Gravitino Python client.
 4. Initialize Gravitino admin client and create a Gravitino metalake.
 5. Initialize Gravitino client and list metalakes.
```

### Comparing `gravitino-0.5.0.dev20/README.md` & `gravitino-0.5.0.dev21/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
 We offer a playground environment to help you quickly understand how to use Gravitino Python
 client to manage non-tabular data on HDFS via Fileset in Gravitino. You can refer to the
 document [How to use the playground#Launch AI components of playground](https://datastrato.ai/docs/latest/how-to-use-the-playground/#launch-ai-components-of-playground)
 to launch a Gravitino server, HDFS and Jupyter notebook environment in you local Docker environment.
 
 Waiting for the playground Docker environment to start, you can directly open
-`http://localhost:8888/lab/tree/gravitino-fileset-sample.ipynb` in the browser and run the example.
+`http://localhost:8888/lab/tree/gravitino-fileset-example.ipynb` in the browser and run the example.
 
-The [gravitino-fileset-example](https://github.com/datastrato/gravitino-playground/blob/main/init/jupyter/gravitino-fileset-sample.ipynb)
+The [gravitino-fileset-example](https://github.com/datastrato/gravitino-playground/blob/main/init/jupyter/gravitino-fileset-example.ipynb)
 contains the following code snippets:
 
 1. Install HDFS Python client.
 2. Create a HDFS client to connect HDFS and to do some test operations.
 3. Install Gravitino Python client.
 4. Initialize Gravitino admin client and create a Gravitino metalake.
 5. Initialize Gravitino client and list metalakes.
```

### Comparing `gravitino-0.5.0.dev20/gravitino/__init__.py` & `gravitino-0.5.0.dev21/gravitino/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/api/audit.py` & `gravitino-0.5.0.dev21/gravitino/api/audit.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/api/catalog.py` & `gravitino-0.5.0.dev21/gravitino/api/catalog.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/api/catalog_change.py` & `gravitino-0.5.0.dev21/gravitino/api/catalog_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/api/fileset.py` & `gravitino-0.5.0.dev21/gravitino/api/fileset.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/api/fileset_change.py` & `gravitino-0.5.0.dev21/gravitino/api/fileset_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/api/metalake.py` & `gravitino-0.5.0.dev21/gravitino/api/metalake.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/api/metalake_change.py` & `gravitino-0.5.0.dev21/gravitino/api/metalake_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/api/schema.py` & `gravitino-0.5.0.dev21/gravitino/api/schema.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/api/schema_change.py` & `gravitino-0.5.0.dev21/gravitino/api/schema_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/api/supports_schemas.py` & `gravitino-0.5.0.dev21/gravitino/api/supports_schemas.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/catalog/base_schema_catalog.py` & `gravitino-0.5.0.dev21/gravitino/catalog/base_schema_catalog.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/catalog/fileset_catalog.py` & `gravitino-0.5.0.dev21/gravitino/catalog/fileset_catalog.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/client/gravitino_admin_client.py` & `gravitino-0.5.0.dev21/gravitino/client/gravitino_admin_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/client/gravitino_client.py` & `gravitino-0.5.0.dev21/gravitino/client/gravitino_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/client/gravitino_client_base.py` & `gravitino-0.5.0.dev21/gravitino/client/gravitino_client_base.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/client/gravitino_metalake.py` & `gravitino-0.5.0.dev21/gravitino/client/gravitino_metalake.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/audit_dto.py` & `gravitino-0.5.0.dev21/gravitino/dto/audit_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/catalog_dto.py` & `gravitino-0.5.0.dev21/gravitino/dto/catalog_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/dto_converters.py` & `gravitino-0.5.0.dev21/gravitino/dto/dto_converters.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/fileset_dto.py` & `gravitino-0.5.0.dev21/gravitino/dto/fileset_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/metalake_dto.py` & `gravitino-0.5.0.dev21/gravitino/dto/metalake_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/requests/catalog_create_request.py` & `gravitino-0.5.0.dev21/gravitino/dto/requests/catalog_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/requests/catalog_update_request.py` & `gravitino-0.5.0.dev21/gravitino/dto/requests/catalog_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/requests/catalog_updates_request.py` & `gravitino-0.5.0.dev21/gravitino/dto/requests/catalog_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/requests/fileset_create_request.py` & `gravitino-0.5.0.dev21/gravitino/dto/requests/fileset_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/requests/fileset_update_request.py` & `gravitino-0.5.0.dev21/gravitino/dto/requests/fileset_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/requests/fileset_updates_request.py` & `gravitino-0.5.0.dev21/gravitino/dto/requests/fileset_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/requests/metalake_create_request.py` & `gravitino-0.5.0.dev21/gravitino/dto/requests/metalake_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/requests/metalake_update_request.py` & `gravitino-0.5.0.dev21/gravitino/dto/requests/metalake_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/requests/metalake_updates_request.py` & `gravitino-0.5.0.dev21/gravitino/dto/requests/metalake_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/requests/schema_create_request.py` & `gravitino-0.5.0.dev21/gravitino/dto/requests/schema_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/requests/schema_update_request.py` & `gravitino-0.5.0.dev21/gravitino/dto/requests/schema_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/requests/schema_updates_request.py` & `gravitino-0.5.0.dev21/gravitino/dto/requests/schema_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/responses/base_response.py` & `gravitino-0.5.0.dev21/gravitino/dto/responses/base_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/responses/catalog_list_response.py` & `gravitino-0.5.0.dev21/gravitino/dto/responses/catalog_list_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/responses/catalog_response.py` & `gravitino-0.5.0.dev21/gravitino/dto/responses/catalog_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/responses/entity_list_response.py` & `gravitino-0.5.0.dev21/gravitino/dto/responses/entity_list_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/responses/fileset_response.py` & `gravitino-0.5.0.dev21/gravitino/dto/responses/fileset_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/responses/metalake_list_response.py` & `gravitino-0.5.0.dev21/gravitino/dto/responses/metalake_list_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/responses/metalake_response.py` & `gravitino-0.5.0.dev21/gravitino/dto/responses/metalake_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/responses/schema_response.py` & `gravitino-0.5.0.dev21/gravitino/dto/responses/schema_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/dto/schema_dto.py` & `gravitino-0.5.0.dev21/gravitino/dto/schema_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/gravitino_client.py` & `gravitino-0.5.0.dev21/gravitino/gravitino_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/name_identifier.py` & `gravitino-0.5.0.dev21/gravitino/name_identifier.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/namespace.py` & `gravitino-0.5.0.dev21/gravitino/namespace.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/rest/rest_message.py` & `gravitino-0.5.0.dev21/gravitino/rest/rest_message.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/service.py` & `gravitino-0.5.0.dev21/gravitino/service.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/utils/exceptions.py` & `gravitino-0.5.0.dev21/gravitino/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino/utils/http_client.py` & `gravitino-0.5.0.dev21/gravitino/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/gravitino.egg-info/PKG-INFO` & `gravitino-0.5.0.dev21/gravitino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gravitino
-Version: 0.5.0.dev20
-Summary: Gravitino Python client
+Version: 0.5.0.dev21
+Summary: Python lib/client for Gravitino
 Home-page: https://github.com/datastrato/gravitino
 Author: datastrato
 Author-email: support@datastrato.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -55,17 +55,17 @@
 
 We offer a playground environment to help you quickly understand how to use Gravitino Python
 client to manage non-tabular data on HDFS via Fileset in Gravitino. You can refer to the
 document [How to use the playground#Launch AI components of playground](https://datastrato.ai/docs/latest/how-to-use-the-playground/#launch-ai-components-of-playground)
 to launch a Gravitino server, HDFS and Jupyter notebook environment in you local Docker environment.
 
 Waiting for the playground Docker environment to start, you can directly open
-`http://localhost:8888/lab/tree/gravitino-fileset-sample.ipynb` in the browser and run the example.
+`http://localhost:8888/lab/tree/gravitino-fileset-example.ipynb` in the browser and run the example.
 
-The [gravitino-fileset-example](https://github.com/datastrato/gravitino-playground/blob/main/init/jupyter/gravitino-fileset-sample.ipynb)
+The [gravitino-fileset-example](https://github.com/datastrato/gravitino-playground/blob/main/init/jupyter/gravitino-fileset-example.ipynb)
 contains the following code snippets:
 
 1. Install HDFS Python client.
 2. Create a HDFS client to connect HDFS and to do some test operations.
 3. Install Gravitino Python client.
 4. Initialize Gravitino admin client and create a Gravitino metalake.
 5. Initialize Gravitino client and list metalakes.
```

### Comparing `gravitino-0.5.0.dev20/gravitino.egg-info/SOURCES.txt` & `gravitino-0.5.0.dev21/gravitino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev20/setup.py` & `gravitino-0.5.0.dev21/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     with open("README.md") as f:
         long_description = f.read()
 except FileNotFoundError:
     long_description = "Gravitino Python client"
 
 setup(
     name="gravitino",
-    description="Gravitino Python client",
-    version="0.5.0.dev20",
+    description="Python lib/client for Gravitino",
+    version="0.5.0.dev21",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/datastrato/gravitino",
     author="datastrato",
     author_email="support@datastrato.com",
     python_requires=">=3.8",
     packages=find_packages(exclude=["tests*"]),
```

### Comparing `gravitino-0.5.0.dev20/tests/test_gravitino_client.py` & `gravitino-0.5.0.dev21/tests/test_gravitino_client.py`

 * *Files identical despite different names*

