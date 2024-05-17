# Comparing `tmp/django-filer-3.1.0.tar.gz` & `tmp/django-filer-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-filer-3.1.0.tar", last modified: Mon Oct  2 14:10:19 2023, max compression
+gzip compressed data, was "django-filer-3.1.1.tar", last modified: Sat Nov 18 00:48:31 2023, max compression
```

## Comparing `django-filer-3.1.0.tar` & `django-filer-3.1.1.tar`

### file list

```diff
@@ -1,379 +1,379 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.984335 django-filer-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2023-10-02 14:10:10.000000 django-filer-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-10-02 14:10:10.000000 django-filer-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2023-10-02 14:10:19.984335 django-filer-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2023-10-02 14:10:10.000000 django-filer-3.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.948334 django-filer-3.1.0/django_filer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2023-10-02 14:10:19.000000 django-filer-3.1.0/django_filer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10577 2023-10-02 14:10:19.000000 django-filer-3.1.0/django_filer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-02 14:10:19.000000 django-filer-3.1.0/django_filer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-02 14:10:19.000000 django-filer-3.1.0/django_filer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-10-02 14:10:19.000000 django-filer-3.1.0/django_filer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-02 14:10:19.000000 django-filer-3.1.0/django_filer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.948334 django-filer-3.1.0/filer/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.952334 django-filer-3.1.0/filer/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/admin/clipboardadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/admin/fileadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)    57507 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/admin/folderadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/admin/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/admin/imageadmin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.952334 django-filer-3.1.0/filer/admin/patched/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/admin/patched/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/admin/patched/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/admin/permissionadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/admin/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/admin/thumbnailoptionadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/admin/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/admin/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.952334 django-filer-3.1.0/filer/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.952334 django-filer-3.1.0/filer/contrib/django_cms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/contrib/django_cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/contrib/django_cms/cms_toolbars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.952334 django-filer-3.1.0/filer/fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/fields/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/fields/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/fields/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/fields/multistorage_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.952334 django-filer-3.1.0/filer/locale/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/README
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.952334 django-filer-3.1.0/filer/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    31860 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.952334 django-filer-3.1.0/filer/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    31357 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.952334 django-filer-3.1.0/filer/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    16627 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    37796 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.952334 django-filer-3.1.0/filer/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    16442 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    37921 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.956334 django-filer-3.1.0/filer/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    21636 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    40821 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.956334 django-filer-3.1.0/filer/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    15724 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    37565 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.956334 django-filer-3.1.0/filer/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    20427 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    40120 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.956334 django-filer-3.1.0/filer/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    32775 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.956334 django-filer-3.1.0/filer/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11064 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    35351 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.956334 django-filer-3.1.0/filer/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    32039 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.956334 django-filer-3.1.0/filer/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    16713 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    37702 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.956334 django-filer-3.1.0/filer/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    22139 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    41417 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/gl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.956334 django-filer-3.1.0/filer/locale/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/gl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    32570 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.956334 django-filer-3.1.0/filer/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    14347 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    37819 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.956334 django-filer-3.1.0/filer/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13374 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    36804 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.956334 django-filer-3.1.0/filer/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    16819 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    37928 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.956334 django-filer-3.1.0/filer/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    17229 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    38419 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.960335 django-filer-3.1.0/filer/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    31244 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.960335 django-filer-3.1.0/filer/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    31258 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/ja_JP/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.940334 django-filer-3.1.0/filer/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.960335 django-filer-3.1.0/filer/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    17336 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    38492 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.944334 django-filer-3.1.0/filer/locale/lt_LT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.960335 django-filer-3.1.0/filer/locale/lt_LT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/lt_LT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    31723 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/lt_LT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.944334 django-filer-3.1.0/filer/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.960335 django-filer-3.1.0/filer/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    36063 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.944334 django-filer-3.1.0/filer/locale/nl_NL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.960335 django-filer-3.1.0/filer/locale/nl_NL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    21260 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/nl_NL/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    40425 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/nl_NL/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.944334 django-filer-3.1.0/filer/locale/nn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.960335 django-filer-3.1.0/filer/locale/nn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12594 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/nn/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    35986 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/nn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.944334 django-filer-3.1.0/filer/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.960335 django-filer-3.1.0/filer/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    17155 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    38530 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.944334 django-filer-3.1.0/filer/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.960335 django-filer-3.1.0/filer/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    31517 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.944334 django-filer-3.1.0/filer/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.960335 django-filer-3.1.0/filer/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    17504 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    38699 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.944334 django-filer-3.1.0/filer/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.960335 django-filer-3.1.0/filer/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    21137 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    42458 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.944334 django-filer-3.1.0/filer/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.960335 django-filer-3.1.0/filer/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    31642 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.944334 django-filer-3.1.0/filer/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.960335 django-filer-3.1.0/filer/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    33878 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.944334 django-filer-3.1.0/filer/locale/vi_VN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.964335 django-filer-3.1.0/filer/locale/vi_VN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18089 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/vi_VN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    38933 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/vi_VN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.944334 django-filer-3.1.0/filer/locale/zh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.964335 django-filer-3.1.0/filer/locale/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    31243 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.944334 django-filer-3.1.0/filer/locale/zh-Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.964335 django-filer-3.1.0/filer/locale/zh-Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    15264 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/zh-Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    35527 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/zh-Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.944334 django-filer-3.1.0/filer/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.964335 django-filer-3.1.0/filer/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    31257 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.944334 django-filer-3.1.0/filer/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.964335 django-filer-3.1.0/filer/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    31258 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.964335 django-filer-3.1.0/filer/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.964335 django-filer-3.1.0/filer/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/management/commands/filer_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/management/commands/generate_thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/management/commands/import_files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.968335 django-filer-3.1.0/filer/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0002_auto_20150606_2003.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0003_thumbnailoption.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0004_auto_20160328_1434.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0005_auto_20160623_1425.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0006_auto_20160623_1627.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0007_auto_20161016_1055.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0008_auto_20171117_1313.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0009_auto_20171220_1635.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0010_auto_20180414_2058.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0011_auto_20190418_0137.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0012_file_mime_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0013_image_width_height_to_float.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0014_folder_permission_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/0017_image__transparent.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.968335 django-filer-3.1.0/filer/models/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9346 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/models/clipboardmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)    13491 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/models/filemodels.py
--rw-r--r--   0 runner    (1001) docker     (127)    12617 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/models/foldermodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/models/imagemodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/models/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/models/thumbnailoptionmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/models/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/models/virtualitems.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.968335 django-filer-3.1.0/filer/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.968335 django-filer-3.1.0/filer/server/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/server/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/server/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/server/backends/default.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/server/backends/nginx.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/server/backends/xsendfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/server/main_server_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/server/thumbnails_server_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/server/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/server/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    12965 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.944334 django-filer-3.1.0/filer/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.948334 django-filer-3.1.0/filer/static/filer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.968335 django-filer-3.1.0/filer/static/filer/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/css/admin_filer.cms.icons.css
--rwxr-xr-x   0 runner    (1001) docker     (127)    91031 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/css/admin_filer.css
--rw-r--r--   0 runner    (1001) docker     (127)    25479 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/css/admin_filer.fa.icons.css
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/css/admin_folderpermissions.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.972335 django-filer-3.1.0/filer/static/filer/css/maps/
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/css/maps/admin_filer.cms.icons.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    87032 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/css/maps/admin_filer.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    65841 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/css/maps/admin_filer.fa.icons.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/css/maps/admin_filer.icons.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.972335 django-filer-3.1.0/filer/static/filer/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   106260 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/django-filer-iconfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/django-filer-iconfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/django-filer-iconfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/django-filer-iconfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/django-filer-iconfont.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    68875 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)   355981 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)   138204 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    81284 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    64464 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.976335 django-filer-3.1.0/filer/static/filer/fonts/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/src/arrow-down.svg
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/src/caret-down.svg
--rw-r--r--   0 runner    (1001) docker     (127)      292 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/src/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/src/download.svg
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/src/expand.svg
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/src/link.svg
--rw-r--r--   0 runner    (1001) docker     (127)      557 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/src/move-to-folder.svg
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/src/picture.svg
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/src/remove-selection.svg
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/src/select.svg
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/src/th-large.svg
--rw-r--r--   0 runner    (1001) docker     (127)      648 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/src/th-list.svg
--rw-r--r--   0 runner    (1001) docker     (127)      523 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/fonts/src/upload.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.976335 django-filer-3.1.0/filer/static/filer/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/icons/cloud-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/icons/file-audio.svg
--rw-r--r--   0 runner    (1001) docker     (127)      637 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/icons/file-empty.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/icons/file-font.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/icons/file-missing.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/icons/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/icons/file-picture.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/icons/file-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/icons/file-video.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/icons/file-zip.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/icons/folder-dropdown.svg
--rw-r--r--   0 runner    (1001) docker     (127)      991 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/icons/folder-root.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/icons/folder-unfiled.svg
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/icons/folder.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.976335 django-filer-3.1.0/filer/static/filer/img/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/img/button-bg.gif
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/img/close.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/img/icon_changelink.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/img/icon_deletelink.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/img/loading_animation.gif
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/img/nav-bg.gif
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/img/select_item-hover.gif
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/img/select_item.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/img/upload_button.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.976335 django-filer-3.1.0/filer/static/filer/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.980335 django-filer-3.1.0/filer/static/filer/js/addons/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/addons/copy-move-files.js
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/addons/dropdown-menu.js
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/addons/dropzone.init.js
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/addons/filer_popup_response.js
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/addons/focal-point.js
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/addons/popup_handling.js
--rw-r--r--   0 runner    (1001) docker     (127)    10389 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/addons/table-dropzone.js
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/addons/toggler.js
--rw-r--r--   0 runner    (1001) docker     (127)      558 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/addons/tooltip.js
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/addons/upload-button.js
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/addons/widget.js
--rw-r--r--   0 runner    (1001) docker     (127)    11918 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/base.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.980335 django-filer-3.1.0/filer/static/filer/js/libs/
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/libs/class.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    34316 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/libs/dropzone.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    18574 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/libs/fileuploader.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   255084 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/libs/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/libs/jquery.cookie.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    95957 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/libs/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/static/filer/js/libs/mediator.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      616 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.948334 django-filer-3.1.0/filer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.948334 django-filer-3.1.0/filer/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.980335 django-filer-3.1.0/filer/templates/admin/filer/
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/actions.html
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/base_site.html
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/delete_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/delete_selected_files_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/dismiss_popup.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.980335 django-filer-3.1.0/filer/templates/admin/filer/file/
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/file/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      324 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/file/popup_response.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.984335 django-filer-3.1.0/filer/templates/admin/filer/folder/
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/folder/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/folder/choose_copy_destination.html
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/folder/choose_images_resize_options.html
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/folder/choose_move_destination.html
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/folder/choose_rename_format.html
--rw-r--r--   0 runner    (1001) docker     (127)    15547 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/folder/directory_listing.html
--rw-r--r--   0 runner    (1001) docker     (127)    17335 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/folder/directory_table_list.html
--rw-r--r--   0 runner    (1001) docker     (127)    13458 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/folder/directory_thumbnail_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/folder/list_type_switcher.html
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/folder/new_folder_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.984335 django-filer-3.1.0/filer/templates/admin/filer/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/image/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/image/expand.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.984335 django-filer-3.1.0/filer/templates/admin/filer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/templatetags/file_icon.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.984335 django-filer-3.1.0/filer/templates/admin/filer/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.984335 django-filer-3.1.0/filer/templates/admin/filer/tools/clipboard/
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/tools/clipboard/clipboard.html
--rw-r--r--   0 runner    (1001) docker     (127)      610 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/tools/detail_info.html
--rw-r--r--   0 runner    (1001) docker     (127)      616 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/tools/search_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.984335 django-filer-3.1.0/filer/templates/admin/filer/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/widgets/admin_file.html
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templates/admin/filer/widgets/admin_folder.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.984335 django-filer-3.1.0/filer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8881 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templatetags/filer_admin_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templatetags/filer_image_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/templatetags/filer_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/thumbnail_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:19.984335 django-filer-3.1.0/filer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/utils/filer_easy_thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/utils/generate_filename.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/utils/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/utils/model_label.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/utils/pil_exif.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/utils/recursive_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/utils/zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-10-02 14:10:10.000000 django-filer-3.1.0/filer/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2023-10-02 14:10:19.988335 django-filer-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2023-10-02 14:10:10.000000 django-filer-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.547062 django-filer-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2023-11-18 00:48:23.000000 django-filer-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2023-11-18 00:48:23.000000 django-filer-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2023-11-18 00:48:31.547062 django-filer-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2023-11-18 00:48:23.000000 django-filer-3.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.503062 django-filer-3.1.1/django_filer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2023-11-18 00:48:31.000000 django-filer-3.1.1/django_filer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2023-11-18 00:48:31.000000 django-filer-3.1.1/django_filer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-18 00:48:31.000000 django-filer-3.1.1/django_filer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-18 00:48:31.000000 django-filer-3.1.1/django_filer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2023-11-18 00:48:31.000000 django-filer-3.1.1/django_filer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-18 00:48:31.000000 django-filer-3.1.1/django_filer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.503062 django-filer-3.1.1/filer/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.507062 django-filer-3.1.1/filer/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/admin/clipboardadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/admin/fileadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57507 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/admin/folderadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/admin/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/admin/imageadmin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.507062 django-filer-3.1.1/filer/admin/patched/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/admin/patched/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/admin/patched/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/admin/permissionadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/admin/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/admin/thumbnailoptionadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/admin/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/admin/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.507062 django-filer-3.1.1/filer/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.507062 django-filer-3.1.1/filer/contrib/django_cms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/contrib/django_cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/contrib/django_cms/cms_toolbars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.507062 django-filer-3.1.1/filer/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/fields/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/fields/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/fields/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/fields/multistorage_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.507062 django-filer-3.1.1/filer/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.491062 django-filer-3.1.1/filer/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.507062 django-filer-3.1.1/filer/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    31860 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.491062 django-filer-3.1.1/filer/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.507062 django-filer-3.1.1/filer/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    31357 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.491062 django-filer-3.1.1/filer/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.507062 django-filer-3.1.1/filer/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16627 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    37796 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.491062 django-filer-3.1.1/filer/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.511062 django-filer-3.1.1/filer/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16442 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    37921 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.491062 django-filer-3.1.1/filer/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.511062 django-filer-3.1.1/filer/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    21636 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    40821 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.491062 django-filer-3.1.1/filer/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.511062 django-filer-3.1.1/filer/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    15724 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    37565 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.491062 django-filer-3.1.1/filer/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.511062 django-filer-3.1.1/filer/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    20427 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    40120 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.491062 django-filer-3.1.1/filer/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.511062 django-filer-3.1.1/filer/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    32775 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.491062 django-filer-3.1.1/filer/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.511062 django-filer-3.1.1/filer/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11064 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    35351 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.491062 django-filer-3.1.1/filer/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.511062 django-filer-3.1.1/filer/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    32039 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.491062 django-filer-3.1.1/filer/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.511062 django-filer-3.1.1/filer/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16713 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    37702 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.491062 django-filer-3.1.1/filer/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.511062 django-filer-3.1.1/filer/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    22139 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    41417 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.491062 django-filer-3.1.1/filer/locale/gl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.511062 django-filer-3.1.1/filer/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/gl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    32570 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.491062 django-filer-3.1.1/filer/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.515062 django-filer-3.1.1/filer/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    14347 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    37819 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.491062 django-filer-3.1.1/filer/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.515062 django-filer-3.1.1/filer/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13374 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    36804 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.491062 django-filer-3.1.1/filer/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.515062 django-filer-3.1.1/filer/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16819 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    37928 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.515062 django-filer-3.1.1/filer/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    17229 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    38419 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.515062 django-filer-3.1.1/filer/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    31244 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.515062 django-filer-3.1.1/filer/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    31258 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/ja_JP/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.515062 django-filer-3.1.1/filer/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    17336 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    38492 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/lt_LT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.515062 django-filer-3.1.1/filer/locale/lt_LT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/lt_LT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    31723 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/lt_LT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.515062 django-filer-3.1.1/filer/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    36063 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/nl_NL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.515062 django-filer-3.1.1/filer/locale/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    21260 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/nl_NL/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    40425 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/nl_NL/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/nn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.515062 django-filer-3.1.1/filer/locale/nn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12594 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/nn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    35986 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/nn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.519062 django-filer-3.1.1/filer/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    17155 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    38530 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.519062 django-filer-3.1.1/filer/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    31517 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.519062 django-filer-3.1.1/filer/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    17504 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    38699 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.519062 django-filer-3.1.1/filer/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    21137 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    42458 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.519062 django-filer-3.1.1/filer/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    31642 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.519062 django-filer-3.1.1/filer/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    33878 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/vi_VN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.519062 django-filer-3.1.1/filer/locale/vi_VN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18089 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/vi_VN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    38933 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/vi_VN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.519062 django-filer-3.1.1/filer/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    31243 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/zh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/zh-Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.519062 django-filer-3.1.1/filer/locale/zh-Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    15264 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/zh-Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    35527 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/zh-Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.495062 django-filer-3.1.1/filer/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.519062 django-filer-3.1.1/filer/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    31257 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.499062 django-filer-3.1.1/filer/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.523062 django-filer-3.1.1/filer/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    31258 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.523062 django-filer-3.1.1/filer/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.523062 django-filer-3.1.1/filer/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/management/commands/filer_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/management/commands/generate_thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/management/commands/import_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.523062 django-filer-3.1.1/filer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0002_auto_20150606_2003.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0003_thumbnailoption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0004_auto_20160328_1434.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0005_auto_20160623_1425.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0006_auto_20160623_1627.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0007_auto_20161016_1055.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0008_auto_20171117_1313.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0009_auto_20171220_1635.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0010_auto_20180414_2058.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0011_auto_20190418_0137.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0012_file_mime_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0013_image_width_height_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0014_folder_permission_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/0017_image__transparent.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.527062 django-filer-3.1.1/filer/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9346 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/models/clipboardmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13491 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/models/filemodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12617 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/models/foldermodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/models/imagemodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/models/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/models/thumbnailoptionmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/models/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/models/virtualitems.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.527062 django-filer-3.1.1/filer/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.527062 django-filer-3.1.1/filer/server/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/server/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/server/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/server/backends/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/server/backends/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/server/backends/xsendfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/server/main_server_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/server/thumbnails_server_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/server/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12965 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.499062 django-filer-3.1.1/filer/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.499062 django-filer-3.1.1/filer/static/filer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.527062 django-filer-3.1.1/filer/static/filer/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/css/admin_filer.cms.icons.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    91031 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/css/admin_filer.css
+-rw-r--r--   0 runner    (1001) docker     (127)    25479 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/css/admin_filer.fa.icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/css/admin_folderpermissions.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.531062 django-filer-3.1.1/filer/static/filer/css/maps/
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/css/maps/admin_filer.cms.icons.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    87032 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/css/maps/admin_filer.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    65841 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/css/maps/admin_filer.fa.icons.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/css/maps/admin_filer.icons.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.531062 django-filer-3.1.1/filer/static/filer/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   106260 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/django-filer-iconfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/django-filer-iconfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/django-filer-iconfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/django-filer-iconfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/django-filer-iconfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    68875 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   355981 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   138204 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    81284 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    64464 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.535062 django-filer-3.1.1/filer/static/filer/fonts/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/src/arrow-down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/src/caret-down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/src/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/src/download.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/src/expand.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/src/link.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/src/move-to-folder.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/src/picture.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/src/remove-selection.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/src/select.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/src/th-large.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/src/th-list.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/fonts/src/upload.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.535062 django-filer-3.1.1/filer/static/filer/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/icons/cloud-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/icons/file-audio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/icons/file-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/icons/file-font.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/icons/file-missing.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/icons/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/icons/file-picture.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/icons/file-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/icons/file-video.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/icons/file-zip.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/icons/folder-dropdown.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/icons/folder-root.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/icons/folder-unfiled.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/icons/folder.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.539062 django-filer-3.1.1/filer/static/filer/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/img/button-bg.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/img/close.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/img/icon_changelink.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/img/icon_deletelink.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/img/loading_animation.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/img/nav-bg.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/img/select_item-hover.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/img/select_item.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/img/upload_button.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.539062 django-filer-3.1.1/filer/static/filer/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.539062 django-filer-3.1.1/filer/static/filer/js/addons/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/addons/copy-move-files.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/addons/dropdown-menu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/addons/dropzone.init.js
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/addons/filer_popup_response.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/addons/focal-point.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/addons/popup_handling.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10389 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/addons/table-dropzone.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/addons/toggler.js
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/addons/tooltip.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/addons/upload-button.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/addons/widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11918 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/base.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.539062 django-filer-3.1.1/filer/static/filer/js/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/libs/class.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34316 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/libs/dropzone.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18574 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/libs/fileuploader.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   255084 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/libs/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/libs/jquery.cookie.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    95957 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/libs/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/static/filer/js/libs/mediator.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.499062 django-filer-3.1.1/filer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.499062 django-filer-3.1.1/filer/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.543062 django-filer-3.1.1/filer/templates/admin/filer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/actions.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/base_site.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/delete_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/delete_selected_files_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/dismiss_popup.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.543062 django-filer-3.1.1/filer/templates/admin/filer/file/
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/file/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/file/popup_response.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.543062 django-filer-3.1.1/filer/templates/admin/filer/folder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/folder/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/folder/choose_copy_destination.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/folder/choose_images_resize_options.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/folder/choose_move_destination.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/folder/choose_rename_format.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15547 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/folder/directory_listing.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17335 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/folder/directory_table_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13458 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/folder/directory_thumbnail_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/folder/list_type_switcher.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/folder/new_folder_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.543062 django-filer-3.1.1/filer/templates/admin/filer/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/image/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/image/expand.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.543062 django-filer-3.1.1/filer/templates/admin/filer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/templatetags/file_icon.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.543062 django-filer-3.1.1/filer/templates/admin/filer/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.547062 django-filer-3.1.1/filer/templates/admin/filer/tools/clipboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/tools/clipboard/clipboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/tools/detail_info.html
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/tools/search_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.547062 django-filer-3.1.1/filer/templates/admin/filer/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/widgets/admin_file.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templates/admin/filer/widgets/admin_folder.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.547062 django-filer-3.1.1/filer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8881 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templatetags/filer_admin_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templatetags/filer_image_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/templatetags/filer_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/thumbnail_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:31.547062 django-filer-3.1.1/filer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/utils/filer_easy_thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/utils/generate_filename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/utils/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/utils/model_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/utils/pil_exif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/utils/recursive_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/utils/zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-18 00:48:23.000000 django-filer-3.1.1/filer/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2023-11-18 00:48:31.547062 django-filer-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2023-11-18 00:48:23.000000 django-filer-3.1.1/setup.py
```

### Comparing `django-filer-3.1.0/LICENSE` & `django-filer-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/PKG-INFO` & `django-filer-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filer
-Version: 3.1.0
+Version: 3.1.1
 Summary: A file management application for django that makes handling of files and images a breeze.
 Home-page: https://github.com/django-cms/django-filer
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `django-filer-3.1.0/README.rst` & `django-filer-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/django_filer.egg-info/PKG-INFO` & `django-filer-3.1.1/django_filer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filer
-Version: 3.1.0
+Version: 3.1.1
 Summary: A file management application for django that makes handling of files and images a breeze.
 Home-page: https://github.com/django-cms/django-filer
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `django-filer-3.1.0/django_filer.egg-info/SOURCES.txt` & `django-filer-3.1.1/django_filer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/__init__.py` & `django-filer-3.1.1/filer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
  5. git push
  6. Assure that all tests pass on https://github.com/django-cms/django-filer/actions
  7. Create a new release on github. Create the new tag against the latest master commit and auto generate
     the release notes https://github.com/django-cms/django-filer/releases/new
  8. Publish the release and it will automatically release to pypi
 """
 
-__version__ = '3.1.0'
+__version__ = '3.1.1'
```

### Comparing `django-filer-3.1.0/filer/admin/__init__.py` & `django-filer-3.1.1/filer/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/admin/clipboardadmin.py` & `django-filer-3.1.1/filer/admin/clipboardadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/admin/fileadmin.py` & `django-filer-3.1.1/filer/admin/fileadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/admin/folderadmin.py` & `django-filer-3.1.1/filer/admin/folderadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/admin/forms.py` & `django-filer-3.1.1/filer/admin/forms.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/admin/imageadmin.py` & `django-filer-3.1.1/filer/admin/imageadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/admin/patched/admin_utils.py` & `django-filer-3.1.1/filer/admin/patched/admin_utils.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/admin/permissionadmin.py` & `django-filer-3.1.1/filer/admin/permissionadmin.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/admin/permissions.py` & `django-filer-3.1.1/filer/admin/permissions.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/admin/tools.py` & `django-filer-3.1.1/filer/admin/tools.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/admin/views.py` & `django-filer-3.1.1/filer/admin/views.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/apps.py` & `django-filer-3.1.1/filer/apps.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/contrib/django_cms/cms_toolbars.py` & `django-filer-3.1.1/filer/contrib/django_cms/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/fields/file.py` & `django-filer-3.1.1/filer/fields/file.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/fields/folder.py` & `django-filer-3.1.1/filer/fields/folder.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/fields/multistorage_file.py` & `django-filer-3.1.1/filer/fields/multistorage_file.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/ar/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/ar/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/bg/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/ca/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/ca/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/cs/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/cs/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/de/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/de/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/en/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/en/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/es/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/es/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/et/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/et/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/eu/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/eu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/eu/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/fa/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/fa/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/fi/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/fi/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/fr/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/fr/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/gl/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/gl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/gl/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/he/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/he/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/hr/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/hr/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/hu/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/hu/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/it/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/it/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/ja/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/ja_JP/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/lt/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/lt/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/lt_LT/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/lt_LT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/lt_LT/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/lt_LT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/nb/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/nb/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/nl_NL/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/nl_NL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/nl_NL/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/nl_NL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/nn/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/nn/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/nn/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/nn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/pl/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/pl/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/pt/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/pt_BR/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/pt_BR/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/ru/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/ru/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/sk/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/sk/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/tr/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/tr/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/vi_VN/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/vi_VN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/vi_VN/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/vi_VN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/zh/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/zh-Hans/LC_MESSAGES/django.mo` & `django-filer-3.1.1/filer/locale/zh-Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/zh-Hans/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/zh-Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/zh_CN/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/locale/zh_TW/LC_MESSAGES/django.po` & `django-filer-3.1.1/filer/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/management/commands/generate_thumbnails.py` & `django-filer-3.1.1/filer/management/commands/generate_thumbnails.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/management/commands/import_files.py` & `django-filer-3.1.1/filer/management/commands/import_files.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/migrations/0001_initial.py` & `django-filer-3.1.1/filer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/migrations/0002_auto_20150606_2003.py` & `django-filer-3.1.1/filer/migrations/0002_auto_20150606_2003.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/migrations/0003_thumbnailoption.py` & `django-filer-3.1.1/filer/migrations/0003_thumbnailoption.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/migrations/0005_auto_20160623_1425.py` & `django-filer-3.1.1/filer/migrations/0005_auto_20160623_1425.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/migrations/0006_auto_20160623_1627.py` & `django-filer-3.1.1/filer/migrations/0006_auto_20160623_1627.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/migrations/0008_auto_20171117_1313.py` & `django-filer-3.1.1/filer/migrations/0008_auto_20171117_1313.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/migrations/0010_auto_20180414_2058.py` & `django-filer-3.1.1/filer/migrations/0010_auto_20180414_2058.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/migrations/0011_auto_20190418_0137.py` & `django-filer-3.1.1/filer/migrations/0011_auto_20190418_0137.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/migrations/0012_file_mime_type.py` & `django-filer-3.1.1/filer/migrations/0012_file_mime_type.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/migrations/0013_image_width_height_to_float.py` & `django-filer-3.1.1/filer/migrations/0013_image_width_height_to_float.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/migrations/0014_folder_permission_choices.py` & `django-filer-3.1.1/filer/migrations/0014_folder_permission_choices.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py` & `django-filer-3.1.1/filer/migrations/0015_alter_file_owner_alter_file_polymorphic_ctype_and_more.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py` & `django-filer-3.1.1/filer/migrations/0016_alter_folder_index_together_remove_folder_level_and_more.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/models/abstract.py` & `django-filer-3.1.1/filer/models/abstract.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/models/clipboardmodels.py` & `django-filer-3.1.1/filer/models/clipboardmodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/models/filemodels.py` & `django-filer-3.1.1/filer/models/filemodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/models/foldermodels.py` & `django-filer-3.1.1/filer/models/foldermodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/models/imagemodels.py` & `django-filer-3.1.1/filer/models/imagemodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/models/mixins.py` & `django-filer-3.1.1/filer/models/mixins.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/models/thumbnailoptionmodels.py` & `django-filer-3.1.1/filer/models/thumbnailoptionmodels.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/models/tools.py` & `django-filer-3.1.1/filer/models/tools.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/models/virtualitems.py` & `django-filer-3.1.1/filer/models/virtualitems.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/server/backends/base.py` & `django-filer-3.1.1/filer/server/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/server/backends/default.py` & `django-filer-3.1.1/filer/server/backends/default.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/server/backends/nginx.py` & `django-filer-3.1.1/filer/server/backends/nginx.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/server/backends/xsendfile.py` & `django-filer-3.1.1/filer/server/backends/xsendfile.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/server/views.py` & `django-filer-3.1.1/filer/server/views.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/settings.py` & `django-filer-3.1.1/filer/settings.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/css/admin_filer.cms.icons.css` & `django-filer-3.1.1/filer/static/filer/css/admin_filer.cms.icons.css`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/css/admin_filer.css` & `django-filer-3.1.1/filer/static/filer/css/admin_filer.css`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/css/admin_filer.fa.icons.css` & `django-filer-3.1.1/filer/static/filer/css/admin_filer.fa.icons.css`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/css/maps/admin_filer.cms.icons.css.map` & `django-filer-3.1.1/filer/static/filer/css/maps/admin_filer.cms.icons.css.map`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/css/maps/admin_filer.css.map` & `django-filer-3.1.1/filer/static/filer/css/maps/admin_filer.css.map`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/css/maps/admin_filer.fa.icons.css.map` & `django-filer-3.1.1/filer/static/filer/css/maps/admin_filer.fa.icons.css.map`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/css/maps/admin_filer.icons.css.map` & `django-filer-3.1.1/filer/static/filer/css/maps/admin_filer.icons.css.map`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/fonts/FontAwesome.otf` & `django-filer-3.1.1/filer/static/filer/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/fonts/django-filer-iconfont.eot` & `django-filer-3.1.1/filer/static/filer/fonts/django-filer-iconfont.eot`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/fonts/django-filer-iconfont.svg` & `django-filer-3.1.1/filer/static/filer/fonts/django-filer-iconfont.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/fonts/django-filer-iconfont.ttf` & `django-filer-3.1.1/filer/static/filer/fonts/django-filer-iconfont.ttf`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/fonts/django-filer-iconfont.woff` & `django-filer-3.1.1/filer/static/filer/fonts/django-filer-iconfont.woff`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/fonts/django-filer-iconfont.woff2` & `django-filer-3.1.1/filer/static/filer/fonts/django-filer-iconfont.woff2`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/fonts/fontawesome-webfont.eot` & `django-filer-3.1.1/filer/static/filer/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/fonts/fontawesome-webfont.svg` & `django-filer-3.1.1/filer/static/filer/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/fonts/fontawesome-webfont.ttf` & `django-filer-3.1.1/filer/static/filer/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/fonts/fontawesome-webfont.woff` & `django-filer-3.1.1/filer/static/filer/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/fonts/fontawesome-webfont.woff2` & `django-filer-3.1.1/filer/static/filer/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/fonts/src/arrow-down.svg` & `django-filer-3.1.1/filer/static/filer/fonts/src/arrow-down.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/fonts/src/link.svg` & `django-filer-3.1.1/filer/static/filer/fonts/src/link.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/fonts/src/move-to-folder.svg` & `django-filer-3.1.1/filer/static/filer/fonts/src/move-to-folder.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/fonts/src/th-list.svg` & `django-filer-3.1.1/filer/static/filer/fonts/src/th-list.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/fonts/src/upload.svg` & `django-filer-3.1.1/filer/static/filer/fonts/src/upload.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/icons/cloud-up.svg` & `django-filer-3.1.1/filer/static/filer/icons/cloud-up.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/icons/file-audio.svg` & `django-filer-3.1.1/filer/static/filer/icons/file-audio.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/icons/file-empty.svg` & `django-filer-3.1.1/filer/static/filer/icons/file-empty.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/icons/file-font.svg` & `django-filer-3.1.1/filer/static/filer/icons/file-font.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/icons/file-missing.svg` & `django-filer-3.1.1/filer/static/filer/icons/file-missing.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/icons/file-pdf.svg` & `django-filer-3.1.1/filer/static/filer/icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/icons/file-picture.svg` & `django-filer-3.1.1/filer/static/filer/icons/file-picture.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/icons/file-unknown.svg` & `django-filer-3.1.1/filer/static/filer/icons/file-unknown.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/icons/file-video.svg` & `django-filer-3.1.1/filer/static/filer/icons/file-video.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/icons/file-zip.svg` & `django-filer-3.1.1/filer/static/filer/icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/icons/folder-dropdown.svg` & `django-filer-3.1.1/filer/static/filer/icons/folder-dropdown.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/icons/folder-root.svg` & `django-filer-3.1.1/filer/static/filer/icons/folder-root.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/icons/folder-unfiled.svg` & `django-filer-3.1.1/filer/static/filer/icons/folder-unfiled.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/icons/folder.svg` & `django-filer-3.1.1/filer/static/filer/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/img/icon_changelink.gif` & `django-filer-3.1.1/filer/static/filer/img/icon_changelink.gif`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/img/icon_deletelink.gif` & `django-filer-3.1.1/filer/static/filer/img/icon_deletelink.gif`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/img/loading_animation.gif` & `django-filer-3.1.1/filer/static/filer/img/loading_animation.gif`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/img/upload_button.png` & `django-filer-3.1.1/filer/static/filer/img/upload_button.png`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/addons/copy-move-files.js` & `django-filer-3.1.1/filer/static/filer/js/addons/copy-move-files.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/addons/dropdown-menu.js` & `django-filer-3.1.1/filer/static/filer/js/addons/dropdown-menu.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/addons/dropzone.init.js` & `django-filer-3.1.1/filer/static/filer/js/addons/dropzone.init.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -161,32 +161,34 @@
             window.filerDropzoneInitialized = true;
             Dropzone.autoDiscover = false;
         }
         dropzones.each(createDropzone);
 
         // Handle initialization of the dropzone on dynamic formsets (i.e. Django admin inlines)
         $(document).on('formset:added', function(ev, row) {
+            var dropzones, rowIdx, row_;
             if (ev.detail && ev.detail.formsetName) {
                 /*
                     Django 4.1 changed the event type being fired when adding
                     a new formset from a jQuery to a vanilla JavaScript event.
                     https://docs.djangoproject.com/en/4.1/ref/contrib/admin/javascript/
 
                     In this case we find the newly added row and initialize the
                     dropzone on any dropzoneSelector on that row.
                 */
-                let rowIdx = parseInt(
+
+                rowIdx = parseInt(
                     document.getElementById(
                         'id_' + event.detail.formsetName + '-TOTAL_FORMS'
                     ).value, 10
                 ) - 1;
-                let row_ = document.getElementById(event.detail.formsetName + '-' + rowIdx);
-                var dropzones = $(row_).find(dropzoneSelector)
+                row_ = document.getElementById(event.detail.formsetName + '-' + rowIdx);
+                dropzones = $(row_).find(dropzoneSelector);
 
             } else {
-                var dropzones = $(row).find(dropzoneSelector);
+                dropzones = $(row).find(dropzoneSelector);
             }
 
             dropzones.each(createDropzone);
         });
     }
 });
```

### Comparing `django-filer-3.1.0/filer/static/filer/js/addons/filer_popup_response.js` & `django-filer-3.1.1/filer/static/filer/js/addons/filer_popup_response.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/addons/focal-point.js` & `django-filer-3.1.1/filer/static/filer/js/addons/focal-point.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/addons/popup_handling.js` & `django-filer-3.1.1/filer/static/filer/js/addons/popup_handling.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/addons/table-dropzone.js` & `django-filer-3.1.1/filer/static/filer/js/addons/table-dropzone.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/addons/toggler.js` & `django-filer-3.1.1/filer/static/filer/js/addons/toggler.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/addons/tooltip.js` & `django-filer-3.1.1/filer/static/filer/js/addons/tooltip.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/addons/upload-button.js` & `django-filer-3.1.1/filer/static/filer/js/addons/upload-button.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/addons/widget.js` & `django-filer-3.1.1/filer/static/filer/js/addons/widget.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/base.js` & `django-filer-3.1.1/filer/static/filer/js/base.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/libs/class.min.js` & `django-filer-3.1.1/filer/static/filer/js/libs/class.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/libs/dropzone.min.js` & `django-filer-3.1.1/filer/static/filer/js/libs/dropzone.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/libs/fileuploader.min.js` & `django-filer-3.1.1/filer/static/filer/js/libs/fileuploader.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/libs/jquery-ui.min.js` & `django-filer-3.1.1/filer/static/filer/js/libs/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/libs/jquery.cookie.min.js` & `django-filer-3.1.1/filer/static/filer/js/libs/jquery.cookie.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/libs/jquery.min.js` & `django-filer-3.1.1/filer/static/filer/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/static/filer/js/libs/mediator.min.js` & `django-filer-3.1.1/filer/static/filer/js/libs/mediator.min.js`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/storage.py` & `django-filer-3.1.1/filer/storage.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/actions.html` & `django-filer-3.1.1/filer/templates/admin/filer/actions.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/base_site.html` & `django-filer-3.1.1/filer/templates/admin/filer/base_site.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/breadcrumbs.html` & `django-filer-3.1.1/filer/templates/admin/filer/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/change_form.html` & `django-filer-3.1.1/filer/templates/admin/filer/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/delete_selected_files_confirmation.html` & `django-filer-3.1.1/filer/templates/admin/filer/delete_selected_files_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/file/change_form.html` & `django-filer-3.1.1/filer/templates/admin/filer/file/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/folder/change_form.html` & `django-filer-3.1.1/filer/templates/admin/filer/folder/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/folder/choose_copy_destination.html` & `django-filer-3.1.1/filer/templates/admin/filer/folder/choose_copy_destination.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/folder/choose_images_resize_options.html` & `django-filer-3.1.1/filer/templates/admin/filer/folder/choose_images_resize_options.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/folder/choose_move_destination.html` & `django-filer-3.1.1/filer/templates/admin/filer/folder/choose_move_destination.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/folder/choose_rename_format.html` & `django-filer-3.1.1/filer/templates/admin/filer/folder/choose_rename_format.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/folder/directory_listing.html` & `django-filer-3.1.1/filer/templates/admin/filer/folder/directory_listing.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/folder/directory_table_list.html` & `django-filer-3.1.1/filer/templates/admin/filer/folder/directory_table_list.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/folder/directory_thumbnail_list.html` & `django-filer-3.1.1/filer/templates/admin/filer/folder/directory_thumbnail_list.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/folder/new_folder_form.html` & `django-filer-3.1.1/filer/templates/admin/filer/folder/new_folder_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/image/change_form.html` & `django-filer-3.1.1/filer/templates/admin/filer/image/change_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/image/expand.html` & `django-filer-3.1.1/filer/templates/admin/filer/image/expand.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/templatetags/file_icon.html` & `django-filer-3.1.1/filer/templates/admin/filer/templatetags/file_icon.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/tools/clipboard/clipboard.html` & `django-filer-3.1.1/filer/templates/admin/filer/tools/clipboard/clipboard.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html` & `django-filer-3.1.1/filer/templates/admin/filer/tools/clipboard/clipboard_item_rows.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/tools/detail_info.html` & `django-filer-3.1.1/filer/templates/admin/filer/tools/detail_info.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/tools/search_form.html` & `django-filer-3.1.1/filer/templates/admin/filer/tools/search_form.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/widgets/admin_file.html` & `django-filer-3.1.1/filer/templates/admin/filer/widgets/admin_file.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templates/admin/filer/widgets/admin_folder.html` & `django-filer-3.1.1/filer/templates/admin/filer/widgets/admin_folder.html`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templatetags/filer_admin_tags.py` & `django-filer-3.1.1/filer/templatetags/filer_admin_tags.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templatetags/filer_image_tags.py` & `django-filer-3.1.1/filer/templatetags/filer_image_tags.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/templatetags/filer_tags.py` & `django-filer-3.1.1/filer/templatetags/filer_tags.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/thumbnail_processors.py` & `django-filer-3.1.1/filer/thumbnail_processors.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/utils/compatibility.py` & `django-filer-3.1.1/filer/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/utils/filer_easy_thumbnails.py` & `django-filer-3.1.1/filer/utils/filer_easy_thumbnails.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/utils/files.py` & `django-filer-3.1.1/filer/utils/files.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/utils/generate_filename.py` & `django-filer-3.1.1/filer/utils/generate_filename.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/utils/loader.py` & `django-filer-3.1.1/filer/utils/loader.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/utils/pil_exif.py` & `django-filer-3.1.1/filer/utils/pil_exif.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/utils/recursive_dictionary.py` & `django-filer-3.1.1/filer/utils/recursive_dictionary.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/utils/zip.py` & `django-filer-3.1.1/filer/utils/zip.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/filer/validation.py` & `django-filer-3.1.1/filer/validation.py`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/setup.cfg` & `django-filer-3.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-filer-3.1.0/setup.py` & `django-filer-3.1.1/setup.py`

 * *Files identical despite different names*

