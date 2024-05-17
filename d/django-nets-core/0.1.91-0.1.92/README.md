# Comparing `tmp/django_nets_core-0.1.91.tar.gz` & `tmp/django_nets_core-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_nets_core-0.1.91.tar", last modified: Tue May  7 18:00:00 2024, max compression
+gzip compressed data, was "django_nets_core-0.1.92.tar", last modified: Tue May  7 18:03:53 2024, max compression
```

## Comparing `django_nets_core-0.1.91.tar` & `django_nets_core-0.1.92.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/LICENSE
--rw-rw-r--   0 dev       (1001) dev       (1001)      396 2024-05-07 17:28:08.000000 django_nets_core-0.1.91/MANIFEST.in
--rw-r--r--   0 dev       (1001) dev       (1001)    14299 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)    12774 2024-05-07 17:59:28.000000 django_nets_core-0.1.91/README.rst
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/django_nets_core.egg-info/
--rw-r--r--   0 dev       (1001) dev       (1001)    14299 2024-05-07 18:00:00.000000 django_nets_core-0.1.91/django_nets_core.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)     2299 2024-05-07 18:00:00.000000 django_nets_core-0.1.91/django_nets_core.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-07 18:00:00.000000 django_nets_core-0.1.91/django_nets_core.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-07 18:00:00.000000 django_nets_core-0.1.91/django_nets_core.egg-info/requires.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-07 18:00:00.000000 django_nets_core-0.1.91/django_nets_core.egg-info/top_level.txt
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.892583 django_nets_core-0.1.91/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2440 2024-05-05 19:35:20.000000 django_nets_core-0.1.91/nets_core/admin.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      665 2024-05-07 16:47:52.000000 django_nets_core-0.1.91/nets_core/apps.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django_nets_core-0.1.91/nets_core/asgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/auth_urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django_nets_core-0.1.91/nets_core/celery.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     4901 2024-05-05 18:50:21.000000 django_nets_core-0.1.91/nets_core/decorators.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/firebase_messages.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/handlers.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2502 2024-05-07 16:19:36.000000 django_nets_core-0.1.91/nets_core/listeners.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     4460 2024-05-05 18:01:33.000000 django_nets_core-0.1.91/nets_core/mail.py
--rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/manage.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.888583 django_nets_core-0.1.91/nets_core/management/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.892583 django_nets_core-0.1.91/nets_core/management/commands/
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 02:03:24.000000 django_nets_core-0.1.91/nets_core/management/commands/__init__.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.892583 django_nets_core-0.1.91/nets_core/management/commands/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)      165 2024-05-05 02:44:07.000000 django_nets_core-0.1.91/nets_core/management/commands/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)    28055 2024-05-05 05:05:51.000000 django_nets_core-0.1.91/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)    22259 2024-05-05 19:59:37.000000 django_nets_core-0.1.91/nets_core/management/commands/nets-settings.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.892583 django_nets_core-0.1.91/nets_core/middleware/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.892583 django_nets_core-0.1.91/nets_core/middleware/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django_nets_core-0.1.91/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)     2113 2024-05-05 19:54:31.000000 django_nets_core-0.1.91/nets_core/middleware/auth_token.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/nets_core/migrations/
--rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0002_alter_verificationcode_token.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0003_userdevice.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0005_userdevice_uuid.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0006_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0007_alter_verificationcode_device.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/0009_userdevice_ip.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6844 2024-05-05 19:06:27.000000 django_nets_core-0.1.91/nets_core/migrations/0010_permission_role_userrole_and_more.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      427 2024-05-05 19:35:28.000000 django_nets_core-0.1.91/nets_core/migrations/0011_role_enabled.py
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/migrations/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)    14960 2024-05-07 17:51:02.000000 django_nets_core-0.1.91/nets_core/models.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/params.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/nets_core/procedures/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/nets_core/procedures/__pycache__/
--rw-rw-r--   0 dev       (1001) dev       (1001)     1511 2024-05-07 16:19:56.000000 django_nets_core-0.1.91/nets_core/procedures/__pycache__/create_nets_core_functions.cpython-312.pyc
--rw-rw-r--   0 dev       (1001) dev       (1001)     1607 2024-05-07 17:30:24.000000 django_nets_core-0.1.91/nets_core/procedures/__pycache__/nets_core_functions.cpython-312.pyc
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/nets_core/procedures/functions/
--rw-rw-r--   0 dev       (1001) dev       (1001)     2269 2024-05-07 17:47:54.000000 django_nets_core-0.1.91/nets_core/procedures/functions/nets_core_postgresql_model_to_json.sql
--rw-rw-r--   0 dev       (1001) dev       (1001)     1284 2024-05-07 17:33:26.000000 django_nets_core-0.1.91/nets_core/procedures/nets_core_functions.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/responses.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/security.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     2490 2024-05-07 17:24:57.000000 django_nets_core-0.1.91/nets_core/serializers.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3387 2024-05-05 18:22:43.000000 django_nets_core-0.1.91/nets_core/settings.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django_nets_core-0.1.91/nets_core/settings_nets.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      753 2024-05-05 05:16:02.000000 django_nets_core-0.1.91/nets_core/tasks.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.888583 django_nets_core-0.1.91/nets_core/templates/
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/nets_core/templates/nets_core/
--rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/templates/nets_core/base.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/templates/nets_core/delete_account.html
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 18:03:29.000000 django_nets_core-0.1.91/nets_core/templates/nets_core/delete_account_info.html
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/nets_core/templates/nets_core/email/
--rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/templates/nets_core/email/base_email.html
--rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/templates/nets_core/email/new_login.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/templates/nets_core/email/verification_code.html
--rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/urls.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     3003 2024-05-05 18:49:07.000000 django_nets_core-0.1.91/nets_core/utils.py
--rw-rw-r--   0 dev       (1001) dev       (1001)    11727 2024-05-05 18:04:42.000000 django_nets_core-0.1.91/nets_core/views.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/nets_core/wsgi.py
--rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django_nets_core-0.1.91/pyproject.toml
--rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django_nets_core-0.1.91/requirements.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-07 18:00:00.896583 django_nets_core-0.1.91/setup.cfg
--rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django_nets_core-0.1.91/setup.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:03:53.861130 django_nets_core-0.1.92/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/LICENSE
+-rw-rw-r--   0 dev       (1001) dev       (1001)      396 2024-05-07 17:28:08.000000 django_nets_core-0.1.92/MANIFEST.in
+-rw-r--r--   0 dev       (1001) dev       (1001)    14299 2024-05-07 18:03:53.861130 django_nets_core-0.1.92/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)    12774 2024-05-07 17:59:28.000000 django_nets_core-0.1.92/README.rst
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:03:53.861130 django_nets_core-0.1.92/django_nets_core.egg-info/
+-rw-r--r--   0 dev       (1001) dev       (1001)    14299 2024-05-07 18:03:53.000000 django_nets_core-0.1.92/django_nets_core.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2388 2024-05-07 18:03:53.000000 django_nets_core-0.1.92/django_nets_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-05-07 18:03:53.000000 django_nets_core-0.1.92/django_nets_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)      286 2024-05-07 18:03:53.000000 django_nets_core-0.1.92/django_nets_core.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       10 2024-05-07 18:03:53.000000 django_nets_core-0.1.92/django_nets_core.egg-info/top_level.txt
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:03:53.857130 django_nets_core-0.1.92/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2440 2024-05-05 19:35:20.000000 django_nets_core-0.1.92/nets_core/admin.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      665 2024-05-07 16:47:52.000000 django_nets_core-0.1.92/nets_core/apps.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      807 2024-05-05 05:05:51.000000 django_nets_core-0.1.92/nets_core/asgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      537 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/auth_urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      229 2024-05-05 05:05:51.000000 django_nets_core-0.1.92/nets_core/celery.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     4901 2024-05-05 18:50:21.000000 django_nets_core-0.1.92/nets_core/decorators.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3276 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/firebase_messages.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6465 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/handlers.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2502 2024-05-07 16:19:36.000000 django_nets_core-0.1.92/nets_core/listeners.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     4460 2024-05-05 18:01:33.000000 django_nets_core-0.1.92/nets_core/mail.py
+-rwxrwxr-x   0 dev       (1001) dev       (1001)      665 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/manage.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:03:53.853130 django_nets_core-0.1.92/nets_core/management/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:03:53.857130 django_nets_core-0.1.92/nets_core/management/commands/
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 02:03:24.000000 django_nets_core-0.1.92/nets_core/management/commands/__init__.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:03:53.857130 django_nets_core-0.1.92/nets_core/management/commands/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)      165 2024-05-05 02:44:07.000000 django_nets_core-0.1.92/nets_core/management/commands/__pycache__/__init__.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)    28055 2024-05-05 05:05:51.000000 django_nets_core-0.1.92/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)    22259 2024-05-05 19:59:37.000000 django_nets_core-0.1.92/nets_core/management/commands/nets-settings.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:03:53.857130 django_nets_core-0.1.92/nets_core/middleware/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:03:53.857130 django_nets_core-0.1.92/nets_core/middleware/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3004 2024-05-05 04:39:30.000000 django_nets_core-0.1.92/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2113 2024-05-05 19:54:31.000000 django_nets_core-0.1.92/nets_core/middleware/auth_token.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:03:53.857130 django_nets_core-0.1.92/nets_core/migrations/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     5274 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      422 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/migrations/0002_alter_verificationcode_token.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2208 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/migrations/0003_userdevice.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      360 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/migrations/0004_remove_userdevice_device_id_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      480 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/migrations/0005_userdevice_uuid.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      454 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/migrations/0006_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      533 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/migrations/0007_alter_verificationcode_device.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2056 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      455 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/migrations/0009_userdevice_ip.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6844 2024-05-05 19:06:27.000000 django_nets_core-0.1.92/nets_core/migrations/0010_permission_role_userrole_and_more.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      427 2024-05-05 19:35:28.000000 django_nets_core-0.1.92/nets_core/migrations/0011_role_enabled.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1939 2024-05-07 18:03:37.000000 django_nets_core-0.1.92/nets_core/migrations/0012_permission_created_permission_updated_role_created_and_more.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/migrations/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)    15007 2024-05-07 18:02:49.000000 django_nets_core-0.1.92/nets_core/models.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6425 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/params.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:03:53.857130 django_nets_core-0.1.92/nets_core/procedures/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:03:53.857130 django_nets_core-0.1.92/nets_core/procedures/__pycache__/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1511 2024-05-07 16:19:56.000000 django_nets_core-0.1.92/nets_core/procedures/__pycache__/create_nets_core_functions.cpython-312.pyc
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1829 2024-05-07 18:02:54.000000 django_nets_core-0.1.92/nets_core/procedures/__pycache__/nets_core_functions.cpython-312.pyc
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:03:53.857130 django_nets_core-0.1.92/nets_core/procedures/functions/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2269 2024-05-07 17:47:54.000000 django_nets_core-0.1.92/nets_core/procedures/functions/nets_core_postgresql_model_to_json.sql
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1284 2024-05-07 17:33:26.000000 django_nets_core-0.1.92/nets_core/procedures/nets_core_functions.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      902 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/responses.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3055 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/security.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2490 2024-05-07 17:24:57.000000 django_nets_core-0.1.92/nets_core/serializers.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3387 2024-05-05 18:22:43.000000 django_nets_core-0.1.92/nets_core/settings.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1820 2024-05-05 05:05:51.000000 django_nets_core-0.1.92/nets_core/settings_nets.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      753 2024-05-05 05:16:02.000000 django_nets_core-0.1.92/nets_core/tasks.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:03:53.853130 django_nets_core-0.1.92/nets_core/templates/
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:03:53.861130 django_nets_core-0.1.92/nets_core/templates/nets_core/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     6978 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/templates/nets_core/base.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1954 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/templates/nets_core/delete_account.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-05-05 18:03:29.000000 django_nets_core-0.1.92/nets_core/templates/nets_core/delete_account_info.html
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-05-07 18:03:53.861130 django_nets_core-0.1.92/nets_core/templates/nets_core/email/
+-rw-rw-r--   0 dev       (1001) dev       (1001)    16103 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/templates/nets_core/email/base_email.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1032 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/templates/nets_core/email/new_login.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      316 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/templates/nets_core/email/verification_code.html
+-rw-rw-r--   0 dev       (1001) dev       (1001)      824 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/urls.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     3003 2024-05-05 18:49:07.000000 django_nets_core-0.1.92/nets_core/utils.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)    11727 2024-05-05 18:04:42.000000 django_nets_core-0.1.92/nets_core/views.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      395 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/nets_core/wsgi.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)      100 2024-05-05 00:47:40.000000 django_nets_core-0.1.92/pyproject.toml
+-rw-rw-r--   0 dev       (1001) dev       (1001)      181 2024-05-05 01:49:02.000000 django_nets_core-0.1.92/requirements.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1334 2024-05-07 18:03:53.861130 django_nets_core-0.1.92/setup.cfg
+-rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-05-04 23:43:26.000000 django_nets_core-0.1.92/setup.py
```

### Comparing `django_nets_core-0.1.91/PKG-INFO` & `django_nets_core-0.1.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nets-core
-Version: 0.1.91
+Version: 0.1.92
 Summary: A lazy API rest request handler.
 Home-page: https://github.com/esbozos/django-nets-core
 Author: Norman Torres
 Author-email: norman.nets@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_nets_core-0.1.91/README.rst` & `django_nets_core-0.1.92/README.rst`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/django_nets_core.egg-info/PKG-INFO` & `django_nets_core-0.1.92/django_nets_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nets-core
-Version: 0.1.91
+Version: 0.1.92
 Summary: A lazy API rest request handler.
 Home-page: https://github.com/esbozos/django-nets-core
 Author: Norman Torres
 Author-email: norman.nets@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_nets_core-0.1.91/django_nets_core.egg-info/SOURCES.txt` & `django_nets_core-0.1.92/django_nets_core.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 nets_core/migrations/0005_userdevice_uuid.py
 nets_core/migrations/0006_verificationcode_device.py
 nets_core/migrations/0007_alter_verificationcode_device.py
 nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py
 nets_core/migrations/0009_userdevice_ip.py
 nets_core/migrations/0010_permission_role_userrole_and_more.py
 nets_core/migrations/0011_role_enabled.py
+nets_core/migrations/0012_permission_created_permission_updated_role_created_and_more.py
 nets_core/migrations/__init__.py
 nets_core/procedures/nets_core_functions.py
 nets_core/procedures/__pycache__/create_nets_core_functions.cpython-312.pyc
 nets_core/procedures/__pycache__/nets_core_functions.cpython-312.pyc
 nets_core/procedures/functions/nets_core_postgresql_model_to_json.sql
 nets_core/templates/nets_core/base.html
 nets_core/templates/nets_core/delete_account.html
```

### Comparing `django_nets_core-0.1.91/nets_core/admin.py` & `django_nets_core-0.1.92/nets_core/admin.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/apps.py` & `django_nets_core-0.1.92/nets_core/apps.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/asgi.py` & `django_nets_core-0.1.92/nets_core/asgi.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/auth_urls.py` & `django_nets_core-0.1.92/nets_core/auth_urls.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/decorators.py` & `django_nets_core-0.1.92/nets_core/decorators.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/firebase_messages.py` & `django_nets_core-0.1.92/nets_core/firebase_messages.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/handlers.py` & `django_nets_core-0.1.92/nets_core/handlers.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/listeners.py` & `django_nets_core-0.1.92/nets_core/listeners.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/mail.py` & `django_nets_core-0.1.92/nets_core/mail.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/manage.py` & `django_nets_core-0.1.92/nets_core/manage.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc` & `django_nets_core-0.1.92/nets_core/management/commands/__pycache__/nets-settings.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/management/commands/nets-settings.py` & `django_nets_core-0.1.92/nets_core/management/commands/nets-settings.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc` & `django_nets_core-0.1.92/nets_core/middleware/__pycache__/auth_token.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/middleware/auth_token.py` & `django_nets_core-0.1.92/nets_core/middleware/auth_token.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/migrations/0001_initial.py` & `django_nets_core-0.1.92/nets_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/migrations/0003_userdevice.py` & `django_nets_core-0.1.92/nets_core/migrations/0003_userdevice.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/migrations/0007_alter_verificationcode_device.py` & `django_nets_core-0.1.92/nets_core/migrations/0007_alter_verificationcode_device.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py` & `django_nets_core-0.1.92/nets_core/migrations/0008_verificationcode_ip_userfirebasenotification.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/migrations/0010_permission_role_userrole_and_more.py` & `django_nets_core-0.1.92/nets_core/migrations/0010_permission_role_userrole_and_more.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/models.py` & `django_nets_core-0.1.92/nets_core/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,25 +72,25 @@
         if not isinstance(fields, tuple):
             raise ValueError(_("Fields must be a tuple"))
         
         from nets_core.serializers import NetsCoreModelToJson
         return NetsCoreModelToJson(self, fields).to_json()
 
 
-class OwnedModel(models.Model):
+class OwnedModel(NetsCoreBaseModel):
     user = models.ForeignKey(User, on_delete=models.CASCADE)
     created = models.DateTimeField(_('Created'), auto_now_add=True)
     updated = models.DateTimeField(_('updated'), auto_now=True)
     
     objects = NetsCoreBaseManager()
 
     class Meta:
         abstract = True
 
-class Permission(models.Model):
+class Permission(NetsCoreBaseModel):
     name = models.CharField(_("Name"), max_length=150)
     codename = models.CharField(_("Codename"), max_length=150)
     description = models.CharField(_("Description"), max_length=250, null=True, blank=True)
     project_content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE, null=True, blank=True, related_name='nets_core_permissions')
     project_id = models.PositiveIntegerField(null=True, blank=True)
     project = GenericForeignKey('project_content_type', 'project_id')
     
@@ -112,15 +112,15 @@
     def save(self, *args, **kwargs):
         self.codename = self.codename.lower()
         if not self.name:
             self.name = self.codename
             
         super(Permission, self).save(*args, **kwargs)
         
-class Role(models.Model):
+class Role(NetsCoreBaseModel):
     name = models.CharField(_("Name"), max_length=150)
     codename = models.CharField(_("Codename"), max_length=150)
     description = models.CharField(_("Description"), max_length=250)
     permissions = models.ManyToManyField(Permission, related_name='roles')
     project_content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE, null=True, blank=True)
     project_id = models.PositiveIntegerField(null=True, blank=True)
     project = GenericForeignKey('project_content_type', 'project_id')
@@ -141,16 +141,16 @@
             return f'{self.name} - {self.project}'
         return self.name
         
     def save(self, *args, **kwargs):
         self.codename = self.codename.lower()
         super(Role, self).save(*args, **kwargs)
         
-class UserRole(models.Model):
-    user = models.ForeignKey(User, on_delete=models.CASCADE)
+class UserRole(NetsCoreBaseModel):
+    user = models.ForeignKey(User, on_delete=models.CASCADE, related_name='roles')
     role = models.ForeignKey(Role, on_delete=models.CASCADE)
     project_content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE, null=True, blank=True)
     project_id = models.PositiveIntegerField(null=True, blank=True)
     project = GenericForeignKey('project_content_type', 'project_id')
 
     objects = NetsCoreBaseManager()
     
@@ -291,15 +291,15 @@
         indexes = [
             models.Index(fields=['project_content_type', 'project_id'], name='custom_email_index')
         ]
 
     def __str__(self):
         return self.subject
 
-class EmailNotification(models.Model):
+class EmailNotification(NetsCoreBaseModel):
     subject = models.CharField(_("subject"), max_length=250)
     to = models.TextField(_("To Email"), max_length=250)
     from_email = models.CharField(_("From Email"), max_length=250)
     body = models.TextField(_("HTML Body"))
     txt_body = models.TextField(_("TXT Body"), null=True, blank=True)
     sent = models.BooleanField(_("sent"), default=False)
     tries = models.IntegerField(_("tries"), default=0)
```

### Comparing `django_nets_core-0.1.91/nets_core/params.py` & `django_nets_core-0.1.92/nets_core/params.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/procedures/__pycache__/create_nets_core_functions.cpython-312.pyc` & `django_nets_core-0.1.92/nets_core/procedures/__pycache__/create_nets_core_functions.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/procedures/functions/nets_core_postgresql_model_to_json.sql` & `django_nets_core-0.1.92/nets_core/procedures/functions/nets_core_postgresql_model_to_json.sql`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/procedures/nets_core_functions.py` & `django_nets_core-0.1.92/nets_core/procedures/nets_core_functions.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/responses.py` & `django_nets_core-0.1.92/nets_core/responses.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/security.py` & `django_nets_core-0.1.92/nets_core/security.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/serializers.py` & `django_nets_core-0.1.92/nets_core/serializers.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/settings.py` & `django_nets_core-0.1.92/nets_core/settings.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/settings_nets.py` & `django_nets_core-0.1.92/nets_core/settings_nets.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/tasks.py` & `django_nets_core-0.1.92/nets_core/tasks.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/templates/nets_core/base.html` & `django_nets_core-0.1.92/nets_core/templates/nets_core/base.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/templates/nets_core/delete_account.html` & `django_nets_core-0.1.92/nets_core/templates/nets_core/delete_account.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/templates/nets_core/email/base_email.html` & `django_nets_core-0.1.92/nets_core/templates/nets_core/email/base_email.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/templates/nets_core/email/new_login.html` & `django_nets_core-0.1.92/nets_core/templates/nets_core/email/new_login.html`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/urls.py` & `django_nets_core-0.1.92/nets_core/urls.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/utils.py` & `django_nets_core-0.1.92/nets_core/utils.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/nets_core/views.py` & `django_nets_core-0.1.92/nets_core/views.py`

 * *Files identical despite different names*

### Comparing `django_nets_core-0.1.91/setup.cfg` & `django_nets_core-0.1.92/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-nets-core
-version = 0.1.91
+version = 0.1.92
 description = A lazy API rest request handler.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/esbozos/django-nets-core
 author = Norman Torres
 author_email = norman.nets@gmail.com
 license = BSD-3-Clause
```

