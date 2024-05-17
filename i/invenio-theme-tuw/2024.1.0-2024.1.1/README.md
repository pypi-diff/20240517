# Comparing `tmp/invenio-theme-tuw-2024.1.0.tar.gz` & `tmp/invenio-theme-tuw-2024.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-theme-tuw-2024.1.0.tar", last modified: Fri Mar  1 22:59:53 2024, max compression
+gzip compressed data, was "invenio-theme-tuw-2024.1.1.tar", last modified: Thu Mar 14 10:40:13 2024, max compression
```

## Comparing `invenio-theme-tuw-2024.1.0.tar` & `invenio-theme-tuw-2024.1.1.tar`

### file list

```diff
@@ -1,265 +1,264 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.960035 invenio-theme-tuw-2024.1.0/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.0/.dockerignore
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      617 2022-11-23 16:27:37.000000 invenio-theme-tuw-2024.1.0/.editorconfig
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2022-11-23 16:27:37.000000 invenio-theme-tuw-2024.1.0/.git-blame-ignore-revs
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.936034 invenio-theme-tuw-2024.1.0/.tx/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1042 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.0/.tx/config
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      287 2021-07-15 12:29:34.000000 invenio-theme-tuw-2024.1.0/AUTHORS.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7081 2024-03-01 12:06:40.000000 invenio-theme-tuw-2024.1.0/CHANGES.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3370 2021-07-15 12:29:34.000000 invenio-theme-tuw-2024.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      202 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.0/INSTALL.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.0/LICENSE
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1746 2024-02-29 16:56:49.000000 invenio-theme-tuw-2024.1.0/MANIFEST.in
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     9356 2024-03-01 22:59:53.960035 invenio-theme-tuw-2024.1.0/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      380 2024-02-29 16:56:49.000000 invenio-theme-tuw-2024.1.0/Pipfile
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1040 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.0/README.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      535 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.0/babel.ini
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.940034 invenio-theme-tuw-2024.1.0/docs/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7453 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.0/docs/Makefile
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      233 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.0/docs/authors.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      233 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.0/docs/changes.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10182 2024-02-29 16:56:49.000000 invenio-theme-tuw-2024.1.0/docs/conf.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      238 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.0/docs/contributing.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      441 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.0/docs/index.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.0/docs/license.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7003 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.0/docs/make.bat
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.0/docs/requirements.txt
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.940034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      372 2024-03-01 12:06:40.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/__init__.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.940034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/build_project/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       78 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/build_project/.babelrc
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       11 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/build_project/.eslintignore
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      849 2023-04-24 15:50:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/build_project/.eslintrc.js
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.940034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/build_project/build/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7181 2023-04-24 15:50:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/build_project/build/webpack.config.js
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2385 2023-08-25 12:49:04.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/build_project/package.json
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.940034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/build_project/patches/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      560 2023-04-24 15:50:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/build_project/patches/watchpack+1.7.5.patch
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4376 2023-12-13 15:21:45.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2617 2023-08-25 08:52:24.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/ext.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      763 2022-10-17 09:59:49.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/search.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.936034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.932034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.932034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.932034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/js/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.932034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.940034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      576 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/index.js
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.940034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/snowfall/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      517 2023-12-13 15:21:45.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/snowfall/index.js
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.940034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      966 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/index.js
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.932034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.940034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.940034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.944034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      213 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/breadcrumb.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       70 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/breadcrumb.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      984 2022-09-07 12:08:20.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/grid.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/grid.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7166 2023-09-11 19:50:33.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1040 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       69 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/message.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      210 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/message.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/table.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/table.variables
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.944034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      479 2022-09-08 10:53:10.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/contact.less
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      665 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/file-list.less
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1312 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/flip-card.less
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3045 2022-11-25 16:08:24.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/fonts.less
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.944034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      503 2022-09-02 11:49:31.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      725 2022-09-02 11:49:31.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      599 2022-09-02 13:37:47.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       68 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/divider.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/divider.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/flag.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/flag.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/header.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/header.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      331 2022-10-27 14:52:31.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/icon.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/icon.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/image.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/image.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/input.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/input.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/label.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/label.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/list.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/list.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/loader.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/loader.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/rail.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/rail.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/reveal.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/reveal.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/segment.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/segment.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/step.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/step.variables
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.948034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   287936 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Bold.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   209784 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-BoldItalic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   270524 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Italic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   278168 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Regular.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168060 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Black.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   174108 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BlackItalic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   167336 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Bold.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   171508 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BoldItalic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   170504 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Italic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   167000 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Light.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   173172 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-LightItalic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168644 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Medium.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   173416 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-MediumItalic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168260 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Regular.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168488 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Thin.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   172860 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-ThinItalic.ttf
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.952035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      291 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/reset.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/reset.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4302 2023-04-24 11:32:11.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1150 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.variables
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.952035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    36366 2022-10-10 09:44:16.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-background.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    22946 2022-10-10 09:44:16.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-contact.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    43552 2022-10-10 09:44:16.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-policies.webp
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.952035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/accordion.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/accordion.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/chatroom.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/chatroom.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2569 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dimmer.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dimmer.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      154 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dropdown.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      161 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dropdown.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/embed.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/embed.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/modal.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/modal.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       59 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/nag.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       59 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/nag.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/popup.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/popup.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/progress.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/progress.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/rating.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/rating.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/search.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/search.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/shape.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/shape.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      369 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sidebar.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      338 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sidebar.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sticky.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sticky.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/tab.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/tab.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/transition.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/transition.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2326 2023-05-03 16:49:56.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/theme.less
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.956035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       56 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/ad.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       56 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/ad.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/card.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/card.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/comment.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/comment.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/feed.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/feed.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       60 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/item.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/item.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/statistic.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/statistic.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2022-09-05 14:21:18.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/tuwstone.less
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.936034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.956035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      794 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/favicon-16x16.png
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1101 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/favicon-32x32.png
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.956035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/features/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    12850 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/features/faq.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    27714 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/features/magnifying-glass.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    13548 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/features/online-chat.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    21722 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/features/upload-file.webp
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.956035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/footer-logos/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   201844 2023-09-11 19:50:33.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/footer-logos/fairsharing-logo.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    29306 2023-09-11 19:50:33.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/footer-logos/inveniordm-logo.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4636 2022-11-30 11:55:52.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.png
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2512 2022-11-30 11:55:52.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     9811 2022-11-30 11:55:52.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.png
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3926 2022-11-30 11:55:52.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    13674 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/pdf.webp
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.956035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    19926 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/analytics.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    36394 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/connection.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8098 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/git.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    37302 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/group.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    34924 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/online-community.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    22964 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/team.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    29404 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/user.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    31176 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/version.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10686 2023-10-04 10:01:08.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/tu-wien-logo-hd.png
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2626 2023-10-04 10:01:08.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/tu-wien-logo.png
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.956035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/tuwstones/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    70038 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/tuwstones/fwoerister.png
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.936034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.936034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.936034 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.960035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16065 2023-04-24 14:08:12.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/detail.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      955 2023-04-24 14:08:12.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/search.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.960035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1719 2022-10-03 16:21:50.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      679 2023-08-30 13:44:57.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_mail_html.jinja
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      591 2023-08-25 12:49:04.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_mail_text.jinja
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3294 2023-08-25 08:52:24.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_uploader.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.960035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7653 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/details.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2836 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/side_bar.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      981 2023-08-30 13:44:57.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/uploaders.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.960035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1710 2023-02-20 18:21:08.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/community.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1649 2023-04-05 13:35:38.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/deposit.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.960035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      974 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/detail.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.960035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2458 2023-09-11 19:50:33.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/footer.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8340 2023-10-18 13:58:40.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/frontpage.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5012 2023-02-20 18:21:08.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/header.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      657 2023-12-13 15:21:45.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/javascript.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1501 2023-04-24 14:08:12.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/login_user.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8550 2023-04-24 14:08:12.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      758 2023-04-24 14:08:12.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page_error.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2101 2023-04-24 14:08:12.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/signup.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2676 2023-02-20 18:21:08.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/policies.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      668 2022-10-03 16:21:50.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/search_bar.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.960035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/settings/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2045 2023-12-22 13:32:07.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/settings/curation.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1463 2022-11-30 11:55:52.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/terms_of_use.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.960035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1278 2022-09-05 14:21:18.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/florian_woerister.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11739 2024-02-29 16:56:49.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/views.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3246 2023-12-13 15:21:45.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw/webpack.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.960035 invenio-theme-tuw-2024.1.0/invenio_theme_tuw.egg-info/
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     9356 2024-03-01 22:59:53.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16509 2024-03-01 22:59:53.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-03-01 22:59:53.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      228 2024-03-01 22:59:53.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-03-01 22:59:47.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw.egg-info/not-zip-safe
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      174 2024-03-01 22:59:53.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       18 2024-03-01 22:59:53.000000 invenio-theme-tuw-2024.1.0/invenio_theme_tuw.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2022-11-23 16:27:37.000000 invenio-theme-tuw-2024.1.0/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      491 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.0/requirements-devel.txt
--rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      712 2024-02-29 16:56:49.000000 invenio-theme-tuw-2024.1.0/run-tests.sh
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2399 2024-03-01 22:59:53.964035 invenio-theme-tuw-2024.1.0/setup.cfg
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      294 2022-11-23 16:27:37.000000 invenio-theme-tuw-2024.1.0/setup.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-01 22:59:53.960035 invenio-theme-tuw-2024.1.0/tests/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8379 2024-02-29 16:56:49.000000 invenio-theme-tuw-2024.1.0/tests/conftest.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3849 2024-02-29 17:31:49.000000 invenio-theme-tuw-2024.1.0/tests/test_functions.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1935 2024-02-29 16:56:49.000000 invenio-theme-tuw-2024.1.0/tests/test_invenio_theme_tuw.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1263 2024-02-29 16:56:49.000000 invenio-theme-tuw-2024.1.0/tests/test_routes.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.904856 invenio-theme-tuw-2024.1.1/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.1/.dockerignore
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      617 2022-11-23 16:27:37.000000 invenio-theme-tuw-2024.1.1/.editorconfig
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2022-11-23 16:27:37.000000 invenio-theme-tuw-2024.1.1/.git-blame-ignore-revs
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.880855 invenio-theme-tuw-2024.1.1/.tx/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1042 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.1/.tx/config
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      287 2021-07-15 12:29:34.000000 invenio-theme-tuw-2024.1.1/AUTHORS.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7069 2024-03-14 10:35:07.000000 invenio-theme-tuw-2024.1.1/CHANGES.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3370 2021-07-15 12:29:34.000000 invenio-theme-tuw-2024.1.1/CONTRIBUTING.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      202 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.1/INSTALL.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.1/LICENSE
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1746 2024-03-14 10:32:25.000000 invenio-theme-tuw-2024.1.1/MANIFEST.in
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     9383 2024-03-14 10:40:13.904856 invenio-theme-tuw-2024.1.1/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1040 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.1/README.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      535 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.1/babel.ini
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.880855 invenio-theme-tuw-2024.1.1/docs/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7453 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.1/docs/Makefile
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      233 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.1/docs/authors.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      233 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.1/docs/changes.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10182 2024-02-29 16:56:49.000000 invenio-theme-tuw-2024.1.1/docs/conf.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      238 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.1/docs/contributing.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      441 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.1/docs/index.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.1/docs/license.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7003 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.1/docs/make.bat
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.1/docs/requirements.txt
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.880855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      372 2024-03-14 10:35:07.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/__init__.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.884855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/build_project/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       78 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/build_project/.babelrc
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       11 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/build_project/.eslintignore
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      849 2023-04-24 15:50:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/build_project/.eslintrc.js
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.884855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/build_project/build/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7181 2023-04-24 15:50:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/build_project/build/webpack.config.js
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2385 2023-08-25 12:49:04.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/build_project/package.json
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.884855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/build_project/patches/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      560 2023-04-24 15:50:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/build_project/patches/watchpack+1.7.5.patch
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4376 2023-12-13 15:21:45.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2617 2023-08-25 08:52:24.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/ext.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      763 2022-10-17 09:59:49.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/search.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.876855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.876855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.876855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.876855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/js/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.876855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.884855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      576 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/index.js
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.884855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/snowfall/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      517 2023-12-13 15:21:45.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/snowfall/index.js
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.884855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      966 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/index.js
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.876855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.884855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.884855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.884855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      213 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/breadcrumb.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       70 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/breadcrumb.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      984 2022-09-07 12:08:20.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/grid.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/grid.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7166 2023-09-11 19:50:33.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1040 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       69 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/message.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      210 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/message.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/table.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/table.variables
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.884855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      479 2022-09-08 10:53:10.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/contact.less
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      665 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/file-list.less
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1312 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/flip-card.less
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3045 2022-11-25 16:08:24.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/fonts.less
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.888855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      503 2022-09-02 11:49:31.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      725 2022-09-02 11:49:31.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      599 2022-09-02 13:37:47.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       68 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/divider.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/divider.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/flag.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/flag.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/header.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/header.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      331 2022-10-27 14:52:31.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/icon.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/icon.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/image.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/image.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/input.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/input.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/label.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/label.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/list.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/list.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/loader.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/loader.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/rail.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/rail.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/reveal.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/reveal.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/segment.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/segment.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/step.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/step.variables
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.892855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   287936 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Bold.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   209784 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-BoldItalic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   270524 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Italic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   278168 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Regular.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168060 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Black.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   174108 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BlackItalic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   167336 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Bold.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   171508 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BoldItalic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   170504 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Italic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   167000 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Light.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   173172 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-LightItalic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168644 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Medium.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   173416 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-MediumItalic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168260 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Regular.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168488 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Thin.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   172860 2022-09-19 15:50:46.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-ThinItalic.ttf
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.892855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      291 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/reset.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/reset.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4302 2023-04-24 11:32:11.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1150 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.variables
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.892855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    36366 2022-10-10 09:44:16.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-background.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    22946 2022-10-10 09:44:16.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-contact.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    43552 2022-10-10 09:44:16.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-policies.webp
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.896855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/accordion.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/accordion.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/chatroom.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/chatroom.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2569 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dimmer.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dimmer.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      154 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dropdown.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      161 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dropdown.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/embed.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/embed.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/modal.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/modal.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       59 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/nag.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       59 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/nag.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/popup.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/popup.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/progress.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/progress.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/rating.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/rating.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/search.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/search.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/shape.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/shape.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      369 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sidebar.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      338 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sidebar.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sticky.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sticky.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/tab.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/tab.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/transition.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/transition.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2326 2023-05-03 16:49:56.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/theme.less
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.896855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       56 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/ad.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       56 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/ad.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/card.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/card.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/comment.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/comment.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/feed.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/feed.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       60 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/item.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/item.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/statistic.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/statistic.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2022-09-05 14:21:18.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/tuwstone.less
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.876855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.896855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      794 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/favicon-16x16.png
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1101 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/favicon-32x32.png
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.900855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/features/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    12850 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/features/faq.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    27714 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/features/magnifying-glass.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    13548 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/features/online-chat.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    21722 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/features/upload-file.webp
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.900855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/footer-logos/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   201844 2023-09-11 19:50:33.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/footer-logos/fairsharing-logo.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    29306 2023-09-11 19:50:33.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/footer-logos/inveniordm-logo.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4636 2022-11-30 11:55:52.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.png
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2512 2022-11-30 11:55:52.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     9811 2022-11-30 11:55:52.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.png
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3926 2022-11-30 11:55:52.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    13674 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/pdf.webp
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.900855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    19926 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/analytics.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    36394 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/connection.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8098 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/git.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    37302 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/group.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    34924 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/online-community.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    22964 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/team.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    29404 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/user.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    31176 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/version.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10686 2023-10-04 10:01:08.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/tu-wien-logo-hd.png
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2626 2023-10-04 10:01:08.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/tu-wien-logo.png
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.900855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/tuwstones/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    70038 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/tuwstones/fwoerister.png
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.876855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.876855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.876855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.900855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16065 2023-04-24 14:08:12.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/detail.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      955 2023-04-24 14:08:12.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/search.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.900855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1719 2022-10-03 16:21:50.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      679 2023-08-30 13:44:57.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_mail_html.jinja
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      591 2023-08-25 12:49:04.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_mail_text.jinja
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3294 2023-08-25 08:52:24.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_uploader.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.900855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7653 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/details.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2836 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/side_bar.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      981 2023-08-30 13:44:57.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/uploaders.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.900855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1710 2023-02-20 18:21:08.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/community.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1649 2023-04-05 13:35:38.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/deposit.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.900855 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      974 2022-07-14 09:43:44.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/detail.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.904856 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2458 2023-09-11 19:50:33.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/footer.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8340 2023-10-18 13:58:40.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/frontpage.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5012 2023-02-20 18:21:08.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/header.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      657 2023-12-13 15:21:45.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/javascript.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1501 2023-04-24 14:08:12.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/login_user.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8550 2023-04-24 14:08:12.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      758 2023-04-24 14:08:12.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page_error.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2101 2023-04-24 14:08:12.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/signup.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2676 2023-02-20 18:21:08.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/policies.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      668 2022-10-03 16:21:50.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/search_bar.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.904856 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/settings/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2045 2023-12-22 13:32:07.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/settings/curation.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1463 2022-11-30 11:55:52.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/terms_of_use.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.904856 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1278 2022-09-05 14:21:18.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/florian_woerister.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11739 2024-02-29 16:56:49.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/views.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3246 2023-12-13 15:21:45.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw/webpack.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.904856 invenio-theme-tuw-2024.1.1/invenio_theme_tuw.egg-info/
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     9383 2024-03-14 10:40:13.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16501 2024-03-14 10:40:13.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-03-14 10:40:13.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      228 2024-03-14 10:40:13.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-03-14 10:40:07.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw.egg-info/not-zip-safe
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      215 2024-03-14 10:40:13.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       18 2024-03-14 10:40:13.000000 invenio-theme-tuw-2024.1.1/invenio_theme_tuw.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2022-11-23 16:27:37.000000 invenio-theme-tuw-2024.1.1/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      491 2021-07-05 13:11:26.000000 invenio-theme-tuw-2024.1.1/requirements-devel.txt
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      712 2024-02-29 16:56:49.000000 invenio-theme-tuw-2024.1.1/run-tests.sh
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2403 2024-03-14 10:40:13.904856 invenio-theme-tuw-2024.1.1/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      294 2022-11-23 16:27:37.000000 invenio-theme-tuw-2024.1.1/setup.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-14 10:40:13.904856 invenio-theme-tuw-2024.1.1/tests/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8379 2024-02-29 16:56:49.000000 invenio-theme-tuw-2024.1.1/tests/conftest.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3849 2024-02-29 17:31:49.000000 invenio-theme-tuw-2024.1.1/tests/test_functions.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1935 2024-02-29 16:56:49.000000 invenio-theme-tuw-2024.1.1/tests/test_invenio_theme_tuw.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1263 2024-02-29 16:56:49.000000 invenio-theme-tuw-2024.1.1/tests/test_routes.py
```

### Comparing `invenio-theme-tuw-2024.1.0/.editorconfig` & `invenio-theme-tuw-2024.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/.tx/config` & `invenio-theme-tuw-2024.1.1/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/CHANGES.rst` & `invenio-theme-tuw-2024.1.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,16 @@
     Invenio-Theme-TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2024.1 (released 2024-03-01)
+Version 2024.1 (released 2024-03-01, updated 2024-03-14)
 
-- Add Pipfile to source control
 - Views: add status code in guards' response
 - Add automated tests
 
 
 Version 2023.2 (released 2023-04-24, updated 2023-12-22)
 
 - v11 compat: Update templates and frontend build project
```

### Comparing `invenio-theme-tuw-2024.1.0/CONTRIBUTING.rst` & `invenio-theme-tuw-2024.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/LICENSE` & `invenio-theme-tuw-2024.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/MANIFEST.in` & `invenio-theme-tuw-2024.1.1/MANIFEST.in`

 * *Files 7% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 #  git add -A
 #  pip install -e .[all]
 #  check-manifest -u
 
 # exclude CI/CD stuff
 exclude sonar-project.properties
 exclude .gitlab-ci.yml
+exclude Pipfile
 
 include .git-blame-ignore-revs
 include .dockerignore
 include .editorconfig
 include .tx/config
 prune docs/_build
 recursive-include .github/workflows *.yml
 recursive-include invenio_theme_tuw/translations *.po *.pot *.mo
 
 # added by check-manifest
 include *.rst
 include *.sh
 include *.txt
-include Pipfile
 include LICENSE
 include babel.ini
 include pytest.ini
 recursive-include docs *.bat
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs *.txt
```

### Comparing `invenio-theme-tuw-2024.1.0/PKG-INFO` & `invenio-theme-tuw-2024.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: invenio-theme-tuw
-Version: 2024.1.0
+Version: 2024.1.1
 Summary: "TU Wien theme for Invenio (RDM)."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-theme-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio theme tuw
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: Flask-WebpackExt>=1.0.0
 Requires-Dist: Invenio-App-RDM>=11.0.0
+Requires-Dist: Invenio-Search>=2.0.0
 Requires-Dist: Flask<2.3,>=2.0.2
-Requires-Dist: Flask-Session-Captcha>=1.3.0
+Requires-Dist: Flask-Session-Captcha<1.4,>=1.3.0
 Provides-Extra: tests
-Requires-Dist: pytest-black<0.3.10,>=0.3.0; extra == "tests"
+Requires-Dist: pytest-black>=0.3.0; extra == "tests"
 Requires-Dist: pytest-invenio>=1.4.0; extra == "tests"
 Requires-Dist: sphinx>=4.5; extra == "tests"
+Requires-Dist: opensearch-dsl>=2.1.0; extra == "tests"
 Provides-Extra: docs
 
 ..
     Copyright (C) 2020 - 2021 TU Wien.
 
     Invenio-Theme-TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
@@ -73,17 +74,16 @@
     Invenio-Theme-TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2024.1 (released 2024-03-01)
+Version 2024.1 (released 2024-03-01, updated 2024-03-14)
 
-- Add Pipfile to source control
 - Views: add status code in guards' response
 - Add automated tests
 
 
 Version 2023.2 (released 2023-04-24, updated 2023-12-22)
 
 - v11 compat: Update templates and frontend build project
```

### Comparing `invenio-theme-tuw-2024.1.0/README.rst` & `invenio-theme-tuw-2024.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/babel.ini` & `invenio-theme-tuw-2024.1.1/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/docs/Makefile` & `invenio-theme-tuw-2024.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/docs/conf.py` & `invenio-theme-tuw-2024.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/docs/make.bat` & `invenio-theme-tuw-2024.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/build_project/.eslintrc.js` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/build_project/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/build_project/build/webpack.config.js` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/build_project/build/webpack.config.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/build_project/package.json` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/build_project/package.json`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/build_project/patches/watchpack+1.7.5.patch` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/build_project/patches/watchpack+1.7.5.patch`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/config.py` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/config.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/ext.py` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/search.py` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/search.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/index.js` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/index.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/snowfall/index.js` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/snowfall/index.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/index.js` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/index.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.overrides` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.overrides` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.variables` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.variables`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/file-list.less` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/file-list.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/flip-card.less` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/flip-card.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/fonts.less` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/fonts.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.variables` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.variables`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.overrides` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Bold.ttf` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-BoldItalic.ttf` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Italic.ttf` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Regular.ttf` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Black.ttf` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BlackItalic.ttf` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Bold.ttf` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BoldItalic.ttf` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Italic.ttf` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Light.ttf` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-LightItalic.ttf` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Medium.ttf` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-MediumItalic.ttf` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Regular.ttf` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Thin.ttf` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-ThinItalic.ttf` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.overrides` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.variables` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.variables`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-background.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-background.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-contact.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-contact.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-policies.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-policies.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.overrides` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/theme.less` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/theme.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/tuwstone.less` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/tuwstone.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/favicon-16x16.png` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/favicon-32x32.png` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/features/faq.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/features/faq.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/features/magnifying-glass.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/features/magnifying-glass.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/features/online-chat.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/features/online-chat.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/features/upload-file.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/features/upload-file.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/footer-logos/fairsharing-logo.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/footer-logos/fairsharing-logo.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/footer-logos/inveniordm-logo.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/footer-logos/inveniordm-logo.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.png` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.png` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/pdf.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/pdf.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/analytics.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/analytics.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/connection.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/connection.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/git.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/git.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/group.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/group.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/online-community.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/online-community.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/team.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/team.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/user.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/user.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/planned-features/version.webp` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/planned-features/version.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/tu-wien-logo-hd.png` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/tu-wien-logo-hd.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/tu-wien-logo.png` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/tu-wien-logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/static/images/tuwstones/fwoerister.png` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/static/images/tuwstones/fwoerister.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/detail.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/detail.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/search.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/search.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_mail_html.jinja` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_mail_html.jinja`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_mail_text.jinja` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_mail_text.jinja`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_uploader.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact_uploader.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/details.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/details.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/side_bar.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/side_bar.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/uploaders.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/uploaders.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/community.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/community.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/deposit.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/deposit.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/detail.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/detail.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/footer.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/footer.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/frontpage.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/frontpage.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/header.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/javascript.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/javascript.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/login_user.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page_error.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page_error.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/signup.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/signup.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/policies.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/policies.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/search_bar.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/search_bar.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/settings/curation.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/settings/curation.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/terms_of_use.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/terms_of_use.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/florian_woerister.html` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/florian_woerister.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/views.py` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/views.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw/webpack.py` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw.egg-info/PKG-INFO` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: invenio-theme-tuw
-Version: 2024.1.0
+Version: 2024.1.1
 Summary: "TU Wien theme for Invenio (RDM)."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-theme-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio theme tuw
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: Flask-WebpackExt>=1.0.0
 Requires-Dist: Invenio-App-RDM>=11.0.0
+Requires-Dist: Invenio-Search>=2.0.0
 Requires-Dist: Flask<2.3,>=2.0.2
-Requires-Dist: Flask-Session-Captcha>=1.3.0
+Requires-Dist: Flask-Session-Captcha<1.4,>=1.3.0
 Provides-Extra: tests
-Requires-Dist: pytest-black<0.3.10,>=0.3.0; extra == "tests"
+Requires-Dist: pytest-black>=0.3.0; extra == "tests"
 Requires-Dist: pytest-invenio>=1.4.0; extra == "tests"
 Requires-Dist: sphinx>=4.5; extra == "tests"
+Requires-Dist: opensearch-dsl>=2.1.0; extra == "tests"
 Provides-Extra: docs
 
 ..
     Copyright (C) 2020 - 2021 TU Wien.
 
     Invenio-Theme-TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
@@ -73,17 +74,16 @@
     Invenio-Theme-TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2024.1 (released 2024-03-01)
+Version 2024.1 (released 2024-03-01, updated 2024-03-14)
 
-- Add Pipfile to source control
 - Views: add status code in guards' response
 - Add automated tests
 
 
 Version 2023.2 (released 2023-04-24, updated 2023-12-22)
 
 - v11 compat: Update templates and frontend build project
```

### Comparing `invenio-theme-tuw-2024.1.0/invenio_theme_tuw.egg-info/SOURCES.txt` & `invenio-theme-tuw-2024.1.1/invenio_theme_tuw.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 .git-blame-ignore-revs
 AUTHORS.rst
 CHANGES.rst
 CONTRIBUTING.rst
 INSTALL.rst
 LICENSE
 MANIFEST.in
-Pipfile
 README.rst
 babel.ini
 pyproject.toml
 requirements-devel.txt
 run-tests.sh
 setup.cfg
 setup.py
```

### Comparing `invenio-theme-tuw-2024.1.0/run-tests.sh` & `invenio-theme-tuw-2024.1.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/setup.cfg` & `invenio-theme-tuw-2024.1.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -12,35 +12,36 @@
 classifiers = 
 	Environment :: Web Environment
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 	Topic :: Software Development :: Libraries :: Python Modules
 	Programming Language :: Python
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Development Status :: 5 - Production/Stable
 
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.7
 zip_safe = False
 install_requires = 
 	Flask-WebpackExt>=1.0.0
 	Invenio-App-RDM>=11.0.0
+	Invenio-Search>=2.0.0
 	Flask>=2.0.2,<2.3
-	Flask-Session-Captcha>=1.3.0
+	Flask-Session-Captcha>=1.3.0,<1.4
 
 [options.extras_require]
 tests = 
-	pytest-black>=0.3.0,<0.3.10
+	pytest-black>=0.3.0
 	pytest-invenio>=1.4.0
 	sphinx>=4.5
+	opensearch-dsl>=2.1.0
 docs = 
 
 [options.entry_points]
 invenio_base.apps = 
 	invenio_theme_tuw = invenio_theme_tuw:InvenioThemeTUW
 invenio_assets.webpack = 
 	invenio_theme_tuw_theme = invenio_theme_tuw.webpack:theme
```

### Comparing `invenio-theme-tuw-2024.1.0/tests/conftest.py` & `invenio-theme-tuw-2024.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/tests/test_functions.py` & `invenio-theme-tuw-2024.1.1/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/tests/test_invenio_theme_tuw.py` & `invenio-theme-tuw-2024.1.1/tests/test_invenio_theme_tuw.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2024.1.0/tests/test_routes.py` & `invenio-theme-tuw-2024.1.1/tests/test_routes.py`

 * *Files identical despite different names*

