# Comparing `tmp/ckanext_files-0.2.6.tar.gz` & `tmp/ckanext_files-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext_files-0.2.6.tar", last modified: Wed Apr 24 11:53:12 2024, max compression
+gzip compressed data, was "ckanext_files-0.3.0.tar", last modified: Thu May 16 22:32:57 2024, max compression
```

## Comparing `ckanext_files-0.2.6.tar` & `ckanext_files-0.3.0.tar`

### file list

```diff
@@ -1,108 +1,125 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.384065 ckanext_files-0.2.6/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34517 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      211 2024-04-24 11:51:24.000000 ckanext_files-0.2.6/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15608 2024-04-24 11:53:12.384065 ckanext_files-0.2.6/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14070 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.357399 ckanext_files-0.2.6/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.360732 ckanext_files-0.2.6/ckanext/file_manager/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-02-04 13:46:59.000000 ckanext_files-0.2.6/ckanext/file_manager/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4162 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/file_manager/collection.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1423 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/file_manager/plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3519 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/file_manager/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.367399 ckanext_files-0.2.6/ckanext/files/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/ckanext/files/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.367399 ckanext_files-0.2.6/ckanext/files/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      187 2024-04-09 01:54:26.000000 ckanext_files-0.2.6/ckanext/files/assets/resource.config
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.367399 ckanext_files-0.2.6/ckanext/files/assets/scripts/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8237 2024-04-15 14:21:37.000000 ckanext_files-0.2.6/ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)    37143 2024-04-15 14:21:37.000000 ckanext_files-0.2.6/ckanext/files/assets/scripts/files--modules.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)      797 2024-04-15 14:21:37.000000 ckanext_files-0.2.6/ckanext/files/assets/scripts/files--shared-uploader.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)    44969 2024-04-15 14:21:37.000000 ckanext_files-0.2.6/ckanext/files/assets/scripts/files--shared.js
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.367399 ckanext_files-0.2.6/ckanext/files/assets/styles/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      197 2024-04-09 02:46:04.000000 ckanext_files-0.2.6/ckanext/files/assets/styles/files--style.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)      360 2024-04-09 01:54:34.000000 ckanext_files-0.2.6/ckanext/files/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14339 2024-04-15 14:22:47.000000 ckanext_files-0.2.6/ckanext/files/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      840 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/cli.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1355 2024-04-07 14:32:45.000000 ckanext_files-0.2.6/ckanext/files/command.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1245 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      373 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/config_declaration.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4998 2024-04-20 10:44:26.000000 ckanext_files-0.2.6/ckanext/files/exceptions.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1031 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      564 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.370732 ckanext_files-0.2.6/ckanext/files/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/ckanext/files/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9785 2024-04-22 16:49:03.000000 ckanext_files-0.2.6/ckanext/files/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3907 2024-04-07 14:32:45.000000 ckanext_files-0.2.6/ckanext/files/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2875 2024-04-07 16:20:32.000000 ckanext_files-0.2.6/ckanext/files/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1098 2024-04-15 14:22:08.000000 ckanext_files-0.2.6/ckanext/files/logic/validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.354066 ckanext_files-0.2.6/ckanext/files/migration/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.370732 ckanext_files-0.2.6/ckanext/files/migration/files/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1774 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/ckanext/files/migration/files/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/migration/files/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/ckanext/files/migration/files/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.374065 ckanext_files-0.2.6/ckanext/files/migration/files/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      595 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/migration/files/versions/2c5f1f90888c_add_file_last_access_field.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      921 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/migration/files/versions/2fbd30a1b364_create_owner_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      849 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/migration/files/versions/3c69eb68cecd_create_upload_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3061 2024-04-07 14:32:45.000000 ckanext_files-0.2.6/ckanext/files/migration/files/versions/5851e09b7ca3_remove_path_rename_kind_add_stats.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1019 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      484 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/migration/files/versions/76fdef67f479_add_access_column_to_owner_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      883 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.374065 ckanext_files-0.2.6/ckanext/files/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       77 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      211 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/model/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2472 2024-04-07 14:32:45.000000 ckanext_files-0.2.6/ckanext/files/model/file.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1547 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/model/owner.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4614 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.354066 ckanext_files-0.2.6/ckanext/files/public/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.354066 ckanext_files-0.2.6/ckanext/files/public/ckanext-files/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.374065 ckanext_files-0.2.6/ckanext/files/public/ckanext-files/scripts/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      797 2024-04-15 14:21:37.000000 ckanext_files-0.2.6/ckanext/files/public/ckanext-files/scripts/files--shared-uploader.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)      363 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/shared.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.377399 ckanext_files-0.2.6/ckanext/files/storage/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      312 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/storage/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7410 2024-04-09 11:03:43.000000 ckanext_files-0.2.6/ckanext/files/storage/fs.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11028 2024-04-20 10:44:26.000000 ckanext_files-0.2.6/ckanext/files/storage/google_cloud.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4719 2024-04-15 14:21:38.000000 ckanext_files-0.2.6/ckanext/files/storage/redis.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.377399 ckanext_files-0.2.6/ckanext/files/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.357399 ckanext_files-0.2.6/ckanext/files/templates/files/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.377399 ckanext_files-0.2.6/ckanext/files/templates/files/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       59 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/templates/files/snippets/_asset.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)       29 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/templates/files/snippets/_resource.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5167 2024-04-09 03:20:53.000000 ckanext_files-0.2.6/ckanext/files/templates/files/snippets/file_table.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2451 2024-04-09 05:48:11.000000 ckanext_files-0.2.6/ckanext/files/templates/files/snippets/uploader_v1.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.377399 ckanext_files-0.2.6/ckanext/files/templates/files/user/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      550 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/templates/files/user/delete.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      847 2024-04-22 16:49:06.000000 ckanext_files-0.2.6/ckanext/files/templates/files/user/index.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      274 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/templates/page.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.380732 ckanext_files-0.2.6/ckanext/files/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/ckanext/files/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3442 2024-04-07 16:20:32.000000 ckanext_files-0.2.6/ckanext/files/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.380732 ckanext_files-0.2.6/ckanext/files/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/ckanext/files/tests/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1506 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/tests/logic/test_action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1725 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/tests/logic/test_validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.380732 ckanext_files-0.2.6/ckanext/files/tests/storage/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/tests/storage/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7502 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/tests/storage/test_fs.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10311 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/tests/storage/test_google_cloud.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3814 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/tests/storage/test_redis.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11805 2024-04-09 11:08:13.000000 ckanext_files-0.2.6/ckanext/files/tests/test_base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3061 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/tests/test_config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6777 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/tests/test_utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1128 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/types.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5490 2024-04-15 14:21:38.000000 ckanext_files-0.2.6/ckanext/files/utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4522 2024-04-20 10:44:26.000000 ckanext_files-0.2.6/ckanext/files/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.384065 ckanext_files-0.2.6/ckanext_files.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15608 2024-04-24 11:53:11.000000 ckanext_files-0.2.6/ckanext_files.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3151 2024-04-24 11:53:12.000000 ckanext_files-0.2.6/ckanext_files.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-24 11:53:11.000000 ckanext_files-0.2.6/ckanext_files.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      241 2024-04-24 11:53:11.000000 ckanext_files-0.2.6/ckanext_files.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-24 11:53:11.000000 ckanext_files-0.2.6/ckanext_files.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      359 2024-04-24 11:53:11.000000 ckanext_files-0.2.6/ckanext_files.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-24 11:53:11.000000 ckanext_files-0.2.6/ckanext_files.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4286 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2000 2024-04-24 11:53:12.387399 ckanext_files-0.2.6/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      262 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.529283 ckanext_files-0.3.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34517 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      309 2024-04-24 12:11:35.000000 ckanext_files-0.3.0/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15637 2024-05-16 22:32:57.529283 ckanext_files-0.3.0/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14099 2024-05-07 23:58:43.000000 ckanext_files-0.3.0/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.499282 ckanext_files-0.3.0/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2024-01-28 01:59:52.000000 ckanext_files-0.3.0/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.499282 ckanext_files-0.3.0/ckanext/file_manager/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-02-04 13:46:59.000000 ckanext_files-0.3.0/ckanext/file_manager/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.499282 ckanext_files-0.3.0/ckanext/file_manager/assets/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.502616 ckanext_files-0.3.0/ckanext/file_manager/assets/js/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1226 2024-02-04 13:46:59.000000 ckanext_files-0.3.0/ckanext/file_manager/assets/js/fm-htmx.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      182 2024-02-04 13:46:59.000000 ckanext_files-0.3.0/ckanext/file_manager/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4162 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/file_manager/collection.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1423 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/file_manager/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.495949 ckanext_files-0.3.0/ckanext/file_manager/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.502616 ckanext_files-0.3.0/ckanext/file_manager/templates/file_manager/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1253 2024-02-04 13:46:59.000000 ckanext_files-0.3.0/ckanext/file_manager/templates/file_manager/list.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1047 2024-02-04 13:46:59.000000 ckanext_files-0.3.0/ckanext/file_manager/templates/file_manager/record.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1082 2024-02-04 13:46:59.000000 ckanext_files-0.3.0/ckanext/file_manager/templates/file_manager/upload_file_modal.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      180 2024-02-04 13:46:59.000000 ckanext_files-0.3.0/ckanext/file_manager/templates/file_manager/upload_file_modal_form.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3519 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/file_manager/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.509282 ckanext_files-0.3.0/ckanext/files/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.3.0/ckanext/files/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.509282 ckanext_files-0.3.0/ckanext/files/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      187 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/assets/resource.config
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.509282 ckanext_files-0.3.0/ckanext/files/assets/scripts/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8236 2024-05-16 22:32:34.000000 ckanext_files-0.3.0/ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    38532 2024-05-16 22:32:34.000000 ckanext_files-0.3.0/ckanext/files/assets/scripts/files--modules.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      796 2024-05-16 22:32:34.000000 ckanext_files-0.3.0/ckanext/files/assets/scripts/files--shared-uploader.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    46195 2024-05-16 22:32:34.000000 ckanext_files-0.3.0/ckanext/files/assets/scripts/files--shared.js
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.509282 ckanext_files-0.3.0/ckanext/files/assets/styles/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      197 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/assets/styles/files--style.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      360 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15234 2024-05-08 00:07:06.000000 ckanext_files-0.3.0/ckanext/files/base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2913 2024-05-08 00:07:49.000000 ckanext_files-0.3.0/ckanext/files/cli.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1355 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/command.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1244 2024-05-10 01:11:43.000000 ckanext_files-0.3.0/ckanext/files/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      373 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/config_declaration.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4993 2024-05-08 00:09:47.000000 ckanext_files-0.3.0/ckanext/files/exceptions.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1031 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      564 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/interfaces.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.509282 ckanext_files-0.3.0/ckanext/files/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.3.0/ckanext/files/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10027 2024-05-16 22:04:35.000000 ckanext_files-0.3.0/ckanext/files/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3951 2024-05-07 23:59:35.000000 ckanext_files-0.3.0/ckanext/files/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2875 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/logic/schema.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1098 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/logic/validators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.495949 ckanext_files-0.3.0/ckanext/files/migration/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.512616 ckanext_files-0.3.0/ckanext/files/migration/files/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1774 2024-01-28 01:59:52.000000 ckanext_files-0.3.0/ckanext/files/migration/files/alembic.ini
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/migration/files/env.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2024-01-28 01:59:52.000000 ckanext_files-0.3.0/ckanext/files/migration/files/script.py.mako
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.512616 ckanext_files-0.3.0/ckanext/files/migration/files/versions/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      595 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/migration/files/versions/2c5f1f90888c_add_file_last_access_field.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      921 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/migration/files/versions/2fbd30a1b364_create_owner_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      849 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/migration/files/versions/3c69eb68cecd_create_upload_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3061 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/migration/files/versions/5851e09b7ca3_remove_path_rename_kind_add_stats.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1019 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      484 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/migration/files/versions/76fdef67f479_add_access_column_to_owner_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      883 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.515949 ckanext_files-0.3.0/ckanext/files/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       77 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      211 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/model/base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2904 2024-05-08 00:07:07.000000 ckanext_files-0.3.0/ckanext/files/model/file.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1547 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/model/owner.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4614 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.495949 ckanext_files-0.3.0/ckanext/files/public/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.495949 ckanext_files-0.3.0/ckanext/files/public/ckanext-files/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.515949 ckanext_files-0.3.0/ckanext/files/public/ckanext-files/scripts/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      796 2024-05-16 22:32:34.000000 ckanext_files-0.3.0/ckanext/files/public/ckanext-files/scripts/files--shared-uploader.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      363 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/shared.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.515949 ckanext_files-0.3.0/ckanext/files/storage/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      312 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/storage/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8199 2024-05-09 17:00:53.000000 ckanext_files-0.3.0/ckanext/files/storage/fs.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11198 2024-05-08 00:09:57.000000 ckanext_files-0.3.0/ckanext/files/storage/google_cloud.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4719 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/storage/redis.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.515949 ckanext_files-0.3.0/ckanext/files/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.495949 ckanext_files-0.3.0/ckanext/files/templates/files/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.515949 ckanext_files-0.3.0/ckanext/files/templates/files/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       59 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/templates/files/snippets/_asset.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       29 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/templates/files/snippets/_resource.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5166 2024-05-07 23:37:22.000000 ckanext_files-0.3.0/ckanext/files/templates/files/snippets/file_table.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2451 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/templates/files/snippets/uploader_v1.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.515949 ckanext_files-0.3.0/ckanext/files/templates/files/user/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      550 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/templates/files/user/delete.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      847 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/templates/files/user/index.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      274 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/templates/page.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.519283 ckanext_files-0.3.0/ckanext/files/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.3.0/ckanext/files/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3443 2024-05-09 17:43:24.000000 ckanext_files-0.3.0/ckanext/files/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.522616 ckanext_files-0.3.0/ckanext/files/tests/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.3.0/ckanext/files/tests/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1506 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/tests/logic/test_action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1725 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/tests/logic/test_validators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.525950 ckanext_files-0.3.0/ckanext/files/tests/storage/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/tests/storage/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7502 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/tests/storage/test_fs.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10311 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/tests/storage/test_google_cloud.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3814 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/tests/storage/test_redis.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11805 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/tests/test_base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3061 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/tests/test_config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6777 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/ckanext/files/tests/test_utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1438 2024-05-08 00:07:06.000000 ckanext_files-0.3.0/ckanext/files/types.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5805 2024-05-10 01:38:52.000000 ckanext_files-0.3.0/ckanext/files/utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4485 2024-05-08 00:07:07.000000 ckanext_files-0.3.0/ckanext/files/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.525950 ckanext_files-0.3.0/ckanext/files_uploader/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-05-07 20:36:18.000000 ckanext_files-0.3.0/ckanext/files_uploader/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6115 2024-05-16 11:37:56.000000 ckanext_files-0.3.0/ckanext/files_uploader/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.525950 ckanext_files-0.3.0/ckanext/files_uploader/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-05-09 17:42:54.000000 ckanext_files-0.3.0/ckanext/files_uploader/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:37:23.000000 ckanext_files-0.3.0/ckanext/files_uploader/tests/conftest.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3636 2024-05-16 11:37:27.000000 ckanext_files-0.3.0/ckanext/files_uploader/tests/test_plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 22:32:57.525950 ckanext_files-0.3.0/ckanext_files.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15637 2024-05-16 22:32:57.000000 ckanext_files-0.3.0/ckanext_files.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3678 2024-05-16 22:32:57.000000 ckanext_files-0.3.0/ckanext_files.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-05-16 22:32:57.000000 ckanext_files-0.3.0/ckanext_files.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      308 2024-05-16 22:32:57.000000 ckanext_files-0.3.0/ckanext_files.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-05-16 22:32:57.000000 ckanext_files-0.3.0/ckanext_files.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      359 2024-05-16 22:32:57.000000 ckanext_files-0.3.0/ckanext_files.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-05-16 22:32:57.000000 ckanext_files-0.3.0/ckanext_files.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4286 2024-04-24 12:10:46.000000 ckanext_files-0.3.0/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.3.0/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2068 2024-05-16 22:32:57.529283 ckanext_files-0.3.0/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      262 2024-01-28 01:59:52.000000 ckanext_files-0.3.0/setup.py
```

### Comparing `ckanext_files-0.2.6/LICENSE` & `ckanext_files-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/PKG-INFO` & `ckanext_files-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-files
-Version: 0.2.6
+Version: 0.3.0
 Home-page: https://github.com/DataShades/ckanext-files
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -53,15 +53,16 @@
 | 2.10         | yes         |
 | master       | yes         |
 
 CKAN v2.8 and v2.9 are supported by ckanext-files v0.2. Starting from v1.0 this
 extension switches to CKAN support policy of two latest CKAN releases. I.e,
 ckanext-files v1.0 supports only CKAN v2.10 and v2.11.
 
-v0.2 will not receive any new features, only bug-fixes.
+v0.* will not receive any new major features, only bug-fixes and small
+improvements.
 
 It's recommended to install the extension via pip, so you probably have all the
 requirements pinned already. If you are using GitHub version of this extension,
 stick to the vX.Y.Z tags to avoid breaking changes. Check the changelog before
 upgrading the extension.
 
 ## Installation
```

### Comparing `ckanext_files-0.2.6/README.md` & `ckanext_files-0.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 | 2.10         | yes         |
 | master       | yes         |
 
 CKAN v2.8 and v2.9 are supported by ckanext-files v0.2. Starting from v1.0 this
 extension switches to CKAN support policy of two latest CKAN releases. I.e,
 ckanext-files v1.0 supports only CKAN v2.10 and v2.11.
 
-v0.2 will not receive any new features, only bug-fixes.
+v0.* will not receive any new major features, only bug-fixes and small
+improvements.
 
 It's recommended to install the extension via pip, so you probably have all the
 requirements pinned already. If you are using GitHub version of this extension,
 stick to the vX.Y.Z tags to avoid breaking changes. Check the changelog before
 upgrading the extension.
 
 ## Installation
```

### Comparing `ckanext_files-0.2.6/ckanext/file_manager/collection.py` & `ckanext_files-0.3.0/ckanext/file_manager/collection.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/file_manager/plugin.py` & `ckanext_files-0.3.0/ckanext/file_manager/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/file_manager/views.py` & `ckanext_files-0.3.0/ckanext/file_manager/views.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js` & `ckanext_files-0.3.0/ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text, with very long lines (5858)*

 * *Files 0% similar despite different names*

```diff
@@ -508,8 +508,8 @@
 00001fb0: 4b54 7463 6269 4167 4943 4167 4943 4167  KTtcbiAgICAgICAg
 00001fc0: 4943 4167 4943 4167 6653 7863 6269 4167  ICAgICAgfSxcbiAg
 00001fd0: 4943 4167 4943 4167 4943 4167 4943 6b37  ICAgICAgICAgICk7
 00001fe0: 5847 3467 4943 4167 4943 4167 4943 4167  XG4gICAgICAgICAg
 00001ff0: 6653 6b37 5847 3467 4943 4167 4943 4167  fSk7XG4gICAgICAg
 00002000: 4948 3163 6269 4167 4943 4167 4948 3163  IH1cbiAgICAgIH1c
 00002010: 6269 4167 4943 4239 5847 3467 4948 3163  biAgICB9XG4gIH1c
-00002020: 626e 3163 6269 4a64 6651 3d3d 0a         bn1cbiJdfQ==.
+00002020: 626e 3163 6269 4a64 6651 3d3d            bn1cbiJdfQ==
```

### Comparing `ckanext_files-0.2.6/ckanext/files/assets/scripts/files--modules.js` & `ckanext_files-0.3.0/ckanext/files/assets/scripts/files--modules.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -91,18 +91,20 @@
         _onChange(event) {
             const file = event.target.files?.[0];
             if (!file) {
                 return;
             }
             if (this.options.name && file.name !== this.options.name) {
                 this.sandbox.notify("Name mismatch.", `Expected name: ${this.options.name}`);
+                this.sandbox.notify.el[0].scrollIntoView();
                 return;
             }
             if (this.options.size && file.size !== this.options.size) {
                 this.sandbox.notify("Size mismatch.", `Expected size: ${this.options.size.toLocaleString()} bytes`);
+                this.sandbox.notify.el[0].scrollIntoView();
                 return;
             }
             this.sandbox.publish(ckan.CKANEXT_FILES.topics.restoreFileInQueue, file, {
                 id: this.options.id,
                 uploaded: this.options.uploaded,
                 immediate: this.options.immediate,
             });
@@ -161,31 +163,35 @@
             info.uploader.addEventListener("commit", (event) => (info.id = event.detail.id));
             info.uploader.addEventListener("fail", ({
                 detail: {
                     reasons,
                     file
                 },
             }) => {
+                console.log(info.uploader, 1);
                 this.sandbox.notify(file.name, Object.entries(reasons)
                     .filter(([k, v]) => k[0] !== "_")
                     .map(([k, v]) => Array.isArray(v) ? v.join("; ") : v)
                     .join("; "));
+                this.sandbox.notify.el[0].scrollIntoView();
                 this.toggleAnimation(widget, false);
                 widget
                     .find("[data-upload-progress]")
                     .removeClass("bg-primary bg-secondary")
                     .addClass("bg-danger progress-bar-danger");
             });
             info.uploader.addEventListener("error", ({
                 detail: {
                     message,
                     file
                 },
             }) => {
+                console.log(info.uploader, 2);
                 this.sandbox.notify(file.name, message);
+                this.sandbox.notify.el[0].scrollIntoView();
                 this.toggleAnimation(widget, false);
                 widget
                     .find("[data-upload-progress]")
                     .removeClass("bg-primary bg-secondary")
                     .addClass("bg-danger progress-bar-danger");
             });
             info.uploader.addEventListener("progress", ({
@@ -257,8 +263,8 @@
                 .removeClass("bg-primary")
                 .addClass("bg-secondary");
             info.uploader.pause(info.file);
             this.toggleAnimation(widget, false);
         },
     };
 });
-//# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiZmlsZXMtLW1vZHVsZXMuanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi90cy9maWxlcy0tbW9kdWxlcy50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiQUFBQTs7OztHQUlHO0FBQ0gsSUFBSSxDQUFDLE1BQU0sQ0FBQyxrQkFBa0IsRUFBRSxVQUFVLENBQUM7SUFDdkMsT0FBTztRQUNILE9BQU8sRUFBRTtZQUNMLFNBQVMsRUFBRSxLQUFLO1NBQ25CO1FBQ0QsVUFBVTtZQUNOLE1BQU0sU0FBUyxHQUFHLElBQUksQ0FBQyxDQUFDLENBQUMsd0JBQXdCLENBQUMsQ0FBQztZQUNuRCxTQUFTLENBQUMsRUFBRSxDQUFDLE1BQU0sRUFBRSxDQUFDLEtBQVksRUFBRSxFQUFFLENBQUMsS0FBSyxDQUFDLGNBQWMsRUFBRSxDQUFDLENBQUM7WUFDL0QsU0FBUyxDQUFDLEVBQUUsQ0FBQyxRQUFRLEVBQUUsQ0FBQyxLQUFZLEVBQUUsRUFBRSxDQUNwQyxJQUFJLENBQUMsSUFBSSxDQUFDLEdBQUksS0FBSyxDQUFDLE1BQTJCLENBQUMsS0FBTSxDQUFDLENBQzFELENBQUM7UUFDTixDQUFDO1FBRUQsSUFBSSxDQUFDLEdBQUcsS0FBYTtZQUNqQixLQUFLLENBQUMsT0FBTyxDQUFDLENBQUMsSUFBSSxFQUFFLEVBQUUsQ0FDbkIsSUFBSSxDQUFDLE9BQU8sQ0FBQyxPQUFPLENBQ2hCLElBQUksQ0FBQyxhQUFhLENBQUMsTUFBTSxDQUFDLGNBQWMsRUFDeEMsSUFBSSxFQUNKLEVBQUUsU0FBUyxFQUFFLElBQUksQ0FBQyxPQUFPLENBQUMsU0FBUyxFQUFFLENBQ3hDLENBQ0osQ0FBQztRQUNOLENBQUM7S0FDSixDQUFDO0FBQ04sQ0FBQyxDQUFDLENBQUM7QUFFSDs7O0dBR0c7QUFDSCxJQUFJLENBQUMsTUFBTSxDQUFDLGlCQUFpQixFQUFFLFVBQVUsQ0FBQztJQUN0QyxPQUFPO1FBQ0gsT0FBTyxFQUFFO1lBQ0wsU0FBUyxFQUFFLEtBQUs7U0FDbkI7UUFF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Q3hDLENBQUM7S0FDSixDQUFDO0FBQ04sQ0FBQyxDQUFDLENBQUMiLCJzb3VyY2VzQ29udGVudCI6WyIvKipcbiAqIEFkZCBzZWxlY3RlZCBmaWxlIHRvIHVwbG9hZCBxdWV1ZSB3aGVuZXZlciBgW2RhdGEtcXVldWUtc2NoZWR1bGVyXWBcbiAqIGRpc3BhdGNoZXMgYGNoYW5nZWAgZXZlbnQuXG4gKlxuICovXG5ja2FuLm1vZHVsZShcImZpbGVzLS1zY2hlZHVsZXJcIiwgZnVuY3Rpb24gKCQpIHtcbiAgICByZXR1cm4ge1xuICAgICAgICBvcHRpb25zOiB7XG4gICAgICAgICAgICBpbW1lZGlhdGU6IGZhbHNlLFxuICAgICAgICB9LFxuICAgICAgICBpbml0aWFsaXplKCkge1xuICAgICAgICAgICAgY29uc3Qgc2NoZWR1bGVyID0gdGhpcy4kKFwiW2RhdGEtcXVldWUtc2NoZWR1bGVyXVwiKTtcbiAgICAgICAgICAgIHNjaGVkdWxlci5vbihcImRyb3BcIiwgKGV2ZW50OiBFdmVudCkgPT4gZXZlbnQucHJldmVudERlZmF1bHQoKSk7XG4gICAgICAgICAgICBzY2hlZHVsZXIub24oXCJjaGFuZ2VcIiwgKGV2ZW50OiBFdmVudCkgPT5cbiAgICAgICAgICAgICAgICB0aGlzLnB1c2goLi4uKGV2ZW50LnRhcmdldCBhcyBIVE1MSW5wdXRFbGVtZW50KS5maWxlcyEpLFxuICAgICAgICAgICAgKTtcbiAgICAgICAgfSxcblxuICAgICAgICBwdXNoKC4uLmZpbGVzOiBGaWxlW10pIHtcbiAgICAgICAgICAgIGZpbGVzLmZvckVhY2goKGZpbGUpID0+XG4gICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94LnB1Ymxpc2goXG4gICAgICAgICAgICAgICAgICAgIGNrYW4uQ0tBTkVYVF9GSUxFUy50b3BpY3MuYWRkRmlsZVRvUXVldWUsXG4gICAgICAgICAgICAgICAgICAgIGZpbGUsXG4gICAgICAgICAgICAgICAgICAgIHsgaW1tZWRpYXRlOiB0aGlzLm9wdGlvbnMuaW1tZWRpYXRlIH0sXG4gICAgICAgICAgICAgICAgKSxcbiAgICAgICAgICAgICk7XG4gICAgICAgIH0sXG4gICAgfTtcbn0pO1xuXG4vKipcbiAqIEFkZCBmaWxlL2RpcmVjdG9yaWVzIHRvIHVwbG9hZCBxdWV1ZSB2aWEgZHJhZyduJ2Ryb3AuXG4gKlxuICovXG5ja2FuLm1vZHVsZShcImZpbGVzLS1kcm9wem9uZVwiLCBmdW5jdGlvbiAoJCkge1xuICAgIHJldHVybiB7XG4gICAgICAgIG9wdGlvbnM6IHtcbiAgICAgICAgICAgIGltbWVkaWF0ZTogZmFsc2UsXG4gICAgICAgIH0sXG5cbiAgICAgICAgaW5pdGlhbGl6ZSgpIHtcbiAgICAgICAgICAgICQucHJveHlBbGwodGhpcywgL19vbi8pO1xuICAgICAgICAgICAgY29uc3QgZWxlbWVudCA9IHRoaXMuZWxbMF07XG5cbiAgICAgICAgICAgIGVsZW1lbnQuYWRkRXZlbnRMaXN0ZW5lcihcImRyYWdvdmVyXCIsIHRoaXMuX29uRHJhZ092ZXIpO1xuICAgICAgICAgICAgZWxlbWVudC5hZGRFdmVudExpc3RlbmVyKFwiZHJhZ2VudGVyXCIsIHRoaXMuX29uRHJhZ0VudGVyKTtcbiAgICAgICAgICAgIGVsZW1lbnQuYWRkRXZlbnRMaXN0ZW5lcihcImRyYWdsZWF2ZVwiLCB0aGlzLl9vbkRyYWdMZWF2ZSk7XG4gICAgICAgICAgICBlbGVtZW50LmFkZEV2ZW50TGlzdGVuZXIoXCJkcm9wXCIsIHRoaXMuX29uRHJvcCk7XG4gICAgICAgIH0sXG5cbiAgICAgICAgX29uRHJhZ092ZXIoZXZlbnQ6IERyYWdFdmVudCkge1xuICAgICAgICAgICAgZXZlbnQucHJldmVudERlZmF1bHQoKTtcbiAgICAgICAgfSxcbiAgICAgICAgX29uRHJhZ0VudGVyKGV2ZW50OiBEcmFnRXZlbnQpIHt9LFxuICAgICAgICBfb25EcmFnTGVhdmUoZXZlbnQ6IERyYWdFdmVudCkge30sXG5cbiAgICAgICAgX29uRHJvcChldmVudDogRHJhZ0V2ZW50KSB7XG4gICAgICAgICAgICBldmVudC5wcmV2ZW50RGVmYXVsdCgpO1xuICAgICAgICAgICAgaWYgKCFldmVudC5kYXRhVHJhbnNmZXIpIHtcbiAgICAgICAgICAgICAgICByZXR1cm47XG4gICAgICAgICAgICB9XG5cbiAgICAgICAgICAgIGZvciAobGV0IGVudHJ5IG9mIGV2ZW50LmRhdGFUcmFuc2Zlci5pdGVtcykge1xuICAgICAgICAgICAgICAgIHRoaXMuc2NhbkVudHJ5KGVudHJ5LndlYmtpdEdldEFzRW50cnkoKSwgKGZpbGU6IEZpbGUpID0+XG4gICAgICAgICAgICAgICAgICAgIHRoaXMucHVzaChmaWxlKSxcbiAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgfVxuICAgICAgICB9LFxuXG4gICAgICAgIHNjYW5FbnRyeShcbiAgICAgICAgICAgIGVudHJ5OiBGaWxlU3lzdGVtRmlsZUVudHJ5IHwgRmlsZVN5c3RlbURpcmVjdG9yeUVudHJ5LFxuICAgICAgICAgICAgY2I6IChmaWxlOiBGaWxlKSA9PiB2b2lkLFxuICAgICAgICApIHtcbiAgICAgICAgICAgIGlmIChlbnRyeS5pc0ZpbGUpIHtcbiAgICAgICAgICAgICAgICAoZW50cnkgYXMgRmlsZVN5c3RlbUZpbGVFbnRyeSkuZmlsZShjYik7XG4gICAgICAgICAgICB9IGVsc2Uge1xuICAgICAgICAgICAgICAgIChlbnRyeSBhcyBGaWxlU3lzdGVtRGlyZWN0b3J5RW50cnkpXG4gICAgICAgICAgICAgICAgICAgIC5jcmVhdGVSZWFkZXIoKVxuICAgICAgICAgICAgICAgICAgICAucmVhZEVudHJpZXMoKGVudHJpZXMpID0+XG4gICAgICAgICAgICAgICAgICAgICAgICBlbnRyaWVzLmZvckVhY2goKGUpID0+IHRoaXMuc2NhbkVudHJ5KGUsIGNiKSksXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICB9XG4gICAgICAgIH0sXG5cbiAgICAgICAgcHVzaChmaWxlOiBGaWxlKSB7XG4gICAgICAgICAgICB0aGlzLnNhbmRib3gucHVibGlzaChcbiAgICAgICAgICAgICAgICBja2FuLkNLQU5FWFRfRklMRVMudG9waWNzLmFkZEZpbGVUb1F1ZXVlLFxuICAgICAgICAgICAgICAgIGZpbGUsXG4gICAgICAgICAgICAgICAgeyBpbW1lZGlhdGU6IHRoaXMub3B0aW9ucy5pbW1lZGlhdGUgfSxcbiAgICAgICAgICAgICk7XG4gICAgICAgIH0sXG4gICAgfTtcbn0pO1xuXG4vKipcbiAqIEFkZCB0byBxdWV1ZSBhIGZpbGUsIHRoYXQgaGFzIGFzc29jaWF0ZWQgaW5jb21wbGV0ZSB1cGxvYWQuXG4gKlxuICogU3VwcG9ydHMgYSBudW1iZXIgb2YgcHJvcGVydGllcyB0byB2ZXJpZnkgdGhhdCB0aGUgbmV3IGZpbGUgbWF0Y2hlc1xuICogcHJldmlvdXNseSB1cGxvYWRlZCBmaWxlLlxuICpcbiAqXG4gKi9cbmNrYW4ubW9kdWxlKFwiZmlsZXMtLXJlc3RvcmVyXCIsIGZ1bmN0aW9uICgkKSB7XG4gICAgcmV0dXJuIHtcbiAgICAgICAgb3B0aW9uczoge1xuICAgICAgICAgICAgbmFtZTogXCJcIixcbiAgICAgICAgICAgIHNpemU6IDAsXG4gICAgICAgICAgICB1cGxvYWRlZDogMCxcbiAgICAgICAgICAgIGlkOiBcIlwiLFxuICAgICAgICAgICAgaW1tZWRpYXRlOiBmYWxzZSxcbiAgICAgICAgfSxcblxuICAgICAgICBpbml0aWFsaXplKCkge1xuICAgICAgICAgICAgJC5wcm94eUFsbCh0aGlzLCAvX29uLyk7XG4gICAgICAgICAgICB0aGlzLmVsLm9uKFwiY2hhbmdlXCIsIHRoaXMuX29uQ2hhbmdlKTtcbiAgICAgICAgfSxcblxuICAgICAgICBfb25DaGFuZ2UoZXZlbnQ6IEV2ZW50KSB7XG4gICAgICAgICAgICBjb25zdCBmaWxlID0gKGV2ZW50LnRhcmdldCBhcyBIVE1MSW5wdXRFbGVtZW50KS5maWxlcz8uWzBdO1xuXG4gICAgICAgICAgICBpZiAoIWZpbGUpIHtcbiAgICAgICAgICAgICAgICByZXR1cm47XG4gICAgICAgICAgICB9XG5cbiAgICAgICAgICAgIGlmICh0aGlzLm9wdGlvbnMubmFtZSAmJiBmaWxlLm5hbWUgIT09IHRoaXMub3B0aW9ucy5uYW1lKSB7XG4gICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94Lm5vdGlmeShcbiAgICAgICAgICAgICAgICAgICAgXCJOYW1lIG1pc21hdGNoLlwiLFxuICAgICAgICAgICAgICAgICAgICBgRXhwZWN0ZWQgbmFtZTogJHt0aGlzLm9wdGlvbnMubmFtZX1gLFxuICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgcmV0dXJuO1xuICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICBpZiAodGhpcy5vcHRpb25zLnNpemUgJiYgZmlsZS5zaXplICE9PSB0aGlzLm9wdGlvbnMuc2l6ZSkge1xuICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5ub3RpZnkoXG4gICAgICAgICAgICAgICAgICAgIFwiU2l6ZSBtaXNtYXRjaC5cIixcbiAgICAgICAgICAgICAgICAgICAgYEV4cGVjdGVkIHNpemU6ICR7dGhpcy5vcHRpb25zLnNpemUudG9Mb2NhbGVTdHJpbmcoKX0gYnl0ZXNgLFxuICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgcmV0dXJuO1xuICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICB0aGlzLnNhbmRib3gucHVibGlzaChcbiAgICAgICAgICAgICAgICBja2FuLkNLQU5FWFRfRklMRVMudG9waWNzLnJlc3RvcmVGaWxlSW5RdWV1ZSxcbiAgICAgICAgICAgICAgICBmaWxlLFxuICAgICAgICAgICAgICAgIHtcbiAgICAgICAgICAgICAgICAgICAgaWQ6IHRoaXMub3B0aW9ucy5pZCxcbiAgICAgICAgICAgICAgICAgICAgdXBsb2FkZWQ6IHRoaXMub3B0aW9ucy51cGxvYWRlZCxcbiAgICAgICAgICAgICAgICAgICAgaW1tZWRpYXRlOiB0aGlzLm9wdGlvbnMuaW1tZWRpYXRlLFxuICAgICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICApO1xuICAgICAgICB9LFxuICAgIH07XG59KTtcblxuY2thbi5tb2R1bGUoXCJmaWxlcy0tc2hhcmVkLXF1ZXVlXCIsIGZ1bmN0aW9uICgkKSB7XG4gICAgcmV0dXJuIHtcbiAgICAgICAgaW5pdGlhbGl6ZSgpIHtcbiAgICAgICAgICAgICQucHJveHlBbGwodGhpcywgL19vbi8pO1xuXG4gICAgICAgICAgICB0aGlzLndvcmtlciA9IG5ldyBTaGFyZWRXb3JrZXIoXG4gICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94LnVybChcbiAgICAgICAgICAgICAgICAgICAgXCJja2FuZXh0LWZpbGVzL3NjcmlwdHMvZmlsZXMtLXNoYXJlZC11cGxvYWRlci5qc1wiLFxuICAgICAgICAgICAgICAgICksXG4gICAgICAgICAgICApO1xuXG4gICAgICAgICAgICB0aGlzLndvcmtlci5wb3J0Lm9ubWVzc2FnZSA9IGNvbnNvbGUuZGVidWc7XG4gICAgICAgIH0sXG4gICAgfTtcbn0pO1xuXG5ja2FuLm1vZHVsZShcImZpbGVzLS1xdWV1ZVwiLCBmdW5jdGlvbiAoJCkge1xuICAgIHJldHVybiB7XG4gICAgICAgIG9wdGlvbnM6IHtcbiAgICAgICAgICAgIHN0b3JhZ2U6IFwiZGVmYXVsdFwiLFxuICAgICAgICAgICAgdXBsb2FkZXI6IFwiU3RhbmRhcmRcIixcbiAgICAgICAgfSxcblxuICAgICAgICBpbml0aWFsaXplKCkge1xuICAgICAgICAgICAgJC5wcm94eUFsbCh0aGlzLCAvX29uLyk7XG4gICAgICAgICAgICBja2FuLnB1YnN1Yi5zdWJzY3JpYmUoXG4gICAgICAgICAgICAgICAgY2thbi5DS0FORVhUX0ZJTEVTLnRvcGljcy5hZGRGaWxlVG9RdWV1ZSxcbiAgICAgICAgICAgICAgICB0aGlzLl9vbkZpbGUsXG4gICAgICAgICAgICApO1xuICAgICAgICAgICAgY2thbi5wdWJzdWIuc3Vic2NyaWJlKFxuICAgICAgICAgICAgICAgIGNrYW4uQ0tBTkVYVF9GSUxFUy50b3BpY3MucmVzdG9yZUZpbGVJblF1ZXVlLFxuICAgICAgICAgICAgICAgIHRoaXMuX29uRmlsZSxcbiAgICAgICAgICAgICk7XG5cbiAgICAgICAgICAgIHRoaXMudHBsID0gdGhpcy4kKFwiW2RhdGEtdXBsb2FkLXRlbXBsYXRlXVwiKVxuICAgICAgICAgICAgICAgIC5yZW1vdmUoKVxuICAgICAgICAgICAgICAgIC5yZW1vdmVBdHRyKFwiZGF0YS11cGxvYWQtdGVtcGxhdGUgaGlkZGVuXCIpO1xuXG4gICAgICAgICAgICB0aGlzLndpZGdldHMgPSBuZXcgV2Vha01hcCgpO1xuICAgICAgICB9LFxuXG4gICAgICAgIHRlYXJkb3duKCkge1xuICAgICAgICAgICAgY2thbi5wdWJzdWIudW5zdWJzY3JpYmUoXG4gICAgICAgICAgICAgICAgY2thbi5DS0FORVhUX0ZJTEVTLnRvcGljcy5hZGRGaWxlVG9RdWV1ZSxcbiAgICAgICAgICAgICAgICB0aGlzLl9vbkZpbGUsXG4gICAgICAgICAgICApO1xuICAgICAgICAgICAgY2thbi5wdWJzdWIudW5zdWJzY3JpYmUoXG4gICAgICAgICAgICAgICAgY2thbi5DS0FORVhUX0ZJTEVTLnRvcGljcy5yZXN0b3JlRmlsZUluUXVldWUsXG4gICAgICAgICAgICAgICAgdGhpcy5fb25GaWxlLFxuICAgICAgICAgICAgKTtcbiAgICAgICAgfSxcblxuICAgICAgICBfb25GaWxlKFxuICAgICAgICAgICAgZmlsZTogRmlsZSxcbiAgICAgICAgICAgIG9wdGlvbnMgPSB7XG4gICAgICAgICAgICAgICAgaW1tZWRpYXRlOiBmYWxzZSxcbiAgICAgICAgICAgICAgICBpZDogXCJcIixcbiAgICAgICAgICAgICAgICB1cGxvYWRlZDogMCxcbiAgICAgICAgICAgICAgICB1cGxvYWRlckluc3RhbmNlOiBudWxsLFxuICAgICAgICAgICAgICAgIHVwbG9hZGVyOiBudWxsLFxuICAgICAgICAgICAgICAgIHN0b3JhZ2U6IG51bGwsXG4gICAgICAgICAgICB9LFxuICAgICAgICApIHtcbiAgICAgICAgICAgIGNvbnN0IHdpZGdldCA9IHRoaXMudHBsLmNsb25lKHRydWUpLmFwcGVuZFRvKHRoaXMuZWwpO1xuICAgICAgICAgICAgY29uc3QgaW5mbyA9IHtcbiAgICAgICAgICAgICAgICBmaWxlLFxuICAgICAgICAgICAgICAgIGlkOiBvcHRpb25zLmlkLFxuICAgICAgICAgICAgICAgIHVwbG9hZGVkOiBvcHRpb25zLnVwbG9hZGVkIHx8IDAsXG4gICAgICAgICAgICAgICAgdXBsb2FkZXI6XG4gICAgICAgICAgICAgICAgICAgIG9wdGlvbnMudXBsb2FkZXJJbnN0YW5jZSB8fFxuICAgICAgICAgICAgICAgICAgICB0aGlzLnNhbmRib3guZmlsZXMubWFrZVVwbG9hZGVyKFxuICAgICAgICAgICAgICAgICAgICAgICAgb3B0aW9ucy51cGxvYWRlciB8fCB0aGlzLm9wdGlvbnMudXBsb2FkZXIsXG4gICAgICAgICAgICAgICAgICAgICAgICB7IHN0b3JhZ2U6IG9wdGlvbnMuc3RvcmFnZSB8fCB0aGlzLm9wdGlvbnMuc3RvcmFnZSB9LFxuICAgICAgICAgICAgICAgICAgICApLFxuICAgICAgICAgICAgfTtcblxuICAgICAgICAgICAgdGhpcy53aWRnZXRzLnNldCh3aWRnZXRbMF0sIGluZm8pO1xuXG4gICAgICAgICAgICB3aWRnZXQub24oXCJjbGlja1wiLCBcIltkYXRhLXVwbG9hZC1yZXN1bWVdXCIsIHRoaXMuX29uV2lkZ2V0UmVzdW1lKTtcbiAgICAgICAgICAgIHdpZGdldC5vbihcImNsaWNrXCIsIFwiW2RhdGEtdXBsb2FkLXBhdXNlXVwiLCB0aGlzLl9vbldpZGdldFBhdXNlKTtcblxuICAgICAgICAgICAgaW5mby51cGxvYWRlci5hZGRFdmVudExpc3RlbmVyKFxuICAgICAgICAgICAgICAgIFwiY29tbWl0XCIsXG4gICAgICAgICAgICAgICAgKGV2ZW50OiBDdXN0b21FdmVudCkgPT4gKGluZm8uaWQgPSBldmVudC5kZXRhaWwuaWQpLFxuICAgICAgICAgICAgKTtcbiAgICAgICAgICAgIGluZm8udXBsb2FkZXIuYWRkRXZlbnRMaXN0ZW5lcihcbiAgICAgICAgICAgICAgICBcImZhaWxcIixcbiAgICAgICAgICAgICAgICAoe1xuICAgICAgICAgICAgICAgICAgICBkZXRhaWw6IHsgcmVhc29ucywgZmlsZSB9LFxuICAgICAgICAgICAgICAgIH06IEN1c3RvbUV2ZW50PHtcbiAgICAgICAgICAgICAgICAgICAgcmVhc29uczogeyBba2V5OiBzdHJpbmddOiBzdHJpbmdbXSB9O1xuICAgICAgICAgICAgICAgICAgICBmaWxlOiBGaWxlO1xuICAgICAgICAgICAgICAgIH0+KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5ub3RpZnkoXG4gICAgICAgICAgICAgICAgICAgICAgICBmaWxlLm5hbWUsXG4gICAgICAgICAgICAgICAgICAgICAgICBPYmplY3QuZW50cmllcyhyZWFzb25zKVxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIC5maWx0ZXIoKFtrLCB2XSkgPT4ga1swXSAhPT0gXCJfXCIpXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgLm1hcCgoW2ssIHZdKSA9PlxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBBcnJheS5pc0FycmF5KHYpID8gdi5qb2luKFwiOyBcIikgOiB2LFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIClcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAuam9pbihcIjsgXCIpLFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgICAgICB0aGlzLnRvZ2dsZUFuaW1hdGlvbih3aWRnZXQsIGZhbHNlKTtcblxuICAgICAgICAgICAgICAgICAgICB3aWRnZXRcbiAgICAgICAgICAgICAgICAgICAgICAgIC5maW5kKFwiW2RhdGEtdXBsb2FkLXByb2dyZXNzXVwiKVxuICAgICAgICAgICAgICAgICAgICAgICAgLnJlbW92ZUNsYXNzKFwiYmctcHJpbWFyeSBiZy1zZWNvbmRhcnlcIilcbiAgICAgICAgICAgICAgICAgICAgICAgIC5hZGRDbGFzcyhcImJnLWRhbmdlciBwcm9ncmVzcy1iYXItZGFuZ2VyXCIpO1xuICAgICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICApO1xuICAgICAgICAgICAgaW5mby51cGxvYWRlci5hZGRFdmVudExpc3RlbmVyKFxuICAgICAgICAgICAgICAgIFwiZXJyb3JcIixcbiAgICAgICAgICAgICAgICAoe1xuICAgICAgICAgICAgICAgICAgICBkZXRhaWw6IHsgbWVzc2FnZSwgZmlsZSB9LFxuICAgICAgICAgICAgICAgIH06IEN1c3RvbUV2ZW50PHsgbWVzc2FnZTogc3RyaW5nOyBmaWxlOiBGaWxlIH0+KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5ub3RpZnkoZmlsZS5uYW1lLCBtZXNzYWdlKTtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy50b2dnbGVBbmltYXRpb24od2lkZ2V0LCBmYWxzZSk7XG4gICAgICAgICAgICAgICAgICAgIHdpZGdldFxuICAgICAgICAgICAgICAgICAgICAgICAgLmZpbmQoXCJbZGF0YS11cGxvYWQtcHJvZ3Jlc3NdXCIpXG4gICAgICAgICAgICAgICAgICAgICAgICAucmVtb3ZlQ2xhc3MoXCJiZy1wcmltYXJ5IGJnLXNlY29uZGFyeVwiKVxuICAgICAgICAgICAgICAgICAgICAgICAgLmFkZENsYXNzKFwiYmctZGFuZ2VyIHByb2dyZXNzLWJhci1kYW5nZXJcIik7XG4gICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICk7XG5cbiAgICAgICAgICAgIGluZm8udXBsb2FkZXIuYWRkRXZlbnRMaXN0ZW5lcihcbiAgICAgICAgICAgICAgICBcInByb2dyZXNzXCIsXG4gICAgICAgICAgICAgICAgKHsgZGV0YWlsOiB7IGxvYWRlZCwgdG90YWwgfSB9OiBDdXN0b21FdmVudCkgPT5cbiAgICAgICAgICAgICAgICAgICAgdGhpcy5zZXRXaWRnZXRDb21wbGV0aW9uKHdpZGdldCwgbG9hZGVkLCB0b3RhbCksXG4gICAgICAgICAgICApO1xuICAgICAgICAgICAgaW5mby51cGxvYWRlci5hZGRFdmVudExpc3RlbmVyKFxuICAgICAgICAgICAgICAgIFwiZmluaXNoXCIsXG4gICAgICAgICAgICAgICAgKHsgZGV0YWlsOiB7IGZpbGUsIHJlc3VsdCB9IH06IEN1c3RvbUV2ZW50KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMudG9nZ2xlQW5pbWF0aW9uKHdpZGdldCwgZmFsc2UpO1xuICAgICAgICAgICAgICAgICAgICB3aWRnZXRcbiAgICAgICAgICAgICAgICAgICAgICAgIC5maW5kKFwiW2RhdGEtdXBsb2FkLXByb2dyZXNzXVwiKVxuICAgICAgICAgICAgICAgICAgICAgICAgLnJlbW92ZUNsYXNzKFwiYmctcHJpbWFyeSBiZy1zZWNvbmRhcnlcIilcbiAgICAgICAgICAgICAgICAgICAgICAgIC5hZGRDbGFzcyhcImJnLXN1Y2Nlc3MgcHJvZ3Jlc3MtYmFyLXN1Y2Nlc3NcIik7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5wdWJsaXNoKFxuICAgICAgICAgICAgICAgICAgICAgICAgY2thbi5DS0FORVhUX0ZJTEVTLnRvcGljcy5xdWV1ZUl0ZW1VcGxvYWRlZCxcbiAgICAgICAgICAgICAgICAgICAgICAgIGZpbGUsXG4gICAgICAgICAgICAgICAgICAgICAgICByZXN1bHQsXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICk7XG5cbiAgICAgICAgICAgIHRoaXMuc2V0V2lkZ2V0TmFtZSh3aWRnZXQsIGluZm8uZmlsZS5uYW1lKTtcbiAgICAgICAgICAgIHRoaXMuc2V0V2lkZ2V0Q29tcGxldGlvbih3aWRnZXQsIGluZm8udXBsb2FkZWQsIGluZm8uZmlsZS5zaXplKTtcblxuICAgICAgICAgICAgaWYgKG9wdGlvbnMuaW1tZWRpYXRlKSB7XG4gICAgICAgICAgICAgICAgd2lkZ2V0LmZpbmQoXCJbZGF0YS11cGxvYWQtcmVzdW1lXVwiKS50cmlnZ2VyKFwiY2xpY2tcIik7XG4gICAgICAgICAgICB9XG4gICAgICAgIH0sXG5cbiAgICAgICAgc2V0V2lkZ2V0TmFtZSh3aWRnZXQ6IEpRdWVyeSwgbmFtZTogc3RyaW5nKSB7XG4gICAgICAgICAgICB3aWRnZXQuZmluZChcIltkYXRhLWl0ZW0tbmFtZV1cIikudGV4dChuYW1lKTtcbiAgICAgICAgfSxcblxuICAgICAgICBzZXRXaWRnZXRDb21wbGV0aW9uKHdpZGdldDogSlF1ZXJ5LCB1cGxvYWRlZDogbnVtYmVyLCB0b3RhbDogbnVtYmVyKSB7XG4gICAgICAgICAgICBjb25zdCB2YWx1ZSA9ICh1cGxvYWRlZCAqIDEwMCkgLyB0b3RhbDtcbiAgICAgICAgICAgIGNvbnN0IGluZm8gPSB0aGlzLndpZGdldHMuZ2V0KHdpZGdldFswXSk7XG4gICAgICAgICAgICBpbmZvLnVwbG9hZGVkID0gdXBsb2FkZWQ7XG5cbiAgICAgICAgICAgIGNvbnN0IGNvbXBsZXRpb24gPSB2YWx1ZS50b0ZpeGVkKDApICsgXCIlXCI7XG4gICAgICAgICAgICB3aWRnZXRcbiAgICAgICAgICAgICAgICAuZmluZChcIltkYXRhLXVwbG9hZC1wcm9ncmVzc11cIilcbiAgICAgICAgICAgICAgICAudGV4dChjb21wbGV0aW9uKVxuICAgICAgICAgICAgICAgIC5jc3MoXCJ3aWR0aFwiLCBjb21wbGV0aW9uKTtcbiAgICAgICAgfSxcblxuICAgICAgICB0b2dnbGVBbmltYXRpb24od2lkZ2V0OiBKUXVlcnksIHN0YXRlOiBib29sZWFuKSB7XG4gICAgICAgICAgICB3aWRnZXRcbiAgICAgICAgICAgICAgICAuZmluZChcIltkYXRhLXVwbG9hZC1wcm9ncmVzc11cIilcbiAgICAgICAgICAgICAgICAudG9nZ2xlQ2xhc3MoXCJwcm9ncmVzcy1iYXItYW5pbWF0ZWQgYWN0aXZlXCIsIHN0YXRlKTtcbiAgICAgICAgfSxcblxuICAgICAgICBfb25XaWRnZXRSZXN1bWUoZXZlbnQ6IEpRdWVyeS5UcmlnZ2VyZWRFdmVudCkge1xuICAgICAgICAgICAgY29uc3QgaW5mbyA9IHRoaXMud2lkZ2V0cy5nZXQoZXZlbnQuZGVsZWdhdGVUYXJnZXQpO1xuICAgICAgICAgICAgaWYgKGluZm8udXBsb2FkZWQgPj0gaW5mby50b3RhbCkgcmV0dXJuO1xuXG4gICAgICAgICAgICBjb25zdCB3aWRnZXQgPSAkKGV2ZW50LmRlbGVnYXRlVGFyZ2V0KTtcbiAgICAgICAgICAgIHdpZGdldFxuICAgICAgICAgICAgICAgIC5maW5kKFwiW2RhdGEtdXBsb2FkLXByb2dyZXNzXVwiKVxuICAgICAgICAgICAgICAgIC5yZW1vdmVDbGFzcyhcImJnLXNlY29uZGFyeVwiKVxuICAgICAgICAgICAgICAgIC5hZGRDbGFzcyhcImJnLXByaW1hcnlcIik7XG5cbiAgICAgICAgICAgIGlmIChpbmZvLmlkKSB7XG4gICAgICAgICAgICAgICAgaW5mby51cGxvYWRlci5yZXN1bWUoaW5mby5maWxlLCBpbmZvLmlkKTtcbiAgICAgICAgICAgIH0gZWxzZSB7XG4gICAgICAgICAgICAgICAgaW5mby51cGxvYWRlci51cGxvYWQoaW5mby5maWxlKTtcbiAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgdGhpcy50b2dnbGVBbmltYXRpb24od2lkZ2V0LCB0cnVlKTtcbiAgICAgICAgfSxcblxuICAgICAgICBfb25XaWRnZXRQYXVzZShldmVudDogSlF1ZXJ5LlRyaWdnZXJlZEV2ZW50KSB7XG4gICAgICAgICAgICBjb25zdCBpbmZvID0gdGhpcy53aWRnZXRzLmdldChldmVudC5kZWxlZ2F0ZVRhcmdldCk7XG4gICAgICAgICAgICBpZiAoaW5mby51cGxvYWRlZCA+PSBpbmZvLnRvdGFsKSByZXR1cm47XG5cbiAgICAgICAgICAgIGNvbnN0IHdpZGdldCA9ICQoZXZlbnQuZGVsZWdhdGVUYXJnZXQpO1xuICAgICAgICAgICAgd2lkZ2V0XG4gICAgICAgICAgICAgICAgLmZpbmQoXCJbZGF0YS11cGxvYWQtcHJvZ3Jlc3NdXCIpXG4gICAgICAgICAgICAgICAgLnJlbW92ZUNsYXNzKFwiYmctcHJpbWFyeVwiKVxuICAgICAgICAgICAgICAgIC5hZGRDbGFzcyhcImJnLXNlY29uZGFyeVwiKTtcblxuICAgICAgICAgICAgaW5mby51cGxvYWRlci5wYXVzZShpbmZvLmZpbGUpO1xuICAgICAgICAgICAgdGhpcy50b2dnbGVBbmltYXRpb24od2lkZ2V0LCBmYWxzZSk7XG4gICAgICAgIH0sXG4gICAgfTtcbn0pO1xuIl19
+//# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiZmlsZXMtLW1vZHVsZXMuanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi90cy9maWxlcy0tbW9kdWxlcy50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiQUFBQTs7OztHQUlHO0FBQ0gsSUFBSSxDQUFDLE1BQU0sQ0FBQyxrQkFBa0IsRUFBRSxVQUFVLENBQUM7SUFDdkMsT0FBTztRQUNILE9BQU8sRUFBRTtZQUNMLFNBQVMsRUFBRSxLQUFLO1NBQ25CO1FBQ0QsVUFBVTtZQUNOLE1BQU0sU0FBUyxHQUFHLElBQUksQ0FBQyxDQUFDLENBQUMsd0JBQXdCLENBQUMsQ0FBQztZQUNuRCxTQUFTLENBQUMsRUFBRSxDQUFDLE1BQU0sRUFBRSxDQUFDLEtBQVksRUFBRSxFQUFFLENBQUMsS0FBSyxDQUFDLGNBQWMsRUFBRSxDQUFDLENBQUM7WUFDL0QsU0FBUyxDQUFDLEVBQUUsQ0FBQyxRQUFRLEVBQUUsQ0FBQyxLQUFZLEVBQUUsRUFBRSxDQUNwQyxJQUFJLENBQUMsSUFBSSxDQUFDLEdBQUksS0FBSyxDQUFDLE1BQTJCLENBQUMsS0FBTSxDQUFDLENBQzFELENBQUM7UUFDTixDQUFDO1FBRUQsSUFBSSxDQUFDLEdBQUcsS0FBYTtZQUNqQixLQUFLLENBQUMsT0FBTyxDQUFDLENBQUMsSUFBSSxFQUFFLEVBQUUsQ0FDbkIsSUFBSSxDQUFDLE9BQU8sQ0FBQyxPQUFPLENBQ2hCLElBQUksQ0FBQyxhQUFhLENBQUMsTUFBTSxDQUFDLGNBQWMsRUFDeEMsSUFBSSxFQUNKLEVBQUUsU0FBUyxFQUFFLElBQUksQ0FBQyxPQUFPLENBQUMsU0FBUyxFQUFFLENBQ3hDLENBQ0osQ0FBQztRQUNOLENBQUM7S0FDSixDQUFDO0FBQ04sQ0FBQyxDQUFDLENBQUM7QUFFSDs7O0dBR0c7QUFDSCxJQUFJLENBQUMsTUFBTSxDQUFDLGlCQUFpQixFQUFFLFVBQVUsQ0FBQztJQUN0QyxPQUFPO1FBQ0gsT0FBTyxFQUFFO1lBQ0wsU0FBUyxFQUFFLEtBQUs7U0FDbkI7UUFF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QUN2QyxDQUFDO1FBRUQsY0FBYyxDQUFDLEtBQTRCO1lBQ3ZDLE1BQU0sSUFBSSxHQUFHLElBQUksQ0FBQyxPQUFPLENBQUMsR0FBRyxDQUFDLEtBQUssQ0FBQyxjQUFjLENBQUMsQ0FBQztZQUNwRCxJQUFJLElBQUksQ0FBQyxRQUFRLElBQUksSUFBSSxDQUFDLEtBQUs7Z0JBQUUsT0FBTztZQUV4QyxNQUFNLE1BQU0sR0FBRyxDQUFDLENBQUMsS0FBSyxDQUFDLGNBQWMsQ0FBQyxDQUFDO1lBQ3ZDLE1BQU07aUJBQ0QsSUFBSSxDQUFDLHdCQUF3QixDQUFDO2lCQUM5QixXQUFXLENBQUMsWUFBWSxDQUFDO2lCQUN6QixRQUFRLENBQUMsY0FBYyxDQUFDLENBQUM7WUFFOUIsSUFBSSxDQUFDLFFBQVEsQ0FBQyxLQUFLLENBQUMsSUFBSSxDQUFDLElBQUksQ0FBQyxDQUFDO1lBQy9CLElBQUksQ0FBQyxlQUFlLENBQUMsTUFBTSxFQUFFLEtBQUssQ0FBQyxDQUFDO1FBQ3hDLENBQUM7S0FDSixDQUFDO0FBQ04sQ0FBQyxDQUFDLENBQUMiLCJzb3VyY2VzQ29udGVudCI6WyIvKipcbiAqIEFkZCBzZWxlY3RlZCBmaWxlIHRvIHVwbG9hZCBxdWV1ZSB3aGVuZXZlciBgW2RhdGEtcXVldWUtc2NoZWR1bGVyXWBcbiAqIGRpc3BhdGNoZXMgYGNoYW5nZWAgZXZlbnQuXG4gKlxuICovXG5ja2FuLm1vZHVsZShcImZpbGVzLS1zY2hlZHVsZXJcIiwgZnVuY3Rpb24gKCQpIHtcbiAgICByZXR1cm4ge1xuICAgICAgICBvcHRpb25zOiB7XG4gICAgICAgICAgICBpbW1lZGlhdGU6IGZhbHNlLFxuICAgICAgICB9LFxuICAgICAgICBpbml0aWFsaXplKCkge1xuICAgICAgICAgICAgY29uc3Qgc2NoZWR1bGVyID0gdGhpcy4kKFwiW2RhdGEtcXVldWUtc2NoZWR1bGVyXVwiKTtcbiAgICAgICAgICAgIHNjaGVkdWxlci5vbihcImRyb3BcIiwgKGV2ZW50OiBFdmVudCkgPT4gZXZlbnQucHJldmVudERlZmF1bHQoKSk7XG4gICAgICAgICAgICBzY2hlZHVsZXIub24oXCJjaGFuZ2VcIiwgKGV2ZW50OiBFdmVudCkgPT5cbiAgICAgICAgICAgICAgICB0aGlzLnB1c2goLi4uKGV2ZW50LnRhcmdldCBhcyBIVE1MSW5wdXRFbGVtZW50KS5maWxlcyEpLFxuICAgICAgICAgICAgKTtcbiAgICAgICAgfSxcblxuICAgICAgICBwdXNoKC4uLmZpbGVzOiBGaWxlW10pIHtcbiAgICAgICAgICAgIGZpbGVzLmZvckVhY2goKGZpbGUpID0+XG4gICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94LnB1Ymxpc2goXG4gICAgICAgICAgICAgICAgICAgIGNrYW4uQ0tBTkVYVF9GSUxFUy50b3BpY3MuYWRkRmlsZVRvUXVldWUsXG4gICAgICAgICAgICAgICAgICAgIGZpbGUsXG4gICAgICAgICAgICAgICAgICAgIHsgaW1tZWRpYXRlOiB0aGlzLm9wdGlvbnMuaW1tZWRpYXRlIH0sXG4gICAgICAgICAgICAgICAgKSxcbiAgICAgICAgICAgICk7XG4gICAgICAgIH0sXG4gICAgfTtcbn0pO1xuXG4vKipcbiAqIEFkZCBmaWxlL2RpcmVjdG9yaWVzIHRvIHVwbG9hZCBxdWV1ZSB2aWEgZHJhZyduJ2Ryb3AuXG4gKlxuICovXG5ja2FuLm1vZHVsZShcImZpbGVzLS1kcm9wem9uZVwiLCBmdW5jdGlvbiAoJCkge1xuICAgIHJldHVybiB7XG4gICAgICAgIG9wdGlvbnM6IHtcbiAgICAgICAgICAgIGltbWVkaWF0ZTogZmFsc2UsXG4gICAgICAgIH0sXG5cbiAgICAgICAgaW5pdGlhbGl6ZSgpIHtcbiAgICAgICAgICAgICQucHJveHlBbGwodGhpcywgL19vbi8pO1xuICAgICAgICAgICAgY29uc3QgZWxlbWVudCA9IHRoaXMuZWxbMF07XG5cbiAgICAgICAgICAgIGVsZW1lbnQuYWRkRXZlbnRMaXN0ZW5lcihcImRyYWdvdmVyXCIsIHRoaXMuX29uRHJhZ092ZXIpO1xuICAgICAgICAgICAgZWxlbWVudC5hZGRFdmVudExpc3RlbmVyKFwiZHJhZ2VudGVyXCIsIHRoaXMuX29uRHJhZ0VudGVyKTtcbiAgICAgICAgICAgIGVsZW1lbnQuYWRkRXZlbnRMaXN0ZW5lcihcImRyYWdsZWF2ZVwiLCB0aGlzLl9vbkRyYWdMZWF2ZSk7XG4gICAgICAgICAgICBlbGVtZW50LmFkZEV2ZW50TGlzdGVuZXIoXCJkcm9wXCIsIHRoaXMuX29uRHJvcCk7XG4gICAgICAgIH0sXG5cbiAgICAgICAgX29uRHJhZ092ZXIoZXZlbnQ6IERyYWdFdmVudCkge1xuICAgICAgICAgICAgZXZlbnQucHJldmVudERlZmF1bHQoKTtcbiAgICAgICAgfSxcbiAgICAgICAgX29uRHJhZ0VudGVyKGV2ZW50OiBEcmFnRXZlbnQpIHt9LFxuICAgICAgICBfb25EcmFnTGVhdmUoZXZlbnQ6IERyYWdFdmVudCkge30sXG5cbiAgICAgICAgX29uRHJvcChldmVudDogRHJhZ0V2ZW50KSB7XG4gICAgICAgICAgICBldmVudC5wcmV2ZW50RGVmYXVsdCgpO1xuICAgICAgICAgICAgaWYgKCFldmVudC5kYXRhVHJhbnNmZXIpIHtcbiAgICAgICAgICAgICAgICByZXR1cm47XG4gICAgICAgICAgICB9XG5cbiAgICAgICAgICAgIGZvciAobGV0IGVudHJ5IG9mIGV2ZW50LmRhdGFUcmFuc2Zlci5pdGVtcykge1xuICAgICAgICAgICAgICAgIHRoaXMuc2NhbkVudHJ5KGVudHJ5LndlYmtpdEdldEFzRW50cnkoKSwgKGZpbGU6IEZpbGUpID0+XG4gICAgICAgICAgICAgICAgICAgIHRoaXMucHVzaChmaWxlKSxcbiAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgfVxuICAgICAgICB9LFxuXG4gICAgICAgIHNjYW5FbnRyeShcbiAgICAgICAgICAgIGVudHJ5OiBGaWxlU3lzdGVtRmlsZUVudHJ5IHwgRmlsZVN5c3RlbURpcmVjdG9yeUVudHJ5LFxuICAgICAgICAgICAgY2I6IChmaWxlOiBGaWxlKSA9PiB2b2lkLFxuICAgICAgICApIHtcbiAgICAgICAgICAgIGlmIChlbnRyeS5pc0ZpbGUpIHtcbiAgICAgICAgICAgICAgICAoZW50cnkgYXMgRmlsZVN5c3RlbUZpbGVFbnRyeSkuZmlsZShjYik7XG4gICAgICAgICAgICB9IGVsc2Uge1xuICAgICAgICAgICAgICAgIChlbnRyeSBhcyBGaWxlU3lzdGVtRGlyZWN0b3J5RW50cnkpXG4gICAgICAgICAgICAgICAgICAgIC5jcmVhdGVSZWFkZXIoKVxuICAgICAgICAgICAgICAgICAgICAucmVhZEVudHJpZXMoKGVudHJpZXMpID0+XG4gICAgICAgICAgICAgICAgICAgICAgICBlbnRyaWVzLmZvckVhY2goKGUpID0+IHRoaXMuc2NhbkVudHJ5KGUsIGNiKSksXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICB9XG4gICAgICAgIH0sXG5cbiAgICAgICAgcHVzaChmaWxlOiBGaWxlKSB7XG4gICAgICAgICAgICB0aGlzLnNhbmRib3gucHVibGlzaChcbiAgICAgICAgICAgICAgICBja2FuLkNLQU5FWFRfRklMRVMudG9waWNzLmFkZEZpbGVUb1F1ZXVlLFxuICAgICAgICAgICAgICAgIGZpbGUsXG4gICAgICAgICAgICAgICAgeyBpbW1lZGlhdGU6IHRoaXMub3B0aW9ucy5pbW1lZGlhdGUgfSxcbiAgICAgICAgICAgICk7XG4gICAgICAgIH0sXG4gICAgfTtcbn0pO1xuXG4vKipcbiAqIEFkZCB0byBxdWV1ZSBhIGZpbGUsIHRoYXQgaGFzIGFzc29jaWF0ZWQgaW5jb21wbGV0ZSB1cGxvYWQuXG4gKlxuICogU3VwcG9ydHMgYSBudW1iZXIgb2YgcHJvcGVydGllcyB0byB2ZXJpZnkgdGhhdCB0aGUgbmV3IGZpbGUgbWF0Y2hlc1xuICogcHJldmlvdXNseSB1cGxvYWRlZCBmaWxlLlxuICpcbiAqXG4gKi9cbmNrYW4ubW9kdWxlKFwiZmlsZXMtLXJlc3RvcmVyXCIsIGZ1bmN0aW9uICgkKSB7XG4gICAgcmV0dXJuIHtcbiAgICAgICAgb3B0aW9uczoge1xuICAgICAgICAgICAgbmFtZTogXCJcIixcbiAgICAgICAgICAgIHNpemU6IDAsXG4gICAgICAgICAgICB1cGxvYWRlZDogMCxcbiAgICAgICAgICAgIGlkOiBcIlwiLFxuICAgICAgICAgICAgaW1tZWRpYXRlOiBmYWxzZSxcbiAgICAgICAgfSxcblxuICAgICAgICBpbml0aWFsaXplKCkge1xuICAgICAgICAgICAgJC5wcm94eUFsbCh0aGlzLCAvX29uLyk7XG4gICAgICAgICAgICB0aGlzLmVsLm9uKFwiY2hhbmdlXCIsIHRoaXMuX29uQ2hhbmdlKTtcbiAgICAgICAgfSxcblxuICAgICAgICBfb25DaGFuZ2UoZXZlbnQ6IEV2ZW50KSB7XG4gICAgICAgICAgICBjb25zdCBmaWxlID0gKGV2ZW50LnRhcmdldCBhcyBIVE1MSW5wdXRFbGVtZW50KS5maWxlcz8uWzBdO1xuXG4gICAgICAgICAgICBpZiAoIWZpbGUpIHtcbiAgICAgICAgICAgICAgICByZXR1cm47XG4gICAgICAgICAgICB9XG5cbiAgICAgICAgICAgIGlmICh0aGlzLm9wdGlvbnMubmFtZSAmJiBmaWxlLm5hbWUgIT09IHRoaXMub3B0aW9ucy5uYW1lKSB7XG4gICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94Lm5vdGlmeShcbiAgICAgICAgICAgICAgICAgICAgXCJOYW1lIG1pc21hdGNoLlwiLFxuICAgICAgICAgICAgICAgICAgICBgRXhwZWN0ZWQgbmFtZTogJHt0aGlzLm9wdGlvbnMubmFtZX1gLFxuICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94Lm5vdGlmeS5lbFswXS5zY3JvbGxJbnRvVmlldygpO1xuICAgICAgICAgICAgICAgIHJldHVybjtcbiAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgaWYgKHRoaXMub3B0aW9ucy5zaXplICYmIGZpbGUuc2l6ZSAhPT0gdGhpcy5vcHRpb25zLnNpemUpIHtcbiAgICAgICAgICAgICAgICB0aGlzLnNhbmRib3gubm90aWZ5KFxuICAgICAgICAgICAgICAgICAgICBcIlNpemUgbWlzbWF0Y2guXCIsXG4gICAgICAgICAgICAgICAgICAgIGBFeHBlY3RlZCBzaXplOiAke3RoaXMub3B0aW9ucy5zaXplLnRvTG9jYWxlU3RyaW5nKCl9IGJ5dGVzYCxcbiAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5ub3RpZnkuZWxbMF0uc2Nyb2xsSW50b1ZpZXcoKTtcbiAgICAgICAgICAgICAgICByZXR1cm47XG4gICAgICAgICAgICB9XG5cbiAgICAgICAgICAgIHRoaXMuc2FuZGJveC5wdWJsaXNoKFxuICAgICAgICAgICAgICAgIGNrYW4uQ0tBTkVYVF9GSUxFUy50b3BpY3MucmVzdG9yZUZpbGVJblF1ZXVlLFxuICAgICAgICAgICAgICAgIGZpbGUsXG4gICAgICAgICAgICAgICAge1xuICAgICAgICAgICAgICAgICAgICBpZDogdGhpcy5vcHRpb25zLmlkLFxuICAgICAgICAgICAgICAgICAgICB1cGxvYWRlZDogdGhpcy5vcHRpb25zLnVwbG9hZGVkLFxuICAgICAgICAgICAgICAgICAgICBpbW1lZGlhdGU6IHRoaXMub3B0aW9ucy5pbW1lZGlhdGUsXG4gICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICk7XG4gICAgICAgIH0sXG4gICAgfTtcbn0pO1xuXG5ja2FuLm1vZHVsZShcImZpbGVzLS1zaGFyZWQtcXVldWVcIiwgZnVuY3Rpb24gKCQpIHtcbiAgICByZXR1cm4ge1xuICAgICAgICBpbml0aWFsaXplKCkge1xuICAgICAgICAgICAgJC5wcm94eUFsbCh0aGlzLCAvX29uLyk7XG5cbiAgICAgICAgICAgIHRoaXMud29ya2VyID0gbmV3IFNoYXJlZFdvcmtlcihcbiAgICAgICAgICAgICAgICB0aGlzLnNhbmRib3gudXJsKFxuICAgICAgICAgICAgICAgICAgICBcImNrYW5leHQtZmlsZXMvc2NyaXB0cy9maWxlcy0tc2hhcmVkLXVwbG9hZGVyLmpzXCIsXG4gICAgICAgICAgICAgICAgKSxcbiAgICAgICAgICAgICk7XG5cbiAgICAgICAgICAgIHRoaXMud29ya2VyLnBvcnQub25tZXNzYWdlID0gY29uc29sZS5kZWJ1ZztcbiAgICAgICAgfSxcbiAgICB9O1xufSk7XG5cbmNrYW4ubW9kdWxlKFwiZmlsZXMtLXF1ZXVlXCIsIGZ1bmN0aW9uICgkKSB7XG4gICAgcmV0dXJuIHtcbiAgICAgICAgb3B0aW9uczoge1xuICAgICAgICAgICAgc3RvcmFnZTogXCJkZWZhdWx0XCIsXG4gICAgICAgICAgICB1cGxvYWRlcjogXCJTdGFuZGFyZFwiLFxuICAgICAgICB9LFxuXG4gICAgICAgIGluaXRpYWxpemUoKSB7XG4gICAgICAgICAgICAkLnByb3h5QWxsKHRoaXMsIC9fb24vKTtcbiAgICAgICAgICAgIGNrYW4ucHVic3ViLnN1YnNjcmliZShcbiAgICAgICAgICAgICAgICBja2FuLkNLQU5FWFRfRklMRVMudG9waWNzLmFkZEZpbGVUb1F1ZXVlLFxuICAgICAgICAgICAgICAgIHRoaXMuX29uRmlsZSxcbiAgICAgICAgICAgICk7XG4gICAgICAgICAgICBja2FuLnB1YnN1Yi5zdWJzY3JpYmUoXG4gICAgICAgICAgICAgICAgY2thbi5DS0FORVhUX0ZJTEVTLnRvcGljcy5yZXN0b3JlRmlsZUluUXVldWUsXG4gICAgICAgICAgICAgICAgdGhpcy5fb25GaWxlLFxuICAgICAgICAgICAgKTtcblxuICAgICAgICAgICAgdGhpcy50cGwgPSB0aGlzLiQoXCJbZGF0YS11cGxvYWQtdGVtcGxhdGVdXCIpXG4gICAgICAgICAgICAgICAgLnJlbW92ZSgpXG4gICAgICAgICAgICAgICAgLnJlbW92ZUF0dHIoXCJkYXRhLXVwbG9hZC10ZW1wbGF0ZSBoaWRkZW5cIik7XG5cbiAgICAgICAgICAgIHRoaXMud2lkZ2V0cyA9IG5ldyBXZWFrTWFwKCk7XG4gICAgICAgIH0sXG5cbiAgICAgICAgdGVhcmRvd24oKSB7XG4gICAgICAgICAgICBja2FuLnB1YnN1Yi51bnN1YnNjcmliZShcbiAgICAgICAgICAgICAgICBja2FuLkNLQU5FWFRfRklMRVMudG9waWNzLmFkZEZpbGVUb1F1ZXVlLFxuICAgICAgICAgICAgICAgIHRoaXMuX29uRmlsZSxcbiAgICAgICAgICAgICk7XG4gICAgICAgICAgICBja2FuLnB1YnN1Yi51bnN1YnNjcmliZShcbiAgICAgICAgICAgICAgICBja2FuLkNLQU5FWFRfRklMRVMudG9waWNzLnJlc3RvcmVGaWxlSW5RdWV1ZSxcbiAgICAgICAgICAgICAgICB0aGlzLl9vbkZpbGUsXG4gICAgICAgICAgICApO1xuICAgICAgICB9LFxuXG4gICAgICAgIF9vbkZpbGUoXG4gICAgICAgICAgICBmaWxlOiBGaWxlLFxuICAgICAgICAgICAgb3B0aW9ucyA9IHtcbiAgICAgICAgICAgICAgICBpbW1lZGlhdGU6IGZhbHNlLFxuICAgICAgICAgICAgICAgIGlkOiBcIlwiLFxuICAgICAgICAgICAgICAgIHVwbG9hZGVkOiAwLFxuICAgICAgICAgICAgICAgIHVwbG9hZGVySW5zdGFuY2U6IG51bGwsXG4gICAgICAgICAgICAgICAgdXBsb2FkZXI6IG51bGwsXG4gICAgICAgICAgICAgICAgc3RvcmFnZTogbnVsbCxcbiAgICAgICAgICAgIH0sXG4gICAgICAgICkge1xuICAgICAgICAgICAgY29uc3Qgd2lkZ2V0ID0gdGhpcy50cGwuY2xvbmUodHJ1ZSkuYXBwZW5kVG8odGhpcy5lbCk7XG4gICAgICAgICAgICBjb25zdCBpbmZvID0ge1xuICAgICAgICAgICAgICAgIGZpbGUsXG4gICAgICAgICAgICAgICAgaWQ6IG9wdGlvbnMuaWQsXG4gICAgICAgICAgICAgICAgdXBsb2FkZWQ6IG9wdGlvbnMudXBsb2FkZWQgfHwgMCxcbiAgICAgICAgICAgICAgICB1cGxvYWRlcjpcbiAgICAgICAgICAgICAgICAgICAgb3B0aW9ucy51cGxvYWRlckluc3RhbmNlIHx8XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5maWxlcy5tYWtlVXBsb2FkZXIoXG4gICAgICAgICAgICAgICAgICAgICAgICBvcHRpb25zLnVwbG9hZGVyIHx8IHRoaXMub3B0aW9ucy51cGxvYWRlcixcbiAgICAgICAgICAgICAgICAgICAgICAgIHsgc3RvcmFnZTogb3B0aW9ucy5zdG9yYWdlIHx8IHRoaXMub3B0aW9ucy5zdG9yYWdlIH0sXG4gICAgICAgICAgICAgICAgICAgICksXG4gICAgICAgICAgICB9O1xuXG4gICAgICAgICAgICB0aGlzLndpZGdldHMuc2V0KHdpZGdldFswXSwgaW5mbyk7XG5cbiAgICAgICAgICAgIHdpZGdldC5vbihcImNsaWNrXCIsIFwiW2RhdGEtdXBsb2FkLXJlc3VtZV1cIiwgdGhpcy5fb25XaWRnZXRSZXN1bWUpO1xuICAgICAgICAgICAgd2lkZ2V0Lm9uKFwiY2xpY2tcIiwgXCJbZGF0YS11cGxvYWQtcGF1c2VdXCIsIHRoaXMuX29uV2lkZ2V0UGF1c2UpO1xuXG4gICAgICAgICAgICBpbmZvLnVwbG9hZGVyLmFkZEV2ZW50TGlzdGVuZXIoXG4gICAgICAgICAgICAgICAgXCJjb21taXRcIixcbiAgICAgICAgICAgICAgICAoZXZlbnQ6IEN1c3RvbUV2ZW50KSA9PiAoaW5mby5pZCA9IGV2ZW50LmRldGFpbC5pZCksXG4gICAgICAgICAgICApO1xuICAgICAgICAgICAgaW5mby51cGxvYWRlci5hZGRFdmVudExpc3RlbmVyKFxuICAgICAgICAgICAgICAgIFwiZmFpbFwiLFxuICAgICAgICAgICAgICAgICh7XG4gICAgICAgICAgICAgICAgICAgIGRldGFpbDogeyByZWFzb25zLCBmaWxlIH0sXG4gICAgICAgICAgICAgICAgfTogQ3VzdG9tRXZlbnQ8e1xuICAgICAgICAgICAgICAgICAgICByZWFzb25zOiB7IFtrZXk6IHN0cmluZ106IHN0cmluZ1tdIH07XG4gICAgICAgICAgICAgICAgICAgIGZpbGU6IEZpbGU7XG4gICAgICAgICAgICAgICAgfT4pID0+IHtcbiAgICAgICAgICAgICAgICAgICAgY29uc29sZS5sb2coaW5mby51cGxvYWRlciwgMSlcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94Lm5vdGlmeShcbiAgICAgICAgICAgICAgICAgICAgICAgIGZpbGUubmFtZSxcbiAgICAgICAgICAgICAgICAgICAgICAgIE9iamVjdC5lbnRyaWVzKHJlYXNvbnMpXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgLmZpbHRlcigoW2ssIHZdKSA9PiBrWzBdICE9PSBcIl9cIilcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAubWFwKChbaywgdl0pID0+XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIEFycmF5LmlzQXJyYXkodikgPyB2LmpvaW4oXCI7IFwiKSA6IHYsXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgKVxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIC5qb2luKFwiOyBcIiksXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5ub3RpZnkuZWxbMF0uc2Nyb2xsSW50b1ZpZXcoKTtcblxuICAgICAgICAgICAgICAgICAgICB0aGlzLnRvZ2dsZUFuaW1hdGlvbih3aWRnZXQsIGZhbHNlKTtcblxuICAgICAgICAgICAgICAgICAgICB3aWRnZXRcbiAgICAgICAgICAgICAgICAgICAgICAgIC5maW5kKFwiW2RhdGEtdXBsb2FkLXByb2dyZXNzXVwiKVxuICAgICAgICAgICAgICAgICAgICAgICAgLnJlbW92ZUNsYXNzKFwiYmctcHJpbWFyeSBiZy1zZWNvbmRhcnlcIilcbiAgICAgICAgICAgICAgICAgICAgICAgIC5hZGRDbGFzcyhcImJnLWRhbmdlciBwcm9ncmVzcy1iYXItZGFuZ2VyXCIpO1xuICAgICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICApO1xuICAgICAgICAgICAgaW5mby51cGxvYWRlci5hZGRFdmVudExpc3RlbmVyKFxuICAgICAgICAgICAgICAgIFwiZXJyb3JcIixcbiAgICAgICAgICAgICAgICAoe1xuICAgICAgICAgICAgICAgICAgICBkZXRhaWw6IHsgbWVzc2FnZSwgZmlsZSB9LFxuICAgICAgICAgICAgICAgIH06IEN1c3RvbUV2ZW50PHsgbWVzc2FnZTogc3RyaW5nOyBmaWxlOiBGaWxlIH0+KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgIGNvbnNvbGUubG9nKGluZm8udXBsb2FkZXIsIDIpXG4gICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5ub3RpZnkoZmlsZS5uYW1lLCBtZXNzYWdlKTtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94Lm5vdGlmeS5lbFswXS5zY3JvbGxJbnRvVmlldygpO1xuXG4gICAgICAgICAgICAgICAgICAgIHRoaXMudG9nZ2xlQW5pbWF0aW9uKHdpZGdldCwgZmFsc2UpO1xuICAgICAgICAgICAgICAgICAgICB3aWRnZXRcbiAgICAgICAgICAgICAgICAgICAgICAgIC5maW5kKFwiW2RhdGEtdXBsb2FkLXByb2dyZXNzXVwiKVxuICAgICAgICAgICAgICAgICAgICAgICAgLnJlbW92ZUNsYXNzKFwiYmctcHJpbWFyeSBiZy1zZWNvbmRhcnlcIilcbiAgICAgICAgICAgICAgICAgICAgICAgIC5hZGRDbGFzcyhcImJnLWRhbmdlciBwcm9ncmVzcy1iYXItZGFuZ2VyXCIpO1xuICAgICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICApO1xuXG4gICAgICAgICAgICBpbmZvLnVwbG9hZGVyLmFkZEV2ZW50TGlzdGVuZXIoXG4gICAgICAgICAgICAgICAgXCJwcm9ncmVzc1wiLFxuICAgICAgICAgICAgICAgICh7IGRldGFpbDogeyBsb2FkZWQsIHRvdGFsIH0gfTogQ3VzdG9tRXZlbnQpID0+XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuc2V0V2lkZ2V0Q29tcGxldGlvbih3aWRnZXQsIGxvYWRlZCwgdG90YWwpLFxuICAgICAgICAgICAgKTtcbiAgICAgICAgICAgIGluZm8udXBsb2FkZXIuYWRkRXZlbnRMaXN0ZW5lcihcbiAgICAgICAgICAgICAgICBcImZpbmlzaFwiLFxuICAgICAgICAgICAgICAgICh7IGRldGFpbDogeyBmaWxlLCByZXN1bHQgfSB9OiBDdXN0b21FdmVudCkgPT4ge1xuICAgICAgICAgICAgICAgICAgICB0aGlzLnRvZ2dsZUFuaW1hdGlvbih3aWRnZXQsIGZhbHNlKTtcbiAgICAgICAgICAgICAgICAgICAgd2lkZ2V0XG4gICAgICAgICAgICAgICAgICAgICAgICAuZmluZChcIltkYXRhLXVwbG9hZC1wcm9ncmVzc11cIilcbiAgICAgICAgICAgICAgICAgICAgICAgIC5yZW1vdmVDbGFzcyhcImJnLXByaW1hcnkgYmctc2Vjb25kYXJ5XCIpXG4gICAgICAgICAgICAgICAgICAgICAgICAuYWRkQ2xhc3MoXCJiZy1zdWNjZXNzIHByb2dyZXNzLWJhci1zdWNjZXNzXCIpO1xuICAgICAgICAgICAgICAgICAgICB0aGlzLnNhbmRib3gucHVibGlzaChcbiAgICAgICAgICAgICAgICAgICAgICAgIGNrYW4uQ0tBTkVYVF9GSUxFUy50b3BpY3MucXVldWVJdGVtVXBsb2FkZWQsXG4gICAgICAgICAgICAgICAgICAgICAgICBmaWxlLFxuICAgICAgICAgICAgICAgICAgICAgICAgcmVzdWx0LFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICApO1xuXG4gICAgICAgICAgICB0aGlzLnNldFdpZGdldE5hbWUod2lkZ2V0LCBpbmZvLmZpbGUubmFtZSk7XG4gICAgICAgICAgICB0aGlzLnNldFdpZGdldENvbXBsZXRpb24od2lkZ2V0LCBpbmZvLnVwbG9hZGVkLCBpbmZvLmZpbGUuc2l6ZSk7XG5cbiAgICAgICAgICAgIGlmIChvcHRpb25zLmltbWVkaWF0ZSkge1xuICAgICAgICAgICAgICAgIHdpZGdldC5maW5kKFwiW2RhdGEtdXBsb2FkLXJlc3VtZV1cIikudHJpZ2dlcihcImNsaWNrXCIpO1xuICAgICAgICAgICAgfVxuICAgICAgICB9LFxuXG4gICAgICAgIHNldFdpZGdldE5hbWUod2lkZ2V0OiBKUXVlcnksIG5hbWU6IHN0cmluZykge1xuICAgICAgICAgICAgd2lkZ2V0LmZpbmQoXCJbZGF0YS1pdGVtLW5hbWVdXCIpLnRleHQobmFtZSk7XG4gICAgICAgIH0sXG5cbiAgICAgICAgc2V0V2lkZ2V0Q29tcGxldGlvbih3aWRnZXQ6IEpRdWVyeSwgdXBsb2FkZWQ6IG51bWJlciwgdG90YWw6IG51bWJlcikge1xuICAgICAgICAgICAgY29uc3QgdmFsdWUgPSAodXBsb2FkZWQgKiAxMDApIC8gdG90YWw7XG4gICAgICAgICAgICBjb25zdCBpbmZvID0gdGhpcy53aWRnZXRzLmdldCh3aWRnZXRbMF0pO1xuICAgICAgICAgICAgaW5mby51cGxvYWRlZCA9IHVwbG9hZGVkO1xuXG4gICAgICAgICAgICBjb25zdCBjb21wbGV0aW9uID0gdmFsdWUudG9GaXhlZCgwKSArIFwiJVwiO1xuICAgICAgICAgICAgd2lkZ2V0XG4gICAgICAgICAgICAgICAgLmZpbmQoXCJbZGF0YS11cGxvYWQtcHJvZ3Jlc3NdXCIpXG4gICAgICAgICAgICAgICAgLnRleHQoY29tcGxldGlvbilcbiAgICAgICAgICAgICAgICAuY3NzKFwid2lkdGhcIiwgY29tcGxldGlvbik7XG4gICAgICAgIH0sXG5cbiAgICAgICAgdG9nZ2xlQW5pbWF0aW9uKHdpZGdldDogSlF1ZXJ5LCBzdGF0ZTogYm9vbGVhbikge1xuICAgICAgICAgICAgd2lkZ2V0XG4gICAgICAgICAgICAgICAgLmZpbmQoXCJbZGF0YS11cGxvYWQtcHJvZ3Jlc3NdXCIpXG4gICAgICAgICAgICAgICAgLnRvZ2dsZUNsYXNzKFwicHJvZ3Jlc3MtYmFyLWFuaW1hdGVkIGFjdGl2ZVwiLCBzdGF0ZSk7XG4gICAgICAgIH0sXG5cbiAgICAgICAgX29uV2lkZ2V0UmVzdW1lKGV2ZW50OiBKUXVlcnkuVHJpZ2dlcmVkRXZlbnQpIHtcbiAgICAgICAgICAgIGNvbnN0IGluZm8gPSB0aGlzLndpZGdldHMuZ2V0KGV2ZW50LmRlbGVnYXRlVGFyZ2V0KTtcbiAgICAgICAgICAgIGlmIChpbmZvLnVwbG9hZGVkID49IGluZm8udG90YWwpIHJldHVybjtcblxuICAgICAgICAgICAgY29uc3Qgd2lkZ2V0ID0gJChldmVudC5kZWxlZ2F0ZVRhcmdldCk7XG4gICAgICAgICAgICB3aWRnZXRcbiAgICAgICAgICAgICAgICAuZmluZChcIltkYXRhLXVwbG9hZC1wcm9ncmVzc11cIilcbiAgICAgICAgICAgICAgICAucmVtb3ZlQ2xhc3MoXCJiZy1zZWNvbmRhcnlcIilcbiAgICAgICAgICAgICAgICAuYWRkQ2xhc3MoXCJiZy1wcmltYXJ5XCIpO1xuXG4gICAgICAgICAgICBpZiAoaW5mby5pZCkge1xuICAgICAgICAgICAgICAgIGluZm8udXBsb2FkZXIucmVzdW1lKGluZm8uZmlsZSwgaW5mby5pZCk7XG4gICAgICAgICAgICB9IGVsc2Uge1xuICAgICAgICAgICAgICAgIGluZm8udXBsb2FkZXIudXBsb2FkKGluZm8uZmlsZSk7XG4gICAgICAgICAgICB9XG5cbiAgICAgICAgICAgIHRoaXMudG9nZ2xlQW5pbWF0aW9uKHdpZGdldCwgdHJ1ZSk7XG4gICAgICAgIH0sXG5cbiAgICAgICAgX29uV2lkZ2V0UGF1c2UoZXZlbnQ6IEpRdWVyeS5UcmlnZ2VyZWRFdmVudCkge1xuICAgICAgICAgICAgY29uc3QgaW5mbyA9IHRoaXMud2lkZ2V0cy5nZXQoZXZlbnQuZGVsZWdhdGVUYXJnZXQpO1xuICAgICAgICAgICAgaWYgKGluZm8udXBsb2FkZWQgPj0gaW5mby50b3RhbCkgcmV0dXJuO1xuXG4gICAgICAgICAgICBjb25zdCB3aWRnZXQgPSAkKGV2ZW50LmRlbGVnYXRlVGFyZ2V0KTtcbiAgICAgICAgICAgIHdpZGdldFxuICAgICAgICAgICAgICAgIC5maW5kKFwiW2RhdGEtdXBsb2FkLXByb2dyZXNzXVwiKVxuICAgICAgICAgICAgICAgIC5yZW1vdmVDbGFzcyhcImJnLXByaW1hcnlcIilcbiAgICAgICAgICAgICAgICAuYWRkQ2xhc3MoXCJiZy1zZWNvbmRhcnlcIik7XG5cbiAgICAgICAgICAgIGluZm8udXBsb2FkZXIucGF1c2UoaW5mby5maWxlKTtcbiAgICAgICAgICAgIHRoaXMudG9nZ2xlQW5pbWF0aW9uKHdpZGdldCwgZmFsc2UpO1xuICAgICAgICB9LFxuICAgIH07XG59KTtcbiJdfQ==
```

### Comparing `ckanext_files-0.2.6/ckanext/files/assets/scripts/files--shared-uploader.js` & `ckanext_files-0.3.0/ckanext/files/assets/scripts/files--shared-uploader.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: ASCII text, with very long lines (698)*

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 000002a0: 4943 426a 6232 357a 6443 4277 6233 4a30  ICBjb25zdCBwb3J0
 000002b0: 4944 3067 5a58 5a6c 626e 5175 6347 3979  ID0gZXZlbnQucG9y
 000002c0: 6448 4e62 4d46 3163 6269 4167 4943 4277  dHNbMF1cbiAgICBw
 000002d0: 6233 4a30 4c6d 3975 6257 567a 6332 466e  b3J0Lm9ubWVzc2Fn
 000002e0: 5a53 4139 4943 686c 4f69 424e 5a58 4e7a  ZSA9IChlOiBNZXNz
 000002f0: 5957 646c 5258 5a6c 626e 5170 4944 302b  YWdlRXZlbnQpID0+
 00000300: 4948 7463 6269 4167 4943 4239 5847 3563  IHtcbiAgICB9XG5c
-00000310: 626e 3163 6269 4a64 6651 3d3d 0a         bn1cbiJdfQ==.
+00000310: 626e 3163 6269 4a64 6651 3d3d            bn1cbiJdfQ==
```

### Comparing `ckanext_files-0.2.6/ckanext/files/assets/scripts/files--shared.js` & `ckanext_files-0.3.0/ckanext/files/assets/scripts/files--shared.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -198,15 +198,24 @@
                         if (uploaded <= start) {
                             throw new Error("Uploaded size is reduced");
                         }
                         this.dispatchProgress(file, uploaded, file.size);
                         start = uploaded;
                     }
                     this.dispatchProgress(file, file.size, file.size);
-                    info = await this._completeUpload(info);
+                    try {
+                        info = await this._completeUpload(info);
+                    } catch (err) {
+                        if (typeof err === "string") {
+                            this.dispatchError(file, err);
+                        } else {
+                            this.dispatchFail(file, err);
+                        }
+                        return;
+                    }
                     this.dispatchFinish(file, info);
                 }
                 _initializeUpload(file) {
                     return new Promise((done, fail) => this.sandbox.client.call("POST", "files_upload_initialize", Object.assign({}, this.settings.initializePayload || {}, {
                         storage: this.settings.storage,
                         name: file.name,
                         size: file.size,
@@ -272,8 +281,8 @@
             Multipart.defaultSettings = {
                 chunkSize: 1024 * 1024 * 5
             };
             adapters.Multipart = Multipart;
         })(adapters = CKANEXT_FILES.adapters || (CKANEXT_FILES.adapters = {}));
     })(CKANEXT_FILES = ckan.CKANEXT_FILES || (ckan.CKANEXT_FILES = {}));
 })(ckan || (ckan = {}));
-//# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiZmlsZXMtLXNoYXJlZC5qcyIsInNvdXJjZVJvb3QiOiIiLCJzb3VyY2VzIjpbIi4uL3RzL2ZpbGVzLS1zaGFyZWQudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6IkFBQUEsSUFBVSxJQUFJLENBeVliO0FBellELFdBQVUsSUFBSTtJQUtWLElBQWlCLGFBQWEsQ0FtWTdCO0lBbllELFdBQWlCLGFBQWE7UUFNYixvQkFBTSxHQUFHO1lBQ2xCLGNBQWMsRUFBRSw4QkFBOEI7WUFDOUMsa0JBQWtCLEVBQUUsa0NBQWtDO1lBQ3RELGlCQUFpQixFQUFFLG1DQUFtQztTQUN6RCxDQUFDO1FBRVcsNkJBQWUsR0FBRztZQUMzQixPQUFPLEVBQUUsU0FBUztTQUNyQixDQUFDO1FBRUYsU0FBUyxNQUFNLENBQ1gsSUFBVSxFQUNWLFdBQTBCLFlBQVksQ0FBQyxVQUFVLENBQUM7WUFFbEQsT0FBTyxRQUFRLENBQUMsTUFBTSxDQUFDLElBQUksQ0FBQyxDQUFDO1FBQ2pDLENBQUM7UUFFRCxTQUFTLFlBQVksQ0FBQyxPQUFlLEVBQUUsR0FBRyxPQUFZO1lBQ2xELE1BQU0sT0FBTyxHQUE2QyxRQUFTLENBQy9ELE9BQU8sQ0FDVixDQUFDO1lBQ0YsSUFBSSxDQUFDLE9BQU8sRUFBRSxDQUFDO2dCQUNYLE1BQU0sSUFBSSxLQUFLLENBQUMsWUFBWSxPQUFPLG9CQUFvQixDQUFDLENBQUM7WUFDN0QsQ0FBQztZQUNELE9BQU8sSUFBSSxPQUFPLENBQUMsR0FBRyxPQUFPLENBQUMsQ0FBQztRQUNuQyxDQUFDO1FBRUQsSUFBSSxDQUFDLE9BQU8sQ0FBQyxNQUFNLENBQUMsRUFBRSxLQUFLLEVBQUUsRUFBRSxNQUFNLEVBQUUsWUFBWSxFQUFFLEVBQUUsQ0FBQyxDQUFDO1FBRXpELElBQWlCLFFBQVEsQ0ErVnhCO1FBL1ZELFdBQWlCLFFBQVE7WUFXckIsTUFBYSxJQUFLLFNBQVEsV0FBVztnQkFNakMsWUFBWSxRQUFRLEdBQUcsRUFBRTtvQkFDckIsS0FBSyxFQUFFLENBQUM7b0JB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Q0FBQyxPQUFPLENBQUMsTUFBTSxDQUFDLElBQUksQ0FDcEIsTUFBTSxFQUNOLHVCQUF1QixFQUN2QixNQUFNLENBQUMsTUFBTSxDQUNULEVBQUUsRUFDRixJQUFJLENBQUMsUUFBUSxDQUFDLGVBQWUsSUFBSSxFQUFFLEVBQ25DO3dCQUNJLEVBQUUsRUFBRSxJQUFJLENBQUMsRUFBRTtxQkFDZCxDQUNKLEVBQ0QsQ0FBQyxJQUFTLEVBQUUsRUFBRTt3QkFDVixJQUFJLENBQUMsSUFBSSxDQUFDLE1BQU0sQ0FBQyxDQUFDO29CQUN0QixDQUFDLEVBQ0QsQ0FBQyxJQUFTLEVBQUUsRUFBRTt3QkFDVixJQUFJLENBQ0EsT0FBTyxJQUFJLENBQUMsWUFBWSxLQUFLLFFBQVE7NEJBQ2pDLENBQUMsQ0FBQyxJQUFJLENBQUMsWUFBWTs0QkFDbkIsQ0FBQyxDQUFDLElBQUksQ0FBQyxZQUFZLENBQUMsS0FBSyxDQUNoQyxDQUFDO29CQUNOLENBQUMsQ0FDSixDQUNKLENBQUM7Z0JBQ04sQ0FBQzs7WUE5TU0seUJBQWUsR0FBRyxFQUFFLFNBQVMsRUFBRSxJQUFJLEdBQUcsSUFBSSxHQUFHLENBQUMsRUFBRSxBQUFqQyxDQUFrQztZQUQvQyxrQkFBUyxZQWdOckIsQ0FBQTtRQUNMLENBQUMsRUEvVmdCLFFBQVEsR0FBUixzQkFBUSxLQUFSLHNCQUFRLFFBK1Z4QjtJQUNMLENBQUMsRUFuWWdCLGFBQWEsR0FBYixrQkFBYSxLQUFiLGtCQUFhLFFBbVk3QjtBQUNMLENBQUMsRUF6WVMsSUFBSSxLQUFKLElBQUksUUF5WWIiLCJzb3VyY2VzQ29udGVudCI6WyJuYW1lc3BhY2UgY2thbiB7XG4gICAgZXhwb3J0IHZhciBzYW5kYm94OiBhbnk7XG4gICAgZXhwb3J0IHZhciBwdWJzdWI6IGFueTtcbiAgICBleHBvcnQgdmFyIG1vZHVsZTogKG5hbWU6IHN0cmluZywgaW5pdGlhbGl6ZXI6ICgkOiBhbnkpID0+IGFueSkgPT4gYW55O1xuXG4gICAgZXhwb3J0IG5hbWVzcGFjZSBDS0FORVhUX0ZJTEVTIHtcbiAgICAgICAgdHlwZSBVcGxvYWRlclNldHRpbmdzID0ge1xuICAgICAgICAgICAgc3RvcmFnZTogc3RyaW5nO1xuICAgICAgICAgICAgW2tleTogc3RyaW5nXTogYW55O1xuICAgICAgICB9O1xuXG4gICAgICAgIGV4cG9ydCBjb25zdCB0b3BpY3MgPSB7XG4gICAgICAgICAgICBhZGRGaWxlVG9RdWV1ZTogXCJja2FuZXh0OmZpbGVzOnF1ZXVlOmZpbGU6YWRkXCIsXG4gICAgICAgICAgICByZXN0b3JlRmlsZUluUXVldWU6IFwiY2thbmV4dDpmaWxlczpxdWV1ZTpmaWxlOnJlc3RvcmVcIixcbiAgICAgICAgICAgIHF1ZXVlSXRlbVVwbG9hZGVkOiBcImNrYW5leHQ6ZmlsZXM6cXVldWU6ZmlsZTp1cGxvYWRlZFwiLFxuICAgICAgICB9O1xuXG4gICAgICAgIGV4cG9ydCBjb25zdCBkZWZhdWx0U2V0dGluZ3MgPSB7XG4gICAgICAgICAgICBzdG9yYWdlOiBcImRlZmF1bHRcIixcbiAgICAgICAgfTtcblxuICAgICAgICBmdW5jdGlvbiB1cGxvYWQoXG4gICAgICAgICAgICBmaWxlOiBGaWxlLFxuICAgICAgICAgICAgdXBsb2FkZXI6IGFkYXB0ZXJzLkJhc2UgPSBtYWtlVXBsb2FkZXIoXCJTdGFuZGFyZFwiKSxcbiAgICAgICAgKSB7XG4gICAgICAgICAgICByZXR1cm4gdXBsb2FkZXIudXBsb2FkKGZpbGUpO1xuICAgICAgICB9XG5cbiAgICAgICAgZnVuY3Rpb24gbWFrZVVwbG9hZGVyKGFkYXB0ZXI6IHN0cmluZywgLi4ub3B0aW9uczogYW55KSB7XG4gICAgICAgICAgICBjb25zdCBmYWN0b3J5ID0gKDx7IFtrZXk6IHN0cmluZ106IHR5cGVvZiBhZGFwdGVycy5CYXNlIH0+YWRhcHRlcnMpW1xuICAgICAgICAgICAgICAgIGFkYXB0ZXJcbiAgICAgICAgICAgIF07XG4gICAgICAgICAgICBpZiAoIWZhY3RvcnkpIHtcbiAgICAgICAgICAgICAgICB0aHJvdyBuZXcgRXJyb3IoYFVwbG9hZGVyICR7YWRhcHRlcn0gaXMgbm90IHJlZ2lzdGVyZWRgKTtcbiAgICAgICAgICAgIH1cbiAgICAgICAgICAgIHJldHVybiBuZXcgZmFjdG9yeSguLi5vcHRpb25zKTtcbiAgICAgICAgfVxuXG4gICAgICAgIGNrYW4uc2FuZGJveC5leHRlbmQoeyBmaWxlczogeyB1cGxvYWQsIG1ha2VVcGxvYWRlciB9IH0pO1xuXG4gICAgICAgIGV4cG9ydCBuYW1lc3BhY2UgYWRhcHRlcnMge1xuICAgICAgICAgICAgZXhwb3J0IHR5cGUgU3RvcmFnZURhdGEgPSB7XG4gICAgICAgICAgICAgICAgdXBsb2FkZWQ6IG51bWJlcjtcbiAgICAgICAgICAgICAgICBzaXplOiBudW1iZXI7XG4gICAgICAgICAgICB9O1xuXG4gICAgICAgICAgICBleHBvcnQgdHlwZSBVcGxvYWRJbmZvID0ge1xuICAgICAgICAgICAgICAgIGlkOiBzdHJpbmc7XG4gICAgICAgICAgICAgICAgc3RvcmFnZV9kYXRhOiBTdG9yYWdlRGF0YTtcbiAgICAgICAgICAgIH07XG5cbiAgICAgICAgICAgIGV4cG9ydCBjbGFzcyBCYXNlIGV4dGVuZHMgRXZlbnRUYXJnZXQge1xuICAgICAgICAgICAgICAgIHN0YXRpYyBkZWZhdWx0U2V0dGluZ3M6IE9iamVjdCA9IHt9O1xuICAgICAgICAgICAgICAgIHByb3RlY3RlZCBzZXR0aW5nczogVXBsb2FkZXJTZXR0aW5ncztcbiAgICAgICAgICAgICAgICBwcm90ZWN0ZWQgc2FuZGJveDogYW55O1xuICAgICAgICAgICAgICAgIHByb3RlY3RlZCBjc3JmVG9rZW46IHN0cmluZztcblxuICAgICAgICAgICAgICAgIGNvbnN0cnVjdG9yKHNldHRpbmdzID0ge30pIHtcbiAgICAgICAgICAgICAgICAgICAgc3VwZXIoKTtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5zZXR0aW5ncyA9IHtcbiAgICAgICAgICAgICAgICAgICAgICAgIC4uLmRlZmF1bHRTZXR0aW5ncyxcbiAgICAgICAgICAgICAgICAgICAgICAgIC4uLih0aGlzLmNvbnN0cnVjdG9yIGFzIHR5cGVvZiBCYXNlKS5kZWZhdWx0U2V0dGluZ3MsXG4gICAgICAgICAgICAgICAgICAgICAgICAuLi5zZXR0aW5ncyxcbiAgICAgICAgICAgICAgICAgICAgfTtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94ID0gY2thbi5zYW5kYm94KCk7XG5cbiAgICAgICAgICAgICAgICAgICAgY29uc3QgY3NyZkZpZWxkID1cbiAgICAgICAgICAgICAgICAgICAgICAgIGRvY3VtZW50XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgLnF1ZXJ5U2VsZWN0b3IoXCJtZXRhW25hbWU9Y3NyZl9maWVsZF9uYW1lXVwiKVxuICAgICAgICAgICAgICAgICAgICAgICAgICAgID8uZ2V0QXR0cmlidXRlKFwiY29udGVudFwiKSA/PyBcIl9jc3JmX3Rva2VuXCI7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuY3NyZlRva2VuID1cbiAgICAgICAgICAgICAgICAgICAgICAgIGRvY3VtZW50XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgLnF1ZXJ5U2VsZWN0b3IoYG1ldGFbbmFtZT0ke2NzcmZGaWVsZH1dYClcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICA/LmdldEF0dHJpYnV0ZShcImNvbnRlbnRcIikgfHwgXCJcIjtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICB1cGxvYWQoZmlsZTogRmlsZSkge1xuICAgICAgICAgICAgICAgICAgICB0aHJvdyBuZXcgRXJyb3IoXCJCYXNlLnVwbG9hZCBpcyBub3QgaW1wbGVtZW50ZWRcIik7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgcmVzdW1lKGZpbGU6IEZpbGUsIGlkOiBzdHJpbmcpIHtcbiAgICAgICAgICAgICAgICAgICAgdGhyb3cgbmV3IEVycm9yKFwiQmFzZS5yZXN1bWUgaXMgbm90IGltcGxlbWVudGVkXCIpO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIGRpc3BhdGNoU3RhcnQoZmlsZTogRmlsZSkge1xuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRXZlbnQoXG4gICAgICAgICAgICAgICAgICAgICAgICBuZXcgQ3VzdG9tRXZlbnQoXCJzdGFydFwiLCB7IGRldGFpbDogeyBmaWxlIH0gfSksXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgIGRpc3BhdGNoQ29tbWl0KGZpbGU6IEZpbGUsIGlkOiBzdHJpbmcpIHtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEV2ZW50KFxuICAgICAgICAgICAgICAgICAgICAgICAgbmV3IEN1c3RvbUV2ZW50KFwiY29tbWl0XCIsIHsgZGV0YWlsOiB7IGZpbGUsIGlkIH0gfSksXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgIGRpc3BhdGNoUHJvZ3Jlc3MoZmlsZTogRmlsZSwgbG9hZGVkOiBudW1iZXIsIHRvdGFsOiBudW1iZXIpIHtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEV2ZW50KFxuICAgICAgICAgICAgICAgICAgICAgICAgbmV3IEN1c3RvbUV2ZW50KFwicHJvZ3Jlc3NcIiwge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIGRldGFpbDogeyBmaWxlLCBsb2FkZWQsIHRvdGFsIH0sXG4gICAgICAgICAgICAgICAgICAgICAgICB9KSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgZGlzcGF0Y2hGaW5pc2goZmlsZTogRmlsZSwgcmVzdWx0OiBPYmplY3QpIHtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEV2ZW50KFxuICAgICAgICAgICAgICAgICAgICAgICAgbmV3IEN1c3RvbUV2ZW50KFwiZmluaXNoXCIsIHsgZGV0YWlsOiB7IGZpbGUsIHJlc3VsdCB9IH0pLFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICBkaXNwYXRjaEZhaWwoZmlsZTogRmlsZSwgcmVhc29uczogeyBba2V5OiBzdHJpbmddOiBzdHJpbmdbXSB9KSB7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hFdmVudChcbiAgICAgICAgICAgICAgICAgICAgICAgIG5ldyBDdXN0b21FdmVudChcImZhaWxcIiwgeyBkZXRhaWw6IHsgZmlsZSwgcmVhc29ucyB9IH0pLFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICBkaXNwYXRjaEVycm9yKGZpbGU6IEZpbGUsIG1lc3NhZ2U6IHN0cmluZykge1xuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRXZlbnQoXG4gICAgICAgICAgICAgICAgICAgICAgICBuZXcgQ3VzdG9tRXZlbnQoXCJlcnJvclwiLCB7IGRldGFpbDogeyBmaWxlLCBtZXNzYWdlIH0gfSksXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICBleHBvcnQgY2xhc3MgU3RhbmRhcmQgZXh0ZW5kcyBCYXNlIHtcbiAgICAgICAgICAgICAgICB1cGxvYWQoZmlsZTogRmlsZSkge1xuICAgICAgICAgICAgICAgICAgICBjb25zdCByZXF1ZXN0ID0gbmV3IFhNTEh0dHBSZXF1ZXN0KCk7XG4gICAgICAgICAgICAgICAgICAgIGNvbnN0IHByb21pc2UgPSB0aGlzLl9hZGRMaXN0ZW5lcnMocmVxdWVzdCwgZmlsZSk7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuX3ByZXBhcmVSZXF1ZXN0KHJlcXVlc3QsIGZpbGUpO1xuICAgICAgICAgICAgICAgICAgICB0aGlzLl9zZW5kUmVxdWVzdChyZXF1ZXN0LCBmaWxlKTtcbiAgICAgICAgICAgICAgICAgICAgcmV0dXJuIHByb21pc2U7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgX2FkZExpc3RlbmVycyhcbiAgICAgICAgICAgICAgICAgICAgcmVxdWVzdDogWE1MSHR0cFJlcXVlc3QsXG4gICAgICAgICAgICAgICAgICAgIGZpbGU6IEZpbGUsXG4gICAgICAgICAgICAgICAgKTogUHJvbWlzZTxVcGxvYWRJbmZvPiB7XG4gICAgICAgICAgICAgICAgICAgIHJlcXVlc3QudXBsb2FkLmFkZEV2ZW50TGlzdGVuZXIoXCJsb2Fkc3RhcnRcIiwgKGV2ZW50KSA9PlxuICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaFN0YXJ0KGZpbGUpLFxuICAgICAgICAgICAgICAgICAgICApO1xuXG4gICAgICAgICAgICAgICAgICAgIHJlcXVlc3QudXBsb2FkLmFkZEV2ZW50TGlzdGVuZXIoXCJwcm9ncmVzc1wiLCAoZXZlbnQpID0+XG4gICAgICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoUHJvZ3Jlc3MoZmlsZSwgZXZlbnQubG9hZGVkLCBldmVudC50b3RhbCksXG4gICAgICAgICAgICAgICAgICAgICk7XG5cbiAgICAgICAgICAgICAgICAgICAgcmV0dXJuIG5ldyBQcm9taXNlKChkb25lLCBmYWlsKSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LmFkZEV2ZW50TGlzdGVuZXIoXCJsb2FkXCIsIChldmVudCkgPT4ge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIGNvbnN0IHJlc3VsdCA9IEpTT04ucGFyc2UocmVxdWVzdC5yZXNwb25zZVRleHQpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIGlmIChyZXN1bHQuc3VjY2Vzcykge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoQ29tbWl0KGZpbGUsIHJlc3VsdC5yZXN1bHQuaWQpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRmluaXNoKGZpbGUsIHJlc3VsdC5yZXN1bHQpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBkb25lKHJlc3VsdC5yZXN1bHQpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIH0gZWxzZSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hGYWlsKGZpbGUsIHJlc3VsdC5lcnJvcik7XG5cbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZmFpbChyZXN1bHQuZXJyb3IpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICAgICAgICAgIH0pO1xuXG4gICAgICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LmFkZEV2ZW50TGlzdGVuZXIoXCJlcnJvclwiLCAoZXZlbnQpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRXJyb3IoZmlsZSwgcmVxdWVzdC5yZXNwb25zZVRleHQpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIGZhaWwocmVxdWVzdC5yZXNwb25zZVRleHQpO1xuICAgICAgICAgICAgICAgICAgICAgICAgfSk7XG4gICAgICAgICAgICAgICAgICAgIH0pO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIF9wcmVwYXJlUmVxdWVzdChyZXF1ZXN0OiBYTUxIdHRwUmVxdWVzdCwgZmlsZTogRmlsZSkge1xuICAgICAgICAgICAgICAgICAgICByZXF1ZXN0Lm9wZW4oXG4gICAgICAgICAgICAgICAgICAgICAgICBcIlBPU1RcIixcbiAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5jbGllbnQudXJsKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiL2FwaS9hY3Rpb24vZmlsZXNfZmlsZV9jcmVhdGVcIixcbiAgICAgICAgICAgICAgICAgICAgICAgICksXG4gICAgICAgICAgICAgICAgICAgICk7XG5cbiAgICAgICAgICAgICAgICAgICAgaWYgKHRoaXMuY3NyZlRva2VuKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LnNldFJlcXVlc3RIZWFkZXIoXCJYLUNTUkZUb2tlblwiLCB0aGlzLmNzcmZUb2tlbik7XG4gICAgICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBfc2VuZFJlcXVlc3QocmVxdWVzdDogWE1MSHR0cFJlcXVlc3QsIGZpbGU6IEZpbGUpIHtcbiAgICAgICAgICAgICAgICAgICAgY29uc3QgZGF0YSA9IG5ldyBGb3JtRGF0YSgpO1xuICAgICAgICAgICAgICAgICAgICBkYXRhLmFwcGVuZChcInVwbG9hZFwiLCBmaWxlKTtcblxuICAgICAgICAgICAgICAgICAgICBkYXRhLmFwcGVuZChcInN0b3JhZ2VcIiwgdGhpcy5zZXR0aW5ncy5zdG9yYWdlKTtcbiAgICAgICAgICAgICAgICAgICAgcmVxdWVzdC5zZW5kKGRhdGEpO1xuICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgZXhwb3J0IGNsYXNzIE11bHRpcGFydCBleHRlbmRzIEJhc2Uge1xuICAgICAgICAgICAgICAgIHN0YXRpYyBkZWZhdWx0U2V0dGluZ3MgPSB7IGNodW5rU2l6ZTogMTAyNCAqIDEwMjQgKiA1IH07XG5cbiAgICAgICAgICAgICAgICBwcml2YXRlIF9hY3RpdmUgPSBuZXcgU2V0PEZpbGU+KCk7XG5cbiAgICAgICAgICAgICAgICBjb25zdHJ1Y3RvcihzZXR0aW5nczogT2JqZWN0KSB7XG4gICAgICAgICAgICAgICAgICAgIHN1cGVyKHNldHRpbmdzKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBhc3luYyB1cGxvYWQoZmlsZTogRmlsZSkge1xuICAgICAgICAgICAgICAgICAgICBpZiAodGhpcy5fYWN0aXZlLmhhcyhmaWxlKSkge1xuICAgICAgICAgICAgICAgICAgICAgICAgY29uc29sZS53YXJuKFwiRmlsZSB1cGxvYWQgaW4gcHJvZ3Jlc3NcIik7XG4gICAgICAgICAgICAgICAgICAgICAgICByZXR1cm47XG4gICAgICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICAgICAgdGhpcy5fYWN0aXZlLmFkZChmaWxlKTtcblxuICAgICAgICAgICAgICAgICAgICBsZXQgaW5mbztcblxuICAgICAgICAgICAgICAgICAgICB0cnkge1xuICAgICAgICAgICAgICAgICAgICAgICAgaW5mbyA9IGF3YWl0IHRoaXMuX2luaXRpYWxpemVVcGxvYWQoZmlsZSk7XG4gICAgICAgICAgICAgICAgICAgIH0gY2F0Y2ggKGVycikge1xuICAgICAgICAgICAgICAgICAgICAgICAgaWYgKHR5cGVvZiBlcnIgPT09IFwic3RyaW5nXCIpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRXJyb3IoZmlsZSwgZXJyKTtcbiAgICAgICAgICAgICAgICAgICAgICAgIH0gZWxzZSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEZhaWwoZmlsZSwgZXJyIGFzIGFueSk7XG4gICAgICAgICAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgICAgICAgICByZXR1cm47XG4gICAgICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoQ29tbWl0KGZpbGUsIGluZm8uaWQpO1xuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoU3RhcnQoZmlsZSk7XG5cbiAgICAgICAgICAgICAgICAgICAgdGhpcy5fZG9VcGxvYWQoZmlsZSwgaW5mbyk7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgYXN5bmMgcmVzdW1lKGZpbGU6IEZpbGUsIGlkOiBzdHJpbmcpIHtcbiAgICAgICAgICAgICAgICAgICAgaWYgKHRoaXMuX2FjdGl2ZS5oYXMoZmlsZSkpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgIGNvbnNvbGUud2FybihcIkZpbGUgdXBsb2FkIGluIHByb2dyZXNzXCIpO1xuICAgICAgICAgICAgICAgICAgICAgICAgcmV0dXJuO1xuICAgICAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuX2FjdGl2ZS5hZGQoZmlsZSk7XG5cbiAgICAgICAgICAgICAgICAgICAgbGV0IGluZm8gPSBhd2FpdCB0aGlzLl9zaG93VXBsb2FkKGlkKTtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaFN0YXJ0KGZpbGUpO1xuXG4gICAgICAgICAgICAgICAgICAgIHRoaXMuX2RvVXBsb2FkKGZpbGUsIGluZm8pO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIHBhdXNlKGZpbGU6IEZpbGUpIHtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5fYWN0aXZlLmRlbGV0ZShmaWxlKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBhc3luYyBfZG9VcGxvYWQoZmlsZTogRmlsZSwgaW5mbzogVXBsb2FkSW5mbykge1xuICAgICAgICAgICAgICAgICAgICBsZXQgc3RhcnQgPSBpbmZvLnN0b3JhZ2VfZGF0YS51cGxvYWRlZCB8fCAwO1xuXG4gICAgICAgICAgICAgICAgICAgIHdoaWxlIChzdGFydCA8IGZpbGUuc2l6ZSkge1xuICAgICAgICAgICAgICAgICAgICAgICAgaWYgKCF0aGlzLl9hY3RpdmUuaGFzKGZpbGUpKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgY29uc29sZS5pbmZvKFwiRmlsZSB1cGxvYWQgaXMgcGF1c2VkXCIpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIHJldHVybjtcbiAgICAgICAgICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgICAgICAgICAgaW5mbyA9IGF3YWl0IHRoaXMuX3VwbG9hZENodW5rKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIGluZm8sXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgZmlsZS5zbGljZShzdGFydCwgc3RhcnQgKyB0aGlzLnNldHRpbmdzLmNodW5rU2l6ZSksXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgc3RhcnQsXG4gICAgICAgICAgICAgICAgICAgICAgICApO1xuXG4gICAgICAgICAgICAgICAgICAgICAgICBjb25zdCB1cGxvYWRlZCA9IGluZm8uc3RvcmFnZV9kYXRhLnVwbG9hZGVkO1xuICAgICAgICAgICAgICAgICAgICAgICAgaWYgKHVwbG9hZGVkIDw9IHN0YXJ0KSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhyb3cgbmV3IEVycm9yKFwiVXBsb2FkZWQgc2l6ZSBpcyByZWR1Y2VkXCIpO1xuICAgICAgICAgICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoUHJvZ3Jlc3MoZmlsZSwgdXBsb2FkZWQsIGZpbGUuc2l6ZSk7XG4gICAgICAgICAgICAgICAgICAgICAgICBzdGFydCA9IHVwbG9hZGVkO1xuICAgICAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaFByb2dyZXNzKGZpbGUsIGZpbGUuc2l6ZSwgZmlsZS5zaXplKTtcbiAgICAgICAgICAgICAgICAgICAgaW5mbyA9IGF3YWl0IHRoaXMuX2NvbXBsZXRlVXBsb2FkKGluZm8pO1xuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRmluaXNoKGZpbGUsIGluZm8pO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIF9pbml0aWFsaXplVXBsb2FkKGZpbGU6IEZpbGUpOiBQcm9taXNlPFVwbG9hZEluZm8+IHtcbiAgICAgICAgICAgICAgICAgICAgcmV0dXJuIG5ldyBQcm9taXNlKChkb25lLCBmYWlsKSA9PlxuICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94LmNsaWVudC5jYWxsKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiUE9TVFwiLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiZmlsZXNfdXBsb2FkX2luaXRpYWxpemVcIixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBPYmplY3QuYXNzaWduKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB7fSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5zZXR0aW5ncy5pbml0aWFsaXplUGF5bG9hZCB8fCB7fSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgc3RvcmFnZTogdGhpcy5zZXR0aW5ncy5zdG9yYWdlLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgbmFtZTogZmlsZS5uYW1lLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgc2l6ZTogZmlsZS5zaXplLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICksXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgKGRhdGE6IGFueSkgPT4ge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBkb25lKGRhdGEucmVzdWx0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIChyZXNwOiBhbnkpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZmFpbChcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHR5cGVvZiByZXNwLnJlc3BvbnNlSlNPTiA9PT0gXCJzdHJpbmdcIlxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgID8gcmVzcC5yZXNwb25zZVRleHRcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICA6IHJlc3AucmVzcG9uc2VKU09OLmVycm9yLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICAgICAgICAgICAgICApLFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIF9zaG93VXBsb2FkKGlkOiBzdHJpbmcpOiBQcm9taXNlPFVwbG9hZEluZm8+IHtcbiAgICAgICAgICAgICAgICAgICAgcmV0dXJuIG5ldyBQcm9taXNlKChkb25lLCBmYWlsKSA9PlxuICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94LmNsaWVudC5jYWxsKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiR0VUXCIsXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgXCJmaWxlc191cGxvYWRfc2hvd1wiLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIGA/aWQ9JHtpZH1gLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIChkYXRhOiBhbnkpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZG9uZShkYXRhLnJlc3VsdCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAocmVzcDogYW55KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGZhaWwoXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB0eXBlb2YgcmVzcC5yZXNwb25zZUpTT04gPT09IFwic3RyaW5nXCJcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICA/IHJlc3AucmVzcG9uc2VUZXh0XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgOiByZXNwLnJlc3BvbnNlSlNPTi5lcnJvcixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgKSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBfdXBsb2FkQ2h1bmsoXG4gICAgICAgICAgICAgICAgICAgIGluZm86IFVwbG9hZEluZm8sXG4gICAgICAgICAgICAgICAgICAgIHBhcnQ6IEJsb2IsXG4gICAgICAgICAgICAgICAgICAgIHN0YXJ0OiBudW1iZXIsXG4gICAgICAgICAgICAgICAgKTogUHJvbWlzZTxVcGxvYWRJbmZvPiB7XG4gICAgICAgICAgICAgICAgICAgIGlmICghcGFydC5zaXplKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICB0aHJvdyBuZXcgRXJyb3IoXCIwLWxlbmd0aCBjaHVua3MgYXJlIG5vdCBhbGxvd2VkXCIpO1xuICAgICAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgICAgIGNvbnN0IHJlcXVlc3QgPSBuZXcgWE1MSHR0cFJlcXVlc3QoKTtcblxuICAgICAgICAgICAgICAgICAgICBjb25zdCByZXN1bHQgPSBuZXcgUHJvbWlzZTxVcGxvYWRJbmZvPigoZG9uZSwgZmFpbCkgPT4ge1xuICAgICAgICAgICAgICAgICAgICAgICAgcmVxdWVzdC5hZGRFdmVudExpc3RlbmVyKFwibG9hZFwiLCAoZXZlbnQpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBjb25zdCByZXN1bHQgPSBKU09OLnBhcnNlKHJlcXVlc3QucmVzcG9uc2VUZXh0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBpZiAocmVzdWx0LnN1Y2Nlc3MpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZG9uZShyZXN1bHQucmVzdWx0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9IGVsc2Uge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBmYWlsKHJlc3VsdC5lcnJvcik7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgICAgICAgICAgfSk7XG5cbiAgICAgICAgICAgICAgICAgICAgICAgIHJlcXVlc3QuYWRkRXZlbnRMaXN0ZW5lcihcImVycm9yXCIsIChldmVudCkgPT5cbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBmYWlsKHJlcXVlc3QucmVzcG9uc2VUZXh0KSxcbiAgICAgICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgICAgIH0pO1xuXG4gICAgICAgICAgICAgICAgICAgIHJlcXVlc3Qub3BlbihcbiAgICAgICAgICAgICAgICAgICAgICAgIFwiUE9TVFwiLFxuICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94LmNsaWVudC51cmwoXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgXCIvYXBpL2FjdGlvbi9maWxlc191cGxvYWRfdXBkYXRlXCIsXG4gICAgICAgICAgICAgICAgICAgICAgICApLFxuICAgICAgICAgICAgICAgICAgICApO1xuXG4gICAgICAgICAgICAgICAgICAgIGlmICh0aGlzLmNzcmZUb2tlbikge1xuICAgICAgICAgICAgICAgICAgICAgICAgcmVxdWVzdC5zZXRSZXF1ZXN0SGVhZGVyKFwiWC1DU1JGVG9rZW5cIiwgdGhpcy5jc3JmVG9rZW4pO1xuICAgICAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICAgICAgdGhpcy5fc2VuZFJlcXVlc3QocmVxdWVzdCwgcGFydCwgc3RhcnQsIGluZm8uaWQpO1xuXG4gICAgICAgICAgICAgICAgICAgIHJldHVybiByZXN1bHQ7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgX3NlbmRSZXF1ZXN0KFxuICAgICAgICAgICAgICAgICAgICByZXF1ZXN0OiBYTUxIdHRwUmVxdWVzdCxcbiAgICAgICAgICAgICAgICAgICAgcGFydDogQmxvYixcbiAgICAgICAgICAgICAgICAgICAgcG9zaXRpb246IG51bWJlcixcbiAgICAgICAgICAgICAgICAgICAgaWQ6IHN0cmluZyxcbiAgICAgICAgICAgICAgICApIHtcbiAgICAgICAgICAgICAgICAgICAgY29uc3QgZm9ybSA9IG5ldyBGb3JtRGF0YSgpO1xuICAgICAgICAgICAgICAgICAgICBmb3JtLmFwcGVuZChcInVwbG9hZFwiLCBwYXJ0KTtcbiAgICAgICAgICAgICAgICAgICAgZm9ybS5hcHBlbmQoXCJwb3NpdGlvblwiLCBTdHJpbmcocG9zaXRpb24pKTtcbiAgICAgICAgICAgICAgICAgICAgZm9ybS5hcHBlbmQoXCJpZFwiLCBpZCk7XG4gICAgICAgICAgICAgICAgICAgIHJlcXVlc3Quc2VuZChmb3JtKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBfY29tcGxldGVVcGxvYWQoaW5mbzogVXBsb2FkSW5mbyk6IFByb21pc2U8VXBsb2FkSW5mbz4ge1xuICAgICAgICAgICAgICAgICAgICByZXR1cm4gbmV3IFByb21pc2UoKGRvbmUsIGZhaWwpID0+XG4gICAgICAgICAgICAgICAgICAgICAgICB0aGlzLnNhbmRib3guY2xpZW50LmNhbGwoXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgXCJQT1NUXCIsXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgXCJmaWxlc191cGxvYWRfY29tcGxldGVcIixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBPYmplY3QuYXNzaWduKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB7fSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5zZXR0aW5ncy5jb21wbGV0ZVBheWxvYWQgfHwge30sXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGlkOiBpbmZvLmlkLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICksXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgKGRhdGE6IGFueSkgPT4ge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBkb25lKGRhdGEucmVzdWx0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIChyZXNwOiBhbnkpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZmFpbChcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHR5cGVvZiByZXNwLnJlc3BvbnNlSlNPTiA9PT0gXCJzdHJpbmdcIlxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgID8gcmVzcC5yZXNwb25zZVRleHRcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICA6IHJlc3AucmVzcG9uc2VKU09OLmVycm9yLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICAgICAgICAgICAgICApLFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgIH1cbiAgICAgICAgfVxuICAgIH1cbn1cbiJdfQ==
+//# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiZmlsZXMtLXNoYXJlZC5qcyIsInNvdXJjZVJvb3QiOiIiLCJzb3VyY2VzIjpbIi4uL3RzL2ZpbGVzLS1zaGFyZWQudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6IkFBQUEsSUFBVSxJQUFJLENBbVpiO0FBblpELFdBQVUsSUFBSTtJQUtWLElBQWlCLGFBQWEsQ0E2WTdCO0lBN1lELFdBQWlCLGFBQWE7UUFNYixvQkFBTSxHQUFHO1lBQ2xCLGNBQWMsRUFBRSw4QkFBOEI7WUFDOUMsa0JBQWtCLEVBQUUsa0NBQWtDO1lBQ3RELGlCQUFpQixFQUFFLG1DQUFtQztTQUN6RCxDQUFDO1FBRVcsNkJBQWUsR0FBRztZQUMzQixPQUFPLEVBQUUsU0FBUztTQUNyQixDQUFDO1FBRUYsU0FBUyxNQUFNLENBQ1gsSUFBVSxFQUNWLFdBQTBCLFlBQVksQ0FBQyxVQUFVLENBQUM7WUFFbEQsT0FBTyxRQUFRLENBQUMsTUFBTSxDQUFDLElBQUksQ0FBQyxDQUFDO1FBQ2pDLENBQUM7UUFFRCxTQUFTLFlBQVksQ0FBQyxPQUFlLEVBQUUsR0FBRyxPQUFZO1lBQ2xELE1BQU0sT0FBTyxHQUE2QyxRQUFTLENBQy9ELE9BQU8sQ0FDVixDQUFDO1lBQ0YsSUFBSSxDQUFDLE9BQU8sRUFBRSxDQUFDO2dCQUNYLE1BQU0sSUFBSSxLQUFLLENBQUMsWUFBWSxPQUFPLG9CQUFvQixDQUFDLENBQUM7WUFDN0QsQ0FBQztZQUNELE9BQU8sSUFBSSxPQUFPLENBQUMsR0FBRyxPQUFPLENBQUMsQ0FBQztRQUNuQyxDQUFDO1FBRUQsSUFBSSxDQUFDLE9BQU8sQ0FBQyxNQUFNLENBQUMsRUFBRSxLQUFLLEVBQUUsRUFBRSxNQUFNLEVBQUUsWUFBWSxFQUFFLEVBQUUsQ0FBQyxDQUFDO1FBRXpELElBQWlCLFFBQVEsQ0F5V3hCO1FBeldELFdBQWlCLFFBQVE7WUFXckIsTUFBYSxJQUFLLFNBQVEsV0FBVztnQkFNakMsWUFBWSxRQUFRLEdBQUcsRUFBRTtvQkFDckIsS0FBSyxFQUFFLENBQUM7b0JBQ1IsSUFBSSxDQUFDLFFBQVEsR0FBRzt3QkFDWixHQUFHLGNBQUEsZUFBZTt3QkFDbEIsR0FBSSxJQUFJLENBQUMsV0FBMkIsQ0FBQyxlQUFlO3dCQUNwRCxHQUFHLFFBQVE7cUJBQ2QsQ0FBQztvQkFDRixJQUFJLENBQUMsT0FBTyxHQUFHLElBQUksQ0FBQyxPQUFPLEVBQUUsQ0FBQztvQkFFOUIsTUFBTSxTQUFTLEdBQ1gsUUFBUTt5QkFDSCxhQUFhLENBQUMsNEJBQTRCLENBQUM7d0JBQzVDLEVBQUUsWUFBWSxDQUFDLFNBQVMsQ0FBQyxJQUFJLGFBQWEsQ0FBQztvQkFDbkQsSUFBSSxDQUFDLFNBQVM7d0JBQ1YsUUFBUTs2QkFDSCxhQUFhLENBQUMsYUFBYSxTQUFTLEdBQUcsQ0FBQzs0QkFDekMsRUFBRSxZQUFZLENBQUMsU0FBUyxDQUFDLElBQUksRUFBRSxDQUFDO2dCQUM1QyxDQUFDO2dCQUVELE1BQU0sQ0FBQyxJQUFVO29CQUNiLE1BQU0sSUFBSSxLQUFLLENBQUMsZ0NBQWdDLENBQUMsQ0FBQztnQkFDdEQsQ0FBQztnQkFFRCxNQUFNLENBQUMsSUFBVSxFQUFFLEVBQVU7b0JBQ3pCLE1BQU0sSUFBSSxLQUFLLENBQUMsZ0NBQWdDLENBQUMsQ0FBQztnQkFDdEQsQ0FBQztnQkFFRCxhQUFhLENBQUMsSUFBVTtvQkFDcEIsSUFBSSxDQUFDLGFBQWEsQ0FDZCxJQUFJLFdBQVcsQ0FBQyxPQUFPLEVBQUUsRUFBRSxNQUFNLEVBQUUsRUFBRSxJQUFJLEVBQUUsRUFBRSxDQUFDLENBQ2pELENBQUM7Z0JBQ04sQ0FBQztnQkFDRCxjQUFjLENBQUMsSUFBVSxFQUFFLEVBQVU7b0JBQ2pDLElBQUksQ0FBQyxhQUFhLENBQ2QsSUFBSSxXQUFXLENBQUMsUUFBUSxFQUFFLEVBQUUsTUFBTSxFQUFFLEVBQUUsSUFBSSxFQUFFLEVBQUUsRUFBRSxFQUFFLENBQUMsQ0FDdEQsQ0FBQztnQkFDTixDQUFDO2dCQUNELGdCQUFnQixDQUFDLElBQVUsRUFBRSxNQUFjLEVBQUUsS0FBYTtvQkFDdEQsSUFBSSxDQUFDLGFBQWEsQ0FDZCxJQUFJLFdBQVcsQ0FBQyxVQUFVLEVBQUU7d0JBQ3hCLE1BQU0sRUFBRSxFQUFFLElBQUksRUFBRSxNQUFNLEVBQUUsS0FBSyxFQUFFO3FCQUNsQyxDQUFDLENBQ0wsQ0FBQztnQkFDTixDQUFDO2dCQUNELGNBQWMsQ0FBQyxJQUFVLEVBQUUsTUFBYztvQkFDckMsSUFBSSxDQUFDLGFBQWEsQ0FDZCxJQUFJLFdBQVcsQ0FBQyxRQUFRLEVBQUUsRUFBRSxNQUFNLEVBQUUsRUFBRSxJQUFJLEVBQUUsTUFBTSxFQUFFLEVBQUUsQ0FBQyxDQUMxRCxDQUFDO2dCQUNOLENBQUM7Z0JBQ0QsWUFBWSxDQUFDLElBQVUsRUFBRSxPQUFvQztvQkFDekQsSUFBSSxDQUFDLGFBQWEsQ0FDZCxJQUFJLFdBQVcsQ0FBQyxNQUFNLEVBQUUsRUFBRSxNQUFNLEVBQUUsRUFBRSxJQUFJLEVBQUUsT0FBTyxFQUFFLEVBQUUsQ0FBQyxDQUN6RCxDQUFDO2dCQUNOLENBQUM7Z0JBQ0QsYUFBYSxDQUFDLElBQVUsRUFBRSxPQUFlO29CQUNyQyxJQUFJLENBQUMsYUFBYSxDQUNkLElBQUksV0FBVyxDQUFDLE9BQU8sRUFBRSxFQUFFLE1BQU0sRUFBRSxFQUFFLElBQUksRUFBRSxPQUFPLEVBQUUsRUFBRSxDQUFDLENBQzFELENBQUM7Z0JBQ04sQ0FBQzs7WUEvRE0sb0JBQWUsR0FBVyxFQUFFLENBQUM7WUFEM0IsYUFBSSxPQWlFaEIsQ0FBQTtZQUVELE1BQWEsUUFBUyxTQUFRLElBQUk7Z0JBQzlCLE1BQU0sQ0FBQyxJQUFVO29CQUNiLE1BQU0sT0FBTyxHQUFHLElBQUksY0FBYyxFQUFFLENBQUM7b0JBQ3JDLE1BQU0sT0FBTyxHQUFHLElBQUksQ0FBQyxhQUFhLENBQUMsT0FBTyxFQUFFLElBQUksQ0FBQyxDQUFDO29CQUNsRCxJQUFJLENBQUMsZUFBZSxDQUFDLE9BQU8sRUFBRSxJQUFJLENBQUMsQ0FBQztvQkFDcEMsSUFBSSxDQUFDLFlBQVksQ0FBQyxPQUFPLEVBQUUsSUFBSSxDQUFDLENBQUM7b0JBQ2pDLE9BQU8sT0FBTyxDQUFDO2dCQUNuQixDQUFDO2dCQUVELGFBQWEsQ0FDVCxPQUF1QixFQUN2QixJQUFVO29CQUVWLE9BQU8sQ0FBQyxNQUFNLENBQUMsZ0JBQWdCLENBQUMsV0FBVyxFQUFFLENBQUMsS0FBSyxFQUFFLEVBQUUsQ0FDbkQsSUFBSSxDQUFDLGFBQWEsQ0FBQyxJQUFJLENBQUMsQ0FDM0IsQ0FBQztvQkFFRixPQUFPLENBQUMsTUFBTSxDQUFDLGdCQUFnQixDQUFDLFVBQVUsRUFBRSxDQUFDLEtBQUssRUFBRSxFQUFFLENBQ2xELElBQUksQ0FBQyxnQkFBZ0IsQ0FBQyxJQUFJLEVBQUUsS0FBSyxDQUFDLE1BQU0sRUFBRSxLQUFLLENBQUMsS0FBSyxDQUFDLENBQ3pELENBQUM7b0JBRUYsT0FBTyxJQUFJLE9BQU8sQ0FBQyxDQUFDLElBQUksRUFBRSxJQUFJLEVBQUUsRUFBRTt3QkFDOUIsT0FBTyxDQUFDLGdCQUFnQixDQUFDLE1BQU0sRUFBRSxDQUFDLEtBQUssRUFBRSxFQUFFOzRCQUN2QyxNQUFNLE1BQU0sR0FBRyxJQUFJLENBQUMsS0FBSyxDQUFDLE9BQU8sQ0FBQyxZQUFZLENBQUMsQ0FBQzs0QkFDaEQsSUFBSSxNQUFNLENBQUMsT0FBTyxFQUFFLENBQUM7Z0NBQ2pCLElBQUksQ0FBQyxjQUFjLENBQUMsSUFBSSxFQUFFLE1BQU0sQ0FBQyxNQUFNLENBQUMsRUFBRSxDQUFDLENBQUM7Z0NBQzVDLElBQUksQ0FBQyxjQUFjLENBQUMsSUFBSSxFQUFFLE1BQU0sQ0FBQyxNQUFNLENBQUMsQ0FBQztnQ0FDekMsSUFBSSxDQUFDLE1BQU0sQ0FBQyxNQUFNLENBQUMsQ0FBQzs0QkFDeEIsQ0FBQztpQ0FBTSxDQUFDO2dDQUNKLElBQUksQ0FBQyxZQUFZLENBQUMsSUFBSSxFQUFFLE1BQU0sQ0FBQyxLQUFLLENBQUMsQ0FBQztnQ0FFdEMsSUFBSSxDQUFDLE1BQU0sQ0FBQyxLQUFLLENBQUMsQ0FBQzs0QkFDdkIsQ0FBQzt3QkFDTCxDQUFDLENBQUMsQ0FBQzt3QkFFSCxPQUFPLENBQUMsZ0JBQWdCLENBQUMsT0FBTyxFQUFFLENBQUMsS0FBSyxFQUFFLEVBQUU7NEJBQ3hDLElBQUksQ0FBQyxhQUFhLENBQUMsSUFBSSxFQUFFLE9BQU8sQ0FBQyxZQUFZLENBQUMsQ0FBQzs0QkFDL0MsSUFBSSxDQUFDLE9BQU8sQ0FBQyxZQUFZLENBQUMsQ0FBQzt3QkFDL0IsQ0FBQyxDQUFDLENBQUM7b0JBQ1AsQ0FBQyxDQUFDLENBQUM7Z0JBQ1AsQ0FBQztnQkFFRCxlQUFlLENBQUMsT0FBdUIsRUFBRSxJQUFVO29CQUMvQyxPQUFPLENBQUMsSUFBSSxDQUNSLE1BQU0sRUFDTixJQUFJLENBQUMsT0FBTyxDQUFDLE1BQU0sQ0FBQyxHQUFHLENBQ25CLCtCQUErQixDQUNsQyxDQUNKLENBQUM7b0JBRUYsSUFBSSxJQUFJLENBQUMsU0FBUyxFQUFFLENBQUM7d0JBQ2pCLE9BQU8sQ0FBQyxnQkFBZ0IsQ0FBQyxhQUFhLEVBQUUsSUFBSSxDQUFDLFNBQVMsQ0FBQyxDQUFDO29CQUM1RCxDQUFDO2dCQUNMLENBQUM7Z0JBRUQsWUFBWSxDQUFDLE9BQXVCLEVBQUUsSUFBVTtvQkFDNUMsTUFBTSxJQUFJLEdBQUcsSUFBSSxRQUFRLEVBQUUsQ0FBQztvQkFDNUIsSUFBSSxDQUFDLE1BQU0sQ0FBQyxRQUFRLEVBQUUsSUFBSSxDQUFDLENBQUM7b0JBRTVCLElBQUksQ0FBQyxNQUFNLENBQUMsU0FBUyxFQUFFLElBQUksQ0FBQyxRQUFRLENBQUMsT0FBTyxDQUFDLENBQUM7b0JBQzlDLE9BQU8sQ0FBQyxJQUFJLENBQUMsSUFBSSxDQUFDLENBQUM7Z0JBQ3ZCLENBQUM7YUFDSjtZQTlEWSxpQkFBUSxXQThEcEIsQ0FBQTtZQUVELE1BQWEsU0FBVSxTQUFRLElBQUk7Z0JBSy9CLFlBQVksUUFBZ0I7b0JBQ3hCLEtBQUssQ0FBQyxRQUFRLENBQUMsQ0FBQztvQkFIWixZQUFPLEdBQUcsSUFBSSxHQUFHLEVBQVEsQ0FBQztnQkFJbEMsQ0FBQztnQkFFRCxLQUFLLENBQUMsTUFBTSxDQUFDLElBQVU7b0JBQ25CLElBQUksSUFBSSxDQUFDLE9BQU8sQ0FBQyxHQUFHLENBQUMsSUFBSSxDQUFDLEVBQUUsQ0FBQzt3QkFDekIsT0FBTyxDQUFDLElBQUksQ0FBQyx5QkFBeUIsQ0FBQyxDQUFDO3dCQUN4QyxPQUFPO29CQUNYLENBQUM7b0JBQ0QsSUFBSSxDQUFDLE9BQU8sQ0FBQyxHQUFHLENBQUMsSUFBSSxDQUFDLENBQUM7b0JBRXZCLElBQUksSUFBSSxDQUFDO29CQUVULElBQUksQ0FBQzt3QkFDRCxJQUFJLEdBQUcsTUFBTSxJQUFJLENBQUMsaUJBQWlCLENBQUMsSUFBSSxDQUFDLENBQUM7b0JBQzlDLENBQUM7b0JBQUMsT0FBTyxHQUFHLEVBQUUsQ0FBQzt3QkFDWCxJQUFJLE9BQU8sR0FBRyxLQUFLLFFBQVEsRUFBRSxDQUFDOzRCQUMxQixJQUFJLENBQUMsYUFBYSxDQUFDLElBQUksRUFBRSxHQUFHLENBQUMsQ0FBQzt3QkFDbEMsQ0FBQzs2QkFBTSxDQUFDOzRCQUNKLElBQUksQ0FBQyxZQUFZLENBQUMsSUFBSSxFQUFFLEdBQVUsQ0FBQyxDQUFDO3dCQUN4QyxDQUFDO3dCQUNELE9BQU87b0JBQ1gsQ0FBQztvQkFFRCxJQUFJLENBQUMsY0FBYyxDQUFDLElBQUksRUFBRSxJQUFJLENBQUMsRUFBRSxDQUFDLENBQUM7b0JBQ25DLElBQUksQ0FBQyxhQUFhLENBQUMsSUFBSSxDQUFDLENBQUM7b0JBRXpCLElBQUksQ0FBQyxTQUFTLENBQUMsSUFBSSxFQUFFLElBQUksQ0FBQyxDQUFDO2dCQUMvQixDQUFDO2dCQUVELEtBQUssQ0FBQyxNQUFNLENBQUMsSUFBVSxFQUFFLEVBQVU7b0JBQy9CLElBQUksSUFBSSxDQUFDLE9BQU8sQ0FBQyxHQUFHLENBQUMsSUFBSSxDQUFDLEVBQUUsQ0FBQzt3QkFDekIsT0FBTyxDQUFDLElBQUksQ0FBQyx5QkFBeUIsQ0FBQyxDQUFDO3dCQUN4QyxPQUFPO29CQUNYLENBQUM7b0JBQ0QsSUFBSSxDQUFDLE9BQU8sQ0FBQyxHQUFHLENBQUMsSUFBSSxDQUFDLENBQUM7b0JBRXZCLElBQUksSUFBSSxHQUFHLE1BQU0sSUFBSSxDQUFDLFdBQVcsQ0FBQyxFQUFFLENBQUMsQ0FBQztvQkFDdEMsSUFBSSxDQUFDLGFBQWEsQ0FBQyxJQUFJLENBQUMsQ0FBQztvQkFFekIsSUFBSSxDQUFDLFNBQVMsQ0FBQyxJQUFJLEVBQUUsSUFBSSxDQUFDLENBQUM7Z0JBQy9CLENBQUM7Z0JBRUQsS0FBSyxDQUFDLElBQVU7b0JBQ1osSUFBSSxDQUFDLE9BQU8sQ0FBQyxNQUFNLENBQUMsSUFBSSxDQUFDLENBQUM7Z0JBQzlCLENBQUM7Z0JBRUQsS0FBSyxDQUFDLFNBQVMsQ0FBQyxJQUFVLEVBQUUsSUFBZ0I7b0JBQ3hDLElBQUksS0FBSyxHQUFHLElBQUksQ0FBQyxZQUFZLENBQUMsUUFBUSxJQUFJLENBQUMsQ0FBQztvQkFFNUMsT0FBTyxLQUFLLEdBQUcsSUFBSSxDQUFDLElBQUksRUFBRSxDQUFDO3dCQUN2QixJQUFJLENBQUMsSUFBSSxDQUFDLE9BQU8sQ0FBQyxHQUFHLENBQUMsSUFBSSxDQUFDLEVBQUUsQ0FBQzs0QkFDMUIsT0FBTyxDQUFDLElBQUksQ0FBQyx1QkFBdUIsQ0FBQyxDQUFDOzRCQUN0QyxPQUFPO3dCQUNYLENBQUM7d0JBRUQsSUFBSSxHQUFHLE1BQU0sSUFBSSxDQUFDLFlBQVksQ0FDMUIsSUFBSSxFQUNKLElBQUksQ0FBQyxLQUFLLENBQUMsS0FBSyxFQUFFLEtBQUssR0FBRyxJQUFJLENBQUMsUUFBUSxDQUFDLFNBQVMsQ0FBQyxFQUNsRCxLQUFLLENBQ1IsQ0FBQzt3QkFFRixNQUFNLFFBQVEsR0FBRyxJQUFJLENBQUMsWUFBWSxDQUFDLFFBQVEsQ0FBQzt3QkFDNUMsSUFBSSxRQUFRLElBQUksS0FBSyxFQUFFLENBQUM7NEJBQ3BCLE1BQU0sSUFBSSxLQUFLLENBQUMsMEJBQTBCLENBQUMsQ0FBQzt3QkFDaEQsQ0FBQzt3QkFFRCxJQUFJLENBQUMsZ0JBQWdCLENBQUMsSUFBSSxFQUFFLFFBQVEsRUFBRSxJQUFJLENBQUMsSUFBSSxDQUFDLENBQUM7d0JBQ2pELEtBQUssR0FBRyxRQUFRLENBQUM7b0JBQ3JCLENBQUM7b0JBRUQsSUFBSSxDQUFDLGdCQUFnQixDQUFDLElBQUksRUFBRSxJQUFJLENBQUMsSUFBSSxFQUFFLElBQUksQ0FBQyxJQUFJLENBQUMsQ0FBQztvQkFDbEQsSUFBSSxDQUFDO3dCQUNELElBQUksR0FBRyxNQUFNLElBQUksQ0FBQyxlQUFlLENBQUMsSUFBSSxDQUFDLENBQUM7b0JBQzVDLENBQUM7b0JBQUMsT0FBTyxHQUFHLEVBQUUsQ0FBQzt3QkFDWCxJQUFJLE9BQU8sR0FBRyxLQUFLLFFBQVEsRUFBRSxDQUFDOzRCQUMxQixJQUFJLENBQUMsYUFBYSxDQUFDLElBQUksRUFBRSxHQUFHLENBQUMsQ0FBQzt3QkFDbEMsQ0FBQzs2QkFBTSxDQUFDOzRCQUNKLElBQUksQ0FBQyxZQUFZLENBQUMsSUFBSSxFQUFFLEdBQVUsQ0FBQyxDQUFDO3dCQUN4QyxDQUFDO3dCQUVELE9BQU87b0JBQ1gsQ0FBQztvQkFDRCxJQUFJLENBQUMsY0FBYyxDQUFDLElBQUksRUFBRSxJQUFJLENBQUMsQ0FBQztnQkFDcEMsQ0FBQztnQkFFRCxpQkFBaUIsQ0FBQyxJQUFVO29CQUN4QixPQUFPLElBQUksT0FBTyxDQUFDLENBQUMsSUFBSSxFQUFFLElBQUksRUFBRSxFQUFFLENBQzlCLElBQUksQ0FBQyxPQUFPLENBQUMsTUFBTSxDQUFDLElBQUksQ0FDcEIsTUFBTSxFQUNOLHlCQUF5QixFQUN6QixNQUFNLENBQUMsTUFBTSxDQUNULEVBQUUsRUFDRixJQUFJLENBQUMsUUFBUSxDQUFDLGlCQUFpQixJQUFJLEVBQUUsRUFDckM7d0JBQ0ksT0FBTyxFQUFFLElBQUksQ0FBQyxRQUFRLENBQUMsT0FBTzt3QkFDOUIsSUFBSSxFQUFFLElBQUksQ0FBQyxJQUFJO3dCQUNmLElBQUksRUFBRSxJQUFJLENBQUMsSUFBSTtxQkFDbEIsQ0FDSixFQUNELENBQUMsSUFBUyxFQUFFLEVBQUU7d0JBQ1YsSUFBSSxDQUFDLElBQUksQ0FBQyxNQUFNLENBQUMsQ0FBQztvQkFDdEIsQ0FBQyxFQUNELENBQUMsSUFBUyxFQUFFLEVBQUU7d0JBQ1YsSUFBSSxDQUNBLE9BQU8sSUFBSSxDQUFDLFlBQVksS0FBSyxRQUFROzRCQUNqQyxDQUFDLENBQUMsSUFBSSxDQUFDLFlBQVk7NEJBQ25CLENBQUMsQ0FBQyxJQUFJLENBQUMsWUFBWSxDQUFDLEtBQUssQ0FDaEMsQ0FBQztvQkFDTixDQUFDLENBQ0osQ0FDSixDQUFDO2dCQUNOLENBQUM7Z0JBRUQsV0FBVyxDQUFDLEVBQVU7b0JBQ2xCLE9BQU8sSUFBSSxPQUFPLENBQUMsQ0FBQyxJQUFJLEVBQUUsSUFBSSxFQUFFLEVBQUUsQ0FDOUIsSUFBSSxDQUFDLE9BQU8sQ0FBQyxNQUFNLENBQUMsSUFBSSxDQUNwQixLQUFLLEVBQ0wsbUJBQW1CLEVBQ25CLE9BQU8sRUFBRSxFQUFFLEVBQ1gsQ0FBQyxJQUFTLEVBQUUsRUFBRTt3QkFDVixJQUFJLENBQUMsSUFBSSxDQUFDLE1BQU0sQ0FBQyxDQUFDO29CQUN0QixDQUFDLEVBQ0QsQ0FBQyxJQUFTLEVBQUUsRUFBRTt3QkFDVixJQUFJLENBQ0EsT0FBTyxJQUFJLENBQUMsWUFBWSxLQUFLLFFBQVE7NEJBQ2pDLENBQUMsQ0FBQyxJQUFJLENBQUMsWUFBWTs0QkFDbkIsQ0FBQyxDQUFDLElBQUksQ0FBQyxZQUFZLENBQUMsS0FBSyxDQUNoQyxDQUFDO29CQUNOLENBQUMsQ0FDSixDQUNKLENBQUM7Z0JBQ04sQ0FBQztnQkFFRCxZQUFZLENBQ1IsSUFBZ0IsRUFDaEIsSUFBVSxFQUNWLEtBQWE7b0JBRWIsSUFBSSxDQUFDLElBQUksQ0FBQyxJQUFJLEVBQUUsQ0FBQzt3QkFDYixNQUFNLElBQUksS0FBSyxDQUFDLGlDQUFpQyxDQUFDLENBQUM7b0JBQ3ZELENBQUM7b0JBQ0QsTUFBTSxPQUFPLEdBQUcsSUFBSSxjQUFjLEVBQUUsQ0FBQztvQkFFckMsTUFBTSxNQUFNLEdBQUcsSUFBSSxPQUFPLENBQWEsQ0FBQyxJQUFJLEVBQUUsSUFBSSxFQUFFLEVBQUU7d0JBQ2xELE9BQU8sQ0FBQyxnQkFBZ0IsQ0FBQyxNQUFNLEVBQUUsQ0FBQyxLQUFLLEVBQUUsRUFBRTs0QkFDdkMsTUFBTSxNQUFNLEdBQUcsSUFBSSxDQUFDLEtBQUssQ0FBQyxPQUFPLENBQUMsWUFBWSxDQUFDLENBQUM7NEJBQ2hELElBQUksTUFBTSxDQUFDLE9BQU8sRUFBRSxDQUFDO2dDQUNqQixJQUFJLENBQUMsTUFBTSxDQUFDLE1BQU0sQ0FBQyxDQUFDOzRCQUN4QixDQUFDO2lDQUFNLENBQUM7Z0NBQ0osSUFBSSxDQUFDLE1BQU0sQ0FBQyxLQUFLLENBQUMsQ0FBQzs0QkFDdkIsQ0FBQzt3QkFDTCxDQUFDLENBQUMsQ0FBQzt3QkFFSCxPQUFPLENBQUMsZ0JBQWdCLENBQUMsT0FBTyxFQUFFLENBQUMsS0FBSyxFQUFFLEVBQUUsQ0FDeEMsSUFBSSxDQUFDLE9BQU8sQ0FBQyxZQUFZLENBQUMsQ0FDN0IsQ0FBQztvQkFDTixDQUFDLENBQUMsQ0FBQztvQkFFSCxPQUFPLENBQUMsSUFBSSxDQUNSLE1BQU0sRUFDTixJQUFJLENBQUMsT0FBTyxDQUFDLE1BQU0sQ0FBQyxHQUFHLENBQ25CLGlDQUFpQyxDQUNwQyxDQUNKLENBQUM7b0JBRUYsSUFBSSxJQUFJLENBQUMsU0FBUyxFQUFFLENBQUM7d0JBQ2pCLE9BQU8sQ0FBQyxnQkFBZ0IsQ0FBQyxhQUFhLEVBQUUsSUFBSSxDQUFDLFNBQVMsQ0FBQyxDQUFDO29CQUM1RCxDQUFDO29CQUVELElBQUksQ0FBQyxZQUFZLENBQUMsT0FBTyxFQUFFLElBQUksRUFBRSxLQUFLLEVBQUUsSUFBSSxDQUFDLEVBQUUsQ0FBQyxDQUFDO29CQUVqRCxPQUFPLE1BQU0sQ0FBQztnQkFDbEIsQ0FBQztnQkFFRCxZQUFZLENBQ1IsT0FBdUIsRUFDdkIsSUFBVSxFQUNWLFFBQWdCLEVBQ2hCLEVBQVU7b0JBRVYsTUFBTSxJQUFJLEdBQUcsSUFBSSxRQUFRLEVBQUUsQ0FBQztvQkFDNUIsSUFBSSxDQUFDLE1BQU0sQ0FBQyxRQUFRLEVBQUUsSUFBSSxDQUFDLENBQUM7b0JBQzVCLElBQUksQ0FBQyxNQUFNLENBQUMsVUFBVSxFQUFFLE1BQU0sQ0FBQyxRQUFRLENBQUMsQ0FBQyxDQUFDO29CQUMxQyxJQUFJLENBQUMsTUFBTSxDQUFDLElBQUksRUFBRSxFQUFFLENBQUMsQ0FBQztvQkFDdEIsT0FBTyxDQUFDLElBQUksQ0FBQyxJQUFJLENBQUMsQ0FBQztnQkFDdkIsQ0FBQztnQkFFRCxlQUFlLENBQUMsSUFBZ0I7b0JBQzVCLE9BQU8sSUFBSSxPQUFPLENBQUMsQ0FBQyxJQUFJLEVBQUUsSUFBSSxFQUFFLEVBQUUsQ0FDOUIsSUFBSSxDQUFDLE9BQU8sQ0FBQyxNQUFNLENBQUMsSUFBSSxDQUNwQixNQUFNLEVBQ04sdUJBQXVCLEVBQ3ZCLE1BQU0sQ0FBQyxNQUFNLENBQ1QsRUFBRSxFQUNGLElBQUksQ0FBQyxRQUFRLENBQUMsZUFBZSxJQUFJLEVBQUUsRUFDbkM7d0JBQ0ksRUFBRSxFQUFFLElBQUksQ0FBQyxFQUFFO3FCQUNkLENBQ0osRUFDRCxDQUFDLElBQVMsRUFBRSxFQUFFO3dCQUNWLElBQUksQ0FBQyxJQUFJLENBQUMsTUFBTSxDQUFDLENBQUM7b0JBQ3RCLENBQUMsRUFDRCxDQUFDLElBQVMsRUFBRSxFQUFFO3dCQUNWLElBQUksQ0FDQSxPQUFPLElBQUksQ0FBQyxZQUFZLEtBQUssUUFBUTs0QkFDakMsQ0FBQyxDQUFDLElBQUksQ0FBQyxZQUFZOzRCQUNuQixDQUFDLENBQUMsSUFBSSxDQUFDLFlBQVksQ0FBQyxLQUFLLENBQ2hDLENBQUM7b0JBQ04sQ0FBQyxDQUNKLENBQ0osQ0FBQztnQkFDTixDQUFDOztZQXhOTSx5QkFBZSxHQUFHLEVBQUUsU0FBUyxFQUFFLElBQUksR0FBRyxJQUFJLEdBQUcsQ0FBQyxFQUFFLEFBQWpDLENBQWtDO1lBRC9DLGtCQUFTLFlBME5yQixDQUFBO1FBQ0wsQ0FBQyxFQXpXZ0IsUUFBUSxHQUFSLHNCQUFRLEtBQVIsc0JBQVEsUUF5V3hCO0lBQ0wsQ0FBQyxFQTdZZ0IsYUFBYSxHQUFiLGtCQUFhLEtBQWIsa0JBQWEsUUE2WTdCO0FBQ0wsQ0FBQyxFQW5aUyxJQUFJLEtBQUosSUFBSSxRQW1aYiIsInNvdXJjZXNDb250ZW50IjpbIm5hbWVzcGFjZSBja2FuIHtcbiAgICBleHBvcnQgdmFyIHNhbmRib3g6IGFueTtcbiAgICBleHBvcnQgdmFyIHB1YnN1YjogYW55O1xuICAgIGV4cG9ydCB2YXIgbW9kdWxlOiAobmFtZTogc3RyaW5nLCBpbml0aWFsaXplcjogKCQ6IGFueSkgPT4gYW55KSA9PiBhbnk7XG5cbiAgICBleHBvcnQgbmFtZXNwYWNlIENLQU5FWFRfRklMRVMge1xuICAgICAgICB0eXBlIFVwbG9hZGVyU2V0dGluZ3MgPSB7XG4gICAgICAgICAgICBzdG9yYWdlOiBzdHJpbmc7XG4gICAgICAgICAgICBba2V5OiBzdHJpbmddOiBhbnk7XG4gICAgICAgIH07XG5cbiAgICAgICAgZXhwb3J0IGNvbnN0IHRvcGljcyA9IHtcbiAgICAgICAgICAgIGFkZEZpbGVUb1F1ZXVlOiBcImNrYW5leHQ6ZmlsZXM6cXVldWU6ZmlsZTphZGRcIixcbiAgICAgICAgICAgIHJlc3RvcmVGaWxlSW5RdWV1ZTogXCJja2FuZXh0OmZpbGVzOnF1ZXVlOmZpbGU6cmVzdG9yZVwiLFxuICAgICAgICAgICAgcXVldWVJdGVtVXBsb2FkZWQ6IFwiY2thbmV4dDpmaWxlczpxdWV1ZTpmaWxlOnVwbG9hZGVkXCIsXG4gICAgICAgIH07XG5cbiAgICAgICAgZXhwb3J0IGNvbnN0IGRlZmF1bHRTZXR0aW5ncyA9IHtcbiAgICAgICAgICAgIHN0b3JhZ2U6IFwiZGVmYXVsdFwiLFxuICAgICAgICB9O1xuXG4gICAgICAgIGZ1bmN0aW9uIHVwbG9hZChcbiAgICAgICAgICAgIGZpbGU6IEZpbGUsXG4gICAgICAgICAgICB1cGxvYWRlcjogYWRhcHRlcnMuQmFzZSA9IG1ha2VVcGxvYWRlcihcIlN0YW5kYXJkXCIpLFxuICAgICAgICApIHtcbiAgICAgICAgICAgIHJldHVybiB1cGxvYWRlci51cGxvYWQoZmlsZSk7XG4gICAgICAgIH1cblxuICAgICAgICBmdW5jdGlvbiBtYWtlVXBsb2FkZXIoYWRhcHRlcjogc3RyaW5nLCAuLi5vcHRpb25zOiBhbnkpIHtcbiAgICAgICAgICAgIGNvbnN0IGZhY3RvcnkgPSAoPHsgW2tleTogc3RyaW5nXTogdHlwZW9mIGFkYXB0ZXJzLkJhc2UgfT5hZGFwdGVycylbXG4gICAgICAgICAgICAgICAgYWRhcHRlclxuICAgICAgICAgICAgXTtcbiAgICAgICAgICAgIGlmICghZmFjdG9yeSkge1xuICAgICAgICAgICAgICAgIHRocm93IG5ldyBFcnJvcihgVXBsb2FkZXIgJHthZGFwdGVyfSBpcyBub3QgcmVnaXN0ZXJlZGApO1xuICAgICAgICAgICAgfVxuICAgICAgICAgICAgcmV0dXJuIG5ldyBmYWN0b3J5KC4uLm9wdGlvbnMpO1xuICAgICAgICB9XG5cbiAgICAgICAgY2thbi5zYW5kYm94LmV4dGVuZCh7IGZpbGVzOiB7IHVwbG9hZCwgbWFrZVVwbG9hZGVyIH0gfSk7XG5cbiAgICAgICAgZXhwb3J0IG5hbWVzcGFjZSBhZGFwdGVycyB7XG4gICAgICAgICAgICBleHBvcnQgdHlwZSBTdG9yYWdlRGF0YSA9IHtcbiAgICAgICAgICAgICAgICB1cGxvYWRlZDogbnVtYmVyO1xuICAgICAgICAgICAgICAgIHNpemU6IG51bWJlcjtcbiAgICAgICAgICAgIH07XG5cbiAgICAgICAgICAgIGV4cG9ydCB0eXBlIFVwbG9hZEluZm8gPSB7XG4gICAgICAgICAgICAgICAgaWQ6IHN0cmluZztcbiAgICAgICAgICAgICAgICBzdG9yYWdlX2RhdGE6IFN0b3JhZ2VEYXRhO1xuICAgICAgICAgICAgfTtcblxuICAgICAgICAgICAgZXhwb3J0IGNsYXNzIEJhc2UgZXh0ZW5kcyBFdmVudFRhcmdldCB7XG4gICAgICAgICAgICAgICAgc3RhdGljIGRlZmF1bHRTZXR0aW5nczogT2JqZWN0ID0ge307XG4gICAgICAgICAgICAgICAgcHJvdGVjdGVkIHNldHRpbmdzOiBVcGxvYWRlclNldHRpbmdzO1xuICAgICAgICAgICAgICAgIHByb3RlY3RlZCBzYW5kYm94OiBhbnk7XG4gICAgICAgICAgICAgICAgcHJvdGVjdGVkIGNzcmZUb2tlbjogc3RyaW5nO1xuXG4gICAgICAgICAgICAgICAgY29uc3RydWN0b3Ioc2V0dGluZ3MgPSB7fSkge1xuICAgICAgICAgICAgICAgICAgICBzdXBlcigpO1xuICAgICAgICAgICAgICAgICAgICB0aGlzLnNldHRpbmdzID0ge1xuICAgICAgICAgICAgICAgICAgICAgICAgLi4uZGVmYXVsdFNldHRpbmdzLFxuICAgICAgICAgICAgICAgICAgICAgICAgLi4uKHRoaXMuY29uc3RydWN0b3IgYXMgdHlwZW9mIEJhc2UpLmRlZmF1bHRTZXR0aW5ncyxcbiAgICAgICAgICAgICAgICAgICAgICAgIC4uLnNldHRpbmdzLFxuICAgICAgICAgICAgICAgICAgICB9O1xuICAgICAgICAgICAgICAgICAgICB0aGlzLnNhbmRib3ggPSBja2FuLnNhbmRib3goKTtcblxuICAgICAgICAgICAgICAgICAgICBjb25zdCBjc3JmRmllbGQgPVxuICAgICAgICAgICAgICAgICAgICAgICAgZG9jdW1lbnRcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAucXVlcnlTZWxlY3RvcihcIm1ldGFbbmFtZT1jc3JmX2ZpZWxkX25hbWVdXCIpXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgPy5nZXRBdHRyaWJ1dGUoXCJjb250ZW50XCIpID8/IFwiX2NzcmZfdG9rZW5cIjtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5jc3JmVG9rZW4gPVxuICAgICAgICAgICAgICAgICAgICAgICAgZG9jdW1lbnRcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAucXVlcnlTZWxlY3RvcihgbWV0YVtuYW1lPSR7Y3NyZkZpZWxkfV1gKVxuICAgICAgICAgICAgICAgICAgICAgICAgICAgID8uZ2V0QXR0cmlidXRlKFwiY29udGVudFwiKSB8fCBcIlwiO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIHVwbG9hZChmaWxlOiBGaWxlKSB7XG4gICAgICAgICAgICAgICAgICAgIHRocm93IG5ldyBFcnJvcihcIkJhc2UudXBsb2FkIGlzIG5vdCBpbXBsZW1lbnRlZFwiKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICByZXN1bWUoZmlsZTogRmlsZSwgaWQ6IHN0cmluZykge1xuICAgICAgICAgICAgICAgICAgICB0aHJvdyBuZXcgRXJyb3IoXCJCYXNlLnJlc3VtZSBpcyBub3QgaW1wbGVtZW50ZWRcIik7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgZGlzcGF0Y2hTdGFydChmaWxlOiBGaWxlKSB7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hFdmVudChcbiAgICAgICAgICAgICAgICAgICAgICAgIG5ldyBDdXN0b21FdmVudChcInN0YXJ0XCIsIHsgZGV0YWlsOiB7IGZpbGUgfSB9KSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgZGlzcGF0Y2hDb21taXQoZmlsZTogRmlsZSwgaWQ6IHN0cmluZykge1xuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRXZlbnQoXG4gICAgICAgICAgICAgICAgICAgICAgICBuZXcgQ3VzdG9tRXZlbnQoXCJjb21taXRcIiwgeyBkZXRhaWw6IHsgZmlsZSwgaWQgfSB9KSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgZGlzcGF0Y2hQcm9ncmVzcyhmaWxlOiBGaWxlLCBsb2FkZWQ6IG51bWJlciwgdG90YWw6IG51bWJlcikge1xuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRXZlbnQoXG4gICAgICAgICAgICAgICAgICAgICAgICBuZXcgQ3VzdG9tRXZlbnQoXCJwcm9ncmVzc1wiLCB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgZGV0YWlsOiB7IGZpbGUsIGxvYWRlZCwgdG90YWwgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgIH0pLFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICBkaXNwYXRjaEZpbmlzaChmaWxlOiBGaWxlLCByZXN1bHQ6IE9iamVjdCkge1xuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRXZlbnQoXG4gICAgICAgICAgICAgICAgICAgICAgICBuZXcgQ3VzdG9tRXZlbnQoXCJmaW5pc2hcIiwgeyBkZXRhaWw6IHsgZmlsZSwgcmVzdWx0IH0gfSksXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgIGRpc3BhdGNoRmFpbChmaWxlOiBGaWxlLCByZWFzb25zOiB7IFtrZXk6IHN0cmluZ106IHN0cmluZ1tdIH0pIHtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEV2ZW50KFxuICAgICAgICAgICAgICAgICAgICAgICAgbmV3IEN1c3RvbUV2ZW50KFwiZmFpbFwiLCB7IGRldGFpbDogeyBmaWxlLCByZWFzb25zIH0gfSksXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgIGRpc3BhdGNoRXJyb3IoZmlsZTogRmlsZSwgbWVzc2FnZTogc3RyaW5nKSB7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hFdmVudChcbiAgICAgICAgICAgICAgICAgICAgICAgIG5ldyBDdXN0b21FdmVudChcImVycm9yXCIsIHsgZGV0YWlsOiB7IGZpbGUsIG1lc3NhZ2UgfSB9KSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICB9XG5cbiAgICAgICAgICAgIGV4cG9ydCBjbGFzcyBTdGFuZGFyZCBleHRlbmRzIEJhc2Uge1xuICAgICAgICAgICAgICAgIHVwbG9hZChmaWxlOiBGaWxlKSB7XG4gICAgICAgICAgICAgICAgICAgIGNvbnN0IHJlcXVlc3QgPSBuZXcgWE1MSHR0cFJlcXVlc3QoKTtcbiAgICAgICAgICAgICAgICAgICAgY29uc3QgcHJvbWlzZSA9IHRoaXMuX2FkZExpc3RlbmVycyhyZXF1ZXN0LCBmaWxlKTtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5fcHJlcGFyZVJlcXVlc3QocmVxdWVzdCwgZmlsZSk7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuX3NlbmRSZXF1ZXN0KHJlcXVlc3QsIGZpbGUpO1xuICAgICAgICAgICAgICAgICAgICByZXR1cm4gcHJvbWlzZTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBfYWRkTGlzdGVuZXJzKFxuICAgICAgICAgICAgICAgICAgICByZXF1ZXN0OiBYTUxIdHRwUmVxdWVzdCxcbiAgICAgICAgICAgICAgICAgICAgZmlsZTogRmlsZSxcbiAgICAgICAgICAgICAgICApOiBQcm9taXNlPFVwbG9hZEluZm8+IHtcbiAgICAgICAgICAgICAgICAgICAgcmVxdWVzdC51cGxvYWQuYWRkRXZlbnRMaXN0ZW5lcihcImxvYWRzdGFydFwiLCAoZXZlbnQpID0+XG4gICAgICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoU3RhcnQoZmlsZSksXG4gICAgICAgICAgICAgICAgICAgICk7XG5cbiAgICAgICAgICAgICAgICAgICAgcmVxdWVzdC51cGxvYWQuYWRkRXZlbnRMaXN0ZW5lcihcInByb2dyZXNzXCIsIChldmVudCkgPT5cbiAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hQcm9ncmVzcyhmaWxlLCBldmVudC5sb2FkZWQsIGV2ZW50LnRvdGFsKSxcbiAgICAgICAgICAgICAgICAgICAgKTtcblxuICAgICAgICAgICAgICAgICAgICByZXR1cm4gbmV3IFByb21pc2UoKGRvbmUsIGZhaWwpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgIHJlcXVlc3QuYWRkRXZlbnRMaXN0ZW5lcihcImxvYWRcIiwgKGV2ZW50KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgY29uc3QgcmVzdWx0ID0gSlNPTi5wYXJzZShyZXF1ZXN0LnJlc3BvbnNlVGV4dCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgaWYgKHJlc3VsdC5zdWNjZXNzKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hDb21taXQoZmlsZSwgcmVzdWx0LnJlc3VsdC5pZCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hGaW5pc2goZmlsZSwgcmVzdWx0LnJlc3VsdCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGRvbmUocmVzdWx0LnJlc3VsdCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfSBlbHNlIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEZhaWwoZmlsZSwgcmVzdWx0LmVycm9yKTtcblxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBmYWlsKHJlc3VsdC5lcnJvcik7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgICAgICAgICAgfSk7XG5cbiAgICAgICAgICAgICAgICAgICAgICAgIHJlcXVlc3QuYWRkRXZlbnRMaXN0ZW5lcihcImVycm9yXCIsIChldmVudCkgPT4ge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hFcnJvcihmaWxlLCByZXF1ZXN0LnJlc3BvbnNlVGV4dCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgZmFpbChyZXF1ZXN0LnJlc3BvbnNlVGV4dCk7XG4gICAgICAgICAgICAgICAgICAgICAgICB9KTtcbiAgICAgICAgICAgICAgICAgICAgfSk7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgX3ByZXBhcmVSZXF1ZXN0KHJlcXVlc3Q6IFhNTEh0dHBSZXF1ZXN0LCBmaWxlOiBGaWxlKSB7XG4gICAgICAgICAgICAgICAgICAgIHJlcXVlc3Qub3BlbihcbiAgICAgICAgICAgICAgICAgICAgICAgIFwiUE9TVFwiLFxuICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94LmNsaWVudC51cmwoXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgXCIvYXBpL2FjdGlvbi9maWxlc19maWxlX2NyZWF0ZVwiLFxuICAgICAgICAgICAgICAgICAgICAgICAgKSxcbiAgICAgICAgICAgICAgICAgICAgKTtcblxuICAgICAgICAgICAgICAgICAgICBpZiAodGhpcy5jc3JmVG9rZW4pIHtcbiAgICAgICAgICAgICAgICAgICAgICAgIHJlcXVlc3Quc2V0UmVxdWVzdEhlYWRlcihcIlgtQ1NSRlRva2VuXCIsIHRoaXMuY3NyZlRva2VuKTtcbiAgICAgICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIF9zZW5kUmVxdWVzdChyZXF1ZXN0OiBYTUxIdHRwUmVxdWVzdCwgZmlsZTogRmlsZSkge1xuICAgICAgICAgICAgICAgICAgICBjb25zdCBkYXRhID0gbmV3IEZvcm1EYXRhKCk7XG4gICAgICAgICAgICAgICAgICAgIGRhdGEuYXBwZW5kKFwidXBsb2FkXCIsIGZpbGUpO1xuXG4gICAgICAgICAgICAgICAgICAgIGRhdGEuYXBwZW5kKFwic3RvcmFnZVwiLCB0aGlzLnNldHRpbmdzLnN0b3JhZ2UpO1xuICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LnNlbmQoZGF0YSk7XG4gICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICBleHBvcnQgY2xhc3MgTXVsdGlwYXJ0IGV4dGVuZHMgQmFzZSB7XG4gICAgICAgICAgICAgICAgc3RhdGljIGRlZmF1bHRTZXR0aW5ncyA9IHsgY2h1bmtTaXplOiAxMDI0ICogMTAyNCAqIDUgfTtcblxuICAgICAgICAgICAgICAgIHByaXZhdGUgX2FjdGl2ZSA9IG5ldyBTZXQ8RmlsZT4oKTtcblxuICAgICAgICAgICAgICAgIGNvbnN0cnVjdG9yKHNldHRpbmdzOiBPYmplY3QpIHtcbiAgICAgICAgICAgICAgICAgICAgc3VwZXIoc2V0dGluZ3MpO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIGFzeW5jIHVwbG9hZChmaWxlOiBGaWxlKSB7XG4gICAgICAgICAgICAgICAgICAgIGlmICh0aGlzLl9hY3RpdmUuaGFzKGZpbGUpKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICBjb25zb2xlLndhcm4oXCJGaWxlIHVwbG9hZCBpbiBwcm9ncmVzc1wiKTtcbiAgICAgICAgICAgICAgICAgICAgICAgIHJldHVybjtcbiAgICAgICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgICAgICB0aGlzLl9hY3RpdmUuYWRkKGZpbGUpO1xuXG4gICAgICAgICAgICAgICAgICAgIGxldCBpbmZvO1xuXG4gICAgICAgICAgICAgICAgICAgIHRyeSB7XG4gICAgICAgICAgICAgICAgICAgICAgICBpbmZvID0gYXdhaXQgdGhpcy5faW5pdGlhbGl6ZVVwbG9hZChmaWxlKTtcbiAgICAgICAgICAgICAgICAgICAgfSBjYXRjaCAoZXJyKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICBpZiAodHlwZW9mIGVyciA9PT0gXCJzdHJpbmdcIikge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hFcnJvcihmaWxlLCBlcnIpO1xuICAgICAgICAgICAgICAgICAgICAgICAgfSBlbHNlIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRmFpbChmaWxlLCBlcnIgYXMgYW55KTtcbiAgICAgICAgICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICAgICAgICAgIHJldHVybjtcbiAgICAgICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hDb21taXQoZmlsZSwgaW5mby5pZCk7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hTdGFydChmaWxlKTtcblxuICAgICAgICAgICAgICAgICAgICB0aGlzLl9kb1VwbG9hZChmaWxlLCBpbmZvKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBhc3luYyByZXN1bWUoZmlsZTogRmlsZSwgaWQ6IHN0cmluZykge1xuICAgICAgICAgICAgICAgICAgICBpZiAodGhpcy5fYWN0aXZlLmhhcyhmaWxlKSkge1xuICAgICAgICAgICAgICAgICAgICAgICAgY29uc29sZS53YXJuKFwiRmlsZSB1cGxvYWQgaW4gcHJvZ3Jlc3NcIik7XG4gICAgICAgICAgICAgICAgICAgICAgICByZXR1cm47XG4gICAgICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICAgICAgdGhpcy5fYWN0aXZlLmFkZChmaWxlKTtcblxuICAgICAgICAgICAgICAgICAgICBsZXQgaW5mbyA9IGF3YWl0IHRoaXMuX3Nob3dVcGxvYWQoaWQpO1xuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoU3RhcnQoZmlsZSk7XG5cbiAgICAgICAgICAgICAgICAgICAgdGhpcy5fZG9VcGxvYWQoZmlsZSwgaW5mbyk7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgcGF1c2UoZmlsZTogRmlsZSkge1xuICAgICAgICAgICAgICAgICAgICB0aGlzLl9hY3RpdmUuZGVsZXRlKGZpbGUpO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIGFzeW5jIF9kb1VwbG9hZChmaWxlOiBGaWxlLCBpbmZvOiBVcGxvYWRJbmZvKSB7XG4gICAgICAgICAgICAgICAgICAgIGxldCBzdGFydCA9IGluZm8uc3RvcmFnZV9kYXRhLnVwbG9hZGVkIHx8IDA7XG5cbiAgICAgICAgICAgICAgICAgICAgd2hpbGUgKHN0YXJ0IDwgZmlsZS5zaXplKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICBpZiAoIXRoaXMuX2FjdGl2ZS5oYXMoZmlsZSkpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBjb25zb2xlLmluZm8oXCJGaWxlIHVwbG9hZCBpcyBwYXVzZWRcIik7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgcmV0dXJuO1xuICAgICAgICAgICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgICAgICAgICBpbmZvID0gYXdhaXQgdGhpcy5fdXBsb2FkQ2h1bmsoXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgaW5mbyxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBmaWxlLnNsaWNlKHN0YXJ0LCBzdGFydCArIHRoaXMuc2V0dGluZ3MuY2h1bmtTaXplKSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBzdGFydCxcbiAgICAgICAgICAgICAgICAgICAgICAgICk7XG5cbiAgICAgICAgICAgICAgICAgICAgICAgIGNvbnN0IHVwbG9hZGVkID0gaW5mby5zdG9yYWdlX2RhdGEudXBsb2FkZWQ7XG4gICAgICAgICAgICAgICAgICAgICAgICBpZiAodXBsb2FkZWQgPD0gc3RhcnQpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB0aHJvdyBuZXcgRXJyb3IoXCJVcGxvYWRlZCBzaXplIGlzIHJlZHVjZWRcIik7XG4gICAgICAgICAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hQcm9ncmVzcyhmaWxlLCB1cGxvYWRlZCwgZmlsZS5zaXplKTtcbiAgICAgICAgICAgICAgICAgICAgICAgIHN0YXJ0ID0gdXBsb2FkZWQ7XG4gICAgICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoUHJvZ3Jlc3MoZmlsZSwgZmlsZS5zaXplLCBmaWxlLnNpemUpO1xuICAgICAgICAgICAgICAgICAgICB0cnkge1xuICAgICAgICAgICAgICAgICAgICAgICAgaW5mbyA9IGF3YWl0IHRoaXMuX2NvbXBsZXRlVXBsb2FkKGluZm8pO1xuICAgICAgICAgICAgICAgICAgICB9IGNhdGNoIChlcnIpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgIGlmICh0eXBlb2YgZXJyID09PSBcInN0cmluZ1wiKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEVycm9yKGZpbGUsIGVycik7XG4gICAgICAgICAgICAgICAgICAgICAgICB9IGVsc2Uge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hGYWlsKGZpbGUsIGVyciBhcyBhbnkpO1xuICAgICAgICAgICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgICAgICAgICByZXR1cm47XG4gICAgICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEZpbmlzaChmaWxlLCBpbmZvKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBfaW5pdGlhbGl6ZVVwbG9hZChmaWxlOiBGaWxlKTogUHJvbWlzZTxVcGxvYWRJbmZvPiB7XG4gICAgICAgICAgICAgICAgICAgIHJldHVybiBuZXcgUHJvbWlzZSgoZG9uZSwgZmFpbCkgPT5cbiAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5jbGllbnQuY2FsbChcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBcIlBPU1RcIixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBcImZpbGVzX3VwbG9hZF9pbml0aWFsaXplXCIsXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgT2JqZWN0LmFzc2lnbihcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAge30sXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2V0dGluZ3MuaW5pdGlhbGl6ZVBheWxvYWQgfHwge30sXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHN0b3JhZ2U6IHRoaXMuc2V0dGluZ3Muc3RvcmFnZSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIG5hbWU6IGZpbGUubmFtZSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHNpemU6IGZpbGUuc2l6ZSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICApLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIChkYXRhOiBhbnkpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZG9uZShkYXRhLnJlc3VsdCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAocmVzcDogYW55KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGZhaWwoXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB0eXBlb2YgcmVzcC5yZXNwb25zZUpTT04gPT09IFwic3RyaW5nXCJcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICA/IHJlc3AucmVzcG9uc2VUZXh0XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgOiByZXNwLnJlc3BvbnNlSlNPTi5lcnJvcixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgKSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBfc2hvd1VwbG9hZChpZDogc3RyaW5nKTogUHJvbWlzZTxVcGxvYWRJbmZvPiB7XG4gICAgICAgICAgICAgICAgICAgIHJldHVybiBuZXcgUHJvbWlzZSgoZG9uZSwgZmFpbCkgPT5cbiAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5jbGllbnQuY2FsbChcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBcIkdFVFwiLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiZmlsZXNfdXBsb2FkX3Nob3dcIixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBgP2lkPSR7aWR9YCxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAoZGF0YTogYW55KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGRvbmUoZGF0YS5yZXN1bHQpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgKHJlc3A6IGFueSkgPT4ge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBmYWlsKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgdHlwZW9mIHJlc3AucmVzcG9uc2VKU09OID09PSBcInN0cmluZ1wiXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgPyByZXNwLnJlc3BvbnNlVGV4dFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIDogcmVzcC5yZXNwb25zZUpTT04uZXJyb3IsXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICksXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgX3VwbG9hZENodW5rKFxuICAgICAgICAgICAgICAgICAgICBpbmZvOiBVcGxvYWRJbmZvLFxuICAgICAgICAgICAgICAgICAgICBwYXJ0OiBCbG9iLFxuICAgICAgICAgICAgICAgICAgICBzdGFydDogbnVtYmVyLFxuICAgICAgICAgICAgICAgICk6IFByb21pc2U8VXBsb2FkSW5mbz4ge1xuICAgICAgICAgICAgICAgICAgICBpZiAoIXBhcnQuc2l6ZSkge1xuICAgICAgICAgICAgICAgICAgICAgICAgdGhyb3cgbmV3IEVycm9yKFwiMC1sZW5ndGggY2h1bmtzIGFyZSBub3QgYWxsb3dlZFwiKTtcbiAgICAgICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgICAgICBjb25zdCByZXF1ZXN0ID0gbmV3IFhNTEh0dHBSZXF1ZXN0KCk7XG5cbiAgICAgICAgICAgICAgICAgICAgY29uc3QgcmVzdWx0ID0gbmV3IFByb21pc2U8VXBsb2FkSW5mbz4oKGRvbmUsIGZhaWwpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgIHJlcXVlc3QuYWRkRXZlbnRMaXN0ZW5lcihcImxvYWRcIiwgKGV2ZW50KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgY29uc3QgcmVzdWx0ID0gSlNPTi5wYXJzZShyZXF1ZXN0LnJlc3BvbnNlVGV4dCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgaWYgKHJlc3VsdC5zdWNjZXNzKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGRvbmUocmVzdWx0LnJlc3VsdCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfSBlbHNlIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZmFpbChyZXN1bHQuZXJyb3IpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICAgICAgICAgIH0pO1xuXG4gICAgICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LmFkZEV2ZW50TGlzdGVuZXIoXCJlcnJvclwiLCAoZXZlbnQpID0+XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgZmFpbChyZXF1ZXN0LnJlc3BvbnNlVGV4dCksXG4gICAgICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgICAgICB9KTtcblxuICAgICAgICAgICAgICAgICAgICByZXF1ZXN0Lm9wZW4oXG4gICAgICAgICAgICAgICAgICAgICAgICBcIlBPU1RcIixcbiAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5jbGllbnQudXJsKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiL2FwaS9hY3Rpb24vZmlsZXNfdXBsb2FkX3VwZGF0ZVwiLFxuICAgICAgICAgICAgICAgICAgICAgICAgKSxcbiAgICAgICAgICAgICAgICAgICAgKTtcblxuICAgICAgICAgICAgICAgICAgICBpZiAodGhpcy5jc3JmVG9rZW4pIHtcbiAgICAgICAgICAgICAgICAgICAgICAgIHJlcXVlc3Quc2V0UmVxdWVzdEhlYWRlcihcIlgtQ1NSRlRva2VuXCIsIHRoaXMuY3NyZlRva2VuKTtcbiAgICAgICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgICAgIHRoaXMuX3NlbmRSZXF1ZXN0KHJlcXVlc3QsIHBhcnQsIHN0YXJ0LCBpbmZvLmlkKTtcblxuICAgICAgICAgICAgICAgICAgICByZXR1cm4gcmVzdWx0O1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIF9zZW5kUmVxdWVzdChcbiAgICAgICAgICAgICAgICAgICAgcmVxdWVzdDogWE1MSHR0cFJlcXVlc3QsXG4gICAgICAgICAgICAgICAgICAgIHBhcnQ6IEJsb2IsXG4gICAgICAgICAgICAgICAgICAgIHBvc2l0aW9uOiBudW1iZXIsXG4gICAgICAgICAgICAgICAgICAgIGlkOiBzdHJpbmcsXG4gICAgICAgICAgICAgICAgKSB7XG4gICAgICAgICAgICAgICAgICAgIGNvbnN0IGZvcm0gPSBuZXcgRm9ybURhdGEoKTtcbiAgICAgICAgICAgICAgICAgICAgZm9ybS5hcHBlbmQoXCJ1cGxvYWRcIiwgcGFydCk7XG4gICAgICAgICAgICAgICAgICAgIGZvcm0uYXBwZW5kKFwicG9zaXRpb25cIiwgU3RyaW5nKHBvc2l0aW9uKSk7XG4gICAgICAgICAgICAgICAgICAgIGZvcm0uYXBwZW5kKFwiaWRcIiwgaWQpO1xuICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LnNlbmQoZm9ybSk7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgX2NvbXBsZXRlVXBsb2FkKGluZm86IFVwbG9hZEluZm8pOiBQcm9taXNlPFVwbG9hZEluZm8+IHtcbiAgICAgICAgICAgICAgICAgICAgcmV0dXJuIG5ldyBQcm9taXNlKChkb25lLCBmYWlsKSA9PlxuICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94LmNsaWVudC5jYWxsKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiUE9TVFwiLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiZmlsZXNfdXBsb2FkX2NvbXBsZXRlXCIsXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgT2JqZWN0LmFzc2lnbihcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAge30sXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2V0dGluZ3MuY29tcGxldGVQYXlsb2FkIHx8IHt9LFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBpZDogaW5mby5pZCxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICApLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIChkYXRhOiBhbnkpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZG9uZShkYXRhLnJlc3VsdCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAocmVzcDogYW55KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGZhaWwoXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB0eXBlb2YgcmVzcC5yZXNwb25zZUpTT04gPT09IFwic3RyaW5nXCJcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICA/IHJlc3AucmVzcG9uc2VUZXh0XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgOiByZXNwLnJlc3BvbnNlSlNPTi5lcnJvcixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgKSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICB9XG4gICAgICAgIH1cbiAgICB9XG59XG4iXX0=
```

### Comparing `ckanext_files-0.2.6/ckanext/files/base.py` & `ckanext_files-0.3.0/ckanext/files/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,14 +158,17 @@
 
     # combine multiple files into a new one
     COMPOSE = types.CapabilityUnit(1 << 9)
 
     # return specific range of file bytes
     RANGE = types.CapabilityUnit(1 << 10)
 
+    # return file details from the storage
+    ANALYZE = types.CapabilityUnit(1 << 11)
+
 
 class OptionChecker(object):
     """Mixin for standard access to required settings.
 
     Example:
     >>> value = storage.ensure_option({...}, "option_name")
 
@@ -259,14 +262,24 @@
         raise NotImplementedError
 
     def move(self, data, name, extras):
         # type: (types.MinimalStorageData, str, dict[str, types.Any]) -> types.MinimalStorageData
         """Move file to a different location inside the storage."""
         raise NotImplementedError
 
+    def scan(self):
+        # type: () -> types.Iterable[str]
+        """List all filenames in storage."""
+        raise NotImplementedError
+
+    def analyze(self, filename):
+        # type: (str) -> types.MinimalStorageData
+        """Return all details about filename."""
+        raise NotImplementedError
+
 
 class Reader(StorageService):
     def stream(self, data):
         # type: (types.MinimalStorageData) -> types.IO[bytes]
         """Return byte-stream of the file content."""
 
         raise NotImplementedError
@@ -397,14 +410,28 @@
     def remove(self, data):
         # type: (types.MinimalStorageData) -> bool
         if not self.supports(Capability.REMOVE):
             raise exceptions.UnsupportedOperationError("remove", type(self).__name__)
 
         return self.manager.remove(data)
 
+    def scan(self):
+        # type: () -> types.Iterable[str]
+        if not self.supports(Capability.SCAN):
+            raise exceptions.UnsupportedOperationError("scan", type(self).__name__)
+
+        return self.manager.scan()
+
+    def analyze(self, filename):
+        # type: (str) -> types.MinimalStorageData
+        if not self.supports(Capability.ANALYZE):
+            raise exceptions.UnsupportedOperationError("analyze", type(self).__name__)
+
+        return self.manager.analyze(filename)
+
     def stream(self, data):
         # type: (types.MinimalStorageData) -> types.IO[bytes]
         if not self.supports(Capability.STREAM):
             raise exceptions.UnsupportedOperationError("stream", type(self).__name__)
 
         return self.reader.stream(data)
```

### Comparing `ckanext_files-0.2.6/ckanext/files/command.py` & `ckanext_files-0.3.0/ckanext/files/command.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/config.py` & `ckanext_files-0.3.0/ckanext/files/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
     return tk.config.get(DEFAULT_STORAGE, "default")
 
 
 def storages():
     # type: () -> dict[str, dict[str, Any]]
     """Mapping of storage names to their settings."""
-
     storages = defaultdict(dict)  # type: dict[str, dict[str, Any]]
     prefix_len = len(STORAGE_PREFIX)
     for k, v in tk.config.items():
         if not k.startswith(STORAGE_PREFIX):
             continue
 
         try:
```

### Comparing `ckanext_files-0.2.6/ckanext/files/exceptions.py` & `ckanext_files-0.3.0/ckanext/files/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,22 +83,22 @@
     def __init__(self, adapter, operation, problem):
         # type: (type, str, str) -> None
         self.adapter = adapter
         self.operation = operation
         self.problem = problem
 
     def __str__(self):
-        return "Storage {} does not have sufficient permissions to perform {} operation: {}".format(
+        msg = "Storage {} is not allowed to perform {} operation: {}"
+        return msg.format(
             self.adapter.__name__,
             self.operation,
             self.problem,
         )
 
 
-
 class MissingStorageConfigurationError(InvalidStorageConfigurationError):
     """Storage cannot be initialized due to missing option."""
 
     def __init__(self, adapter, option):
         # type: (type, str) -> None
         return super(MissingStorageConfigurationError, self).__init__(
             adapter,
```

### Comparing `ckanext_files-0.2.6/ckanext/files/helpers.py` & `ckanext_files-0.3.0/ckanext/files/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/interfaces.py` & `ckanext_files-0.3.0/ckanext/files/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/logic/action.py` & `ckanext_files-0.3.0/ckanext/files/logic/action.py`

 * *Files 9% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
     try:
         storage_data = storage.upload(
             secure_filename(data_dict["name"]),
             data_dict["upload"],
             extras,
         )
-    except exceptions.LargeUploadError as err:
+    except exceptions.UploadError as err:
         raise tk.ValidationError({"upload": [str(err)]})  # noqa: B904
 
     fileobj = File(
         name=data_dict["name"],
         storage=data_dict["storage"],
         storage_data=storage_data,
         completed=True,
@@ -189,15 +189,15 @@
     storage = shared.get_storage(fileobj.storage)
     if not storage.supports(Capability.REMOVE):
         raise tk.ValidationError({"storage": ["Operation is not supported"]})
 
     try:
         storage.remove(fileobj.storage_data)
     except exceptions.PermissionError as err:
-        raise tk.NotAuthorized(str(err))
+        raise tk.NotAuthorized(str(err))  # noqa: B904
 
     _delete_owner(context, "file", fileobj.id)
     context["session"].delete(fileobj)
     context["session"].commit()
 
     return fileobj.dictize(context)
 
@@ -255,15 +255,15 @@
         raise tk.ValidationError({"storage": ["Operation is not supported"]})
 
     try:
         storage_data = storage.initialize_multipart_upload(
             secure_filename(data_dict["name"]),
             extras,
         )
-    except exceptions.LargeUploadError as err:
+    except exceptions.UploadError as err:
         raise tk.ValidationError({"upload": [str(err)]})  # noqa: B904
 
     fileobj = File(
         name=data_dict["name"],
         storage=data_dict["storage"],
         storage_data=storage_data,
     )
@@ -301,15 +301,19 @@
 
     fileobj = context["session"].query(File).filter_by(id=data_dict["id"]).one_or_none()
     if not fileobj:
         raise tk.ObjectNotFound("upload")
 
     storage = shared.get_storage(fileobj.storage)
 
-    fileobj.storage_data = storage.update_multipart_upload(fileobj.storage_data, extras)
+    try:
+        fileobj.storage_data = storage.update_multipart_upload(fileobj.storage_data, extras)
+    except exceptions.UploadError as err:
+        raise tk.ValidationError({"upload": [str(err)]})
+
     context["session"].commit()
 
     return fileobj.dictize(context)
 
 
 @action
 @validate(schema.upload_complete)
@@ -322,15 +326,19 @@
     data_dict["id"]
     fileobj = context["session"].query(File).filter_by(id=data_dict["id"]).one_or_none()
     if not fileobj:
         raise tk.ObjectNotFound("upload")
 
     storage = shared.get_storage(fileobj.storage)
 
-    fileobj.storage_data = storage.complete_multipart_upload(
-        fileobj.storage_data,
-        extras,
-    )
+    try:
+        fileobj.storage_data = storage.complete_multipart_upload(
+            fileobj.storage_data,
+            extras,
+        )
+    except exceptions.UploadError as err:
+        raise tk.ValidationError({"upload": [str(err)]})
+
     fileobj.completed = True
     context["session"].commit()
 
     return fileobj.dictize(context)
```

### Comparing `ckanext_files-0.2.6/ckanext/files/logic/auth.py` & `ckanext_files-0.3.0/ckanext/files/logic/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     }
 
 
 @auth
 @tk.auth_disallow_anonymous_access
 def files_file_create(context, data_dict):
     # type: (types.Any, dict[str, types.Any]) -> types.Any
-    return {"success": True}
+    return authz.is_authorized("files_manage_files", context, data_dict)
 
 
 @auth
 @tk.auth_disallow_anonymous_access
 def files_file_delete(context, data_dict):
     # type: (types.Any, dict[str, types.Any]) -> types.Any
     """Only owner can remove files."""
```

### Comparing `ckanext_files-0.2.6/ckanext/files/logic/schema.py` & `ckanext_files-0.3.0/ckanext/files/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/logic/validators.py` & `ckanext_files-0.3.0/ckanext/files/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/migration/files/alembic.ini` & `ckanext_files-0.3.0/ckanext/files/migration/files/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/migration/files/env.py` & `ckanext_files-0.3.0/ckanext/files/migration/files/env.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/migration/files/versions/2c5f1f90888c_add_file_last_access_field.py` & `ckanext_files-0.3.0/ckanext/files/migration/files/versions/2c5f1f90888c_add_file_last_access_field.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/migration/files/versions/2fbd30a1b364_create_owner_table.py` & `ckanext_files-0.3.0/ckanext/files/migration/files/versions/2fbd30a1b364_create_owner_table.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/migration/files/versions/3c69eb68cecd_create_upload_table.py` & `ckanext_files-0.3.0/ckanext/files/migration/files/versions/3c69eb68cecd_create_upload_table.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/migration/files/versions/5851e09b7ca3_remove_path_rename_kind_add_stats.py` & `ckanext_files-0.3.0/ckanext/files/migration/files/versions/5851e09b7ca3_remove_path_rename_kind_add_stats.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py` & `ckanext_files-0.3.0/ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py` & `ckanext_files-0.3.0/ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/model/file.py` & `ckanext_files-0.3.0/ckanext/files/model/file.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import copy
 
 import six
 import sqlalchemy as sa
 from sqlalchemy import Column, DateTime, UnicodeText
 from sqlalchemy.dialects.postgresql import JSONB
 
+import ckan.plugins.toolkit as tk
 from ckan.lib.dictization import table_dictize
 from ckan.model.types import make_uuid
 
 from .base import Base, now
 
 from datetime import datetime  # isort: skip # noqa: F401
 
@@ -72,7 +73,20 @@
                 target = target.setdefault(part, {})
                 if not isinstance(target, dict):
                     raise TypeError(part)
         target.update(patch)
 
         setattr(self, prop, data)
         return data
+
+    @classmethod
+    def by_location(cls, location, storage=None):
+        # type: (str, str | None) -> sa.sql.Select
+        selectable = cls if tk.check_ckan_version("2.9") else [cls]
+
+        stmt = sa.select(selectable).where(
+            cls.storage_data["filename"].astext == location,
+        )
+        if storage:
+            stmt = stmt.where(cls.storage == storage)
+
+        return stmt
```

### Comparing `ckanext_files-0.2.6/ckanext/files/model/owner.py` & `ckanext_files-0.3.0/ckanext/files/model/owner.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/plugin.py` & `ckanext_files-0.3.0/ckanext/files/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/public/ckanext-files/scripts/files--shared-uploader.js` & `ckanext_files-0.3.0/ckanext/files/public/ckanext-files/scripts/files--shared-uploader.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: ASCII text, with very long lines (698)*

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 000002a0: 4943 426a 6232 357a 6443 4277 6233 4a30  ICBjb25zdCBwb3J0
 000002b0: 4944 3067 5a58 5a6c 626e 5175 6347 3979  ID0gZXZlbnQucG9y
 000002c0: 6448 4e62 4d46 3163 6269 4167 4943 4277  dHNbMF1cbiAgICBw
 000002d0: 6233 4a30 4c6d 3975 6257 567a 6332 466e  b3J0Lm9ubWVzc2Fn
 000002e0: 5a53 4139 4943 686c 4f69 424e 5a58 4e7a  ZSA9IChlOiBNZXNz
 000002f0: 5957 646c 5258 5a6c 626e 5170 4944 302b  YWdlRXZlbnQpID0+
 00000300: 4948 7463 6269 4167 4943 4239 5847 3563  IHtcbiAgICB9XG5c
-00000310: 626e 3163 6269 4a64 6651 3d3d 0a         bn1cbiJdfQ==.
+00000310: 626e 3163 6269 4a64 6651 3d3d            bn1cbiJdfQ==
```

### Comparing `ckanext_files-0.2.6/ckanext/files/storage/fs.py` & `ckanext_files-0.3.0/ckanext/files/storage/fs.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     )
 
     def upload(self, name, upload, extras):
         # type: (str, types.Upload, dict[str, types.Any]) -> FsStorageData
         filename = self.storage.compute_name(name, extras, upload)
         filepath = os.path.join(self.storage.settings["path"], filename)
 
+        os.makedirs(os.path.dirname(filepath), exist_ok=True)
+
         reader = HashingReader(upload.stream)
         with open(filepath, "wb") as dest:
             for chunk in reader:
                 dest.write(chunk)
 
         return {
             "filename": filename,
@@ -148,25 +150,44 @@
             "size": size,
             "hash": reader.get_hash(),
         }
 
 
 class FileSystemManager(Manager):
     required_options = ["path"]
-    capabilities = utils.combine_capabilities(Capability.REMOVE)
+    capabilities = utils.combine_capabilities(Capability.REMOVE, Capability.ANALYZE)
 
     def remove(self, data):
         # type: (dict[str, types.Any]) -> bool
         filepath = os.path.join(str(self.storage.settings["path"]), data["filename"])
         if not os.path.exists(filepath):
             return False
 
         os.remove(filepath)
         return True
 
+    def analyze(self, filename):
+        # type: (str) -> types.FsStorageData
+        """Return all details about filename."""
+        filepath = os.path.join(str(self.storage.settings["path"]), filename)
+        if not os.path.exists(filepath):
+            raise exceptions.MissingFileError(self.storage.settings["name"], filepath)
+
+        with open(filepath, "rb") as src:
+            reader = HashingReader(src)
+            content_type = magic.from_buffer(next(reader, b""), True)
+            reader.exhaust()
+
+        return {
+            "filename": filename,
+            "content_type": content_type,
+            "size": os.path.getsize(filepath),
+            "hash": reader.get_hash(),
+        }
+
 
 class FileSystemReader(Reader):
     required_options = ["path"]
     capabilities = utils.combine_capabilities(Capability.STREAM)
 
     def stream(self, data):
         # type: (dict[str, types.Any]) -> types.IO[bytes]
```

### Comparing `ckanext_files-0.2.6/ckanext/files/storage/google_cloud.py` & `ckanext_files-0.3.0/ckanext/files/storage/google_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,21 +256,29 @@
         filepath = os.path.join(str(self.storage.settings["path"]), data["filename"])
         client = self.storage.client  # type: Client
         blob = client.bucket(self.storage.settings["bucket"]).blob(filepath)
 
         try:
             exists = blob.exists()
         except Forbidden as err:
-            raise exceptions.PermissionError(type(self), "exists", str(err))
+            raise exceptions.PermissionError(  # noqa: B904
+                type(self),
+                "exists",
+                str(err),
+            )
 
         if exists:
             try:
                 blob.delete()
             except Forbidden as err:
-                raise exceptions.PermissionError(type(self), "remove", str(err))
+                raise exceptions.PermissionError(  # noqa: B904
+                    type(self),
+                    "remove",
+                    str(err),
+                )
             return True
         return False
 
 
 class GoogleCloudStorage(Storage):
     def __init__(self, **settings):
         # type: (**types.Any) -> None
```

### Comparing `ckanext_files-0.2.6/ckanext/files/storage/redis.py` & `ckanext_files-0.3.0/ckanext/files/storage/redis.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/templates/files/snippets/file_table.html` & `ckanext_files-0.3.0/ckanext/files/templates/files/snippets/file_table.html`

 * *Files 1% similar despite different names*

```diff
@@ -57,18 +57,18 @@
                         <td>
                             <div title="{{  h.time_ago_from_timestamp(file.ctime) }}" class=""file-item__creation-time>
                                 {{ h.render_datetime(file.ctime, with_hours=true) }}
                             </div>
                         </td>
                         <td>
                             {% set content_type = file.storage_data.content_type %}
-                            <div data-content-type="{{ content_type }}" class="file-item__type">
+                            <div data-content-type="{{ content_type }}" class="file-item__type" title="{{ content_type }}">
                                 {% set icon_path = h.files_content_type_icon(content_type, "amy-dark", "svg") %}
                                 {% if icon_path %}
-                                    <img alt="type icon" src="{{ icon_path }}" title="{{ content_type }}" />
+                                    <img alt="type icon" src="{{ icon_path }}"/>
                                 {% endif %}
 
                                 {{ _(h.files_humanize_content_type(file.storage_data.content_type)) }}
                             </div>
                         </td>
                         <td>
                             {{ h.localised_filesize(file.storage_data.size) }}
```

### Comparing `ckanext_files-0.2.6/ckanext/files/templates/files/snippets/uploader_v1.html` & `ckanext_files-0.3.0/ckanext/files/templates/files/snippets/uploader_v1.html`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/templates/files/user/delete.html` & `ckanext_files-0.3.0/ckanext/files/templates/files/user/delete.html`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/templates/files/user/index.html` & `ckanext_files-0.3.0/ckanext/files/templates/files/user/index.html`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/tests/conftest.py` & `ckanext_files-0.3.0/ckanext/files/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         reset_db()
         create_tables()
 
 
 class FakeFileStorage(FileStorage):
     def __init__(self, stream, filename):
         # type: (Any, str) -> None
-        super(FakeFileStorage, self).__init__(stream, filename, "uplod")
+        super(FakeFileStorage, self).__init__(stream, filename, "upload")
 
 
 @pytest.fixture
 def create_with_upload(ckan_config, monkeypatch, tmpdir):
     # type: (Any, Any, Any) -> Any
     """Reimplementation of original CKAN fixture with better fake storage.
```

### Comparing `ckanext_files-0.2.6/ckanext/files/tests/logic/test_action.py` & `ckanext_files-0.3.0/ckanext/files/tests/logic/test_action.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/tests/logic/test_validators.py` & `ckanext_files-0.3.0/ckanext/files/tests/logic/test_validators.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/tests/storage/test_fs.py` & `ckanext_files-0.3.0/ckanext/files/tests/storage/test_fs.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/tests/storage/test_google_cloud.py` & `ckanext_files-0.3.0/ckanext/files/tests/storage/test_google_cloud.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/tests/storage/test_redis.py` & `ckanext_files-0.3.0/ckanext/files/tests/storage/test_redis.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/tests/test_base.py` & `ckanext_files-0.3.0/ckanext/files/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/tests/test_config.py` & `ckanext_files-0.3.0/ckanext/files/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/tests/test_utils.py` & `ckanext_files-0.3.0/ckanext/files/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/ckanext/files/utils.py` & `ckanext_files-0.3.0/ckanext/files/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 stored here, to avoid import cycles.
 
 """
 
 import cgi
 import mimetypes
 import re
+import tempfile
 from io import BytesIO
 
 import magic
 import six
 from werkzeug.datastructures import FileStorage
 
 from ckanext.files import exceptions
@@ -186,14 +187,22 @@
     if isinstance(value, FileStorage):
         if not value.content_length:
             value.stream.seek(0, 2)
             value.headers["content-length"] = str(value.stream.tell())
             value.stream.seek(0)
         return value
 
+    if isinstance(value, tempfile.SpooledTemporaryFile):
+        mime = magic.from_buffer(value.read(1024), True)
+        value.seek(0, 2)
+        size = value.tell()
+        value.seek(0)
+
+        return FileStorage(value, "", content_type=mime, content_length=size)
+
     if isinstance(value, cgi.FieldStorage):
         if not value.filename or not value.file:
             raise ValueError(value)
 
         mime, _encoding = mimetypes.guess_type(value.filename)
         if not mime:
             mime = magic.from_buffer(value.file.read(1024), True)
@@ -209,16 +218,18 @@
             content_length=size,
         )
 
     if isinstance(value, six.text_type):
         value = value.encode()
 
     if isinstance(value, (bytes, bytearray)):
-        stream = BytesIO(value)
-        mime = magic.from_buffer(stream.read(1024), True)
-        stream.seek(0, 2)
-        size = stream.tell()
-        stream.seek(0)
+        value = BytesIO(value)
+
+    if isinstance(value, BytesIO):
+        mime = magic.from_buffer(value.read(1024), True)
+        value.seek(0, 2)
+        size = value.tell()
+        value.seek(0)
 
-        return FileStorage(stream, content_type=mime, content_length=size)
+        return FileStorage(value, content_type=mime, content_length=size)
 
     raise TypeError(type(value))
```

### Comparing `ckanext_files-0.2.6/ckanext/files/views.py` & `ckanext_files-0.3.0/ckanext/files/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 from functools import partial
 
-from ckan.logic import NotAuthorized
 from flask import Blueprint
 from flask.views import MethodView
 
 import ckan.plugins.toolkit as tk
 from ckan.lib.helpers import Page
 
 from ckanext.files import types  # isort: skip # noqa: F401
```

### Comparing `ckanext_files-0.2.6/ckanext_files.egg-info/PKG-INFO` & `ckanext_files-0.3.0/ckanext_files.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-files
-Version: 0.2.6
+Version: 0.3.0
 Home-page: https://github.com/DataShades/ckanext-files
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -53,15 +53,16 @@
 | 2.10         | yes         |
 | master       | yes         |
 
 CKAN v2.8 and v2.9 are supported by ckanext-files v0.2. Starting from v1.0 this
 extension switches to CKAN support policy of two latest CKAN releases. I.e,
 ckanext-files v1.0 supports only CKAN v2.10 and v2.11.
 
-v0.2 will not receive any new features, only bug-fixes.
+v0.* will not receive any new major features, only bug-fixes and small
+improvements.
 
 It's recommended to install the extension via pip, so you probably have all the
 requirements pinned already. If you are using GitHub version of this extension,
 stick to the vX.Y.Z tags to avoid breaking changes. Check the changelog before
 upgrading the extension.
 
 ## Installation
```

### Comparing `ckanext_files-0.2.6/ckanext_files.egg-info/SOURCES.txt` & `ckanext_files-0.3.0/ckanext_files.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 setup.cfg
 setup.py
 ckanext/__init__.py
 ckanext/file_manager/__init__.py
 ckanext/file_manager/collection.py
 ckanext/file_manager/plugin.py
 ckanext/file_manager/views.py
+ckanext/file_manager/assets/webassets.yml
+ckanext/file_manager/assets/js/fm-htmx.js
+ckanext/file_manager/templates/file_manager/list.html
+ckanext/file_manager/templates/file_manager/record.html
+ckanext/file_manager/templates/file_manager/upload_file_modal.html
+ckanext/file_manager/templates/file_manager/upload_file_modal_form.html
 ckanext/files/__init__.py
 ckanext/files/base.py
 ckanext/files/cli.py
 ckanext/files/command.py
 ckanext/files/config.py
 ckanext/files/config_declaration.yaml
 ckanext/files/exceptions.py
@@ -70,14 +76,19 @@
 ckanext/files/tests/logic/__init__.py
 ckanext/files/tests/logic/test_action.py
 ckanext/files/tests/logic/test_validators.py
 ckanext/files/tests/storage/__init__.py
 ckanext/files/tests/storage/test_fs.py
 ckanext/files/tests/storage/test_google_cloud.py
 ckanext/files/tests/storage/test_redis.py
+ckanext/files_uploader/__init__.py
+ckanext/files_uploader/plugin.py
+ckanext/files_uploader/tests/__init__.py
+ckanext/files_uploader/tests/conftest.py
+ckanext/files_uploader/tests/test_plugin.py
 ckanext_files.egg-info/PKG-INFO
 ckanext_files.egg-info/SOURCES.txt
 ckanext_files.egg-info/dependency_links.txt
 ckanext_files.egg-info/entry_points.txt
 ckanext_files.egg-info/namespace_packages.txt
 ckanext_files.egg-info/requires.txt
 ckanext_files.egg-info/top_level.txt
```

### Comparing `ckanext_files-0.2.6/pyproject.toml` & `ckanext_files-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.6/setup.cfg` & `ckanext_files-0.3.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-files
-version = 0.2.6
+version = 0.3.0
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-files
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
@@ -40,14 +40,15 @@
 	%(test)s
 gcs = 
 	google-cloud-storage
 
 [options.entry_points]
 ckan.plugins = 
 	files = ckanext.files.plugin:FilesPlugin
+	files_uploader = ckanext.files_uploader.plugin:FilesUploaderPlugin
 	file_manager = ckanext.file_manager.plugin:FileManagerPlugin
 babel.extractors = 
 	ckan = ckan.lib.extract:extract_ckan
 paste.paster_command = 
 	files = ckanext.files.command:FilesCommand
 
 [extract_messages]
```

