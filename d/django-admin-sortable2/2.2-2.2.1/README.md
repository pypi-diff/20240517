# Comparing `tmp/django_admin_sortable2-2.2.tar.gz` & `tmp/django_admin_sortable2-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_admin_sortable2-2.2.tar", last modified: Wed May 15 15:08:57 2024, max compression
+gzip compressed data, was "django_admin_sortable2-2.2.1.tar", last modified: Fri May 17 07:14:38 2024, max compression
```

## Comparing `django_admin_sortable2-2.2.tar` & `django_admin_sortable2-2.2.1.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.264046 django_admin_sortable2-2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-15 15:08:57.264046 django_admin_sortable2-2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.256045 django_admin_sortable2-2.2/adminsortable2/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22603 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.256045 django_admin_sortable2-2.2/adminsortable2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.252045 django_admin_sortable2-2.2/adminsortable2/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.256045 django_admin_sortable2-2.2/adminsortable2/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.252045 django_admin_sortable2-2.2/adminsortable2/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.256045 django_admin_sortable2-2.2/adminsortable2/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.252045 django_admin_sortable2-2.2/adminsortable2/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.260046 django_admin_sortable2-2.2/adminsortable2/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.252045 django_admin_sortable2-2.2/adminsortable2/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.260046 django_admin_sortable2-2.2/adminsortable2/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.252045 django_admin_sortable2-2.2/adminsortable2/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.260046 django_admin_sortable2-2.2/adminsortable2/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.252045 django_admin_sortable2-2.2/adminsortable2/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.260046 django_admin_sortable2-2.2/adminsortable2/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.256045 django_admin_sortable2-2.2/adminsortable2/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.260046 django_admin_sortable2-2.2/adminsortable2/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.256045 django_admin_sortable2-2.2/adminsortable2/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.260046 django_admin_sortable2-2.2/adminsortable2/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.260046 django_admin_sortable2-2.2/adminsortable2/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.260046 django_admin_sortable2-2.2/adminsortable2/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/management/commands/reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.256045 django_admin_sortable2-2.2/adminsortable2/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.256045 django_admin_sortable2-2.2/adminsortable2/static/adminsortable2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.260046 django_admin_sortable2-2.2/adminsortable2/static/adminsortable2/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/static/adminsortable2/css/sortable.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.260046 django_admin_sortable2-2.2/adminsortable2/static/adminsortable2/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/static/adminsortable2/icons/drag.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.260046 django_admin_sortable2-2.2/adminsortable2/static/adminsortable2/js/
--rw-r--r--   0 runner    (1001) docker     (127)    50264 2024-05-15 15:08:51.000000 django_admin_sortable2-2.2/adminsortable2/static/adminsortable2/js/adminsortable2.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.256045 django_admin_sortable2-2.2/adminsortable2/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.260046 django_admin_sortable2-2.2/adminsortable2/templates/adminsortable2/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/adminsortable2/templates/adminsortable2/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.264046 django_admin_sortable2-2.2/adminsortable2/templates/adminsortable2/edit_inline/
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-15 15:08:52.000000 django_admin_sortable2-2.2/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.2.html
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-15 15:08:52.000000 django_admin_sortable2-2.2/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-5.0.html
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-15 15:08:52.000000 django_admin_sortable2-2.2/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-15 15:08:52.000000 django_admin_sortable2-2.2/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html.orig
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-15 15:08:52.000000 django_admin_sortable2-2.2/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-5.0.html
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-15 15:08:52.000000 django_admin_sortable2-2.2/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-5.0.html.orig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:08:57.264046 django_admin_sortable2-2.2/django_admin_sortable2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-15 15:08:57.000000 django_admin_sortable2-2.2/django_admin_sortable2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-15 15:08:57.000000 django_admin_sortable2-2.2/django_admin_sortable2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:08:57.000000 django_admin_sortable2-2.2/django_admin_sortable2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:08:57.000000 django_admin_sortable2-2.2/django_admin_sortable2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 15:08:57.000000 django_admin_sortable2-2.2/django_admin_sortable2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 15:08:57.000000 django_admin_sortable2-2.2/django_admin_sortable2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:08:57.264046 django_admin_sortable2-2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-15 15:08:47.000000 django_admin_sortable2-2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.915003 django_admin_sortable2-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-17 07:14:38.915003 django_admin_sortable2-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.911003 django_admin_sortable2-2.2.1/adminsortable2/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22603 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.907003 django_admin_sortable2-2.2.1/adminsortable2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.907003 django_admin_sortable2-2.2.1/adminsortable2/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.911003 django_admin_sortable2-2.2.1/adminsortable2/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.907003 django_admin_sortable2-2.2.1/adminsortable2/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.911003 django_admin_sortable2-2.2.1/adminsortable2/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.907003 django_admin_sortable2-2.2.1/adminsortable2/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.911003 django_admin_sortable2-2.2.1/adminsortable2/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.907003 django_admin_sortable2-2.2.1/adminsortable2/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.911003 django_admin_sortable2-2.2.1/adminsortable2/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.907003 django_admin_sortable2-2.2.1/adminsortable2/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.911003 django_admin_sortable2-2.2.1/adminsortable2/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.907003 django_admin_sortable2-2.2.1/adminsortable2/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.911003 django_admin_sortable2-2.2.1/adminsortable2/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.907003 django_admin_sortable2-2.2.1/adminsortable2/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.911003 django_admin_sortable2-2.2.1/adminsortable2/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.907003 django_admin_sortable2-2.2.1/adminsortable2/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.911003 django_admin_sortable2-2.2.1/adminsortable2/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.911003 django_admin_sortable2-2.2.1/adminsortable2/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.911003 django_admin_sortable2-2.2.1/adminsortable2/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/management/commands/reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.907003 django_admin_sortable2-2.2.1/adminsortable2/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.907003 django_admin_sortable2-2.2.1/adminsortable2/static/adminsortable2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.911003 django_admin_sortable2-2.2.1/adminsortable2/static/adminsortable2/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/static/adminsortable2/css/sortable.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.911003 django_admin_sortable2-2.2.1/adminsortable2/static/adminsortable2/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/static/adminsortable2/icons/drag.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.915003 django_admin_sortable2-2.2.1/adminsortable2/static/adminsortable2/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   116253 2024-05-17 07:14:33.000000 django_admin_sortable2-2.2.1/adminsortable2/static/adminsortable2/js/adminsortable2.js
+-rw-r--r--   0 runner    (1001) docker     (127)    50264 2024-05-17 07:14:32.000000 django_admin_sortable2-2.2.1/adminsortable2/static/adminsortable2/js/adminsortable2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.907003 django_admin_sortable2-2.2.1/adminsortable2/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.915003 django_admin_sortable2-2.2.1/adminsortable2/templates/adminsortable2/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/adminsortable2/templates/adminsortable2/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.915003 django_admin_sortable2-2.2.1/adminsortable2/templates/adminsortable2/edit_inline/
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-17 07:14:33.000000 django_admin_sortable2-2.2.1/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.2.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-17 07:14:34.000000 django_admin_sortable2-2.2.1/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-5.0.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-17 07:14:33.000000 django_admin_sortable2-2.2.1/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-17 07:14:33.000000 django_admin_sortable2-2.2.1/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html.orig
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-17 07:14:34.000000 django_admin_sortable2-2.2.1/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-5.0.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-17 07:14:34.000000 django_admin_sortable2-2.2.1/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-5.0.html.orig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:14:38.915003 django_admin_sortable2-2.2.1/django_admin_sortable2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-17 07:14:38.000000 django_admin_sortable2-2.2.1/django_admin_sortable2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-17 07:14:38.000000 django_admin_sortable2-2.2.1/django_admin_sortable2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 07:14:38.000000 django_admin_sortable2-2.2.1/django_admin_sortable2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 07:14:38.000000 django_admin_sortable2-2.2.1/django_admin_sortable2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 07:14:38.000000 django_admin_sortable2-2.2.1/django_admin_sortable2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 07:14:38.000000 django_admin_sortable2-2.2.1/django_admin_sortable2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 07:14:38.915003 django_admin_sortable2-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-17 07:14:28.000000 django_admin_sortable2-2.2.1/setup.py
```

### Comparing `django_admin_sortable2-2.2/LICENSE` & `django_admin_sortable2-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/PKG-INFO` & `django_admin_sortable2-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-sortable2
-Version: 2.2
+Version: 2.2.1
 Summary: Generic drag-and-drop sorting for the List, the Stacked- and the Tabular-Inlines Views in the Django Admin
 Home-page: https://github.com/jrief/django-admin-sortable2
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: django
 Platform: OS Independent
@@ -16,17 +16,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=4.2
 
 # django-admin-sortable2
```

### Comparing `django_admin_sortable2-2.2/README.md` & `django_admin_sortable2-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/admin.py` & `django_admin_sortable2-2.2.1/adminsortable2/admin.py`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/locale/de/LC_MESSAGES/django.mo` & `django_admin_sortable2-2.2.1/adminsortable2/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/locale/de/LC_MESSAGES/django.po` & `django_admin_sortable2-2.2.1/adminsortable2/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/locale/en/LC_MESSAGES/django.po` & `django_admin_sortable2-2.2.1/adminsortable2/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/locale/es/LC_MESSAGES/django.mo` & `django_admin_sortable2-2.2.1/adminsortable2/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/locale/es/LC_MESSAGES/django.po` & `django_admin_sortable2-2.2.1/adminsortable2/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/locale/fr/LC_MESSAGES/django.mo` & `django_admin_sortable2-2.2.1/adminsortable2/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/locale/fr/LC_MESSAGES/django.po` & `django_admin_sortable2-2.2.1/adminsortable2/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/locale/it/LC_MESSAGES/django.mo` & `django_admin_sortable2-2.2.1/adminsortable2/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/locale/it/LC_MESSAGES/django.po` & `django_admin_sortable2-2.2.1/adminsortable2/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/locale/pl/LC_MESSAGES/django.mo` & `django_admin_sortable2-2.2.1/adminsortable2/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/locale/pl/LC_MESSAGES/django.po` & `django_admin_sortable2-2.2.1/adminsortable2/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/locale/ru/LC_MESSAGES/django.mo` & `django_admin_sortable2-2.2.1/adminsortable2/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/locale/ru/LC_MESSAGES/django.po` & `django_admin_sortable2-2.2.1/adminsortable2/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/locale/uk/LC_MESSAGES/django.mo` & `django_admin_sortable2-2.2.1/adminsortable2/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/locale/uk/LC_MESSAGES/django.po` & `django_admin_sortable2-2.2.1/adminsortable2/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/management/commands/reorder.py` & `django_admin_sortable2-2.2.1/adminsortable2/management/commands/reorder.py`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/static/adminsortable2/css/sortable.css` & `django_admin_sortable2-2.2.1/adminsortable2/static/adminsortable2/css/sortable.css`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/static/adminsortable2/icons/drag.png` & `django_admin_sortable2-2.2.1/adminsortable2/static/adminsortable2/icons/drag.png`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/static/adminsortable2/js/adminsortable2.min.js` & `django_admin_sortable2-2.2.1/adminsortable2/static/adminsortable2/js/adminsortable2.min.js`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.2.html` & `django_admin_sortable2-2.2.1/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.2.html`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-5.0.html` & `django_admin_sortable2-2.2.1/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-5.0.html`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html` & `django_admin_sortable2-2.2.1/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html.orig` & `django_admin_sortable2-2.2.1/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html.orig`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-5.0.html` & `django_admin_sortable2-2.2.1/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-5.0.html`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-5.0.html.orig` & `django_admin_sortable2-2.2.1/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-5.0.html.orig`

 * *Files identical despite different names*

### Comparing `django_admin_sortable2-2.2/django_admin_sortable2.egg-info/PKG-INFO` & `django_admin_sortable2-2.2.1/django_admin_sortable2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-sortable2
-Version: 2.2
+Version: 2.2.1
 Summary: Generic drag-and-drop sorting for the List, the Stacked- and the Tabular-Inlines Views in the Django Admin
 Home-page: https://github.com/jrief/django-admin-sortable2
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: django
 Platform: OS Independent
@@ -16,17 +16,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=4.2
 
 # django-admin-sortable2
```

### Comparing `django_admin_sortable2-2.2/django_admin_sortable2.egg-info/SOURCES.txt` & `django_admin_sortable2-2.2.1/django_admin_sortable2.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 adminsortable2/locale/uk/LC_MESSAGES/django.mo
 adminsortable2/locale/uk/LC_MESSAGES/django.po
 adminsortable2/management/__init__.py
 adminsortable2/management/commands/__init__.py
 adminsortable2/management/commands/reorder.py
 adminsortable2/static/adminsortable2/css/sortable.css
 adminsortable2/static/adminsortable2/icons/drag.png
+adminsortable2/static/adminsortable2/js/adminsortable2.js
 adminsortable2/static/adminsortable2/js/adminsortable2.min.js
 adminsortable2/templates/adminsortable2/change_list.html
 adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.2.html
 adminsortable2/templates/adminsortable2/edit_inline/stacked-django-5.0.html
 adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html
 adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html.orig
 adminsortable2/templates/adminsortable2/edit_inline/tabular-django-5.0.html
```

### Comparing `django_admin_sortable2-2.2/setup.py` & `django_admin_sortable2-2.2.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,17 +20,16 @@
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Topic :: Software Development :: Libraries :: Application Frameworks',
     'Development Status :: 5 - Production/Stable',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
     'Framework :: Django',
-    'Framework :: Django :: 4.0',
-    'Framework :: Django :: 4.1',
     'Framework :: Django :: 4.2',
     'Framework :: Django :: 5.0',
 ]
 
 
 setup(
     name='django-admin-sortable2',
```

