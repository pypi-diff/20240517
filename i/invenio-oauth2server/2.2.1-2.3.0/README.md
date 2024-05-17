# Comparing `tmp/invenio-oauth2server-2.2.1.tar.gz` & `tmp/invenio-oauth2server-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-oauth2server-2.2.1.tar", last modified: Tue Oct 31 16:00:51 2023, max compression
+gzip compressed data, was "dist/invenio-oauth2server-2.3.0.tar", last modified: Fri Mar 22 16:42:33 2024, max compression
```

## Comparing `invenio-oauth2server-2.2.1.tar` & `invenio-oauth2server-2.3.0.tar`

### file list

```diff
@@ -1,320 +1,310 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/.tx/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/.tx/config
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10351 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/examplesapp.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/docs/images/
--rwxr-xr-x   0 runner    (1001) docker     (127)    15165 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/images/authorization-code.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)     8247 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/images/client-credentials.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    13811 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/images/implicit-grant.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      860 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    10987 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)      666 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/examples/app-fixtures.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      893 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/examples/app-setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      229 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/examples/app-teardown.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/examples/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    14540 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/examples/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/examples/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/examples/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/examples/templates/jwt.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/alembic/12a88921ada2_create_oauth2server_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/alembic/4e57407b8e4a_add_on_delete_cascade.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/alembic/aa546f2a8d2f_create_oauth2server_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)    12379 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/authorize.html
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/errors.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/_macros.html
--rw-r--r--   0 runner    (1001) docker     (127)      510 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      988 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/helpers.html
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      993 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/token_new.html
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/token_permission_view.html
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/_macros.html
--rw-r--r--   0 runner    (1001) docker     (127)      510 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/helpers.html
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_new.html
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_permission_view.html
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/theme/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/theme/semantic/
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/theme/semantic/form_styling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18246 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    23011 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18495 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18587 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    21060 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18508 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    22175 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18259 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18259 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18558 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/en_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/en_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/en_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18260 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/en_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/en_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/en_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/en_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18260 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/en_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    21903 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es_CU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es_CU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es_CU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18296 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es_CU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es_MX/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es_MX/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es_MX/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18298 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es_MX/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    21572 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18261 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18427 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fa_IR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18256 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fa_IR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    21116 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr_CI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr_CI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr_CI/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18317 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr_CI/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18309 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr_FR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18245 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hi_IN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hi_IN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18256 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hi_IN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18487 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    22013 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hu_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18262 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hu_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6281 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    20976 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18413 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18583 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18584 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)    18180 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ne/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ne/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ne/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18243 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ne/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18418 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      926 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18569 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18451 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18498 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18669 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18248 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    21107 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    21601 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sv_SE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sv_SE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18259 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sv_SE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8189 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    21910 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18709 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18484 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/uk_UA/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    21080 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18412 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/views/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/views/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/invenio_oauth2server/views/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9983 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/invenio_oauth2server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-31 16:00:50.000000 invenio-oauth2server-2.2.1/invenio_oauth2server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      457 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      842 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 16:00:51.000000 invenio-oauth2server-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    16955 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/tests/test_alembic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7981 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/tests/test_invenio_oauth2server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    37079 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2023-10-31 16:00:40.000000 invenio-oauth2server-2.2.1/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/docs/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15165 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/images/authorization-code.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8247 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/images/client-credentials.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13811 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/images/implicit-grant.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/alembic/12a88921ada2_create_oauth2server_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/alembic/4e57407b8e4a_add_on_delete_cascade.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/alembic/aa546f2a8d2f_create_oauth2server_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12379 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/authorize.html
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/errors.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/helpers.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_new.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_permission_view.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/helpers.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_new.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_permission_view.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/theme/semantic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/theme/semantic/form_styling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18246 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    23011 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18495 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18587 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    21060 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18508 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    22175 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18259 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18259 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18558 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18260 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18260 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    21903 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18298 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    21572 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18261 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18427 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18256 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    21116 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18317 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18309 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18245 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18256 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18487 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    22013 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18262 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    20976 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18413 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18583 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18584 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)    18180 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18243 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18418 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18569 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18451 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18498 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18669 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18248 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    21107 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    21601 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18259 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18709 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18484 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    21080 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-22 16:42:32.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18412 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/views/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/invenio_oauth2server/views/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/invenio_oauth2server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      842 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:42:33.000000 invenio-oauth2server-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17018 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/tests/test_alembic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/tests/test_invenio_oauth2server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37079 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-22 16:42:26.000000 invenio-oauth2server-2.3.0/tests/test_validators.py
```

### Comparing `invenio-oauth2server-2.2.1/.editorconfig` & `invenio-oauth2server-2.3.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/.github/workflows/pypi-publish.yml` & `invenio-oauth2server-2.3.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/.tx/config` & `invenio-oauth2server-2.3.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/AUTHORS.rst` & `invenio-oauth2server-2.3.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/CHANGES.rst` & `invenio-oauth2server-2.3.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.3.0 (released 2024-03-22)
+
+- fix: before_first_request deprecation
+  (add finalise app entrypoint)
+
+
 Version 2.2.1 (released 2023-10-31)
 
 - settings: simplify token query
 
 Version 2.2.0 (released 2023-09-12)
 
 - new-buttons: remove secondary class from buttons
```

### Comparing `invenio-oauth2server-2.2.1/CONTRIBUTING.rst` & `invenio-oauth2server-2.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/LICENSE` & `invenio-oauth2server-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/MANIFEST.in` & `invenio-oauth2server-2.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/PKG-INFO` & `invenio-oauth2server-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-oauth2server
-Version: 2.2.1
+Version: 2.3.0
 Summary: "Invenio module that implements OAuth 2 server."
 Home-page: https://github.com/inveniosoftware/invenio-oauth2server
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -50,14 +50,20 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.3.0 (released 2024-03-22)
+        
+        - fix: before_first_request deprecation
+          (add finalise app entrypoint)
+        
+        
         Version 2.2.1 (released 2023-10-31)
         
         - settings: simplify token query
         
         Version 2.2.0 (released 2023-09-12)
         
         - new-buttons: remove secondary class from buttons
```

### Comparing `invenio-oauth2server-2.2.1/README.rst` & `invenio-oauth2server-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/docs/Makefile` & `invenio-oauth2server-2.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/docs/api.rst` & `invenio-oauth2server-2.3.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/docs/conf.py` & `invenio-oauth2server-2.3.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,16 @@
 # Copyright (C) 2022 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Sphinx configuration."""
 
-from __future__ import print_function
-
 import sys
 
-import sphinx.environment
-
 from invenio_oauth2server import __version__
 
 # Plug example application into module path
 sys.path.append("examples")
 
 # -- General configuration ------------------------------------------------
 
@@ -35,14 +31,20 @@
     "sphinx.ext.autodoc",
     "sphinx.ext.coverage",
     "sphinx.ext.doctest",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
 ]
 
+nitpick_ignore = [
+    ("py:class", "t.ClassVar"),
+    ("py:class", "Query"),
+    ("py:attr", "query_class"),
+]
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 # source_suffix = ['.rst', '.md']
 source_suffix = ".rst"
@@ -51,15 +53,15 @@
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Invenio-OAuth2Server"
-copyright = "2017, CERN"
+copyright = "2023, CERN"
 author = "CERN"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `invenio-oauth2server-2.2.1/docs/images/authorization-code.jpg` & `invenio-oauth2server-2.3.0/docs/images/authorization-code.jpg`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/docs/images/client-credentials.jpg` & `invenio-oauth2server-2.3.0/docs/images/client-credentials.jpg`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/docs/images/implicit-grant.jpg` & `invenio-oauth2server-2.3.0/docs/images/implicit-grant.jpg`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/docs/index.rst` & `invenio-oauth2server-2.3.0/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 .. toctree::
    :maxdepth: 1
 
    overview
    installation
    configuration
    usage
-   examplesapp
 
 
 API Reference
 -------------
 
 If you are looking for information on a specific function, class or method,
 this part of the documentation is for you.
```

### Comparing `invenio-oauth2server-2.2.1/docs/make.bat` & `invenio-oauth2server-2.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/docs/overview.rst` & `invenio-oauth2server-2.3.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/__init__.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2015-2018 CERN.
-# Copyright (C) 2023 Graz University of Technology.
+# Copyright (C) 2023-2024 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio module that implements OAuth 2 server.
 
 Protecting your REST API with authentication
@@ -91,17 +91,14 @@
     def index():
         return 'Front page content.'
 
 So, finally, with this example, we would allow any authenticated client with
 rights to use the ``homepage_scope`` to read the homepage but, prevent from
 reading the email if they do not have rights for using the ``email_scope``.
 
-To test this features you can build your own application or use the provided
-:doc:`example app </examplesapp>` as boilerplate.
-
 Access control
 --------------
 
 It is important to remember that the usage of authentication and scopes is not
 enough in most of the cases so access control need to be configured as well.
 For more information about access control in Invenio you can visit
 `Invenio-Access
@@ -114,15 +111,15 @@
 
 monkey_patch_werkzeug()  # noqa isort:skip
 
 from .decorators import require_api_auth, require_oauth_scopes  # noqa isort:skip
 from .ext import InvenioOAuth2Server, InvenioOAuth2ServerREST  # noqa isort:skip
 from .proxies import current_oauth2server  # noqa isort:skip
 
-__version__ = "2.2.1"
+__version__ = "2.3.0"
 
 __all__ = (
     "__version__",
     "InvenioOAuth2Server",
     "InvenioOAuth2ServerREST",
     "require_api_auth",
     "require_oauth_scopes",
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/_compat.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/_compat.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/admin.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/admin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2016-2018 CERN.
+# Copyright (C) 2024 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Admin views for managing access to actions."""
 
 from flask_admin.contrib.sqla import ModelView
@@ -31,17 +32,17 @@
         "name",
         "description",
         "website",
         "user_id",
         "client_id",
     )
 
-    column_list = (
-        column_searchable_list
-    ) = column_sortable_list = column_details_list = list_all
+    column_list = column_searchable_list = column_sortable_list = (
+        column_details_list
+    ) = list_all
 
     column_list = list_all
     column_default_sort = ("client_id", True)
 
 
 class TokenView(ModelView):
     """View for managing access to actions by users with given role."""
@@ -52,17 +53,17 @@
     list_all = (
         "id",
         "client_id",
         "user_id",
         "token_type",
         "expires",
     )
-    column_list = (
-        column_searchable_list
-    ) = column_sortable_list = column_details_list = list_all
+    column_list = column_searchable_list = column_sortable_list = (
+        column_details_list
+    ) = list_all
 
 
 oauth2server_clients_adminview = {
     "view_class": ClientView,
     "args": [Client, db.session],
     "kwargs": {
         "name": _("OAuth Applications"),
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/alembic/12a88921ada2_create_oauth2server_tables.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/alembic/12a88921ada2_create_oauth2server_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/alembic/4e57407b8e4a_add_on_delete_cascade.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/alembic/4e57407b8e4a_add_on_delete_cascade.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/alembic/aa546f2a8d2f_create_oauth2server_branch.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/alembic/aa546f2a8d2f_create_oauth2server_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/cli.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/config.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/config.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/decorators.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/decorators.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/errors.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/ext.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/ext.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2015-2018 CERN.
 # Copyright (C) 2022 RERO.
-# Copyright (C) 2023 Graz University of Technology.
+# Copyright (C) 2023-2024 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio module that implements OAuth 2 server."""
 
 import os
 import warnings
 
 import importlib_metadata
 import oauthlib.common as oauthlib_commmon
 import six
 from flask import abort, request
 from flask_login import current_user
+from flask_menu import current_menu
+from invenio_i18n import LazyString
+from invenio_i18n import lazy_gettext as _
 from invenio_rest.csrf import csrf
 from werkzeug.utils import cached_property, import_string
 
 from . import config
 from .models import OAuthUserProxy, Scope
 from .provider import oauth2
 
@@ -280,7 +283,24 @@
             warnings.warn(
                 'You are overriding the default OAuthlib "URL encoded" set of '
                 "valid characters. Make sure that the characters defined in "
                 "oauthlib.common.urlencoded are indeed limitting your needs.",
                 RuntimeWarning,
             )
             oauthlib_commmon.urlencoded = always_safe | modified_chars
+
+
+def finalize_app(app):
+    """Finalize app."""
+    icons = app.extensions["invenio-theme"].icons
+
+    current_menu.submenu("settings.applications").register(
+        endpoint="invenio_oauth2server_settings.index",
+        text=_(
+            "%(icon)s Applications",
+            icon=LazyString(lambda: f'<i class="{icons.codepen}"></i>'),
+        ),
+        order=5,
+        active_when=lambda: request.endpoint.startswith(
+            "invenio_oauth2server_settings."
+        ),
+    )
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/forms.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/forms.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/models.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/models.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/provider.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/provider.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/scopes.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/scopes.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/authorize.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/authorize.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/errors.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/errors.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/_macros.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/helpers.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/helpers.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/index.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/index.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/token_new.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_new.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/token_permission_view.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_permission_view.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/_macros.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/helpers.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/helpers.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_new.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_new.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_permission_view.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_permission_view.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html` & `invenio-oauth2server-2.3.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/theme/semantic/form_styling.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/theme/semantic/form_styling.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/af/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/af/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 3% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 00000190: 3129 3b0a 4d49 4d45 2d56 6572 7369 6f6e  1);.MIME-Version
 000001a0: 3a20 312e 300a 436f 6e74 656e 742d 5479  : 1.0.Content-Ty
 000001b0: 7065 3a20 7465 7874 2f70 6c61 696e 3b20  pe: text/plain; 
 000001c0: 6368 6172 7365 743d 7574 662d 380a 436f  charset=utf-8.Co
 000001d0: 6e74 656e 742d 5472 616e 7366 6572 2d45  ntent-Transfer-E
 000001e0: 6e63 6f64 696e 673a 2038 6269 740a 4765  ncoding: 8bit.Ge
 000001f0: 6e65 7261 7465 642d 4279 3a20 4261 6265  nerated-By: Babe
-00000200: 6c20 322e 3133 2e31 0a00                 l 2.13.1..
+00000200: 6c20 322e 3134 2e30 0a00                 l 2.14.0..
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/af/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ar/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ar/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

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
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "%(icon)s Applications"
 msgstr "%(icon)s تطبيقات"
 
 msgid "Access token"
 msgstr "رمز ولوج"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ar/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/bg/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/bg/LC_MESSAGES/messages.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: bg\n"
 "Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/bg/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "Cancel"
 msgstr "Отказ"
 
 msgid "Delete"
 msgstr "Изтриване"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/bg/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ca/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ca/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: ca\n"
 "Language-Team: Catalan (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ca/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "Cancel"
 msgstr "Cancel·la"
 
 msgid "Create"
 msgstr "Crear"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ca/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/cs/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/cs/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/"
 "cs/)\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "%(icon)s Applications"
 msgstr "%(icon)s Aplikace"
 
 msgid "Access token"
 msgstr "Přístupový token"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/cs/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/da/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/da/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: da\n"
 "Language-Team: Danish (https://app.transifex.com/inveniosoftware/teams/23537/"
 "da/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "Cancel"
 msgstr "Afbryd"
 
 msgid "New"
 msgstr "Ny"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/da/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de/LC_MESSAGES/messages.mo`

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
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "%(icon)s Applications"
 msgstr "%(icon)s Anwendungen"
 
 msgid "Access token"
 msgstr "Zugriffstoken"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de_AT/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 2% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 000001a0: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
 000001b0: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
 000001c0: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
 000001d0: 7273 6574 3d75 7466 2d38 0a43 6f6e 7465  rset=utf-8.Conte
 000001e0: 6e74 2d54 7261 6e73 6665 722d 456e 636f  nt-Transfer-Enco
 000001f0: 6469 6e67 3a20 3862 6974 0a47 656e 6572  ding: 8bit.Gener
 00000200: 6174 6564 2d42 793a 2042 6162 656c 2032  ated-By: Babel 2
-00000210: 2e31 332e 310a 00                        .13.1..
+00000210: 2e31 342e 300a 00                        .14.0..
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de_AT/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de_DE/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de_DE/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 2% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 000001a0: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
 000001b0: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
 000001c0: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
 000001d0: 7273 6574 3d75 7466 2d38 0a43 6f6e 7465  rset=utf-8.Conte
 000001e0: 6e74 2d54 7261 6e73 6665 722d 456e 636f  nt-Transfer-Enco
 000001f0: 6469 6e67 3a20 3862 6974 0a47 656e 6572  ding: 8bit.Gener
 00000200: 6174 6564 2d42 793a 2042 6162 656c 2032  ated-By: Babel 2
-00000210: 2e31 332e 310a 00                        .13.1..
+00000210: 2e31 342e 300a 00                        .14.0..
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/de_DE/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/el/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/el/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: el\n"
 "Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/"
 "el/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "Cancel"
 msgstr "Ακύρωση"
 
 msgid "Delete"
 msgstr "Διαγραφή"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/el/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/en_AT/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 2% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 000001a0: 3b0a 4d49 4d45 2d56 6572 7369 6f6e 3a20  ;.MIME-Version: 
 000001b0: 312e 300a 436f 6e74 656e 742d 5479 7065  1.0.Content-Type
 000001c0: 3a20 7465 7874 2f70 6c61 696e 3b20 6368  : text/plain; ch
 000001d0: 6172 7365 743d 7574 662d 380a 436f 6e74  arset=utf-8.Cont
 000001e0: 656e 742d 5472 616e 7366 6572 2d45 6e63  ent-Transfer-Enc
 000001f0: 6f64 696e 673a 2038 6269 740a 4765 6e65  oding: 8bit.Gene
 00000200: 7261 7465 642d 4279 3a20 4261 6265 6c20  rated-By: Babel 
-00000210: 322e 3133 2e31 0a00                      2.13.1..
+00000210: 322e 3134 2e30 0a00                      2.14.0..
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/en_AT/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/en_HU/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es/LC_MESSAGES/messages.mo`

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
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "%(icon)s Applications"
 msgstr "%(icon)s Aplicaciones"
 
 msgid "Access token"
 msgstr "Token de acceso"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es_CU/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 0e02 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 eb01 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d6f 6175 7468 3273   invenio-oauth2s
 00000050: 6572 7665 7220 312e 332e 370a 5265 706f  erver 1.3.7.Repo
 00000060: 7274 2d4d 7367 6964 2d42 7567 732d 546f  rt-Msgid-Bugs-To
 00000070: 3a20 696e 666f 4069 6e76 656e 696f 736f  : info@invenioso
 00000080: 6674 7761 7265 2e6f 7267 0a50 4f54 2d43  ftware.org.POT-C
 00000090: 7265 6174 696f 6e2d 4461 7465 3a20 3230  reation-Date: 20
 000000a0: 3232 2d31 302d 3132 2030 393a 3236 2b30  22-10-12 09:26+0
 000000b0: 3030 300a 504f 2d52 6576 6973 696f 6e2d  000.PO-Revision-
 000000c0: 4461 7465 3a20 3230 3136 2d30 382d 3138  Date: 2016-08-18
 000000d0: 2030 383a 3033 2b30 3030 300a 4c61 7374   08:03+0000.Last
 000000e0: 2d54 7261 6e73 6c61 746f 723a 2046 554c  -Translator: FUL
 000000f0: 4c20 4e41 4d45 203c 454d 4149 4c40 4144  L NAME <EMAIL@AD
 00000100: 4452 4553 533e 0a4c 616e 6775 6167 653a  DRESS>.Language:
-00000110: 2065 735f 4355 0a4c 616e 6775 6167 652d   es_CU.Language-
-00000120: 5465 616d 3a20 5370 616e 6973 6820 2843  Team: Spanish (C
-00000130: 7562 6129 2028 6874 7470 733a 2f2f 6170  uba) (https://ap
-00000140: 702e 7472 616e 7369 6665 782e 636f 6d2f  p.transifex.com/
-00000150: 696e 7665 6e69 6f73 6f66 7477 6172 652f  inveniosoftware/
-00000160: 7465 616d 732f 3233 3533 372f 6573 5f43  teams/23537/es_C
-00000170: 552f 290a 506c 7572 616c 2d46 6f72 6d73  U/).Plural-Forms
-00000180: 3a20 6e70 6c75 7261 6c73 3d33 3b20 706c  : nplurals=3; pl
-00000190: 7572 616c 3d6e 203d 3d20 3120 3f20 3020  ural=n == 1 ? 0 
-000001a0: 3a20 6e20 213d 2030 2026 2620 6e20 2520  : n != 0 && n % 
-000001b0: 3130 3030 3030 3020 3d3d 2030 203f 2031  1000000 == 0 ? 1
-000001c0: 203a 2032 3b0a 4d49 4d45 2d56 6572 7369   : 2;.MIME-Versi
-000001d0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
-000001e0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
-000001f0: 3b20 6368 6172 7365 743d 7574 662d 380a  ; charset=utf-8.
-00000200: 436f 6e74 656e 742d 5472 616e 7366 6572  Content-Transfer
-00000210: 2d45 6e63 6f64 696e 673a 2038 6269 740a  -Encoding: 8bit.
-00000220: 4765 6e65 7261 7465 642d 4279 3a20 4261  Generated-By: Ba
-00000230: 6265 6c20 322e 3133 2e31 0a00            bel 2.13.1..
+00000110: 2065 745f 4545 0a4c 616e 6775 6167 652d   et_EE.Language-
+00000120: 5465 616d 3a20 4573 746f 6e69 616e 2028  Team: Estonian (
+00000130: 4573 746f 6e69 6129 2028 6874 7470 733a  Estonia) (https:
+00000140: 2f2f 6170 702e 7472 616e 7369 6665 782e  //app.transifex.
+00000150: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
+00000160: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
+00000170: 6574 5f45 452f 290a 506c 7572 616c 2d46  et_EE/).Plural-F
+00000180: 6f72 6d73 3a20 6e70 6c75 7261 6c73 3d32  orms: nplurals=2
+00000190: 3b20 706c 7572 616c 3d28 6e20 213d 2031  ; plural=(n != 1
+000001a0: 293b 0a4d 494d 452d 5665 7273 696f 6e3a  );.MIME-Version:
+000001b0: 2031 2e30 0a43 6f6e 7465 6e74 2d54 7970   1.0.Content-Typ
+000001c0: 653a 2074 6578 742f 706c 6169 6e3b 2063  e: text/plain; c
+000001d0: 6861 7273 6574 3d75 7466 2d38 0a43 6f6e  harset=utf-8.Con
+000001e0: 7465 6e74 2d54 7261 6e73 6665 722d 456e  tent-Transfer-En
+000001f0: 636f 6469 6e67 3a20 3862 6974 0a47 656e  coding: 8bit.Gen
+00000200: 6572 6174 6564 2d42 793a 2042 6162 656c  erated-By: Babel
+00000210: 2032 2e31 342e 300a 00                    2.14.0..
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es_CU/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es_MX/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 22% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 000001c0: 2031 203a 2032 3b0a 4d49 4d45 2d56 6572   1 : 2;.MIME-Ver
 000001d0: 7369 6f6e 3a20 312e 300a 436f 6e74 656e  sion: 1.0.Conten
 000001e0: 742d 5479 7065 3a20 7465 7874 2f70 6c61  t-Type: text/pla
 000001f0: 696e 3b20 6368 6172 7365 743d 7574 662d  in; charset=utf-
 00000200: 380a 436f 6e74 656e 742d 5472 616e 7366  8.Content-Transf
 00000210: 6572 2d45 6e63 6f64 696e 673a 2038 6269  er-Encoding: 8bi
 00000220: 740a 4765 6e65 7261 7465 642d 4279 3a20  t.Generated-By: 
-00000230: 4261 6265 6c20 322e 3133 2e31 0a00       Babel 2.13.1..
+00000230: 4261 6265 6c20 322e 3134 2e30 0a00       Babel 2.14.0..
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/es_MX/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/et/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/et/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

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
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "%(icon)s Applications"
 msgstr "%(icon)s Rakendused"
 
 msgid "Access token"
 msgstr "Ligipääsutõend"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/et/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hu_HU/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 eb01 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 ec01 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d6f 6175 7468 3273   invenio-oauth2s
 00000050: 6572 7665 7220 312e 332e 370a 5265 706f  erver 1.3.7.Repo
 00000060: 7274 2d4d 7367 6964 2d42 7567 732d 546f  rt-Msgid-Bugs-To
 00000070: 3a20 696e 666f 4069 6e76 656e 696f 736f  : info@invenioso
 00000080: 6674 7761 7265 2e6f 7267 0a50 4f54 2d43  ftware.org.POT-C
 00000090: 7265 6174 696f 6e2d 4461 7465 3a20 3230  reation-Date: 20
 000000a0: 3232 2d31 302d 3132 2030 393a 3236 2b30  22-10-12 09:26+0
 000000b0: 3030 300a 504f 2d52 6576 6973 696f 6e2d  000.PO-Revision-
 000000c0: 4461 7465 3a20 3230 3136 2d30 382d 3138  Date: 2016-08-18
 000000d0: 2030 383a 3033 2b30 3030 300a 4c61 7374   08:03+0000.Last
 000000e0: 2d54 7261 6e73 6c61 746f 723a 2046 554c  -Translator: FUL
 000000f0: 4c20 4e41 4d45 203c 454d 4149 4c40 4144  L NAME <EMAIL@AD
 00000100: 4452 4553 533e 0a4c 616e 6775 6167 653a  DRESS>.Language:
-00000110: 2065 745f 4545 0a4c 616e 6775 6167 652d   et_EE.Language-
-00000120: 5465 616d 3a20 4573 746f 6e69 616e 2028  Team: Estonian (
-00000130: 4573 746f 6e69 6129 2028 6874 7470 733a  Estonia) (https:
-00000140: 2f2f 6170 702e 7472 616e 7369 6665 782e  //app.transifex.
-00000150: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
-00000160: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
-00000170: 6574 5f45 452f 290a 506c 7572 616c 2d46  et_EE/).Plural-F
-00000180: 6f72 6d73 3a20 6e70 6c75 7261 6c73 3d32  orms: nplurals=2
-00000190: 3b20 706c 7572 616c 3d28 6e20 213d 2031  ; plural=(n != 1
-000001a0: 293b 0a4d 494d 452d 5665 7273 696f 6e3a  );.MIME-Version:
-000001b0: 2031 2e30 0a43 6f6e 7465 6e74 2d54 7970   1.0.Content-Typ
-000001c0: 653a 2074 6578 742f 706c 6169 6e3b 2063  e: text/plain; c
-000001d0: 6861 7273 6574 3d75 7466 2d38 0a43 6f6e  harset=utf-8.Con
-000001e0: 7465 6e74 2d54 7261 6e73 6665 722d 456e  tent-Transfer-En
-000001f0: 636f 6469 6e67 3a20 3862 6974 0a47 656e  coding: 8bit.Gen
-00000200: 6572 6174 6564 2d42 793a 2042 6162 656c  erated-By: Babel
-00000210: 2032 2e31 332e 310a 00                    2.13.1..
+00000110: 2068 755f 4855 0a4c 616e 6775 6167 652d   hu_HU.Language-
+00000120: 5465 616d 3a20 4875 6e67 6172 6961 6e20  Team: Hungarian 
+00000130: 2848 756e 6761 7279 2920 2868 7474 7073  (Hungary) (https
+00000140: 3a2f 2f61 7070 2e74 7261 6e73 6966 6578  ://app.transifex
+00000150: 2e63 6f6d 2f69 6e76 656e 696f 736f 6674  .com/inveniosoft
+00000160: 7761 7265 2f74 6561 6d73 2f32 3335 3337  ware/teams/23537
+00000170: 2f68 755f 4855 2f29 0a50 6c75 7261 6c2d  /hu_HU/).Plural-
+00000180: 466f 726d 733a 206e 706c 7572 616c 733d  Forms: nplurals=
+00000190: 323b 2070 6c75 7261 6c3d 286e 2021 3d20  2; plural=(n != 
+000001a0: 3129 3b0a 4d49 4d45 2d56 6572 7369 6f6e  1);.MIME-Version
+000001b0: 3a20 312e 300a 436f 6e74 656e 742d 5479  : 1.0.Content-Ty
+000001c0: 7065 3a20 7465 7874 2f70 6c61 696e 3b20  pe: text/plain; 
+000001d0: 6368 6172 7365 743d 7574 662d 380a 436f  charset=utf-8.Co
+000001e0: 6e74 656e 742d 5472 616e 7366 6572 2d45  ntent-Transfer-E
+000001f0: 6e63 6f64 696e 673a 2038 6269 740a 4765  ncoding: 8bit.Ge
+00000200: 6e65 7261 7465 642d 4279 3a20 4261 6265  nerated-By: Babe
+00000210: 6c20 322e 3134 2e30 0a00                 l 2.14.0..
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fa/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fa/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: fa\n"
 "Language-Team: Persian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/fa/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "Cancel"
 msgstr "لغو"
 
 msgid "Delete"
 msgstr "حذف"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fa/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fa_IR/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 2% similar despite different names*

```diff
@@ -26,9 +26,9 @@
 00000190: 7572 616c 3d28 6e20 3e20 3129 3b0a 4d49  ural=(n > 1);.MI
 000001a0: 4d45 2d56 6572 7369 6f6e 3a20 312e 300a  ME-Version: 1.0.
 000001b0: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
 000001c0: 7874 2f70 6c61 696e 3b20 6368 6172 7365  xt/plain; charse
 000001d0: 743d 7574 662d 380a 436f 6e74 656e 742d  t=utf-8.Content-
 000001e0: 5472 616e 7366 6572 2d45 6e63 6f64 696e  Transfer-Encodin
 000001f0: 673a 2038 6269 740a 4765 6e65 7261 7465  g: 8bit.Generate
-00000200: 642d 4279 3a20 4261 6265 6c20 322e 3133  d-By: Babel 2.13
-00000210: 2e31 0a00                                .1..
+00000200: 642d 4279 3a20 4261 6265 6c20 322e 3134  d-By: Babel 2.14
+00000210: 2e30 0a00                                .0..
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fa_IR/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/"
 "fr/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "%(icon)s Applications"
 msgstr "Applications %(icon)s"
 
 msgid "Access token"
 msgstr "Jeton d'accès"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr_CI/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 2% similar despite different names*

```diff
@@ -30,9 +30,9 @@
 000001d0: 3020 3f20 3120 3a20 323b 0a4d 494d 452d  0 ? 1 : 2;.MIME-
 000001e0: 5665 7273 696f 6e3a 2031 2e30 0a43 6f6e  Version: 1.0.Con
 000001f0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
 00000200: 706c 6169 6e3b 2063 6861 7273 6574 3d75  plain; charset=u
 00000210: 7466 2d38 0a43 6f6e 7465 6e74 2d54 7261  tf-8.Content-Tra
 00000220: 6e73 6665 722d 456e 636f 6469 6e67 3a20  nsfer-Encoding: 
 00000230: 3862 6974 0a47 656e 6572 6174 6564 2d42  8bit.Generated-B
-00000240: 793a 2042 6162 656c 2032 2e31 332e 310a  y: Babel 2.13.1.
+00000240: 793a 2042 6162 656c 2032 2e31 342e 300a  y: Babel 2.14.0.
 00000250: 00                                       .
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr_CI/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr_FR/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr_FR/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 2% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 000001d0: 323b 0a4d 494d 452d 5665 7273 696f 6e3a  2;.MIME-Version:
 000001e0: 2031 2e30 0a43 6f6e 7465 6e74 2d54 7970   1.0.Content-Typ
 000001f0: 653a 2074 6578 742f 706c 6169 6e3b 2063  e: text/plain; c
 00000200: 6861 7273 6574 3d75 7466 2d38 0a43 6f6e  harset=utf-8.Con
 00000210: 7465 6e74 2d54 7261 6e73 6665 722d 456e  tent-Transfer-En
 00000220: 636f 6469 6e67 3a20 3862 6974 0a47 656e  coding: 8bit.Gen
 00000230: 6572 6174 6564 2d42 793a 2042 6162 656c  erated-By: Babel
-00000240: 2032 2e31 332e 310a 00                    2.13.1..
+00000240: 2032 2e31 342e 300a 00                    2.14.0..
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/fr_FR/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/gl/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -0,0 +1,36 @@
+msgid ""
+msgstr ""
+"Project-Id-Version: invenio-oauth2server 1.3.7\n"
+"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
+"POT-Creation-Date: 2022-10-12 09:26+0000\n"
+"PO-Revision-Date: 2016-08-18 08:03+0000\n"
+"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
+"Language: zh_TW\n"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/"
+"teams/23537/zh_TW/)\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"MIME-Version: 1.0\n"
+"Content-Type: text/plain; charset=utf-8\n"
+"Content-Transfer-Encoding: 8bit\n"
+"Generated-By: Babel 2.14.0\n"
+
+msgid "Cancel"
+msgstr "取消"
+
+msgid "Delete"
+msgstr "刪除"
+
+msgid "Description"
+msgstr "描述"
+
+msgid "Edit"
+msgstr "編輯"
+
+msgid "Name"
+msgstr "名稱"
+
+msgid "Register"
+msgstr "註冊"
+
+msgid "or"
+msgstr "或"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/gl/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hi_IN/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hi_IN/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 4% similar despite different names*

```diff
@@ -26,9 +26,9 @@
 00000190: 7261 6c3d 286e 2021 3d20 3129 3b0a 4d49  ral=(n != 1);.MI
 000001a0: 4d45 2d56 6572 7369 6f6e 3a20 312e 300a  ME-Version: 1.0.
 000001b0: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
 000001c0: 7874 2f70 6c61 696e 3b20 6368 6172 7365  xt/plain; charse
 000001d0: 743d 7574 662d 380a 436f 6e74 656e 742d  t=utf-8.Content-
 000001e0: 5472 616e 7366 6572 2d45 6e63 6f64 696e  Transfer-Encodin
 000001f0: 673a 2038 6269 740a 4765 6e65 7261 7465  g: 8bit.Generate
-00000200: 642d 4279 3a20 4261 6265 6c20 322e 3133  d-By: Babel 2.13
-00000210: 2e31 0a00                                .1..
+00000200: 642d 4279 3a20 4261 6265 6c20 322e 3134  d-By: Babel 2.14
+00000210: 2e30 0a00                                .0..
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hi_IN/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hr/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hr/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language-Team: Croatian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/hr/)\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "Cancel"
 msgstr "Odustani"
 
 msgid "Delete"
 msgstr "Briši"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hr/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hu/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hu/LC_MESSAGES/messages.mo`

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
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "%(icon)s Applications"
 msgstr "%(icon)sAlkalmazások"
 
 msgid "Access token"
 msgstr "Hozzáférési token"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hu/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hu_HU/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/rw/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 ec01 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 de01 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d6f 6175 7468 3273   invenio-oauth2s
 00000050: 6572 7665 7220 312e 332e 370a 5265 706f  erver 1.3.7.Repo
 00000060: 7274 2d4d 7367 6964 2d42 7567 732d 546f  rt-Msgid-Bugs-To
 00000070: 3a20 696e 666f 4069 6e76 656e 696f 736f  : info@invenioso
 00000080: 6674 7761 7265 2e6f 7267 0a50 4f54 2d43  ftware.org.POT-C
 00000090: 7265 6174 696f 6e2d 4461 7465 3a20 3230  reation-Date: 20
 000000a0: 3232 2d31 302d 3132 2030 393a 3236 2b30  22-10-12 09:26+0
 000000b0: 3030 300a 504f 2d52 6576 6973 696f 6e2d  000.PO-Revision-
 000000c0: 4461 7465 3a20 3230 3136 2d30 382d 3138  Date: 2016-08-18
 000000d0: 2030 383a 3033 2b30 3030 300a 4c61 7374   08:03+0000.Last
 000000e0: 2d54 7261 6e73 6c61 746f 723a 2046 554c  -Translator: FUL
 000000f0: 4c20 4e41 4d45 203c 454d 4149 4c40 4144  L NAME <EMAIL@AD
 00000100: 4452 4553 533e 0a4c 616e 6775 6167 653a  DRESS>.Language:
-00000110: 2068 755f 4855 0a4c 616e 6775 6167 652d   hu_HU.Language-
-00000120: 5465 616d 3a20 4875 6e67 6172 6961 6e20  Team: Hungarian 
-00000130: 2848 756e 6761 7279 2920 2868 7474 7073  (Hungary) (https
-00000140: 3a2f 2f61 7070 2e74 7261 6e73 6966 6578  ://app.transifex
-00000150: 2e63 6f6d 2f69 6e76 656e 696f 736f 6674  .com/inveniosoft
-00000160: 7761 7265 2f74 6561 6d73 2f32 3335 3337  ware/teams/23537
-00000170: 2f68 755f 4855 2f29 0a50 6c75 7261 6c2d  /hu_HU/).Plural-
-00000180: 466f 726d 733a 206e 706c 7572 616c 733d  Forms: nplurals=
-00000190: 323b 2070 6c75 7261 6c3d 286e 2021 3d20  2; plural=(n != 
-000001a0: 3129 3b0a 4d49 4d45 2d56 6572 7369 6f6e  1);.MIME-Version
-000001b0: 3a20 312e 300a 436f 6e74 656e 742d 5479  : 1.0.Content-Ty
-000001c0: 7065 3a20 7465 7874 2f70 6c61 696e 3b20  pe: text/plain; 
-000001d0: 6368 6172 7365 743d 7574 662d 380a 436f  charset=utf-8.Co
-000001e0: 6e74 656e 742d 5472 616e 7366 6572 2d45  ntent-Transfer-E
-000001f0: 6e63 6f64 696e 673a 2038 6269 740a 4765  ncoding: 8bit.Ge
-00000200: 6e65 7261 7465 642d 4279 3a20 4261 6265  nerated-By: Babe
-00000210: 6c20 322e 3133 2e31 0a00                 l 2.13.1..
+00000110: 2072 770a 4c61 6e67 7561 6765 2d54 6561   rw.Language-Tea
+00000120: 6d3a 204b 696e 7961 7277 616e 6461 2028  m: Kinyarwanda (
+00000130: 6874 7470 733a 2f2f 6170 702e 7472 616e  https://app.tran
+00000140: 7369 6665 782e 636f 6d2f 696e 7665 6e69  sifex.com/inveni
+00000150: 6f73 6f66 7477 6172 652f 7465 616d 732f  osoftware/teams/
+00000160: 3233 3533 372f 7277 2f29 0a50 6c75 7261  23537/rw/).Plura
+00000170: 6c2d 466f 726d 733a 206e 706c 7572 616c  l-Forms: nplural
+00000180: 733d 323b 2070 6c75 7261 6c3d 286e 2021  s=2; plural=(n !
+00000190: 3d20 3129 3b0a 4d49 4d45 2d56 6572 7369  = 1);.MIME-Versi
+000001a0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
+000001b0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
+000001c0: 3b20 6368 6172 7365 743d 7574 662d 380a  ; charset=utf-8.
+000001d0: 436f 6e74 656e 742d 5472 616e 7366 6572  Content-Transfer
+000001e0: 2d45 6e63 6f64 696e 673a 2038 6269 740a  -Encoding: 8bit.
+000001f0: 4765 6e65 7261 7465 642d 4279 3a20 4261  Generated-By: Ba
+00000200: 6265 6c20 322e 3134 2e30 0a00            bel 2.14.0..
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/hu_HU/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/it/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/it/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language-Team: Italian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/it/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "%(icon)s Applications"
 msgstr "Applicazioni %(icon)s"
 
 msgid "Access token"
 msgstr "Access token"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/it/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ja/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ja/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: ja\n"
 "Language-Team: Japanese (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ja/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "Cancel"
 msgstr "キャンセル"
 
 msgid "Delete"
 msgstr "削除"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ja/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ka/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ka/LC_MESSAGES/messages.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: ka\n"
 "Language-Team: Georgian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ka/)\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "Cancel"
 msgstr "გაუქმება"
 
 msgid "Delete"
 msgstr "წაშლა"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ka/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/lt/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/lt/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -10,15 +10,15 @@
 "teams/23537/lt/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
 "11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
 "1 : n % 1 != 0 ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "Cancel"
 msgstr "Atšaukti"
 
 msgid "Delete"
 msgstr "Ištrinti"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/lt/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/messages.pot` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ne/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ne/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 2% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 00000190: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
 000001a0: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
 000001b0: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
 000001c0: 7273 6574 3d75 7466 2d38 0a43 6f6e 7465  rset=utf-8.Conte
 000001d0: 6e74 2d54 7261 6e73 6665 722d 456e 636f  nt-Transfer-Enco
 000001e0: 6469 6e67 3a20 3862 6974 0a47 656e 6572  ding: 8bit.Gener
 000001f0: 6174 6564 2d42 793a 2042 6162 656c 2032  ated-By: Babel 2
-00000200: 2e31 332e 310a 00                        .13.1..
+00000200: 2e31 342e 300a 00                        .14.0..
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ne/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ne/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/no/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/no/LC_MESSAGES/messages.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: no\n"
 "Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/no/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "Cancel"
 msgstr "Avbryt"
 
 msgid "Delete"
 msgstr "Slett"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/no/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/pl/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/pl/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -10,15 +10,15 @@
 "pl/)\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
 "n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "Cancel"
 msgstr "Anuluj"
 
 msgid "Delete"
 msgstr "Usuń"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/pl/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/pt/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/pt/LC_MESSAGES/messages.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language-Team: Portuguese (https://app.transifex.com/inveniosoftware/"
 "teams/23537/pt/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgid "Delete"
 msgstr "Apagar"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/pt/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ro/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ro/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language-Team: Romanian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ro/)\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
 "2:1));\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "Cancel"
 msgstr "Anulează"
 
 msgid "Delete"
 msgstr "Şterge"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ro/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ru/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ru/LC_MESSAGES/messages.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -10,15 +10,15 @@
 "teams/23537/ru/)\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "Cancel"
 msgstr "Отменить"
 
 msgid "Delete"
 msgstr "Удалить"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/ru/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/rw/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/gl/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 de01 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 db01 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d6f 6175 7468 3273   invenio-oauth2s
 00000050: 6572 7665 7220 312e 332e 370a 5265 706f  erver 1.3.7.Repo
 00000060: 7274 2d4d 7367 6964 2d42 7567 732d 546f  rt-Msgid-Bugs-To
 00000070: 3a20 696e 666f 4069 6e76 656e 696f 736f  : info@invenioso
 00000080: 6674 7761 7265 2e6f 7267 0a50 4f54 2d43  ftware.org.POT-C
 00000090: 7265 6174 696f 6e2d 4461 7465 3a20 3230  reation-Date: 20
 000000a0: 3232 2d31 302d 3132 2030 393a 3236 2b30  22-10-12 09:26+0
 000000b0: 3030 300a 504f 2d52 6576 6973 696f 6e2d  000.PO-Revision-
 000000c0: 4461 7465 3a20 3230 3136 2d30 382d 3138  Date: 2016-08-18
 000000d0: 2030 383a 3033 2b30 3030 300a 4c61 7374   08:03+0000.Last
 000000e0: 2d54 7261 6e73 6c61 746f 723a 2046 554c  -Translator: FUL
 000000f0: 4c20 4e41 4d45 203c 454d 4149 4c40 4144  L NAME <EMAIL@AD
 00000100: 4452 4553 533e 0a4c 616e 6775 6167 653a  DRESS>.Language:
-00000110: 2072 770a 4c61 6e67 7561 6765 2d54 6561   rw.Language-Tea
-00000120: 6d3a 204b 696e 7961 7277 616e 6461 2028  m: Kinyarwanda (
-00000130: 6874 7470 733a 2f2f 6170 702e 7472 616e  https://app.tran
-00000140: 7369 6665 782e 636f 6d2f 696e 7665 6e69  sifex.com/inveni
-00000150: 6f73 6f66 7477 6172 652f 7465 616d 732f  osoftware/teams/
-00000160: 3233 3533 372f 7277 2f29 0a50 6c75 7261  23537/rw/).Plura
-00000170: 6c2d 466f 726d 733a 206e 706c 7572 616c  l-Forms: nplural
-00000180: 733d 323b 2070 6c75 7261 6c3d 286e 2021  s=2; plural=(n !
-00000190: 3d20 3129 3b0a 4d49 4d45 2d56 6572 7369  = 1);.MIME-Versi
-000001a0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
-000001b0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
-000001c0: 3b20 6368 6172 7365 743d 7574 662d 380a  ; charset=utf-8.
-000001d0: 436f 6e74 656e 742d 5472 616e 7366 6572  Content-Transfer
-000001e0: 2d45 6e63 6f64 696e 673a 2038 6269 740a  -Encoding: 8bit.
-000001f0: 4765 6e65 7261 7465 642d 4279 3a20 4261  Generated-By: Ba
-00000200: 6265 6c20 322e 3133 2e31 0a00            bel 2.13.1..
+00000110: 2067 6c0a 4c61 6e67 7561 6765 2d54 6561   gl.Language-Tea
+00000120: 6d3a 2047 616c 6963 6961 6e20 2868 7474  m: Galician (htt
+00000130: 7073 3a2f 2f61 7070 2e74 7261 6e73 6966  ps://app.transif
+00000140: 6578 2e63 6f6d 2f69 6e76 656e 696f 736f  ex.com/invenioso
+00000150: 6674 7761 7265 2f74 6561 6d73 2f32 3335  ftware/teams/235
+00000160: 3337 2f67 6c2f 290a 506c 7572 616c 2d46  37/gl/).Plural-F
+00000170: 6f72 6d73 3a20 6e70 6c75 7261 6c73 3d32  orms: nplurals=2
+00000180: 3b20 706c 7572 616c 3d28 6e20 213d 2031  ; plural=(n != 1
+00000190: 293b 0a4d 494d 452d 5665 7273 696f 6e3a  );.MIME-Version:
+000001a0: 2031 2e30 0a43 6f6e 7465 6e74 2d54 7970   1.0.Content-Typ
+000001b0: 653a 2074 6578 742f 706c 6169 6e3b 2063  e: text/plain; c
+000001c0: 6861 7273 6574 3d75 7466 2d38 0a43 6f6e  harset=utf-8.Con
+000001d0: 7465 6e74 2d54 7261 6e73 6665 722d 456e  tent-Transfer-En
+000001e0: 636f 6469 6e67 3a20 3862 6974 0a47 656e  coding: 8bit.Gen
+000001f0: 6572 6174 6564 2d42 793a 2042 6162 656c  erated-By: Babel
+00000200: 2032 2e31 342e 300a 00                    2.14.0..
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/rw/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sk/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sk/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/"
 "sk/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
 ">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "%(icon)s Applications"
 msgstr "%(icon)s Aplikácie"
 
 msgid "Access token"
 msgstr "Prístupový token"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sk/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sv/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sv/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

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
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "%(icon)s Applications"
 msgstr "%(icon)s Applikationer"
 
 msgid "Access token"
 msgstr "Åtkomsttoken"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sv/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sv_SE/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sv_SE/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 2% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 000001a0: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
 000001b0: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
 000001c0: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
 000001d0: 7273 6574 3d75 7466 2d38 0a43 6f6e 7465  rset=utf-8.Conte
 000001e0: 6e74 2d54 7261 6e73 6665 722d 456e 636f  nt-Transfer-Enco
 000001f0: 6469 6e67 3a20 3862 6974 0a47 656e 6572  ding: 8bit.Gener
 00000200: 6174 6564 2d42 793a 2042 6162 656c 2032  ated-By: Babel 2
-00000210: 2e31 332e 310a 00                        .13.1..
+00000210: 2e31 342e 300a 00                        .14.0..
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/sv_SE/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/tr/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/tr/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

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
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "%(icon)s Applications"
 msgstr "%(icon)s Uygulamalar"
 
 msgid "Access token"
 msgstr "Erişim belirteci"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/tr/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/uk/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/uk/LC_MESSAGES/messages.mo`

 * *Files 12% similar despite different names*

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
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "Cancel"
 msgstr "Скасувати"
 
 msgid "Delete"
 msgstr "Видалити"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/uk/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/uk_UA/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 2% similar despite different names*

```diff
@@ -41,8 +41,8 @@
 00000280: 3b0a 4d49 4d45 2d56 6572 7369 6f6e 3a20  ;.MIME-Version: 
 00000290: 312e 300a 436f 6e74 656e 742d 5479 7065  1.0.Content-Type
 000002a0: 3a20 7465 7874 2f70 6c61 696e 3b20 6368  : text/plain; ch
 000002b0: 6172 7365 743d 7574 662d 380a 436f 6e74  arset=utf-8.Cont
 000002c0: 656e 742d 5472 616e 7366 6572 2d45 6e63  ent-Transfer-Enc
 000002d0: 6f64 696e 673a 2038 6269 740a 4765 6e65  oding: 8bit.Gene
 000002e0: 7261 7465 642d 4279 3a20 4261 6265 6c20  rated-By: Babel 
-000002f0: 322e 3133 2e31 0a00                      2.13.1..
+000002f0: 322e 3134 2e30 0a00                      2.14.0..
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/uk_UA/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.mo`

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
-"Generated-By: Babel 2.13.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "%(icon)s Applications"
 msgstr "%(icon)s应用程序"
 
 msgid "Access token"
 msgstr "访问标识"
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.3.0/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/utils.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/validators.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/validators.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/views/server.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/views/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,15 @@
     abort,
     current_app,
     jsonify,
     redirect,
     render_template,
     request,
 )
-from flask_breadcrumbs import register_breadcrumb
 from flask_login import login_required
-from invenio_i18n import lazy_gettext as _
 from oauthlib.oauth2.rfc6749.errors import InvalidClientError, OAuth2Error
 
 from ..models import Client
 from ..provider import oauth2
 from ..proxies import current_oauth2server
 
 blueprint = Blueprint(
@@ -57,15 +55,14 @@
     return decorated
 
 
 #
 # Views
 #
 @blueprint.route("/authorize", methods=["GET", "POST"])
-@register_breadcrumb(blueprint, ".", _("Authorize application"))
 @login_required
 @error_handler
 @oauth2.authorize_handler
 def authorize(*args, **kwargs):
     """View for rendering authorization request."""
     if request.method == "GET":
         client = Client.query.filter_by(client_id=kwargs.get("client_id")).first()
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server/views/settings.py` & `invenio-oauth2server-2.3.0/invenio_oauth2server/views/settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,21 +9,16 @@
 
 
 """OAuth Server Settings Blueprint."""
 
 from functools import wraps
 
 from flask import Blueprint, abort, redirect, render_template, request, session, url_for
-from flask_breadcrumbs import register_breadcrumb
 from flask_login import current_user, login_required
-from flask_menu import register_menu
 from invenio_db import db
-from invenio_i18n import lazy_gettext as _
-from invenio_theme.proxies import current_theme_icons
-from speaklater import make_lazy_string
 
 from ..forms import ClientForm, TokenForm
 from ..models import Client, Token
 from ..proxies import current_oauth2server
 
 blueprint = Blueprint(
     "invenio_oauth2server_settings",
@@ -92,25 +87,14 @@
 
 
 #
 # Views
 #
 @blueprint.route("/", methods=["GET", "POST"])
 @login_required
-@register_menu(
-    blueprint,
-    "settings.applications",
-    _(
-        "%(icon)s Applications",
-        icon=make_lazy_string(lambda: f'<i class="{current_theme_icons.codepen}"></i>'),
-    ),
-    order=5,
-    active_when=lambda: request.endpoint.startswith("invenio_oauth2server_settings."),
-)
-@register_breadcrumb(blueprint, "breadcrumbs.settings.applications", _("Applications"))
 def index():
     """List user tokens."""
     clients = Client.query.filter_by(
         user_id=current_user.get_id(),
         is_internal=False,
     ).all()
 
@@ -142,17 +126,14 @@
         tokens=tokens,
         authorized_apps=authorized_apps,
     )
 
 
 @blueprint.route("/clients/new/", methods=["GET", "POST"])
 @login_required
-@register_breadcrumb(
-    blueprint, "breadcrumbs.settings.applications.client_new", _("New")
-)
 def client_new():
     """Create new client."""
     form = ClientForm(request.form)
 
     if form.validate_on_submit():
         c = Client(user_id=current_user.get_id())
         c.gen_salt()
@@ -165,17 +146,14 @@
         "invenio_oauth2server/settings/client_new.html",
         form=form,
     )
 
 
 @blueprint.route("/clients/<string:client_id>/", methods=["GET", "POST"])
 @login_required
-@register_breadcrumb(
-    blueprint, "breadcrumbs.settings.applications.client_edit", _("Edit")
-)
 @client_getter()
 def client_view(client):
     """Show client's detail."""
     if request.method == "POST" and "delete" in request.form:
         db.session.delete(client)
         db.session.commit()
         return redirect(url_for(".index"))
@@ -204,15 +182,14 @@
 
 
 #
 # Token views
 #
 @blueprint.route("/tokens/new/", methods=["GET", "POST"])
 @login_required
-@register_breadcrumb(blueprint, "breadcrumbs.settings.applications.token_new", _("New"))
 def token_new():
     """Create new token."""
     form = TokenForm(request.form)
     form.scopes.choices = current_oauth2server.scope_choices()
 
     if form.validate_on_submit():
         t = Token.create_personal(
@@ -229,17 +206,14 @@
         "invenio_oauth2server/settings/token_new.html",
         form=form,
     )
 
 
 @blueprint.route("/tokens/<string:token_id>/", methods=["GET", "POST"])
 @login_required
-@register_breadcrumb(
-    blueprint, "breadcrumbs.settings.applications.token_edit", _("Edit")
-)
 @token_getter()
 def token_view(token):
     """Show token details."""
     if request.method == "POST" and "delete" in request.form:
         db.session.delete(token)
         db.session.commit()
         return redirect(url_for(".index"))
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server.egg-info/PKG-INFO` & `invenio-oauth2server-2.3.0/invenio_oauth2server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-oauth2server
-Version: 2.2.1
+Version: 2.3.0
 Summary: "Invenio module that implements OAuth 2 server."
 Home-page: https://github.com/inveniosoftware/invenio-oauth2server
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -50,14 +50,20 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.3.0 (released 2024-03-22)
+        
+        - fix: before_first_request deprecation
+          (add finalise app entrypoint)
+        
+        
         Version 2.2.1 (released 2023-10-31)
         
         - settings: simplify token query
         
         Version 2.2.0 (released 2023-09-12)
         
         - new-buttons: remove secondary class from buttons
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server.egg-info/SOURCES.txt` & `invenio-oauth2server-2.3.0/invenio_oauth2server.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,32 +22,24 @@
 docs/Makefile
 docs/api.rst
 docs/authors.rst
 docs/changes.rst
 docs/conf.py
 docs/configuration.rst
 docs/contributing.rst
-docs/examplesapp.rst
 docs/index.rst
 docs/installation.rst
 docs/license.rst
 docs/make.bat
 docs/overview.rst
 docs/requirements.txt
 docs/usage.rst
 docs/images/authorization-code.jpg
 docs/images/client-credentials.jpg
 docs/images/implicit-grant.jpg
-examples/app-fixtures.sh
-examples/app-setup.sh
-examples/app-teardown.sh
-examples/app.py
-examples/consumer.py
-examples/requirements.txt
-examples/templates/jwt.html
 invenio_oauth2server/__init__.py
 invenio_oauth2server/_compat.py
 invenio_oauth2server/admin.py
 invenio_oauth2server/cli.py
 invenio_oauth2server/config.py
 invenio_oauth2server/decorators.py
 invenio_oauth2server/errors.py
```

### Comparing `invenio-oauth2server-2.2.1/invenio_oauth2server.egg-info/entry_points.txt` & `invenio-oauth2server-2.3.0/invenio_oauth2server.egg-info/entry_points.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 [invenio_base.apps]
 invenio_oauth2server = invenio_oauth2server:InvenioOAuth2Server
 
 [invenio_base.blueprints]
 invenio_oauth2server = invenio_oauth2server.views.server:blueprint
 invenio_oauth2server_settings = invenio_oauth2server.views.settings:blueprint
 
+[invenio_base.finalize_app]
+invenio_oauth2server = invenio_oauth2server.ext:finalize_app
+
 [invenio_base.secret_key]
 invenio_oauth2server = invenio_oauth2server.utils:rebuild_access_tokens
 
 [invenio_db.alembic]
 invenio_oauth2server = invenio_oauth2server:alembic
 
 [invenio_db.models]
```

### Comparing `invenio-oauth2server-2.2.1/run-tests.sh` & `invenio-oauth2server-2.3.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/setup.cfg` & `invenio-oauth2server-2.3.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -15,31 +15,30 @@
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.7
 zip_safe = False
 install_requires = 
 	cachelib>=0.1
-	Flask-Breadcrumbs>=0.4.0
 	Flask-OAuthlib>=0.9.5
 	Flask-WTF>=0.14.3
 	future>=0.16.0
-	invenio-accounts>=1.3.1
-	invenio-base>=1.2.4
+	invenio-accounts>=5.0.0
+	invenio-base>=1.3.0
 	invenio-i18n>=2.0.0
-	invenio-theme>=1.3.4
+	invenio-theme>=3.0.0
 	pyjwt>=1.5.0
 	requests-oauthlib>=1.1.0,<1.2.0
 	WTForms-Alchemy>=0.15.0
 	WTForms>=2.3.3,<3.0.0
 	importlib_metadata>=4.4
 
 [options.extras_require]
 tests = 
-	pytest-black>=0.3.0,<0.3.10
+	pytest-black-ng>=0.4.0
 	pytest-invenio>=1.4.0
 	invenio-admin>=1.2.1
 	sphinx>=4.5
 	redis>=2.10.5
 	invenio-db[mysql,postgresql,versioning]>=1.0.9,<2.0.0
 admin = 
 docs = 
@@ -68,14 +67,16 @@
 	invenio_oauth2server = invenio_oauth2server.models
 invenio_oauth2server.scopes = 
 	oauth_email = invenio_oauth2server.scopes:email_scope
 invenio_i18n.translations = 
 	messages = invenio_oauth2server
 invenio_base.secret_key = 
 	invenio_oauth2server = invenio_oauth2server.utils:rebuild_access_tokens
+invenio_base.finalize_app = 
+	invenio_oauth2server = invenio_oauth2server.ext:finalize_app
 
 [build_sphinx]
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
 
 [bdist_wheel]
```

### Comparing `invenio-oauth2server-2.2.1/tests/conftest.py` & `invenio-oauth2server-2.3.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2015-2018 CERN.
+# Copyright (C) 2024 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 
 """Pytest configuration."""
 
@@ -16,21 +17,22 @@
 import tempfile
 from unittest.mock import MagicMock
 
 import pytest
 from flask import Flask, url_for
 from flask.cli import ScriptInfo
 from flask.views import MethodView
-from flask_breadcrumbs import Breadcrumbs
 from flask_mail import Mail
 from flask_menu import Menu
 from helpers import create_oauth_client, patch_request
 from invenio_accounts import InvenioAccountsREST, InvenioAccountsUI
 from invenio_accounts.models import User
-from invenio_accounts.views import blueprint as accounts_blueprint
+from invenio_accounts.views.settings import (
+    create_settings_blueprint as create_accounts_blueprint,
+)
 from invenio_db import InvenioDB, db
 from invenio_i18n import InvenioI18N
 from six import get_method_self
 from sqlalchemy_utils.functions import create_database, database_exists, drop_database
 
 from invenio_oauth2server import InvenioOAuth2Server, InvenioOAuth2ServerREST
 from invenio_oauth2server.decorators import require_api_auth, require_oauth_scopes
@@ -85,28 +87,28 @@
             },
             ACCOUNTS_COVER_TEMPLATE="invenio_accounts/base_cover.html",
             ACCOUNTS_BASE_TEMPLATE="invenio_accounts/base.html",
         )
         InvenioI18N(app)
         Mail(app)
         Menu(app)
-        Breadcrumbs(app)
         InvenioDB(app)
         InvenioOAuth2Server(app)
+        InvenioI18N(app)
 
     api_app = Flask("testapiapp", instance_path=instance_path)
     api_app.config.update(APPLICATION_ROOT="/api", ACCOUNTS_REGISTER_BLUEPRINT=True)
     init_app(api_app)
     InvenioAccountsREST(api_app)
     InvenioOAuth2ServerREST(api_app)
 
     app = Flask("testapp", instance_path=instance_path)
     init_app(app)
     InvenioAccountsUI(app)
-    app.register_blueprint(accounts_blueprint)
+    app.register_blueprint(create_accounts_blueprint(app))
     app.register_blueprint(server_blueprint)
     app.register_blueprint(settings_blueprint)
 
     app.wsgi_app = DispatcherMiddleware(app.wsgi_app, {"/api": api_app.wsgi_app})
 
     with app.app_context():
         if str(db.engine.url) != "sqlite://" and not database_exists(
```

### Comparing `invenio-oauth2server-2.2.1/tests/helpers.py` & `invenio-oauth2server-2.3.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/tests/test_admin.py` & `invenio-oauth2server-2.3.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/tests/test_alembic.py` & `invenio-oauth2server-2.3.0/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/tests/test_cli.py` & `invenio-oauth2server-2.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/tests/test_decorators.py` & `invenio-oauth2server-2.3.0/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/tests/test_invenio_oauth2server.py` & `invenio-oauth2server-2.3.0/tests/test_invenio_oauth2server.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/tests/test_models.py` & `invenio-oauth2server-2.3.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/tests/test_provider.py` & `invenio-oauth2server-2.3.0/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/tests/test_server.py` & `invenio-oauth2server-2.3.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/tests/test_settings.py` & `invenio-oauth2server-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/tests/test_utils.py` & `invenio-oauth2server-2.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.2.1/tests/test_validators.py` & `invenio-oauth2server-2.3.0/tests/test_validators.py`

 * *Files identical despite different names*

