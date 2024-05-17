# Comparing `tmp/invenio-drafts-resources-3.0.0.tar.gz` & `tmp/invenio-drafts-resources-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-drafts-resources-3.0.0.tar", last modified: Wed Jan 31 13:09:48 2024, max compression
+gzip compressed data, was "invenio-drafts-resources-3.1.0.tar", last modified: Mon May  6 16:39:58 2024, max compression
```

## Comparing `invenio-drafts-resources-3.0.0.tar` & `invenio-drafts-resources-3.1.0.tar`

### file list

```diff
@@ -1,329 +1,329 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.334655 invenio-drafts-resources-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.290655 invenio-drafts-resources-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.306655 invenio-drafts-resources-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.306655 invenio-drafts-resources-3.0.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-01-31 13:09:48.334655 invenio-drafts-resources-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.306655 invenio-drafts-resources-3.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.306655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.310655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10644 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/records/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.310655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/records/systemfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/records/systemfields/parent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/records/systemfields/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.310655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.310655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/resources/records/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/resources/records/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7724 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/resources/records/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.310655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.310655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.314655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/components/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/components/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/components/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/components/media_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/components/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/components/pid.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/components/relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/search_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    25290 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/uow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.314655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.290655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.314655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.290655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.314655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.290655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.314655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.314655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.314655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.314655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.314655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.314655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.314655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.314655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/en_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.314655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/en_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.314655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.318655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es_CU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.318655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es_MX/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.318655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.318655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.318655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.318655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.318655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.318655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr_CI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.318655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.318655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.318655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hi_IN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.318655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.318655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.294655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.322655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.322655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.322655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.322655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.322655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.322655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ne/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.322655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.322655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.322655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.322655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.322655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.322655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.322655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.326655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.326655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sv_SE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.326655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.326655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.326655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.326655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.326655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.298655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.326655 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.306655 invenio-drafts-resources-3.0.0/invenio_drafts_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-31 13:09:48.000000 invenio-drafts-resources-3.0.0/invenio_drafts_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1905 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-01-31 13:09:48.334655 invenio-drafts-resources-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.326655 invenio-drafts-resources-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.326655 invenio-drafts-resources-3.0.0/tests/mock_module/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.326655 invenio-drafts-resources-3.0.0/tests/mock_module/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.326655 invenio-drafts-resources-3.0.0/tests/mock_module/jsonschemas/records/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/jsonschemas/records/parent-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/jsonschemas/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.330655 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.330655 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.330655 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v1/draftsresources/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v1/draftsresources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.330655 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.330655 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v1/draftsresources/records/
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.330655 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.330655 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v2/draftsresources/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v2/draftsresources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.330655 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.330655 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v2/draftsresources/records/
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.330655 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.330655 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/v7/draftsresources/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/v7/draftsresources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.330655 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/v7/draftsresources/drafts/
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.330655 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/v7/draftsresources/records/
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/mock_module/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.330655 invenio-drafts-resources-3.0.0/tests/records/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    14908 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/records/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.330655 invenio-drafts-resources-3.0.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/resources/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/resources/test_files_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/resources/test_record_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/resources/test_resource_links.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 13:09:48.334655 invenio-drafts-resources-3.0.0/tests/services/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/services/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12155 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/services/test_record_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    22534 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/services/test_record_service_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/services/test_record_service_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/services/test_record_service_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/services/test_records_uow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/services/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-01-31 13:09:38.000000 invenio-drafts-resources-3.0.0/tests/services/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.325873 invenio-drafts-resources-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.285873 invenio-drafts-resources-3.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.297873 invenio-drafts-resources-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.297873 invenio-drafts-resources-3.1.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-06 16:39:58.325873 invenio-drafts-resources-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.301873 invenio-drafts-resources-3.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.301873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.301873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10644 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.301873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/records/systemfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/records/systemfields/parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/records/systemfields/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.301873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.305873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/resources/records/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/resources/records/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7724 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/resources/records/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.305873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.305873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.305873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/components/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/components/media_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/components/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/components/pid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/components/relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/search_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25290 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/uow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.305873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.285873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.305873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.285873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.305873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.285873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.305873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.285873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.305873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.285873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.309873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.285873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.309873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.309873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.309873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.309873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.309873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.309873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.309873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.309873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.309873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.309873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.309873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.309873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.309873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.313873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.313873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.313873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.313873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.313873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.313873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.313873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.313873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.313873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.313873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.313873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.313873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.289873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.313873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.293873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.317873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.293873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.317873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.293873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.317873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.293873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.317873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.293873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.317873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.293873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.317873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.293873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.317873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.293873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.317873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.293873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.317873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.293873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.317873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.293873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.317873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.293873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.317873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.293873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.317873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.293873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.317873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.293873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.301873 invenio-drafts-resources-3.1.0/invenio_drafts_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 16:39:58.000000 invenio-drafts-resources-3.1.0/invenio_drafts_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1905 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-06 16:39:58.325873 invenio-drafts-resources-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/mock_module/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/mock_module/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/mock_module/jsonschemas/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/jsonschemas/records/parent-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/jsonschemas/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v1/draftsresources/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v1/draftsresources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v1/draftsresources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v2/draftsresources/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v2/draftsresources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v2/draftsresources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/v7/draftsresources/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/v7/draftsresources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/v7/draftsresources/drafts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/v7/draftsresources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/mock_module/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.321873 invenio-drafts-resources-3.1.0/tests/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14908 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/records/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.325873 invenio-drafts-resources-3.1.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/resources/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/resources/test_files_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/resources/test_record_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/resources/test_resource_links.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:39:58.325873 invenio-drafts-resources-3.1.0/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/services/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/services/test_record_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22947 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/services/test_record_service_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/services/test_record_service_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/services/test_record_service_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/services/test_records_uow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/services/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-06 16:39:52.000000 invenio-drafts-resources-3.1.0/tests/services/utils.py
```

### Comparing `invenio-drafts-resources-3.0.0/.editorconfig` & `invenio-drafts-resources-3.1.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/.github/workflows/pypi-publish.yml` & `invenio-drafts-resources-3.1.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/.github/workflows/tests.yml` & `invenio-drafts-resources-3.1.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/.tx/config` & `invenio-drafts-resources-3.1.0/.tx/config`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020 CERN.
+# Copyright (C) 2020-2024 CERN.
 # Copyright (C) 2023 Graz University of Technology.
 #
 # Invenio-Drafts-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 #
 # 1) Create message catalog:
@@ -21,12 +21,12 @@
 #    $ tx pull -l <lang>
 # 6) Pull translations for all languages from Transifex
 #    $ tx pull -a
 
 [main]
 host = https://app.transifex.com
 
-[o:inveniosoftware:p:invenio:r:invenio_drafts_resources-messages]
+[o:inveniosoftware:p:invenio:r:invenio-drafts-resources-messages]
 file_filter = invenio_drafts_resources/translations/<lang>/LC_MESSAGES/messages.po
 source_file = invenio_drafts_resources/translations/messages.pot
 source_lang = en
 type = PO
```

### Comparing `invenio-drafts-resources-3.0.0/CHANGES.rst` & `invenio-drafts-resources-3.1.0/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,18 @@
     Invenio-Drafts-Resources is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 3.1.0 (released 2024-05-03)
+
+- media-files: prevent copying to new version
+
 Version 3.0.0 (released 2024-01-31)
 
 - installation: bump dependencies
 - uow: add "bulk_index" param on ParentRecordCommmitOp
 
 Version 2.0.2 (2023-11-07)
```

### Comparing `invenio-drafts-resources-3.0.0/CONTRIBUTING.rst` & `invenio-drafts-resources-3.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/LICENSE` & `invenio-drafts-resources-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/MANIFEST.in` & `invenio-drafts-resources-3.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/PKG-INFO` & `invenio-drafts-resources-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-drafts-resources
-Version: 3.0.0
+Version: 3.1.0
 Summary: Invenio Drafts Resources module to create REST APIs
 Home-page: https://github.com/inveniosoftware/Invenio-Drafts-Resources
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Keywords: invenio records deposit submit versioning drafts
 Platform: any
@@ -58,14 +58,18 @@
     Invenio-Drafts-Resources is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 3.1.0 (released 2024-05-03)
+
+- media-files: prevent copying to new version
+
 Version 3.0.0 (released 2024-01-31)
 
 - installation: bump dependencies
 - uow: add "bulk_index" param on ParentRecordCommmitOp
 
 Version 2.0.2 (2023-11-07)
```

### Comparing `invenio-drafts-resources-3.0.0/README.rst` & `invenio-drafts-resources-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/babel.ini` & `invenio-drafts-resources-3.1.0/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/docs/Makefile` & `invenio-drafts-resources-3.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/docs/conf.py` & `invenio-drafts-resources-3.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/docs/index.rst` & `invenio-drafts-resources-3.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/docs/make.bat` & `invenio-drafts-resources-3.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/records/__init__.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/records/api.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/records/models.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/records/systemfields/parent.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/records/systemfields/parent.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/records/systemfields/versions.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/records/systemfields/versions.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/resources/records/args.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/resources/records/args.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/resources/records/config.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/resources/records/errors.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/resources/records/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/resources/records/resource.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/resources/records/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/components/__init__.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/components/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/components/base.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/components/base.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/components/files.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/components/files.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/components/media_files.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/components/media_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020-2021 CERN.
+# Copyright (C) 2020-2024 CERN.
 # Copyright (C) 2021 Northwestern University.
 # Copyright (C) 2023 Graz University of Technology.
 #
 # Invenio-Drafts-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
@@ -129,17 +129,16 @@
         self._purge_bucket_and_ovs(draft_files)
 
     def new_version(self, identity, draft=None, record=None):
         """New version callback."""
         # We don't copy files from the previous version, but instead allow
         # users to import the files.
         draft_files = self.get_record_files(draft)
-        record_files = self.get_record_files(record)
-        draft_files.enabled = record_files.enabled
-        draft_files.copy(record_files)
+        # Set media files to the default config
+        draft_files.enabled = self.service.config.default_media_files_enabled
 
     def import_files(self, identity, draft=None, record=None):
         """Import files callback."""
         # We don't need the import for media files
         return
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/components/metadata.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/components/metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/components/pid.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/components/pid.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/components/relations.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/components/relations.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/config.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/config.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/permissions.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/schema.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/search_params.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/search_params.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/service.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/service.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/tasks.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/services/records/uow.py` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/services/records/uow.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 00000190: 6e20 213d 2031 293b 0a4d 494d 452d 5665  n != 1);.MIME-Ve
 000001a0: 7273 696f 6e3a 2031 2e30 0a43 6f6e 7465  rsion: 1.0.Conte
 000001b0: 6e74 2d54 7970 653a 2074 6578 742f 706c  nt-Type: text/pl
 000001c0: 6169 6e3b 2063 6861 7273 6574 3d75 7466  ain; charset=utf
 000001d0: 2d38 0a43 6f6e 7465 6e74 2d54 7261 6e73  -8.Content-Trans
 000001e0: 6665 722d 456e 636f 6469 6e67 3a20 3862  fer-Encoding: 8b
 000001f0: 6974 0a47 656e 6572 6174 6564 2d42 793a  it.Generated-By:
-00000200: 2042 6162 656c 2032 2e31 342e 300a 00     Babel 2.14.0..
+00000200: 2042 6162 656c 2032 2e31 352e 300a 00     Babel 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language-Team: Arabic (https://app.transifex.com/inveniosoftware/teams/23537/"
 "ar/)\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "Best match"
 msgstr "أفضل تطابق "
 
 msgid "Files support must be enabled."
 msgstr "دعم الملفات يجب أن يكون مفعّلا ."
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 00000190: 6e20 213d 2031 293b 0a4d 494d 452d 5665  n != 1);.MIME-Ve
 000001a0: 7273 696f 6e3a 2031 2e30 0a43 6f6e 7465  rsion: 1.0.Conte
 000001b0: 6e74 2d54 7970 653a 2074 6578 742f 706c  nt-Type: text/pl
 000001c0: 6169 6e3b 2063 6861 7273 6574 3d75 7466  ain; charset=utf
 000001d0: 2d38 0a43 6f6e 7465 6e74 2d54 7261 6e73  -8.Content-Trans
 000001e0: 6665 722d 456e 636f 6469 6e67 3a20 3862  fer-Encoding: 8b
 000001f0: 6974 0a47 656e 6572 6174 6564 2d42 793a  it.Generated-By:
-00000200: 2042 6162 656c 2032 2e31 342e 300a 00     Babel 2.14.0..
+00000200: 2042 6162 656c 2032 2e31 352e 300a 00     Babel 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,11 +8,11 @@
 "Language: ca\n"
 "Language-Team: Catalan (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ca/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "Version"
 msgstr "Versió"
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,11 +9,11 @@
 "Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/"
 "cs/)\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "Version"
 msgstr "Verze"
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 7% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 000000a0: 653a 2032 3032 322d 3130 2d31 3220 3039  e: 2022-10-12 09
 000000b0: 3a30 372b 3030 3030 0a50 4f2d 5265 7669  :07+0000.PO-Revi
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
-00000110: 7561 6765 3a20 6461 0a4c 616e 6775 6167  uage: da.Languag
-00000120: 652d 5465 616d 3a20 4461 6e69 7368 2028  e-Team: Danish (
-00000130: 6874 7470 733a 2f2f 6170 702e 7472 616e  https://app.tran
-00000140: 7369 6665 782e 636f 6d2f 696e 7665 6e69  sifex.com/inveni
-00000150: 6f73 6f66 7477 6172 652f 7465 616d 732f  osoftware/teams/
-00000160: 3233 3533 372f 6461 2f29 0a50 6c75 7261  23537/da/).Plura
-00000170: 6c2d 466f 726d 733a 206e 706c 7572 616c  l-Forms: nplural
-00000180: 733d 323b 2070 6c75 7261 6c3d 286e 2021  s=2; plural=(n !
-00000190: 3d20 3129 3b0a 4d49 4d45 2d56 6572 7369  = 1);.MIME-Versi
+00000110: 7561 6765 3a20 6b61 0a4c 616e 6775 6167  uage: ka.Languag
+00000120: 652d 5465 616d 3a20 4765 6f72 6769 616e  e-Team: Georgian
+00000130: 2028 6874 7470 733a 2f2f 6170 702e 7472   (https://app.tr
+00000140: 616e 7369 6665 782e 636f 6d2f 696e 7665  ansifex.com/inve
+00000150: 6e69 6f73 6f66 7477 6172 652f 7465 616d  niosoftware/team
+00000160: 732f 3233 3533 372f 6b61 2f29 0a50 6c75  s/23537/ka/).Plu
+00000170: 7261 6c2d 466f 726d 733a 206e 706c 7572  ral-Forms: nplur
+00000180: 616c 733d 323b 2070 6c75 7261 6c3d 286e  als=2; plural=(n
+00000190: 213d 3129 3b0a 4d49 4d45 2d56 6572 7369  !=1);.MIME-Versi
 000001a0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
 000001b0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
 000001c0: 3b20 6368 6172 7365 743d 7574 662d 380a  ; charset=utf-8.
 000001d0: 436f 6e74 656e 742d 5472 616e 7366 6572  Content-Transfer
 000001e0: 2d45 6e63 6f64 696e 673a 2038 6269 740a  -Encoding: 8bit.
 000001f0: 4765 6e65 7261 7465 642d 4279 3a20 4261  Generated-By: Ba
-00000200: 6265 6c20 322e 3134 2e30 0a00            bel 2.14.0..
+00000200: 6265 6c20 322e 3135 2e30 0a00            bel 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: de\n"
 "Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/"
 "de/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "Best match"
 msgstr "Höchste Übereinstimmung"
 
 msgid "Files support must be enabled."
 msgstr "Die Datei-Unterstützung muss aktiviert sein."
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 000001a0: 3d20 3129 3b0a 4d49 4d45 2d56 6572 7369  = 1);.MIME-Versi
 000001b0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
 000001c0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
 000001d0: 3b20 6368 6172 7365 743d 7574 662d 380a  ; charset=utf-8.
 000001e0: 436f 6e74 656e 742d 5472 616e 7366 6572  Content-Transfer
 000001f0: 2d45 6e63 6f64 696e 673a 2038 6269 740a  -Encoding: 8bit.
 00000200: 4765 6e65 7261 7465 642d 4279 3a20 4261  Generated-By: Ba
-00000210: 6265 6c20 322e 3134 2e30 0a00            bel 2.14.0..
+00000210: 6265 6c20 322e 3135 2e30 0a00            bel 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 000001a0: 3d20 3129 3b0a 4d49 4d45 2d56 6572 7369  = 1);.MIME-Versi
 000001b0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
 000001c0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
 000001d0: 3b20 6368 6172 7365 743d 7574 662d 380a  ; charset=utf-8.
 000001e0: 436f 6e74 656e 742d 5472 616e 7366 6572  Content-Transfer
 000001f0: 2d45 6e63 6f64 696e 673a 2038 6269 740a  -Encoding: 8bit.
 00000200: 4765 6e65 7261 7465 642d 4279 3a20 4261  Generated-By: Ba
-00000210: 6265 6c20 322e 3134 2e30 0a00            bel 2.14.0..
+00000210: 6265 6c20 322e 3135 2e30 0a00            bel 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 00000190: 2031 293b 0a4d 494d 452d 5665 7273 696f   1);.MIME-Versio
 000001a0: 6e3a 2031 2e30 0a43 6f6e 7465 6e74 2d54  n: 1.0.Content-T
 000001b0: 7970 653a 2074 6578 742f 706c 6169 6e3b  ype: text/plain;
 000001c0: 2063 6861 7273 6574 3d75 7466 2d38 0a43   charset=utf-8.C
 000001d0: 6f6e 7465 6e74 2d54 7261 6e73 6665 722d  ontent-Transfer-
 000001e0: 456e 636f 6469 6e67 3a20 3862 6974 0a47  Encoding: 8bit.G
 000001f0: 656e 6572 6174 6564 2d42 793a 2042 6162  enerated-By: Bab
-00000200: 656c 2032 2e31 342e 300a 00              el 2.14.0..
+00000200: 656c 2032 2e31 352e 300a 00              el 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 1% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 000001a0: 213d 2031 293b 0a4d 494d 452d 5665 7273  != 1);.MIME-Vers
 000001b0: 696f 6e3a 2031 2e30 0a43 6f6e 7465 6e74  ion: 1.0.Content
 000001c0: 2d54 7970 653a 2074 6578 742f 706c 6169  -Type: text/plai
 000001d0: 6e3b 2063 6861 7273 6574 3d75 7466 2d38  n; charset=utf-8
 000001e0: 0a43 6f6e 7465 6e74 2d54 7261 6e73 6665  .Content-Transfe
 000001f0: 722d 456e 636f 6469 6e67 3a20 3862 6974  r-Encoding: 8bit
 00000200: 0a47 656e 6572 6174 6564 2d42 793a 2042  .Generated-By: B
-00000210: 6162 656c 2032 2e31 342e 300a 00         abel 2.14.0..
+00000210: 6162 656c 2032 2e31 352e 300a 00         abel 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language-Team: Spanish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/es/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "Best match"
 msgstr "Mejor coincidencia"
 
 msgid "Files support must be enabled."
 msgstr "El respaldo de archivos debe estar activado."
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 1% similar despite different names*

```diff
@@ -29,9 +29,9 @@
 000001c0: 3020 3f20 3120 3a20 323b 0a4d 494d 452d  0 ? 1 : 2;.MIME-
 000001d0: 5665 7273 696f 6e3a 2031 2e30 0a43 6f6e  Version: 1.0.Con
 000001e0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
 000001f0: 706c 6169 6e3b 2063 6861 7273 6574 3d75  plain; charset=u
 00000200: 7466 2d38 0a43 6f6e 7465 6e74 2d54 7261  tf-8.Content-Tra
 00000210: 6e73 6665 722d 456e 636f 6469 6e67 3a20  nsfer-Encoding: 
 00000220: 3862 6974 0a47 656e 6572 6174 6564 2d42  8bit.Generated-B
-00000230: 793a 2042 6162 656c 2032 2e31 342e 300a  y: Babel 2.14.0.
+00000230: 793a 2042 6162 656c 2032 2e31 352e 300a  y: Babel 2.15.0.
 00000240: 00                                       .
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -29,9 +29,9 @@
 000001c0: 3d20 3020 3f20 3120 3a20 323b 0a4d 494d  = 0 ? 1 : 2;.MIM
 000001d0: 452d 5665 7273 696f 6e3a 2031 2e30 0a43  E-Version: 1.0.C
 000001e0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
 000001f0: 742f 706c 6169 6e3b 2063 6861 7273 6574  t/plain; charset
 00000200: 3d75 7466 2d38 0a43 6f6e 7465 6e74 2d54  =utf-8.Content-T
 00000210: 7261 6e73 6665 722d 456e 636f 6469 6e67  ransfer-Encoding
 00000220: 3a20 3862 6974 0a47 656e 6572 6174 6564  : 8bit.Generated
-00000230: 2d42 793a 2042 6162 656c 2032 2e31 342e  -By: Babel 2.14.
+00000230: 2d42 793a 2042 6162 656c 2032 2e31 352e  -By: Babel 2.15.
 00000240: 300a 00                                  0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: et\n"
 "Language-Team: Estonian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/et/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "Best match"
 msgstr "Parim vaste"
 
 msgid "Files support must be enabled."
 msgstr "Failide tugi peab olema lubatud."
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 1% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 000001a0: 2021 3d20 3129 3b0a 4d49 4d45 2d56 6572   != 1);.MIME-Ver
 000001b0: 7369 6f6e 3a20 312e 300a 436f 6e74 656e  sion: 1.0.Conten
 000001c0: 742d 5479 7065 3a20 7465 7874 2f70 6c61  t-Type: text/pla
 000001d0: 696e 3b20 6368 6172 7365 743d 7574 662d  in; charset=utf-
 000001e0: 380a 436f 6e74 656e 742d 5472 616e 7366  8.Content-Transf
 000001f0: 6572 2d45 6e63 6f64 696e 673a 2038 6269  er-Encoding: 8bi
 00000200: 740a 4765 6e65 7261 7465 642d 4279 3a20  t.Generated-By: 
-00000210: 4261 6265 6c20 322e 3134 2e30 0a00       Babel 2.14.0..
+00000210: 4261 6265 6c20 322e 3135 2e30 0a00       Babel 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 00000190: 3e20 3129 3b0a 4d49 4d45 2d56 6572 7369  > 1);.MIME-Versi
 000001a0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
 000001b0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
 000001c0: 3b20 6368 6172 7365 743d 7574 662d 380a  ; charset=utf-8.
 000001d0: 436f 6e74 656e 742d 5472 616e 7366 6572  Content-Transfer
 000001e0: 2d45 6e63 6f64 696e 673a 2038 6269 740a  -Encoding: 8bit.
 000001f0: 4765 6e65 7261 7465 642d 4279 3a20 4261  Generated-By: Ba
-00000200: 6265 6c20 322e 3134 2e30 0a00            bel 2.14.0..
+00000200: 6265 6c20 322e 3135 2e30 0a00            bel 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 eb01 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 ee01 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d64 7261 6674 732d   invenio-drafts-
 00000050: 7265 736f 7572 6365 7320 302e 3138 2e32  resources 0.18.2
 00000060: 0a52 6570 6f72 742d 4d73 6769 642d 4275  .Report-Msgid-Bu
 00000070: 6773 2d54 6f3a 2069 6e66 6f40 696e 7665  gs-To: info@inve
 00000080: 6e69 6f73 6f66 7477 6172 652e 6f72 670a  niosoftware.org.
 00000090: 504f 542d 4372 6561 7469 6f6e 2d44 6174  POT-Creation-Dat
 000000a0: 653a 2032 3032 322d 3130 2d31 3220 3039  e: 2022-10-12 09
 000000b0: 3a30 372b 3030 3030 0a50 4f2d 5265 7669  :07+0000.PO-Revi
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
-00000110: 7561 6765 3a20 6661 5f49 520a 4c61 6e67  uage: fa_IR.Lang
-00000120: 7561 6765 2d54 6561 6d3a 2050 6572 7369  uage-Team: Persi
-00000130: 616e 2028 4972 616e 2920 2868 7474 7073  an (Iran) (https
-00000140: 3a2f 2f61 7070 2e74 7261 6e73 6966 6578  ://app.transifex
-00000150: 2e63 6f6d 2f69 6e76 656e 696f 736f 6674  .com/inveniosoft
-00000160: 7761 7265 2f74 6561 6d73 2f32 3335 3337  ware/teams/23537
-00000170: 2f66 615f 4952 2f29 0a50 6c75 7261 6c2d  /fa_IR/).Plural-
-00000180: 466f 726d 733a 206e 706c 7572 616c 733d  Forms: nplurals=
-00000190: 323b 2070 6c75 7261 6c3d 286e 203e 2031  2; plural=(n > 1
-000001a0: 293b 0a4d 494d 452d 5665 7273 696f 6e3a  );.MIME-Version:
-000001b0: 2031 2e30 0a43 6f6e 7465 6e74 2d54 7970   1.0.Content-Typ
-000001c0: 653a 2074 6578 742f 706c 6169 6e3b 2063  e: text/plain; c
-000001d0: 6861 7273 6574 3d75 7466 2d38 0a43 6f6e  harset=utf-8.Con
-000001e0: 7465 6e74 2d54 7261 6e73 6665 722d 456e  tent-Transfer-En
-000001f0: 636f 6469 6e67 3a20 3862 6974 0a47 656e  coding: 8bit.Gen
-00000200: 6572 6174 6564 2d42 793a 2042 6162 656c  erated-By: Babel
-00000210: 2032 2e31 342e 300a 00                    2.14.0..
+00000110: 7561 6765 3a20 7376 5f53 450a 4c61 6e67  uage: sv_SE.Lang
+00000120: 7561 6765 2d54 6561 6d3a 2053 7765 6469  uage-Team: Swedi
+00000130: 7368 2028 5377 6564 656e 2920 2868 7474  sh (Sweden) (htt
+00000140: 7073 3a2f 2f61 7070 2e74 7261 6e73 6966  ps://app.transif
+00000150: 6578 2e63 6f6d 2f69 6e76 656e 696f 736f  ex.com/invenioso
+00000160: 6674 7761 7265 2f74 6561 6d73 2f32 3335  ftware/teams/235
+00000170: 3337 2f73 765f 5345 2f29 0a50 6c75 7261  37/sv_SE/).Plura
+00000180: 6c2d 466f 726d 733a 206e 706c 7572 616c  l-Forms: nplural
+00000190: 733d 323b 2070 6c75 7261 6c3d 286e 2021  s=2; plural=(n !
+000001a0: 3d20 3129 3b0a 4d49 4d45 2d56 6572 7369  = 1);.MIME-Versi
+000001b0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
+000001c0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
+000001d0: 3b20 6368 6172 7365 743d 7574 662d 380a  ; charset=utf-8.
+000001e0: 436f 6e74 656e 742d 5472 616e 7366 6572  Content-Transfer
+000001f0: 2d45 6e63 6f64 696e 673a 2038 6269 740a  -Encoding: 8bit.
+00000200: 4765 6e65 7261 7465 642d 4279 3a20 4261  Generated-By: Ba
+00000210: 6265 6c20 322e 3135 2e30 0a00            bel 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,11 +9,11 @@
 "Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/"
 "fr/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "Version"
 msgstr "Version"
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 000001e0: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
 000001f0: 300a 436f 6e74 656e 742d 5479 7065 3a20  0.Content-Type: 
 00000200: 7465 7874 2f70 6c61 696e 3b20 6368 6172  text/plain; char
 00000210: 7365 743d 7574 662d 380a 436f 6e74 656e  set=utf-8.Conten
 00000220: 742d 5472 616e 7366 6572 2d45 6e63 6f64  t-Transfer-Encod
 00000230: 696e 673a 2038 6269 740a 4765 6e65 7261  ing: 8bit.Genera
 00000240: 7465 642d 4279 3a20 4261 6265 6c20 322e  ted-By: Babel 2.
-00000250: 3134 2e30 0a00                           14.0..
+00000250: 3135 2e30 0a00                           15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 1% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 000001d0: 2031 203a 2032 3b0a 4d49 4d45 2d56 6572   1 : 2;.MIME-Ver
 000001e0: 7369 6f6e 3a20 312e 300a 436f 6e74 656e  sion: 1.0.Conten
 000001f0: 742d 5479 7065 3a20 7465 7874 2f70 6c61  t-Type: text/pla
 00000200: 696e 3b20 6368 6172 7365 743d 7574 662d  in; charset=utf-
 00000210: 380a 436f 6e74 656e 742d 5472 616e 7366  8.Content-Transf
 00000220: 6572 2d45 6e63 6f64 696e 673a 2038 6269  er-Encoding: 8bi
 00000230: 740a 4765 6e65 7261 7465 642d 4279 3a20  t.Generated-By: 
-00000240: 4261 6265 6c20 322e 3134 2e30 0a00       Babel 2.14.0..
+00000240: 4261 6265 6c20 322e 3135 2e30 0a00       Babel 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 e001 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 e101 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d64 7261 6674 732d   invenio-drafts-
 00000050: 7265 736f 7572 6365 7320 302e 3138 2e32  resources 0.18.2
 00000060: 0a52 6570 6f72 742d 4d73 6769 642d 4275  .Report-Msgid-Bu
 00000070: 6773 2d54 6f3a 2069 6e66 6f40 696e 7665  gs-To: info@inve
 00000080: 6e69 6f73 6f66 7477 6172 652e 6f72 670a  niosoftware.org.
 00000090: 504f 542d 4372 6561 7469 6f6e 2d44 6174  POT-Creation-Dat
 000000a0: 653a 2032 3032 322d 3130 2d31 3220 3039  e: 2022-10-12 09
 000000b0: 3a30 372b 3030 3030 0a50 4f2d 5265 7669  :07+0000.PO-Revi
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
-00000110: 7561 6765 3a20 676c 0a4c 616e 6775 6167  uage: gl.Languag
-00000120: 652d 5465 616d 3a20 4761 6c69 6369 616e  e-Team: Galician
-00000130: 2028 6874 7470 733a 2f2f 6170 702e 7472   (https://app.tr
-00000140: 616e 7369 6665 782e 636f 6d2f 696e 7665  ansifex.com/inve
-00000150: 6e69 6f73 6f66 7477 6172 652f 7465 616d  niosoftware/team
-00000160: 732f 3233 3533 372f 676c 2f29 0a50 6c75  s/23537/gl/).Plu
-00000170: 7261 6c2d 466f 726d 733a 206e 706c 7572  ral-Forms: nplur
-00000180: 616c 733d 323b 2070 6c75 7261 6c3d 286e  als=2; plural=(n
-00000190: 2021 3d20 3129 3b0a 4d49 4d45 2d56 6572   != 1);.MIME-Ver
-000001a0: 7369 6f6e 3a20 312e 300a 436f 6e74 656e  sion: 1.0.Conten
-000001b0: 742d 5479 7065 3a20 7465 7874 2f70 6c61  t-Type: text/pla
-000001c0: 696e 3b20 6368 6172 7365 743d 7574 662d  in; charset=utf-
-000001d0: 380a 436f 6e74 656e 742d 5472 616e 7366  8.Content-Transf
-000001e0: 6572 2d45 6e63 6f64 696e 673a 2038 6269  er-Encoding: 8bi
-000001f0: 740a 4765 6e65 7261 7465 642d 4279 3a20  t.Generated-By: 
-00000200: 4261 6265 6c20 322e 3134 2e30 0a00       Babel 2.14.0..
+00000110: 7561 6765 3a20 6e6f 0a4c 616e 6775 6167  uage: no.Languag
+00000120: 652d 5465 616d 3a20 4e6f 7277 6567 6961  e-Team: Norwegia
+00000130: 6e20 2868 7474 7073 3a2f 2f61 7070 2e74  n (https://app.t
+00000140: 7261 6e73 6966 6578 2e63 6f6d 2f69 6e76  ransifex.com/inv
+00000150: 656e 696f 736f 6674 7761 7265 2f74 6561  eniosoftware/tea
+00000160: 6d73 2f32 3335 3337 2f6e 6f2f 290a 506c  ms/23537/no/).Pl
+00000170: 7572 616c 2d46 6f72 6d73 3a20 6e70 6c75  ural-Forms: nplu
+00000180: 7261 6c73 3d32 3b20 706c 7572 616c 3d28  rals=2; plural=(
+00000190: 6e20 213d 2031 293b 0a4d 494d 452d 5665  n != 1);.MIME-Ve
+000001a0: 7273 696f 6e3a 2031 2e30 0a43 6f6e 7465  rsion: 1.0.Conte
+000001b0: 6e74 2d54 7970 653a 2074 6578 742f 706c  nt-Type: text/pl
+000001c0: 6169 6e3b 2063 6861 7273 6574 3d75 7466  ain; charset=utf
+000001d0: 2d38 0a43 6f6e 7465 6e74 2d54 7261 6e73  -8.Content-Trans
+000001e0: 6665 722d 456e 636f 6469 6e67 3a20 3862  fer-Encoding: 8b
+000001f0: 6974 0a47 656e 6572 6174 6564 2d42 793a  it.Generated-By:
+00000200: 2042 6162 656c 2032 2e31 352e 300a 00     Babel 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 000001a0: 293b 0a4d 494d 452d 5665 7273 696f 6e3a  );.MIME-Version:
 000001b0: 2031 2e30 0a43 6f6e 7465 6e74 2d54 7970   1.0.Content-Typ
 000001c0: 653a 2074 6578 742f 706c 6169 6e3b 2063  e: text/plain; c
 000001d0: 6861 7273 6574 3d75 7466 2d38 0a43 6f6e  harset=utf-8.Con
 000001e0: 7465 6e74 2d54 7261 6e73 6665 722d 456e  tent-Transfer-En
 000001f0: 636f 6469 6e67 3a20 3862 6974 0a47 656e  coding: 8bit.Gen
 00000200: 6572 6174 6564 2d42 793a 2042 6162 656c  erated-By: Babel
-00000210: 2032 2e31 342e 300a 00                    2.14.0..
+00000210: 2032 2e31 352e 300a 00                    2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 2802 0000 2d00 0000 0050 726f  ,...(...-....Pro
+00000020: 2c00 0000 1502 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d64 7261 6674 732d   invenio-drafts-
 00000050: 7265 736f 7572 6365 7320 302e 3138 2e32  resources 0.18.2
 00000060: 0a52 6570 6f72 742d 4d73 6769 642d 4275  .Report-Msgid-Bu
 00000070: 6773 2d54 6f3a 2069 6e66 6f40 696e 7665  gs-To: info@inve
 00000080: 6e69 6f73 6f66 7477 6172 652e 6f72 670a  niosoftware.org.
 00000090: 504f 542d 4372 6561 7469 6f6e 2d44 6174  POT-Creation-Dat
 000000a0: 653a 2032 3032 322d 3130 2d31 3220 3039  e: 2022-10-12 09
 000000b0: 3a30 372b 3030 3030 0a50 4f2d 5265 7669  :07+0000.PO-Revi
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
-00000110: 7561 6765 3a20 6872 0a4c 616e 6775 6167  uage: hr.Languag
-00000120: 652d 5465 616d 3a20 4372 6f61 7469 616e  e-Team: Croatian
-00000130: 2028 6874 7470 733a 2f2f 6170 702e 7472   (https://app.tr
-00000140: 616e 7369 6665 782e 636f 6d2f 696e 7665  ansifex.com/inve
-00000150: 6e69 6f73 6f66 7477 6172 652f 7465 616d  niosoftware/team
-00000160: 732f 3233 3533 372f 6872 2f29 0a50 6c75  s/23537/hr/).Plu
-00000170: 7261 6c2d 466f 726d 733a 206e 706c 7572  ral-Forms: nplur
-00000180: 616c 733d 333b 2070 6c75 7261 6c3d 6e25  als=3; plural=n%
-00000190: 3130 3d3d 3120 2626 206e 2531 3030 213d  10==1 && n%100!=
-000001a0: 3131 203f 2030 203a 206e 2531 303e 3d32  11 ? 0 : n%10>=2
-000001b0: 2026 2620 6e25 3130 3c3d 3420 2626 2028   && n%10<=4 && (
-000001c0: 6e25 3130 303c 3130 207c 7c20 6e25 3130  n%100<10 || n%10
-000001d0: 303e 3d32 3029 203f 2031 203a 2032 3b0a  0>=20) ? 1 : 2;.
-000001e0: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
-000001f0: 300a 436f 6e74 656e 742d 5479 7065 3a20  0.Content-Type: 
-00000200: 7465 7874 2f70 6c61 696e 3b20 6368 6172  text/plain; char
-00000210: 7365 743d 7574 662d 380a 436f 6e74 656e  set=utf-8.Conten
-00000220: 742d 5472 616e 7366 6572 2d45 6e63 6f64  t-Transfer-Encod
-00000230: 696e 673a 2038 6269 740a 4765 6e65 7261  ing: 8bit.Genera
-00000240: 7465 642d 4279 3a20 4261 6265 6c20 322e  ted-By: Babel 2.
-00000250: 3134 2e30 0a00                           14.0..
+00000110: 7561 6765 3a20 7074 0a4c 616e 6775 6167  uage: pt.Languag
+00000120: 652d 5465 616d 3a20 506f 7274 7567 7565  e-Team: Portugue
+00000130: 7365 2028 6874 7470 733a 2f2f 6170 702e  se (https://app.
+00000140: 7472 616e 7369 6665 782e 636f 6d2f 696e  transifex.com/in
+00000150: 7665 6e69 6f73 6f66 7477 6172 652f 7465  veniosoftware/te
+00000160: 616d 732f 3233 3533 372f 7074 2f29 0a50  ams/23537/pt/).P
+00000170: 6c75 7261 6c2d 466f 726d 733a 206e 706c  lural-Forms: npl
+00000180: 7572 616c 733d 333b 2070 6c75 7261 6c3d  urals=3; plural=
+00000190: 286e 203d 3d20 3020 7c7c 206e 203d 3d20  (n == 0 || n == 
+000001a0: 3129 203f 2030 203a 206e 2021 3d20 3020  1) ? 0 : n != 0 
+000001b0: 2626 206e 2025 2031 3030 3030 3030 203d  && n % 1000000 =
+000001c0: 3d20 3020 3f20 3120 3a20 323b 0a4d 494d  = 0 ? 1 : 2;.MIM
+000001d0: 452d 5665 7273 696f 6e3a 2031 2e30 0a43  E-Version: 1.0.C
+000001e0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+000001f0: 742f 706c 6169 6e3b 2063 6861 7273 6574  t/plain; charset
+00000200: 3d75 7466 2d38 0a43 6f6e 7465 6e74 2d54  =utf-8.Content-T
+00000210: 7261 6e73 6665 722d 456e 636f 6469 6e67  ransfer-Encoding
+00000220: 3a20 3862 6974 0a47 656e 6572 6174 6564  : 8bit.Generated
+00000230: 2d42 793a 2042 6162 656c 2032 2e31 352e  -By: Babel 2.15.
+00000240: 300a 00                                  0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: hu\n"
 "Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/hu/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "Best match"
 msgstr "Legjobb találat"
 
 msgid "Files support must be enabled."
 msgstr "A fájlok támogatását engedélyezni kell."
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 1% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 000001a0: 6e20 213d 2031 293b 0a4d 494d 452d 5665  n != 1);.MIME-Ve
 000001b0: 7273 696f 6e3a 2031 2e30 0a43 6f6e 7465  rsion: 1.0.Conte
 000001c0: 6e74 2d54 7970 653a 2074 6578 742f 706c  nt-Type: text/pl
 000001d0: 6169 6e3b 2063 6861 7273 6574 3d75 7466  ain; charset=utf
 000001e0: 2d38 0a43 6f6e 7465 6e74 2d54 7261 6e73  -8.Content-Trans
 000001f0: 6665 722d 456e 636f 6469 6e67 3a20 3862  fer-Encoding: 8b
 00000200: 6974 0a47 656e 6572 6174 6564 2d42 793a  it.Generated-By:
-00000210: 2042 6162 656c 2032 2e31 342e 300a 00     Babel 2.14.0..
+00000210: 2042 6162 656c 2032 2e31 352e 300a 00     Babel 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,11 +9,11 @@
 "Language-Team: Italian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/it/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "Version"
 msgstr "Versione"
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 d901 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 e301 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d64 7261 6674 732d   invenio-drafts-
 00000050: 7265 736f 7572 6365 7320 302e 3138 2e32  resources 0.18.2
 00000060: 0a52 6570 6f72 742d 4d73 6769 642d 4275  .Report-Msgid-Bu
 00000070: 6773 2d54 6f3a 2069 6e66 6f40 696e 7665  gs-To: info@inve
 00000080: 6e69 6f73 6f66 7477 6172 652e 6f72 670a  niosoftware.org.
 00000090: 504f 542d 4372 6561 7469 6f6e 2d44 6174  POT-Creation-Dat
 000000a0: 653a 2032 3032 322d 3130 2d31 3220 3039  e: 2022-10-12 09
 000000b0: 3a30 372b 3030 3030 0a50 4f2d 5265 7669  :07+0000.PO-Revi
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
-00000110: 7561 6765 3a20 6a61 0a4c 616e 6775 6167  uage: ja.Languag
-00000120: 652d 5465 616d 3a20 4a61 7061 6e65 7365  e-Team: Japanese
-00000130: 2028 6874 7470 733a 2f2f 6170 702e 7472   (https://app.tr
-00000140: 616e 7369 6665 782e 636f 6d2f 696e 7665  ansifex.com/inve
-00000150: 6e69 6f73 6f66 7477 6172 652f 7465 616d  niosoftware/team
-00000160: 732f 3233 3533 372f 6a61 2f29 0a50 6c75  s/23537/ja/).Plu
-00000170: 7261 6c2d 466f 726d 733a 206e 706c 7572  ral-Forms: nplur
-00000180: 616c 733d 313b 2070 6c75 7261 6c3d 303b  als=1; plural=0;
-00000190: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
-000001a0: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
-000001b0: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
-000001c0: 7273 6574 3d75 7466 2d38 0a43 6f6e 7465  rset=utf-8.Conte
-000001d0: 6e74 2d54 7261 6e73 6665 722d 456e 636f  nt-Transfer-Enco
-000001e0: 6469 6e67 3a20 3862 6974 0a47 656e 6572  ding: 8bit.Gener
-000001f0: 6174 6564 2d42 793a 2042 6162 656c 2032  ated-By: Babel 2
-00000200: 2e31 342e 300a 00                        .14.0..
+00000110: 7561 6765 3a20 7277 0a4c 616e 6775 6167  uage: rw.Languag
+00000120: 652d 5465 616d 3a20 4b69 6e79 6172 7761  e-Team: Kinyarwa
+00000130: 6e64 6120 2868 7474 7073 3a2f 2f61 7070  nda (https://app
+00000140: 2e74 7261 6e73 6966 6578 2e63 6f6d 2f69  .transifex.com/i
+00000150: 6e76 656e 696f 736f 6674 7761 7265 2f74  nveniosoftware/t
+00000160: 6561 6d73 2f32 3335 3337 2f72 772f 290a  eams/23537/rw/).
+00000170: 506c 7572 616c 2d46 6f72 6d73 3a20 6e70  Plural-Forms: np
+00000180: 6c75 7261 6c73 3d32 3b20 706c 7572 616c  lurals=2; plural
+00000190: 3d28 6e20 213d 2031 293b 0a4d 494d 452d  =(n != 1);.MIME-
+000001a0: 5665 7273 696f 6e3a 2031 2e30 0a43 6f6e  Version: 1.0.Con
+000001b0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+000001c0: 706c 6169 6e3b 2063 6861 7273 6574 3d75  plain; charset=u
+000001d0: 7466 2d38 0a43 6f6e 7465 6e74 2d54 7261  tf-8.Content-Tra
+000001e0: 6e73 6665 722d 456e 636f 6469 6e67 3a20  nsfer-Encoding: 
+000001f0: 3862 6974 0a47 656e 6572 6174 6564 2d42  8bit.Generated-B
+00000200: 793a 2042 6162 656c 2032 2e31 352e 300a  y: Babel 2.15.0.
+00000210: 00                                       .
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 000000a0: 653a 2032 3032 322d 3130 2d31 3220 3039  e: 2022-10-12 09
 000000b0: 3a30 372b 3030 3030 0a50 4f2d 5265 7669  :07+0000.PO-Revi
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
-00000110: 7561 6765 3a20 6b61 0a4c 616e 6775 6167  uage: ka.Languag
-00000120: 652d 5465 616d 3a20 4765 6f72 6769 616e  e-Team: Georgian
-00000130: 2028 6874 7470 733a 2f2f 6170 702e 7472   (https://app.tr
-00000140: 616e 7369 6665 782e 636f 6d2f 696e 7665  ansifex.com/inve
-00000150: 6e69 6f73 6f66 7477 6172 652f 7465 616d  niosoftware/team
-00000160: 732f 3233 3533 372f 6b61 2f29 0a50 6c75  s/23537/ka/).Plu
-00000170: 7261 6c2d 466f 726d 733a 206e 706c 7572  ral-Forms: nplur
-00000180: 616c 733d 323b 2070 6c75 7261 6c3d 286e  als=2; plural=(n
-00000190: 213d 3129 3b0a 4d49 4d45 2d56 6572 7369  !=1);.MIME-Versi
+00000110: 7561 6765 3a20 6e65 0a4c 616e 6775 6167  uage: ne.Languag
+00000120: 652d 5465 616d 3a20 4e65 7061 6c69 2028  e-Team: Nepali (
+00000130: 6874 7470 733a 2f2f 6170 702e 7472 616e  https://app.tran
+00000140: 7369 6665 782e 636f 6d2f 696e 7665 6e69  sifex.com/inveni
+00000150: 6f73 6f66 7477 6172 652f 7465 616d 732f  osoftware/teams/
+00000160: 3233 3533 372f 6e65 2f29 0a50 6c75 7261  23537/ne/).Plura
+00000170: 6c2d 466f 726d 733a 206e 706c 7572 616c  l-Forms: nplural
+00000180: 733d 323b 2070 6c75 7261 6c3d 286e 2021  s=2; plural=(n !
+00000190: 3d20 3129 3b0a 4d49 4d45 2d56 6572 7369  = 1);.MIME-Versi
 000001a0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
 000001b0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
 000001c0: 3b20 6368 6172 7365 743d 7574 662d 380a  ; charset=utf-8.
 000001d0: 436f 6e74 656e 742d 5472 616e 7366 6572  Content-Transfer
 000001e0: 2d45 6e63 6f64 696e 673a 2038 6269 740a  -Encoding: 8bit.
 000001f0: 4765 6e65 7261 7465 642d 4279 3a20 4261  Generated-By: Ba
-00000200: 6265 6c20 322e 3134 2e30 0a00            bel 2.14.0..
+00000200: 6265 6c20 322e 3135 2e30 0a00            bel 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -34,9 +34,9 @@
 00000210: 3d20 3020 3f20 323a 2033 293b 0a4d 494d  = 0 ? 2: 3);.MIM
 00000220: 452d 5665 7273 696f 6e3a 2031 2e30 0a43  E-Version: 1.0.C
 00000230: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
 00000240: 742f 706c 6169 6e3b 2063 6861 7273 6574  t/plain; charset
 00000250: 3d75 7466 2d38 0a43 6f6e 7465 6e74 2d54  =utf-8.Content-T
 00000260: 7261 6e73 6665 722d 456e 636f 6469 6e67  ransfer-Encoding
 00000270: 3a20 3862 6974 0a47 656e 6572 6174 6564  : 8bit.Generated
-00000280: 2d42 793a 2042 6162 656c 2032 2e31 342e  -By: Babel 2.14.
+00000280: 2d42 793a 2042 6162 656c 2032 2e31 352e  -By: Babel 2.15.
 00000290: 300a 00                                  0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/messages.pot` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 de01 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 eb01 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d64 7261 6674 732d   invenio-drafts-
 00000050: 7265 736f 7572 6365 7320 302e 3138 2e32  resources 0.18.2
 00000060: 0a52 6570 6f72 742d 4d73 6769 642d 4275  .Report-Msgid-Bu
 00000070: 6773 2d54 6f3a 2069 6e66 6f40 696e 7665  gs-To: info@inve
 00000080: 6e69 6f73 6f66 7477 6172 652e 6f72 670a  niosoftware.org.
 00000090: 504f 542d 4372 6561 7469 6f6e 2d44 6174  POT-Creation-Dat
 000000a0: 653a 2032 3032 322d 3130 2d31 3220 3039  e: 2022-10-12 09
 000000b0: 3a30 372b 3030 3030 0a50 4f2d 5265 7669  :07+0000.PO-Revi
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
-00000110: 7561 6765 3a20 6e65 0a4c 616e 6775 6167  uage: ne.Languag
-00000120: 652d 5465 616d 3a20 4e65 7061 6c69 2028  e-Team: Nepali (
-00000130: 6874 7470 733a 2f2f 6170 702e 7472 616e  https://app.tran
-00000140: 7369 6665 782e 636f 6d2f 696e 7665 6e69  sifex.com/inveni
-00000150: 6f73 6f66 7477 6172 652f 7465 616d 732f  osoftware/teams/
-00000160: 3233 3533 372f 6e65 2f29 0a50 6c75 7261  23537/ne/).Plura
-00000170: 6c2d 466f 726d 733a 206e 706c 7572 616c  l-Forms: nplural
-00000180: 733d 323b 2070 6c75 7261 6c3d 286e 2021  s=2; plural=(n !
-00000190: 3d20 3129 3b0a 4d49 4d45 2d56 6572 7369  = 1);.MIME-Versi
-000001a0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
-000001b0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
-000001c0: 3b20 6368 6172 7365 743d 7574 662d 380a  ; charset=utf-8.
-000001d0: 436f 6e74 656e 742d 5472 616e 7366 6572  Content-Transfer
-000001e0: 2d45 6e63 6f64 696e 673a 2038 6269 740a  -Encoding: 8bit.
-000001f0: 4765 6e65 7261 7465 642d 4279 3a20 4261  Generated-By: Ba
-00000200: 6265 6c20 322e 3134 2e30 0a00            bel 2.14.0..
+00000110: 7561 6765 3a20 6661 5f49 520a 4c61 6e67  uage: fa_IR.Lang
+00000120: 7561 6765 2d54 6561 6d3a 2050 6572 7369  uage-Team: Persi
+00000130: 616e 2028 4972 616e 2920 2868 7474 7073  an (Iran) (https
+00000140: 3a2f 2f61 7070 2e74 7261 6e73 6966 6578  ://app.transifex
+00000150: 2e63 6f6d 2f69 6e76 656e 696f 736f 6674  .com/inveniosoft
+00000160: 7761 7265 2f74 6561 6d73 2f32 3335 3337  ware/teams/23537
+00000170: 2f66 615f 4952 2f29 0a50 6c75 7261 6c2d  /fa_IR/).Plural-
+00000180: 466f 726d 733a 206e 706c 7572 616c 733d  Forms: nplurals=
+00000190: 323b 2070 6c75 7261 6c3d 286e 203e 2031  2; plural=(n > 1
+000001a0: 293b 0a4d 494d 452d 5665 7273 696f 6e3a  );.MIME-Version:
+000001b0: 2031 2e30 0a43 6f6e 7465 6e74 2d54 7970   1.0.Content-Typ
+000001c0: 653a 2074 6578 742f 706c 6169 6e3b 2063  e: text/plain; c
+000001d0: 6861 7273 6574 3d75 7466 2d38 0a43 6f6e  harset=utf-8.Con
+000001e0: 7465 6e74 2d54 7261 6e73 6665 722d 456e  tent-Transfer-En
+000001f0: 636f 6469 6e67 3a20 3862 6974 0a47 656e  coding: 8bit.Gen
+00000200: 6572 6174 6564 2d42 793a 2042 6162 656c  erated-By: Babel
+00000210: 2032 2e31 352e 300a 00                    2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 e101 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 e701 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d64 7261 6674 732d   invenio-drafts-
 00000050: 7265 736f 7572 6365 7320 302e 3138 2e32  resources 0.18.2
 00000060: 0a52 6570 6f72 742d 4d73 6769 642d 4275  .Report-Msgid-Bu
 00000070: 6773 2d54 6f3a 2069 6e66 6f40 696e 7665  gs-To: info@inve
 00000080: 6e69 6f73 6f66 7477 6172 652e 6f72 670a  niosoftware.org.
 00000090: 504f 542d 4372 6561 7469 6f6e 2d44 6174  POT-Creation-Dat
 000000a0: 653a 2032 3032 322d 3130 2d31 3220 3039  e: 2022-10-12 09
 000000b0: 3a30 372b 3030 3030 0a50 4f2d 5265 7669  :07+0000.PO-Revi
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
-00000110: 7561 6765 3a20 6e6f 0a4c 616e 6775 6167  uage: no.Languag
-00000120: 652d 5465 616d 3a20 4e6f 7277 6567 6961  e-Team: Norwegia
-00000130: 6e20 2868 7474 7073 3a2f 2f61 7070 2e74  n (https://app.t
-00000140: 7261 6e73 6966 6578 2e63 6f6d 2f69 6e76  ransifex.com/inv
-00000150: 656e 696f 736f 6674 7761 7265 2f74 6561  eniosoftware/tea
-00000160: 6d73 2f32 3335 3337 2f6e 6f2f 290a 506c  ms/23537/no/).Pl
-00000170: 7572 616c 2d46 6f72 6d73 3a20 6e70 6c75  ural-Forms: nplu
-00000180: 7261 6c73 3d32 3b20 706c 7572 616c 3d28  rals=2; plural=(
-00000190: 6e20 213d 2031 293b 0a4d 494d 452d 5665  n != 1);.MIME-Ve
-000001a0: 7273 696f 6e3a 2031 2e30 0a43 6f6e 7465  rsion: 1.0.Conte
-000001b0: 6e74 2d54 7970 653a 2074 6578 742f 706c  nt-Type: text/pl
-000001c0: 6169 6e3b 2063 6861 7273 6574 3d75 7466  ain; charset=utf
-000001d0: 2d38 0a43 6f6e 7465 6e74 2d54 7261 6e73  -8.Content-Trans
-000001e0: 6665 722d 456e 636f 6469 6e67 3a20 3862  fer-Encoding: 8b
-000001f0: 6974 0a47 656e 6572 6174 6564 2d42 793a  it.Generated-By:
-00000200: 2042 6162 656c 2032 2e31 342e 300a 00     Babel 2.14.0..
+00000110: 7561 6765 3a20 7a68 5f54 570a 4c61 6e67  uage: zh_TW.Lang
+00000120: 7561 6765 2d54 6561 6d3a 2043 6869 6e65  uage-Team: Chine
+00000130: 7365 2028 5461 6977 616e 2920 2868 7474  se (Taiwan) (htt
+00000140: 7073 3a2f 2f61 7070 2e74 7261 6e73 6966  ps://app.transif
+00000150: 6578 2e63 6f6d 2f69 6e76 656e 696f 736f  ex.com/invenioso
+00000160: 6674 7761 7265 2f74 6561 6d73 2f32 3335  ftware/teams/235
+00000170: 3337 2f7a 685f 5457 2f29 0a50 6c75 7261  37/zh_TW/).Plura
+00000180: 6c2d 466f 726d 733a 206e 706c 7572 616c  l-Forms: nplural
+00000190: 733d 313b 2070 6c75 7261 6c3d 303b 0a4d  s=1; plural=0;.M
+000001a0: 494d 452d 5665 7273 696f 6e3a 2031 2e30  IME-Version: 1.0
+000001b0: 0a43 6f6e 7465 6e74 2d54 7970 653a 2074  .Content-Type: t
+000001c0: 6578 742f 706c 6169 6e3b 2063 6861 7273  ext/plain; chars
+000001d0: 6574 3d75 7466 2d38 0a43 6f6e 7465 6e74  et=utf-8.Content
+000001e0: 2d54 7261 6e73 6665 722d 456e 636f 6469  -Transfer-Encodi
+000001f0: 6e67 3a20 3862 6974 0a47 656e 6572 6174  ng: 8bit.Generat
+00000200: 6564 2d42 793a 2042 6162 656c 2032 2e31  ed-By: Babel 2.1
+00000210: 352e 300a 00                             5.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 00000220: 3220 3a20 3329 3b0a 4d49 4d45 2d56 6572  2 : 3);.MIME-Ver
 00000230: 7369 6f6e 3a20 312e 300a 436f 6e74 656e  sion: 1.0.Conten
 00000240: 742d 5479 7065 3a20 7465 7874 2f70 6c61  t-Type: text/pla
 00000250: 696e 3b20 6368 6172 7365 743d 7574 662d  in; charset=utf-
 00000260: 380a 436f 6e74 656e 742d 5472 616e 7366  8.Content-Transf
 00000270: 6572 2d45 6e63 6f64 696e 673a 2038 6269  er-Encoding: 8bi
 00000280: 740a 4765 6e65 7261 7465 642d 4279 3a20  t.Generated-By: 
-00000290: 4261 6265 6c20 322e 3134 2e30 0a00       Babel 2.14.0..
+00000290: 4261 6265 6c20 322e 3135 2e30 0a00       Babel 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -0,0 +1,19 @@
+msgid ""
+msgstr ""
+"Project-Id-Version: invenio-drafts-resources 0.18.2\n"
+"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
+"POT-Creation-Date: 2022-10-12 09:07+0000\n"
+"PO-Revision-Date: 2021-07-13 12:40+0000\n"
+"Last-Translator: Ivan Masár <helix84@centrum.sk>, 2021\n"
+"Language: sk\n"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/"
+"sk/)\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"MIME-Version: 1.0\n"
+"Content-Type: text/plain; charset=utf-8\n"
+"Content-Transfer-Encoding: 8bit\n"
+"Generated-By: Babel 2.15.0\n"
+
+msgid "Version"
+msgstr "Verzia"
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 000001c0: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
 000001d0: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
 000001e0: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
 000001f0: 7273 6574 3d75 7466 2d38 0a43 6f6e 7465  rset=utf-8.Conte
 00000200: 6e74 2d54 7261 6e73 6665 722d 456e 636f  nt-Transfer-Enco
 00000210: 6469 6e67 3a20 3862 6974 0a47 656e 6572  ding: 8bit.Gener
 00000220: 6174 6564 2d42 793a 2042 6162 656c 2032  ated-By: Babel 2
-00000230: 2e31 342e 300a 00                        .14.0..
+00000230: 2e31 352e 300a 00                        .15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 00000220: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
 00000230: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
 00000240: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
 00000250: 7273 6574 3d75 7466 2d38 0a43 6f6e 7465  rset=utf-8.Conte
 00000260: 6e74 2d54 7261 6e73 6665 722d 456e 636f  nt-Transfer-Enco
 00000270: 6469 6e67 3a20 3862 6974 0a47 656e 6572  ding: 8bit.Gener
 00000280: 6174 6564 2d42 793a 2042 6162 656c 2032  ated-By: Babel 2
-00000290: 2e31 342e 300a 00                        .14.0..
+00000290: 2e31 352e 300a 00                        .15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: sv\n"
 "Language-Team: Swedish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/sv/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "Best match"
 msgstr "Bästa matchningen"
 
 msgid "Files support must be enabled."
 msgstr "Filstöd måste vara aktiverat."
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 ee01 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 e001 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d64 7261 6674 732d   invenio-drafts-
 00000050: 7265 736f 7572 6365 7320 302e 3138 2e32  resources 0.18.2
 00000060: 0a52 6570 6f72 742d 4d73 6769 642d 4275  .Report-Msgid-Bu
 00000070: 6773 2d54 6f3a 2069 6e66 6f40 696e 7665  gs-To: info@inve
 00000080: 6e69 6f73 6f66 7477 6172 652e 6f72 670a  niosoftware.org.
 00000090: 504f 542d 4372 6561 7469 6f6e 2d44 6174  POT-Creation-Dat
 000000a0: 653a 2032 3032 322d 3130 2d31 3220 3039  e: 2022-10-12 09
 000000b0: 3a30 372b 3030 3030 0a50 4f2d 5265 7669  :07+0000.PO-Revi
 000000c0: 7369 6f6e 2d44 6174 653a 2032 3032 312d  sion-Date: 2021-
 000000d0: 3037 2d31 3320 3132 3a34 302b 3030 3030  07-13 12:40+0000
 000000e0: 0a4c 6173 742d 5472 616e 736c 6174 6f72  .Last-Translator
 000000f0: 3a20 4655 4c4c 204e 414d 4520 3c45 4d41  : FULL NAME <EMA
 00000100: 494c 4041 4444 5245 5353 3e0a 4c61 6e67  IL@ADDRESS>.Lang
-00000110: 7561 6765 3a20 7376 5f53 450a 4c61 6e67  uage: sv_SE.Lang
-00000120: 7561 6765 2d54 6561 6d3a 2053 7765 6469  uage-Team: Swedi
-00000130: 7368 2028 5377 6564 656e 2920 2868 7474  sh (Sweden) (htt
-00000140: 7073 3a2f 2f61 7070 2e74 7261 6e73 6966  ps://app.transif
-00000150: 6578 2e63 6f6d 2f69 6e76 656e 696f 736f  ex.com/invenioso
-00000160: 6674 7761 7265 2f74 6561 6d73 2f32 3335  ftware/teams/235
-00000170: 3337 2f73 765f 5345 2f29 0a50 6c75 7261  37/sv_SE/).Plura
-00000180: 6c2d 466f 726d 733a 206e 706c 7572 616c  l-Forms: nplural
-00000190: 733d 323b 2070 6c75 7261 6c3d 286e 2021  s=2; plural=(n !
-000001a0: 3d20 3129 3b0a 4d49 4d45 2d56 6572 7369  = 1);.MIME-Versi
-000001b0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
-000001c0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
-000001d0: 3b20 6368 6172 7365 743d 7574 662d 380a  ; charset=utf-8.
-000001e0: 436f 6e74 656e 742d 5472 616e 7366 6572  Content-Transfer
-000001f0: 2d45 6e63 6f64 696e 673a 2038 6269 740a  -Encoding: 8bit.
-00000200: 4765 6e65 7261 7465 642d 4279 3a20 4261  Generated-By: Ba
-00000210: 6265 6c20 322e 3134 2e30 0a00            bel 2.14.0..
+00000110: 7561 6765 3a20 676c 0a4c 616e 6775 6167  uage: gl.Languag
+00000120: 652d 5465 616d 3a20 4761 6c69 6369 616e  e-Team: Galician
+00000130: 2028 6874 7470 733a 2f2f 6170 702e 7472   (https://app.tr
+00000140: 616e 7369 6665 782e 636f 6d2f 696e 7665  ansifex.com/inve
+00000150: 6e69 6f73 6f66 7477 6172 652f 7465 616d  niosoftware/team
+00000160: 732f 3233 3533 372f 676c 2f29 0a50 6c75  s/23537/gl/).Plu
+00000170: 7261 6c2d 466f 726d 733a 206e 706c 7572  ral-Forms: nplur
+00000180: 616c 733d 323b 2070 6c75 7261 6c3d 286e  als=2; plural=(n
+00000190: 2021 3d20 3129 3b0a 4d49 4d45 2d56 6572   != 1);.MIME-Ver
+000001a0: 7369 6f6e 3a20 312e 300a 436f 6e74 656e  sion: 1.0.Conten
+000001b0: 742d 5479 7065 3a20 7465 7874 2f70 6c61  t-Type: text/pla
+000001c0: 696e 3b20 6368 6172 7365 743d 7574 662d  in; charset=utf-
+000001d0: 380a 436f 6e74 656e 742d 5472 616e 7366  8.Content-Transf
+000001e0: 6572 2d45 6e63 6f64 696e 673a 2038 6269  er-Encoding: 8bi
+000001f0: 740a 4765 6e65 7261 7465 642d 4279 3a20  t.Generated-By: 
+00000200: 4261 6265 6c20 322e 3135 2e30 0a00       Babel 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language: tr\n"
 "Language-Team: Turkish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/tr/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "Best match"
 msgstr "En iyi eşleşme"
 
 msgid "Files support must be enabled."
 msgstr "Dosya desteği etkinleştirilmelidir."
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -11,15 +11,15 @@
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
 "11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
 "100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
 "(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "Best match"
 msgstr "Найкраща відповідність"
 
 msgid "Least recently updated"
 msgstr "Найбільш давно не оновлювались"
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-drafts-resources 0.18.2*

 * *Files 2% similar despite different names*

```diff
@@ -41,8 +41,8 @@
 00000280: 323a 2033 293b 0a4d 494d 452d 5665 7273  2: 3);.MIME-Vers
 00000290: 696f 6e3a 2031 2e30 0a43 6f6e 7465 6e74  ion: 1.0.Content
 000002a0: 2d54 7970 653a 2074 6578 742f 706c 6169  -Type: text/plai
 000002b0: 6e3b 2063 6861 7273 6574 3d75 7466 2d38  n; charset=utf-8
 000002c0: 0a43 6f6e 7465 6e74 2d54 7261 6e73 6665  .Content-Transfe
 000002d0: 722d 456e 636f 6469 6e67 3a20 3862 6974  r-Encoding: 8bit
 000002e0: 0a47 656e 6572 6174 6564 2d42 793a 2042  .Generated-By: B
-000002f0: 6162 656c 2032 2e31 342e 300a 00         abel 2.14.0..
+000002f0: 6162 656c 2032 2e31 352e 300a 00         abel 2.15.0..
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: zh_CN\n"
 "Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/"
 "teams/23537/zh_CN/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "Best match"
 msgstr "最佳匹配"
 
 msgid "Files support must be enabled."
 msgstr "必须启用文件支持。"
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources.egg-info/PKG-INFO` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-drafts-resources
-Version: 3.0.0
+Version: 3.1.0
 Summary: Invenio Drafts Resources module to create REST APIs
 Home-page: https://github.com/inveniosoftware/Invenio-Drafts-Resources
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Keywords: invenio records deposit submit versioning drafts
 Platform: any
@@ -58,14 +58,18 @@
     Invenio-Drafts-Resources is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 3.1.0 (released 2024-05-03)
+
+- media-files: prevent copying to new version
+
 Version 3.0.0 (released 2024-01-31)
 
 - installation: bump dependencies
 - uow: add "bulk_index" param on ParentRecordCommmitOp
 
 Version 2.0.2 (2023-11-07)
```

### Comparing `invenio-drafts-resources-3.0.0/invenio_drafts_resources.egg-info/SOURCES.txt` & `invenio-drafts-resources-3.1.0/invenio_drafts_resources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/run-tests.sh` & `invenio-drafts-resources-3.1.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/setup.cfg` & `invenio-drafts-resources-3.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/conftest.py` & `invenio-drafts-resources-3.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/mock_module/api.py` & `invenio-drafts-resources-3.1.0/tests/mock_module/api.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json` & `invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json` & `invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json` & `invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json` & `invenio-drafts-resources-3.1.0/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json` & `invenio-drafts-resources-3.1.0/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json` & `invenio-drafts-resources-3.1.0/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/mock_module/models.py` & `invenio-drafts-resources-3.1.0/tests/mock_module/models.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/mock_module/permissions.py` & `invenio-drafts-resources-3.1.0/tests/mock_module/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/mock_module/resource.py` & `invenio-drafts-resources-3.1.0/tests/mock_module/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/mock_module/schemas.py` & `invenio-drafts-resources-3.1.0/tests/mock_module/schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/mock_module/service.py` & `invenio-drafts-resources-3.1.0/tests/mock_module/service.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/records/conftest.py` & `invenio-drafts-resources-3.1.0/tests/records/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/records/test_api.py` & `invenio-drafts-resources-3.1.0/tests/records/test_api.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/resources/conftest.py` & `invenio-drafts-resources-3.1.0/tests/resources/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/resources/test_files_resource.py` & `invenio-drafts-resources-3.1.0/tests/resources/test_files_resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/resources/test_record_resource.py` & `invenio-drafts-resources-3.1.0/tests/resources/test_record_resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/resources/test_resource_links.py` & `invenio-drafts-resources-3.1.0/tests/resources/test_resource_links.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/services/conftest.py` & `invenio-drafts-resources-3.1.0/tests/services/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/services/test_record_service.py` & `invenio-drafts-resources-3.1.0/tests/services/test_record_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020-2021 CERN.
+# Copyright (C) 2020-2024 CERN.
 # Copyright (C) 2020-2021 Northwestern University.
 #
 # Invenio-Drafts-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Service tests.
@@ -12,19 +12,17 @@
 Test to add:
 - Read a tombstone page
 - Read with missing permissions
 - Read with missing pid
 """
 
 import pytest
-from invenio_db import db
 from invenio_pidstore.errors import PIDDoesNotExistError, PIDUnregistered
 from invenio_pidstore.models import PIDStatus
 from marshmallow.exceptions import ValidationError
-from sqlalchemy.orm.exc import NoResultFound
 
 from .utils import create_and_publish
 
 #
 # Operations tests
 #
```

### Comparing `invenio-drafts-resources-3.0.0/tests/services/test_record_service_files.py` & `invenio-drafts-resources-3.1.0/tests/services/test_record_service_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020-2023 CERN.
+# Copyright (C) 2020-2024 CERN.
 # Copyright (C) 2020-2021 Northwestern University.
 #
 # Invenio-Drafts-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Service tests.
@@ -316,32 +316,37 @@
         service_with_media_files.draft_files, draft.id, "test2", identity_simple
     )
     service.publish(identity_simple, draft.id)
 
     # New version
     draft = service.new_version(identity_simple, draft.id)
 
-    # objects: 1 media file of the record + 1 file of the record
-    # + 1 media file of the draft (copied to new version) = 3
+    # New versions start with the default files config, i.e. disabled media files, so
+    # we need to enable them.
+    data = draft.to_dict()
+    data["media_files"] = {"enabled": True}
+    draft = service.update_draft(identity_simple, draft.id, data)
+
+    # objects: 1 media file of the record + 1 file of the record = 2
     # file instances: 1 media file of the draft, 1 media file of the new version record
-    assert_counts(buckets=4, objs=3, fileinstances=2, filedrafts=0, filerecords=1)
+    assert_counts(buckets=4, objs=2, fileinstances=2, filedrafts=0, filerecords=1)
 
     # Add file
     add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
     # add media file
     add_file_to_draft(
         service_with_media_files.draft_files, draft.id, "test23", identity_simple
     )
 
-    # objects: added 1 file and 1 media file = 5
-    assert_counts(buckets=4, objs=5, fileinstances=4, filedrafts=1, filerecords=1)
+    # objects: added 1 file and 1 media file = 4
+    assert_counts(buckets=4, objs=4, fileinstances=4, filedrafts=1, filerecords=1)
 
     # Publish
     service.publish(identity_simple, draft.id)
-    assert_counts(buckets=4, objs=5, fileinstances=4, filedrafts=0, filerecords=2)
+    assert_counts(buckets=4, objs=4, fileinstances=4, filedrafts=0, filerecords=2)
 
 
 def test_new_version_delete(app, db, service, input_data, identity_simple):
     """Test new version."""
     # Create, publish, new_version, add_file
     draft = service.create(identity_simple, input_data)
     add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
@@ -364,23 +369,29 @@
     draft = service.create(identity_simple, input_data)
     add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
     add_file_to_draft(
         service_with_media_files.draft_files, draft.id, "test2", identity_simple
     )
     service.publish(identity_simple, draft.id)
     draft = service.new_version(identity_simple, draft.id)
+
+    # New versions start with the default files config, i.e. disabled media files, so
+    # we need to enable them.
+    data = draft.to_dict()
+    data["media_files"] = {"enabled": True}
+    draft = service.update_draft(identity_simple, draft.id, data)
+
     add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
     add_file_to_draft(
         service_with_media_files.draft_files, draft.id, "test23", identity_simple
     )
 
-    # objects: 1 media file of the record + 1 file of the record
-    #           + 1 media file of the draft (copied to new version) = 3
+    # objects: 1 media file of the record + 1 file of the record = 2
     #           + 1 media file in a new version + 1 regular file in a new version
-    assert_counts(buckets=4, objs=5, fileinstances=4, filedrafts=1, filerecords=1)
+    assert_counts(buckets=4, objs=4, fileinstances=4, filedrafts=1, filerecords=1)
 
     # Delete new version
     service.delete_draft(identity_simple, draft.id)
     assert_counts(buckets=2, objs=2, fileinstances=4, filedrafts=0, filerecords=1)
 
 
 #
@@ -397,15 +408,15 @@
 
     # Import files
     service.import_files(identity_simple, draft.id)
     assert_counts(buckets=4, objs=2, fileinstances=1, filedrafts=1, filerecords=1)
 
 
 def test_import_files_disabled(app, db, service, input_data, identity_simple):
-    """Test new version."""
+    """Test new version of record with disabled files."""
     # Create, publish, new_version
     input_data["files"]["enabled"] = False
     draft = service.create(identity_simple, input_data)
     service.publish(identity_simple, draft.id)
     draft = service.new_version(identity_simple, draft.id)
     assert_counts(buckets=4, objs=0, fileinstances=0, filedrafts=0, filerecords=0)
```

### Comparing `invenio-drafts-resources-3.0.0/tests/services/test_record_service_search.py` & `invenio-drafts-resources-3.1.0/tests/services/test_record_service_search.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/services/test_record_service_tasks.py` & `invenio-drafts-resources-3.1.0/tests/services/test_record_service_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/services/test_records_uow.py` & `invenio-drafts-resources-3.1.0/tests/services/test_records_uow.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/services/test_services.py` & `invenio-drafts-resources-3.1.0/tests/services/test_services.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-3.0.0/tests/services/utils.py` & `invenio-drafts-resources-3.1.0/tests/services/utils.py`

 * *Files identical despite different names*

