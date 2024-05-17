# Comparing `tmp/eox-core-9.1.0.tar.gz` & `tmp/eox-core-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eox-core-9.1.0.tar", last modified: Fri Jan 12 02:24:56 2024, max compression
+gzip compressed data, was "eox-core-9.1.1.tar", last modified: Thu Jan 25 17:00:17 2024, max compression
```

## Comparing `eox-core-9.1.0.tar` & `eox-core-9.1.1.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.087965 eox-core-9.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-12 02:24:46.000000 eox-core-9.1.0/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-12 02:24:46.000000 eox-core-9.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-12 02:24:46.000000 eox-core-9.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-01-12 02:24:56.087965 eox-core-9.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-01-12 02:24:46.000000 eox-core-9.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.067965 eox-core-9.1.0/eox_core/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.067965 eox-core-9.1.0/eox_core/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.067965 eox-core-9.1.0/eox_core/api/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.067965 eox-core-9.1.0/eox_core/api/data/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/data/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/data/v1/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7135 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/data/v1/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/data/v1/paginators.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/data/v1/routers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/data/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/data/v1/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/data/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/data/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/data/v1/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.071965 eox-core-9.1.0/eox_core/api/support/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/support/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.071965 eox-core-9.1.0/eox_core/api/support/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/support/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/support/v1/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/support/v1/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.071965 eox-core-9.1.0/eox_core/api/support/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/support/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16217 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/support/v1/tests/test_oauth_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/support/v1/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/support/v1/tests/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/support/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/support/v1/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.071965 eox-core-9.1.0/eox_core/api/task_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/task_dispatcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.071965 eox-core-9.1.0/eox_core/api/task_dispatcher/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/task_dispatcher/tests/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.071965 eox-core-9.1.0/eox_core/api/task_dispatcher/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/task_dispatcher/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/task_dispatcher/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/task_dispatcher/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.071965 eox-core-9.1.0/eox_core/api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/v1/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/v1/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.075965 eox-core-9.1.0/eox_core/api/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/v1/tests/test_coursekey.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/v1/tests/test_enrollments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/v1/tests/test_grades.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/v1/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/v1/tests/test_pre_enrollments.py
--rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/v1/tests/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    44819 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/api_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.075965 eox-core-9.1.0/eox_core/edxapp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.079965 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/bearer_authentication_j_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/bearer_authentication_j_v1_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/certificates_h_v1_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/certificates_m_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/comments_service_users_j_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/configuration_helpers_h_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/configuration_helpers_h_v1_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/coursekey_m_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/courses_h_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/courseware_h_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/edxfuture_i_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/edxfuture_o_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/enrollment_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12095 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/enrollment_o_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/grades_h_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/pre_enrollment_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/storages_i_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/storages_i_v1_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/third_party_auth_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13728 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/users_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/users_l_v1_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13787 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/users_m_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/backends/users_m_v1_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/bearer_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/comments_service_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/configuration_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/coursekey.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/courses.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/courseware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/enrollments.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/pre_enrollments.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/storages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.079965 eox-core-9.1.0/eox_core/edxapp_wrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/tests/test_coursekey.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/tests/test_enrollments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/tests/test_pre_enrollments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/tests/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/third_party_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/edxapp_wrapper/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.079965 eox-core-9.1.0/eox_core/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/integrations/sentry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.083965 eox-core-9.1.0/eox_core/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/migrations/0002_moving_contenttypes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.083965 eox-core-9.1.0/eox_core/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/settings/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/social_tpa_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.083965 eox-core-9.1.0/eox_core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.083965 eox-core-9.1.0/eox_core/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20720 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/tests/integration/test_enrollment_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/tests/integration/test_grade_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11028 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/tests/test_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-01-12 02:24:46.000000 eox-core-9.1.0/eox_core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.083965 eox-core-9.1.0/eox_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-01-12 02:24:56.000000 eox-core-9.1.0/eox_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-01-12 02:24:56.000000 eox-core-9.1.0/eox_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 02:24:56.000000 eox-core-9.1.0/eox_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-12 02:24:56.000000 eox-core-9.1.0/eox_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 02:24:55.000000 eox-core-9.1.0/eox_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-12 02:24:56.000000 eox-core-9.1.0/eox_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-12 02:24:56.000000 eox-core-9.1.0/eox_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:24:56.083965 eox-core-9.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-01-12 02:24:46.000000 eox-core-9.1.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 02:24:46.000000 eox-core-9.1.0/requirements/eox-audit-model.in
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-12 02:24:46.000000 eox-core-9.1.0/requirements/sentry.in
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-12 02:24:46.000000 eox-core-9.1.0/requirements/tpa.in
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-01-12 02:24:56.087965 eox-core-9.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-01-12 02:24:46.000000 eox-core-9.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.885875 eox-core-9.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-25 17:00:07.000000 eox-core-9.1.1/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-25 17:00:07.000000 eox-core-9.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-25 17:00:07.000000 eox-core-9.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-01-25 17:00:17.885875 eox-core-9.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-01-25 17:00:07.000000 eox-core-9.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.865875 eox-core-9.1.1/eox_core/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.869876 eox-core-9.1.1/eox_core/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.869876 eox-core-9.1.1/eox_core/api/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.869876 eox-core-9.1.1/eox_core/api/data/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/data/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/data/v1/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7135 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/data/v1/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/data/v1/paginators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/data/v1/routers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/data/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/data/v1/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/data/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/data/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/data/v1/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.869876 eox-core-9.1.1/eox_core/api/support/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/support/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.869876 eox-core-9.1.1/eox_core/api/support/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/support/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/support/v1/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/support/v1/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.869876 eox-core-9.1.1/eox_core/api/support/v1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/support/v1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16217 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/support/v1/tests/test_oauth_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/support/v1/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/support/v1/tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/support/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/support/v1/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.873875 eox-core-9.1.1/eox_core/api/task_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/task_dispatcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.873875 eox-core-9.1.1/eox_core/api/task_dispatcher/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/task_dispatcher/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.873875 eox-core-9.1.1/eox_core/api/task_dispatcher/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/task_dispatcher/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/task_dispatcher/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/task_dispatcher/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.873875 eox-core-9.1.1/eox_core/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/v1/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/v1/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.873875 eox-core-9.1.1/eox_core/api/v1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/v1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/v1/tests/test_coursekey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/v1/tests/test_enrollments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/v1/tests/test_grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/v1/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/v1/tests/test_pre_enrollments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/v1/tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44819 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/api_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.877875 eox-core-9.1.1/eox_core/edxapp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.881875 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/bearer_authentication_j_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/bearer_authentication_j_v1_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/certificates_h_v1_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/certificates_m_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/comments_service_users_j_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/configuration_helpers_h_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/configuration_helpers_h_v1_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/coursekey_m_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/courses_h_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/courseware_h_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/edxfuture_i_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/edxfuture_o_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/enrollment_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12095 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/enrollment_o_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/grades_h_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/pre_enrollment_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/storages_i_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/storages_i_v1_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/third_party_auth_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13728 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/users_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/users_l_v1_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13787 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/users_m_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/backends/users_m_v1_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/bearer_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/comments_service_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/configuration_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/coursekey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/courses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/courseware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/enrollments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/pre_enrollments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/storages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.881875 eox-core-9.1.1/eox_core/edxapp_wrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/tests/test_coursekey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/tests/test_enrollments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/tests/test_pre_enrollments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/third_party_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/edxapp_wrapper/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.881875 eox-core-9.1.1/eox_core/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/integrations/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.881875 eox-core-9.1.1/eox_core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/migrations/0002_moving_contenttypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.881875 eox-core-9.1.1/eox_core/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/settings/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/social_tpa_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.885875 eox-core-9.1.1/eox_core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.885875 eox-core-9.1.1/eox_core/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20720 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/tests/integration/test_enrollment_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/tests/integration/test_grade_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11028 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/tests/test_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-01-25 17:00:07.000000 eox-core-9.1.1/eox_core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.885875 eox-core-9.1.1/eox_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-01-25 17:00:17.000000 eox-core-9.1.1/eox_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-01-25 17:00:17.000000 eox-core-9.1.1/eox_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 17:00:17.000000 eox-core-9.1.1/eox_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-25 17:00:17.000000 eox-core-9.1.1/eox_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 17:00:17.000000 eox-core-9.1.1/eox_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-25 17:00:17.000000 eox-core-9.1.1/eox_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-25 17:00:17.000000 eox-core-9.1.1/eox_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 17:00:17.885875 eox-core-9.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-01-25 17:00:07.000000 eox-core-9.1.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 17:00:07.000000 eox-core-9.1.1/requirements/eox-audit-model.in
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-25 17:00:07.000000 eox-core-9.1.1/requirements/sentry.in
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-25 17:00:07.000000 eox-core-9.1.1/requirements/tpa.in
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-01-25 17:00:17.885875 eox-core-9.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-01-25 17:00:07.000000 eox-core-9.1.1/setup.py
```

### Comparing `eox-core-9.1.0/LICENSE.txt` & `eox-core-9.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/PKG-INFO` & `eox-core-9.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eox-core
-Version: 9.1.0
+Version: 9.1.1
 Summary: eduNEXT Openedx extensions
 Home-page: https://github.com/eduNEXT/eox-core
 Author: eduNEXT
 Author-email: contact@edunext.co
 License: AGPL
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,28 +15,28 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 Requires-Dist: django-oauth-toolkit
-Requires-Dist: edx-api-doc-tools
-Requires-Dist: django-filter
-Requires-Dist: celery
-Requires-Dist: django-waffle
-Requires-Dist: edx-opaque-keys[django]<3.0.0
-Requires-Dist: django
-Requires-Dist: django-oauth2-provider
-Requires-Dist: edx-proctoring>=2.0.1
 Requires-Dist: openedx-events
-Requires-Dist: djangorestframework
-Requires-Dist: edx-drf-extensions
 Requires-Dist: six
+Requires-Dist: django
 Requires-Dist: click
+Requires-Dist: edx-proctoring>=2.0.1
+Requires-Dist: django-oauth2-provider
+Requires-Dist: django-waffle
+Requires-Dist: edx-opaque-keys[django]<3.0.0
 Requires-Dist: social-auth-core
+Requires-Dist: djangorestframework
+Requires-Dist: celery
+Requires-Dist: edx-api-doc-tools
+Requires-Dist: django-filter
+Requires-Dist: edx-drf-extensions
 Provides-Extra: sentry
 Requires-Dist: sentry-sdk==1.5.1; extra == "sentry"
 Provides-Extra: tpa
 Requires-Dist: social-auth-core[openidconnect]; extra == "tpa"
 Provides-Extra: eox-audit
 Requires-Dist: eox-audit-model; extra == "eox-audit"
```

### Comparing `eox-core-9.1.0/README.rst` & `eox-core-9.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/data/v1/fields.py` & `eox-core-9.1.1/eox_core/api/data/v1/fields.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/data/v1/filters.py` & `eox-core-9.1.1/eox_core/api/data/v1/filters.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/data/v1/routers.py` & `eox-core-9.1.1/eox_core/api/data/v1/routers.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/data/v1/serializers.py` & `eox-core-9.1.1/eox_core/api/data/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/data/v1/tasks.py` & `eox-core-9.1.1/eox_core/api/data/v1/tasks.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/data/v1/views.py` & `eox-core-9.1.1/eox_core/api/data/v1/views.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/data/v1/viewsets.py` & `eox-core-9.1.1/eox_core/api/data/v1/viewsets.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/support/v1/permissions.py` & `eox-core-9.1.1/eox_core/api/support/v1/permissions.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/support/v1/serializers.py` & `eox-core-9.1.1/eox_core/api/support/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/support/v1/tests/test_oauth_applications.py` & `eox-core-9.1.1/eox_core/api/support/v1/tests/test_oauth_applications.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/support/v1/tests/test_permissions.py` & `eox-core-9.1.1/eox_core/api/support/v1/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/support/v1/tests/test_users.py` & `eox-core-9.1.1/eox_core/api/support/v1/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/support/v1/views.py` & `eox-core-9.1.1/eox_core/api/support/v1/views.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/task_dispatcher/tests/test_views.py` & `eox-core-9.1.1/eox_core/api/task_dispatcher/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/task_dispatcher/v1/views.py` & `eox-core-9.1.1/eox_core/api/task_dispatcher/v1/views.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/v1/permissions.py` & `eox-core-9.1.1/eox_core/api/v1/permissions.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/v1/serializers.py` & `eox-core-9.1.1/eox_core/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/v1/tests/test_coursekey.py` & `eox-core-9.1.1/eox_core/api/v1/tests/test_coursekey.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/v1/tests/test_enrollments.py` & `eox-core-9.1.1/eox_core/api/v1/tests/test_enrollments.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/v1/tests/test_grades.py` & `eox-core-9.1.1/eox_core/api/v1/tests/test_grades.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/v1/tests/test_permissions.py` & `eox-core-9.1.1/eox_core/api/v1/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/v1/tests/test_pre_enrollments.py` & `eox-core-9.1.1/eox_core/api/v1/tests/test_pre_enrollments.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/v1/tests/test_users.py` & `eox-core-9.1.1/eox_core/api/v1/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api/v1/urls.py` & `eox-core-9.1.1/eox_core/api/v1/urls.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """ urls.py """
 
 from django.conf import settings
-from django.conf.urls import url
+from django.urls import re_path
 
 from eox_core.api.v1 import views
 
 app_name = 'eox_core'  # pylint: disable=invalid-name
 
 urlpatterns = [  # pylint: disable=invalid-name
-    url(r'^user/$', views.EdxappUser.as_view(), name='edxapp-user'),
-    url(r'^enrollment/$', views.EdxappEnrollment.as_view(), name='edxapp-enrollment'),
-    url(r'^grade/$', views.EdxappGrade.as_view(), name='edxapp-grade'),
-    url(r'^pre-enrollment/$', views.EdxappPreEnrollment.as_view(), name='edxapp-pre-enrollment'),
-    url(r'^userinfo/$', views.UserInfo.as_view(), name='edxapp-userinfo'),
+    re_path(r'^user/$', views.EdxappUser.as_view(), name='edxapp-user'),
+    re_path(r'^enrollment/$', views.EdxappEnrollment.as_view(), name='edxapp-enrollment'),
+    re_path(r'^grade/$', views.EdxappGrade.as_view(), name='edxapp-grade'),
+    re_path(r'^pre-enrollment/$', views.EdxappPreEnrollment.as_view(), name='edxapp-pre-enrollment'),
+    re_path(r'^userinfo/$', views.UserInfo.as_view(), name='edxapp-userinfo'),
 ]
 
 if getattr(settings, "EOX_CORE_ENABLE_UPDATE_USERS", None):
     urlpatterns += [
-        url(r'^update-user/$', views.EdxappUserUpdater.as_view(), name='edxapp-user-updater'),
+        re_path(r'^update-user/$', views.EdxappUserUpdater.as_view(), name='edxapp-user-updater'),
     ]
```

### Comparing `eox-core-9.1.0/eox_core/api/v1/views.py` & `eox-core-9.1.1/eox_core/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/api_schema.py` & `eox-core-9.1.1/eox_core/api_schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Swagger view generator
 """
 from django.conf import settings
-from django.conf.urls import url
+from django.urls import re_path
 from drf_yasg.generators import OpenAPISchemaGenerator
 from drf_yasg.openapi import SwaggerDict
 from drf_yasg.views import get_schema_view
 from edx_api_doc_tools import get_docs_cache_timeout, make_api_info
 from rest_framework import permissions
 
 from eox_core.api.v1 import views
@@ -35,22 +35,22 @@
             },
         }
         security_definitions = SwaggerDict.as_odict(security_definitions)
         return security_definitions
 
 
 api_urls = [  # pylint: disable=invalid-name
-    url(r'^enrollment/$', views.EdxappEnrollment.as_view(), name='edxapp-enrollment'),
-    url(r'^grade/$', views.EdxappGrade.as_view(), name='edxapp-grade'),
-    url(r'^user/$', views.EdxappUser.as_view(), name='edxapp-user'),
+    re_path(r'^enrollment/$', views.EdxappEnrollment.as_view(), name='edxapp-enrollment'),
+    re_path(r'^grade/$', views.EdxappGrade.as_view(), name='edxapp-grade'),
+    re_path(r'^user/$', views.EdxappUser.as_view(), name='edxapp-user'),
 ]
 
 if getattr(settings, "EOX_CORE_ENABLE_UPDATE_USERS", None):
     api_urls += [
-        url(r'^update-user/$', views.EdxappUserUpdater.as_view(), name='edxapp-user-updater'),
+        re_path(r'^update-user/$', views.EdxappUserUpdater.as_view(), name='edxapp-user-updater'),
     ]
 
 api_info = make_api_info(  # pylint: disable=invalid-name
     title="eox core",
     version="v1",
     email=" contact@edunext.co",
     description="REST APIs to interact with edxapp",
```

### Comparing `eox-core-9.1.0/eox_core/apps.py` & `eox-core-9.1.1/eox_core/apps.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/backends/bearer_authentication_j_v1.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/backends/bearer_authentication_j_v1.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/backends/certificates_m_v1.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/backends/certificates_m_v1.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/backends/comments_service_users_j_v1.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/backends/comments_service_users_j_v1.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/backends/coursekey_m_v1.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/backends/coursekey_m_v1.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/backends/courses_h_v1.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/backends/courses_h_v1.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/backends/edxfuture_i_v1.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/backends/edxfuture_i_v1.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/backends/edxfuture_o_v1.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/backends/edxfuture_o_v1.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/backends/enrollment_l_v1.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/backends/enrollment_l_v1.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/backends/enrollment_o_v1.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/backends/enrollment_o_v1.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/backends/pre_enrollment_l_v1.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/backends/pre_enrollment_l_v1.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/backends/storages_i_v1.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/backends/storages_i_v1.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/backends/storages_i_v1_test.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/backends/storages_i_v1_test.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/backends/users_l_v1.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/backends/users_l_v1.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/backends/users_l_v1_test.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/backends/users_l_v1_test.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/backends/users_m_v1.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/backends/users_m_v1.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/backends/users_m_v1_test.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/backends/users_m_v1_test.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/certificates.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/certificates.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/coursekey.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/coursekey.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/courses.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/courses.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/enrollments.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/enrollments.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/pre_enrollments.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/pre_enrollments.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/storages.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/storages.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/tests/test_coursekey.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/tests/test_coursekey.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/tests/test_enrollments.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/tests/test_enrollments.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/tests/test_pre_enrollments.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/tests/test_pre_enrollments.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/tests/test_users.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/edxapp_wrapper/users.py` & `eox-core-9.1.1/eox_core/edxapp_wrapper/users.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/integrations/sentry.py` & `eox-core-9.1.1/eox_core/integrations/sentry.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/logging.py` & `eox-core-9.1.1/eox_core/logging.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/middleware.py` & `eox-core-9.1.1/eox_core/middleware.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/migrations/0001_initial.py` & `eox-core-9.1.1/eox_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/migrations/0002_moving_contenttypes.py` & `eox-core-9.1.1/eox_core/migrations/0002_moving_contenttypes.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/models.py` & `eox-core-9.1.1/eox_core/models.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/pipeline.py` & `eox-core-9.1.1/eox_core/pipeline.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/settings/common.py` & `eox-core-9.1.1/eox_core/settings/common.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/settings/devstack.py` & `eox-core-9.1.1/eox_core/settings/devstack.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/settings/production.py` & `eox-core-9.1.1/eox_core/settings/production.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/settings/test.py` & `eox-core-9.1.1/eox_core/settings/test.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/social_tpa_backends.py` & `eox-core-9.1.1/eox_core/social_tpa_backends.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/storage.py` & `eox-core-9.1.1/eox_core/storage.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/test_utils.py` & `eox-core-9.1.1/eox_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/tests/integration/test_enrollment_integration.py` & `eox-core-9.1.1/eox_core/tests/integration/test_enrollment_integration.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/tests/integration/test_grade_integration.py` & `eox-core-9.1.1/eox_core/tests/integration/test_grade_integration.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/tests/test_middleware.py` & `eox-core-9.1.1/eox_core/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/tests/test_models.py` & `eox-core-9.1.1/eox_core/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/tests/test_pipeline.py` & `eox-core-9.1.1/eox_core/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/tests/test_storage.py` & `eox-core-9.1.1/eox_core/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/tests/test_utils.py` & `eox-core-9.1.1/eox_core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/tests/test_views.py` & `eox-core-9.1.1/eox_core/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/tests/test_wrappers.py` & `eox-core-9.1.1/eox_core/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/urls.py` & `eox-core-9.1.1/eox_core/urls.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """ urls.py """
 
-from django.conf.urls import include, url
+from django.urls import include, re_path
 
 from eox_core import views
 from eox_core.api_schema import docs_ui_view
 
 app_name = 'eox_core'  # pylint: disable=invalid-name
 
 urlpatterns = [  # pylint: disable=invalid-name
-    url(r'^eox-info$', views.info_view),
-    url(r'^api/', include('eox_core.api.urls', namespace='eox-api')),
-    url(r'^data-api/', include('eox_core.api.data.v1.urls', namespace='eox-data-api')),
-    url(r'^api-docs/$', docs_ui_view, name='apidocs-ui'),
-    url(r'^tasks-api/', include('eox_core.api.task_dispatcher.v1.urls', namespace='eox-task-api')),
-    url(r'^support-api/', include('eox_core.api.support.urls', namespace='eox-support-api')),
+    re_path(r'^eox-info$', views.info_view),
+    re_path(r'^api/', include('eox_core.api.urls', namespace='eox-api')),
+    re_path(r'^data-api/', include('eox_core.api.data.v1.urls', namespace='eox-data-api')),
+    re_path(r'^api-docs/$', docs_ui_view, name='apidocs-ui'),
+    re_path(r'^tasks-api/', include('eox_core.api.task_dispatcher.v1.urls', namespace='eox-task-api')),
+    re_path(r'^support-api/', include('eox_core.api.support.urls', namespace='eox-support-api')),
 ]
```

### Comparing `eox-core-9.1.0/eox_core/utils.py` & `eox-core-9.1.1/eox_core/utils.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core/views.py` & `eox-core-9.1.1/eox_core/views.py`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/eox_core.egg-info/PKG-INFO` & `eox-core-9.1.1/eox_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eox-core
-Version: 9.1.0
+Version: 9.1.1
 Summary: eduNEXT Openedx extensions
 Home-page: https://github.com/eduNEXT/eox-core
 Author: eduNEXT
 Author-email: contact@edunext.co
 License: AGPL
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,28 +15,28 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 Requires-Dist: django-oauth-toolkit
-Requires-Dist: edx-api-doc-tools
-Requires-Dist: django-filter
-Requires-Dist: celery
-Requires-Dist: django-waffle
-Requires-Dist: edx-opaque-keys[django]<3.0.0
-Requires-Dist: django
-Requires-Dist: django-oauth2-provider
-Requires-Dist: edx-proctoring>=2.0.1
 Requires-Dist: openedx-events
-Requires-Dist: djangorestframework
-Requires-Dist: edx-drf-extensions
 Requires-Dist: six
+Requires-Dist: django
 Requires-Dist: click
+Requires-Dist: edx-proctoring>=2.0.1
+Requires-Dist: django-oauth2-provider
+Requires-Dist: django-waffle
+Requires-Dist: edx-opaque-keys[django]<3.0.0
 Requires-Dist: social-auth-core
+Requires-Dist: djangorestframework
+Requires-Dist: celery
+Requires-Dist: edx-api-doc-tools
+Requires-Dist: django-filter
+Requires-Dist: edx-drf-extensions
 Provides-Extra: sentry
 Requires-Dist: sentry-sdk==1.5.1; extra == "sentry"
 Provides-Extra: tpa
 Requires-Dist: social-auth-core[openidconnect]; extra == "tpa"
 Provides-Extra: eox-audit
 Requires-Dist: eox-audit-model; extra == "eox-audit"
```

### Comparing `eox-core-9.1.0/eox_core.egg-info/SOURCES.txt` & `eox-core-9.1.1/eox_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eox-core-9.1.0/setup.cfg` & `eox-core-9.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 9.1.0
+current_version = 9.1.1
 commit = False
 tag = False
 
 [bumpversion:file:eox_core/__init__.py]
 
 [tool:pytest]
 DJANGO_SETTINGS_MODULE = eox_core.settings.test
```

### Comparing `eox-core-9.1.0/setup.py` & `eox-core-9.1.1/setup.py`

 * *Files identical despite different names*

